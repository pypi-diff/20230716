# Comparing `tmp/pyfsig-0.7.2.tar.gz` & `tmp/pyfsig-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfsig-0.7.2.tar", max compression
+gzip compressed data, was "pyfsig-0.8.2.tar", max compression
```

## Comparing `pyfsig-0.7.2.tar` & `pyfsig-0.8.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1070 2022-07-21 12:42:59.295801 pyfsig-0.7.2/LICENSE
--rw-r--r--   0        0        0    50216 2023-06-27 12:24:12.877968 pyfsig-0.7.2/README.md
--rw-r--r--   0        0        0      344 2023-06-27 12:25:45.677892 pyfsig-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      226 2022-07-22 08:49:13.622952 pyfsig-0.7.2/src/pyfsig/__init__.py
--rw-r--r--   0        0        0    43260 2023-06-27 11:55:30.582268 pyfsig-0.7.2/src/pyfsig/file_signatures.py
--rw-r--r--   0        0        0    56049 1970-01-01 00:00:00.000000 pyfsig-0.7.2/setup.py
--rw-r--r--   0        0        0    50829 1970-01-01 00:00:00.000000 pyfsig-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-07-21 12:42:59.295801 pyfsig-0.8.2/LICENSE
+-rw-r--r--   0        0        0    50216 2023-06-27 12:24:12.877968 pyfsig-0.8.2/README.md
+-rw-r--r--   0        0        0      344 2023-07-16 12:10:09.700930 pyfsig-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      226 2022-07-22 08:49:13.622952 pyfsig-0.8.2/src/pyfsig/__init__.py
+-rw-r--r--   0        0        0    43260 2023-06-27 11:55:30.582268 pyfsig-0.8.2/src/pyfsig/file_signatures.py
+-rw-r--r--   0        0        0    50829 1970-01-01 00:00:00.000000 pyfsig-0.8.2/PKG-INFO
```

### Comparing `pyfsig-0.7.2/LICENSE` & `pyfsig-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfsig-0.7.2/README.md` & `pyfsig-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfsig-0.7.2/src/pyfsig/file_signatures.py` & `pyfsig-0.8.2/src/pyfsig/file_signatures.py`

 * *Files identical despite different names*

### Comparing `pyfsig-0.7.2/PKG-INFO` & `pyfsig-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsig
-Version: 0.7.2
+Version: 0.8.2
 Summary: A library for identifying files form their magic byte signature.
 License: MIT
 Author: schlerp
 Author-email: schlerpderpson@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

