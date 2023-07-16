# Comparing `tmp/tychos-0.0.8.tar.gz` & `tmp/tychos-0.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.8.tar", last modified: Sun Jul 16 14:47:19 2023, max compression
+gzip compressed data, was "tychos-0.0.89.tar", last modified: Sun Jul 16 14:40:21 2023, max compression
```

## Comparing `tychos-0.0.8.tar` & `tychos-0.0.89.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:47:19.205722 tychos-0.0.8/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.8/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)     2774 2023-07-16 14:47:19.205538 tychos-0.0.8/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)     2587 2023-07-16 14:16:28.000000 tychos-0.0.8/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-16 14:47:19.205766 tychos-0.0.8/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-16 14:45:53.000000 tychos-0.0.8/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:47:19.203889 tychos-0.0.8/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.8/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.8/tychos/cli.py
--rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.8/tychos/config.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:47:19.205355 tychos-0.0.8/tychos/helpers/
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.8/tychos/helpers/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1553 2023-07-16 14:30:04.000000 tychos-0.0.8/tychos/vector.py
--rw-r--r--   0 abe732     (501) staff       (20)     1732 2023-07-16 14:30:02.000000 tychos-0.0.8/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:47:19.205207 tychos-0.0.8/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)     2774 2023-07-16 14:47:19.000000 tychos-0.0.8/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      330 2023-07-16 14:47:19.000000 tychos-0.0.8/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-16 14:47:19.000000 tychos-0.0.8/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-16 14:47:19.000000 tychos-0.0.8/tychos.egg-info/entry_points.txt
--rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-16 14:47:19.000000 tychos-0.0.8/tychos.egg-info/requires.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-16 14:47:19.000000 tychos-0.0.8/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.162263 tychos-0.0.89/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.89/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)     2775 2023-07-16 14:40:21.162033 tychos-0.0.89/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)     2587 2023-07-16 14:16:28.000000 tychos-0.0.89/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-16 14:40:21.162320 tychos-0.0.89/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      503 2023-07-16 14:39:53.000000 tychos-0.0.89/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.160331 tychos-0.0.89/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.89/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.89/tychos/cli.py
+-rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.89/tychos/config.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.161763 tychos-0.0.89/tychos/helpers/
+-rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.89/tychos/helpers/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1553 2023-07-16 14:30:04.000000 tychos-0.0.89/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1732 2023-07-16 14:30:02.000000 tychos-0.0.89/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.161522 tychos-0.0.89/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)     2775 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      330 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/entry_points.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.8/LICENSE` & `tychos-0.0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.0.8/PKG-INFO` & `tychos-0.0.89/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.8
+Version: 0.0.89
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
```

### Comparing `tychos-0.0.8/README.md` & `tychos-0.0.89/README.md`

 * *Files identical despite different names*

### Comparing `tychos-0.0.8/tychos/cli.py` & `tychos-0.0.89/tychos/cli.py`

 * *Files identical despite different names*

### Comparing `tychos-0.0.8/tychos/vector.py` & `tychos-0.0.89/tychos/vector.py`

 * *Files identical despite different names*

### Comparing `tychos-0.0.8/tychos/vector_data_store.py` & `tychos-0.0.89/tychos/vector_data_store.py`

 * *Files identical despite different names*

### Comparing `tychos-0.0.8/tychos.egg-info/PKG-INFO` & `tychos-0.0.89/tychos.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.8
+Version: 0.0.89
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
```

