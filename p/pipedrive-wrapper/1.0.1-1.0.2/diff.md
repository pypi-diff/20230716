# Comparing `tmp/pipedrive-wrapper-1.0.1.tar.gz` & `tmp/pipedrive-wrapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipedrive-wrapper-1.0.1.tar", last modified: Sun Jul 16 14:52:50 2023, max compression
+gzip compressed data, was "pipedrive-wrapper-1.0.2.tar", last modified: Sun Jul 16 14:58:59 2023, max compression
```

## Comparing `pipedrive-wrapper-1.0.1.tar` & `pipedrive-wrapper-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 14:52:50.237584 pipedrive-wrapper-1.0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      705 2023-07-16 14:52:50.236581 pipedrive-wrapper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 14:52:50.221551 pipedrive-wrapper-1.0.1/pipedrive/
--rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.1/pipedrive/__init__.py
--rw-rw-rw-   0        0        0     3628 2023-07-16 14:41:55.000000 pipedrive-wrapper-1.0.1/pipedrive/activity.py
--rw-rw-rw-   0        0        0     2915 2023-07-16 14:41:50.000000 pipedrive-wrapper-1.0.1/pipedrive/client.py
--rw-rw-rw-   0        0        0     5541 2023-07-16 14:39:30.000000 pipedrive-wrapper-1.0.1/pipedrive/deal.py
--rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.1/pipedrive/exceptions.py
--rw-rw-rw-   0        0        0     5541 2023-07-16 14:42:13.000000 pipedrive-wrapper-1.0.1/pipedrive/person.py
--rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.1/pipedrive/util.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:52:50.235583 pipedrive-wrapper-1.0.1/pipedrive_wrapper.egg-info/
--rw-rw-rw-   0        0        0      705 2023-07-16 14:52:50.000000 pipedrive-wrapper-1.0.1/pipedrive_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-16 14:52:50.000000 pipedrive-wrapper-1.0.1/pipedrive_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 14:52:50.000000 pipedrive-wrapper-1.0.1/pipedrive_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 14:52:50.000000 pipedrive-wrapper-1.0.1/pipedrive_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-16 14:52:50.000000 pipedrive-wrapper-1.0.1/pipedrive_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 14:52:50.237584 pipedrive-wrapper-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-16 14:52:38.000000 pipedrive-wrapper-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:58:59.983624 pipedrive-wrapper-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      705 2023-07-16 14:58:59.983624 pipedrive-wrapper-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 14:58:59.962922 pipedrive-wrapper-1.0.2/pipedrive/
+-rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.2/pipedrive/__init__.py
+-rw-rw-rw-   0        0        0     3628 2023-07-16 14:41:55.000000 pipedrive-wrapper-1.0.2/pipedrive/activity.py
+-rw-rw-rw-   0        0        0     2915 2023-07-16 14:41:50.000000 pipedrive-wrapper-1.0.2/pipedrive/client.py
+-rw-rw-rw-   0        0        0     6356 2023-07-16 14:58:11.000000 pipedrive-wrapper-1.0.2/pipedrive/deal.py
+-rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.2/pipedrive/exceptions.py
+-rw-rw-rw-   0        0        0     5541 2023-07-16 14:42:13.000000 pipedrive-wrapper-1.0.2/pipedrive/person.py
+-rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.2/pipedrive/util.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:58:59.982624 pipedrive-wrapper-1.0.2/pipedrive_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      705 2023-07-16 14:58:59.000000 pipedrive-wrapper-1.0.2/pipedrive_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-16 14:58:59.000000 pipedrive-wrapper-1.0.2/pipedrive_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 14:58:59.000000 pipedrive-wrapper-1.0.2/pipedrive_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 14:58:59.000000 pipedrive-wrapper-1.0.2/pipedrive_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 14:58:59.000000 pipedrive-wrapper-1.0.2/pipedrive_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 14:58:59.984622 pipedrive-wrapper-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-07-16 14:58:35.000000 pipedrive-wrapper-1.0.2/setup.py
```

### Comparing `pipedrive-wrapper-1.0.1/LICENSE` & `pipedrive-wrapper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.1/PKG-INFO` & `pipedrive-wrapper-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.1/pipedrive/activity.py` & `pipedrive-wrapper-1.0.2/pipedrive/activity.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.1/pipedrive/client.py` & `pipedrive-wrapper-1.0.2/pipedrive/client.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.1/pipedrive/deal.py` & `pipedrive-wrapper-1.0.2/pipedrive/person.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.1/pipedrive/exceptions.py` & `pipedrive-wrapper-1.0.2/pipedrive/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.1/pipedrive/util.py` & `pipedrive-wrapper-1.0.2/pipedrive/util.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.1/pipedrive_wrapper.egg-info/PKG-INFO` & `pipedrive-wrapper-1.0.2/pipedrive_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.1/setup.py` & `pipedrive-wrapper-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pipedrive-wrapper",
-    version="1.0.1",
+    version="1.0.2",
     author="Pedro Cantidio",
     author_email="ppcantidio@gmail.com",
     description="A Python wrapper for the Pipedrive API",
     long_description="A Python wrapper that simplifies interaction with the Pipedrive API",
     url="https://github.com/ppcantidio/pipedrive.py",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
```

