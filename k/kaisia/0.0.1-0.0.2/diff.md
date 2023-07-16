# Comparing `tmp/kaisia-0.0.1.tar.gz` & `tmp/kaisia-0.0.2.tar.gz`

## Comparing `kaisia-0.0.1.tar` & `kaisia-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 kaisia-0.0.1/dev-requirements.in
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kaisia-0.0.1/dev-requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kaisia-0.0.1/requirements.in
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 kaisia-0.0.1/requirements.txt
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 kaisia-0.0.1/src/kaisia/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kaisia-0.0.1/src/kaisia/auth.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 kaisia-0.0.1/src/kaisia/cli.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 kaisia-0.0.1/src/kaisia/config.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kaisia-0.0.1/src/kaisia/exceptions.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 kaisia-0.0.1/src/kaisia/gbq.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kaisia-0.0.1/src/kaisia/version.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 kaisia-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kaisia-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaisia-0.0.1/README.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 kaisia-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 kaisia-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 kaisia-0.0.2/dev-requirements.in
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kaisia-0.0.2/dev-requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kaisia-0.0.2/requirements.in
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 kaisia-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/auth.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/cli.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/config.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/exceptions.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/gbq.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/main.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kaisia-0.0.2/src/kaisia/version.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 kaisia-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kaisia-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaisia-0.0.2/README.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 kaisia-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 kaisia-0.0.2/PKG-INFO
```

### Comparing `kaisia-0.0.1/dev-requirements.txt` & `kaisia-0.0.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/requirements.txt` & `kaisia-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/src/kaisia/__init__.py` & `kaisia-0.0.2/src/kaisia/main.py`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/src/kaisia/cli.py` & `kaisia-0.0.2/src/kaisia/cli.py`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/src/kaisia/config.py` & `kaisia-0.0.2/src/kaisia/config.py`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/src/kaisia/exceptions.py` & `kaisia-0.0.2/src/kaisia/exceptions.py`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/src/kaisia/gbq.py` & `kaisia-0.0.2/src/kaisia/gbq.py`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/.gitignore` & `kaisia-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/LICENSE` & `kaisia-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaisia-0.0.1/pyproject.toml` & `kaisia-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [project]
 name = "kaisia"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Rostislav Bagrov", email="bagrov.rostislav@gmail.com" },
 ]
 dependencies = [
     "google-cloud-bigquery",
 ]
 description = "GCP Big Query Migration helper"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+[project.scripts]
+kaisia = "kaisia.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/rbagrov/GBQM"
 "Bug Tracker" = "https://github.com/rbagrov/GBQM/issues"
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

