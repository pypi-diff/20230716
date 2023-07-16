# Comparing `tmp/lossers-0.0.7.tar.gz` & `tmp/lossers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lossers-0.0.7.tar", last modified: Sat Apr 22 00:17:05 2023, max compression
+gzip compressed data, was "lossers-0.0.8.tar", last modified: Sun Jul 16 04:39:10 2023, max compression
```

## Comparing `lossers-0.0.7.tar` & `lossers-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 00:16:50.000000 lossers-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-22 00:17:05.802178 lossers-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-22 00:16:50.000000 lossers-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/lossers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/lossers/lpips/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/vgg_v0.1.pth
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/lossers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:17:05.802178 lossers-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-22 00:16:50.000000 lossers-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.483449 lossers-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 04:38:59.000000 lossers-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 04:39:10.483449 lossers-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 04:38:59.000000 lossers-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.479449 lossers-0.0.8/lossers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.483449 lossers-0.0.8/lossers/lpips/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/vgg_v0.1.pth
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.483449 lossers-0.0.8/lossers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:39:10.483449 lossers-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-16 04:38:59.000000 lossers-0.0.8/setup.py
```

### Comparing `lossers-0.0.7/LICENSE` & `lossers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lossers-0.0.7/PKG-INFO` & `lossers-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.7
+Version: 0.0.8
 Summary: Deep Learning Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: Deep Learning,Loss Function,Artificial Intelligence
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.7/lossers/gan.py` & `lossers-0.0.8/lossers/gan.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.7/lossers/lpips/lpips.py` & `lossers-0.0.8/lossers/lpips/lpips.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.7/lossers/lpips/pretrained_model.py` & `lossers-0.0.8/lossers/lpips/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.7/lossers/lpips/vgg_v0.1.pth` & `lossers-0.0.8/lossers/lpips/vgg_v0.1.pth`

 * *Files identical despite different names*

### Comparing `lossers-0.0.7/lossers/ssim.py` & `lossers-0.0.8/lossers/ssim.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.7/lossers.egg-info/PKG-INFO` & `lossers-0.0.8/lossers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.7
+Version: 0.0.8
 Summary: Deep Learning Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: Deep Learning,Loss Function,Artificial Intelligence
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.7/setup.py` & `lossers-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lossers',
     packages = find_packages(exclude=['examples']),
     package_data={'': ['*/vgg_v0.1.pth']},
-    version = '0.0.7',
+    version = '0.0.8',
     license='MIT',
     description = 'Deep Learning Loss Function',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/lossers',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

