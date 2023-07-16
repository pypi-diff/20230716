# Comparing `tmp/quik-ai-1.3.1.tar.gz` & `tmp/quik-ai-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik-ai-1.3.1.tar", last modified: Tue Jul  4 16:29:19 2023, max compression
+gzip compressed data, was "quik-ai-1.3.2.tar", last modified: Sun Jul 16 12:08:27 2023, max compression
```

## Comparing `quik-ai-1.3.1.tar` & `quik-ai-1.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.203240 quik-ai-1.3.1/
--rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     2270 2023-07-04 16:29:19.203240 quik-ai-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1732 2023-06-25 22:06:12.000000 quik-ai-1.3.1/README.md
--rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      768 2023-07-04 16:29:19.210744 quik-ai-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.142415 quik-ai-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.175006 quik-ai-1.3.1/src/quik_ai/
--rw-rw-rw-   0        0        0      445 2023-07-04 15:16:34.000000 quik-ai-1.3.1/src/quik_ai/__init__.py
--rw-rw-rw-   0        0        0     2440 2023-06-11 23:04:01.000000 quik-ai-1.3.1/src/quik_ai/backend.py
--rw-rw-rw-   0        0        0    13361 2023-06-27 22:06:46.000000 quik-ai-1.3.1/src/quik_ai/engine.py
--rw-rw-rw-   0        0        0     5511 2023-07-04 15:19:01.000000 quik-ai-1.3.1/src/quik_ai/heads.py
--rw-rw-rw-   0        0        0    20052 2023-06-28 21:09:36.000000 quik-ai-1.3.1/src/quik_ai/layers.py
--rw-rw-rw-   0        0        0      941 2023-06-24 18:02:43.000000 quik-ai-1.3.1/src/quik_ai/losses.py
--rw-rw-rw-   0        0        0     3868 2023-06-28 22:37:12.000000 quik-ai-1.3.1/src/quik_ai/metrics.py
--rw-rw-rw-   0        0        0    30799 2023-07-04 15:17:15.000000 quik-ai-1.3.1/src/quik_ai/models.py
--rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.3.1/src/quik_ai/optimizers.py
--rw-rw-rw-   0        0        0    12821 2023-06-25 14:51:52.000000 quik-ai-1.3.1/src/quik_ai/predictors.py
--rw-rw-rw-   0        0        0     9426 2023-06-24 00:56:24.000000 quik-ai-1.3.1/src/quik_ai/tuners.py
--rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.3.1/src/quik_ai/tuning.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.202219 quik-ai-1.3.1/src/quik_ai.egg-info/
--rw-rw-rw-   0        0        0     2270 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 12:08:27.539530 quik-ai-1.3.2/
+-rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2270 2023-07-16 12:08:27.540528 quik-ai-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-06-25 22:06:12.000000 quik-ai-1.3.2/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      768 2023-07-16 12:08:27.547510 quik-ai-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:08:27.390658 quik-ai-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 12:08:27.508278 quik-ai-1.3.2/src/quik_ai/
+-rw-rw-rw-   0        0        0      445 2023-07-04 15:16:34.000000 quik-ai-1.3.2/src/quik_ai/__init__.py
+-rw-rw-rw-   0        0        0     2440 2023-06-11 23:04:01.000000 quik-ai-1.3.2/src/quik_ai/backend.py
+-rw-rw-rw-   0        0        0    13361 2023-06-27 22:06:46.000000 quik-ai-1.3.2/src/quik_ai/engine.py
+-rw-rw-rw-   0        0        0     7207 2023-07-16 12:05:13.000000 quik-ai-1.3.2/src/quik_ai/heads.py
+-rw-rw-rw-   0        0        0    21977 2023-07-16 12:04:41.000000 quik-ai-1.3.2/src/quik_ai/layers.py
+-rw-rw-rw-   0        0        0      941 2023-06-24 18:02:43.000000 quik-ai-1.3.2/src/quik_ai/losses.py
+-rw-rw-rw-   0        0        0     3868 2023-06-28 22:37:12.000000 quik-ai-1.3.2/src/quik_ai/metrics.py
+-rw-rw-rw-   0        0        0    30799 2023-07-15 18:56:17.000000 quik-ai-1.3.2/src/quik_ai/models.py
+-rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.3.2/src/quik_ai/optimizers.py
+-rw-rw-rw-   0        0        0    13145 2023-07-15 18:56:17.000000 quik-ai-1.3.2/src/quik_ai/predictors.py
+-rw-rw-rw-   0        0        0     9426 2023-06-24 00:56:24.000000 quik-ai-1.3.2/src/quik_ai/tuners.py
+-rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.3.2/src/quik_ai/tuning.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:08:27.538529 quik-ai-1.3.2/src/quik_ai.egg-info/
+-rw-rw-rw-   0        0        0     2270 2023-07-16 12:08:27.000000 quik-ai-1.3.2/src/quik_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-07-16 12:08:27.000000 quik-ai-1.3.2/src/quik_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 12:08:27.000000 quik-ai-1.3.2/src/quik_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-07-16 12:08:27.000000 quik-ai-1.3.2/src/quik_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 12:08:27.000000 quik-ai-1.3.2/src/quik_ai.egg-info/top_level.txt
```

### Comparing `quik-ai-1.3.1/LICENSE` & `quik-ai-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/PKG-INFO` & `quik-ai-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.3.1
+Version: 1.3.2
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.1.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.2.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quik-ai-1.3.1/README.md` & `quik-ai-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/setup.cfg` & `quik-ai-1.3.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7569 6b2d 6169 0d0a 7665 7273   = quik-ai..vers
-00000020: 696f 6e20 3d20 312e 332e 310d 0a61 7574  ion = 1.3.1..aut
+00000020: 696f 6e20 3d20 312e 332e 320d 0a61 7574  ion = 1.3.2..aut
 00000030: 686f 7220 3d20 416c 656b 7361 6e64 7220  hor = Aleksandr 
 00000040: 546f 757a 6f76 0d0a 6465 7363 7269 7074  Touzov..descript
 00000050: 696f 6e20 3d20 5175 6963 6b20 556e 6966  ion = Quick Unif
 00000060: 7969 6e67 2049 6e66 7261 7374 7275 6374  ying Infrastruct
 00000070: 7572 6520 4b69 7420 666f 7220 4d61 6368  ure Kit for Mach
 00000080: 696e 6520 4c65 6172 6e69 6e67 2061 6e64  ine Learning and
 00000090: 2041 490d 0a6c 6f6e 675f 6465 7363 7269   AI..long_descri
@@ -16,15 +16,15 @@
 000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000100: 2f74 6f75 7a6f 7631 3031 322f 7175 696b  /touzov1012/quik
 00000110: 2d61 690d 0a64 6f77 6e6c 6f61 645f 7572  -ai..download_ur
 00000120: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000130: 7562 2e63 6f6d 2f74 6f75 7a6f 7631 3031  ub.com/touzov101
 00000140: 322f 7175 696b 2d61 692f 6172 6368 6976  2/quik-ai/archiv
 00000150: 652f 7265 6673 2f74 6167 732f 7631 2e33  e/refs/tags/v1.3
-00000160: 2e31 2e74 6172 2e67 7a0d 0a63 6c61 7373  .1.tar.gz..class
+00000160: 2e32 2e74 6172 2e67 7a0d 0a63 6c61 7373  .2.tar.gz..class
 00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
 00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
 000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001b0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
 000001c0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
 000001d0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
```

### Comparing `quik-ai-1.3.1/src/quik_ai/backend.py` & `quik-ai-1.3.2/src/quik_ai/backend.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai/engine.py` & `quik-ai-1.3.2/src/quik_ai/engine.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai/layers.py` & `quik-ai-1.3.2/src/quik_ai/layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,62 @@
 import tensorflow_probability as tfp
 
 from keras import backend
 from keras.engine import base_layer
 from keras.utils import control_flow_util
 
 @tf.keras.utils.register_keras_serializable(package="quik_ai")
+class Conv2DTransposeBlock(tf.keras.layers.Layer):
+    def __init__(self, event_shape, num_layers, kernel_size, hidden_dim, **kwargs):
+        super().__init__(**kwargs)
+        self.event_shape = event_shape
+        self.num_layers = num_layers
+        self.kernel_size = kernel_size
+        self.hidden_dim = hidden_dim
+    
+    def build(self, input_shape):
+        # reshape input to the output size
+        self.conv = tf.keras.Sequential([
+            tf.keras.layers.Dense(self.event_shape[0] * self.event_shape[1] * self.hidden_dim),
+            tf.keras.layers.Reshape((self.event_shape[0], self.event_shape[1], self.hidden_dim)),
+        ])
+        
+        # layer sizes
+        output_channels = 1 if len(self.event_shape) == 2 else self.event_shape[-1]
+        if self.num_layers <= 1:
+            sizes = [output_channels]
+        else:
+            sizes = np.geomspace(self.hidden_dim, output_channels, self.num_layers).round(0).astype(int)
+        
+        # add layers
+        for idx in range(len(sizes)):
+            self.conv.add(tf.keras.layers.Conv2DTranspose(sizes[idx], kernel_size=self.kernel_size, strides=1, padding='same'))
+            
+            # add activations for intermediate layers
+            if idx < len(sizes) - 1:
+                self.conv.add(tf.keras.layers.BatchNormalization())
+                self.conv.add(tf.keras.layers.LeakyReLU())
+        
+        # add final shape layer
+        self.conv.add(tf.keras.layers.Reshape(self.event_shape))
+    
+    def call(self, inputs):
+        return self.conv(inputs)
+    
+    def get_config(self):
+        config = super().get_config()
+        config.update({
+            'event_shape' : self.event_shape,
+            'num_layers' : self.num_layers,
+            'kernel_size' : self.kernel_size,
+            'hidden_dim' : self.hidden_dim,
+        })
+        return config
+
+@tf.keras.utils.register_keras_serializable(package="quik_ai")
 class FeatureFlatten(tf.keras.layers.Layer):
     def build(self, input_shape):
         self.flatten_dims = np.prod(input_shape[1:-1])
         super().build(input_shape)
 
     def call(self, inputs):
         shape = tf.shape(inputs)
```

### Comparing `quik-ai-1.3.1/src/quik_ai/losses.py` & `quik-ai-1.3.2/src/quik_ai/losses.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai/metrics.py` & `quik-ai-1.3.2/src/quik_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai/models.py` & `quik-ai-1.3.2/src/quik_ai/models.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai/optimizers.py` & `quik-ai-1.3.2/src/quik_ai/optimizers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai/predictors.py` & `quik-ai-1.3.2/src/quik_ai/predictors.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,325 +1,325 @@
-from quik_ai import tuning
-from quik_ai import layers
-
-import numpy as np
-import tensorflow as tf
-
-class Predictor(tuning.Tunable):
-    def __init__(self, names, drop=False, **kwargs):
-        super().__init__(names, **kwargs)
-        self.names = names if isinstance(names, (list, tuple)) else [names]
-        self.drop = drop
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        config.update({
-            'drop' : self._get_hp(None, 'drop', hp)
-        })
-        return config
-    
-    def transform(self, inputs, driver, time_window, hp):
-        return None
-
-class Lambda(Predictor):
-    def __init__(self, names, lambdas=None, **kwargs):
-        super().__init__(names, **kwargs)
-        
-        if callable(lambdas):
-            lambdas = [lambdas]
-        
-        if not isinstance(lambdas, (list, tuple)):
-            raise ValueError('Expected lambdas as a list of functions')
-        
-        self.lambda_count = len(lambdas)
-        
-        for i in range(self.lambda_count):
-            lbda = lambdas[i]
-            if isinstance(lbda, (list, tuple)):
-                setattr(self, 'lambda_%s' % i, lbda[0])
-                setattr(self, 'lambda_%s_drop' % i, lbda[1])
-            elif callable(lbda):
-                setattr(self, 'lambda_%s' % i, lbda)
-                setattr(self, 'lambda_%s_drop' % i, False)
-            else:
-                raise ValueError('Each lambda in lambdas should be a function or a tuple of (function, boolean)')
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        
-        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
-            for i in range(self.lambda_count):
-                config['lambda_%s_drop' % i] = self._get_hp(scope, 'lambda_%s_drop' % i, hp)
-        
-        return config
-    
-    def transform(self, inputs, driver, time_window, hp):
-        config = self.get_parameters(hp)
-        
-        if config['drop']:
-            return None
-        
-        if self.lambda_count == 0:
-            return None
-        
-        res = []
-        for i in range(self.lambda_count):
-            if not config['lambda_%s_drop' % i]:
-                lbda = getattr(self, 'lambda_%s' % i)
-                res.append(lbda(inputs, driver, time_window, **config))
-        
-        if len(res) == 0:
-            return None
-        
-        return tf.concat(res, axis=-1)
-    
-class Numerical(Lambda):
-    def __init__(self, names, normalize=False, **kwargs):
-        super().__init__(names, lambdas=self.body, **kwargs)
-        self.normalize = normalize
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        
-        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
-            config['normalize'] = self._get_hp(scope, 'normalize', hp)
-        
-        return config
-    
-    def body(self, inputs, driver, time_window, normalize, **kwargs):  
-        
-        outputs = []
-        
-        if normalize:
-            for name in self.names:
-                normal_layer = tf.keras.layers.Normalization()
-                normal_layer.adapt(driver.get_data_tensor(driver.training_data, name))
-                outputs.append(normal_layer(inputs[name]))
-        else:
-            for name in self.names:
-                outputs.append(inputs[name])
-        
-        return tf.concat(outputs, axis=-1)
-
-class Image(Lambda):
-    def __init__(
-        self, 
-        names, 
-        height=None,
-        width=None,
-        standardize=True, 
-        mask_n=None,
-        filters=tuning.HyperInt(min_value=8, max_value=32, step=8),
-        kernel_size=tuning.HyperInt(min_value=4, max_value=8, step=2),
-        stride_rate=tuning.HyperFloat(min_value=0.0, max_value=1.0, step=0.25),
-        **kwargs
-    ):
-        super().__init__(names, lambdas=self.body, **kwargs)
-        
-        self.height = height
-        self.width = width
-        self.standardize = standardize
-        self.mask_n = mask_n
-        self.filters = filters
-        self.kernel_size = kernel_size
-        self.stride_rate = stride_rate
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        
-        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
-            config['height'] = self._get_hp(scope, 'height', hp)
-            config['width'] = self._get_hp(scope, 'width', hp)
-            config['standardize'] = self._get_hp(scope, 'standardize', hp)
-            config['filters'] = self._get_hp(scope, 'filters', hp)
-            config['kernel_size'] = self._get_hp(scope, 'kernel_size', hp)
-            config['stride_rate'] = self._get_hp(scope, 'stride_rate', hp)
-        
-        return config
-    
-    def body(self, inputs, driver, time_window, height, width, standardize, filters, kernel_size, stride_rate, **kwargs):  
-        
-        # we may have negative height and width, this means do not resize
-        height = None if height is not None and height <= 0 else height
-        width = None if width is not None and width <= 0 else width
-        
-        # append the output stack
-        outputs = []
-        for name in self.names:
-            outputs.append(inputs[name])
-        
-        # if for some reason we want to glue the images,
-        # treat the images as extended channels
-        outputs = tf.concat(outputs, axis=-1)
-        
-        # if we want to standardize to [0,1] range
-        if standardize:
-            outputs = tf.keras.layers.Rescaling(1./255)(outputs)
-        
-        # check the input shape size and if we have video
-        has_time = time_window > 1
-        
-        # resize if we need
-        if has_time and len(outputs.shape) != 5 or not has_time and len(outputs.shape) != 4:
-            outputs = tf.expand_dims(outputs, -1)
-        
-        # check that our video has correct dimensions
-        if has_time and len(outputs.shape) != 5:
-            raise ValueError('Image input must have (4) or (5) dimensions for video')
-        
-        # check that our image has correct dimensions
-        if not has_time and len(outputs.shape) != 4:
-            raise ValueError('Image input must have (3) or (4) dimensions for images')
-        
-        # apply resizing to the frames of the video or the image
-        # if we need it, or if we want to improve performance
-        curr_height = outputs.shape[2] if has_time else outputs.shape[1]
-        curr_width = outputs.shape[3] if has_time else outputs.shape[2]
-        if height is None and width is not None:
-            height = int(np.ceil(width / curr_width * curr_height))
-        if width is None and height is not None:
-            width = int(np.ceil(height / curr_height * curr_width))
-        if height is not None and width is not None:
-            resize_layer = tf.keras.layers.Resizing(height, width)
-            resize_layer = tf.keras.layers.TimeDistributed(resize_layer) if has_time else resize_layer
-            outputs = resize_layer(outputs)
-        
-        # if we want to mask the last frame
-        if has_time and self.mask_n is not None:
-            unmasked, masked = tf.split(outputs, [-1, self.mask_n], axis=1)
-            masked = masked * 0.0
-            outputs = tf.concat([unmasked, masked], axis=1)
-        
-        # convolution for patches
-        strides = int(np.maximum(np.round(kernel_size * stride_rate), 1))
-        conv_layer = tf.keras.layers.Conv2D(filters, kernel_size, strides=strides, padding='same')
-        conv_layer = tf.keras.layers.TimeDistributed(conv_layer) if has_time else conv_layer
-        outputs = conv_layer(outputs)
-        
-        # best output shape, either flatten all the features over time, or flatten middle dims
-        outputs = layers.TimeFlatten()(outputs) if has_time else layers.FeatureFlatten()(outputs)
-        
-        # return the result
-        return outputs
-
-class Periodic(Lambda):
-    def __init__(self, names, period, **kwargs):
-        super().__init__(names, lambdas=self.body, **kwargs)
-        self.period = period
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        
-        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
-            config['period'] = self._get_hp(scope, 'period', hp)
-        
-        return config
-    
-    def body(self, inputs, driver, time_window, period, **kwargs):
-        outputs = [inputs[name] for name in self.names]
-        
-        outputs = tf.concat(outputs, axis=-1)
-        
-        theta = 2 * np.pi * outputs / period
-        
-        return tf.concat([tf.math.sin(theta), tf.math.cos(theta)], axis=-1)
-    
-class TimeMasked(Lambda):
-    def __init__(self, names, mask_n=1, **kwargs):
-        super().__init__(names, lambdas=self.body, **kwargs)
-        self.mask_n = mask_n
-    
-    def body(self, inputs, driver, time_window, **kwargs):
-        outputs = [inputs[name] for name in self.names]
-        
-        outputs = tf.concat(outputs, axis=-1)
-        
-        if len(outputs.shape) < 3:
-            raise ValueError('Time masked predictor must have at least (3) dimensions')
-        
-        unmasked, masked = tf.split(outputs, [-1, self.mask_n], axis=1)
-        masked = masked * 0.0
-        
-        return tf.concat([unmasked, masked], axis=1)
-
-class Categorical(Lambda):
-    def __init__(
-        self, 
-        names, 
-        dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        use_one_hot=tuning.HyperBoolean(),
-        embed_dim=tuning.HyperInt(min_value=8, max_value=32, step=8),
-        embed_l2_regularizer=tuning.HyperFloat(min_value=0.0, max_value=0.2, step=0.1),
-        dropout_token='[UNK]',
-        seed=None,
-        **kwargs
-    ):
-        super().__init__(names, lambdas=self.body, **kwargs)
-        self.dropout = dropout
-        self.use_one_hot = use_one_hot
-        self.embed_dim = embed_dim
-        self.embed_l2_regularizer = embed_l2_regularizer
-        self.dropout_token = dropout_token
-        self.seed = seed
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        
-        with self._condition_on_parent(hp, 'drop', [False], scope=None) as drop_scope:
-            config['dropout'] = self._get_hp(drop_scope, 'dropout', hp)
-            config['use_one_hot'] = self._get_hp(drop_scope, 'use_one_hot', hp)
-            with self._condition_on_parent(hp, 'use_one_hot', [False], scope=drop_scope) as one_hot_scope:
-                config['embed_dim'] = self._get_hp(one_hot_scope, 'embed_dim', hp)
-                config['embed_l2_regularizer'] = self._get_hp(one_hot_scope, 'embed_l2_regularizer', hp)
-        
-        return config
-    
-    def body(self, inputs, driver, time_window, dropout, use_one_hot, embed_dim, embed_l2_regularizer, **kwargs):
-        outputs = [inputs[name] for name in self.names]
-        
-        # format to flat tensor for each input, this will be
-        # expanded by a dimension in the end to (3)
-        for i in range(len(outputs)):
-            input_shape = len(outputs[i].shape)
-            
-            if input_shape > 3:
-                raise ValueError('Categorical predictor input must be (1) dims for flat data, or (2) dims for time-series')
-
-            # flatten time series
-            if input_shape == 3:
-                outputs[i] = tf.squeeze(outputs[i], axis=2)
-        
-        # create dropout layer
-        dropout_layer = layers.CategoricalDropout(
-            dropout=dropout, 
-            dropout_token=self.dropout_token,
-            seed=self.seed,
-        )
-        
-        # apply dropout to each input
-        for i in range(len(outputs)):
-            outputs[i] = dropout_layer(outputs[i])
-            
-            # encode to numeric
-            encode_layer = tf.keras.layers.StringLookup(oov_token=self.dropout_token)
-            encode_layer.adapt(np.unique(driver.get_data_tensor(driver.training_data, self.names[i])))
-            outputs[i] = encode_layer(outputs[i])
-            
-            # get the vocab size for this input
-            vocab_size = len(encode_layer.get_vocabulary())
-        
-            # if one hot encoding
-            if use_one_hot:
-                outputs[i] = tf.keras.layers.Embedding(
-                    input_dim=vocab_size,
-                    output_dim=vocab_size,
-                    embeddings_initializer=tf.keras.initializers.Identity(),
-                    trainable=False,
-                )(outputs[i])
-            else: # we are embedding categories
-                outputs[i] = tf.keras.layers.Embedding(
-                    input_dim=vocab_size,
-                    output_dim=embed_dim,
-                    embeddings_regularizer=tf.keras.regularizers.L2(embed_l2_regularizer),
-                )(outputs[i])
-        
+from quik_ai import tuning
+from quik_ai import layers
+
+import numpy as np
+import tensorflow as tf
+
+class Predictor(tuning.Tunable):
+    def __init__(self, names, drop=False, **kwargs):
+        super().__init__(names, **kwargs)
+        self.names = names if isinstance(names, (list, tuple)) else [names]
+        self.drop = drop
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        config.update({
+            'drop' : self._get_hp(None, 'drop', hp)
+        })
+        return config
+    
+    def transform(self, inputs, driver, time_window, hp):
+        return None
+
+class Lambda(Predictor):
+    def __init__(self, names, lambdas=None, **kwargs):
+        super().__init__(names, **kwargs)
+        
+        if callable(lambdas):
+            lambdas = [lambdas]
+        
+        if not isinstance(lambdas, (list, tuple)):
+            raise ValueError('Expected lambdas as a list of functions')
+        
+        self.lambda_count = len(lambdas)
+        
+        for i in range(self.lambda_count):
+            lbda = lambdas[i]
+            if isinstance(lbda, (list, tuple)):
+                setattr(self, 'lambda_%s' % i, lbda[0])
+                setattr(self, 'lambda_%s_drop' % i, lbda[1])
+            elif callable(lbda):
+                setattr(self, 'lambda_%s' % i, lbda)
+                setattr(self, 'lambda_%s_drop' % i, False)
+            else:
+                raise ValueError('Each lambda in lambdas should be a function or a tuple of (function, boolean)')
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        
+        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
+            for i in range(self.lambda_count):
+                config['lambda_%s_drop' % i] = self._get_hp(scope, 'lambda_%s_drop' % i, hp)
+        
+        return config
+    
+    def transform(self, inputs, driver, time_window, hp):
+        config = self.get_parameters(hp)
+        
+        if config['drop']:
+            return None
+        
+        if self.lambda_count == 0:
+            return None
+        
+        res = []
+        for i in range(self.lambda_count):
+            if not config['lambda_%s_drop' % i]:
+                lbda = getattr(self, 'lambda_%s' % i)
+                res.append(lbda(inputs, driver, time_window, **config))
+        
+        if len(res) == 0:
+            return None
+        
+        return tf.concat(res, axis=-1)
+    
+class Numerical(Lambda):
+    def __init__(self, names, normalize=False, **kwargs):
+        super().__init__(names, lambdas=self.body, **kwargs)
+        self.normalize = normalize
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        
+        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
+            config['normalize'] = self._get_hp(scope, 'normalize', hp)
+        
+        return config
+    
+    def body(self, inputs, driver, time_window, normalize, **kwargs):  
+        
+        outputs = []
+        
+        if normalize:
+            for name in self.names:
+                normal_layer = tf.keras.layers.Normalization()
+                normal_layer.adapt(driver.get_data_tensor(driver.training_data, name))
+                outputs.append(normal_layer(inputs[name]))
+        else:
+            for name in self.names:
+                outputs.append(inputs[name])
+        
+        return tf.concat(outputs, axis=-1)
+
+class Image(Lambda):
+    def __init__(
+        self, 
+        names, 
+        height=None,
+        width=None,
+        standardize=True, 
+        mask_n=None,
+        filters=tuning.HyperInt(min_value=8, max_value=32, step=8),
+        kernel_size=tuning.HyperInt(min_value=4, max_value=8, step=2),
+        stride_rate=tuning.HyperFloat(min_value=0.0, max_value=1.0, step=0.25),
+        **kwargs
+    ):
+        super().__init__(names, lambdas=self.body, **kwargs)
+        
+        self.height = height
+        self.width = width
+        self.standardize = standardize
+        self.mask_n = mask_n
+        self.filters = filters
+        self.kernel_size = kernel_size
+        self.stride_rate = stride_rate
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        
+        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
+            config['height'] = self._get_hp(scope, 'height', hp)
+            config['width'] = self._get_hp(scope, 'width', hp)
+            config['standardize'] = self._get_hp(scope, 'standardize', hp)
+            config['filters'] = self._get_hp(scope, 'filters', hp)
+            config['kernel_size'] = self._get_hp(scope, 'kernel_size', hp)
+            config['stride_rate'] = self._get_hp(scope, 'stride_rate', hp)
+        
+        return config
+    
+    def body(self, inputs, driver, time_window, height, width, standardize, filters, kernel_size, stride_rate, **kwargs):  
+        
+        # we may have negative height and width, this means do not resize
+        height = None if height is not None and height <= 0 else height
+        width = None if width is not None and width <= 0 else width
+        
+        # append the output stack
+        outputs = []
+        for name in self.names:
+            outputs.append(inputs[name])
+        
+        # if for some reason we want to glue the images,
+        # treat the images as extended channels
+        outputs = tf.concat(outputs, axis=-1)
+        
+        # if we want to standardize to [0,1] range
+        if standardize:
+            outputs = tf.keras.layers.Rescaling(1./255)(outputs)
+        
+        # check the input shape size and if we have video
+        has_time = time_window > 1
+        
+        # resize if we need
+        if has_time and len(outputs.shape) != 5 or not has_time and len(outputs.shape) != 4:
+            outputs = tf.expand_dims(outputs, -1)
+        
+        # check that our video has correct dimensions
+        if has_time and len(outputs.shape) != 5:
+            raise ValueError('Image input must have (4) or (5) dimensions for video')
+        
+        # check that our image has correct dimensions
+        if not has_time and len(outputs.shape) != 4:
+            raise ValueError('Image input must have (3) or (4) dimensions for images')
+        
+        # apply resizing to the frames of the video or the image
+        # if we need it, or if we want to improve performance
+        curr_height = outputs.shape[2] if has_time else outputs.shape[1]
+        curr_width = outputs.shape[3] if has_time else outputs.shape[2]
+        if height is None and width is not None:
+            height = int(np.ceil(width / curr_width * curr_height))
+        if width is None and height is not None:
+            width = int(np.ceil(height / curr_height * curr_width))
+        if height is not None and width is not None:
+            resize_layer = tf.keras.layers.Resizing(height, width)
+            resize_layer = tf.keras.layers.TimeDistributed(resize_layer) if has_time else resize_layer
+            outputs = resize_layer(outputs)
+        
+        # if we want to mask the last frame
+        if has_time and self.mask_n is not None:
+            unmasked, masked = tf.split(outputs, [-1, self.mask_n], axis=1)
+            masked = masked * 0.0
+            outputs = tf.concat([unmasked, masked], axis=1)
+        
+        # convolution for patches
+        strides = int(np.maximum(np.round(kernel_size * stride_rate), 1))
+        conv_layer = tf.keras.layers.Conv2D(filters, kernel_size, strides=strides, padding='same')
+        conv_layer = tf.keras.layers.TimeDistributed(conv_layer) if has_time else conv_layer
+        outputs = conv_layer(outputs)
+        
+        # best output shape, either flatten all the features over time, or flatten middle dims
+        outputs = layers.TimeFlatten()(outputs) if has_time else layers.FeatureFlatten()(outputs)
+        
+        # return the result
+        return outputs
+
+class Periodic(Lambda):
+    def __init__(self, names, period, **kwargs):
+        super().__init__(names, lambdas=self.body, **kwargs)
+        self.period = period
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        
+        with self._condition_on_parent(hp, 'drop', [False], scope=None) as scope:
+            config['period'] = self._get_hp(scope, 'period', hp)
+        
+        return config
+    
+    def body(self, inputs, driver, time_window, period, **kwargs):
+        outputs = [inputs[name] for name in self.names]
+        
+        outputs = tf.concat(outputs, axis=-1)
+        
+        theta = 2 * np.pi * outputs / period
+        
+        return tf.concat([tf.math.sin(theta), tf.math.cos(theta)], axis=-1)
+    
+class TimeMasked(Lambda):
+    def __init__(self, names, mask_n=1, **kwargs):
+        super().__init__(names, lambdas=self.body, **kwargs)
+        self.mask_n = mask_n
+    
+    def body(self, inputs, driver, time_window, **kwargs):
+        outputs = [inputs[name] for name in self.names]
+        
+        outputs = tf.concat(outputs, axis=-1)
+        
+        if len(outputs.shape) < 3:
+            raise ValueError('Time masked predictor must have at least (3) dimensions')
+        
+        unmasked, masked = tf.split(outputs, [-1, self.mask_n], axis=1)
+        masked = masked * 0.0
+        
+        return tf.concat([unmasked, masked], axis=1)
+
+class Categorical(Lambda):
+    def __init__(
+        self, 
+        names, 
+        dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        use_one_hot=tuning.HyperBoolean(),
+        embed_dim=tuning.HyperInt(min_value=8, max_value=32, step=8),
+        embed_l2_regularizer=tuning.HyperFloat(min_value=0.0, max_value=0.2, step=0.1),
+        dropout_token='[UNK]',
+        seed=None,
+        **kwargs
+    ):
+        super().__init__(names, lambdas=self.body, **kwargs)
+        self.dropout = dropout
+        self.use_one_hot = use_one_hot
+        self.embed_dim = embed_dim
+        self.embed_l2_regularizer = embed_l2_regularizer
+        self.dropout_token = dropout_token
+        self.seed = seed
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        
+        with self._condition_on_parent(hp, 'drop', [False], scope=None) as drop_scope:
+            config['dropout'] = self._get_hp(drop_scope, 'dropout', hp)
+            config['use_one_hot'] = self._get_hp(drop_scope, 'use_one_hot', hp)
+            with self._condition_on_parent(hp, 'use_one_hot', [False], scope=drop_scope) as one_hot_scope:
+                config['embed_dim'] = self._get_hp(one_hot_scope, 'embed_dim', hp)
+                config['embed_l2_regularizer'] = self._get_hp(one_hot_scope, 'embed_l2_regularizer', hp)
+        
+        return config
+    
+    def body(self, inputs, driver, time_window, dropout, use_one_hot, embed_dim, embed_l2_regularizer, **kwargs):
+        outputs = [inputs[name] for name in self.names]
+        
+        # format to flat tensor for each input, this will be
+        # expanded by a dimension in the end to (3)
+        for i in range(len(outputs)):
+            input_shape = len(outputs[i].shape)
+            
+            if input_shape > 3:
+                raise ValueError('Categorical predictor input must be (1) dims for flat data, or (2) dims for time-series')
+
+            # flatten time series
+            if input_shape == 3:
+                outputs[i] = tf.squeeze(outputs[i], axis=2)
+        
+        # create dropout layer
+        dropout_layer = layers.CategoricalDropout(
+            dropout=dropout, 
+            dropout_token=self.dropout_token,
+            seed=self.seed,
+        )
+        
+        # apply dropout to each input
+        for i in range(len(outputs)):
+            outputs[i] = dropout_layer(outputs[i])
+            
+            # encode to numeric
+            encode_layer = tf.keras.layers.StringLookup(oov_token=self.dropout_token)
+            encode_layer.adapt(np.unique(driver.get_data_tensor(driver.training_data, self.names[i])))
+            outputs[i] = encode_layer(outputs[i])
+            
+            # get the vocab size for this input
+            vocab_size = len(encode_layer.get_vocabulary())
+        
+            # if one hot encoding
+            if use_one_hot:
+                outputs[i] = tf.keras.layers.Embedding(
+                    input_dim=vocab_size,
+                    output_dim=vocab_size,
+                    embeddings_initializer=tf.keras.initializers.Identity(),
+                    trainable=False,
+                )(outputs[i])
+            else: # we are embedding categories
+                outputs[i] = tf.keras.layers.Embedding(
+                    input_dim=vocab_size,
+                    output_dim=embed_dim,
+                    embeddings_regularizer=tf.keras.regularizers.L2(embed_l2_regularizer),
+                )(outputs[i])
+        
         return tf.concat(outputs, axis=-1)
```

### Comparing `quik-ai-1.3.1/src/quik_ai/tuners.py` & `quik-ai-1.3.2/src/quik_ai/tuners.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai/tuning.py` & `quik-ai-1.3.2/src/quik_ai/tuning.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.1/src/quik_ai.egg-info/PKG-INFO` & `quik-ai-1.3.2/src/quik_ai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.3.1
+Version: 1.3.2
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.1.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.2.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

