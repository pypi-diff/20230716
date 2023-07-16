# Comparing `tmp/fdfat-0.1.4.tar.gz` & `tmp/fdfat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.4.tar", last modified: Sun Jul 16 06:09:19 2023, max compression
+gzip compressed data, was "fdfat-0.1.5.tar", last modified: Sun Jul 16 09:11:33 2023, max compression
```

## Comparing `fdfat-0.1.4.tar` & `fdfat-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.568327 fdfat-0.1.4/
--rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.4/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 06:09:19.568209 fdfat-0.1.4/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.4/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.563847 fdfat-0.1.4/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-16 06:09:06.000000 fdfat-0.1.4/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.565128 fdfat-0.1.4/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4700 2023-07-16 06:01:25.000000 fdfat-0.1.4/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1796 2023-07-16 06:01:17.000000 fdfat-0.1.4/fdfat/cfg/default.yaml
--rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.4/fdfat/cfg/default_data.yaml
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.4/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.565245 fdfat-0.1.4/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)     1040 2023-07-16 03:13:54.000000 fdfat-0.1.4/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.565675 fdfat-0.1.4/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.4/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4086 2023-07-16 06:03:32.000000 fdfat-0.1.4/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.566308 fdfat-0.1.4/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.4/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     2946 2023-07-16 03:15:10.000000 fdfat-0.1.4/fdfat/engine/base.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.566834 fdfat-0.1.4/fdfat/engine/loop/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.4/fdfat/engine/loop/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.4/fdfat/engine/loop/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     2814 2023-07-16 06:06:48.000000 fdfat-0.1.4/fdfat/engine/loop/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2233 2023-07-16 06:07:42.000000 fdfat-0.1.4/fdfat/engine/loop/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 06:07:55.000000 fdfat-0.1.4/fdfat/engine/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.4/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.4/fdfat/engine/validator.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.567046 fdfat-0.1.4/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.4/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.4/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.567484 fdfat-0.1.4/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.4/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-14 01:18:16.000000 fdfat-0.1.4/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     4714 2023-07-16 03:26:38.000000 fdfat-0.1.4/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     5150 2023-07-14 01:18:47.000000 fdfat-0.1.4/fdfat/nn/module.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.568028 fdfat-0.1.4/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.4/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.4/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7505 2023-07-13 09:25:48.000000 fdfat-0.1.4/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.4/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.4/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 06:09:19.564619 fdfat-0.1.4/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      893 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 06:09:19.000000 fdfat-0.1.4/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.4/requirements.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 06:09:19.568367 fdfat-0.1.4/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.4/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.531662 fdfat-0.1.5/
+-rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.5/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 09:11:33.531529 fdfat-0.1.5/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.5/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.527149 fdfat-0.1.5/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-16 09:11:32.000000 fdfat-0.1.5/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.528472 fdfat-0.1.5/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4734 2023-07-16 08:09:07.000000 fdfat-0.1.5/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1986 2023-07-16 08:08:53.000000 fdfat-0.1.5/fdfat/cfg/default.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.5/fdfat/cfg/default_data.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.5/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.528586 fdfat-0.1.5/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)     1153 2023-07-16 08:01:18.000000 fdfat-0.1.5/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.528792 fdfat-0.1.5/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.5/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4086 2023-07-16 06:03:32.000000 fdfat-0.1.5/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.529467 fdfat-0.1.5/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.5/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3014 2023-07-16 08:26:08.000000 fdfat-0.1.5/fdfat/engine/base.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3359 2023-07-16 08:36:51.000000 fdfat-0.1.5/fdfat/engine/exporter.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.529917 fdfat-0.1.5/fdfat/engine/loop/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.5/fdfat/engine/loop/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.5/fdfat/engine/loop/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2814 2023-07-16 06:06:48.000000 fdfat-0.1.5/fdfat/engine/loop/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2233 2023-07-16 06:07:42.000000 fdfat-0.1.5/fdfat/engine/loop/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 06:07:55.000000 fdfat-0.1.5/fdfat/engine/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.5/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.5/fdfat/engine/validator.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.530125 fdfat-0.1.5/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.5/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.5/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.530617 fdfat-0.1.5/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.5/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3902 2023-07-16 08:24:43.000000 fdfat-0.1.5/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5072 2023-07-16 08:30:38.000000 fdfat-0.1.5/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5929 2023-07-16 08:28:43.000000 fdfat-0.1.5/fdfat/nn/module.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.531306 fdfat-0.1.5/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.5/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.5/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7722 2023-07-16 08:36:19.000000 fdfat-0.1.5/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.5/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.5/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.527970 fdfat-0.1.5/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      918 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.5/requirements.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 09:11:33.531707 fdfat-0.1.5/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.5/setup.py
```

### Comparing `fdfat-0.1.4/PKG-INFO` & `fdfat-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.4/README.md` & `fdfat-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/cfg/__init__.py` & `fdfat-0.1.5/fdfat/cfg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Union
 
 from fdfat.cfg.yaml_utils import yaml_load, yaml_save, yaml_print, DEFAULT_CFG_DICT, DEFAULT_CFG_DATA, IterableSimpleNamespace
 
 CFG_INT_KEYS= 'seed', 'workers', 'imgsz', 'epoch', 'batch_size', 'dump_batch', 'patience', 'warmup'
 CFG_FRACTION_KEYS = ('lr', 'lr0_factor', 'lr_factor', 'aux_pose_weight')
 CFG_FLOAT_KEYS = ("aug", 'muliplier', 'w_jaw', 'w_leyeb', 'w_reyeb', 'w_nose', 'w_nosetip', 'w_leye', 'w_reye', 'w_mount', 'w_purpil')
-CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled", "resume", "warmup", "pre_norm")
+CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled", "resume", "warmup", "pre_norm", "export_simplify", "export_pose")
 
 def cfg2dict(cfg):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Inputs:
         cfg (str) or (Path) or (SimpleNamespace): Configuration object to be converted to a dictionary.
```

### Comparing `fdfat-0.1.4/fdfat/cfg/default.yaml` & `fdfat-0.1.5/fdfat/cfg/default.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # general
-task: train # train, val, predict
+task: train # train, val, predict, export
 name: Landmark # name of experiment
 project: # path to project folder
 seed: 0  # random seed for reproducibility
 override: False # overide project if any, otherwise it will created a new project
 
 # data
 data: # path to dataset file, ie. face_synth.yaml
@@ -33,21 +33,26 @@
 lre_factor: 0.1 # end_lr = current_lr*lr_factor at the end of the trainning
 device: cpu # target device, ie. cuda device=0 or device=0,1,2,3 or device=cpu
 dump_batch: 5 # write sample batch for debug
 save: True # save checkpoint and stats
 pin_memory: False # use pin memory for dataloader
 aux_pose_weight: 0.5 # loss weight for auxiliary pose esimation
 
-# testing
-test_warmup: True # warming up model when testing
-
 # trainning loss weights
 lossw_enabled: False
 w_jaw: 1.0
 w_leyeb: 1.0
 w_reyeb: 1.0
 w_nose: 1.0
 w_nosetip: 1.0
 w_leye: 1.0
 w_reye: 1.0
 w_mount: 1.0
-w_purpil: 1.0
+w_purpil: 1.0
+
+# testing
+test_warmup: True # warming up model when testing
+
+# export
+export_format: onnx # torchscript, onnx, saved_model, tflite
+export_pose: false # export with aux pose estimation
+export_simplify: true # simplify onnx model using onnxsim
```

### Comparing `fdfat-0.1.4/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.5/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/cli/__init__.py` & `fdfat-0.1.5/fdfat/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from types import SimpleNamespace
 
 from fdfat.utils.logger import LOGGER
 from fdfat.cfg import get_cfg
-# from fdfat.main import TrainEngine, ValEngine, TestEngine
-from fdfat.engine import trainer, validator, tester
+# from fdfat.main import TrainEngine, ValEngine, TestEngine, 
+from fdfat.engine import trainer, validator, tester, exporter
 
 def entrypoint():
     default_cfg = get_cfg()
 
     parser = argparse.ArgumentParser(description='train loop.')
     for k, v in default_cfg:
         parser.add_argument(f"--{k}", type=type(v) if v is not None else str, default=v)
@@ -25,7 +25,10 @@
         engine.do_validate()
     elif args.task == "predict":
         engine = tester.TestEngine(args)
         if args.input is None:
             raise ValueError("Input is empty")
         lmk, rendered = engine.predict(args.input, render=True)
         rendered.save("predict.jpg")
+    elif args.task == "export":
+        engine = exporter.ExportEngine(args)
+        engine.export()
```

### Comparing `fdfat-0.1.4/fdfat/data/dataloader.py` & `fdfat-0.1.5/fdfat/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/engine/base.py` & `fdfat-0.1.5/fdfat/engine/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 
     def load_database(self):
         raise NotImplementedError("Not implemented")
     
     def prepare(self):
         raise NotImplementedError("Not implemented")
 
-    def load_model(self, verbose=True):
+    def load_model(self, verbose=True, track_running_stats=False):
         LOGGER.info(f"Load model: {self.cfgs.model}")
-        self.net = getattr(model, self.cfgs.model)(imgz=self.cfgs.imgsz, muliplier=self.cfgs.muliplier, pose_rotation=self.cfgs.aux_pose).to(self.cfgs.device)
+        self.net = getattr(model, self.cfgs.model)(imgz=self.cfgs.imgsz, muliplier=self.cfgs.muliplier, pose_rotation=self.cfgs.aux_pose, track_running_stats=track_running_stats).to(self.cfgs.device)
         if verbose:
             _ = model_info(self.net, detailed=True, imgsz=self.cfgs.imgsz, device=self.cfgs.device)
 
     def load_checkpoint(self, checkpoint):
         if isinstance(checkpoint, str) or isinstance(checkpoint, Path):
             checkpoint = torch.load(checkpoint)
         self.checkpoint = checkpoint
```

### Comparing `fdfat-0.1.4/fdfat/engine/loop/tester.py` & `fdfat-0.1.5/fdfat/engine/loop/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/engine/loop/trainer.py` & `fdfat-0.1.5/fdfat/engine/loop/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/engine/loop/validator.py` & `fdfat-0.1.5/fdfat/engine/loop/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/engine/tester.py` & `fdfat-0.1.5/fdfat/engine/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/engine/trainer.py` & `fdfat-0.1.5/fdfat/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/engine/validator.py` & `fdfat-0.1.5/fdfat/engine/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/metric/metric.py` & `fdfat-0.1.5/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/nn/conv.py` & `fdfat-0.1.5/fdfat/nn/conv.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         p = k // 2 if isinstance(k, int) else [x // 2 for x in k]  # auto-pad
     return p
 
 class Conv(nn.Module):
     """Standard convolution with args(ch_in, ch_out, kernel, stride, padding, groups, dilation, activation)."""
     default_act = nn.SiLU()  # default activation
 
-    def __init__(self, c1, c2, k=1, s=1, p=None, g=1, d=1, act=True):
+    def __init__(self, c1, c2, k=1, s=1, p=None, g=1, d=1, act=True, track_running_stats=False):
         """Initialize Conv layer with given arguments including activation."""
         super().__init__()
         self.conv = nn.Conv2d(c1, c2, k, s, autopad(k, p, d), groups=g, dilation=d, bias=False)
-        self.bn = nn.BatchNorm2d(c2, track_running_stats=False)
+        self.bn = nn.BatchNorm2d(c2, track_running_stats=track_running_stats)
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
         initialize_weights(self)
 
     def forward(self, x):
         """Apply convolution, batch normalization and activation to input tensor."""
         return self.act(self.bn(self.conv(x)))
@@ -46,16 +46,16 @@
     def forward_fuse(self, x):
         """Perform transposed convolution of 2D data."""
         return self.act(self.conv(x))
     
 class DWConv(Conv):
     """Depth-wise convolution."""
 
-    def __init__(self, c1, c2, k=1, s=1, d=1, act=True):  # ch_in, ch_out, kernel, stride, dilation, activation
-        super().__init__(c1, c2, k, s, g=math.gcd(c1, c2), d=d, act=act)
+    def __init__(self, c1, c2, k=1, s=1, d=1, act=True, track_running_stats=False):  # ch_in, ch_out, kernel, stride, dilation, activation
+        super().__init__(c1, c2, k, s, g=math.gcd(c1, c2), d=d, act=act, track_running_stats=track_running_stats)
 
 class Concat(nn.Module):
     """Concatenate a list of tensors along dimension."""
 
     def __init__(self, dimension=1):
         """Concatenates a list of tensors along a specified dimension."""
         super().__init__()
@@ -66,29 +66,29 @@
         return torch.cat(x, self.d)
 
 
 class IdentifyBlock(nn.Module):
 
     default_act = nn.ReLU6()  # default activation
 
-    def __init__(self, in_ch, out_ch, expand, k=3, act=True, stride=1, dilation_rate=1):
+    def __init__(self, in_ch, out_ch, expand, k=3, act=True, stride=1, dilation_rate=1, track_running_stats=False):
         super().__init__()
 
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
         
         expand_ch = int(expand*in_ch)
 
         # expansion
-        self.conv1 = Conv(in_ch, expand_ch, k=1, act=self.act)
+        self.conv1 = Conv(in_ch, expand_ch, k=1, act=self.act, track_running_stats=track_running_stats)
 
         # depthwise
-        self.conv2 = DWConv(expand_ch, expand_ch, k=k, s=stride, d=dilation_rate, act=self.act)
+        self.conv2 = DWConv(expand_ch, expand_ch, k=k, s=stride, d=dilation_rate, act=self.act, track_running_stats=track_running_stats)
 
         # squeeze
-        self.conv3 = Conv(expand_ch, out_ch, k=1, act=False)
+        self.conv3 = Conv(expand_ch, out_ch, k=1, act=False, track_running_stats=track_running_stats)
 
         self.need_fuse = in_ch == out_ch
         self.need_pool = stride == 2
         if self.need_fuse and self.need_pool:
             self.pool = nn.MaxPool2d(2, stride=2)
 
         initialize_weights(self)
```

### Comparing `fdfat-0.1.4/fdfat/nn/model.py` & `fdfat-0.1.5/fdfat/nn/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,32 +30,32 @@
         csd = intersect_dicts(csd, self.state_dict())  # intersect
         self.load_state_dict(csd, strict=False)  # load
         if verbose:
             LOGGER.info(f'Transferred {len(csd)}/{len(self.state_dict())} items from pretrained weights')
 
 class LightWeightModel(BaseModel):
 
-    def __init__(self, imgz=128, muliplier=1, pose_rotation=False):
+    def __init__(self, imgz=128, muliplier=1, pose_rotation=False, track_running_stats=False):
         super().__init__()
         self.pose_rotation = pose_rotation
 
         # backbone, output size = size/4
-        self.backbone = module.LightWeightBackbone(muliplier=muliplier)
+        self.backbone = module.LightWeightBackbone(muliplier=muliplier, track_running_stats=track_running_stats)
 
         # mainstream, output size:
         # x1 = size/8
         # x2 = size/16
         # x3 = size/16
-        self.mainstream = module.MainStreamModule(muliplier=muliplier)
+        self.mainstream = module.MainStreamModule(muliplier=muliplier, track_running_stats=track_running_stats)
 
         if pose_rotation:
-            self.aux = module.AuxiliaryBackbone(int(16*muliplier), 3, muliplier=muliplier)
+            self.aux = module.AuxiliaryBackbone(int(16*muliplier), 3, muliplier=muliplier, track_running_stats=track_running_stats)
             
         output_ch = int((128 + 128 + 128)*muliplier)
-        self.logit = module.FERegress(output_ch, 70*2)
+        self.logit = module.FERegress(output_ch, 70*2, track_running_stats=track_running_stats)
 
         self.concat = Concat()
 
         initialize_weights(self)
 
     def forward(self, x):
 
@@ -71,56 +71,56 @@
         if self.pose_rotation:
             x = self.concat([x, aux])
 
         return x
 
 class LandmarkModel(BaseModel):
 
-    def __init__(self, imgz=128, muliplier=1, pose_rotation=False):
+    def __init__(self, imgz=128, muliplier=1, pose_rotation=False, track_running_stats=False):
         super().__init__()
         
         self.stack1 = nn.Sequential(
             nn.Conv2d( 3, int(32*muliplier), 3, stride=2, padding=2),
-            nn.BatchNorm2d(int(32*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(32*muliplier), track_running_stats=track_running_stats),
             nn.ReLU(),
             nn.Conv2d(int(32*muliplier), int(32*muliplier), 3, padding=1),
-            nn.BatchNorm2d(int(32*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(32*muliplier), track_running_stats=track_running_stats),
             nn.ReLU()
         )
 
         self.stack2 = nn.Sequential(
             nn.Conv2d(int(32*muliplier), int(64*muliplier), 3, stride=2, padding=2),
-            nn.BatchNorm2d(int(64*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(64*muliplier), track_running_stats=track_running_stats),
             nn.ReLU(),
             nn.Conv2d(int(64*muliplier), int(64*muliplier), 3, padding=1),
-            nn.BatchNorm2d(int(64*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(64*muliplier), track_running_stats=track_running_stats),
             nn.ReLU()
         )
 
         self.stack3 = nn.Sequential(
             nn.Conv2d(int(64*muliplier), int(128*muliplier), 3, stride=2, padding=2),
-            nn.BatchNorm2d(int(128*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(128*muliplier), track_running_stats=track_running_stats),
             nn.ReLU(),
             nn.Conv2d(int(128*muliplier), int(128*muliplier), 3, padding=1),
-            nn.BatchNorm2d(int(128*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(128*muliplier), track_running_stats=track_running_stats),
             nn.ReLU(),
             nn.Conv2d(int(128*muliplier), int(128*muliplier), 3, padding=1),
-            nn.BatchNorm2d(int(128*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(128*muliplier), track_running_stats=track_running_stats),
             nn.ReLU()
         )
 
         self.stack4 = nn.Sequential(
             nn.Conv2d(int(128*muliplier), int(256*muliplier), 3, stride=2, padding=2),
-            nn.BatchNorm2d(int(256*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(256*muliplier), track_running_stats=track_running_stats),
             nn.ReLU(),
             nn.Conv2d(int(256*muliplier), int(256*muliplier), 3, padding=1),
-            nn.BatchNorm2d(int(256*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(256*muliplier), track_running_stats=track_running_stats),
             nn.ReLU(),
             nn.Conv2d(int(256*muliplier), int(256*muliplier), 3, padding=1),
-            nn.BatchNorm2d(int(256*muliplier), track_running_stats=False),
+            nn.BatchNorm2d(int(256*muliplier), track_running_stats=track_running_stats),
             nn.ReLU(),
             nn.AdaptiveAvgPool2d((1, 1)),
         )
 
         self.stack5 = nn.Sequential(
             nn.Linear(int(256*muliplier), int(192*muliplier)),
             nn.Tanh(),
```

### Comparing `fdfat-0.1.4/fdfat/utils/logger.py` & `fdfat-0.1.5/fdfat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/utils/model_utils.py` & `fdfat-0.1.5/fdfat/utils/model_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,8 +145,12 @@
     """Returns a dictionary of intersecting keys with matching shapes, excluding 'exclude' keys, using da values."""
     return {k: v for k, v in da.items() if k in db and all(x not in k for x in exclude) and v.shape == db[k].shape}
 
 def preprocess(img_pil, imgsz):
     img_pil = img_pil.resize((imgsz, imgsz))
     img_np = np.array(img_pil)/127.5 - 1
     img_np = np.transpose(img_np, [2, 0, 1])[np.newaxis, ...]
-    return img_np
+    return img_np
+
+def get_latest_opset():
+    """Return second-most (for maturity) recently supported ONNX opset by this version of torch."""
+    return max(int(k[14:]) for k in vars(torch.onnx) if 'symbolic_opset' in k) - 1  # opset
```

### Comparing `fdfat-0.1.4/fdfat/utils/pose_estimation.py` & `fdfat-0.1.5/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat/utils/utils.py` & `fdfat-0.1.5/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/fdfat.egg-info/PKG-INFO` & `fdfat-0.1.5/fdfat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.4/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.5/fdfat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 fdfat/cfg/default_data.yaml
 fdfat/cfg/yaml_utils.py
 fdfat/cli/__init__.py
 fdfat/data/__init__.py
 fdfat/data/dataloader.py
 fdfat/engine/__init__.py
 fdfat/engine/base.py
+fdfat/engine/exporter.py
 fdfat/engine/tester.py
 fdfat/engine/trainer.py
 fdfat/engine/validator.py
 fdfat/engine/loop/__init__.py
 fdfat/engine/loop/tester.py
 fdfat/engine/loop/trainer.py
 fdfat/engine/loop/validator.py
```

### Comparing `fdfat-0.1.4/requirements.txt` & `fdfat-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.4/setup.py` & `fdfat-0.1.5/setup.py`

 * *Files identical despite different names*

