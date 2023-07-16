# Comparing `tmp/tensorwrap-0.0.1.2.tar.gz` & `tmp/tensorwrap-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorwrap-0.0.1.2.tar", last modified: Sun Jul 16 17:14:13 2023, max compression
+gzip compressed data, was "tensorwrap-0.0.1.3.tar", last modified: Sun Jul 16 19:59:58 2023, max compression
```

## Comparing `tensorwrap-0.0.1.2.tar` & `tensorwrap-0.0.1.3.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/
--rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/LICENSE
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6345 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/README.md
--rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/setup.cfg
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1891 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/setup.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:12.999533 tensorwrap-0.0.1.2/tensorwrap/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1547 2023-07-16 17:11:32.000000 tensorwrap-0.0.1.2/tensorwrap/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/config.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap/core/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       20 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/__init__.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap/core/losses/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      107 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/losses/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      419 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/losses/categorical.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      274 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/losses/mean.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/data.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap/experimental/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      133 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/experimental/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/experimental/serialize.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/experimental/wrappers.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     2924 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/module.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      562 2023-07-16 17:08:50.000000 tensorwrap-0.0.1.2/tensorwrap/nn/__init__.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/activations/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       55 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/activations/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1402 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/activations/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/nn/callbacks.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/nn/checkpoints.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/initializers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      604 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/initializers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      124 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/initializers/base.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/layers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       51 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/layers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     4484 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/layers/base.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/losses/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      126 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      371 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      451 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/categorical.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      697 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/mean.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/tensorwrap/nn/models/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      102 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/models/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     7455 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/models/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)       71 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/models/train.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       66 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      775 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      663 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/ops.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-05-26 22:29:10.000000 tensorwrap-0.0.1.2/tensorwrap/test.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      110 2023-07-16 17:14:07.000000 tensorwrap-0.0.1.2/tensorwrap/version.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap.egg-info/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1191 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/SOURCES.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/dependency_links.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 17:13:28.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/not-zip-safe
--rw-r--r--   0 impureking  (1000) impureking  (1000)      315 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/requires.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/top_level.txt
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/LICENSE
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6345 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/README.md
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/setup.cfg
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1918 2023-07-16 18:50:48.000000 tensorwrap-0.0.1.3/setup.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.161547 tensorwrap-0.0.1.3/tensorwrap/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1609 2023-07-16 18:43:03.000000 tensorwrap-0.0.1.3/tensorwrap/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/config.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap/core/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       20 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap/core/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      107 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      419 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      274 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/losses/mean.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/data.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap/experimental/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      133 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/experimental/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/experimental/serialize.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/experimental/wrappers.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     2924 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/module.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      562 2023-07-16 17:08:50.000000 tensorwrap-0.0.1.3/tensorwrap/nn/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/activations/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       55 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/activations/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1402 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/activations/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/nn/callbacks.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/nn/checkpoints.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/initializers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      604 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/initializers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      124 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/initializers/base.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/layers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      125 2023-07-16 19:58:59.000000 tensorwrap-0.0.1.3/tensorwrap/nn/layers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     4489 2023-07-16 17:43:32.000000 tensorwrap-0.0.1.3/tensorwrap/nn/layers/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      629 2023-07-16 19:55:13.000000 tensorwrap-0.0.1.3/tensorwrap/nn/layers/lambda_layers.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/tensorwrap/nn/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      156 2023-07-16 19:04:47.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      371 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      585 2023-07-16 19:55:31.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      697 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/mean.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      912 2023-07-16 19:03:35.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/metrics.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/tensorwrap/nn/models/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      102 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/models/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     7384 2023-07-16 17:34:25.000000 tensorwrap-0.0.1.3/tensorwrap/nn/models/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       71 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/models/train.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       66 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      775 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      663 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/ops.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-05-26 22:29:10.000000 tensorwrap-0.0.1.3/tensorwrap/test.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      110 2023-07-16 19:59:53.000000 tensorwrap-0.0.1.3/tensorwrap/version.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap.egg-info/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1261 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/not-zip-safe
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      335 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/requires.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/top_level.txt
```

### Comparing `tensorwrap-0.0.1.2/LICENSE` & `tensorwrap-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/PKG-INFO` & `tensorwrap-0.0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tensorwrap-0.0.1.2/README.md` & `tensorwrap-0.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/setup.py` & `tensorwrap-0.0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     "numpy>=1.12",
     "jax>=0.3.16",
     "jaxlib",
     "dill",
     "matplotlib",  # only needed for tensorboard export
     "pandas",
     "jaxtyping",
-    "optax"
+    "optax",
+    "tensorflow-datasets"
 ]
 
 tests_require = [
     "atari-py==0.2.5",  # Last version does not have the ROMs we test on pre-packaged
     "clu",  # All examples.
     "gym==0.18.3",
     "jaxlib",
```

### Comparing `tensorwrap-0.0.1.2/tensorwrap/__init__.py` & `tensorwrap-0.0.1.3/tensorwrap/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,8 +40,10 @@
                        eye as identity,
                        shape,
                        prod,
                        max,
                        min,
                        maximum,
                        minimum,
-                       zeros)
+                       zeros,
+                       argmax,
+                       argmin)
```

### Comparing `tensorwrap-0.0.1.2/tensorwrap/config.py` & `tensorwrap-0.0.1.3/tensorwrap/config.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/experimental/serialize.py` & `tensorwrap-0.0.1.3/tensorwrap/experimental/serialize.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/module.py` & `tensorwrap-0.0.1.3/tensorwrap/module.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/nn/__init__.py` & `tensorwrap-0.0.1.3/tensorwrap/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/nn/activations/base.py` & `tensorwrap-0.0.1.3/tensorwrap/nn/activations/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/nn/initializers/__init__.py` & `tensorwrap-0.0.1.3/tensorwrap/nn/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/nn/layers/base.py` & `tensorwrap-0.0.1.3/tensorwrap/nn/layers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         self.build(inputs)
         self.built=True
         return self.trainable_variables
 
     def compute_output_shape(self):
         raise NotImplementedError("Method `compute_output_shape` has not been implemented.")
 
+    
     @final
     def __call__(self, params: dict, inputs: Array):
         if not self.built:
             self.init_params(inputs)
             params = self.trainable_variables
         out = self.call(params, inputs)
         return out
```

### Comparing `tensorwrap-0.0.1.2/tensorwrap/nn/losses/mean.py` & `tensorwrap-0.0.1.3/tensorwrap/nn/losses/mean.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/nn/models/base.py` & `tensorwrap-0.0.1.3/tensorwrap/nn/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,16 +158,14 @@
 
         NOTE: Doesn't support batching and requires initiating of parameters and compilation of loss function
         and optimizers.
         """
         if epochs < 1:
             raise ValueError("Epochs must be a positive value.")
 
-        # Jitting Trainstep:
-        # step = jax.jit(self.train_step)
 
         for epoch in range(1, epochs + 1):
             self.trainable_variables, (loss, pred) = self.train_step(self.trainable_variables, x_train, y_train)
             metric = self.metrics(y_train, pred)
             print(f"Epoch: {epoch} \t\t Loss: {loss:.5f} \t\t Metrics: {metric:.5f}")
```

### Comparing `tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/base.py` & `tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap/ops.py` & `tensorwrap-0.0.1.3/tensorwrap/ops.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.2/tensorwrap.egg-info/PKG-INFO` & `tensorwrap-0.0.1.3/tensorwrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tensorwrap-0.0.1.2/tensorwrap.egg-info/SOURCES.txt` & `tensorwrap-0.0.1.3/tensorwrap.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 tensorwrap/nn/checkpoints.py
 tensorwrap/nn/activations/__init__.py
 tensorwrap/nn/activations/base.py
 tensorwrap/nn/initializers/__init__.py
 tensorwrap/nn/initializers/base.py
 tensorwrap/nn/layers/__init__.py
 tensorwrap/nn/layers/base.py
+tensorwrap/nn/layers/lambda_layers.py
 tensorwrap/nn/losses/__init__.py
 tensorwrap/nn/losses/base.py
 tensorwrap/nn/losses/categorical.py
 tensorwrap/nn/losses/mean.py
+tensorwrap/nn/losses/metrics.py
 tensorwrap/nn/models/__init__.py
 tensorwrap/nn/models/base.py
 tensorwrap/nn/models/train.py
 tensorwrap/nn/optimizers/__init__.py
 tensorwrap/nn/optimizers/base.py
```

