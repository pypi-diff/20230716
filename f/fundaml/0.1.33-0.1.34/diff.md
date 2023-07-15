# Comparing `tmp/fundaml-0.1.33.tar.gz` & `tmp/fundaml-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundaml-0.1.33.tar", max compression
+gzip compressed data, was "fundaml-0.1.34.tar", max compression
```

## Comparing `fundaml-0.1.33.tar` & `fundaml-0.1.34.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1069 2023-07-13 13:27:54.203014 fundaml-0.1.33/LICENSE
--rw-r--r--   0        0        0     2284 2023-07-13 13:27:54.203014 fundaml-0.1.33/README.md
--rw-r--r--   0        0        0     1614 2023-07-13 13:40:01.281395 fundaml-0.1.33/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/__init__.py
--rw-r--r--   0        0        0     1058 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/eda.py
--rw-r--r--   0        0        0     1400 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/models.py
--rw-r--r--   0        0        0     1032 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/scores.py
--rw-r--r--   0        0        0    17645 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/trainers.py
--rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 fundaml-0.1.33/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-15 22:46:23.198281 fundaml-0.1.34/LICENSE
+-rw-r--r--   0        0        0     2284 2023-07-15 22:46:23.198281 fundaml-0.1.34/README.md
+-rw-r--r--   0        0        0     1614 2023-07-15 23:03:27.770897 fundaml-0.1.34/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-15 22:46:23.658285 fundaml-0.1.34/src/fundaml/__init__.py
+-rw-r--r--   0        0        0     1058 2023-07-15 22:46:23.658285 fundaml-0.1.34/src/fundaml/eda.py
+-rw-r--r--   0        0        0     3247 2023-07-15 22:46:23.658285 fundaml-0.1.34/src/fundaml/models.py
+-rw-r--r--   0        0        0     1032 2023-07-15 22:46:23.658285 fundaml-0.1.34/src/fundaml/scores.py
+-rw-r--r--   0        0        0    17645 2023-07-15 22:46:23.658285 fundaml-0.1.34/src/fundaml/trainers.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 fundaml-0.1.34/PKG-INFO
```

### Comparing `fundaml-0.1.33/LICENSE` & `fundaml-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.33/README.md` & `fundaml-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.33/pyproject.toml` & `fundaml-0.1.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fundaml"
-version = "0.1.33"
+version = "0.1.34"
 description = "A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks."
 authors = ["Tony Zoght"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `fundaml-0.1.33/src/fundaml/eda.py` & `fundaml-0.1.34/src/fundaml/eda.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.33/src/fundaml/scores.py` & `fundaml-0.1.34/src/fundaml/scores.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.33/src/fundaml/trainers.py` & `fundaml-0.1.34/src/fundaml/trainers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.33/PKG-INFO` & `fundaml-0.1.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundaml
-Version: 0.1.33
+Version: 0.1.34
 Summary: A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks.
 License: MIT
 Author: Tony Zoght
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

