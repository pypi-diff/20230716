# Comparing `tmp/ml4s-0.0.2.tar.gz` & `tmp/ml4s-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ml4s-0.0.2.tar", last modified: Fri Jul 14 15:55:38 2023, max compression
+gzip compressed data, was "dist\ml4s-0.1.0.tar", last modified: Sat Jul 15 22:05:16 2023, max compression
```

## Comparing `ml4s-0.0.2.tar` & `ml4s-0.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:38.159747 ml4s-0.0.2/
--rw-rw-rw-   0        0        0      105 2023-07-14 14:43:53.000000 ml4s-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4556 2023-07-14 15:55:38.159747 ml4s-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    12063 2023-07-14 15:50:55.000000 ml4s-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:37.912929 ml4s-0.0.2/ml4s/
--rw-rw-rw-   0        0        0        5 2023-06-14 14:39:12.000000 ml4s-0.0.2/ml4s/VERSION
--rw-rw-rw-   0        0        0     1090 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/__init__.py
--rw-rw-rw-   0        0        0     8432 2023-07-14 14:43:37.000000 ml4s-0.0.2/ml4s/_troubleshoot.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:38.033111 ml4s-0.0.2/ml4s/backend/
--rw-rw-rw-   0        0        0     1140 2023-06-14 08:33:28.000000 ml4s-0.0.2/ml4s/backend/__init__.py
--rw-rw-rw-   0        0        0    71763 2023-07-14 14:43:38.000000 ml4s-0.0.2/ml4s/backend/_backend.py
--rw-rw-rw-   0        0        0     6142 2023-06-19 15:56:23.000000 ml4s-0.0.2/ml4s/backend/_dtype.py
--rw-rw-rw-   0        0        0    38859 2023-07-14 14:43:37.000000 ml4s-0.0.2/ml4s/backend/_linalg.py
--rw-rw-rw-   0        0        0     3101 2023-06-11 18:52:32.000000 ml4s-0.0.2/ml4s/backend/_linalg_preconditioner.py
--rw-rw-rw-   0        0        0     9048 2023-06-11 18:52:32.000000 ml4s-0.0.2/ml4s/backend/_minimize.py
--rw-rw-rw-   0        0        0    20027 2023-06-16 08:55:17.000000 ml4s-0.0.2/ml4s/backend/_numpy_backend.py
--rw-rw-rw-   0        0        0     1345 2023-06-14 08:33:28.000000 ml4s-0.0.2/ml4s/backend/_object.py
--rw-rw-rw-   0        0        0    19229 2023-06-11 18:52:32.000000 ml4s-0.0.2/ml4s/backend/_partition.py
--rw-rw-rw-   0        0        0    22492 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/backend/_profile.py
--rw-rw-rw-   0        0        0      449 2023-06-11 18:52:32.000000 ml4s-0.0.2/ml4s/backend/_triangular_wip.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:38.053137 ml4s-0.0.2/ml4s/backend/jax/
--rw-rw-rw-   0        0        0      163 2023-06-12 21:40:30.000000 ml4s-0.0.2/ml4s/backend/jax/__init__.py
--rw-rw-rw-   0        0        0    25135 2023-06-19 16:24:52.000000 ml4s-0.0.2/ml4s/backend/jax/_jax_backend.py
--rw-rw-rw-   0        0        0    39603 2023-07-14 14:43:37.000000 ml4s-0.0.2/ml4s/backend/jax/stax_nets.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:38.095173 ml4s-0.0.2/ml4s/backend/tensorflow/
--rw-rw-rw-   0        0        0      906 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/backend/tensorflow/__init__.py
--rw-rw-rw-   0        0        0     4228 2023-06-12 21:40:30.000000 ml4s-0.0.2/ml4s/backend/tensorflow/_compile_cuda.py
--rw-rw-rw-   0        0        0     1950 2023-06-12 21:40:30.000000 ml4s-0.0.2/ml4s/backend/tensorflow/_profiling.py
--rw-rw-rw-   0        0        0    34022 2023-06-19 16:10:01.000000 ml4s-0.0.2/ml4s/backend/tensorflow/_tf_backend.py
--rw-rw-rw-   0        0        0     3280 2023-06-12 21:40:30.000000 ml4s-0.0.2/ml4s/backend/tensorflow/_tf_cuda_resample.py
--rw-rw-rw-   0        0        0    24962 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/backend/tensorflow/nets.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:38.108183 ml4s-0.0.2/ml4s/backend/torch/
--rw-rw-rw-   0        0        0      224 2023-06-12 21:40:30.000000 ml4s-0.0.2/ml4s/backend/torch/__init__.py
--rw-rw-rw-   0        0        0    60051 2023-07-14 14:43:38.000000 ml4s-0.0.2/ml4s/backend/torch/_torch_backend.py
--rw-rw-rw-   0        0        0    29784 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/backend/torch/nets.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:38.157746 ml4s-0.0.2/ml4s/math/
--rw-rw-rw-   0        0        0     4809 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/__init__.py
--rw-rw-rw-   0        0        0     3777 2023-06-11 18:52:32.000000 ml4s-0.0.2/ml4s/math/_fit.py
--rw-rw-rw-   0        0        0    56926 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_functional.py
--rw-rw-rw-   0        0        0    37500 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_magic_ops.py
--rw-rw-rw-   0        0        0    32286 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_nd.py
--rw-rw-rw-   0        0        0   126238 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_ops.py
--rw-rw-rw-   0        0        0    45700 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_optimize.py
--rw-rw-rw-   0        0        0    76206 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_shape.py
--rw-rw-rw-   0        0        0    55027 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_sparse.py
--rw-rw-rw-   0        0        0   106638 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/_tensors.py
--rw-rw-rw-   0        0        0    18568 2023-06-16 08:55:17.000000 ml4s-0.0.2/ml4s/math/_trace.py
--rw-rw-rw-   0        0        0    60714 2023-07-14 14:43:37.000000 ml4s-0.0.2/ml4s/math/extrapolation.py
--rw-rw-rw-   0        0        0    32845 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/math/magic.py
--rw-rw-rw-   0        0        0    12669 2023-07-14 14:43:53.000000 ml4s-0.0.2/ml4s/nn.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:55:37.947796 ml4s-0.0.2/ml4s.egg-info/
--rw-rw-rw-   0        0        0     4556 2023-07-14 15:55:37.000000 ml4s-0.0.2/ml4s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1237 2023-07-14 15:55:37.000000 ml4s-0.0.2/ml4s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:55:37.000000 ml4s-0.0.2/ml4s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-14 15:55:37.000000 ml4s-0.0.2/ml4s.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-14 15:55:37.000000 ml4s-0.0.2/ml4s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-14 15:55:38.162750 ml4s-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     6898 2023-07-14 14:43:53.000000 ml4s-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.523181 ml4s-0.1.0/
+-rw-rw-rw-   0        0        0      105 2023-07-15 10:52:41.000000 ml4s-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4556 2023-07-15 22:05:16.523181 ml4s-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12063 2023-07-15 10:52:41.000000 ml4s-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.146848 ml4s-0.1.0/ml4s/
+-rw-rw-rw-   0        0        0        5 2023-07-15 10:55:51.000000 ml4s-0.1.0/ml4s/VERSION
+-rw-rw-rw-   0        0        0     1090 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/__init__.py
+-rw-rw-rw-   0        0        0     8432 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/_troubleshoot.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.278351 ml4s-0.1.0/ml4s/backend/
+-rw-rw-rw-   0        0        0     1140 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/__init__.py
+-rw-rw-rw-   0        0        0    71763 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_backend.py
+-rw-rw-rw-   0        0        0     6142 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_dtype.py
+-rw-rw-rw-   0        0        0    38859 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_linalg.py
+-rw-rw-rw-   0        0        0     3101 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_linalg_preconditioner.py
+-rw-rw-rw-   0        0        0     9048 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_minimize.py
+-rw-rw-rw-   0        0        0    20027 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_numpy_backend.py
+-rw-rw-rw-   0        0        0     1345 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_object.py
+-rw-rw-rw-   0        0        0    19229 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_partition.py
+-rw-rw-rw-   0        0        0    22492 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_profile.py
+-rw-rw-rw-   0        0        0      449 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/_triangular_wip.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.299206 ml4s-0.1.0/ml4s/backend/jax/
+-rw-rw-rw-   0        0        0      163 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/jax/__init__.py
+-rw-rw-rw-   0        0        0    25135 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/jax/_jax_backend.py
+-rw-rw-rw-   0        0        0    39603 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/jax/stax_nets.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.354310 ml4s-0.1.0/ml4s/backend/tensorflow/
+-rw-rw-rw-   0        0        0      906 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0     4228 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/tensorflow/_compile_cuda.py
+-rw-rw-rw-   0        0        0     1950 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/tensorflow/_profiling.py
+-rw-rw-rw-   0        0        0    34022 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/tensorflow/_tf_backend.py
+-rw-rw-rw-   0        0        0     3280 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/tensorflow/_tf_cuda_resample.py
+-rw-rw-rw-   0        0        0    24962 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/tensorflow/nets.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.378781 ml4s-0.1.0/ml4s/backend/torch/
+-rw-rw-rw-   0        0        0      224 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/torch/__init__.py
+-rw-rw-rw-   0        0        0    60051 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/torch/_torch_backend.py
+-rw-rw-rw-   0        0        0    29784 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/backend/torch/nets.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.521179 ml4s-0.1.0/ml4s/math/
+-rw-rw-rw-   0        0        0     4809 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/__init__.py
+-rw-rw-rw-   0        0        0     3777 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/_fit.py
+-rw-rw-rw-   0        0        0    57021 2023-07-15 11:46:26.000000 ml4s-0.1.0/ml4s/math/_functional.py
+-rw-rw-rw-   0        0        0    37718 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/_magic_ops.py
+-rw-rw-rw-   0        0        0    32297 2023-07-15 21:02:23.000000 ml4s-0.1.0/ml4s/math/_nd.py
+-rw-rw-rw-   0        0        0   126541 2023-07-15 21:02:23.000000 ml4s-0.1.0/ml4s/math/_ops.py
+-rw-rw-rw-   0        0        0    45700 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/_optimize.py
+-rw-rw-rw-   0        0        0    76206 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/_shape.py
+-rw-rw-rw-   0        0        0    55027 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/_sparse.py
+-rw-rw-rw-   0        0        0   107930 2023-07-15 21:02:23.000000 ml4s-0.1.0/ml4s/math/_tensors.py
+-rw-rw-rw-   0        0        0    17724 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/_trace.py
+-rw-rw-rw-   0        0        0    60714 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/extrapolation.py
+-rw-rw-rw-   0        0        0    32845 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/math/magic.py
+-rw-rw-rw-   0        0        0    12669 2023-07-15 10:52:42.000000 ml4s-0.1.0/ml4s/nn.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:05:16.177670 ml4s-0.1.0/ml4s.egg-info/
+-rw-rw-rw-   0        0        0     4556 2023-07-15 22:05:15.000000 ml4s-0.1.0/ml4s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1237 2023-07-15 22:05:15.000000 ml4s-0.1.0/ml4s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 22:05:15.000000 ml4s-0.1.0/ml4s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-15 22:05:15.000000 ml4s-0.1.0/ml4s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-15 22:05:15.000000 ml4s-0.1.0/ml4s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 22:05:16.525733 ml4s-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     6898 2023-07-15 10:52:42.000000 ml4s-0.1.0/setup.py
```

### Comparing `ml4s-0.0.2/PKG-INFO` & `ml4s-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml4s
-Version: 0.0.2
+Version: 0.1.0
 Summary: Unified API for machine learning
 Home-page: https://github.com/holl-/ML4Science
 Author: Philipp Holl
 Author-email: philipp.holl@tum.de
 License: MIT
-Download-URL: https://github.com/holl-/ML4Science/archive/0.0.2.tar.gz
+Download-URL: https://github.com/holl-/ML4Science/archive/0.1.0.tar.gz
 Description: # ML4Science
         
         [🌐 **Homepage**](https://github.com/holl-/ML4Science)
         &nbsp;&nbsp;&nbsp; [📖 **Documentation**](https://holl-.github.io/ML4Science/)
         &nbsp;&nbsp;&nbsp; [🔗 **API**](https://holl-.github.io/ML4Science/ml4s)
         &nbsp; • &nbsp; [**▶ Videos**]()
         &nbsp; • &nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16>](https://colab.research.google.com/github/holl-/ML4Science/blob/main/docs/Examples.ipynb) [**Examples**](https://holl-.github.io/ML4Science/Examples.html)
```

### Comparing `ml4s-0.0.2/README.md` & `ml4s-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/__init__.py` & `ml4s-0.1.0/ml4s/__init__.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/_troubleshoot.py` & `ml4s-0.1.0/ml4s/_troubleshoot.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/__init__.py` & `ml4s-0.1.0/ml4s/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_backend.py` & `ml4s-0.1.0/ml4s/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_dtype.py` & `ml4s-0.1.0/ml4s/backend/_dtype.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_linalg.py` & `ml4s-0.1.0/ml4s/backend/_linalg.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_linalg_preconditioner.py` & `ml4s-0.1.0/ml4s/backend/_linalg_preconditioner.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_minimize.py` & `ml4s-0.1.0/ml4s/backend/_minimize.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_numpy_backend.py` & `ml4s-0.1.0/ml4s/backend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_object.py` & `ml4s-0.1.0/ml4s/backend/_object.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_partition.py` & `ml4s-0.1.0/ml4s/backend/_partition.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/_profile.py` & `ml4s-0.1.0/ml4s/backend/_profile.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/jax/_jax_backend.py` & `ml4s-0.1.0/ml4s/backend/jax/_jax_backend.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/jax/stax_nets.py` & `ml4s-0.1.0/ml4s/backend/jax/stax_nets.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/tensorflow/__init__.py` & `ml4s-0.1.0/ml4s/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/tensorflow/_compile_cuda.py` & `ml4s-0.1.0/ml4s/backend/tensorflow/_compile_cuda.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/tensorflow/_profiling.py` & `ml4s-0.1.0/ml4s/backend/tensorflow/_profiling.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/tensorflow/_tf_backend.py` & `ml4s-0.1.0/ml4s/backend/tensorflow/_tf_backend.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/tensorflow/_tf_cuda_resample.py` & `ml4s-0.1.0/ml4s/backend/tensorflow/_tf_cuda_resample.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/tensorflow/nets.py` & `ml4s-0.1.0/ml4s/backend/tensorflow/nets.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/torch/_torch_backend.py` & `ml4s-0.1.0/ml4s/backend/torch/_torch_backend.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/backend/torch/nets.py` & `ml4s-0.1.0/ml4s/backend/torch/nets.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/math/__init__.py` & `ml4s-0.1.0/ml4s/math/__init__.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/math/_fit.py` & `ml4s-0.1.0/ml4s/math/_fit.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/math/_functional.py` & `ml4s-0.1.0/ml4s/math/_functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 
 from . import _ops as math
 from ._magic_ops import stack
 from ._shape import EMPTY_SHAPE, Shape, spatial, instance, batch, channel
 from ._sparse import SparseCoordinateTensor
-from ._tensors import Tensor, disassemble_tree, assemble_tree, disassemble_tensors, assemble_tensors, variable_attributes, wrap, specs_equal
+from ._tensors import Tensor, disassemble_tree, assemble_tree, disassemble_tensors, assemble_tensors, variable_attributes, wrap, specs_equal, equality_by_value
 from ._trace import ShiftLinTracer, matrix_from_function, LinearTraceInProgress
 from ..backend import Backend, NUMPY
 from ..backend._backend import get_spatial_derivative_order, functional_derivative_evaluation, ML_LOGGER
 from .magic import PhiTreeNode
 
 X = TypeVar('X')
 Y = TypeVar('Y')
@@ -42,27 +42,29 @@
         self.spatial_derivative_order = get_spatial_derivative_order()
 
     def __repr__(self):
         return f"{self.tree} with shapes {self.shapes}"
 
     def __eq__(self, other: 'SignatureKey'):
         assert isinstance(other, SignatureKey)
-        cond_equal = self.auxiliary_kwargs == other.auxiliary_kwargs
+        with equality_by_value():
+            cond_equal = self.auxiliary_kwargs == other.auxiliary_kwargs
         if isinstance(cond_equal, Tensor):
             cond_equal = cond_equal.all
         # shapes need not be compared because they are included in specs
         specs = specs_equal(self.specs, other.specs)
         return self.tree == other.tree and specs and self.backend == other.backend and self.spatial_derivative_order == other.spatial_derivative_order and cond_equal
 
     def __hash__(self):
         return hash(self.shapes) + hash(self.backend)
 
     def matches_structure_and_names(self, other: 'SignatureKey'):
         assert isinstance(other, SignatureKey)
-        cond_equal = self.auxiliary_kwargs == other.auxiliary_kwargs
+        with equality_by_value():
+            cond_equal = self.auxiliary_kwargs == other.auxiliary_kwargs
         if isinstance(cond_equal, Tensor):
             cond_equal = cond_equal.all
         return self.tree == other.tree and all(s1.names == s2.names for s1, s2 in zip(self.shapes, other.shapes)) and self.backend == other.backend and cond_equal
 
     def extrapolate(self, rec_in: 'SignatureKey', new_in: 'SignatureKey') -> 'SignatureKey':
         assert self.source_function is not None, "extrapolate() must be called on output keys"
         shapes = [self._extrapolate_shape(s, rec_in, new_in) for s in self.shapes]
```

### Comparing `ml4s-0.0.2/ml4s/math/_magic_ops.py` & `ml4s-0.1.0/ml4s/math/_magic_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,17 @@
         (x=0.000, y=1.000); (x=0.000, y=1.000) (bᵇ=2, cᶜ=x,y)
 
         >>> stack([vec(x=1, y=0), vec(x=2, y=3.)], batch('b'))
         (x=1.000, y=0.000); (x=2.000, y=3.000) (bᵇ=2, vectorᶜ=x,y)
     """
     assert len(values) > 0, f"stack() got empty sequence {values}"
     assert isinstance(dim, Shape)
+    if not dim:
+        assert len(values) == 1, f"Only one element can be passed as `values` if no dim is passed but got {values}"
+        return next(iter(values.values())) if isinstance(values, dict) else values[0]
     values_ = tuple(values.values()) if isinstance(values, dict) else values
     if not expand_values:
         for v in values_[1:]:
             assert set(non_batch(v).names) == set(non_batch(values_[0]).names), f"Stacked values must have the same non-batch dimensions but got {non_batch(values_[0])} and {non_batch(v)}"
     # --- Add missing dimensions ---
     if expand_values:
         all_dims = merge_shapes(*values_, allow_varying_sizes=True)
```

### Comparing `ml4s-0.0.2/ml4s/math/_nd.py` & `ml4s-0.1.0/ml4s/math/_nd.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,22 +385,22 @@
     pad_upper = max(0, max(offsets))
     if padding is not None:
         x = math.pad(x, {axis: (pad_lower + extend_bounds, pad_upper + extend_bounds) for axis in dims}, mode=padding)
     if extend_bounds:
         assert padding is not None
     offset_tensors = []
     for offset in offsets:
-        components = []
+        components = {}
         for dimension in dims:
             if padding:
                 slices = {dim: slice(pad_lower + offset, (-pad_upper + offset) or None) if dim == dimension else slice(pad_lower, -pad_upper or None) for dim in dims}
             else:
                 slices = {dim: slice(pad_lower + offset, (-pad_upper + offset) or None) if dim == dimension else slice(None, None) for dim in dims}
-            components.append(x[slices])
-        offset_tensors.append(stack(components, stack_dim) if stack_dim is not None else components[0])
+            components[dimension] = x[slices]
+        offset_tensors.append(stack(components, stack_dim) if stack_dim is not None else next(iter(components.values())))
     return offset_tensors
 
 
 def masked_fill(values: Tensor, valid: Tensor, distance: int = 1) -> Tuple[Tensor, Tensor]:
     """
     Extrapolates the values of `values` which are marked by the nonzero values of `valid` for `distance` steps in all spatial directions.
     Overlapping extrapolated values get averaged. Extrapolation also includes diagonals.
@@ -495,15 +495,15 @@
         pad: How many cells to extend the result compared to `grid`.
             This value is added to the internal padding. For non-trivial extrapolations, this gives the correct result while manual padding before or after this operation would not respect the boundary locations.
 
     Returns:
         `Tensor`
     """
     grid = wrap(grid)
-    if stack_dim is not None and stack_dim in grid.shape:
+    if stack_dim and stack_dim in grid.shape:
         assert grid.shape.only(stack_dim).size == 1, f"spatial_gradient() cannot list components along {stack_dim.name} because that dimension already exists on grid {grid}"
         grid = grid[{stack_dim.name: 0}]
     dims = grid.shape.only(dims)
     dx = wrap(dx)
     if dx.vector.exists:
         dx = dx.vector[dims]
         if dx.vector.size in (None, 1):
```

### Comparing `ml4s-0.0.2/ml4s/math/_ops.py` & `ml4s-0.1.0/ml4s/math/_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,15 @@
         shapes = shape.unstack(stack_dim.name)
         tensors = [_initialize(uniform_initializer, s) for s in shapes]
         return stack_tensors(tensors, stack_dim)
     else:
         return uniform_initializer(shape)
 
 
-def zeros(*shape: Shape, dtype=None) -> Tensor:
+def zeros(*shape: Shape, dtype: Union[DType, tuple, type] = None) -> Tensor:
     """
     Define a tensor with specified shape with value `0.0` / `0` / `False` everywhere.
     
     This method may not immediately allocate the memory to store the values.
 
     See Also:
         `zeros_like()`, `ones()`.
@@ -490,15 +490,15 @@
     for val in values:
         val = wrap(val)
         with val.default_backend:
             zeros_.append(zeros(val.shape, dtype=val.dtype))
     return assemble_tree(nest, zeros_)
 
 
-def ones(*shape: Shape, dtype=None) -> Tensor:
+def ones(*shape: Shape, dtype: Union[DType, tuple, type] = None) -> Tensor:
     """
     Define a tensor with specified shape with value `1.0`/ `1` / `True` everywhere.
     
     This method may not immediately allocate the memory to store the values.
 
     See Also:
         `ones_like()`, `zeros()`.
@@ -514,15 +514,15 @@
 
 
 def ones_like(value: Tensor) -> Tensor:
     """ Create a `Tensor` containing only `1.0` / `1` / `True` with the same shape and dtype as `obj`. """
     return zeros_like(value) + 1
 
 
-def random_normal(*shape: Shape, dtype=None) -> Tensor:
+def random_normal(*shape: Shape, dtype: Union[DType, tuple, type] = None) -> Tensor:
     """
     Creates a `Tensor` with the specified shape, filled with random values sampled from a normal / Gaussian distribution.
 
     Implementations:
 
     * NumPy: [`numpy.random.standard_normal`](https://numpy.org/doc/stable/reference/random/generated/numpy.random.standard_normal.html)
     * PyTorch: [`torch.randn`](https://pytorch.org/docs/stable/generated/torch.randn.html)
@@ -543,15 +543,15 @@
 
     return _initialize(uniform_random_normal, shape)
 
 
 def random_uniform(*shape: Shape,
                    low: Union[Tensor, float] = 0,
                    high: Union[Tensor, float] = 1,
-                   dtype: Union[DType, tuple] = None) -> Tensor:
+                   dtype: Union[DType, tuple, type] = None) -> Tensor:
     """
     Creates a `Tensor` with the specified shape, filled with random values sampled from a uniform distribution.
 
     Args:
         *shape: This (possibly empty) sequence of `Shape`s is concatenated, preserving the order.
         dtype: (optional) `DType` or `(kind, bits)`.
             The dtype kind must be one of `float`, `int`, `complex`.
@@ -694,17 +694,19 @@
         assert len(channels) == 1, f"meshgrid with multiple dimension requires a valid stack_dim but got {stack_dim}"
         return channels[0]
     if stack_dim.item_names[0] is None:
         stack_dim = stack_dim.with_size(tuple(dimensions.keys()))
     return stack_tensors(channels, stack_dim)
 
 
-def linspace(start: Union[float, Tensor], stop: Union[float, Tensor], dim: Shape) -> Tensor:
+def linspace(start: Union[float, Tensor, tuple, list], stop: Union[float, Tensor, tuple, list], dim: Shape) -> Tensor:
     """
-    Returns `number` evenly spaced numbers between `start` and `stop`.
+    Returns `number` evenly spaced numbers between `start` and `stop` along `dim`.
+
+    If `dim` contains multiple dimensions, evenly spaces values along each dimension, then stacks the result along a new channel dimension called `vector`.
 
     See Also:
         `arange()`, `meshgrid()`.
 
     Args:
         start: First value, `int` or `Tensor`.
         stop: Last value, `int` or `Tensor`.
@@ -718,20 +720,22 @@
     Examples:
         >>> math.linspace(0, 1, spatial(x=5))
         (0.000, 0.250, 0.500, 0.750, 1.000) along xˢ
 
         >>> math.linspace(0, (-1, 1), spatial(x=3))
         (0.000, 0.000); (-0.500, 0.500); (-1.000, 1.000) (xˢ=3, vectorᶜ=2)
     """
-    assert isinstance(dim, Shape) and dim.rank == 1, f"dim must be a single-dimension Shape but got {dim}"
+    assert isinstance(dim, Shape), f"dim must be a Shape but got {dim}"
+    start = wrap(start)
+    stop = wrap(stop)
+    if dim.rank > 1:
+        return meshgrid(dim) / (dim - 1) * (stop - start) + start
     if is_scalar(start) and is_scalar(stop):
-        if isinstance(start, Tensor):
-            start = start.native()
-        if isinstance(stop, Tensor):
-            stop = stop.native()
+        start = start.native()
+        stop = stop.native()
         native_linspace = choose_backend(start, stop, prefer_default=True).linspace(start, stop, dim.size)
         return NativeTensor(native_linspace, dim)
     else:
         return map_(linspace, start, stop, dim=dim)
 
 
 def arange(dim: Shape, start_or_stop: Union[int, None] = None, stop: Union[int, None] = None, step=1):
```

### Comparing `ml4s-0.0.2/ml4s/math/_optimize.py` & `ml4s-0.1.0/ml4s/math/_optimize.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/math/_shape.py` & `ml4s-0.1.0/ml4s/math/_shape.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/math/_sparse.py` & `ml4s-0.1.0/ml4s/math/_sparse.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/math/_tensors.py` & `ml4s-0.1.0/ml4s/math/_tensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,23 +126,29 @@
                 return self._op2(inputs[0], lambda x, y: y % x, lambda x, y: choose_backend(x, y).mod(y, x), 'r_remainder', '%')
         if ufunc.__name__ == 'power':
             if inputs[0] is self:
                 return self._op2(inputs[1], lambda x, y: x ** y, lambda x, y: choose_backend(x, y).pow(x, y), 'power', '**')
             else:
                 return self._op2(inputs[0], lambda x, y: y ** x, lambda x, y: choose_backend(x, y).pow(y, x), 'r_power', '**')
         if ufunc.__name__ == 'equal':
-            if _EQUALITY_BY_REF:
+            if _EQUALITY_REDUCE[-1] == 'ref':
                 return wrap(inputs[0] is inputs[1])
+            elif _EQUALITY_REDUCE[-1] == 'value':
+                from ._ops import close
+                return wrap(close(inputs[0], inputs[1], rel_tolerance=0, abs_tolerance=0))
             if inputs[0] is self:
                 return self._op2(inputs[1], lambda x, y: x == y, lambda x, y: choose_backend(x, y).equal(x, y), 'equal', '==')
             else:
                 return self._op2(inputs[0], lambda x, y: y == x, lambda x, y: choose_backend(x, y).equal(y, x), 'r_equal', '==')
         if ufunc.__name__ == 'not_equal':
-            if _EQUALITY_BY_REF:
+            if _EQUALITY_REDUCE[-1] == 'ref':
                 return wrap(inputs[0] is not inputs[1])
+            elif _EQUALITY_REDUCE[-1] == 'value':
+                from ._ops import close
+                return wrap(not close(inputs[0], inputs[1], rel_tolerance=0, abs_tolerance=0))
             if inputs[0] is self:
                 return self._op2(inputs[1], lambda x, y: x != y, lambda x, y: choose_backend(x, y).not_equal(x, y), 'equal', '!=')
             else:
                 return self._op2(inputs[0], lambda x, y: y != x, lambda x, y: choose_backend(x, y).not_equal(y, x), 'r_equal', '!=')
         if ufunc.__name__ == 'greater':
             if inputs[0] is self:
                 return self._op2(inputs[1], lambda x, y: x > y, lambda x, y: choose_backend(x, y).greater_than(x, y), 'greater', '>')
@@ -631,23 +637,29 @@
     def __mod__(self, other):
         return self._op2(other, lambda x, y: x % y, lambda x, y: choose_backend(x, y).mod(x, y), 'mod', '%')
 
     def __rmod__(self, other):
         return self._op2(other, lambda x, y: y % x, lambda x, y: choose_backend(x, y).mod(y, x), 'rmod', '%')
 
     def __eq__(self, other):
-        if _EQUALITY_BY_REF:
+        if _EQUALITY_REDUCE[-1] == 'ref':
             return wrap(self is other)
+        elif _EQUALITY_REDUCE[-1] == 'value':
+            from ._ops import close
+            return wrap(close(self, other, rel_tolerance=0, abs_tolerance=0))
         if other is None:
             other = float('nan')
         return self._op2(other, lambda x, y: x == y, lambda x, y: choose_backend(x, y).equal(x, y), 'eq', '==')
 
     def __ne__(self, other):
-        if _EQUALITY_BY_REF:
+        if _EQUALITY_REDUCE[-1] == 'ref':
             return wrap(self is not other)
+        elif _EQUALITY_REDUCE[-1] == 'value':
+            from ._ops import close
+            return wrap(not close(self, other, rel_tolerance=0, abs_tolerance=0))
         if other is None:
             other = float('nan')
         return self._op2(other, lambda x, y: x != y, lambda x, y: choose_backend(x, y).not_equal(x, y), 'ne', '!=')
 
     def __lt__(self, other):
         return self._op2(other, lambda x, y: x < y, lambda x, y: choose_backend(x, y).greater_than(y, x), 'lt', '<')
 
@@ -868,27 +880,39 @@
         return sum_(self.tensor, self.name)
 
     def prod(self):
         from ._ops import prod
         return prod(self.tensor, self.name)
 
 
-_EQUALITY_BY_REF = []
+_EQUALITY_REDUCE = [None]
 
 
 @contextmanager
 def equality_by_ref():
     """
     Enables Tensor.__bool__
     """
-    _EQUALITY_BY_REF.append(True)
+    _EQUALITY_REDUCE.append('ref')
     try:
         yield None
     finally:
-        _EQUALITY_BY_REF.pop(-1)
+        assert _EQUALITY_REDUCE.pop(-1) == 'ref'
+
+
+@contextmanager
+def equality_by_value():
+    """
+    Enables Tensor.__bool__
+    """
+    _EQUALITY_REDUCE.append('value')
+    try:
+        yield None
+    finally:
+        assert _EQUALITY_REDUCE.pop(-1) == 'value'
 
 
 class Layout(Tensor):
     """
     Tensor representation of a PyTree consisting of only lists, tuples and leaves.
     Leaves can be any Python object or primitive, including tuples and lists.
     The PyTree may be deeper but only the outer `shape.rank` levels are represented as a tensor.
@@ -1040,21 +1064,21 @@
             return iter(self._obj)
         elif self.rank == 0:
             return iter([self._obj])
         else:
             return iter(self._as_list())
 
     def __eq__(self, other):
-        if _EQUALITY_BY_REF:
-            return wrap(self is other)
+        if _EQUALITY_REDUCE[-1]:
+            return Tensor.__eq__(self, other)
         return self._op2(other, lambda x, y: x == y, lambda x, y: x == y, 'eq', '==')
 
     def __ne__(self, other):
-        if _EQUALITY_BY_REF:
-            return wrap(self is not other)
+        if _EQUALITY_REDUCE[-1]:
+            return Tensor.__ne__(self, other)
         return self._op2(other, lambda x, y: x != y, lambda x, y: x != y, 'ne', '!=')
     
     def _assert_close(self, other: Tensor, rel_tolerance: float, abs_tolerance: float, msg: str, verbose: bool):
         from ._ops import assert_close
         inner_test = lambda x, y: assert_close(x, y, rel_tolerance=rel_tolerance, abs_tolerance=abs_tolerance, msg=msg, verbose=verbose)
         return self._op2(other, inner_test, inner_test, 'assert_close', '≈')
 
@@ -1541,18 +1565,23 @@
         else:
             if None in shape.sizes:
                 shape = shape.with_sizes(data.shape.sizes)
             return data._with_shape_replaced(shape)
     elif isinstance(data, Shape):
         if shape is None:
             shape = channel('dims')
+            shape = shape.with_size(data.names)
+            data = data.sizes
+        elif not shape:
+            assert data.rank == 1, f"When wrapping a Shape as a scalar tensor, it must be a rank-1 shape but got {data}"
+            data = data.size
         else:
             assert shape.rank == 1, "Can only convert 1D shapes to Tensors"
-        shape = shape.with_size(data.names)
-        data = data.sizes
+            shape = shape.with_size(data.names)
+            data = data.sizes
     elif isinstance(data, str) or data is None:
         return layout(data)
     elif isinstance(data, (numbers.Number, bool)):
         assert not shape, f"Trying to create a zero-dimensional Tensor from value '{data}' but shape={shape}"
         if convert:
             data = default_backend().as_tensor(data, convert_external=True)
         return NativeTensor(data, EMPTY_SHAPE)
@@ -1690,15 +1719,16 @@
             data = backend.as_tensor(data)
         if len(shape) == compat_shape.channel_rank:
             other_tensor = wrap(data, compat_shape.channel)
             return other_tensor
         if compat_shape.channel_rank > 1 and len(shape) == 1 and 'vector' in compat_shape.channel:
             return wrap(data, compat_shape['vector'].without_sizes())
         elif len(shape) == compat_shape.rank:
-            warnings.warn(f"Combining a ml4s.math.Tensor with a {data_type} of same shape is not invariant under shape permutations. Please convert the {data_type} to a ml4s.math.Tensor first. Shapes: {shape} and {compat_shape}", SyntaxWarning, stacklevel=5)
+            if len(shape) > 1:
+                warnings.warn(f"Combining a ml4s.math.Tensor with a {data_type} of same shape is not invariant under shape permutations. Please convert the {data_type} to a ml4s.math.Tensor first. Shapes: {shape} and {compat_shape}", SyntaxWarning, stacklevel=5)
             return NativeTensor(data, compat_shape.with_sizes(shape))
         else:
             raise ValueError(f"Cannot combine tensor of shape {shape} with tensor of shape {compat_shape}")
 
 
 def broadcastable_native_tensors(*tensors):
     """
```

### Comparing `ml4s-0.0.2/ml4s/math/_trace.py` & `ml4s-0.1.0/ml4s/math/_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,33 +43,14 @@
             assert shift_.only(sorted(shift_.names), reorder=True) == shift_
         self.bias = bias
         self._shape = shape
 
     def __repr__(self):
         return f"Linear tracer {self._shape}"
 
-    def native(self, order: Union[str, tuple, list, Shape] = None):
-        """
-        Evaluates the value of the linear operation applied to the original source tensor.
-
-        This is done by building a sparse matrix for all dimensions that are affected by the linear operation.
-        These dimensions are detected automatically during the creation of the linear operation.
-        All other dimensions (independent dimensions) are combined into a single batch dimensions for the sparse matrix multiplication.
-
-        Args:
-          order: str or tuple or list:  (Default value = None)
-
-        Returns:
-
-        """
-        order = parse_dim_order(order, check_rank=self.rank)
-        result = self.apply(self.source)
-        result_order = order if order is not None else self._shape.names
-        return result.native(result_order)
-
     @property
     def dependent_dims(self) -> Set[str]:
         """
         Dimensions relevant to the linear operation.
         This includes `pattern_dims` as well as dimensions along which only the values vary.
         These dimensions cannot be parallelized trivially with a non-batched matrix.
         """
```

### Comparing `ml4s-0.0.2/ml4s/math/extrapolation.py` & `ml4s-0.1.0/ml4s/math/extrapolation.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/math/magic.py` & `ml4s-0.1.0/ml4s/math/magic.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s/nn.py` & `ml4s-0.1.0/ml4s/nn.py`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/ml4s.egg-info/PKG-INFO` & `ml4s-0.1.0/ml4s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml4s
-Version: 0.0.2
+Version: 0.1.0
 Summary: Unified API for machine learning
 Home-page: https://github.com/holl-/ML4Science
 Author: Philipp Holl
 Author-email: philipp.holl@tum.de
 License: MIT
-Download-URL: https://github.com/holl-/ML4Science/archive/0.0.2.tar.gz
+Download-URL: https://github.com/holl-/ML4Science/archive/0.1.0.tar.gz
 Description: # ML4Science
         
         [🌐 **Homepage**](https://github.com/holl-/ML4Science)
         &nbsp;&nbsp;&nbsp; [📖 **Documentation**](https://holl-.github.io/ML4Science/)
         &nbsp;&nbsp;&nbsp; [🔗 **API**](https://holl-.github.io/ML4Science/ml4s)
         &nbsp; • &nbsp; [**▶ Videos**]()
         &nbsp; • &nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16>](https://colab.research.google.com/github/holl-/ML4Science/blob/main/docs/Examples.ipynb) [**Examples**](https://holl-.github.io/ML4Science/Examples.html)
```

### Comparing `ml4s-0.0.2/ml4s.egg-info/SOURCES.txt` & `ml4s-0.1.0/ml4s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml4s-0.0.2/setup.py` & `ml4s-0.1.0/setup.py`

 * *Files identical despite different names*

