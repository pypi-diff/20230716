# Comparing `tmp/eznet_keras-1.0.1.tar.gz` & `tmp/eznet_keras-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eznet_keras-1.0.1.tar", last modified: Sun Jul 16 11:46:36 2023, max compression
+gzip compressed data, was "eznet_keras-1.0.2.tar", last modified: Sun Jul 16 12:29:35 2023, max compression
```

## Comparing `eznet_keras-1.0.1.tar` & `eznet_keras-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.469225 eznet_keras-1.0.1/
--rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0    14243 2023-07-16 11:46:36.469225 eznet_keras-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    13171 2023-07-16 11:45:27.000000 eznet_keras-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.440410 eznet_keras-1.0.1/eznet_keras/
--rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-1.0.1/eznet_keras/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.454364 eznet_keras-1.0.1/eznet_keras/keras2cpp/
--rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/__init__.py
--rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/create_unit_tests.py
--rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/keras2cpp.py
--rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/python_model.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.468226 eznet_keras-1.0.1/eznet_keras/models/
--rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-1.0.1/eznet_keras/models/__init__.py
--rw-rw-rw-   0        0        0    17915 2023-07-15 17:25:36.000000 eznet_keras-1.0.1/eznet_keras/models/ann.py
--rw-rw-rw-   0        0        0    26308 2023-07-14 09:38:07.000000 eznet_keras-1.0.1/eznet_keras/models/conv_block.py
--rw-rw-rw-   0        0        0    31608 2023-07-16 11:44:21.000000 eznet_keras-1.0.1/eznet_keras/models/conv_network.py
--rw-rw-rw-   0        0        0    11975 2023-07-14 12:26:34.000000 eznet_keras-1.0.1/eznet_keras/models/dense_block.py
--rw-rw-rw-   0        0        0    11960 2023-07-15 17:49:42.000000 eznet_keras-1.0.1/eznet_keras/models/keras_smart_module.py
--rw-rw-rw-   0        0        0    25219 2023-07-15 17:23:22.000000 eznet_keras-1.0.1/eznet_keras/models/recurrent_network.py
--rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-1.0.1/eznet_keras/models/var_ae.py
--rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-1.0.1/eznet_keras/test.py
--rw-rw-rw-   0        0        0    13856 2023-07-15 13:47:05.000000 eznet_keras-1.0.1/eznet_keras/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.453368 eznet_keras-1.0.1/eznet_keras.egg-info/
--rw-rw-rw-   0        0        0    14243 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-16 11:46:36.470226 eznet_keras-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1823 2023-07-16 11:45:31.000000 eznet_keras-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.441559 eznet_keras-1.0.2/
+-rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    14243 2023-07-16 12:29:35.442556 eznet_keras-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13171 2023-07-16 12:07:46.000000 eznet_keras-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.421105 eznet_keras-1.0.2/eznet_keras/
+-rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-1.0.2/eznet_keras/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.437572 eznet_keras-1.0.2/eznet_keras/keras2cpp/
+-rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/__init__.py
+-rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/create_unit_tests.py
+-rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/keras2cpp.py
+-rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/python_model.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.441559 eznet_keras-1.0.2/eznet_keras/models/
+-rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-1.0.2/eznet_keras/models/__init__.py
+-rw-rw-rw-   0        0        0    17915 2023-07-15 17:25:36.000000 eznet_keras-1.0.2/eznet_keras/models/ann.py
+-rw-rw-rw-   0        0        0    26308 2023-07-14 09:38:07.000000 eznet_keras-1.0.2/eznet_keras/models/conv_block.py
+-rw-rw-rw-   0        0        0    31709 2023-07-16 12:07:25.000000 eznet_keras-1.0.2/eznet_keras/models/conv_network.py
+-rw-rw-rw-   0        0        0    11975 2023-07-14 12:26:34.000000 eznet_keras-1.0.2/eznet_keras/models/dense_block.py
+-rw-rw-rw-   0        0        0    11960 2023-07-15 17:49:42.000000 eznet_keras-1.0.2/eznet_keras/models/keras_smart_module.py
+-rw-rw-rw-   0        0        0    25219 2023-07-15 17:23:22.000000 eznet_keras-1.0.2/eznet_keras/models/recurrent_network.py
+-rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-1.0.2/eznet_keras/models/var_ae.py
+-rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-1.0.2/eznet_keras/test.py
+-rw-rw-rw-   0        0        0    13856 2023-07-15 13:47:05.000000 eznet_keras-1.0.2/eznet_keras/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.435578 eznet_keras-1.0.2/eznet_keras.egg-info/
+-rw-rw-rw-   0        0        0    14243 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-16 12:29:35.443552 eznet_keras-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2023-07-16 12:07:54.000000 eznet_keras-1.0.2/setup.py
```

### Comparing `eznet_keras-1.0.1/LICENSE.txt` & `eznet_keras-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/PKG-INFO` & `eznet_keras-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eznet_keras
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_keras
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: tensorflow,keras,deep learning,neural network,keras2cpp
 Classifier: Development Status :: 3 - Alpha
@@ -25,15 +25,15 @@
 
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 1.0.1  
+Version: 1.0.2  
 Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.1/README.md` & `eznet_keras-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 1.0.1  
+Version: 1.0.2  
 Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.1/eznet_keras/keras2cpp/create_unit_tests.py` & `eznet_keras-1.0.2/eznet_keras/keras2cpp/create_unit_tests.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/keras2cpp/keras2cpp.py` & `eznet_keras-1.0.2/eznet_keras/keras2cpp/keras2cpp.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/keras2cpp/python_model.py` & `eznet_keras-1.0.2/eznet_keras/keras2cpp/python_model.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/models/ann.py` & `eznet_keras-1.0.2/eznet_keras/models/ann.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/models/conv_block.py` & `eznet_keras-1.0.2/eznet_keras/models/conv_block.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/models/conv_network.py` & `eznet_keras-1.0.2/eznet_keras/models/conv_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,17 @@
         "conv_spatial_dropout": None,
         "pool_type": "Max",
         "pool_kernel_size": 2,
         "pool_padding": 'valid',
         "pool_stride": 1,
         "pool_params": None,
         "min_image_size": 4,
-        "flatten_before_dense": True,
+        "flatten_after_conv": True,
         # Fully connected blocks
+        "include_dense_layers": True,
         "dense_width": "auto",
         "dense_depth": 2,
         "dense_activation": "relu",
         "dense_activation_params": None,
         "dense_norm_layer_type": "BatchNormalization",
         "dense_norm_layer_position": "before",
         "dense_norm_layer_params": None,
@@ -298,27 +299,31 @@
             d = add_conv_block(**_kwargs)
             self.net = d['model']
             output_image = d['output_image']
             self.size_list.append(output_image+[out_channels])
             # in_channels = out_channels
             input_image = output_image
             
-        # Flattening (Image embedding)
+        # Including Dense or Output layers
         self._dense_depth = hparams.get("dense_depth")
-        self._flatten_before_dense = hparams["flatten_before_dense"] if "flatten_before_dense" in hparams else \
+        self._include_dense_layers = hparams["include_dense_layers"] if "include_dense_layers" in hparams else \
             (self._dense_depth is not None and self._dense_depth > 0)
-        if self._flatten_before_dense:
+        self._include_output_layer = hparams["include_output_layer"] if "include_output_layer" in hparams else True
+        
+        # Flattening
+        self._flatten_after_conv = hparams["flatten_after_conv"] if "flatten_after_conv" in hparams else (len(self._output_shape)==1)
+        if self._flatten_after_conv:
             self.net.add(tf.keras.layers.Flatten())
             self._dense_input_size = np.prod(output_image) * out_channels
         else:
             self._dense_input_size = out_channels
         self.size_list.append([self._dense_input_size])
         
-        # Check to see if we will have dense layers
-        if self._dense_depth is not None and self._dense_depth > 0:
+        # Construct dense layers
+        if self._include_dense_layers:
             
             # Dense layers hyperparameters
             self._dense_width = hparams.get("dense_width")
             self._dense_activation = hparams.get("dense_activation")
             self._dense_activation_params = hparams.get("dense_activation_params")
             self._dense_norm_layer_type = hparams.get("dense_norm_layer_type")
             self._dense_norm_layer_params = hparams.get("dense_norm_layer_params")
@@ -351,19 +356,15 @@
                         'dropout': self._dense_dropout_vec[i],
                         'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)
                     }
                     add_dense_block(**_kwargs)
                     # in_size = out_size
                     self.size_list.append([out_size])
         
-        
-        
-        # Check to see if there will be an output layer
-        self._include_output_layer = hparams.get("include_output_layer") if "include_output_layer" in hparams else True
-        
+        # Construct output layer
         if self._include_output_layer:
             # Output hyperparameters
             self._output_activation = hparams.get("output_activation")
             self._output_activation_params = hparams.get("output_activation_params")
         
             # Output layer
             self.net.add(tf.keras.layers.Dense(self._output_shape[-1], kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)))
```

### Comparing `eznet_keras-1.0.1/eznet_keras/models/dense_block.py` & `eznet_keras-1.0.2/eznet_keras/models/dense_block.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/models/keras_smart_module.py` & `eznet_keras-1.0.2/eznet_keras/models/keras_smart_module.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/models/recurrent_network.py` & `eznet_keras-1.0.2/eznet_keras/models/recurrent_network.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/models/var_ae.py` & `eznet_keras-1.0.2/eznet_keras/models/var_ae.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/test.py` & `eznet_keras-1.0.2/eznet_keras/test.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras/utils.py` & `eznet_keras-1.0.2/eznet_keras/utils.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/eznet_keras.egg-info/PKG-INFO` & `eznet_keras-1.0.2/eznet_keras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eznet-keras
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_keras
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: tensorflow,keras,deep learning,neural network,keras2cpp
 Classifier: Development Status :: 3 - Alpha
@@ -25,15 +25,15 @@
 
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 1.0.1  
+Version: 1.0.2  
 Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.1/eznet_keras.egg-info/SOURCES.txt` & `eznet_keras-1.0.2/eznet_keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.1/setup.py` & `eznet_keras-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = '1.0.1' 
+VERSION = '1.0.2' 
 DESCRIPTION = "Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc."
 
 # Setting up
 setup(
         # the name must match the folder name
         name="eznet_keras", 
         version=VERSION,
```

