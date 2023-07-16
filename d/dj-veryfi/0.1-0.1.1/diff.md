# Comparing `tmp/dj-veryfi-0.1.tar.gz` & `tmp/dj-veryfi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-veryfi-0.1.tar", last modified: Sat Jul 15 23:59:10 2023, max compression
+gzip compressed data, was "dist/dj-veryfi-0.1.1.tar", last modified: Sun Jul 16 00:02:05 2023, max compression
```

## Comparing `dj-veryfi-0.1.tar` & `dj-veryfi-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-15 23:59:10.000000 dj-veryfi-0.1/
--rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1/LICENSE
--rw-r--r--   0 tony      (1000) tony      (1000)       31 2023-07-15 23:57:56.000000 dj-veryfi-0.1/MANIFEST.in
--rw-r--r--   0 tony      (1000) tony      (1000)     3497 2023-07-15 23:59:10.000000 dj-veryfi-0.1/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     2884 2023-07-15 23:59:03.000000 dj-veryfi-0.1/README
--rw-r--r--   0 tony      (1000) tony      (1000)     2923 2023-07-15 23:58:12.000000 dj-veryfi-0.1/README.rst
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-15 23:59:10.000000 dj-veryfi-0.1/dj_veryfi.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3497 2023-07-15 23:59:10.000000 dj-veryfi-0.1/dj_veryfi.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      285 2023-07-15 23:59:10.000000 dj-veryfi-0.1/dj_veryfi.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-15 23:59:10.000000 dj-veryfi-0.1/dj_veryfi.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-15 23:59:10.000000 dj-veryfi-0.1/dj_veryfi.egg-info/requires.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       11 2023-07-15 23:59:10.000000 dj-veryfi-0.1/dj_veryfi.egg-info/top_level.txt
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-15 23:59:10.000000 dj-veryfi-0.1/migrations/
--rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1/migrations/0001_initial.py
--rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1/migrations/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)       88 2023-07-15 23:03:01.000000 dj-veryfi-0.1/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      692 2023-07-15 23:59:10.000000 dj-veryfi-0.1/setup.cfg
--rw-r--r--   0 tony      (1000) tony      (1000)       80 2023-07-15 23:57:15.000000 dj-veryfi-0.1/setup.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/
+-rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.1/LICENSE
+-rw-r--r--   0 tony      (1000) tony      (1000)       35 2023-07-16 00:00:43.000000 dj-veryfi-0.1.1/MANIFEST.in
+-rw-r--r--   0 tony      (1000) tony      (1000)     3499 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     2884 2023-07-15 23:59:03.000000 dj-veryfi-0.1.1/README
+-rw-r--r--   0 tony      (1000) tony      (1000)     2923 2023-07-15 23:58:12.000000 dj-veryfi-0.1.1/README.rst
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/dj_veryfi.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3499 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/dj_veryfi.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      285 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/dj_veryfi.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/dj_veryfi.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/dj_veryfi.egg-info/requires.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       11 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/dj_veryfi.egg-info/top_level.txt
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/migrations/
+-rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.1/migrations/0001_initial.py
+-rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.1/migrations/__init__.py
+-rw-r--r--   0 tony      (1000) tony      (1000)       88 2023-07-15 23:03:01.000000 dj-veryfi-0.1.1/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      694 2023-07-16 00:02:05.000000 dj-veryfi-0.1.1/setup.cfg
+-rw-r--r--   0 tony      (1000) tony      (1000)       80 2023-07-15 23:57:15.000000 dj-veryfi-0.1.1/setup.py
```

### Comparing `dj-veryfi-0.1/LICENSE` & `dj-veryfi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1/PKG-INFO` & `dj-veryfi-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1
+Version: 0.1.1
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-veryfi-0.1/README` & `dj-veryfi-0.1.1/README`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1/README.rst` & `dj-veryfi-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1/dj_veryfi.egg-info/PKG-INFO` & `dj-veryfi-0.1.1/dj_veryfi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1
+Version: 0.1.1
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-veryfi-0.1/migrations/0001_initial.py` & `dj-veryfi-0.1.1/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1/setup.cfg` & `dj-veryfi-0.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-veryfi
-version = 0.1
+version = 0.1.1
 description = Django integration for Veryfi OCR API.
 long_description = file: README
 url = https://github.com/tonykamillo/dj-veryfi
 author = Tony Kamillo
 author_email = tonykamillo@gmail.com
 license = DBAD
 classifiers =
```

