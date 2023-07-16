# Comparing `tmp/tensorwrap-0.0.1.1.tar.gz` & `tmp/tensorwrap-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorwrap-0.0.1.1.tar", last modified: Sun Jul 16 15:21:06 2023, max compression
+gzip compressed data, was "tensorwrap-0.0.1.2.tar", last modified: Sun Jul 16 17:14:13 2023, max compression
```

## Comparing `tensorwrap-0.0.1.1.tar` & `tensorwrap-0.0.1.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/
--rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/LICENSE
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6444 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)     5875 2023-05-27 02:36:24.000000 tensorwrap-0.0.1.1/README.md
--rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/setup.cfg
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1891 2023-07-15 21:24:36.000000 tensorwrap-0.0.1.1/setup.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.727131 tensorwrap-0.0.1.1/tensorwrap/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1549 2023-07-15 20:22:23.000000 tensorwrap-0.0.1.1/tensorwrap/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/config.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.728131 tensorwrap-0.0.1.1/tensorwrap/core/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       20 2023-06-16 00:46:59.000000 tensorwrap-0.0.1.1/tensorwrap/core/__init__.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.728131 tensorwrap-0.0.1.1/tensorwrap/core/losses/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      107 2023-06-16 00:41:45.000000 tensorwrap-0.0.1.1/tensorwrap/core/losses/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      419 2023-06-16 01:15:18.000000 tensorwrap-0.0.1.1/tensorwrap/core/losses/categorical.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      274 2023-06-15 22:56:13.000000 tensorwrap-0.0.1.1/tensorwrap/core/losses/mean.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/data.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/experimental/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      133 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/experimental/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/experimental/serialize.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/experimental/wrappers.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     2924 2023-07-16 14:25:46.000000 tensorwrap-0.0.1.1/tensorwrap/module.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      508 2023-07-15 20:45:34.000000 tensorwrap-0.0.1.1/tensorwrap/nn/__init__.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/activations/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       55 2023-07-16 14:48:55.000000 tensorwrap-0.0.1.1/tensorwrap/nn/activations/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1402 2023-07-16 14:54:01.000000 tensorwrap-0.0.1.1/tensorwrap/nn/activations/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/nn/callbacks.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/nn/checkpoints.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/initializers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      604 2023-07-15 21:02:53.000000 tensorwrap-0.0.1.1/tensorwrap/nn/initializers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      124 2023-07-15 20:56:21.000000 tensorwrap-0.0.1.1/tensorwrap/nn/initializers/base.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/layers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       51 2023-06-09 20:26:57.000000 tensorwrap-0.0.1.1/tensorwrap/nn/layers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     4484 2023-07-16 14:50:37.000000 tensorwrap-0.0.1.1/tensorwrap/nn/layers/base.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/tensorwrap/nn/losses/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      126 2023-06-16 01:05:54.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      371 2023-06-16 00:28:46.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      451 2023-06-16 00:41:32.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/categorical.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      697 2023-06-15 23:22:21.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/mean.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/tensorwrap/nn/models/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      102 2023-06-10 15:50:36.000000 tensorwrap-0.0.1.1/tensorwrap/nn/models/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     7455 2023-07-16 15:15:14.000000 tensorwrap-0.0.1.1/tensorwrap/nn/models/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)       71 2023-07-16 13:21:05.000000 tensorwrap-0.0.1.1/tensorwrap/nn/models/train.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/tensorwrap/nn/optimizers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       66 2023-06-09 19:51:14.000000 tensorwrap-0.0.1.1/tensorwrap/nn/optimizers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      775 2023-06-10 15:54:39.000000 tensorwrap-0.0.1.1/tensorwrap/nn/optimizers/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      663 2023-07-15 20:22:08.000000 tensorwrap-0.0.1.1/tensorwrap/ops.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-05-26 22:29:10.000000 tensorwrap-0.0.1.1/tensorwrap/test.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      110 2023-07-16 15:20:59.000000 tensorwrap-0.0.1.1/tensorwrap/version.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.728131 tensorwrap-0.0.1.1/tensorwrap.egg-info/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6444 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1191 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/SOURCES.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/dependency_links.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 15:17:39.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/not-zip-safe
--rw-r--r--   0 impureking  (1000) impureking  (1000)      315 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/requires.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/top_level.txt
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/LICENSE
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6345 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/README.md
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/setup.cfg
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1891 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/setup.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:12.999533 tensorwrap-0.0.1.2/tensorwrap/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1547 2023-07-16 17:11:32.000000 tensorwrap-0.0.1.2/tensorwrap/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/config.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap/core/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       20 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap/core/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      107 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      419 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      274 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/core/losses/mean.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/data.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap/experimental/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      133 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/experimental/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/experimental/serialize.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/experimental/wrappers.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     2924 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/module.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      562 2023-07-16 17:08:50.000000 tensorwrap-0.0.1.2/tensorwrap/nn/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/activations/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       55 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/activations/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1402 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/activations/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/nn/callbacks.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.2/tensorwrap/nn/checkpoints.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/initializers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      604 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/initializers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      124 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/initializers/base.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/layers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       51 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/layers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     4484 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/layers/base.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.001533 tensorwrap-0.0.1.2/tensorwrap/nn/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      126 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      371 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      451 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      697 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/losses/mean.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/tensorwrap/nn/models/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      102 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/models/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     7455 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/models/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       71 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/models/train.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.002533 tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       66 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      775 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      663 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.2/tensorwrap/ops.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-05-26 22:29:10.000000 tensorwrap-0.0.1.2/tensorwrap/test.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      110 2023-07-16 17:14:07.000000 tensorwrap-0.0.1.2/tensorwrap/version.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 17:14:13.000533 tensorwrap-0.0.1.2/tensorwrap.egg-info/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1191 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 17:13:28.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/not-zip-safe
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      315 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/requires.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-07-16 17:14:12.000000 tensorwrap-0.0.1.2/tensorwrap.egg-info/top_level.txt
```

### Comparing `tensorwrap-0.0.1.1/LICENSE` & `tensorwrap-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/PKG-INFO` & `tensorwrap-0.0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -23,17 +23,17 @@
 ![PyPI version](https://img.shields.io/pypi/v/tensorwrap)
 
 | [**Install guide**](#installation)
 
 
 ## What is TensorWrap?
 
-TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar feel of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
+TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar elements of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
 
-TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
+TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting its own explicit and magic free design philosophy. This allows TensorWrap to be fast and efficient, while remaining nearly fully compatible with all custom operations and other tools from the JAX ecosystem. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
 
 This is a personal project, not professionally affliated with Google in any way. Expect bugs and several incompatibilities/difference from the original libraries.
 Please help by trying it out, [reporting
 bugs](https://github.com/Impure-King/base-tensorwrap/issues), and letting me know what you
 think!
 
 ### Contents
@@ -54,27 +54,30 @@
 
 class Dense(nn.layers.Layer):
     def __init__(self, units) -> None:
         super().__init__() # Needed for tracking trainable_variables.
         self.units = units # Defining the output shape
   
     def build(self, input_shape: tuple) -> None:
+        super().build() # Required for letting model know that layer is built.
         input_shape = tf.shape(input_shape) # Getting appropriate input shape
         
         # Naming each parameter to later access from model.trainable_variables
         self.kernel = self.add_weights([input_shape, self.units],
                                        initializer = 'glorot_uniform',
                                        name='kernel')
         self.bias = self.add_weights([self.units],
                                      initializer = 'zeros',
                                      name='bias')
-        super().build() # Required for letting model know that layer is built.
+        
     
-    # Use call not __call__ to define the flow. No tf.function needed either.
-    def call(self, params, inputs):
+    # Use call not __call__ to define the flow. To support JIT compilation, we use staticmethod.
+    @staticmethod
+    @tf.function
+    def call(params, inputs):
         return inputs @ params['kernel'] + params['bias'] # Using params as an input, allows use to pass in the model.trainable_variables later.
  ```
 
 2) Just In Time Compiling with tf.function
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
@@ -84,19 +87,32 @@
 def mse(y_pred, y_true):
     return tf.mean(tf.square(y_pred - y_true))
 
 print(mse(100, 102))
 ```
 3) Custom Models
 ```python 
+import tensorwrap as tf
+from tensorwrap import nn
 
-class CheckPoint(Module):
-    def __init__(self, metrics) -> None:
-        
-
+class Sequential(nn.Model):
+    def __init__(self, layers: list) -> None:
+        super().__init__(name = "Sequential") # Starts the tracking of internal variables. Allows for name definition.
+        self.layers = layers
+
+    def __call__(self, inputs):
+        x = inputs
+        for layer in self.layers:
+            x = layer(x)
+        return x
+
+model = Sequential([
+    nn.layers.Dense(100),
+    nn.layers.Dense(10)
+])
 ```
 
 
 ### Current Gimmicks
 1. Current models are all compiled by JAX's internal jit, so any error may remain a bit more cryptic than PyTorchs. However, this problem is still being worked on.
 
 2. Also, using ``tensorwrap.Module`` is currently not recommended, since other superclasses offer more functionality and ease of use.
```

### Comparing `tensorwrap-0.0.1.1/README.md` & `tensorwrap-0.0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ![PyPI version](https://img.shields.io/pypi/v/tensorwrap)
 
 | [**Install guide**](#installation)
 
 
 ## What is TensorWrap?
 
-TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar feel of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
+TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar elements of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
 
-TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
+TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting its own explicit and magic free design philosophy. This allows TensorWrap to be fast and efficient, while remaining nearly fully compatible with all custom operations and other tools from the JAX ecosystem. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
 
 This is a personal project, not professionally affliated with Google in any way. Expect bugs and several incompatibilities/difference from the original libraries.
 Please help by trying it out, [reporting
 bugs](https://github.com/Impure-King/base-tensorwrap/issues), and letting me know what you
 think!
 
 ### Contents
@@ -38,27 +38,30 @@
 
 class Dense(nn.layers.Layer):
     def __init__(self, units) -> None:
         super().__init__() # Needed for tracking trainable_variables.
         self.units = units # Defining the output shape
   
     def build(self, input_shape: tuple) -> None:
+        super().build() # Required for letting model know that layer is built.
         input_shape = tf.shape(input_shape) # Getting appropriate input shape
         
         # Naming each parameter to later access from model.trainable_variables
         self.kernel = self.add_weights([input_shape, self.units],
                                        initializer = 'glorot_uniform',
                                        name='kernel')
         self.bias = self.add_weights([self.units],
                                      initializer = 'zeros',
                                      name='bias')
-        super().build() # Required for letting model know that layer is built.
+        
     
-    # Use call not __call__ to define the flow. No tf.function needed either.
-    def call(self, params, inputs):
+    # Use call not __call__ to define the flow. To support JIT compilation, we use staticmethod.
+    @staticmethod
+    @tf.function
+    def call(params, inputs):
         return inputs @ params['kernel'] + params['bias'] # Using params as an input, allows use to pass in the model.trainable_variables later.
  ```
 
 2) Just In Time Compiling with tf.function
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
@@ -68,19 +71,32 @@
 def mse(y_pred, y_true):
     return tf.mean(tf.square(y_pred - y_true))
 
 print(mse(100, 102))
 ```
 3) Custom Models
 ```python 
+import tensorwrap as tf
+from tensorwrap import nn
 
-class CheckPoint(Module):
-    def __init__(self, metrics) -> None:
-        
-
+class Sequential(nn.Model):
+    def __init__(self, layers: list) -> None:
+        super().__init__(name = "Sequential") # Starts the tracking of internal variables. Allows for name definition.
+        self.layers = layers
+
+    def __call__(self, inputs):
+        x = inputs
+        for layer in self.layers:
+            x = layer(x)
+        return x
+
+model = Sequential([
+    nn.layers.Dense(100),
+    nn.layers.Dense(10)
+])
 ```
 
 
 ### Current Gimmicks
 1. Current models are all compiled by JAX's internal jit, so any error may remain a bit more cryptic than PyTorchs. However, this problem is still being worked on.
 
 2. Also, using ``tensorwrap.Module`` is currently not recommended, since other superclasses offer more functionality and ease of use.
```

### Comparing `tensorwrap-0.0.1.1/setup.py` & `tensorwrap-0.0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/__init__.py` & `tensorwrap-0.0.1.2/tensorwrap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                             randu,
                             randn)
 
 # JAX Built-ins:
 from jax import (disable_jit,
                  value_and_grad,
                  grad)
-from jax.numpy import (array as Variable,
+from jax.numpy import (array as tensor,
                        arange as range,
                        expand_dims,
                        matmul,
                        square,
                        abs,
                        mean,
                        sum,
```

### Comparing `tensorwrap-0.0.1.1/tensorwrap/config.py` & `tensorwrap-0.0.1.2/tensorwrap/config.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/experimental/serialize.py` & `tensorwrap-0.0.1.2/tensorwrap/experimental/serialize.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/module.py` & `tensorwrap-0.0.1.2/tensorwrap/module.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/nn/activations/base.py` & `tensorwrap-0.0.1.2/tensorwrap/nn/activations/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/nn/initializers/__init__.py` & `tensorwrap-0.0.1.2/tensorwrap/nn/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/nn/layers/base.py` & `tensorwrap-0.0.1.2/tensorwrap/nn/layers/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/nn/losses/mean.py` & `tensorwrap-0.0.1.2/tensorwrap/nn/losses/mean.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/nn/models/base.py` & `tensorwrap-0.0.1.2/tensorwrap/nn/models/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/nn/optimizers/base.py` & `tensorwrap-0.0.1.2/tensorwrap/nn/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap/ops.py` & `tensorwrap-0.0.1.2/tensorwrap/ops.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.1/tensorwrap.egg-info/PKG-INFO` & `tensorwrap-0.0.1.2/tensorwrap.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -23,17 +23,17 @@
 ![PyPI version](https://img.shields.io/pypi/v/tensorwrap)
 
 | [**Install guide**](#installation)
 
 
 ## What is TensorWrap?
 
-TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar feel of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
+TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar elements of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
 
-TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
+TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting its own explicit and magic free design philosophy. This allows TensorWrap to be fast and efficient, while remaining nearly fully compatible with all custom operations and other tools from the JAX ecosystem. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
 
 This is a personal project, not professionally affliated with Google in any way. Expect bugs and several incompatibilities/difference from the original libraries.
 Please help by trying it out, [reporting
 bugs](https://github.com/Impure-King/base-tensorwrap/issues), and letting me know what you
 think!
 
 ### Contents
@@ -54,27 +54,30 @@
 
 class Dense(nn.layers.Layer):
     def __init__(self, units) -> None:
         super().__init__() # Needed for tracking trainable_variables.
         self.units = units # Defining the output shape
   
     def build(self, input_shape: tuple) -> None:
+        super().build() # Required for letting model know that layer is built.
         input_shape = tf.shape(input_shape) # Getting appropriate input shape
         
         # Naming each parameter to later access from model.trainable_variables
         self.kernel = self.add_weights([input_shape, self.units],
                                        initializer = 'glorot_uniform',
                                        name='kernel')
         self.bias = self.add_weights([self.units],
                                      initializer = 'zeros',
                                      name='bias')
-        super().build() # Required for letting model know that layer is built.
+        
     
-    # Use call not __call__ to define the flow. No tf.function needed either.
-    def call(self, params, inputs):
+    # Use call not __call__ to define the flow. To support JIT compilation, we use staticmethod.
+    @staticmethod
+    @tf.function
+    def call(params, inputs):
         return inputs @ params['kernel'] + params['bias'] # Using params as an input, allows use to pass in the model.trainable_variables later.
  ```
 
 2) Just In Time Compiling with tf.function
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
@@ -84,19 +87,32 @@
 def mse(y_pred, y_true):
     return tf.mean(tf.square(y_pred - y_true))
 
 print(mse(100, 102))
 ```
 3) Custom Models
 ```python 
+import tensorwrap as tf
+from tensorwrap import nn
 
-class CheckPoint(Module):
-    def __init__(self, metrics) -> None:
-        
-
+class Sequential(nn.Model):
+    def __init__(self, layers: list) -> None:
+        super().__init__(name = "Sequential") # Starts the tracking of internal variables. Allows for name definition.
+        self.layers = layers
+
+    def __call__(self, inputs):
+        x = inputs
+        for layer in self.layers:
+            x = layer(x)
+        return x
+
+model = Sequential([
+    nn.layers.Dense(100),
+    nn.layers.Dense(10)
+])
 ```
 
 
 ### Current Gimmicks
 1. Current models are all compiled by JAX's internal jit, so any error may remain a bit more cryptic than PyTorchs. However, this problem is still being worked on.
 
 2. Also, using ``tensorwrap.Module`` is currently not recommended, since other superclasses offer more functionality and ease of use.
```

### Comparing `tensorwrap-0.0.1.1/tensorwrap.egg-info/SOURCES.txt` & `tensorwrap-0.0.1.2/tensorwrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

