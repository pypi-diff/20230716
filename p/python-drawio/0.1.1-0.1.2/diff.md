# Comparing `tmp/python-drawio-0.1.1.tar.gz` & `tmp/python-drawio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-drawio-0.1.1.tar", last modified: Sun Jul 16 15:57:40 2023, max compression
+gzip compressed data, was "python-drawio-0.1.2.tar", last modified: Sun Jul 16 16:16:47 2023, max compression
```

## Comparing `python-drawio-0.1.1.tar` & `python-drawio-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:57:40.902545 python-drawio-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-16 15:57:40.902545 python-drawio-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-16 15:57:27.000000 python-drawio-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 15:57:27.000000 python-drawio-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:57:40.902545 python-drawio-0.1.1/python_drawio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-16 15:57:40.000000 python-drawio-0.1.1/python_drawio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-16 15:57:40.000000 python-drawio-0.1.1/python_drawio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:57:40.000000 python-drawio-0.1.1/python_drawio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 15:57:40.000000 python-drawio-0.1.1/python_drawio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:57:40.902545 python-drawio-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-16 15:57:27.000000 python-drawio-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:57:40.898545 python-drawio-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:57:40.902545 python-drawio-0.1.1/src/python_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-16 15:57:27.000000 python-drawio-0.1.1/src/python_drawio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-16 15:57:27.000000 python-drawio-0.1.1/src/python_drawio/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-16 15:57:27.000000 python-drawio-0.1.1/src/python_drawio/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-16 15:57:27.000000 python-drawio-0.1.1/src/python_drawio/rectangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:16:47.982490 python-drawio-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-16 16:16:47.982490 python-drawio-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-16 16:16:34.000000 python-drawio-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 16:16:34.000000 python-drawio-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:16:47.982490 python-drawio-0.1.2/python_drawio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-16 16:16:47.000000 python-drawio-0.1.2/python_drawio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-16 16:16:47.000000 python-drawio-0.1.2/python_drawio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:16:47.000000 python-drawio-0.1.2/python_drawio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 16:16:47.000000 python-drawio-0.1.2/python_drawio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:16:47.982490 python-drawio-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-16 16:16:34.000000 python-drawio-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:16:47.982490 python-drawio-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:16:47.982490 python-drawio-0.1.2/src/python_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-16 16:16:34.000000 python-drawio-0.1.2/src/python_drawio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-16 16:16:34.000000 python-drawio-0.1.2/src/python_drawio/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-16 16:16:34.000000 python-drawio-0.1.2/src/python_drawio/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-16 16:16:34.000000 python-drawio-0.1.2/src/python_drawio/rectangle.py
```

### Comparing `python-drawio-0.1.1/setup.py` & `python-drawio-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='python-drawio',
-      version='0.1.1',
+      version='0.1.2',
       description='Draw.io, with Python',
-      long_description="long_description",
+      long_description=long_description,
+      long_description_content_type='text/markdown',
       author='Raphaël JOIE',
       author_email='info@widespot.be',
       url='https://github.com/widespot/python-drawio/',
       packages=['python_drawio'],
       package_dir={'python_drawio': 'src/python_drawio'},
       )
```

### Comparing `python-drawio-0.1.1/src/python_drawio/__init__.py` & `python-drawio-0.1.2/src/python_drawio/__init__.py`

 * *Files identical despite different names*

### Comparing `python-drawio-0.1.1/src/python_drawio/line.py` & `python-drawio-0.1.2/src/python_drawio/line.py`

 * *Files identical despite different names*

### Comparing `python-drawio-0.1.1/src/python_drawio/rectangle.py` & `python-drawio-0.1.2/src/python_drawio/rectangle.py`

 * *Files identical despite different names*

