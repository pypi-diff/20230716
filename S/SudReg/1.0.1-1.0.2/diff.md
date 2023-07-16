# Comparing `tmp/SudReg-1.0.1.tar.gz` & `tmp/SudReg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SudReg-1.0.1.tar", last modified: Sun Jul  9 17:07:42 2023, max compression
+gzip compressed data, was "SudReg-1.0.2.tar", last modified: Sun Jul 16 16:27:24 2023, max compression
```

## Comparing `SudReg-1.0.1.tar` & `SudReg-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:07:42.278518 SudReg-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-09 17:07:33.000000 SudReg-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-09 17:07:42.274518 SudReg-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-09 17:07:33.000000 SudReg-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:07:42.274518 SudReg-1.0.1/SudReg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-09 17:07:42.000000 SudReg-1.0.1/SudReg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-09 17:07:42.000000 SudReg-1.0.1/SudReg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:07:42.000000 SudReg-1.0.1/SudReg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 17:07:42.000000 SudReg-1.0.1/SudReg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 17:07:42.000000 SudReg-1.0.1/SudReg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:07:42.278518 SudReg-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-09 17:07:33.000000 SudReg-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:07:42.274518 SudReg-1.0.1/sudreg/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:07:33.000000 SudReg-1.0.1/sudreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15980 2023-07-09 17:07:33.000000 SudReg-1.0.1/sudreg/sudreg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:27:24.034063 SudReg-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-16 16:27:09.000000 SudReg-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-16 16:27:24.034063 SudReg-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-16 16:27:09.000000 SudReg-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:27:24.034063 SudReg-1.0.2/SudReg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-16 16:27:24.000000 SudReg-1.0.2/SudReg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-16 16:27:24.000000 SudReg-1.0.2/SudReg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:27:24.000000 SudReg-1.0.2/SudReg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 16:27:24.000000 SudReg-1.0.2/SudReg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 16:27:24.000000 SudReg-1.0.2/SudReg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:27:24.034063 SudReg-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-16 16:27:09.000000 SudReg-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:27:24.034063 SudReg-1.0.2/sudreg/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:27:09.000000 SudReg-1.0.2/sudreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33240 2023-07-16 16:27:09.000000 SudReg-1.0.2/sudreg/sudreg.py
```

### Comparing `SudReg-1.0.1/LICENSE.md` & `SudReg-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SudReg-1.0.1/setup.py` & `SudReg-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='SudReg',
-    version='1.0.1',
+    version='1.0.2',
     url='https://github.com/0xe20x8d0xbc/sudreg',
     author='Your Name',
     author_email='0xe20x8d0xbc@gmail.com',
     description='A light weight Python library for the SudReg Web API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

