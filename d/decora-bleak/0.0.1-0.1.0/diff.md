# Comparing `tmp/decora_bleak-0.0.1.tar.gz` & `tmp/decora_bleak-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decora_bleak-0.0.1.tar", last modified: Tue Jul 11 22:11:01 2023, max compression
+gzip compressed data, was "decora_bleak-0.1.0.tar", last modified: Sun Jul 16 06:41:20 2023, max compression
```

## Comparing `decora_bleak-0.0.1.tar` & `decora_bleak-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-11 22:11:01.507160 decora_bleak-0.0.1/
--rw-r--r--   0 colinc     (501) staff       (20)     4462 2023-07-11 21:05:16.000000 decora_bleak-0.0.1/CONNECTION_NOTES.md
--rw-r--r--   0 colinc     (501) staff       (20)     1111 2023-07-11 03:01:46.000000 decora_bleak-0.0.1/LICENSE
--rw-r--r--   0 colinc     (501) staff       (20)       26 2023-07-11 21:59:56.000000 decora_bleak-0.0.1/MANIFEST.in
--rw-r--r--   0 colinc     (501) staff       (20)     1309 2023-07-11 22:11:01.507053 decora_bleak-0.0.1/PKG-INFO
--rw-r--r--   0 colinc     (501) staff       (20)      824 2023-07-11 21:58:00.000000 decora_bleak-0.0.1/README.md
--rw-r--r--   0 colinc     (501) staff       (20)     3056 2023-07-11 21:34:42.000000 decora_bleak-0.0.1/example.py
--rw-r--r--   0 colinc     (501) staff       (20)      944 2023-07-11 22:04:08.000000 decora_bleak-0.0.1/pyproject.toml
--rw-r--r--   0 colinc     (501) staff       (20)       38 2023-07-11 22:11:01.507188 decora_bleak-0.0.1/setup.cfg
--rw-r--r--   0 colinc     (501) staff       (20)      376 2023-07-11 21:57:12.000000 decora_bleak-0.0.1/setup.py
-drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-11 22:11:01.505124 decora_bleak-0.0.1/src/
-drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-11 22:11:01.506299 decora_bleak-0.0.1/src/decora_bleak/
--rw-r--r--   0 colinc     (501) staff       (20)      418 2023-07-11 21:57:12.000000 decora_bleak-0.0.1/src/decora_bleak/__init__.py
--rw-r--r--   0 colinc     (501) staff       (20)      482 2023-07-11 20:43:06.000000 decora_bleak-0.0.1/src/decora_bleak/const.py
--rw-r--r--   0 colinc     (501) staff       (20)     3550 2023-07-11 21:42:46.000000 decora_bleak-0.0.1/src/decora_bleak/decora_bleak.py
--rw-r--r--   0 colinc     (501) staff       (20)      179 2023-07-11 16:51:13.000000 decora_bleak-0.0.1/src/decora_bleak/models.py
-drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-11 22:11:01.506885 decora_bleak-0.0.1/src/decora_bleak.egg-info/
--rw-r--r--   0 colinc     (501) staff       (20)     1309 2023-07-11 22:11:01.000000 decora_bleak-0.0.1/src/decora_bleak.egg-info/PKG-INFO
--rw-r--r--   0 colinc     (501) staff       (20)      398 2023-07-11 22:11:01.000000 decora_bleak-0.0.1/src/decora_bleak.egg-info/SOURCES.txt
--rw-r--r--   0 colinc     (501) staff       (20)        1 2023-07-11 22:11:01.000000 decora_bleak-0.0.1/src/decora_bleak.egg-info/dependency_links.txt
--rw-r--r--   0 colinc     (501) staff       (20)       52 2023-07-11 22:11:01.000000 decora_bleak-0.0.1/src/decora_bleak.egg-info/requires.txt
--rw-r--r--   0 colinc     (501) staff       (20)       13 2023-07-11 22:11:01.000000 decora_bleak-0.0.1/src/decora_bleak.egg-info/top_level.txt
+drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-16 06:41:20.232322 decora_bleak-0.1.0/
+-rw-r--r--   0 colinc     (501) staff       (20)     4462 2023-07-11 21:05:16.000000 decora_bleak-0.1.0/CONNECTION_NOTES.md
+-rw-r--r--   0 colinc     (501) staff       (20)     1111 2023-07-11 03:01:46.000000 decora_bleak-0.1.0/LICENSE
+-rw-r--r--   0 colinc     (501) staff       (20)       26 2023-07-11 21:59:56.000000 decora_bleak-0.1.0/MANIFEST.in
+-rw-r--r--   0 colinc     (501) staff       (20)     1391 2023-07-16 06:41:20.232211 decora_bleak-0.1.0/PKG-INFO
+-rw-r--r--   0 colinc     (501) staff       (20)      906 2023-07-13 21:55:21.000000 decora_bleak-0.1.0/README.md
+-rw-r--r--   0 colinc     (501) staff       (20)     1032 2023-07-16 06:40:39.000000 decora_bleak-0.1.0/pyproject.toml
+-rw-r--r--   0 colinc     (501) staff       (20)       38 2023-07-16 06:41:20.232353 decora_bleak-0.1.0/setup.cfg
+-rw-r--r--   0 colinc     (501) staff       (20)      376 2023-07-16 06:40:39.000000 decora_bleak-0.1.0/setup.py
+drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-16 06:41:20.229107 decora_bleak-0.1.0/src/
+drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-16 06:41:20.230751 decora_bleak-0.1.0/src/decora_bleak/
+-rw-r--r--   0 colinc     (501) staff       (20)      540 2023-07-16 06:40:39.000000 decora_bleak-0.1.0/src/decora_bleak/__init__.py
+-rw-r--r--   0 colinc     (501) staff       (20)     4113 2023-07-16 06:38:16.000000 decora_bleak-0.1.0/src/decora_bleak/cmd.py
+-rw-r--r--   0 colinc     (501) staff       (20)      767 2023-07-13 23:56:48.000000 decora_bleak-0.1.0/src/decora_bleak/const.py
+-rw-r--r--   0 colinc     (501) staff       (20)     7254 2023-07-16 06:38:16.000000 decora_bleak-0.1.0/src/decora_bleak/decora_bleak.py
+-rw-r--r--   0 colinc     (501) staff       (20)      365 2023-07-14 00:01:50.000000 decora_bleak-0.1.0/src/decora_bleak/models.py
+drwxr-xr-x   0 colinc     (501) staff       (20)        0 2023-07-16 06:41:20.232064 decora_bleak-0.1.0/src/decora_bleak.egg-info/
+-rw-r--r--   0 colinc     (501) staff       (20)     1391 2023-07-16 06:41:20.000000 decora_bleak-0.1.0/src/decora_bleak.egg-info/PKG-INFO
+-rw-r--r--   0 colinc     (501) staff       (20)      454 2023-07-16 06:41:20.000000 decora_bleak-0.1.0/src/decora_bleak.egg-info/SOURCES.txt
+-rw-r--r--   0 colinc     (501) staff       (20)        1 2023-07-16 06:41:20.000000 decora_bleak-0.1.0/src/decora_bleak.egg-info/dependency_links.txt
+-rw-r--r--   0 colinc     (501) staff       (20)       49 2023-07-16 06:41:20.000000 decora_bleak-0.1.0/src/decora_bleak.egg-info/entry_points.txt
+-rw-r--r--   0 colinc     (501) staff       (20)       81 2023-07-16 06:41:20.000000 decora_bleak-0.1.0/src/decora_bleak.egg-info/requires.txt
+-rw-r--r--   0 colinc     (501) staff       (20)       13 2023-07-16 06:41:20.000000 decora_bleak-0.1.0/src/decora_bleak.egg-info/top_level.txt
```

### Comparing `decora_bleak-0.0.1/CONNECTION_NOTES.md` & `decora_bleak-0.1.0/CONNECTION_NOTES.md`

 * *Files identical despite different names*

### Comparing `decora_bleak-0.0.1/LICENSE` & `decora_bleak-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decora_bleak-0.0.1/PKG-INFO` & `decora_bleak-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decora_bleak
-Version: 0.0.1
+Version: 0.1.0
 Summary: A package for interacting with Decora switches and dimmers over BLE
 Author-email: Colin Campbell <colin.campbell@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,24 +14,26 @@
 
 # decora_bleak
 
 Python module for interacting with Leviton bluetooth switches and dimmers via BLE (Bluetooth Low Energy). There is prior art in this space, namely https://github.com/mjg59/python-decora and https://github.com/lucapinello/pydecora_ble, both of which primarily use the bluepy module. This project aims to provide the same support using Bleak which is used for interacting with BLE devices in Home Assistant.
 
 ## Using
 
+Once the package is installed (and assuming the repo was cloned to make changes) using `python -m pip install -e .`:
+
 ```
-python3 example.py
+decora scan
 ```
 
 ```
-python3 example.py --address "C84441EE-5C57-2681-1BD5-82AF18C58F5D"
+decora connect -a "C84441EE-5C57-2681-1BD5-82AF18C58F5D"
 ```
 
 ```
-python3 example.py --address "C84441EE-5C57-2681-1BD5-82AF18C58F5D" --api-key "8c4c89fa00"
+decora connect -a "C84441EE-5C57-2681-1BD5-82AF18C58F5D" -k "8c4c89fa00"
 ```
 
 ## Releasing
 
 One of
 
 ```
```

### Comparing `decora_bleak-0.0.1/README.md` & `decora_bleak-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # decora_bleak
 
 Python module for interacting with Leviton bluetooth switches and dimmers via BLE (Bluetooth Low Energy). There is prior art in this space, namely https://github.com/mjg59/python-decora and https://github.com/lucapinello/pydecora_ble, both of which primarily use the bluepy module. This project aims to provide the same support using Bleak which is used for interacting with BLE devices in Home Assistant.
 
 ## Using
 
+Once the package is installed (and assuming the repo was cloned to make changes) using `python -m pip install -e .`:
+
 ```
-python3 example.py
+decora scan
 ```
 
 ```
-python3 example.py --address "C84441EE-5C57-2681-1BD5-82AF18C58F5D"
+decora connect -a "C84441EE-5C57-2681-1BD5-82AF18C58F5D"
 ```
 
 ```
-python3 example.py --address "C84441EE-5C57-2681-1BD5-82AF18C58F5D" --api-key "8c4c89fa00"
+decora connect -a "C84441EE-5C57-2681-1BD5-82AF18C58F5D" -k "8c4c89fa00"
 ```
 
 ## Releasing
 
 One of
 
 ```
```

### Comparing `decora_bleak-0.0.1/pyproject.toml` & `decora_bleak-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "decora_bleak"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Colin Campbell", email="colin.campbell@gmail.com" },
 ]
 description = "A package for interacting with Decora switches and dimmers over BLE"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "bleak >= 0.20.2"
+  "bleak >= 0.20.2",
+  "bleak_retry_connector >= 3.0.0"
 ]
 
 [project.optional-dependencies]
 dev = ["bumpver", "isort", "pip-tools", "pytest"]
 
+[project.scripts]
+decora = "decora_bleak.cmd:main"
+
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "setup.py" = ['version="{version}"']
 "src/decora_bleak/__init__.py" = ['__version__ = "{version}"']
```

### Comparing `decora_bleak-0.0.1/src/decora_bleak.egg-info/PKG-INFO` & `decora_bleak-0.1.0/src/decora_bleak.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decora-bleak
-Version: 0.0.1
+Version: 0.1.0
 Summary: A package for interacting with Decora switches and dimmers over BLE
 Author-email: Colin Campbell <colin.campbell@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,24 +14,26 @@
 
 # decora_bleak
 
 Python module for interacting with Leviton bluetooth switches and dimmers via BLE (Bluetooth Low Energy). There is prior art in this space, namely https://github.com/mjg59/python-decora and https://github.com/lucapinello/pydecora_ble, both of which primarily use the bluepy module. This project aims to provide the same support using Bleak which is used for interacting with BLE devices in Home Assistant.
 
 ## Using
 
+Once the package is installed (and assuming the repo was cloned to make changes) using `python -m pip install -e .`:
+
 ```
-python3 example.py
+decora scan
 ```
 
 ```
-python3 example.py --address "C84441EE-5C57-2681-1BD5-82AF18C58F5D"
+decora connect -a "C84441EE-5C57-2681-1BD5-82AF18C58F5D"
 ```
 
 ```
-python3 example.py --address "C84441EE-5C57-2681-1BD5-82AF18C58F5D" --api-key "8c4c89fa00"
+decora connect -a "C84441EE-5C57-2681-1BD5-82AF18C58F5D" -k "8c4c89fa00"
 ```
 
 ## Releasing
 
 One of
 
 ```
```

