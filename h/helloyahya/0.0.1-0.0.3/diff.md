# Comparing `tmp/helloyahya-0.0.1.tar.gz` & `tmp/helloyahya-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helloyahya-0.0.1.tar", last modified: Sat Jul 15 22:41:37 2023, max compression
+gzip compressed data, was "helloyahya-0.0.3.tar", last modified: Sat Jul 15 19:14:39 2023, max compression
```

## Comparing `helloyahya-0.0.1.tar` & `helloyahya-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 yahyaali   (501) staff       (20)        0 2023-07-15 22:41:37.743291 helloyahya-0.0.1/
--rw-r--r--   0 yahyaali   (501) staff       (20)      493 2023-07-15 22:41:37.741323 helloyahya-0.0.1/PKG-INFO
--rw-r--r--   0 yahyaali   (501) staff       (20)       18 2023-07-15 22:16:27.000000 helloyahya-0.0.1/README.md
-drwxr-xr-x   0 yahyaali   (501) staff       (20)        0 2023-07-15 22:41:37.734010 helloyahya-0.0.1/helloPackage/
--rw-r--r--   0 yahyaali   (501) staff       (20)       63 2023-07-15 22:16:27.000000 helloyahya-0.0.1/helloPackage/HelloYahya.py
--rw-r--r--   0 yahyaali   (501) staff       (20)        0 2023-07-15 22:33:04.000000 helloyahya-0.0.1/helloPackage/__init__.py
-drwxr-xr-x   0 yahyaali   (501) staff       (20)        0 2023-07-15 22:41:37.738791 helloyahya-0.0.1/helloyahya.egg-info/
--rw-r--r--   0 yahyaali   (501) staff       (20)      493 2023-07-15 22:41:37.000000 helloyahya-0.0.1/helloyahya.egg-info/PKG-INFO
--rw-r--r--   0 yahyaali   (501) staff       (20)      206 2023-07-15 22:41:37.000000 helloyahya-0.0.1/helloyahya.egg-info/SOURCES.txt
--rw-r--r--   0 yahyaali   (501) staff       (20)        1 2023-07-15 22:41:37.000000 helloyahya-0.0.1/helloyahya.egg-info/dependency_links.txt
--rw-r--r--   0 yahyaali   (501) staff       (20)       13 2023-07-15 22:41:37.000000 helloyahya-0.0.1/helloyahya.egg-info/top_level.txt
--rw-r--r--   0 yahyaali   (501) staff       (20)       38 2023-07-15 22:41:37.743524 helloyahya-0.0.1/setup.cfg
--rw-r--r--   0 yahyaali   (501) staff       (20)      791 2023-07-15 22:41:30.000000 helloyahya-0.0.1/setup.py
+drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 19:14:39.847414 helloyahya-0.0.3/
+-rw-r--r--   0 noorhashem   (501) staff       (20)      550 2023-07-15 19:14:39.847279 helloyahya-0.0.3/PKG-INFO
+drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 19:14:39.846301 helloyahya-0.0.3/helloyahya/
+-rw-r--r--   0 noorhashem   (501) staff       (20)       34 2023-07-15 19:13:29.000000 helloyahya-0.0.3/helloyahya/__init__.py
+-rw-r--r--   0 noorhashem   (501) staff       (20)       62 2023-07-15 19:11:30.000000 helloyahya-0.0.3/helloyahya/hello.py
+drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 19:14:39.847075 helloyahya-0.0.3/helloyahya.egg-info/
+-rw-r--r--   0 noorhashem   (501) staff       (20)      550 2023-07-15 19:14:39.000000 helloyahya-0.0.3/helloyahya.egg-info/PKG-INFO
+-rw-r--r--   0 noorhashem   (501) staff       (20)      187 2023-07-15 19:14:39.000000 helloyahya-0.0.3/helloyahya.egg-info/SOURCES.txt
+-rw-r--r--   0 noorhashem   (501) staff       (20)        1 2023-07-15 19:14:39.000000 helloyahya-0.0.3/helloyahya.egg-info/dependency_links.txt
+-rw-r--r--   0 noorhashem   (501) staff       (20)       11 2023-07-15 19:14:39.000000 helloyahya-0.0.3/helloyahya.egg-info/top_level.txt
+-rw-r--r--   0 noorhashem   (501) staff       (20)       38 2023-07-15 19:14:39.847466 helloyahya-0.0.3/setup.cfg
+-rw-r--r--   0 noorhashem   (501) staff       (20)      794 2023-07-15 19:13:00.000000 helloyahya-0.0.3/setup.py
```

### Comparing `helloyahya-0.0.1/setup.py` & `helloyahya-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.3'
 DESCRIPTION = 'Saying hi to Yahya'
 LONG_DESCRIPTION = 'Saying hi to Yahya'
 
 # Setting up
 setup(
     name="helloyahya",
     version=VERSION,
-    author="Yahya Ali",
-    author_email="yahya.ali97@outlook.com",
+    author="Noor Hashem",
+    author_email="noor.hashem@hotmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

