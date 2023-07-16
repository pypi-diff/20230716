# Comparing `tmp/ppyNotion-0.0.1.1.tar.gz` & `tmp/ppyNotion-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppyNotion-0.0.1.1.tar", last modified: Sun Jul 16 08:52:43 2023, max compression
+gzip compressed data, was "ppyNotion-0.0.2.1.tar", last modified: Sun Jul 16 09:01:47 2023, max compression
```

## Comparing `ppyNotion-0.0.1.1.tar` & `ppyNotion-0.0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jirayuwat   (501) staff       (20)        0 2023-07-16 08:52:43.814522 ppyNotion-0.0.1.1/
--rw-r--r--   0 jirayuwat   (501) staff       (20)    35149 2023-07-16 07:39:09.000000 ppyNotion-0.0.1.1/LICENSE
--rw-r--r--   0 jirayuwat   (501) staff       (20)      572 2023-07-16 08:52:43.814396 ppyNotion-0.0.1.1/PKG-INFO
--rw-r--r--   0 jirayuwat   (501) staff       (20)      144 2023-07-16 08:41:12.000000 ppyNotion-0.0.1.1/README.md
-drwxr-xr-x   0 jirayuwat   (501) staff       (20)        0 2023-07-16 08:52:43.813635 ppyNotion-0.0.1.1/code/
--rw-r--r--   0 jirayuwat   (501) staff       (20)        0 2023-07-16 08:37:52.000000 ppyNotion-0.0.1.1/code/__init__.py
-drwxr-xr-x   0 jirayuwat   (501) staff       (20)        0 2023-07-16 08:52:43.814217 ppyNotion-0.0.1.1/ppyNotion.egg-info/
--rw-r--r--   0 jirayuwat   (501) staff       (20)      572 2023-07-16 08:52:43.000000 ppyNotion-0.0.1.1/ppyNotion.egg-info/PKG-INFO
--rw-r--r--   0 jirayuwat   (501) staff       (20)      175 2023-07-16 08:52:43.000000 ppyNotion-0.0.1.1/ppyNotion.egg-info/SOURCES.txt
--rw-r--r--   0 jirayuwat   (501) staff       (20)        1 2023-07-16 08:52:43.000000 ppyNotion-0.0.1.1/ppyNotion.egg-info/dependency_links.txt
--rw-r--r--   0 jirayuwat   (501) staff       (20)        5 2023-07-16 08:52:43.000000 ppyNotion-0.0.1.1/ppyNotion.egg-info/top_level.txt
--rw-r--r--   0 jirayuwat   (501) staff       (20)       38 2023-07-16 08:52:43.814572 ppyNotion-0.0.1.1/setup.cfg
--rw-r--r--   0 jirayuwat   (501) staff       (20)      637 2023-07-16 08:52:40.000000 ppyNotion-0.0.1.1/setup.py
+drwxr-xr-x   0 jirayuwat   (501) staff       (20)        0 2023-07-16 09:01:47.731827 ppyNotion-0.0.2.1/
+-rw-r--r--   0 jirayuwat   (501) staff       (20)    35149 2023-07-16 07:39:09.000000 ppyNotion-0.0.2.1/LICENSE
+-rw-r--r--   0 jirayuwat   (501) staff       (20)      572 2023-07-16 09:01:47.731709 ppyNotion-0.0.2.1/PKG-INFO
+-rw-r--r--   0 jirayuwat   (501) staff       (20)      144 2023-07-16 08:41:12.000000 ppyNotion-0.0.2.1/README.md
+drwxr-xr-x   0 jirayuwat   (501) staff       (20)        0 2023-07-16 09:01:47.731047 ppyNotion-0.0.2.1/code/
+-rw-r--r--   0 jirayuwat   (501) staff       (20)        0 2023-07-16 08:37:52.000000 ppyNotion-0.0.2.1/code/__init__.py
+drwxr-xr-x   0 jirayuwat   (501) staff       (20)        0 2023-07-16 09:01:47.731539 ppyNotion-0.0.2.1/ppyNotion.egg-info/
+-rw-r--r--   0 jirayuwat   (501) staff       (20)      572 2023-07-16 09:01:47.000000 ppyNotion-0.0.2.1/ppyNotion.egg-info/PKG-INFO
+-rw-r--r--   0 jirayuwat   (501) staff       (20)      175 2023-07-16 09:01:47.000000 ppyNotion-0.0.2.1/ppyNotion.egg-info/SOURCES.txt
+-rw-r--r--   0 jirayuwat   (501) staff       (20)        1 2023-07-16 09:01:47.000000 ppyNotion-0.0.2.1/ppyNotion.egg-info/dependency_links.txt
+-rw-r--r--   0 jirayuwat   (501) staff       (20)        5 2023-07-16 09:01:47.000000 ppyNotion-0.0.2.1/ppyNotion.egg-info/top_level.txt
+-rw-r--r--   0 jirayuwat   (501) staff       (20)       38 2023-07-16 09:01:47.731872 ppyNotion-0.0.2.1/setup.cfg
+-rw-r--r--   0 jirayuwat   (501) staff       (20)      637 2023-07-16 08:54:02.000000 ppyNotion-0.0.2.1/setup.py
```

### Comparing `ppyNotion-0.0.1.1/LICENSE` & `ppyNotion-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ppyNotion-0.0.1.1/PKG-INFO` & `ppyNotion-0.0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppyNotion
-Version: 0.0.1.1
+Version: 0.0.2.1
 Summary: Connect to your Notion database with ease.
 Home-page: https://github.com/jirayuwat12/ppyNotion
 Author: jirayuwat b.
 Author-email: jirayuwat.work@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ppyNotion-0.0.1.1/ppyNotion.egg-info/PKG-INFO` & `ppyNotion-0.0.2.1/ppyNotion.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppyNotion
-Version: 0.0.1.1
+Version: 0.0.2.1
 Summary: Connect to your Notion database with ease.
 Home-page: https://github.com/jirayuwat12/ppyNotion
 Author: jirayuwat b.
 Author-email: jirayuwat.work@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ppyNotion-0.0.1.1/setup.py` & `ppyNotion-0.0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ppyNotion",
-    version="0.0.1.1",
+    version="0.0.2.1",
     author="jirayuwat b.",
     author_email="jirayuwat.work@gmail.com",
     description="Connect to your Notion database with ease.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jirayuwat12/ppyNotion",
     packages=setuptools.find_packages(),
```

