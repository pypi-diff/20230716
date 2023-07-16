# Comparing `tmp/kuro2sudachi-0.4.5.tar.gz` & `tmp/kuro2sudachi-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuro2sudachi-0.4.5.tar", max compression
+gzip compressed data, was "kuro2sudachi-0.4.6.tar", max compression
```

## Comparing `kuro2sudachi-0.4.5.tar` & `kuro2sudachi-0.4.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2851 2023-07-09 08:48:36.492983 kuro2sudachi-0.4.5/README.md
--rw-r--r--   0        0        0      694 2023-07-16 15:41:10.065486 kuro2sudachi-0.4.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.4.5/src/kuro2sudachi/__init__.py
--rw-r--r--   0        0        0     7981 2023-07-16 15:40:36.737813 kuro2sudachi-0.4.5/src/kuro2sudachi/core.py
--rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.4.5/src/kuro2sudachi/normalizer.py
--rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.4.5/src/kuro2sudachi/rewrite.def
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 kuro2sudachi-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     2851 2023-07-09 08:48:36.492983 kuro2sudachi-0.4.6/README.md
+-rw-r--r--   0        0        0      694 2023-07-16 15:50:46.588692 kuro2sudachi-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.4.6/src/kuro2sudachi/__init__.py
+-rw-r--r--   0        0        0     8165 2023-07-16 15:49:11.005810 kuro2sudachi-0.4.6/src/kuro2sudachi/core.py
+-rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.4.6/src/kuro2sudachi/normalizer.py
+-rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.4.6/src/kuro2sudachi/rewrite.def
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 kuro2sudachi-0.4.6/PKG-INFO
```

### Comparing `kuro2sudachi-0.4.5/README.md` & `kuro2sudachi-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.5/pyproject.toml` & `kuro2sudachi-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuro2sudachi"
-version = "0.4.5"
+version = "0.4.6"
 description = ""
 authors = ["po3rin"]
 repository = "http://github.com/po3rin/kuro2sudachi"
 homepage = "http://github.com/po3rin/kuro2sudachi"
 readme = "README.md"
 license = "Apache-2.0"
 include = ["rewrite.def"]
```

### Comparing `kuro2sudachi-0.4.5/src/kuro2sudachi/core.py` & `kuro2sudachi-0.4.6/src/kuro2sudachi/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,17 +178,23 @@
                     # Therefore, look up the word again in the dictionary and obtain the word_id(TODO).
                     print(f"{str(m)} word_id {m.word_id()} is greater than max_id {MAX_WORD_ID}. So lookup the word directly from the dictionary.")
                     lookup_list = self.dic.lookup(str(m))
 
                     word_id = None
                     for l in lookup_list:
                         if str(m) == str(l):
-                            word_ids.append(str(m.word_id()))
-                            break
-                    return "*"
+                            print(l.word_id())
+                            word_id = str(l.word_id())
+
+                    if word_id is None:
+                        return "*"
+                    else:
+                        word_ids.append(word_id)
+                        continue
+                        
                 word_ids.append(str(m.word_id()))
 
         if len(oov) > 0:
             raise OOVError(f"split word has out of vocab: {oov} in {word}")
 
         return "/".join(word_ids)
```

### Comparing `kuro2sudachi-0.4.5/src/kuro2sudachi/normalizer.py` & `kuro2sudachi-0.4.6/src/kuro2sudachi/normalizer.py`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.5/src/kuro2sudachi/rewrite.def` & `kuro2sudachi-0.4.6/src/kuro2sudachi/rewrite.def`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.4.5/PKG-INFO` & `kuro2sudachi-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuro2sudachi
-Version: 0.4.5
+Version: 0.4.6
 Summary: 
 Home-page: http://github.com/po3rin/kuro2sudachi
 License: Apache-2.0
 Author: po3rin
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

