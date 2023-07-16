# Comparing `tmp/noun-decomposition-0.0.7.tar.gz` & `tmp/noun-decomposition-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noun-decomposition-0.0.7.tar", last modified: Sun Jul 16 13:48:32 2023, max compression
+gzip compressed data, was "noun-decomposition-0.0.8.tar", last modified: Sun Jul 16 14:23:49 2023, max compression
```

## Comparing `noun-decomposition-0.0.7.tar` & `noun-decomposition-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:48:32.670043 noun-decomposition-0.0.7/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.7/LICENSE.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 13:48:32.670129 noun-decomposition-0.0.7/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2030 2023-07-16 13:20:33.000000 noun-decomposition-0.0.7/README.md
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:48:32.666061 noun-decomposition-0.0.7/Secos/
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:48:32.668158 noun-decomposition-0.0.7/Secos/models/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-16 13:20:33.000000 noun-decomposition-0.0.7/Secos/models/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-16 13:20:33.000000 noun-decomposition-0.0.7/Secos/models/download.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      517 2023-07-16 13:20:33.000000 noun-decomposition-0.0.7/Secos/models/load.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-16 13:20:33.000000 noun-decomposition-0.0.7/Secos/models/models.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:48:32.668689 noun-decomposition-0.0.7/Secos/utils/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-16 13:20:33.000000 noun-decomposition-0.0.7/Secos/utils/__init__.py
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-16 13:20:33.000000 noun-decomposition-0.0.7/Secos/utils/utils.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:48:32.669549 noun-decomposition-0.0.7/noun_decomposition.egg-info/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 13:48:32.000000 noun-decomposition-0.0.7/noun_decomposition.egg-info/PKG-INFO
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      416 2023-07-16 13:48:32.000000 noun-decomposition-0.0.7/noun_decomposition.egg-info/SOURCES.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:48:32.000000 noun-decomposition-0.0.7/noun_decomposition.egg-info/dependency_links.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 13:48:32.000000 noun-decomposition-0.0.7/noun_decomposition.egg-info/requires.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 13:48:32.000000 noun-decomposition-0.0.7/noun_decomposition.egg-info/top_level.txt
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 13:48:32.670451 noun-decomposition-0.0.7/setup.cfg
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 13:48:18.000000 noun-decomposition-0.0.7/setup.py
-drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 13:48:32.669759 noun-decomposition-0.0.7/tests/
--rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.7/tests/test_decomposition.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 14:23:49.810967 noun-decomposition-0.0.8/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)    11356 2023-07-10 14:38:44.000000 noun-decomposition-0.0.8/LICENSE.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 14:23:49.811058 noun-decomposition-0.0.8/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2030 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/README.md
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 14:23:49.810139 noun-decomposition-0.0.8/Secos/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     3274 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/Decomposition.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       40 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      754 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/__main__.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 14:23:49.807987 noun-decomposition-0.0.8/Secos/models/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       92 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/models/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1200 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/models/download.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      517 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/models/load.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1393 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/models/models.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 14:23:49.808521 noun-decomposition-0.0.8/Secos/utils/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       68 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/utils/__init__.py
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2087 2023-07-16 13:20:33.000000 noun-decomposition-0.0.8/Secos/utils/utils.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 14:23:49.809456 noun-decomposition-0.0.8/noun_decomposition.egg-info/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     2469 2023-07-16 14:23:49.000000 noun-decomposition-0.0.8/noun_decomposition.egg-info/PKG-INFO
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      614 2023-07-16 14:23:49.000000 noun-decomposition-0.0.8/noun_decomposition.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        1 2023-07-16 14:23:49.000000 noun-decomposition-0.0.8/noun_decomposition.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       53 2023-07-16 14:23:49.000000 noun-decomposition-0.0.8/noun_decomposition.egg-info/requires.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)        6 2023-07-16 14:23:49.000000 noun-decomposition-0.0.8/noun_decomposition.egg-info/top_level.txt
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)       79 2023-07-16 14:23:49.811410 noun-decomposition-0.0.8/setup.cfg
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)      812 2023-07-16 14:22:46.000000 noun-decomposition-0.0.8/setup.py
+drwxr-xr-x   0 mathiashaugestad   (501) staff       (20)        0 2023-07-16 14:23:49.810564 noun-decomposition-0.0.8/tests/
+-rw-r--r--   0 mathiashaugestad   (501) staff       (20)     1085 2023-06-10 06:03:57.000000 noun-decomposition-0.0.8/tests/test_decomposition.py
```

### Comparing `noun-decomposition-0.0.7/LICENSE.txt` & `noun-decomposition-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.7/PKG-INFO` & `noun-decomposition-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: noun-decomposition
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python module to decompose nouns based on the SECOS algorithm
 Home-page: https://github.com/mhaugestad/noun-decomposition
-Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.7.tar.gz
+Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.8.tar.gz
 Author: Mathias Haugestad
 Author-email: mhaugestad@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SECOS
```

### Comparing `noun-decomposition-0.0.7/README.md` & `noun-decomposition-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.7/Secos/models/download.py` & `noun-decomposition-0.0.8/Secos/models/download.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.7/Secos/models/load.py` & `noun-decomposition-0.0.8/Secos/models/load.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.7/Secos/models/models.py` & `noun-decomposition-0.0.8/Secos/models/models.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.7/Secos/utils/utils.py` & `noun-decomposition-0.0.8/Secos/utils/utils.py`

 * *Files identical despite different names*

### Comparing `noun-decomposition-0.0.7/noun_decomposition.egg-info/PKG-INFO` & `noun-decomposition-0.0.8/noun_decomposition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: noun-decomposition
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python module to decompose nouns based on the SECOS algorithm
 Home-page: https://github.com/mhaugestad/noun-decomposition
-Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.7.tar.gz
+Download-URL: https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.8.tar.gz
 Author: Mathias Haugestad
 Author-email: mhaugestad@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SECOS
```

### Comparing `noun-decomposition-0.0.7/setup.py` & `noun-decomposition-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="noun-decomposition",
-    version="0.0.7",
+    version="0.0.8",
     author="Mathias Haugestad",
     author_email="mhaugestad@gmail.com",
     description="Python module to decompose nouns based on the SECOS algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mhaugestad/noun-decomposition",
-    packages=setuptools.find_packages(include=['Secos', 'Secos.*']),
+    packages=setuptools.find_packages(include=['secos', 'secos.*']),
     install_requires=['scipy', 'numpy', 'pytest', 'importlib-resources', 'requests', 'tqdm'],
     python_requires='>=3.6',
-    download_url='https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.7.tar.gz'
+    download_url='https://github.com/mhaugestad/noun-decomposition/archive/refs/tags/0.0.8.tar.gz'
 )
```

### Comparing `noun-decomposition-0.0.7/tests/test_decomposition.py` & `noun-decomposition-0.0.8/tests/test_decomposition.py`

 * *Files identical despite different names*

