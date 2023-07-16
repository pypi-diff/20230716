# Comparing `tmp/doy-1.2.tar.gz` & `tmp/doy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-1.2.tar", max compression
+gzip compressed data, was "doy-1.3.tar", max compression
```

## Comparing `doy-1.2.tar` & `doy-1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.2/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.2/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.2/doy/__init__.py
--rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.2/doy/data.py
--rw-r--r--   0        0        0     1482 2023-07-12 13:55:22.467360 doy-1.2/doy/logger.py
--rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.2/doy/plotting.py
--rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.2/doy/progress.py
--rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.2/doy/rich_utils.py
--rw-r--r--   0        0        0     2948 2023-07-13 11:03:55.427841 doy-1.2/doy/utils.py
--rw-r--r--   0        0        0      360 2023-07-13 11:04:06.411932 doy-1.2/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 doy-1.2/setup.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 doy-1.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.3/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.3/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     1277 2023-07-13 13:37:12.584726 doy-1.3/doy/.unused.py
+-rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.3/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.3/doy/data.py
+-rw-r--r--   0        0        0     1469 2023-07-16 13:41:36.146818 doy-1.3/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.3/doy/plotting.py
+-rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.3/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.3/doy/rich_utils.py
+-rw-r--r--   0        0        0     4774 2023-07-16 14:01:14.840805 doy-1.3/doy/utils.py
+-rw-r--r--   0        0        0      360 2023-07-16 14:01:23.428876 doy-1.3/pyproject.toml
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 doy-1.3/setup.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 doy-1.3/PKG-INFO
```

### Comparing `doy-1.2/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.3/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-1.2/doy/data.py` & `doy-1.3/doy/data.py`

 * *Files identical despite different names*

### Comparing `doy-1.2/doy/logger.py` & `doy-1.3/doy/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections import defaultdict
-from doy.utils import smooth_ema, smooth_conv
-from typing import Optional, Union
-import os
-import wandb
-import doy
+from typing import Optional
+
 import numpy as np
 
+from doy.utils import smooth_conv, smooth_ema
+
 
 class Logger:
     def __init__(self, use_wandb: bool = True):
         self.data = defaultdict(list)
         self.data_x = defaultdict(list)
         self.use_wandb = use_wandb
 
@@ -25,14 +24,16 @@
             except AttributeError:
                 pass
 
             self.data[k].append(v)
             self.data_x[k].append(step)
 
         if self.use_wandb:
+            import wandb
+
             wandb.log(data=kwargs, step=step)
 
     def __getitem__(self, key):
         return np.array(self.data[key])
 
     def get(self, key, smooth_args: Optional[tuple] = ("ema", 0.9)):
         if smooth_args is None:
```

### Comparing `doy-1.2/doy/plotting.py` & `doy-1.3/doy/plotting.py`

 * *Files identical despite different names*

### Comparing `doy-1.2/doy/progress.py` & `doy-1.3/doy/progress.py`

 * *Files identical despite different names*

### Comparing `doy-1.2/doy/rich_utils.py` & `doy-1.3/doy/rich_utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.2/setup.py` & `doy-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0', 'wandb>=0.15.5']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '1.2',
+    'version': '1.3',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `doy-1.2/PKG-INFO` & `doy-1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doy
-Version: 1.2
+Version: 1.3
 Summary: 
 Author: Dominik Schmidt
 Author-email: schmidtdominik30@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

