# Comparing `tmp/clean_base-0.1.0.tar.gz` & `tmp/clean_base-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_base-0.1.0.tar", last modified: Sun Jul 16 15:09:07 2023, max compression
+gzip compressed data, was "clean_base-0.1.1.tar", last modified: Sun Jul 16 19:16:10 2023, max compression
```

## Comparing `clean_base-0.1.0.tar` & `clean_base-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 15:09:07.789639 clean_base-0.1.0/
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      210 2023-07-16 15:08:34.000000 clean_base-0.1.0/.cz.toml
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      172 2023-07-16 14:57:01.000000 clean_base-0.1.0/.gitignore
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1103 2023-07-16 15:05:04.000000 clean_base-0.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      158 2023-07-16 15:05:09.000000 clean_base-0.1.0/.pypirc
-drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 15:09:07.789639 clean_base-0.1.0/.vscode/
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       51 2023-07-16 14:30:15.000000 clean_base-0.1.0/.vscode/settings.json
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       51 2023-07-16 15:02:22.000000 clean_base-0.1.0/CHANGELOG.md
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1072 2023-07-16 14:35:40.000000 clean_base-0.1.0/LICENSE
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      819 2023-07-16 15:09:07.789639 clean_base-0.1.0/PKG-INFO
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      328 2023-07-16 15:05:43.000000 clean_base-0.1.0/Pipfile
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       62 2023-07-16 14:31:43.000000 clean_base-0.1.0/README.md
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1967 2023-07-16 15:08:34.000000 clean_base-0.1.0/pyproject.toml
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       38 2023-07-16 15:09:07.789639 clean_base-0.1.0/setup.cfg
-drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 15:09:07.785639 clean_base-0.1.0/src/
-drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 15:09:07.789639 clean_base-0.1.0/src/clean_base/
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 14:04:41.000000 clean_base-0.1.0/src/clean_base/__main__.py
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1628 2023-07-16 14:20:32.000000 clean_base-0.1.0/src/clean_base/either.py
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     7008 2023-07-16 14:19:09.000000 clean_base-0.1.0/src/clean_base/entities.py
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     9349 2023-07-16 14:28:35.000000 clean_base-0.1.0/src/clean_base/exceptions.py
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     3640 2023-07-16 14:13:04.000000 clean_base-0.1.0/src/clean_base/lock.py
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1367 2023-07-16 14:13:35.000000 clean_base-0.1.0/src/clean_base/settings.py
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      861 2023-07-16 14:30:43.000000 clean_base-0.1.0/src/clean_base/validations.py
-drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 15:09:07.789639 clean_base-0.1.0/src/clean_base.egg-info/
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      819 2023-07-16 15:09:07.000000 clean_base-0.1.0/src/clean_base.egg-info/PKG-INFO
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      467 2023-07-16 15:09:07.000000 clean_base-0.1.0/src/clean_base.egg-info/SOURCES.txt
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)        1 2023-07-16 15:09:07.000000 clean_base-0.1.0/src/clean_base.egg-info/dependency_links.txt
--rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       11 2023-07-16 15:09:07.000000 clean_base-0.1.0/src/clean_base.egg-info/top_level.txt
+drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 19:16:10.456181 clean_base-0.1.1/
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      210 2023-07-16 19:15:19.000000 clean_base-0.1.1/.cz.toml
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      172 2023-07-16 14:57:01.000000 clean_base-0.1.1/.gitignore
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1103 2023-07-16 15:05:04.000000 clean_base-0.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      158 2023-07-16 15:05:09.000000 clean_base-0.1.1/.pypirc
+drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 19:16:10.452181 clean_base-0.1.1/.vscode/
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       51 2023-07-16 14:30:15.000000 clean_base-0.1.1/.vscode/settings.json
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      145 2023-07-16 19:15:19.000000 clean_base-0.1.1/CHANGELOG.md
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1072 2023-07-16 14:35:40.000000 clean_base-0.1.1/LICENSE
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      819 2023-07-16 19:16:10.456181 clean_base-0.1.1/PKG-INFO
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      327 2023-07-16 19:13:15.000000 clean_base-0.1.1/Pipfile
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       62 2023-07-16 14:31:43.000000 clean_base-0.1.1/README.md
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1967 2023-07-16 19:15:19.000000 clean_base-0.1.1/pyproject.toml
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       38 2023-07-16 19:16:10.456181 clean_base-0.1.1/setup.cfg
+drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 19:16:10.452181 clean_base-0.1.1/src/
+drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 19:16:10.452181 clean_base-0.1.1/src/clean_base/
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 14:04:41.000000 clean_base-0.1.1/src/clean_base/__main__.py
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1628 2023-07-16 14:20:32.000000 clean_base-0.1.1/src/clean_base/either.py
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     7008 2023-07-16 14:19:09.000000 clean_base-0.1.1/src/clean_base/entities.py
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     9351 2023-07-16 19:12:12.000000 clean_base-0.1.1/src/clean_base/exceptions.py
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     3640 2023-07-16 14:13:04.000000 clean_base-0.1.1/src/clean_base/lock.py
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)     1367 2023-07-16 14:13:35.000000 clean_base-0.1.1/src/clean_base/settings.py
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      861 2023-07-16 14:30:43.000000 clean_base-0.1.1/src/clean_base/validations.py
+drwxrwxr-x   0 sgelias   (1000) sgelias   (1000)        0 2023-07-16 19:16:10.456181 clean_base-0.1.1/src/clean_base.egg-info/
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      819 2023-07-16 19:16:10.000000 clean_base-0.1.1/src/clean_base.egg-info/PKG-INFO
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)      467 2023-07-16 19:16:10.000000 clean_base-0.1.1/src/clean_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)        1 2023-07-16 19:16:10.000000 clean_base-0.1.1/src/clean_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 sgelias   (1000) sgelias   (1000)       11 2023-07-16 19:16:10.000000 clean_base-0.1.1/src/clean_base.egg-info/top_level.txt
```

### Comparing `clean_base-0.1.0/.pre-commit-config.yaml` & `clean_base-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `clean_base-0.1.0/LICENSE` & `clean_base-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_base-0.1.0/PKG-INFO` & `clean_base-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean_base
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple and lighweight package tor clean softwares.
 Author-email: Samuel Galvão Elias <sgelias@outlook.com>
 Project-URL: Homepage, https://github.com/sgelias/clean-base-py
 Keywords: Bioinformatics,Clean Architecture,Monad Either
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clean_base-0.1.0/pyproject.toml` & `clean_base-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # ? ----------------------------------------------------------------------------
 # ? Building
 # ? ----------------------------------------------------------------------------
 
 [project]
 
 name = "clean_base"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Samuel Galvão Elias", email = "sgelias@outlook.com" },
 ]
 description = "A simple and lighweight package tor clean softwares."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["Bioinformatics", "Clean Architecture", "Monad Either"]
```

### Comparing `clean_base-0.1.0/src/clean_base/either.py` & `clean_base-0.1.1/src/clean_base/either.py`

 * *Files identical despite different names*

### Comparing `clean_base-0.1.0/src/clean_base/entities.py` & `clean_base-0.1.1/src/clean_base/entities.py`

 * *Files identical despite different names*

### Comparing `clean_base-0.1.0/src/clean_base/exceptions.py` & `clean_base-0.1.1/src/clean_base/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import IntEnum, auto
 from logging import Logger, getLogger
 from typing import Any, Self
 
-from agrobase.settings import LOGGER
+from clean_base.settings import LOGGER
 
 from .either import Left, left
 
 
 class ErrorCodes(IntEnum):
     # Default option
     UNDEFINED_ERROR = 0
```

### Comparing `clean_base-0.1.0/src/clean_base/lock.py` & `clean_base-0.1.1/src/clean_base/lock.py`

 * *Files identical despite different names*

### Comparing `clean_base-0.1.0/src/clean_base/settings.py` & `clean_base-0.1.1/src/clean_base/settings.py`

 * *Files identical despite different names*

### Comparing `clean_base-0.1.0/src/clean_base/validations.py` & `clean_base-0.1.1/src/clean_base/validations.py`

 * *Files identical despite different names*

### Comparing `clean_base-0.1.0/src/clean_base.egg-info/PKG-INFO` & `clean_base-0.1.1/src/clean_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-base
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple and lighweight package tor clean softwares.
 Author-email: Samuel Galvão Elias <sgelias@outlook.com>
 Project-URL: Homepage, https://github.com/sgelias/clean-base-py
 Keywords: Bioinformatics,Clean Architecture,Monad Either
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

