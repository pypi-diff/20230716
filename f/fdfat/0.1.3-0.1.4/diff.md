# Comparing `tmp/fdfat-0.1.3.tar.gz` & `tmp/fdfat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.3.tar", last modified: Sun Jul 16 04:40:15 2023, max compression
+gzip compressed data, was "fdfat-0.1.4.tar", last modified: Sun Jul 16 06:09:19 2023, max compression
```

## Comparing `fdfat-0.1.3.tar` & `fdfat-0.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.328289 fdfat-0.1.3/
--rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.3/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 04:40:15.328147 fdfat-0.1.3/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.3/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.323641 fdfat-0.1.3/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-16 04:40:13.000000 fdfat-0.1.3/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.324991 fdfat-0.1.3/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4688 2023-07-13 09:29:43.000000 fdfat-0.1.3/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1696 2023-07-14 11:13:03.000000 fdfat-0.1.3/fdfat/cfg/default.yaml
--rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.3/fdfat/cfg/default_data.yaml
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.3/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.325298 fdfat-0.1.3/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)     1040 2023-07-16 03:13:54.000000 fdfat-0.1.3/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.325550 fdfat-0.1.3/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.3/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4202 2023-07-11 11:08:58.000000 fdfat-0.1.3/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.326188 fdfat-0.1.3/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.3/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     2946 2023-07-16 03:15:10.000000 fdfat-0.1.3/fdfat/engine/base.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.326696 fdfat-0.1.3/fdfat/engine/loop/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.3/fdfat/engine/loop/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/engine/loop/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     2702 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/engine/loop/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2113 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/engine/loop/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 03:16:47.000000 fdfat-0.1.3/fdfat/engine/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.3/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.3/fdfat/engine/validator.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.326900 fdfat-0.1.3/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.3/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.3/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.327348 fdfat-0.1.3/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.3/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-14 01:18:16.000000 fdfat-0.1.3/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     4714 2023-07-16 03:26:38.000000 fdfat-0.1.3/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     5150 2023-07-14 01:18:47.000000 fdfat-0.1.3/fdfat/nn/module.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.327942 fdfat-0.1.3/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.3/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.3/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7505 2023-07-13 09:25:48.000000 fdfat-0.1.3/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.3/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.3/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 04:40:15.324505 fdfat-0.1.3/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      893 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 04:40:15.000000 fdfat-0.1.3/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.3/requirements.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 04:40:15.328338 fdfat-0.1.3/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 04:37:36.000000 fdfat-0.1.3/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.568327 fdfat-0.1.4/
+-rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.4/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 06:09:19.568209 fdfat-0.1.4/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.4/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.563847 fdfat-0.1.4/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-16 06:09:06.000000 fdfat-0.1.4/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.565128 fdfat-0.1.4/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4700 2023-07-16 06:01:25.000000 fdfat-0.1.4/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1796 2023-07-16 06:01:17.000000 fdfat-0.1.4/fdfat/cfg/default.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.4/fdfat/cfg/default_data.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.4/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.565245 fdfat-0.1.4/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)     1040 2023-07-16 03:13:54.000000 fdfat-0.1.4/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.565675 fdfat-0.1.4/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.4/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4086 2023-07-16 06:03:32.000000 fdfat-0.1.4/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.566308 fdfat-0.1.4/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.4/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2946 2023-07-16 03:15:10.000000 fdfat-0.1.4/fdfat/engine/base.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.566834 fdfat-0.1.4/fdfat/engine/loop/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.4/fdfat/engine/loop/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.4/fdfat/engine/loop/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2814 2023-07-16 06:06:48.000000 fdfat-0.1.4/fdfat/engine/loop/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2233 2023-07-16 06:07:42.000000 fdfat-0.1.4/fdfat/engine/loop/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 06:07:55.000000 fdfat-0.1.4/fdfat/engine/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.4/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.4/fdfat/engine/validator.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.567046 fdfat-0.1.4/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.4/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.4/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.567484 fdfat-0.1.4/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.4/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-14 01:18:16.000000 fdfat-0.1.4/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4714 2023-07-16 03:26:38.000000 fdfat-0.1.4/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5150 2023-07-14 01:18:47.000000 fdfat-0.1.4/fdfat/nn/module.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.568028 fdfat-0.1.4/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.4/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.4/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7505 2023-07-13 09:25:48.000000 fdfat-0.1.4/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.4/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.4/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.564619 fdfat-0.1.4/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      893 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.4/requirements.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 06:09:19.568367 fdfat-0.1.4/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.4/setup.py
```

### Comparing `fdfat-0.1.3/PKG-INFO` & `fdfat-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.3/README.md` & `fdfat-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/cfg/__init__.py` & `fdfat-0.1.4/fdfat/cfg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Union
 
 from fdfat.cfg.yaml_utils import yaml_load, yaml_save, yaml_print, DEFAULT_CFG_DICT, DEFAULT_CFG_DATA, IterableSimpleNamespace
 
 CFG_INT_KEYS= 'seed', 'workers', 'imgsz', 'epoch', 'batch_size', 'dump_batch', 'patience', 'warmup'
 CFG_FRACTION_KEYS = ('lr', 'lr0_factor', 'lr_factor', 'aux_pose_weight')
 CFG_FLOAT_KEYS = ("aug", 'muliplier', 'w_jaw', 'w_leyeb', 'w_reyeb', 'w_nose', 'w_nosetip', 'w_leye', 'w_reye', 'w_mount', 'w_purpil')
-CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled", "resume", "warmup")
+CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled", "resume", "warmup", "pre_norm")
 
 def cfg2dict(cfg):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Inputs:
         cfg (str) or (Path) or (SimpleNamespace): Configuration object to be converted to a dictionary.
```

### Comparing `fdfat-0.1.3/fdfat/cfg/default.yaml` & `fdfat-0.1.4/fdfat/cfg/default.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # data
 data: # path to dataset file, ie. face_synth.yaml
 workers: 8 # number of workers for dataloader
 aug: 0.5 # aug
 input: # input file path/url for prediction
 validation: val # validation target set in the data yaml, one of train, val, test
+pre_norm: true # normalize data in dataloader instead of normalizing right before feeding to model 
 
 # model
 model: # modelname
 imgsz: 128 # size of input image as integer
 aux_pose: False # model with auxiliary pose esimation
 muliplier: 1.0 # model depth multiplier
 checkpoint: # target checkpoint to load
```

### Comparing `fdfat-0.1.3/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.4/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/cli/__init__.py` & `fdfat-0.1.4/fdfat/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/data/dataloader.py` & `fdfat-0.1.4/fdfat/data/dataloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     offset_ab = (2*np.random.random(2)-1)*offset*size
 
     size = size*np.random.uniform(low=scale[0], high=scale[1], size=1)
     center = center + offset_ab
 
     return np.vstack([center-size/2, center+size/2])
 
-def read_data(img_path, lmk_scale=1.0, aug=None, imgsz=128):
+def read_data(img_path, lmk_scale=1.0, aug=None, imgsz=128, norm=True):
     img = Image.open(img_path)
     lmk_path = img_path.replace(".png", "_ldmks.txt")
     with open(lmk_path, 'r') as f:
         lmk = f.readlines()
         lmk = np.array([[float(n) for n in l.strip("\n").split(" ")] for l in lmk])
 
     bbox = gen_bbox(lmk)
@@ -44,34 +44,31 @@
 
     if aug is not None:
         transformed = aug(image=croped, keypoints=lmk)
         croped = transformed['image']
         lmk = transformed['keypoints']
         lmk = np.array(lmk)
 
-    croped = (croped / 127.5) - 1
-
     # normalize
     lmk /= imgsz
     lmk -= 0.5
     lmk *= lmk_scale
+    lmk = lmk.astype(np.float32)
 
-    # bbox_center = (bbox[0, :] + bbox[1, :]) / 2
-    # lmk[:,0] -= bbox_center[0]
-    # lmk[:,1] -= bbox_center[1]
-    # lmk[:,0] /= croped.size[0]
-    # lmk[:,1] /= croped.size[1]
-    # lmk[:,0] *= lmk_scale
-    # lmk[:,1] *= lmk_scale
-    # lmk = lmk.astype(np.float32)
+    if norm:
+        croped = (croped / 127.5) - 1
+        croped = croped.astype(np.float32)
+    else:
+        croped.astype(np.uint8)
 
-    return croped.astype(np.float32), lmk.astype(np.float32)
+    return croped, lmk
 
 class LandmarkDataset(Dataset):
     def __init__(self, cfgs, annotations_files, imgsz=128, aug=True, pose_rotation=False):
+        self.norm = cfgs.pre_norm
         self.img_paths = annotations_files
         self.imgsz = imgsz
         self.pose_rotation = pose_rotation
 
         if aug:
             self.aug = A.Compose([
                 # A.HorizontalFlip(p=0.5), # wrong lmk idx
@@ -103,15 +100,15 @@
 
     def __len__(self):
         return len(self.img_paths)
 
     def __getitem__(self, idx):
         img_path = self.img_paths[idx]
 
-        img, lmk = read_data(img_path, aug=self.aug, imgsz=self.imgsz)
+        img, lmk = read_data(img_path, aug=self.aug, imgsz=self.imgsz, norm=self.norm)
         
         if self.pose_rotation:
             estimator = PoseEstimator(self.imgsz, self.imgsz)
             lmk_denorm = (lmk + 0.5)*self.imgsz
             rot_vec, _ = estimator.solve(lmk_denorm[:68,:])
             rot_vec_norm = np.divide(rot_vec[:,0] - POSE_ROTAION_MED, POSE_ROTATION_STD*2)
```

### Comparing `fdfat-0.1.3/fdfat/engine/base.py` & `fdfat-0.1.4/fdfat/engine/base.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/engine/loop/tester.py` & `fdfat-0.1.4/fdfat/engine/loop/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/engine/loop/trainer.py` & `fdfat-0.1.4/fdfat/engine/loop/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
     num_batches = len(dataloader)
     pbar = tqdm.tqdm(enumerate(dataloader), total=num_batches, bar_format=TQDM_BAR_FORMAT)
 
     model.train()
     for batch, (x, y) in pbar:
         x_device = x.to(cfgs.device, non_blocking=True)
+        if not cfgs.pre_norm:
+            x_device = ((x_device / 127.5) - 1).type(torch.float32)
         y_device = y.to(cfgs.device, non_blocking=True)
 
         pred = model(x_device)
 
         if cfgs.aux_pose:
             loss = loss_fn(pred, y_device[:,:-1])
 
@@ -64,13 +66,13 @@
             loss_dict["pose"] += (loss[:,-3:] / cfgs.aux_pose_weight).mean().item()
             losses_str = f"{losses_str}, pose: {loss_dict['pose']/(batch+1):>7f}"
 
         pbar.set_description(f"{name} epoch [{current_epoch+1:3d}/{cfgs.epoch:3d}] {losses_str}")
         
         if current_epoch == 0 and batch < cfgs.dump_batch:
             save_batch_png = cfgs.save_dir / f'{name}_batch{batch}.png'
-            render_batch(x.cpu().detach().numpy(), y[:,:70*2].cpu().detach().numpy(), save_batch_png)
+            render_batch(x_device.cpu().detach().numpy(), y_device[:,:70*2].cpu().detach().numpy(), save_batch_png)
 
     for k in loss_dict.keys():
         loss_dict[k] /= num_batches
 
     return loss_dict
```

### Comparing `fdfat-0.1.3/fdfat/engine/loop/validator.py` & `fdfat-0.1.4/fdfat/engine/loop/validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     num_batches = len(dataloader)
     pbar = tqdm.tqdm(enumerate(dataloader), total=num_batches, bar_format=TQDM_BAR_FORMAT)
 
     model.eval()
     with torch.no_grad():
         for batch, (x, y) in pbar:
             x_device = x.to(cfgs.device, non_blocking=True)
+            if not cfgs.pre_norm:
+                x_device = ((x_device / 127.5) - 1).type(torch.float32)
             y_device = y.to(cfgs.device, non_blocking=True)
 
             pred = model(x_device)
 
             if cfgs.aux_pose:
                 loss = loss_fn(pred, y_device[:,:-1])
                 pose_weight = y_device[:,-1:]
@@ -42,13 +44,13 @@
                 loss_dict["pose"] += (loss[:,-3:] / cfgs.aux_pose_weight).mean().item()
                 losses_str = f"{losses_str}, pose: {loss_dict['pose']/(batch+1):>7f}"
 
             pbar.set_description(f"{name} epoch [{current_epoch+1:3d}/{cfgs.epoch:3d}] {losses_str}")
 
             if current_epoch == 0 and batch < cfgs.dump_batch:
                 save_batch_png = cfgs.save_dir / f'{name}_batch{batch}.png'
-                render_batch(x.cpu().detach().numpy(), y[:,:70*2].cpu().detach().numpy(), save_batch_png)
+                render_batch(x_device.cpu().detach().numpy(), y_device[:,:70*2].cpu().detach().numpy(), save_batch_png)
 
     for k in loss_dict.keys():
         loss_dict[k] /= num_batches
 
     return loss_dict
```

### Comparing `fdfat-0.1.3/fdfat/engine/tester.py` & `fdfat-0.1.4/fdfat/engine/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/engine/trainer.py` & `fdfat-0.1.4/fdfat/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/engine/validator.py` & `fdfat-0.1.4/fdfat/engine/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/metric/metric.py` & `fdfat-0.1.4/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/nn/conv.py` & `fdfat-0.1.4/fdfat/nn/conv.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/nn/model.py` & `fdfat-0.1.4/fdfat/nn/model.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/nn/module.py` & `fdfat-0.1.4/fdfat/nn/module.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/utils/logger.py` & `fdfat-0.1.4/fdfat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/utils/model_utils.py` & `fdfat-0.1.4/fdfat/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/utils/pose_estimation.py` & `fdfat-0.1.4/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat/utils/utils.py` & `fdfat-0.1.4/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/fdfat.egg-info/PKG-INFO` & `fdfat-0.1.4/fdfat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.3/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.4/fdfat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/requirements.txt` & `fdfat-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.3/setup.py` & `fdfat-0.1.4/setup.py`

 * *Files identical despite different names*

