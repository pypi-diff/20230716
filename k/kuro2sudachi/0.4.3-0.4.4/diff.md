# Comparing `tmp/kuro2sudachi-0.4.3.tar.gz` & `tmp/kuro2sudachi-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuro2sudachi-0.4.3.tar", max compression
+gzip compressed data, was "kuro2sudachi-0.4.4.tar", max compression
```

## Comparing `kuro2sudachi-0.4.3.tar` & `kuro2sudachi-0.4.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2851 2023-07-09 08:48:36.492983 kuro2sudachi-0.4.3/README.md
--rw-r--r--   0        0        0      694 2023-07-16 10:07:38.055781 kuro2sudachi-0.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.4.3/src/kuro2sudachi/__init__.py
--rw-r--r--   0        0        0     7645 2023-07-16 10:04:06.932006 kuro2sudachi-0.4.3/src/kuro2sudachi/core.py
--rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.4.3/src/kuro2sudachi/normalizer.py
--rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.4.3/src/kuro2sudachi/rewrite.def
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 kuro2sudachi-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2851 2023-07-09 08:48:36.492983 kuro2sudachi-0.4.4/README.md
+-rw-r--r--   0        0        0      694 2023-07-16 13:49:58.644778 kuro2sudachi-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.4.4/src/kuro2sudachi/__init__.py
+-rw-r--r--   0        0        0     7682 2023-07-16 13:47:45.484545 kuro2sudachi-0.4.4/src/kuro2sudachi/core.py
+-rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.4.4/src/kuro2sudachi/normalizer.py
+-rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.4.4/src/kuro2sudachi/rewrite.def
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 kuro2sudachi-0.4.4/PKG-INFO
```

### Comparing `kuro2sudachi-0.4.3/README.md` & `kuro2sudachi-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.3/pyproject.toml` & `kuro2sudachi-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuro2sudachi"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["po3rin"]
 repository = "http://github.com/po3rin/kuro2sudachi"
 homepage = "http://github.com/po3rin/kuro2sudachi"
 readme = "README.md"
 license = "Apache-2.0"
 include = ["rewrite.def"]
@@ -18,14 +18,14 @@
 importlib-metadata = "^6.7.0"
 sudachipy = "^0.6.7"
 sudachidict-core = "^20230110"
 sudachidict-full = "^20230110"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
-pytest = "^6.2.1"
+pytest = "^6.2.2"
 twine = "^4.0.2"
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `kuro2sudachi-0.4.3/src/kuro2sudachi/core.py` & `kuro2sudachi-0.4.4/src/kuro2sudachi/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,24 +165,23 @@
             if ",".join(m.part_of_speech()) == "名詞,数詞,*,*,*,*":
                 return "*"
 
             if m.is_oov() or m.dictionary_id() == -1:
                 oov.append(m.surface())
                 continue
 
-            if m.word_id() > MAX_WORD_ID:
-                # If word_mask and word_id match, there is a possibility that the word was generated by the rewrite plugin.
-                # In that case word_id is not defined, so you get an error when building the dictionary.
-                # Therefore, look up the word again in the dictionary and obtain the word_id(TODO).
-                print(f"{str(m)} word_id is greater than max_id {MAX_WORD_ID}. So skip without splitting.")
-                return "*"
-
             if str(m) in self.unit_words_dict:
                 word_ids.append(f"U{str(self.unit_words_dict[str(m)].word_id)}")
             else:
+                if m.word_id() > MAX_WORD_ID:
+                    # If word_mask and word_id match, there is a possibility that the word was generated by the rewrite plugin.
+                    # In that case word_id is not defined, so you get an error when building the dictionary.
+                    # Therefore, look up the word again in the dictionary and obtain the word_id(TODO).
+                    print(f"{str(m)} word_id {m.word_id()} is greater than max_id {MAX_WORD_ID}. So skip without splitting.")
+                    return "*"
                 word_ids.append(str(m.word_id()))
 
         if len(oov) > 0:
             raise OOVError(f"split word has out of vocab: {oov} in {word}")
 
         return "/".join(word_ids)
```

### Comparing `kuro2sudachi-0.4.3/src/kuro2sudachi/normalizer.py` & `kuro2sudachi-0.4.4/src/kuro2sudachi/normalizer.py`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.3/src/kuro2sudachi/rewrite.def` & `kuro2sudachi-0.4.4/src/kuro2sudachi/rewrite.def`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.3/PKG-INFO` & `kuro2sudachi-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuro2sudachi
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Home-page: http://github.com/po3rin/kuro2sudachi
 License: Apache-2.0
 Author: po3rin
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

