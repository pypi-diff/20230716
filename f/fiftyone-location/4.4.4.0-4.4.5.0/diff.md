# Comparing `tmp/fiftyone_location-4.4.4.0.tar.gz` & `tmp/fiftyone_location-4.4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_location-4.4.4.0.tar", last modified: Fri Jul 14 01:29:19 2023, max compression
+gzip compressed data, was "fiftyone_location-4.4.5.0.tar", last modified: Sun Jul 16 01:29:40 2023, max compression
```

## Comparing `fiftyone_location-4.4.4.0.tar` & `fiftyone_location-4.4.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:29:19.372193 fiftyone_location-4.4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 01:29:14.000000 fiftyone_location-4.4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-14 01:29:19.372193 fiftyone_location-4.4.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:29:19.368193 fiftyone_location-4.4.4.0/fiftyone_location/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:29:14.000000 fiftyone_location-4.4.4.0/fiftyone_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-14 01:29:14.000000 fiftyone_location-4.4.4.0/fiftyone_location/location_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-14 01:29:14.000000 fiftyone_location-4.4.4.0/fiftyone_location/location_pipelinebuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:29:19.368193 fiftyone_location-4.4.4.0/fiftyone_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-14 01:29:19.000000 fiftyone_location-4.4.4.0/fiftyone_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 01:29:19.000000 fiftyone_location-4.4.4.0/fiftyone_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:29:19.000000 fiftyone_location-4.4.4.0/fiftyone_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 01:29:19.000000 fiftyone_location-4.4.4.0/fiftyone_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 01:29:19.000000 fiftyone_location-4.4.4.0/fiftyone_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:29:19.372193 fiftyone_location-4.4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-14 01:29:14.000000 fiftyone_location-4.4.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 01:29:18.000000 fiftyone_location-4.4.4.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:29:40.454457 fiftyone_location-4.4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-16 01:29:33.000000 fiftyone_location-4.4.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-16 01:29:40.454457 fiftyone_location-4.4.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:29:40.454457 fiftyone_location-4.4.5.0/fiftyone_location/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 01:29:33.000000 fiftyone_location-4.4.5.0/fiftyone_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-16 01:29:33.000000 fiftyone_location-4.4.5.0/fiftyone_location/location_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-16 01:29:33.000000 fiftyone_location-4.4.5.0/fiftyone_location/location_pipelinebuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:29:40.454457 fiftyone_location-4.4.5.0/fiftyone_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-16 01:29:40.000000 fiftyone_location-4.4.5.0/fiftyone_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-16 01:29:40.000000 fiftyone_location-4.4.5.0/fiftyone_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:29:40.000000 fiftyone_location-4.4.5.0/fiftyone_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 01:29:40.000000 fiftyone_location-4.4.5.0/fiftyone_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-16 01:29:40.000000 fiftyone_location-4.4.5.0/fiftyone_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 01:29:40.454457 fiftyone_location-4.4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-16 01:29:33.000000 fiftyone_location-4.4.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 01:29:39.000000 fiftyone_location-4.4.5.0/version.txt
```

### Comparing `fiftyone_location-4.4.4.0/PKG-INFO` & `fiftyone_location-4.4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_location
-Version: 4.4.4.0
+Version: 4.4.5.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This repository contains the geo-location engines for the Python implementation of the Pipeline API.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_location-4.4.4.0/fiftyone_location/location_cloud.py` & `fiftyone_location-4.4.5.0/fiftyone_location/location_cloud.py`

 * *Files identical despite different names*

### Comparing `fiftyone_location-4.4.4.0/fiftyone_location/location_pipelinebuilder.py` & `fiftyone_location-4.4.5.0/fiftyone_location/location_pipelinebuilder.py`

 * *Files identical despite different names*

### Comparing `fiftyone_location-4.4.4.0/fiftyone_location.egg-info/PKG-INFO` & `fiftyone_location-4.4.5.0/fiftyone_location.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-location
-Version: 4.4.4.0
+Version: 4.4.5.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This repository contains the geo-location engines for the Python implementation of the Pipeline API.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_location-4.4.4.0/setup.py` & `fiftyone_location-4.4.5.0/setup.py`

 * *Files identical despite different names*

