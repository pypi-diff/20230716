# Comparing `tmp/summo-0.0.5.tar.gz` & `tmp/summo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summo-0.0.5.tar", last modified: Mon Jul 10 23:07:12 2023, max compression
+gzip compressed data, was "summo-0.0.6.tar", last modified: Sun Jul 16 16:42:39 2023, max compression
```

## Comparing `summo-0.0.5.tar` & `summo-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 23:07:03.000000 summo-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-10 23:07:12.787935 summo-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 23:07:03.000000 summo-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-10 23:07:03.000000 summo-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:07:12.787935 summo-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/src/summo/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 23:07:03.000000 summo-0.0.5/src/summo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-10 23:07:03.000000 summo-0.0.5/src/summo/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/src/summo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:07:12.000000 summo-0.0.5/src/summo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:07:12.787935 summo-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-10 23:07:03.000000 summo-0.0.5/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:39.813058 summo-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 16:42:30.000000 summo-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-16 16:42:39.813058 summo-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-16 16:42:30.000000 summo-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-16 16:42:30.000000 summo-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:42:39.813058 summo-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:39.813058 summo-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:39.813058 summo-0.0.6/src/summo/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-16 16:42:30.000000 summo-0.0.6/src/summo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-16 16:42:30.000000 summo-0.0.6/src/summo/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:39.813058 summo-0.0.6/src/summo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-16 16:42:39.000000 summo-0.0.6/src/summo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-16 16:42:39.000000 summo-0.0.6/src/summo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:42:39.000000 summo-0.0.6/src/summo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-16 16:42:39.000000 summo-0.0.6/src/summo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 16:42:39.000000 summo-0.0.6/src/summo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:39.813058 summo-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-16 16:42:30.000000 summo-0.0.6/tests/test_summary.py
```

### Comparing `summo-0.0.5/LICENSE` & `summo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `summo-0.0.5/PKG-INFO` & `summo-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: summo
-Version: 0.0.5
-Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
-License: MIT License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tests
-Provides-Extra: typing
-License-File: LICENSE
-
 # Summo
 
 Summo is a Python package to summarize a dataset information
 
 ```python
 import summo
 import pandas as pd
@@ -64,8 +52,8 @@
         },
     },
 }
 ```
 
 ## Installation
 
-- `pip install summo`
+- `pip install summo`
```

### Comparing `summo-0.0.5/pyproject.toml` & `summo-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "summo"
-version = "0.0.5"
-description = ""
+dynamic = ["version"]
+description = "Describe in detail a pandas DataFrame"
+keywords = ["dataframe", "describe", "statistics"]
 requires-python = ">=3.9"
 readme = "README.md"
 license = { text = "MIT License" }
 authors = [{ name = "Rafael Sanabria", email = "rafael.d.sanabria@gmail.com" }]
 dependencies = ["pandas >= 2.0.0"]
-classifiers = []
+classifiers = [
+  "Development Status :: 1 - Planning",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Scientific/Engineering"
+]
+
+[project.urls]
+repository = "https://github.com/rfsan/summo"
 
 # consider including tox, build, twine
 [project.optional-dependencies]
 dev = ["pytest >= 7.3", "black >= 23.3.0", "ruff>=0.0.275"]
 tests = ["pytest >= 7.3", "deepdiff >= 6.3.1"]
 typing = ["pandas-stubs > 2.0.0"]
 
+[tool.setuptools.dynamic]
+version = {attr = "summo.__version__"}
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.black]
 line-length = 100
 
 [tool.ruff]
```

### Comparing `summo-0.0.5/src/summo/summary.py` & `summo-0.0.6/src/summo/summary.py`

 * *Files identical despite different names*

### Comparing `summo-0.0.5/tests/test_summary.py` & `summo-0.0.6/tests/test_summary.py`

 * *Files identical despite different names*

