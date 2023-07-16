# Comparing `tmp/kuro2sudachi-0.4.0.tar.gz` & `tmp/kuro2sudachi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuro2sudachi-0.4.0.tar", max compression
+gzip compressed data, was "kuro2sudachi-0.4.2.tar", max compression
```

## Comparing `kuro2sudachi-0.4.0.tar` & `kuro2sudachi-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2851 2023-07-08 16:34:19.105217 kuro2sudachi-0.4.0/README.md
--rw-r--r--   0        0        0      694 2023-07-08 16:34:19.115112 kuro2sudachi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.4.0/src/kuro2sudachi/__init__.py
--rw-r--r--   0        0        0     7051 2023-07-08 16:34:19.117661 kuro2sudachi-0.4.0/src/kuro2sudachi/core.py
--rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.4.0/src/kuro2sudachi/normalizer.py
--rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.4.0/src/kuro2sudachi/rewrite.def
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 kuro2sudachi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2851 2023-07-09 08:48:36.492983 kuro2sudachi-0.4.2/README.md
+-rw-r--r--   0        0        0      694 2023-07-16 09:51:02.008145 kuro2sudachi-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.4.2/src/kuro2sudachi/__init__.py
+-rw-r--r--   0        0        0     7538 2023-07-16 09:44:37.059658 kuro2sudachi-0.4.2/src/kuro2sudachi/core.py
+-rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.4.2/src/kuro2sudachi/normalizer.py
+-rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.4.2/src/kuro2sudachi/rewrite.def
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 kuro2sudachi-0.4.2/PKG-INFO
```

### Comparing `kuro2sudachi-0.4.0/README.md` & `kuro2sudachi-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.0/pyproject.toml` & `kuro2sudachi-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuro2sudachi"
-version = "0.4.0"
+version = "0.4.2"
 description = ""
 authors = ["po3rin"]
 repository = "http://github.com/po3rin/kuro2sudachi"
 homepage = "http://github.com/po3rin/kuro2sudachi"
 readme = "README.md"
 license = "Apache-2.0"
 include = ["rewrite.def"]
```

### Comparing `kuro2sudachi-0.4.0/src/kuro2sudachi/core.py` & `kuro2sudachi-0.4.2/src/kuro2sudachi/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import fileinput
 import json
 import os
 import re
 from dataclasses import dataclass
 
 import jaconv
-from sudachipy import dictionary, tokenizer
+from sudachipy import dictionary, SplitMode
 
 from kuro2sudachi.normalizer import SudachiCharNormalizer
 
-mode = tokenizer.Tokenizer.SplitMode.C
+
+MAX_WORD_ID = 2912274
 
 parser = argparse.ArgumentParser(
     description="convert kuromoji user dict to sudacchi user dict"
 )
 parser.add_argument("file", help="kuromoji dict file path")
 parser.add_argument(
     "-c",
@@ -89,111 +90,116 @@
 
 class Converter:
     def __init__(
         self,
         rewrite_file,
         config=None,
         sudachi_setting=None,
-        dict_type="core",
+        sudachi_dict="core",
         rm=False,
         unit_words_dict: dict[str, UnitWord] = {},
-    ):
+    ) -> None:
         if rewrite_file == "":
             raise DictFormatError("rewrite.def file path is required")
 
-        self.tokenizer = dictionary.Dictionary(
-            config_path=sudachi_setting, dict=dict_type
-        ).create()
+        dic = dictionary.Dictionary(
+            config_path=sudachi_setting,
+            dict=sudachi_dict
+        )
+        self.tokenizer = dic.create()
 
         if config is not None:
             with open(config) as f:
                 s = json.load(f)
         else:
             s = default_setting
 
         self.rewrite = rewrite_file
         self.setting = s
         self.rm = rm
         self.normalizer = SudachiCharNormalizer(rewrite_def_path=self.rewrite)
         self.unit_words_dict = unit_words_dict
+        self.dic = dic
 
     def convert(self, line: str) -> str:
         data = line.split(",")
         try:
             word = data[0]
-            # splited = data[1]
             yomi = self.nomlized_yomi(data[2].replace(" ", ""))
             pos = self.pos_convert(data[3].replace(" ", ""))
         except IndexError:
             raise DictFormatError(f"'{line}' is invalid format")
 
-        words = [m.surface() for m in self.tokenizer.tokenize(word, mode)]
-
-        # alrady exists in system dic
+        words = [m.surface() for m in self.tokenizer.tokenize(text=word, mode=SplitMode.C)]
         if self.rm and len(words) == 1:
+            # alrady exists in system dic (mode C)
             return ""
 
-        normalized = self.normalizer.rewrite(word)
-        unit_div_info = "*,*"
-
-        try:
-            if (udm := pos.get("unit_div_mode")) != None:
-                unit_div_info = self.split(normalized, udm)
-        except OOVError as e:
-            print(e)
-            raise e
+        normalized_word = self.normalizer.rewrite(text=word)
+        
+        if (unit_div_mode := pos.get("unit_div_mode")) != None:
+            unit_div_info = self.split(word=normalized_word, unit_div_mode=unit_div_mode)
+        else:
+            unit_div_info = "*,*"
 
         split_mode = pos.get("split_mode", "*")
-        return f"{normalized},{pos['left_id']},{pos['right_id']},{pos['cost']},{word},{pos['sudachi_pos']},{yomi},{word},*,{split_mode},{unit_div_info},*"
+        return f"{normalized_word},{pos['left_id']},{pos['right_id']},{pos['cost']},{word},{pos['sudachi_pos']},{yomi},{word},*,{split_mode},{unit_div_info},*"
 
-    def pos_convert(self, pos: str):
+    def pos_convert(self, pos: str) -> dict[str, any]:
         try:
             spos = self.setting[pos]
             return spos
         except KeyError:
             raise UnSupportedPosError(f"{pos} is not supported pos")
 
     def nomlized_yomi(self, yomi: str) -> str:
-        yomi = jaconv.hira2kata(yomi)
-        if p.fullmatch(yomi):
+        yomi = jaconv.hira2kata(text=yomi)
+        if p.fullmatch(string=yomi):
             return yomi
         return ""
 
-    def split_info(self, normalized: str, udm: list[str], mode: any) -> str:
+    def split_info(self, word: str, mode: SplitMode) -> str:
         word_ids = []
         oov = []
-        for m in self.tokenizer.tokenize(normalized, mode):
+        ms = self.tokenizer.tokenize(text=word, mode=mode)
+        for m in ms:
             if ",".join(m.part_of_speech()) == "名詞,数詞,*,*,*,*":
                 return "*"
 
             if m.is_oov() or m.dictionary_id() == -1:
                 oov.append(m.surface())
                 continue
 
+            if m.word_id() >= MAX_WORD_ID:
+                # If word_mask and word_id match, there is a possibility that the word was generated by the rewrite plugin.
+                # In that case word_id is not defined, so you get an error when building the dictionary.
+                # Therefore, look up the word again in the dictionary and obtain the word_id(TODO).
+                return "*"
+
             if str(m) in self.unit_words_dict:
                 word_ids.append(f"U{str(self.unit_words_dict[str(m)].word_id)}")
             else:
                 word_ids.append(str(m.word_id()))
 
         if len(oov) > 0:
-            raise OOVError(f"split word has out of vocab: {oov} in {normalized}")
+            raise OOVError(f"split word has out of vocab: {oov} in {word}")
 
         return "/".join(word_ids)
 
-    def split(self, normalized: str, udm: list[str]) -> str:
+    def split(self, word: str, unit_div_mode: list[str]) -> str:
         try:
-            unit_div_info = []
-            if "A" in udm:
-                info = self.split_info(normalized, udm, tokenizer.Tokenizer.SplitMode.A)
+            unit_div_info: list[str] = []
+            if "A" in unit_div_mode:
+                info = self.split_info(word=word, mode=SplitMode.A)
                 unit_div_info.append(info)
             else:
                 unit_div_info.append("*")
 
-            if "B" in udm:
-                info = self.split_info(normalized, udm, tokenizer.Tokenizer.SplitMode.B)
+            if "B" in unit_div_mode:
+                info = self.split_info(word=word, mode=SplitMode.B)
                 unit_div_info.append(info)
             else:
                 unit_div_info.append("*")
 
             return ",".join(unit_div_info)
         except OOVError as e:
             raise e
@@ -209,23 +215,24 @@
     sudachi_dict_type = args.sudachi_dict_type
     unit_word_dict = args.unit_word_dict
 
     unit_words_dict: dict[str, UnitWord] = {}
     if not unit_word_dict == "":
         with fileinput.input(files=unit_word_dict) as merge_dict:
             for i, line in enumerate(merge_dict):
+                w = line.split(",")[0]
                 line = line.replace("\n", "")
-                unit_words_dict[line.split(",")[0]] = UnitWord(word_id=i, line=line)
+                unit_words_dict[w] = UnitWord(word_id=i, line=line)
                 out.write(f"{line}\n")
 
     c = Converter(
         rewrite,
         config,
         sudachi_setting=sudachi_setting,
-        dict_type=sudachi_dict_type,
+        sudachi_dict=sudachi_dict_type,
         rm=rm,
         unit_words_dict=unit_words_dict,
     )
 
     with fileinput.input(files=args.file) as input:
         for line in input:
             line = line.strip()
```

### Comparing `kuro2sudachi-0.4.0/src/kuro2sudachi/normalizer.py` & `kuro2sudachi-0.4.2/src/kuro2sudachi/normalizer.py`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.0/src/kuro2sudachi/rewrite.def` & `kuro2sudachi-0.4.2/src/kuro2sudachi/rewrite.def`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.0/PKG-INFO` & `kuro2sudachi-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuro2sudachi
-Version: 0.4.0
+Version: 0.4.2
 Summary: 
 Home-page: http://github.com/po3rin/kuro2sudachi
 License: Apache-2.0
 Author: po3rin
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

