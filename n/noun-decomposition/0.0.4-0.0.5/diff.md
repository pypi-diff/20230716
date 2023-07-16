# Comparing `tmp/noun-decomposition-0.0.4.tar.gz` & `tmp/noun-decomposition-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noun-decomposition-0.0.4.tar", last modified: Sun Jul 16 13:14:14 2023, max compression
+gzip compressed data, was "dist/noun-decomposition-0.0.5.tar", last modified: Sun Jul 16 13:32:58 2023, max compression
```

## Comparing `noun-decomposition-0.0.4.tar` & `noun-decomposition-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.419647 noun-decomposition-0.0.4/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.4/LICENSE.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 13:14:14.419742 noun-decomposition-0.0.4/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2030 2023-07-16 11:24:10.000000 noun-decomposition-0.0.4/README.md
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.415390 noun-decomposition-0.0.4/Secos/
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.417702 noun-decomposition-0.0.4/Secos/models/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/models/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/models/download.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      517 2023-07-16 12:48:45.000000 noun-decomposition-0.0.4/Secos/models/load.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/models/models.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.418155 noun-decomposition-0.0.4/Secos/utils/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/utils/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-15 21:11:41.000000 noun-decomposition-0.0.4/Secos/utils/utils.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.419198 noun-decomposition-0.0.4/noun_decomposition.egg-info/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/SOURCES.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/dependency_links.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/requires.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:14:14.000000 noun-decomposition-0.0.4/noun_decomposition.egg-info/top_level.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 13:14:14.420246 noun-decomposition-0.0.4/setup.cfg
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 12:49:46.000000 noun-decomposition-0.0.4/setup.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:14:14.419376 noun-decomposition-0.0.4/tests/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.4/tests/test_decomposition.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.161073 noun-decomposition-0.0.5/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.5/LICENSE.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2505 2023-07-16 13:32:58.161162 noun-decomposition-0.0.5/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2030 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/README.md
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.157109 noun-decomposition-0.0.5/Secos/
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.159289 noun-decomposition-0.0.5/Secos/models/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/download.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      517 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/load.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/models/models.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.159679 noun-decomposition-0.0.5/Secos/utils/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/utils/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-16 13:20:33.000000 noun-decomposition-0.0.5/Secos/utils/utils.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.160517 noun-decomposition-0.0.5/noun_decomposition.egg-info/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2505 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/requires.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:32:58.000000 noun-decomposition-0.0.5/noun_decomposition.egg-info/top_level.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 13:32:58.161481 noun-decomposition-0.0.5/setup.cfg
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 13:32:06.000000 noun-decomposition-0.0.5/setup.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:32:58.160671 noun-decomposition-0.0.5/tests/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.5/tests/test_decomposition.py
```

### Comparing `noun-decomposition-0.0.4/LICENSE.txt` & `noun-decomposition-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.4/PKG-INFO` & `noun-decomposition-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: noun-decomposition
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python module to decompose nouns based on the SECOS algorithm
 Home-page: https://github.com/mhaugestad/noun-decomposition
-Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.3.tar.gz
 Author: Mathias Haugestad
 Author-email: mhaugestad@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.5.tar.gz
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SECOS
 This repo is a modular python implementation of the SECOS algorithm for decomposing composite nouns.
 
@@ -83,7 +85,8 @@
 secos.decompose("Bundesfinanzministerium")
 
 ['bundes', 'finanz', 'ministerium']
 ```
 
 # Evaluation
 The evaluation folder in the github repo includes code for the evaluation of the pretrained models.
+
```

### Comparing `noun-decomposition-0.0.4/README.md` & `noun-decomposition-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.4/Secos/models/download.py` & `noun-decomposition-0.0.5/Secos/models/download.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.4/Secos/models/load.py` & `noun-decomposition-0.0.5/Secos/models/load.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.4/Secos/models/models.py` & `noun-decomposition-0.0.5/Secos/models/models.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.4/Secos/utils/utils.py` & `noun-decomposition-0.0.5/Secos/utils/utils.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.4/noun_decomposition.egg-info/PKG-INFO` & `noun-decomposition-0.0.5/noun_decomposition.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: noun-decomposition
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python module to decompose nouns based on the SECOS algorithm
 Home-page: https://github.com/mhaugestad/noun-decomposition
-Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.3.tar.gz
 Author: Mathias Haugestad
 Author-email: mhaugestad@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.5.tar.gz
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SECOS
 This repo is a modular python implementation of the SECOS algorithm for decomposing composite nouns.
 
@@ -83,7 +85,8 @@
 secos.decompose("Bundesfinanzministerium")
 
 ['bundes', 'finanz', 'ministerium']
 ```
 
 # Evaluation
 The evaluation folder in the github repo includes code for the evaluation of the pretrained models.
+
```

### Comparing `noun-decomposition-0.0.4/setup.py` & `noun-decomposition-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="noun-decomposition",
-    version="0.0.4",
+    version="0.0.5",
     author="Mathias Haugestad",
     author_email="mhaugestad@gmail.com",
     description="Python module to decompose nouns based on the SECOS algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mhaugestad/noun-decomposition",
     packages=setuptools.find_packages(include=['Secos', 'Secos.*']),
     install_requires=['scipy', 'numpy', 'pytest', 'importlib-resources', 'requests', 'tqdm'],
     python_requires='>=3.6',
-    download_url='https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.3.tar.gz'
+    download_url='https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.5.tar.gz'
 )
```

### Comparing `noun-decomposition-0.0.4/tests/test_decomposition.py` & `noun-decomposition-0.0.5/tests/test_decomposition.py`

 * *Files identical despite different names*

