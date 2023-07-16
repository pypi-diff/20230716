# Comparing `tmp/noun-decomposition-0.0.5.tar.gz` & `tmp/noun-decomposition-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/noun-decomposition-0.0.5.tar", last modified: Sun Jul 16 13:32:58 2023, max compression
+gzip compressed data, was "dist/noun-decomposition-0.0.6.tar", last modified: Sun Jul 16 13:42:00 2023, max compression
```

## Comparing `noun-decomposition-0.0.5.tar` & `noun-decomposition-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.161073 noun-decomposition-0.0.5/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.5/LICENSE.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2505 2023-07-16 13:32:58.161162 noun-decomposition-0.0.5/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2030 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/README.md
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.157109 noun-decomposition-0.0.5/Secos/
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.159289 noun-decomposition-0.0.5/Secos/models/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/download.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      517 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/load.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/models.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.159679 noun-decomposition-0.0.5/Secos/utils/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/utils/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/utils/utils.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.160517 noun-decomposition-0.0.5/noun_decomposition.egg-info/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2505 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/SOURCES.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/dependency_links.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/requires.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/top_level.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 13:32:58.161481 noun-decomposition-0.0.5/setup.cfg
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 13:32:06.000000 noun-decomposition-0.0.5/setup.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.160671 noun-decomposition-0.0.5/tests/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.5/tests/test_decomposition.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:42:00.347532 noun-decomposition-0.0.6/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.6/LICENSE.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2505 2023-07-16 13:42:00.347628 noun-decomposition-0.0.6/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2030 2023-07-16 13:20:33.000000 noun-decomposition-0.0.6/README.md
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:42:00.343568 noun-decomposition-0.0.6/Secos/
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:42:00.345677 noun-decomposition-0.0.6/Secos/models/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-16 13:20:33.000000 noun-decomposition-0.0.6/Secos/models/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-16 13:20:33.000000 noun-decomposition-0.0.6/Secos/models/download.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      517 2023-07-16 13:20:33.000000 noun-decomposition-0.0.6/Secos/models/load.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-16 13:20:33.000000 noun-decomposition-0.0.6/Secos/models/models.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:42:00.346137 noun-decomposition-0.0.6/Secos/utils/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-16 13:20:33.000000 noun-decomposition-0.0.6/Secos/utils/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-16 13:20:33.000000 noun-decomposition-0.0.6/Secos/utils/utils.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:42:00.347017 noun-decomposition-0.0.6/noun_decomposition.egg-info/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2505 2023-07-16 13:42:00.000000 noun-decomposition-0.0.6/noun_decomposition.egg-info/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 13:42:00.000000 noun-decomposition-0.0.6/noun_decomposition.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:42:00.000000 noun-decomposition-0.0.6/noun_decomposition.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 13:42:00.000000 noun-decomposition-0.0.6/noun_decomposition.egg-info/requires.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:42:00.000000 noun-decomposition-0.0.6/noun_decomposition.egg-info/top_level.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 13:42:00.347939 noun-decomposition-0.0.6/setup.cfg
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 13:41:56.000000 noun-decomposition-0.0.6/setup.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:42:00.347210 noun-decomposition-0.0.6/tests/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.6/tests/test_decomposition.py
```

### Comparing `noun-decomposition-0.0.5/LICENSE.txt` & `noun-decomposition-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.5/PKG-INFO` & `noun-decomposition-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noun-decomposition
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python module to decompose nouns based on the SECOS algorithm
 Home-page: https://github.com/mhaugestad/noun-decomposition
 Author: Mathias Haugestad
 Author-email: mhaugestad@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.5.tar.gz
 Platform: UNKNOWN
```

### Comparing `noun-decomposition-0.0.5/README.md` & `noun-decomposition-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.5/Secos/models/download.py` & `noun-decomposition-0.0.6/Secos/models/download.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.5/Secos/models/load.py` & `noun-decomposition-0.0.6/Secos/models/load.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.5/Secos/models/models.py` & `noun-decomposition-0.0.6/Secos/models/models.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.5/Secos/utils/utils.py` & `noun-decomposition-0.0.6/Secos/utils/utils.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.5/noun_decomposition.egg-info/PKG-INFO` & `noun-decomposition-0.0.6/noun_decomposition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noun-decomposition
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python module to decompose nouns based on the SECOS algorithm
 Home-page: https://github.com/mhaugestad/noun-decomposition
 Author: Mathias Haugestad
 Author-email: mhaugestad@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.5.tar.gz
 Platform: UNKNOWN
```

### Comparing `noun-decomposition-0.0.5/setup.py` & `noun-decomposition-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="noun-decomposition",
-    version="0.0.5",
+    version="0.0.6",
     author="Mathias Haugestad",
     author_email="mhaugestad@gmail.com",
     description="Python module to decompose nouns based on the SECOS algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mhaugestad/noun-decomposition",
     packages=setuptools.find_packages(include=['Secos', 'Secos.*']),
```

### Comparing `noun-decomposition-0.0.5/tests/test_decomposition.py` & `noun-decomposition-0.0.6/tests/test_decomposition.py`

 * *Files identical despite different names*

