# Comparing `tmp/fdfat-0.1.2.tar.gz` & `tmp/fdfat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.2.tar", last modified: Sun Jul 16 03:28:33 2023, max compression
+gzip compressed data, was "fdfat-0.1.3.tar", last modified: Sun Jul 16 04:40:15 2023, max compression
```

## Comparing `fdfat-0.1.2.tar` & `fdfat-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.862378 fdfat-0.1.2/
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 03:28:33.862227 fdfat-0.1.2/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.2/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.855740 fdfat-0.1.2/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      240 2023-07-16 03:28:06.000000 fdfat-0.1.2/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.856890 fdfat-0.1.2/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4688 2023-07-13 09:29:43.000000 fdfat-0.1.2/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.2/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.857260 fdfat-0.1.2/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)     1040 2023-07-16 03:13:54.000000 fdfat-0.1.2/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.857555 fdfat-0.1.2/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.2/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4202 2023-07-11 11:08:58.000000 fdfat-0.1.2/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.858686 fdfat-0.1.2/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.2/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     2946 2023-07-16 03:15:10.000000 fdfat-0.1.2/fdfat/engine/base.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.859215 fdfat-0.1.2/fdfat/engine/loop/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.2/fdfat/engine/loop/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/engine/loop/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     2702 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/engine/loop/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2113 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/engine/loop/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 03:16:47.000000 fdfat-0.1.2/fdfat/engine/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.2/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.2/fdfat/engine/validator.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.859464 fdfat-0.1.2/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.2/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.2/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.860398 fdfat-0.1.2/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.2/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-14 01:18:16.000000 fdfat-0.1.2/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     4714 2023-07-16 03:26:38.000000 fdfat-0.1.2/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     5150 2023-07-14 01:18:47.000000 fdfat-0.1.2/fdfat/nn/module.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.861758 fdfat-0.1.2/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.2/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7505 2023-07-13 09:25:48.000000 fdfat-0.1.2/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.2/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.2/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.856421 fdfat-0.1.2/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      813 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 03:28:33.862426 fdfat-0.1.2/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-11 11:16:04.000000 fdfat-0.1.2/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.328289 fdfat-0.1.3/
+-rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.3/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 04:40:15.328147 fdfat-0.1.3/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.3/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.323641 fdfat-0.1.3/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-16 04:40:13.000000 fdfat-0.1.3/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.324991 fdfat-0.1.3/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4688 2023-07-13 09:29:43.000000 fdfat-0.1.3/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1696 2023-07-14 11:13:03.000000 fdfat-0.1.3/fdfat/cfg/default.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.3/fdfat/cfg/default_data.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.3/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.325298 fdfat-0.1.3/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)     1040 2023-07-16 03:13:54.000000 fdfat-0.1.3/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.325550 fdfat-0.1.3/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.3/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4202 2023-07-11 11:08:58.000000 fdfat-0.1.3/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.326188 fdfat-0.1.3/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.3/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2946 2023-07-16 03:15:10.000000 fdfat-0.1.3/fdfat/engine/base.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.326696 fdfat-0.1.3/fdfat/engine/loop/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.3/fdfat/engine/loop/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/engine/loop/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2702 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/engine/loop/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2113 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/engine/loop/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 03:16:47.000000 fdfat-0.1.3/fdfat/engine/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.3/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.3/fdfat/engine/validator.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.326900 fdfat-0.1.3/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.3/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.3/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.327348 fdfat-0.1.3/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.3/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-14 01:18:16.000000 fdfat-0.1.3/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4714 2023-07-16 03:26:38.000000 fdfat-0.1.3/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5150 2023-07-14 01:18:47.000000 fdfat-0.1.3/fdfat/nn/module.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.327942 fdfat-0.1.3/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.3/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7505 2023-07-13 09:25:48.000000 fdfat-0.1.3/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.3/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.3/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.324505 fdfat-0.1.3/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      893 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.3/requirements.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 04:40:15.328338 fdfat-0.1.3/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 04:37:36.000000 fdfat-0.1.3/setup.py
```

### Comparing `fdfat-0.1.2/PKG-INFO` & `fdfat-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.2/README.md` & `fdfat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/cfg/__init__.py` & `fdfat-0.1.3/fdfat/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.3/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/cli/__init__.py` & `fdfat-0.1.3/fdfat/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/data/dataloader.py` & `fdfat-0.1.3/fdfat/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/engine/base.py` & `fdfat-0.1.3/fdfat/engine/base.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/engine/loop/tester.py` & `fdfat-0.1.3/fdfat/engine/loop/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/engine/loop/trainer.py` & `fdfat-0.1.3/fdfat/engine/loop/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/engine/loop/validator.py` & `fdfat-0.1.3/fdfat/engine/loop/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/engine/tester.py` & `fdfat-0.1.3/fdfat/engine/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/engine/trainer.py` & `fdfat-0.1.3/fdfat/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/engine/validator.py` & `fdfat-0.1.3/fdfat/engine/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/metric/metric.py` & `fdfat-0.1.3/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/nn/conv.py` & `fdfat-0.1.3/fdfat/nn/conv.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/nn/model.py` & `fdfat-0.1.3/fdfat/nn/model.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/nn/module.py` & `fdfat-0.1.3/fdfat/nn/module.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/utils/logger.py` & `fdfat-0.1.3/fdfat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/utils/model_utils.py` & `fdfat-0.1.3/fdfat/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/utils/pose_estimation.py` & `fdfat-0.1.3/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat/utils/utils.py` & `fdfat-0.1.3/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.2/fdfat.egg-info/PKG-INFO` & `fdfat-0.1.3/fdfat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.2/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.3/fdfat.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 fdfat/__init__.py
 fdfat.egg-info/PKG-INFO
 fdfat.egg-info/SOURCES.txt
 fdfat.egg-info/dependency_links.txt
 fdfat.egg-info/entry_points.txt
 fdfat.egg-info/requires.txt
 fdfat.egg-info/top_level.txt
 fdfat/cfg/__init__.py
+fdfat/cfg/default.yaml
+fdfat/cfg/default_data.yaml
 fdfat/cfg/yaml_utils.py
 fdfat/cli/__init__.py
 fdfat/data/__init__.py
 fdfat/data/dataloader.py
 fdfat/engine/__init__.py
 fdfat/engine/base.py
 fdfat/engine/tester.py
```

### Comparing `fdfat-0.1.2/setup.py` & `fdfat-0.1.3/setup.py`

 * *Files identical despite different names*

