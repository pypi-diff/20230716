# Comparing `tmp/eznet_keras-1.0.0.tar.gz` & `tmp/eznet_keras-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eznet_keras-1.0.0.tar", last modified: Sat Jul 15 17:58:53 2023, max compression
+gzip compressed data, was "eznet_keras-1.0.1.tar", last modified: Sun Jul 16 11:46:36 2023, max compression
```

## Comparing `eznet_keras-1.0.0.tar` & `eznet_keras-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.317383 eznet_keras-1.0.0/
--rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0    14243 2023-07-15 17:58:53.317383 eznet_keras-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13171 2023-07-15 17:55:34.000000 eznet_keras-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.300040 eznet_keras-1.0.0/eznet_keras/
--rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-1.0.0/eznet_keras/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.312382 eznet_keras-1.0.0/eznet_keras/keras2cpp/
--rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/__init__.py
--rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/create_unit_tests.py
--rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/keras2cpp.py
--rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/python_model.py
-drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.316370 eznet_keras-1.0.0/eznet_keras/models/
--rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-1.0.0/eznet_keras/models/__init__.py
--rw-rw-rw-   0        0        0    17915 2023-07-15 17:25:36.000000 eznet_keras-1.0.0/eznet_keras/models/ann.py
--rw-rw-rw-   0        0        0    26308 2023-07-14 09:38:07.000000 eznet_keras-1.0.0/eznet_keras/models/conv_block.py
--rw-rw-rw-   0        0        0    31561 2023-07-15 17:26:46.000000 eznet_keras-1.0.0/eznet_keras/models/conv_network.py
--rw-rw-rw-   0        0        0    11975 2023-07-14 12:26:34.000000 eznet_keras-1.0.0/eznet_keras/models/dense_block.py
--rw-rw-rw-   0        0        0    11960 2023-07-15 17:49:42.000000 eznet_keras-1.0.0/eznet_keras/models/keras_smart_module.py
--rw-rw-rw-   0        0        0    25219 2023-07-15 17:23:22.000000 eznet_keras-1.0.0/eznet_keras/models/recurrent_network.py
--rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-1.0.0/eznet_keras/models/var_ae.py
--rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-1.0.0/eznet_keras/test.py
--rw-rw-rw-   0        0        0    13856 2023-07-15 13:47:05.000000 eznet_keras-1.0.0/eznet_keras/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.310390 eznet_keras-1.0.0/eznet_keras.egg-info/
--rw-rw-rw-   0        0        0    14243 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-15 17:58:53.321459 eznet_keras-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1823 2023-07-15 17:56:31.000000 eznet_keras-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.469225 eznet_keras-1.0.1/
+-rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    14243 2023-07-16 11:46:36.469225 eznet_keras-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13171 2023-07-16 11:45:27.000000 eznet_keras-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.440410 eznet_keras-1.0.1/eznet_keras/
+-rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-1.0.1/eznet_keras/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.454364 eznet_keras-1.0.1/eznet_keras/keras2cpp/
+-rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/__init__.py
+-rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/create_unit_tests.py
+-rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/keras2cpp.py
+-rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-1.0.1/eznet_keras/keras2cpp/python_model.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.468226 eznet_keras-1.0.1/eznet_keras/models/
+-rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-1.0.1/eznet_keras/models/__init__.py
+-rw-rw-rw-   0        0        0    17915 2023-07-15 17:25:36.000000 eznet_keras-1.0.1/eznet_keras/models/ann.py
+-rw-rw-rw-   0        0        0    26308 2023-07-14 09:38:07.000000 eznet_keras-1.0.1/eznet_keras/models/conv_block.py
+-rw-rw-rw-   0        0        0    31608 2023-07-16 11:44:21.000000 eznet_keras-1.0.1/eznet_keras/models/conv_network.py
+-rw-rw-rw-   0        0        0    11975 2023-07-14 12:26:34.000000 eznet_keras-1.0.1/eznet_keras/models/dense_block.py
+-rw-rw-rw-   0        0        0    11960 2023-07-15 17:49:42.000000 eznet_keras-1.0.1/eznet_keras/models/keras_smart_module.py
+-rw-rw-rw-   0        0        0    25219 2023-07-15 17:23:22.000000 eznet_keras-1.0.1/eznet_keras/models/recurrent_network.py
+-rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-1.0.1/eznet_keras/models/var_ae.py
+-rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-1.0.1/eznet_keras/test.py
+-rw-rw-rw-   0        0        0    13856 2023-07-15 13:47:05.000000 eznet_keras-1.0.1/eznet_keras/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:46:36.453368 eznet_keras-1.0.1/eznet_keras.egg-info/
+-rw-rw-rw-   0        0        0    14243 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 11:46:36.000000 eznet_keras-1.0.1/eznet_keras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-16 11:46:36.470226 eznet_keras-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2023-07-16 11:45:31.000000 eznet_keras-1.0.1/setup.py
```

### Comparing `eznet_keras-1.0.0/LICENSE.txt` & `eznet_keras-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/PKG-INFO` & `eznet_keras-1.0.1/eznet_keras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eznet_keras
-Version: 1.0.0
+Name: eznet-keras
+Version: 1.0.1
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
-Version: 1.0.0  
+Version: 1.0.1  
 Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.0/README.md` & `eznet_keras-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 1.0.0  
+Version: 1.0.1  
 Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.0/eznet_keras/keras2cpp/create_unit_tests.py` & `eznet_keras-1.0.1/eznet_keras/keras2cpp/create_unit_tests.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/keras2cpp/keras2cpp.py` & `eznet_keras-1.0.1/eznet_keras/keras2cpp/keras2cpp.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/keras2cpp/python_model.py` & `eznet_keras-1.0.1/eznet_keras/keras2cpp/python_model.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/models/ann.py` & `eznet_keras-1.0.1/eznet_keras/models/ann.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/models/conv_block.py` & `eznet_keras-1.0.1/eznet_keras/models/conv_block.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/models/conv_network.py` & `eznet_keras-1.0.1/eznet_keras/models/conv_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,15 @@
                     add_dense_block(**_kwargs)
                     # in_size = out_size
                     self.size_list.append([out_size])
         
         
         
         # Check to see if there will be an output layer
-        self._include_output_layer = hparams.get("include_output_layer")
+        self._include_output_layer = hparams.get("include_output_layer") if "include_output_layer" in hparams else True
         
         if self._include_output_layer:
             # Output hyperparameters
             self._output_activation = hparams.get("output_activation")
             self._output_activation_params = hparams.get("output_activation_params")
         
             # Output layer
```

### Comparing `eznet_keras-1.0.0/eznet_keras/models/dense_block.py` & `eznet_keras-1.0.1/eznet_keras/models/dense_block.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/models/keras_smart_module.py` & `eznet_keras-1.0.1/eznet_keras/models/keras_smart_module.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/models/recurrent_network.py` & `eznet_keras-1.0.1/eznet_keras/models/recurrent_network.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/models/var_ae.py` & `eznet_keras-1.0.1/eznet_keras/models/var_ae.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/test.py` & `eznet_keras-1.0.1/eznet_keras/test.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras/utils.py` & `eznet_keras-1.0.1/eznet_keras/utils.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/eznet_keras.egg-info/PKG-INFO` & `eznet_keras-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eznet-keras
-Version: 1.0.0
+Name: eznet_keras
+Version: 1.0.1
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
-Version: 1.0.0  
+Version: 1.0.1  
 Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.0/eznet_keras.egg-info/SOURCES.txt` & `eznet_keras-1.0.1/eznet_keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.0/setup.py` & `eznet_keras-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = '1.0.0' 
+VERSION = '1.0.1' 
 DESCRIPTION = "Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc."
 
 # Setting up
 setup(
         # the name must match the folder name
         name="eznet_keras", 
         version=VERSION,
```

