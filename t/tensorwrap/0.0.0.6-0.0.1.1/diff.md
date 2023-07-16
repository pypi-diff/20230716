# Comparing `tmp/tensorwrap-0.0.0.6.tar.gz` & `tmp/tensorwrap-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorwrap-0.0.0.6.tar", last modified: Wed Apr  5 01:43:23 2023, max compression
+gzip compressed data, was "tensorwrap-0.0.1.1.tar", last modified: Sun Jul 16 15:21:06 2023, max compression
```

## Comparing `tensorwrap-0.0.0.6.tar` & `tensorwrap-0.0.1.1.tar`

### file list

```diff
@@ -1,38 +1,56 @@
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:43:23.085567 tensorwrap-0.0.0.6/
--rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-01-28 23:45:44.000000 tensorwrap-0.0.0.6/LICENSE
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6338 2023-04-05 01:43:23.085567 tensorwrap-0.0.0.6/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)     5769 2023-04-02 16:55:44.000000 tensorwrap-0.0.0.6/README.md
--rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-04-05 01:43:23.085567 tensorwrap-0.0.0.6/setup.cfg
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1878 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/setup.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:43:23.083567 tensorwrap-0.0.0.6/tensorwrap/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1547 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/__init__.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:43:23.084567 tensorwrap-0.0.0.6/tensorwrap/autograph/
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:18:38.000000 tensorwrap-0.0.0.6/tensorwrap/autograph/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)       61 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/autograph/core.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/tensorwrap/config.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-04-02 16:55:44.000000 tensorwrap-0.0.0.6/tensorwrap/data.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:43:23.084567 tensorwrap-0.0.0.6/tensorwrap/experimental/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      133 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/tensorwrap/experimental/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-04-05 01:18:38.000000 tensorwrap-0.0.0.6/tensorwrap/experimental/serialize.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/tensorwrap/experimental/wrappers.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1984 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/module.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:43:23.085567 tensorwrap-0.0.0.6/tensorwrap/nn/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      498 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/tensorwrap/nn/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1291 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/nn/activations.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/tensorwrap/nn/callbacks.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/nn/checkpoints.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/tensorwrap/nn/initializers.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     8956 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/nn/layers.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      234 2023-03-28 12:47:08.000000 tensorwrap-0.0.0.6/tensorwrap/nn/losses.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     4317 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/nn/models.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      976 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/nn/optimizers.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1472 2023-04-05 01:18:44.000000 tensorwrap-0.0.0.6/tensorwrap/ops.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-03-06 22:52:48.000000 tensorwrap-0.0.0.6/tensorwrap/test.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)       58 2023-04-05 01:18:38.000000 tensorwrap-0.0.0.6/tensorwrap/version.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-04-05 01:43:23.084567 tensorwrap-0.0.0.6/tensorwrap.egg-info/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6338 2023-04-05 01:43:23.000000 tensorwrap-0.0.0.6/tensorwrap.egg-info/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)      783 2023-04-05 01:43:23.000000 tensorwrap-0.0.0.6/tensorwrap.egg-info/SOURCES.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-04-05 01:43:23.000000 tensorwrap-0.0.0.6/tensorwrap.egg-info/dependency_links.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-04-05 01:43:23.000000 tensorwrap-0.0.0.6/tensorwrap.egg-info/not-zip-safe
--rw-r--r--   0 impureking  (1000) impureking  (1000)      309 2023-04-05 01:43:23.000000 tensorwrap-0.0.0.6/tensorwrap.egg-info/requires.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-04-05 01:43:23.000000 tensorwrap-0.0.0.6/tensorwrap.egg-info/top_level.txt
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/LICENSE
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6444 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     5875 2023-05-27 02:36:24.000000 tensorwrap-0.0.1.1/README.md
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/setup.cfg
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1891 2023-07-15 21:24:36.000000 tensorwrap-0.0.1.1/setup.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.727131 tensorwrap-0.0.1.1/tensorwrap/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1549 2023-07-15 20:22:23.000000 tensorwrap-0.0.1.1/tensorwrap/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/config.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.728131 tensorwrap-0.0.1.1/tensorwrap/core/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       20 2023-06-16 00:46:59.000000 tensorwrap-0.0.1.1/tensorwrap/core/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.728131 tensorwrap-0.0.1.1/tensorwrap/core/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      107 2023-06-16 00:41:45.000000 tensorwrap-0.0.1.1/tensorwrap/core/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      419 2023-06-16 01:15:18.000000 tensorwrap-0.0.1.1/tensorwrap/core/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      274 2023-06-15 22:56:13.000000 tensorwrap-0.0.1.1/tensorwrap/core/losses/mean.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/data.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/experimental/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      133 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/experimental/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/experimental/serialize.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/experimental/wrappers.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     2924 2023-07-16 14:25:46.000000 tensorwrap-0.0.1.1/tensorwrap/module.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      508 2023-07-15 20:45:34.000000 tensorwrap-0.0.1.1/tensorwrap/nn/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/activations/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       55 2023-07-16 14:48:55.000000 tensorwrap-0.0.1.1/tensorwrap/nn/activations/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1402 2023-07-16 14:54:01.000000 tensorwrap-0.0.1.1/tensorwrap/nn/activations/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/nn/callbacks.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.1/tensorwrap/nn/checkpoints.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/initializers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      604 2023-07-15 21:02:53.000000 tensorwrap-0.0.1.1/tensorwrap/nn/initializers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      124 2023-07-15 20:56:21.000000 tensorwrap-0.0.1.1/tensorwrap/nn/initializers/base.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.729131 tensorwrap-0.0.1.1/tensorwrap/nn/layers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       51 2023-06-09 20:26:57.000000 tensorwrap-0.0.1.1/tensorwrap/nn/layers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     4484 2023-07-16 14:50:37.000000 tensorwrap-0.0.1.1/tensorwrap/nn/layers/base.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/tensorwrap/nn/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      126 2023-06-16 01:05:54.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      371 2023-06-16 00:28:46.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      451 2023-06-16 00:41:32.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      697 2023-06-15 23:22:21.000000 tensorwrap-0.0.1.1/tensorwrap/nn/losses/mean.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/tensorwrap/nn/models/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      102 2023-06-10 15:50:36.000000 tensorwrap-0.0.1.1/tensorwrap/nn/models/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     7455 2023-07-16 15:15:14.000000 tensorwrap-0.0.1.1/tensorwrap/nn/models/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       71 2023-07-16 13:21:05.000000 tensorwrap-0.0.1.1/tensorwrap/nn/models/train.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.730131 tensorwrap-0.0.1.1/tensorwrap/nn/optimizers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       66 2023-06-09 19:51:14.000000 tensorwrap-0.0.1.1/tensorwrap/nn/optimizers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      775 2023-06-10 15:54:39.000000 tensorwrap-0.0.1.1/tensorwrap/nn/optimizers/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      663 2023-07-15 20:22:08.000000 tensorwrap-0.0.1.1/tensorwrap/ops.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-05-26 22:29:10.000000 tensorwrap-0.0.1.1/tensorwrap/test.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      110 2023-07-16 15:20:59.000000 tensorwrap-0.0.1.1/tensorwrap/version.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 15:21:06.728131 tensorwrap-0.0.1.1/tensorwrap.egg-info/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6444 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1191 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 15:17:39.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/not-zip-safe
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      315 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/requires.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-07-16 15:21:06.000000 tensorwrap-0.0.1.1/tensorwrap.egg-info/top_level.txt
```

### Comparing `tensorwrap-0.0.0.6/LICENSE` & `tensorwrap-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.0.6/PKG-INFO` & `tensorwrap-0.0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.0.6
+Version: 0.0.1.1
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 | [**Install guide**](#installation)
 
 
 ## What is TensorWrap?
 
 TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar feel of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
 
-TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting Autograd in native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library aims to improve the poor design of the TensorFlow API and making it more friendly towards research and educational audiences.
+TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
 
 This is a personal project, not professionally affliated with Google in any way. Expect bugs and several incompatibilities/difference from the original libraries.
 Please help by trying it out, [reporting
 bugs](https://github.com/Impure-King/base-tensorwrap/issues), and letting me know what you
 think!
 
 ### Contents
@@ -50,81 +50,82 @@
 1) Custom Layers
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
 
 class Dense(nn.layers.Layer):
     def __init__(self, units) -> None:
-        super().__init__() # Needed for making it JIT compatible.
+        super().__init__() # Needed for tracking trainable_variables.
         self.units = units # Defining the output shape
   
     def build(self, input_shape: tuple) -> None:
         input_shape = tf.shape(input_shape) # Getting appropriate input shape
+        
+        # Naming each parameter to later access from model.trainable_variables
         self.kernel = self.add_weights([input_shape, self.units],
-                                       initializer = 'glorot_uniform')
+                                       initializer = 'glorot_uniform',
+                                       name='kernel')
         self.bias = self.add_weights([self.units],
-                                     initializer = 'zeros')
-        super().build(self.kernel, self.bias) # Needed to add the kernel to model.
+                                     initializer = 'zeros',
+                                     name='bias')
+        super().build() # Required for letting model know that layer is built.
     
     # Use call not __call__ to define the flow. No tf.function needed either.
-    def call(self, inputs):
-        return inputs @ self.kernel + self.bias
-```
+    def call(self, params, inputs):
+        return inputs @ params['kernel'] + params['bias'] # Using params as an input, allows use to pass in the model.trainable_variables later.
+ ```
 
 2) Just In Time Compiling with tf.function
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
 tf.test.is_device_available(device_type = 'cuda')
 
 @tf.function
 def mse(y_pred, y_true):
     return tf.mean(tf.square(y_pred - y_true))
 
 print(mse(100, 102))
 ```
-3) Customizing with Module Class
+3) Custom Models
 ```python 
 
 class CheckPoint(Module):
     def __init__(self, metrics) -> None:
         
 
 ```
 
 
 ### Current Gimmicks
 1. Current models are all compiled by JAX's internal jit, so any error may remain a bit more cryptic than PyTorchs. However, this problem is still being worked on.
 
 2. Also, using ``tensorwrap.Module`` is currently not recommended, since other superclasses offer more functionality and ease of use.
 
-3. Sometime, the JAX backend may give out and give an algorithmic error. Another high priority, though this one is hidden in the C++ api of JIT.
-
-4. The JIT compilation is currently double of TensorFlow's on big models. However, the speed up is immense.
+3. Graph execution is currently not available, which means that all exported models can only be deployed within a python environment.
 
-5. Graph execution is currently not available, which means that all exported models can only be deployed within a python environment.
 
 
 ### Installation
 
-The device installation of TensorWrap depends on its backend, being JAX. Thus, our normal install will be covering both the GPU and CPU installation.
+The device installation of TensorWrap depends on its backend, being JAX. Thus, our normal install will be covering only the cpu version. For gpu version, please check [JAX](https://github.com/google/jax)'s documentation.
 
 ```bash
 pip install --upgrade pip
 pip install --upgrade tensorwrap
 ```
 
 On Linux, it is often necessary to first update `pip` to a version that supports
 `manylinux2014` wheels. Also note that for Linux, we currently release wheels for `x86_64` architectures only, other architectures require building from source. Trying to pip install with other Linux architectures may lead to `jaxlib` not being installed alongside `jax`, although `jax` may successfully install (but fail at runtime). 
 **These `pip` installations do not work with Windows, and may fail silently; see
 [above](#installation).**
 
 **Note**
 
-If any problems occur with cuda installation, please visit the [JAX](www.github.com/google/jax) github page, in order to understand the problem with lower API installation.
+If any problems occur with cuda installation, please visit the [JAX](https://github.com/google/jax#installation) github page, in order to understand the problem with lower API installation.
 
 ## Citations
 
 This project have been heavily inspired by __TensorFlow__ and once again, is built on the open-source machine learning XLA framework __JAX__. Therefore, I recognize the authors of JAX and TensorFlow for the exceptional work they have done and understand that my library doesn't profit in any sort of way, since it is merely an add-on to the already existing community.
 
 ```
 @software{jax2018github,
```

### Comparing `tensorwrap-0.0.0.6/README.md` & `tensorwrap-0.0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 | [**Install guide**](#installation)
 
 
 ## What is TensorWrap?
 
 TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar feel of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
 
-TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting Autograd in native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library aims to improve the poor design of the TensorFlow API and making it more friendly towards research and educational audiences.
+TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
 
 This is a personal project, not professionally affliated with Google in any way. Expect bugs and several incompatibilities/difference from the original libraries.
 Please help by trying it out, [reporting
 bugs](https://github.com/Impure-King/base-tensorwrap/issues), and letting me know what you
 think!
 
 ### Contents
@@ -34,81 +34,82 @@
 1) Custom Layers
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
 
 class Dense(nn.layers.Layer):
     def __init__(self, units) -> None:
-        super().__init__() # Needed for making it JIT compatible.
+        super().__init__() # Needed for tracking trainable_variables.
         self.units = units # Defining the output shape
   
     def build(self, input_shape: tuple) -> None:
         input_shape = tf.shape(input_shape) # Getting appropriate input shape
+        
+        # Naming each parameter to later access from model.trainable_variables
         self.kernel = self.add_weights([input_shape, self.units],
-                                       initializer = 'glorot_uniform')
+                                       initializer = 'glorot_uniform',
+                                       name='kernel')
         self.bias = self.add_weights([self.units],
-                                     initializer = 'zeros')
-        super().build(self.kernel, self.bias) # Needed to add the kernel to model.
+                                     initializer = 'zeros',
+                                     name='bias')
+        super().build() # Required for letting model know that layer is built.
     
     # Use call not __call__ to define the flow. No tf.function needed either.
-    def call(self, inputs):
-        return inputs @ self.kernel + self.bias
-```
+    def call(self, params, inputs):
+        return inputs @ params['kernel'] + params['bias'] # Using params as an input, allows use to pass in the model.trainable_variables later.
+ ```
 
 2) Just In Time Compiling with tf.function
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
 tf.test.is_device_available(device_type = 'cuda')
 
 @tf.function
 def mse(y_pred, y_true):
     return tf.mean(tf.square(y_pred - y_true))
 
 print(mse(100, 102))
 ```
-3) Customizing with Module Class
+3) Custom Models
 ```python 
 
 class CheckPoint(Module):
     def __init__(self, metrics) -> None:
         
 
 ```
 
 
 ### Current Gimmicks
 1. Current models are all compiled by JAX's internal jit, so any error may remain a bit more cryptic than PyTorchs. However, this problem is still being worked on.
 
 2. Also, using ``tensorwrap.Module`` is currently not recommended, since other superclasses offer more functionality and ease of use.
 
-3. Sometime, the JAX backend may give out and give an algorithmic error. Another high priority, though this one is hidden in the C++ api of JIT.
-
-4. The JIT compilation is currently double of TensorFlow's on big models. However, the speed up is immense.
+3. Graph execution is currently not available, which means that all exported models can only be deployed within a python environment.
 
-5. Graph execution is currently not available, which means that all exported models can only be deployed within a python environment.
 
 
 ### Installation
 
-The device installation of TensorWrap depends on its backend, being JAX. Thus, our normal install will be covering both the GPU and CPU installation.
+The device installation of TensorWrap depends on its backend, being JAX. Thus, our normal install will be covering only the cpu version. For gpu version, please check [JAX](https://github.com/google/jax)'s documentation.
 
 ```bash
 pip install --upgrade pip
 pip install --upgrade tensorwrap
 ```
 
 On Linux, it is often necessary to first update `pip` to a version that supports
 `manylinux2014` wheels. Also note that for Linux, we currently release wheels for `x86_64` architectures only, other architectures require building from source. Trying to pip install with other Linux architectures may lead to `jaxlib` not being installed alongside `jax`, although `jax` may successfully install (but fail at runtime). 
 **These `pip` installations do not work with Windows, and may fail silently; see
 [above](#installation).**
 
 **Note**
 
-If any problems occur with cuda installation, please visit the [JAX](www.github.com/google/jax) github page, in order to understand the problem with lower API installation.
+If any problems occur with cuda installation, please visit the [JAX](https://github.com/google/jax#installation) github page, in order to understand the problem with lower API installation.
 
 ## Citations
 
 This project have been heavily inspired by __TensorFlow__ and once again, is built on the open-source machine learning XLA framework __JAX__. Therefore, I recognize the authors of JAX and TensorFlow for the exceptional work they have done and understand that my library doesn't profit in any sort of way, since it is merely an add-on to the already existing community.
 
 ```
 @software{jax2018github,
```

### Comparing `tensorwrap-0.0.0.6/setup.py` & `tensorwrap-0.0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 install_requires = [
     "numpy>=1.12",
     "jax>=0.3.16",
     "jaxlib",
     "dill",
     "matplotlib",  # only needed for tensorboard export
     "pandas",
-    "jaxtyping"
+    "jaxtyping",
+    "optax"
 ]
 
 tests_require = [
     "atari-py==0.2.5",  # Last version does not have the ROMs we test on pre-packaged
     "clu",  # All examples.
     "gym==0.18.3",
     "jaxlib",
```

### Comparing `tensorwrap-0.0.0.6/tensorwrap/__init__.py` & `tensorwrap-0.0.1.1/tensorwrap/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 # Error Silencer:
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
 # Library Paths:
 from tensorwrap import nn
-from tensorwrap import module
 from tensorwrap import test
 from tensorwrap import config
 
 # Path Shortener:
 from tensorwrap.module import Module
 from tensorwrap.version import __version__
 from tensorwrap.experimental.serialize import save_model, load_model
 from tensorwrap.experimental.wrappers import function
-from tensorwrap.ops import last_dim, comprehend, jit_decoder, jit_encoder, object_decoder, object_encoder
+from tensorwrap.ops import (last_dim,
+                            randu,
+                            randn)
 
 # JAX Built-ins:
 from jax import (disable_jit,
                  value_and_grad,
                  grad)
 from jax.numpy import (array as Variable,
                        arange as range,
@@ -38,8 +39,9 @@
                        float64,
                        eye as identity,
                        shape,
                        prod,
                        max,
                        min,
                        maximum,
-                       minimum)
+                       minimum,
+                       zeros)
```

### Comparing `tensorwrap-0.0.0.6/tensorwrap/config.py` & `tensorwrap-0.0.1.1/tensorwrap/config.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.0.6/tensorwrap/experimental/serialize.py` & `tensorwrap-0.0.1.1/tensorwrap/experimental/serialize.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.0.6/tensorwrap/module.py` & `tensorwrap-0.0.1.1/tensorwrap/module.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,83 @@
+import jax
 from typing import Any
 from abc import ABCMeta, abstractmethod
 from jax import jit
 from jax.tree_util import register_pytree_node_class
-
+from inspect import signature
+import tensorwrap as tf
 
 # All classes allowed for export.
 __all__ = ["Module"]
 
 
-class BaseModule(metaclass=ABCMeta):
-    """ This is the most basic template that defines all subclass items to be a pytree and accept arguments flexibly.
-    Don't use this template and instead refer to the Module Template, in order to create custom parts. If really needed,
-    use the PyTorch variation which will be suited for research."""
-
-    def __init__(self, *args, **kwargs) -> None:
-        # Setting all the argument attributes:
-        for key, value in enumerate(args):
-            setattr(self, f"arg_{key}", value)
-
-        # Setting all the keyword argument attributes:
-        for key, value in kwargs.items():
-            setattr(self, key, value)
+@register_pytree_node_class
+class Module(metaclass=ABCMeta):
+    """ Basic neural network module class.
+    
+    A module class is a named container that acts to transform all subclassed containers into
+    pytrees by appropriately defining the tree_flatten and tree_unflatten. Additionally, it 
+    defines the trackable trainable_variables for all the subclasses.
+    
+    NOTE: Due to the limited functionality of the Module class, it isn't recommended for 
+    general or even research use. Additionally, the Module class lacks functionality of the 
+    original TensorFlow implementation, so avoid any implementations of this class. Only made
+    for internal use and public api placeholder."""
+
+    def __init__(self) -> None:
+        """Helps instantiate the class and assign a self.trainable_variables to subclass."""
+        self.trainable_variables = {}
+        self.__unflattened = False
+
+    @classmethod
+    def __init_initialize__(cls):
+        """An extremely dangerous method which empties our the __init__ method and then create an instance. 
+        After, repurposing the __init__ again and it returns an instance with an empty init function. DO NOT USE for external uses."""
+        
+        # function to replace __init__ temporarily:
+        def init_rep(self):
+            self.trainable_variables = {}
+        prev_init = cls.__init__ # Storing __init__ functionality
+        
+        # Emptying and creating a new instance
+        cls.__init__ = init_rep
+        instance = cls()
+
+        # Reverting changes and returning instance
+        cls.__init__ = prev_init
+
+        return instance
 
-    # This function is responsible for making the subclasses into PyTrees:
     def __init_subclass__(cls) -> None:
+        """Used to convert and register all the subclasses into Pytrees."""
         register_pytree_node_class(cls)
 
     def __call__(self, *args, **kwargs) -> Any:
+        """Maintains the call() convention for all subclasses."""
         return self.call(*args, **kwargs)
 
-    @abstractmethod
     def call(self, *args, **kwargs):
+        """Acts as an abstract method to force all implementation to occur in the `call` method."""
         pass
 
-
-# Creating the unrolled tree class:
-class Module(BaseModule):
-    """This is the base class for all types of functions and components.
-    This is going to be a static type component, in order to allow jit.compile
-    from jax and accelerate the training process."""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-    
-    def __init_subclass__(cls) -> None:
-        super().__init_subclass__()
-
-    # Please improve in future versions
     def tree_flatten(self):
-        dic = vars(self).copy()
-        aux_data = {}
-        children = vars(self).values()
-        return (children, aux_data)
+        self.__unflattened = True
+        leaves = {}
+        # for key in self.trainable_variables:
+        #     leaves[key] = self.trainable_variables[key]
+        
+        # Removing trainable_variables:
+        aux_data = vars(self).copy()
+        # aux_data.pop("trainable_variables")
+
+        return leaves, aux_data
 
     @classmethod
     def tree_unflatten(cls, aux_data, children):
-        instance = cls(*children, **aux_data)
+        instance = cls.__init_initialize__()
+        instance.trainable_variables = children
+        vars(instance).update(aux_data)
         return instance
+    
+
 
-    def call(self):
-        pass
```

### Comparing `tensorwrap-0.0.0.6/tensorwrap.egg-info/PKG-INFO` & `tensorwrap-0.0.1.1/tensorwrap.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.0.6
+Version: 0.0.1.1
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 | [**Install guide**](#installation)
 
 
 ## What is TensorWrap?
 
 TensorWrap is high performance neural network library that acts as a wrapper around [JAX](https://github.com/google/jax) (another high performance machine learning library), bringing the familiar feel of the [TensorFlow](https://tensorflow.org) (2.x.x). This is currently aimed towards prototyping over deployment, in the current state. 
 
-TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting Autograd in native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library aims to improve the poor design of the TensorFlow API and making it more friendly towards research and educational audiences.
+TensorWrap works by creating a layer of abstraction over JAX's low level api and introducing similar TensorFlow-like component's while supporting native JAX operations. Additionally, the api has been updated to become more simpler and concise than TensorFlow's current API, by removing the redundant API's and deprecations that it possesses. Additionally, this library adds additional features and leverages JAX's optimizations, making it more friendly towards research and educational audiences.
 
 This is a personal project, not professionally affliated with Google in any way. Expect bugs and several incompatibilities/difference from the original libraries.
 Please help by trying it out, [reporting
 bugs](https://github.com/Impure-King/base-tensorwrap/issues), and letting me know what you
 think!
 
 ### Contents
@@ -50,81 +50,82 @@
 1) Custom Layers
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
 
 class Dense(nn.layers.Layer):
     def __init__(self, units) -> None:
-        super().__init__() # Needed for making it JIT compatible.
+        super().__init__() # Needed for tracking trainable_variables.
         self.units = units # Defining the output shape
   
     def build(self, input_shape: tuple) -> None:
         input_shape = tf.shape(input_shape) # Getting appropriate input shape
+        
+        # Naming each parameter to later access from model.trainable_variables
         self.kernel = self.add_weights([input_shape, self.units],
-                                       initializer = 'glorot_uniform')
+                                       initializer = 'glorot_uniform',
+                                       name='kernel')
         self.bias = self.add_weights([self.units],
-                                     initializer = 'zeros')
-        super().build(self.kernel, self.bias) # Needed to add the kernel to model.
+                                     initializer = 'zeros',
+                                     name='bias')
+        super().build() # Required for letting model know that layer is built.
     
     # Use call not __call__ to define the flow. No tf.function needed either.
-    def call(self, inputs):
-        return inputs @ self.kernel + self.bias
-```
+    def call(self, params, inputs):
+        return inputs @ params['kernel'] + params['bias'] # Using params as an input, allows use to pass in the model.trainable_variables later.
+ ```
 
 2) Just In Time Compiling with tf.function
 ```python
 import tensorwrap as tf
 from tensorwrap import nn
 tf.test.is_device_available(device_type = 'cuda')
 
 @tf.function
 def mse(y_pred, y_true):
     return tf.mean(tf.square(y_pred - y_true))
 
 print(mse(100, 102))
 ```
-3) Customizing with Module Class
+3) Custom Models
 ```python 
 
 class CheckPoint(Module):
     def __init__(self, metrics) -> None:
         
 
 ```
 
 
 ### Current Gimmicks
 1. Current models are all compiled by JAX's internal jit, so any error may remain a bit more cryptic than PyTorchs. However, this problem is still being worked on.
 
 2. Also, using ``tensorwrap.Module`` is currently not recommended, since other superclasses offer more functionality and ease of use.
 
-3. Sometime, the JAX backend may give out and give an algorithmic error. Another high priority, though this one is hidden in the C++ api of JIT.
-
-4. The JIT compilation is currently double of TensorFlow's on big models. However, the speed up is immense.
+3. Graph execution is currently not available, which means that all exported models can only be deployed within a python environment.
 
-5. Graph execution is currently not available, which means that all exported models can only be deployed within a python environment.
 
 
 ### Installation
 
-The device installation of TensorWrap depends on its backend, being JAX. Thus, our normal install will be covering both the GPU and CPU installation.
+The device installation of TensorWrap depends on its backend, being JAX. Thus, our normal install will be covering only the cpu version. For gpu version, please check [JAX](https://github.com/google/jax)'s documentation.
 
 ```bash
 pip install --upgrade pip
 pip install --upgrade tensorwrap
 ```
 
 On Linux, it is often necessary to first update `pip` to a version that supports
 `manylinux2014` wheels. Also note that for Linux, we currently release wheels for `x86_64` architectures only, other architectures require building from source. Trying to pip install with other Linux architectures may lead to `jaxlib` not being installed alongside `jax`, although `jax` may successfully install (but fail at runtime). 
 **These `pip` installations do not work with Windows, and may fail silently; see
 [above](#installation).**
 
 **Note**
 
-If any problems occur with cuda installation, please visit the [JAX](www.github.com/google/jax) github page, in order to understand the problem with lower API installation.
+If any problems occur with cuda installation, please visit the [JAX](https://github.com/google/jax#installation) github page, in order to understand the problem with lower API installation.
 
 ## Citations
 
 This project have been heavily inspired by __TensorFlow__ and once again, is built on the open-source machine learning XLA framework __JAX__. Therefore, I recognize the authors of JAX and TensorFlow for the exceptional work they have done and understand that my library doesn't profit in any sort of way, since it is merely an add-on to the already existing community.
 
 ```
 @software{jax2018github,
```

