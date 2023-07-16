# Comparing `tmp/noun-decomposition-0.0.2.tar.gz` & `tmp/noun-decomposition-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/noun-decomposition-0.0.2.tar", last modified: Mon Jul 10 22:00:57 2023, max compression
+gzip compressed data, was "noun-decomposition-0.0.3.tar", last modified: Sun Jul 16 07:16:40 2023, max compression
```

## Comparing `noun-decomposition-0.0.2.tar` & `noun-decomposition-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-10 22:00:57.401471 noun-decomposition-0.0.2/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.2/LICENSE.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1621 2023-07-10 22:00:57.401560 noun-decomposition-0.0.2/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1146 2023-07-10 21:53:58.000000 noun-decomposition-0.0.2/README.md
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-10 22:00:57.398289 noun-decomposition-0.0.2/Secos/
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-10 22:00:57.399913 noun-decomposition-0.0.2/Secos/models/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-06-05 20:37:48.000000 noun-decomposition-0.0.2/Secos/models/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-03 19:48:53.000000 noun-decomposition-0.0.2/Secos/models/download.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      339 2023-07-10 21:54:13.000000 noun-decomposition-0.0.2/Secos/models/load.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-06-05 18:46:05.000000 noun-decomposition-0.0.2/Secos/models/models.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-10 22:00:57.400327 noun-decomposition-0.0.2/Secos/utils/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-06-03 17:18:21.000000 noun-decomposition-0.0.2/Secos/utils/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-06-10 04:47:28.000000 noun-decomposition-0.0.2/Secos/utils/utils.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-10 22:00:57.401172 noun-decomposition-0.0.2/noun_decomposition.egg-info/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1621 2023-07-10 22:00:57.000000 noun-decomposition-0.0.2/noun_decomposition.egg-info/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-10 22:00:57.000000 noun-decomposition-0.0.2/noun_decomposition.egg-info/SOURCES.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-10 22:00:57.000000 noun-decomposition-0.0.2/noun_decomposition.egg-info/dependency_links.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-10 22:00:57.000000 noun-decomposition-0.0.2/noun_decomposition.egg-info/requires.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-10 22:00:57.000000 noun-decomposition-0.0.2/noun_decomposition.egg-info/top_level.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-10 22:00:57.401855 noun-decomposition-0.0.2/setup.cfg
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-10 22:00:39.000000 noun-decomposition-0.0.2/setup.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-10 22:00:57.401331 noun-decomposition-0.0.2/tests/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.2/tests/test_decomposition.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.945878 noun-decomposition-0.0.3/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.3/LICENSE.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1874 2023-07-16 07:16:40.945965 noun-decomposition-0.0.3/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1435 2023-07-15 20:43:14.000000 noun-decomposition-0.0.3/README.md
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.940971 noun-decomposition-0.0.3/Secos/
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.943426 noun-decomposition-0.0.3/Secos/models/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/download.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      339 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/load.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/models/models.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.944117 noun-decomposition-0.0.3/Secos/utils/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/utils/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-15 21:11:41.000000 noun-decomposition-0.0.3/Secos/utils/utils.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.945212 noun-decomposition-0.0.3/noun_decomposition.egg-info/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1874 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/requires.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 07:16:40.000000 noun-decomposition-0.0.3/noun_decomposition.egg-info/top_level.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 07:16:40.946276 noun-decomposition-0.0.3/setup.cfg
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 07:14:51.000000 noun-decomposition-0.0.3/setup.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 07:16:40.945431 noun-decomposition-0.0.3/tests/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.3/tests/test_decomposition.py
```

### Comparing `noun-decomposition-0.0.2/LICENSE.txt` & `noun-decomposition-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.2/PKG-INFO` & `noun-decomposition-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: noun-decomposition
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python module to decompose nouns based on the SECOS algorithm
 Home-page: https://github.com/mhaugestad/noun-decomposition
+Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.3.tar.gz
 Author: Mathias Haugestad
 Author-email: mhaugestad@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.2.tar.gz
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SECOS
 This repo is a modular python implementation of the SECOS algorithm for decomposing composite nouns.
 
@@ -37,33 +35,49 @@
 ```
 pip install noun-decomposition
 ```
 
 ## Installing models:
 The module relies on pretrained models to be passed in. These can be downloaded from command line as follows:
 
-`python -m Secos download --model german`
+`python -m Secos download --model de`
 
 Or from a python script or notebook like this:
 
 ```
 from secos import Decomposition
 
-Decomposition.download_model('german')
+Decomposition.download_model('de')
 ```
 
+Available models and their names are:
+
+| Language  | Model |
+| ------------- | ------------- |
+| Danish | da |
+| German | de |
+| English | en |
+| Spanish | es |
+| Estonian | et |
+| Finnish | fi |
+| Hungarian | hu |
+| Latin | la |
+| Latvian | lv |
+| Netherland | nl |
+| Norway | no |
+| Swedish | sv |
+
 # Basic Usage
 ```
 from secos import Decomposition
 
-model = Decomposition.load_model('german')
+model = Decomposition.load_model('de')
 
 secos = Decomposition(model)
 
 secos.decompose("Bundesfinanzministerium")
 
-['Bundes', 'finanz', 'ministerium']
+['bundes', 'finanz', 'ministerium']
 ```
 
 # Evaluation
 The evaluation folder includes code for the evaluation of the pretrained models.
-
```

### Comparing `noun-decomposition-0.0.2/README.md` & `noun-decomposition-0.0.3/noun_decomposition.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: noun-decomposition
+Version: 0.0.3
+Summary: Python module to decompose nouns based on the SECOS algorithm
+Home-page: https://github.com/mhaugestad/noun-decomposition
+Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.3.tar.gz
+Author: Mathias Haugestad
+Author-email: mhaugestad@gmail.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # SECOS
 This repo is a modular python implementation of the SECOS algorithm for decomposing composite nouns.
 
 Based on the SECOS algorithm:
 
 [original implementation](https://github.com/riedlma/SECOS)
 
@@ -23,32 +35,49 @@
 ```
 pip install noun-decomposition
 ```
 
 ## Installing models:
 The module relies on pretrained models to be passed in. These can be downloaded from command line as follows:
 
-`python -m Secos download --model german`
+`python -m Secos download --model de`
 
 Or from a python script or notebook like this:
 
 ```
 from secos import Decomposition
 
-Decomposition.download_model('german')
+Decomposition.download_model('de')
 ```
 
+Available models and their names are:
+
+| Language  | Model |
+| ------------- | ------------- |
+| Danish | da |
+| German | de |
+| English | en |
+| Spanish | es |
+| Estonian | et |
+| Finnish | fi |
+| Hungarian | hu |
+| Latin | la |
+| Latvian | lv |
+| Netherland | nl |
+| Norway | no |
+| Swedish | sv |
+
 # Basic Usage
 ```
 from secos import Decomposition
 
-model = Decomposition.load_model('german')
+model = Decomposition.load_model('de')
 
 secos = Decomposition(model)
 
 secos.decompose("Bundesfinanzministerium")
 
-['Bundes', 'finanz', 'ministerium']
+['bundes', 'finanz', 'ministerium']
 ```
 
 # Evaluation
-The evaluation folder includes code for the evaluation of the pretrained models.
+The evaluation folder includes code for the evaluation of the pretrained models.
```

### Comparing `noun-decomposition-0.0.2/Secos/models/download.py` & `noun-decomposition-0.0.3/Secos/models/download.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.2/Secos/models/models.py` & `noun-decomposition-0.0.3/Secos/models/models.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.2/Secos/utils/utils.py` & `noun-decomposition-0.0.3/Secos/utils/utils.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.2/setup.py` & `noun-decomposition-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="noun-decomposition",
-    version="0.0.2",
+    version="0.0.3",
     author="Mathias Haugestad",
     author_email="mhaugestad@gmail.com",
     description="Python module to decompose nouns based on the SECOS algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mhaugestad/noun-decomposition",
     packages=setuptools.find_packages(include=['Secos', 'Secos.*']),
     install_requires=['scipy', 'numpy', 'pytest', 'importlib-resources', 'requests', 'tqdm'],
     python_requires='>=3.6',
-    download_url='https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.2.tar.gz'
+    download_url='https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.3.tar.gz'
 )
```

### Comparing `noun-decomposition-0.0.2/tests/test_decomposition.py` & `noun-decomposition-0.0.3/tests/test_decomposition.py`

 * *Files identical despite different names*

