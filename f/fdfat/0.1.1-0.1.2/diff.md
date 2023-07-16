# Comparing `tmp/fdfat-0.1.1.tar.gz` & `tmp/fdfat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.1.tar", last modified: Tue Jul 11 13:34:53 2023, max compression
+gzip compressed data, was "fdfat-0.1.2.tar", last modified: Sun Jul 16 03:28:33 2023, max compression
```

## Comparing `fdfat-0.1.1.tar` & `fdfat-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.985430 fdfat-0.1.1/
--rw-r--r--   0 ryan       (501) staff       (20)     2625 2023-07-11 13:34:53.985297 fdfat-0.1.1/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     1344 2023-07-11 11:22:59.000000 fdfat-0.1.1/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.978545 fdfat-0.1.1/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      240 2023-07-11 13:34:26.000000 fdfat-0.1.1/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.979502 fdfat-0.1.1/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4678 2023-07-11 12:42:35.000000 fdfat-0.1.1/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.979864 fdfat-0.1.1/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)      433 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.980306 fdfat-0.1.1/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.1/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4202 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.981238 fdfat-0.1.1/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 07:53:43.000000 fdfat-0.1.1/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/engine/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     2702 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2113 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/engine/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     6862 2023-07-11 13:34:19.000000 fdfat-0.1.1/fdfat/main.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.981601 fdfat-0.1.1/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.1/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.1/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.983549 fdfat-0.1.1/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.1/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-10 01:40:50.000000 fdfat-0.1.1/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     6047 2023-07-10 01:40:40.000000 fdfat-0.1.1/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     4920 2023-07-09 05:55:54.000000 fdfat-0.1.1/fdfat/nn/module.py
--rw-r--r--   0 ryan       (501) staff       (20)     4925 2023-07-09 05:19:14.000000 fdfat-0.1.1/fdfat/nn/module2.py
--rw-r--r--   0 ryan       (501) staff       (20)     4925 2023-07-10 01:41:37.000000 fdfat-0.1.1/fdfat/nn/module3.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.984934 fdfat-0.1.1/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.1/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7031 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.1/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-10 09:42:57.000000 fdfat-0.1.1/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.979268 fdfat-0.1.1/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     2625 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      728 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-11 13:34:53.985477 fdfat-0.1.1/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-11 11:16:04.000000 fdfat-0.1.1/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.862378 fdfat-0.1.2/
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 03:28:33.862227 fdfat-0.1.2/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.2/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.855740 fdfat-0.1.2/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      240 2023-07-16 03:28:06.000000 fdfat-0.1.2/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.856890 fdfat-0.1.2/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4688 2023-07-13 09:29:43.000000 fdfat-0.1.2/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.2/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.857260 fdfat-0.1.2/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)     1040 2023-07-16 03:13:54.000000 fdfat-0.1.2/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.857555 fdfat-0.1.2/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.2/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4202 2023-07-11 11:08:58.000000 fdfat-0.1.2/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.858686 fdfat-0.1.2/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.2/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2946 2023-07-16 03:15:10.000000 fdfat-0.1.2/fdfat/engine/base.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.859215 fdfat-0.1.2/fdfat/engine/loop/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.2/fdfat/engine/loop/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/engine/loop/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2702 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/engine/loop/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2113 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/engine/loop/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 03:16:47.000000 fdfat-0.1.2/fdfat/engine/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.2/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.2/fdfat/engine/validator.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.859464 fdfat-0.1.2/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.2/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.2/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.860398 fdfat-0.1.2/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.2/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-14 01:18:16.000000 fdfat-0.1.2/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4714 2023-07-16 03:26:38.000000 fdfat-0.1.2/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5150 2023-07-14 01:18:47.000000 fdfat-0.1.2/fdfat/nn/module.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.861758 fdfat-0.1.2/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.2/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.2/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7505 2023-07-13 09:25:48.000000 fdfat-0.1.2/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.2/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.2/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 03:28:33.856421 fdfat-0.1.2/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      813 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 03:28:33.000000 fdfat-0.1.2/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 03:28:33.862426 fdfat-0.1.2/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-11 11:16:04.000000 fdfat-0.1.2/setup.py
```

### Comparing `fdfat-0.1.1/fdfat/cfg/__init__.py` & `fdfat-0.1.2/fdfat/cfg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Union
 
 from fdfat.cfg.yaml_utils import yaml_load, yaml_save, yaml_print, DEFAULT_CFG_DICT, DEFAULT_CFG_DATA, IterableSimpleNamespace
 
 CFG_INT_KEYS= 'seed', 'workers', 'imgsz', 'epoch', 'batch_size', 'dump_batch', 'patience', 'warmup'
 CFG_FRACTION_KEYS = ('lr', 'lr0_factor', 'lr_factor', 'aux_pose_weight')
 CFG_FLOAT_KEYS = ("aug", 'muliplier', 'w_jaw', 'w_leyeb', 'w_reyeb', 'w_nose', 'w_nosetip', 'w_leye', 'w_reye', 'w_mount', 'w_purpil')
-CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled", "resume")
+CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled", "resume", "warmup")
 
 def cfg2dict(cfg):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Inputs:
         cfg (str) or (Path) or (SimpleNamespace): Configuration object to be converted to a dictionary.
```

### Comparing `fdfat-0.1.1/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.2/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/data/dataloader.py` & `fdfat-0.1.2/fdfat/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/engine/tester.py` & `fdfat-0.1.2/fdfat/engine/loop/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/engine/trainer.py` & `fdfat-0.1.2/fdfat/engine/loop/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/engine/validator.py` & `fdfat-0.1.2/fdfat/engine/loop/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/metric/metric.py` & `fdfat-0.1.2/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/nn/conv.py` & `fdfat-0.1.2/fdfat/nn/conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         return torch.cat(x, self.d)
 
 
 class IdentifyBlock(nn.Module):
 
     default_act = nn.ReLU6()  # default activation
 
-    def __init__(self, in_ch, out_ch, expand, k=3, act=None, stride=1, dilation_rate=1):
+    def __init__(self, in_ch, out_ch, expand, k=3, act=True, stride=1, dilation_rate=1):
         super().__init__()
 
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
         
         expand_ch = int(expand*in_ch)
 
         # expansion
```

### Comparing `fdfat-0.1.1/fdfat/nn/module.py` & `fdfat-0.1.2/fdfat/nn/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 from .conv import *
         
 class LightWeightBackbone(nn.Module):
 
     default_act = nn.ReLU6()  # default activation
 
-    def __init__(self, expand_rate=2, muliplier=1, act=None):
+    def __init__(self, expand_rate=2, muliplier=1, act=True):
         super().__init__()
 
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
         # early dropout
-        self.conv11 = Conv(3, 16, s=2, act=nn.PReLU())
+        self.conv11 = Conv(3, 16, k=3, s=2, act=nn.PReLU())
 
         self.conv21 = IdentifyBlock(16, int(16*muliplier), expand_rate, stride=2, act=self.act)
         self.conv22 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
         self.conv23 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
         self.conv24 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
         self.conv25 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
 
@@ -32,34 +32,34 @@
         x = self.conv24(x)
         x = self.conv25(x)
 
         return x
     
 class AuxiliaryBackbone(nn.Module):
 
-    default_act = nn.PReLU()  # default activation
+    default_act = nn.ReLU6()  # default activation
 
-    def __init__(self, in_ch, out_ch, muliplier=1, act=None):
+    def __init__(self, in_ch, out_ch, muliplier=1, act=True):
         super().__init__()
 
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
         self.stack1 = nn.Sequential(
             nn.Conv2d(in_ch, int(32*muliplier), 3, 2, autopad(3)),
             nn.BatchNorm2d(int(32*muliplier), track_running_stats=False),
-            nn.PReLU(),
+            self.act,
             nn.Conv2d(int(32*muliplier), int(64*muliplier), 3, 1, autopad(3)),
             nn.BatchNorm2d(int(64*muliplier), track_running_stats=False),
-            nn.PReLU(),
+            self.act,
             nn.Conv2d(int(64*muliplier), int(64*muliplier), 3, 2, autopad(3)),
             nn.BatchNorm2d(int(64*muliplier), track_running_stats=False),
-            nn.PReLU(),
+            self.act,
             nn.Conv2d(int(64*muliplier), int(128*muliplier), 3, 1, autopad(3)),
             nn.BatchNorm2d(int(128*muliplier), track_running_stats=False),
-            nn.PReLU(),
+            self.act,
             nn.AdaptiveAvgPool2d((1, 1)),
         )
 
         self.stack2 = nn.Sequential(
             nn.Linear(int(128*muliplier), out_ch*3),
             nn.Tanh(),
             nn.Linear(out_ch*3, out_ch),
@@ -75,31 +75,33 @@
         x = self.stack2(x)
 
         return x
     
 class MainStreamModule(nn.Module):
     default_act = nn.ReLU6()  # default activation
 
-    def __init__(self, expand_rate=2, muliplier=1, act=None):
+    def __init__(self, expand_rate=2, muliplier=1, act=True):
         super().__init__()
 
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
         self.conv11 = IdentifyBlock(int(16*muliplier), int(32*muliplier), expand_rate, stride=2, act=self.act)
 
         self.conv21 = IdentifyBlock(int(32*muliplier), int(32*muliplier), expand_rate*2, stride=1, act=self.act)
         self.conv22 = IdentifyBlock(int(32*muliplier), int(32*muliplier), expand_rate*2, stride=1, act=self.act)
-        self.conv23 = IdentifyBlock(int(32*muliplier), int(32*muliplier), expand_rate*2, stride=1, act=self.act)
-        self.conv24 = IdentifyBlock(int(32*muliplier), int(32*muliplier), expand_rate*2, stride=1, act=self.act)
-        self.conv25 = IdentifyBlock(int(32*muliplier), int(32*muliplier), expand_rate*2, stride=1, act=self.act)
+        self.conv23 = IdentifyBlock(int(32*muliplier), int(64*muliplier), expand_rate*2, stride=1, act=self.act)
+        self.conv24 = IdentifyBlock(int(64*muliplier), int(64*muliplier), expand_rate*2, stride=1, act=self.act)
+        self.conv25 = IdentifyBlock(int(64*muliplier), int(64*muliplier), expand_rate*2, stride=1, act=self.act)
 
         # Pyramic scale
-        self.convp1 = IdentifyBlock(int(32*muliplier), int(64*muliplier), expand_rate, stride=1, act=self.act)
-        self.convp2 = Conv(int(64*muliplier), int(64*muliplier), k=3, s=2, act=nn.PReLU())
-        self.convp3 = Conv(int(64*muliplier), int(64*muliplier), k=5, act=nn.PReLU())
+        self.convp1 = IdentifyBlock(int(64*muliplier), int(128*muliplier), expand_rate, stride=1, act=self.act)
+        self.convp2 = IdentifyBlock(int(128*muliplier), int(128*muliplier), expand_rate, stride=2, act=self.act)
+        self.convp3 = IdentifyBlock(int(128*muliplier), int(128*muliplier), expand_rate, stride=1, act=self.act)
+        # self.convp2 = Conv(int(128*muliplier), int(128*muliplier), k=3, s=2, act=nn.SiLU())
+        # self.convp3 = Conv(int(128*muliplier), int(128*muliplier), k=3, act=nn.SiLU())
 
         self.concat = Concat()
         self.global_pool = nn.AdaptiveAvgPool2d((1, 1))
 
         initialize_weights(self)
 
     def forward(self, x):
```

### Comparing `fdfat-0.1.1/fdfat/utils/logger.py` & `fdfat-0.1.2/fdfat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/utils/model_utils.py` & `fdfat-0.1.2/fdfat/utils/model_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,8 +135,18 @@
         # Prefer MPS if available
         s += 'MPS\n'
         arg = 'mps'
     else:  # revert to CPU
         s += 'CPU\n'
         arg = 'cpu'
 
-    return torch.device(arg)
+    return torch.device(arg)
+
+def intersect_dicts(da, db, exclude=()):
+    """Returns a dictionary of intersecting keys with matching shapes, excluding 'exclude' keys, using da values."""
+    return {k: v for k, v in da.items() if k in db and all(x not in k for x in exclude) and v.shape == db[k].shape}
+
+def preprocess(img_pil, imgsz):
+    img_pil = img_pil.resize((imgsz, imgsz))
+    img_np = np.array(img_pil)/127.5 - 1
+    img_np = np.transpose(img_np, [2, 0, 1])[np.newaxis, ...]
+    return img_np
```

### Comparing `fdfat-0.1.1/fdfat/utils/pose_estimation.py` & `fdfat-0.1.2/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat/utils/utils.py` & `fdfat-0.1.2/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.1/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.2/fdfat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 README.md
 setup.py
 fdfat/__init__.py
-fdfat/main.py
 fdfat.egg-info/PKG-INFO
 fdfat.egg-info/SOURCES.txt
 fdfat.egg-info/dependency_links.txt
 fdfat.egg-info/entry_points.txt
 fdfat.egg-info/requires.txt
 fdfat.egg-info/top_level.txt
 fdfat/cfg/__init__.py
 fdfat/cfg/yaml_utils.py
 fdfat/cli/__init__.py
 fdfat/data/__init__.py
 fdfat/data/dataloader.py
 fdfat/engine/__init__.py
+fdfat/engine/base.py
 fdfat/engine/tester.py
 fdfat/engine/trainer.py
 fdfat/engine/validator.py
+fdfat/engine/loop/__init__.py
+fdfat/engine/loop/tester.py
+fdfat/engine/loop/trainer.py
+fdfat/engine/loop/validator.py
 fdfat/metric/__init__.py
 fdfat/metric/metric.py
 fdfat/nn/__init__.py
 fdfat/nn/conv.py
 fdfat/nn/model.py
 fdfat/nn/module.py
-fdfat/nn/module2.py
-fdfat/nn/module3.py
 fdfat/utils/__init__.py
 fdfat/utils/logger.py
 fdfat/utils/model_utils.py
 fdfat/utils/pose_estimation.py
 fdfat/utils/utils.py
```

### Comparing `fdfat-0.1.1/setup.py` & `fdfat-0.1.2/setup.py`

 * *Files identical despite different names*

