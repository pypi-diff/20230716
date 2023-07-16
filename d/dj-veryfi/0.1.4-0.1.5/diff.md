# Comparing `tmp/dj-veryfi-0.1.4.tar.gz` & `tmp/dj-veryfi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-veryfi-0.1.4.tar", last modified: Sun Jul 16 00:30:48 2023, max compression
+gzip compressed data, was "dist/dj-veryfi-0.1.5.tar", last modified: Sun Jul 16 00:40:47 2023, max compression
```

## Comparing `dj-veryfi-0.1.4.tar` & `dj-veryfi-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/
--rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.4/LICENSE
--rw-r--r--   0 tony      (1000) tony      (1000)       66 2023-07-16 00:30:32.000000 dj-veryfi-0.1.4/MANIFEST.in
--rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     2884 2023-07-16 00:08:30.000000 dj-veryfi-0.1.4/README
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/dj_veryfi.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/dj_veryfi.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      294 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/dj_veryfi.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/dj_veryfi.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/dj_veryfi.egg-info/requires.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       11 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/dj_veryfi.egg-info/top_level.txt
--rw-r--r--   0 tony      (1000) tony      (1000)     1758 2023-07-15 22:01:27.000000 dj-veryfi-0.1.4/fields.py
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/migrations/
--rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.4/migrations/0001_initial.py
--rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.4/migrations/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)       88 2023-07-15 23:03:01.000000 dj-veryfi-0.1.4/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      694 2023-07-16 00:30:48.000000 dj-veryfi-0.1.4/setup.cfg
--rw-r--r--   0 tony      (1000) tony      (1000)       83 2023-07-16 00:10:10.000000 dj-veryfi-0.1.4/setup.py
--rw-r--r--   0 tony      (1000) tony      (1000)      398 2023-07-15 18:33:52.000000 dj-veryfi-0.1.4/veryfi.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/
+-rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.5/LICENSE
+-rw-r--r--   0 tony      (1000) tony      (1000)       66 2023-07-16 00:30:32.000000 dj-veryfi-0.1.5/MANIFEST.in
+-rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     2884 2023-07-16 00:08:30.000000 dj-veryfi-0.1.5/README
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      294 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/requires.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       11 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/top_level.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)     1758 2023-07-15 22:01:27.000000 dj-veryfi-0.1.5/fields.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/migrations/
+-rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.5/migrations/0001_initial.py
+-rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.5/migrations/__init__.py
+-rw-r--r--   0 tony      (1000) tony      (1000)       88 2023-07-15 23:03:01.000000 dj-veryfi-0.1.5/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      694 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/setup.cfg
+-rw-r--r--   0 tony      (1000) tony      (1000)       83 2023-07-16 00:10:10.000000 dj-veryfi-0.1.5/setup.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      398 2023-07-15 18:33:52.000000 dj-veryfi-0.1.5/veryfi.py
```

### Comparing `dj-veryfi-0.1.4/LICENSE` & `dj-veryfi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.4/PKG-INFO` & `dj-veryfi-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-veryfi-0.1.4/README` & `dj-veryfi-0.1.5/README`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.4/dj_veryfi.egg-info/PKG-INFO` & `dj-veryfi-0.1.5/dj_veryfi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-veryfi-0.1.4/fields.py` & `dj-veryfi-0.1.5/fields.py`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.4/migrations/0001_initial.py` & `dj-veryfi-0.1.5/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.4/setup.cfg` & `dj-veryfi-0.1.5/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-veryfi
-version = 0.1.4
+version = 0.1.5
 description = Django integration for Veryfi OCR API.
 long_description = file: README
 url = https://github.com/tonykamillo/dj-veryfi
 author = Tony Kamillo
 author_email = tonykamillo@gmail.com
 license = DBAD
 classifiers =
```

