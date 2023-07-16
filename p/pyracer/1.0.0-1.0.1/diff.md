# Comparing `tmp/pyracer-1.0.0.tar.gz` & `tmp/pyracer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracer-1.0.0.tar", last modified: Sun Jul 16 11:15:02 2023, max compression
+gzip compressed data, was "pyracer-1.0.1.tar", last modified: Sun Jul 16 15:52:10 2023, max compression
```

## Comparing `pyracer-1.0.0.tar` & `pyracer-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:15:02.270822 pyracer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-16 11:14:50.000000 pyracer-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-16 11:15:02.270822 pyracer-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:15:02.270822 pyracer-1.0.0/RACER/
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-07-16 11:14:50.000000 pyracer-1.0.0/RACER/RACER.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 11:14:50.000000 pyracer-1.0.0/RACER/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-16 11:14:50.000000 pyracer-1.0.0/RACER/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 11:14:50.000000 pyracer-1.0.0/RACER/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-16 11:14:50.000000 pyracer-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:15:02.270822 pyracer-1.0.0/pyracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-16 11:15:02.000000 pyracer-1.0.0/pyracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 11:15:02.000000 pyracer-1.0.0/pyracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:15:02.000000 pyracer-1.0.0/pyracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 11:15:02.000000 pyracer-1.0.0/pyracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 11:15:02.000000 pyracer-1.0.0/pyracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:15:02.270822 pyracer-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-16 11:14:50.000000 pyracer-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:52:10.535327 pyracer-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-16 15:52:00.000000 pyracer-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-16 15:52:10.535327 pyracer-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:52:10.531326 pyracer-1.0.1/RACER/
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/RACER.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-16 15:52:00.000000 pyracer-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:52:10.531326 pyracer-1.0.1/pyracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:52:10.535327 pyracer-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-16 15:52:00.000000 pyracer-1.0.1/setup.py
```

### Comparing `pyracer-1.0.0/LICENSE` & `pyracer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracer-1.0.0/PKG-INFO` & `pyracer-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
-Author: Adversarian
+Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyracer-1.0.0/RACER/RACER.py` & `pyracer-1.0.1/RACER/RACER.py`

 * *Files identical despite different names*

### Comparing `pyracer-1.0.0/RACER/preprocessing.py` & `pyracer-1.0.1/RACER/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyracer-1.0.0/pyracer.egg-info/PKG-INFO` & `pyracer-1.0.1/pyracer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
-Author: Adversarian
+Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyracer-1.0.0/setup.py` & `pyracer-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 setup(
     name="pyracer",
     packages=find_packages(),
     version=__version__,
     license="MIT",
     description="Unofficial Python implementation of the RACER classification algorithm.",
-    author="Adversarian",
+    author="Arian Tashakkor, Mohammad Safaiyan",
     author_email="a77physics@gmail.com",
     url="https://github.com/Adversarian/RACER",
     long_description_content_type="text/markdown",
     keywords=["machine learning", "classification", "RACER"],
     install_requires=[
         "numpy",
         "pandas",
```

