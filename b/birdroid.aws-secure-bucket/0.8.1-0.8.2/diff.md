# Comparing `tmp/birdroid.aws-secure-bucket-0.8.1.tar.gz` & `tmp/birdroid.aws-secure-bucket-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birdroid.aws-secure-bucket-0.8.1.tar", last modified: Fri Jul 14 17:24:12 2023, max compression
+gzip compressed data, was "birdroid.aws-secure-bucket-0.8.2.tar", last modified: Sat Jul 15 17:23:25 2023, max compression
```

## Comparing `birdroid.aws-secure-bucket-0.8.1.tar` & `birdroid.aws-secure-bucket-0.8.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:24:12.397611 birdroid.aws-secure-bucket-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-14 17:24:12.397611 birdroid.aws-secure-bucket-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:24:12.397611 birdroid.aws-secure-bucket-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:24:12.393611 birdroid.aws-secure-bucket-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:24:12.393611 birdroid.aws-secure-bucket-0.8.1/src/birdroid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:24:12.393611 birdroid.aws-secure-bucket-0.8.1/src/birdroid/aws_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid/aws_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:24:12.397611 birdroid.aws-secure-bucket-0.8.1/src/birdroid/aws_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid/aws_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30746 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:23:55.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid/aws_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:24:12.393611 birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-14 17:24:12.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-14 17:24:12.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:24:12.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 17:24:12.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 17:24:12.000000 birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:23:25.848670 birdroid.aws-secure-bucket-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-15 17:23:25.848670 birdroid.aws-secure-bucket-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:23:25.848670 birdroid.aws-secure-bucket-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:23:25.844670 birdroid.aws-secure-bucket-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:23:25.844670 birdroid.aws-secure-bucket-0.8.2/src/birdroid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:23:25.848670 birdroid.aws-secure-bucket-0.8.2/src/birdroid/aws_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid/aws_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:23:25.848670 birdroid.aws-secure-bucket-0.8.2/src/birdroid/aws_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid/aws_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30742 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:23:12.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid/aws_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:23:25.848670 birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-15 17:23:25.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-15 17:23:25.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:23:25.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-15 17:23:25.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 17:23:25.000000 birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/top_level.txt
```

### Comparing `birdroid.aws-secure-bucket-0.8.1/LICENSE` & `birdroid.aws-secure-bucket-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `birdroid.aws-secure-bucket-0.8.1/PKG-INFO` & `birdroid.aws-secure-bucket-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdroid.aws-secure-bucket
-Version: 0.8.1
+Version: 0.8.2
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/yicr/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `birdroid.aws-secure-bucket-0.8.1/README.md` & `birdroid.aws-secure-bucket-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `birdroid.aws-secure-bucket-0.8.1/setup.py` & `birdroid.aws-secure-bucket-0.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "birdroid.aws-secure-bucket",
-    "version": "0.8.1",
+    "version": "0.8.2",
     "description": "This is a Simple S3 Secure Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "birdroid.aws_secure_bucket",
         "birdroid.aws_secure_bucket._jsii"
     ],
     "package_data": {
         "birdroid.aws_secure_bucket._jsii": [
-            "aws-secure-bucket@0.8.1.jsii.tgz"
+            "aws-secure-bucket@0.8.2.jsii.tgz"
         ],
         "birdroid.aws_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `birdroid.aws-secure-bucket-0.8.1/src/birdroid/aws_secure_bucket/__init__.py` & `birdroid.aws-secure-bucket-0.8.2/src/birdroid/aws_secure_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO` & `birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdroid.aws-secure-bucket
-Version: 0.8.1
+Version: 0.8.2
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/yicr/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `birdroid.aws-secure-bucket-0.8.1/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt` & `birdroid.aws-secure-bucket-0.8.2/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt
 src/birdroid.aws_secure_bucket.egg-info/dependency_links.txt
 src/birdroid.aws_secure_bucket.egg-info/requires.txt
 src/birdroid.aws_secure_bucket.egg-info/top_level.txt
 src/birdroid/aws_secure_bucket/__init__.py
 src/birdroid/aws_secure_bucket/py.typed
 src/birdroid/aws_secure_bucket/_jsii/__init__.py
-src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.1.jsii.tgz
+src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.2.jsii.tgz
```

