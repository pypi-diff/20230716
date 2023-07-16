# Comparing `tmp/doy-1.3.1.tar.gz` & `tmp/doy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-1.3.1.tar", max compression
+gzip compressed data, was "doy-1.3.2.tar", max compression
```

## Comparing `doy-1.3.1.tar` & `doy-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.3.1/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.3.1/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     1277 2023-07-13 13:37:12.584726 doy-1.3.1/doy/.unused.py
--rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.3.1/doy/__init__.py
--rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.3.1/doy/data.py
--rw-r--r--   0        0        0     1542 2023-07-16 14:48:24.576188 doy-1.3.1/doy/logger.py
--rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.3.1/doy/plotting.py
--rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.3.1/doy/progress.py
--rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.3.1/doy/rich_utils.py
--rw-r--r--   0        0        0     4774 2023-07-16 14:22:10.927178 doy-1.3.1/doy/utils.py
--rw-r--r--   0        0        0      362 2023-07-16 14:48:33.828265 doy-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 doy-1.3.1/setup.py
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 doy-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.3.2/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.3.2/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     1277 2023-07-13 13:37:12.584726 doy-1.3.2/doy/.unused.py
+-rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.3.2/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.3.2/doy/data.py
+-rw-r--r--   0        0        0     1542 2023-07-16 14:48:24.576188 doy-1.3.2/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.3.2/doy/plotting.py
+-rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.3.2/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.3.2/doy/rich_utils.py
+-rw-r--r--   0        0        0     4775 2023-07-16 15:21:29.692855 doy-1.3.2/doy/utils.py
+-rw-r--r--   0        0        0      362 2023-07-16 15:21:33.628888 doy-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 doy-1.3.2/setup.py
+-rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 doy-1.3.2/PKG-INFO
```

### Comparing `doy-1.3.1/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.3.2/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-1.3.1/doy/.unused.py` & `doy-1.3.2/doy/.unused.py`

 * *Files identical despite different names*

### Comparing `doy-1.3.1/doy/data.py` & `doy-1.3.2/doy/data.py`

 * *Files identical despite different names*

### Comparing `doy-1.3.1/doy/logger.py` & `doy-1.3.2/doy/logger.py`

 * *Files identical despite different names*

### Comparing `doy-1.3.1/doy/plotting.py` & `doy-1.3.2/doy/plotting.py`

 * *Files identical despite different names*

### Comparing `doy-1.3.1/doy/progress.py` & `doy-1.3.2/doy/progress.py`

 * *Files identical despite different names*

### Comparing `doy-1.3.1/doy/rich_utils.py` & `doy-1.3.2/doy/rich_utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.3.1/doy/utils.py` & `doy-1.3.2/doy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         **kwargs,
     ):
         opt_param_groups = []
         self.schedules = []
 
         for name, (schedule, modules) in param_groups.items():
             opt_param_groups.append(
-                {"params": get_params_from_modules(modules), "lr": schedule(0)}
+                {"params": get_params_from_modules(*modules), "lr": schedule(0)}
             )
             self.schedules.append((name, schedule))
 
         self.opt = opt_cls(params=opt_param_groups, **kwargs)
 
     @classmethod
     def make(
```

### Comparing `doy-1.3.1/setup.py` & `doy-1.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0', 'wandb>=0.15.5']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `doy-1.3.1/PKG-INFO` & `doy-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doy
-Version: 1.3.1
+Version: 1.3.2
 Summary: 
 Author: Dominik Schmidt
 Author-email: schmidtdominik30@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

