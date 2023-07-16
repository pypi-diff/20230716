# Comparing `tmp/noun-decomposition-0.0.3.tar.gz` & `tmp/noun-decomposition-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noun-decomposition-0.0.3.tar", last modified: Sun Jul 16 07:16:40 2023, max compression
+gzip compressed data, was "noun-decomposition-0.0.4.tar", last modified: Sun Jul 16 13:14:14 2023, max compression
```

## Comparing `noun-decomposition-0.0.3.tar` & `noun-decomposition-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.945878 noun-decomposition-0.0.3/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.3/LICENSE.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1874 2023-07-16 07:16:40.945965 noun-decomposition-0.0.3/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1435 2023-07-15 20:43:14.000000 noun-decomposition-0.0.3/README.md
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.940971 noun-decomposition-0.0.3/Secos/
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.943426 noun-decomposition-0.0.3/Secos/models/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/download.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      339 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/load.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/models.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.944117 noun-decomposition-0.0.3/Secos/utils/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/utils/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/utils/utils.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.945212 noun-decomposition-0.0.3/noun_decomposition.egg-info/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1874 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/SOURCES.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/dependency_links.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/requires.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/top_level.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 07:16:40.946276 noun-decomposition-0.0.3/setup.cfg
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 07:14:51.000000 noun-decomposition-0.0.3/setup.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.945431 noun-decomposition-0.0.3/tests/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.3/tests/test_decomposition.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.419647 noun-decomposition-0.0.4/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.4/LICENSE.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 13:14:14.419742 noun-decomposition-0.0.4/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2030 2023-07-16 11:24:10.000000 noun-decomposition-0.0.4/README.md
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.415390 noun-decomposition-0.0.4/Secos/
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.417702 noun-decomposition-0.0.4/Secos/models/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/models/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/models/download.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      517 2023-07-16 12:48:45.000000 noun-decomposition-0.0.4/Secos/models/load.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/models/models.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.418155 noun-decomposition-0.0.4/Secos/utils/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/utils/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/utils/utils.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.419198 noun-decomposition-0.0.4/noun_decomposition.egg-info/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/requires.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/top_level.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 13:14:14.420246 noun-decomposition-0.0.4/setup.cfg
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 12:49:46.000000 noun-decomposition-0.0.4/setup.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.419376 noun-decomposition-0.0.4/tests/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.4/tests/test_decomposition.py
```

### Comparing `noun-decomposition-0.0.3/LICENSE.txt` & `noun-decomposition-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.3/Secos/models/download.py` & `noun-decomposition-0.0.4/Secos/models/download.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.3/Secos/models/models.py` & `noun-decomposition-0.0.4/Secos/models/models.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.3/Secos/utils/utils.py` & `noun-decomposition-0.0.4/Secos/utils/utils.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.3/setup.py` & `noun-decomposition-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="noun-decomposition",
-    version="0.0.3",
+    version="0.0.4",
     author="Mathias Haugestad",
     author_email="mhaugestad@gmail.com",
     description="Python module to decompose nouns based on the SECOS algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mhaugestad/noun-decomposition",
     packages=setuptools.find_packages(include=['Secos', 'Secos.*']),
```

### Comparing `noun-decomposition-0.0.3/tests/test_decomposition.py` & `noun-decomposition-0.0.4/tests/test_decomposition.py`

 * *Files identical despite different names*

