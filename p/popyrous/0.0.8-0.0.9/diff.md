# Comparing `tmp/popyrous-0.0.8.tar.gz` & `tmp/popyrous-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popyrous-0.0.8.tar", last modified: Sat Jul 15 18:30:03 2023, max compression
+gzip compressed data, was "popyrous-0.0.9.tar", last modified: Sun Jul 16 09:36:32 2023, max compression
```

## Comparing `popyrous-0.0.8.tar` & `popyrous-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.386049 popyrous-0.0.8/
--rw-rw-rw-   0        0        0     1072 2023-01-20 07:48:00.000000 popyrous-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     9279 2023-07-15 18:30:03.387223 popyrous-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8532 2023-07-15 18:28:58.000000 popyrous-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.368582 popyrous-0.0.8/popyrous/
--rw-rw-rw-   0        0        0      304 2023-01-21 19:46:08.000000 popyrous-0.0.8/popyrous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.378077 popyrous-0.0.8/popyrous/matlab/
--rw-rw-rw-   0        0        0       22 2023-01-19 13:24:02.000000 popyrous-0.0.8/popyrous/matlab/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-01-19 13:24:24.000000 popyrous-0.0.8/popyrous/matlab/matlab.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.379073 popyrous-0.0.8/popyrous/ml/
--rw-rw-rw-   0        0        0       15 2023-01-21 13:53:00.000000 popyrous-0.0.8/popyrous/ml/__init__.py
--rw-rw-rw-   0        0        0     4333 2023-01-21 13:54:45.000000 popyrous-0.0.8/popyrous/ml/confusion_matrix.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.380069 popyrous-0.0.8/popyrous/packages/
--rw-rw-rw-   0        0        0       47 2023-01-19 11:52:33.000000 popyrous-0.0.8/popyrous/packages/__init__.py
--rw-rw-rw-   0        0        0     6288 2023-01-19 11:55:04.000000 popyrous-0.0.8/popyrous/packages/packages.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.384057 popyrous-0.0.8/popyrous/timeseries/
--rw-rw-rw-   0        0        0      185 2023-01-20 20:11:43.000000 popyrous-0.0.8/popyrous/timeseries/__init__.py
--rw-rw-rw-   0        0        0     7172 2023-01-21 12:14:16.000000 popyrous-0.0.8/popyrous/timeseries/cwt.py
--rw-rw-rw-   0        0        0    21072 2023-01-21 19:43:36.000000 popyrous-0.0.8/popyrous/timeseries/datasets.py
--rw-rw-rw-   0        0        0    74704 2023-05-01 19:23:41.000000 popyrous-0.0.8/popyrous/timeseries/experiment.py
--rw-rw-rw-   0        0        0     1781 2023-01-19 13:48:53.000000 popyrous-0.0.8/popyrous/timeseries/filt.py
--rw-rw-rw-   0        0        0     2686 2023-01-19 16:08:55.000000 popyrous-0.0.8/popyrous/timeseries/metrics.py
--rw-rw-rw-   0        0        0     1862 2022-08-06 15:20:20.000000 popyrous-0.0.8/popyrous/timeseries/recipe_577504_1.py
--rw-rw-rw-   0        0        0     4342 2023-01-19 13:33:36.000000 popyrous-0.0.8/popyrous/timeseries/sliding_window.py
--rw-rw-rw-   0        0        0      459 2023-01-19 16:12:28.000000 popyrous-0.0.8/popyrous/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.385053 popyrous-0.0.8/popyrous/web/
--rw-rw-rw-   0        0        0       24 2023-01-19 12:24:39.000000 popyrous-0.0.8/popyrous/web/__init__.py
--rw-rw-rw-   0        0        0     8751 2023-01-19 13:10:54.000000 popyrous-0.0.8/popyrous/web/download.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.386049 popyrous-0.0.8/popyrous/zipfiles/
--rw-rw-rw-   0        0        0       24 2023-01-19 13:21:58.000000 popyrous-0.0.8/popyrous/zipfiles/__init__.py
--rw-rw-rw-   0        0        0     1791 2023-01-19 13:28:12.000000 popyrous-0.0.8/popyrous/zipfiles/zipfiles.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.377062 popyrous-0.0.8/popyrous.egg-info/
--rw-rw-rw-   0        0        0     9279 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      779 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-15 18:30:03.391404 popyrous-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-07-15 18:29:18.000000 popyrous-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.902601 popyrous-0.0.9/
+-rw-rw-rw-   0        0        0     1072 2023-01-20 07:48:00.000000 popyrous-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     9313 2023-07-16 09:36:32.902601 popyrous-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8566 2023-07-16 09:34:11.000000 popyrous-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.880672 popyrous-0.0.9/popyrous/
+-rw-rw-rw-   0        0        0      304 2023-01-21 19:46:08.000000 popyrous-0.0.9/popyrous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.893630 popyrous-0.0.9/popyrous/matlab/
+-rw-rw-rw-   0        0        0       22 2023-01-19 13:24:02.000000 popyrous-0.0.9/popyrous/matlab/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-01-19 13:24:24.000000 popyrous-0.0.9/popyrous/matlab/matlab.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.894626 popyrous-0.0.9/popyrous/ml/
+-rw-rw-rw-   0        0        0       15 2023-01-21 13:53:00.000000 popyrous-0.0.9/popyrous/ml/__init__.py
+-rw-rw-rw-   0        0        0     4333 2023-01-21 13:54:45.000000 popyrous-0.0.9/popyrous/ml/confusion_matrix.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.895623 popyrous-0.0.9/popyrous/packages/
+-rw-rw-rw-   0        0        0       47 2023-01-19 11:52:33.000000 popyrous-0.0.9/popyrous/packages/__init__.py
+-rw-rw-rw-   0        0        0     6288 2023-01-19 11:55:04.000000 popyrous-0.0.9/popyrous/packages/packages.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.899610 popyrous-0.0.9/popyrous/timeseries/
+-rw-rw-rw-   0        0        0      185 2023-01-20 20:11:43.000000 popyrous-0.0.9/popyrous/timeseries/__init__.py
+-rw-rw-rw-   0        0        0     7172 2023-01-21 12:14:16.000000 popyrous-0.0.9/popyrous/timeseries/cwt.py
+-rw-rw-rw-   0        0        0    28730 2023-07-16 09:30:33.000000 popyrous-0.0.9/popyrous/timeseries/datasets.py
+-rw-rw-rw-   0        0        0    79873 2023-07-16 09:24:27.000000 popyrous-0.0.9/popyrous/timeseries/experiment.py
+-rw-rw-rw-   0        0        0     1781 2023-01-19 13:48:53.000000 popyrous-0.0.9/popyrous/timeseries/filt.py
+-rw-rw-rw-   0        0        0     2686 2023-01-19 16:08:55.000000 popyrous-0.0.9/popyrous/timeseries/metrics.py
+-rw-rw-rw-   0        0        0     1862 2022-08-06 15:20:20.000000 popyrous-0.0.9/popyrous/timeseries/recipe_577504_1.py
+-rw-rw-rw-   0        0        0     4342 2023-01-19 13:33:36.000000 popyrous-0.0.9/popyrous/timeseries/sliding_window.py
+-rw-rw-rw-   0        0        0      459 2023-01-19 16:12:28.000000 popyrous-0.0.9/popyrous/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.900607 popyrous-0.0.9/popyrous/web/
+-rw-rw-rw-   0        0        0       24 2023-01-19 12:24:39.000000 popyrous-0.0.9/popyrous/web/__init__.py
+-rw-rw-rw-   0        0        0     8751 2023-01-19 13:10:54.000000 popyrous-0.0.9/popyrous/web/download.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.902601 popyrous-0.0.9/popyrous/zipfiles/
+-rw-rw-rw-   0        0        0       24 2023-01-19 13:21:58.000000 popyrous-0.0.9/popyrous/zipfiles/__init__.py
+-rw-rw-rw-   0        0        0     1791 2023-01-19 13:28:12.000000 popyrous-0.0.9/popyrous/zipfiles/zipfiles.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:36:32.892638 popyrous-0.0.9/popyrous.egg-info/
+-rw-rw-rw-   0        0        0     9313 2023-07-16 09:36:32.000000 popyrous-0.0.9/popyrous.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      779 2023-07-16 09:36:32.000000 popyrous-0.0.9/popyrous.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 09:36:32.000000 popyrous-0.0.9/popyrous.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-16 09:36:32.000000 popyrous-0.0.9/popyrous.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 09:36:32.000000 popyrous-0.0.9/popyrous.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-16 09:36:32.903596 popyrous-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-07-16 09:33:22.000000 popyrous-0.0.9/setup.py
```

### Comparing `popyrous-0.0.8/LICENSE.txt` & `popyrous-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/PKG-INFO` & `popyrous-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popyrous
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pouya's Python routines. A collection of useful Python routines for everyday and professional life.
 Home-page: https://github.com/pniaz20/popyrous
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: python,routines,matlab,zipfile,packages,time series,filtering,download,web
 Classifier: Development Status :: 3 - Alpha
@@ -15,19 +15,19 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Popyrous
 
-(Pouya's Python Routines) A collection of useful Python routines for science, research, development, and everyday life.
+(Pouya's Python Routines) A collection of useful and frequently encountered Python routines for (data) science, research, development, and everyday life.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.8  
-Last Update: July 15, 2023
+Version: 0.0.9  
+Last Update: July 16, 2023
 
 This is a collection of Python routines for the following purposes:
 
 - Checking for packages and installing missing ones iwithin scripts without the need for Jupyter and symbols like "!" and "%".
 - Reading and writing `.mat` files coming to/from MathWorks MATLAB software.
 - Building and manipulating time series data using sliding windows, low-pass filtering, etc.
 - Building flexible and easy-to-use datasets for data analysis or machine learning out of structured time series experiments (multiple subjects, conditions, repetitions, etc.).
```

### Comparing `popyrous-0.0.8/README.md` & `popyrous-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Popyrous
 
-(Pouya's Python Routines) A collection of useful Python routines for science, research, development, and everyday life.
+(Pouya's Python Routines) A collection of useful and frequently encountered Python routines for (data) science, research, development, and everyday life.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.8  
-Last Update: July 15, 2023
+Version: 0.0.9  
+Last Update: July 16, 2023
 
 This is a collection of Python routines for the following purposes:
 
 - Checking for packages and installing missing ones iwithin scripts without the need for Jupyter and symbols like "!" and "%".
 - Reading and writing `.mat` files coming to/from MathWorks MATLAB software.
 - Building and manipulating time series data using sliding windows, low-pass filtering, etc.
 - Building flexible and easy-to-use datasets for data analysis or machine learning out of structured time series experiments (multiple subjects, conditions, repetitions, etc.).
```

### Comparing `popyrous-0.0.8/popyrous/matlab/matlab.py` & `popyrous-0.0.9/popyrous/matlab/matlab.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/ml/confusion_matrix.py` & `popyrous-0.0.9/popyrous/ml/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/packages/packages.py` & `popyrous-0.0.9/popyrous/packages/packages.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/timeseries/cwt.py` & `popyrous-0.0.9/popyrous/timeseries/cwt.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/timeseries/experiment.py` & `popyrous-0.0.9/popyrous/timeseries/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,47 +61,56 @@
                 'trainset' or 'testset'. If it is a float, it will by default come from test set, if any.
                 If there is no test set applicable according to the settings, training set will be used.
                 If this is a tuple, it should be e.g. [0.2, 'trainset'] or [0.1,'testset'].
             
             
             ** Description of data downsampling and sequence downsampling **
             
-            Data downsampling downsamples the existing datapoints before generating any sliding window or sequences or anything.
-            It therefore decreases the size of the training set.
-            
-            If a specific sequence length is required in units of time for meaningful extraction of features, but the sampling frequency
-            is extremely large, then the generated sequences will be too large to fit in memory. This is where sequence downsampling comes in.
-            
-            Sequence downsampling simply downsamples the sequences in every data point, so number of training samples is unaffected,
-            the true time length of the sequences are also unaffected, but the sequences themselves are downsampled, so they have
-            fewer time steps in them. Therefore, the number of time steps are fewer, less memory is occupied, but training set size and
-            the true time length of the sequences are preserved.
-                
-            Note that data downsampling decreases dataset size AND makes sequences more coarsely sampled without
-            changing the true time length of the sequence. Sequence downsampling, on the other hand, does not touch
-            dataset size. It only downsamples the sequences that are already generated from the sliding window.
+            The data downsampling rate downsamples the data when extracting it, so dataset size (number of samples) is divided by the downsampling rate.
+            After the time series is downsampled by the `data_downsampling`, sequences are extracted from it using a sliding window. After the sequences are extracted, they can 
+            still have too many time steps in them especially if the sampling rate was high to begin with. Then, the `sequence_downsampling` is applied, and all the extracted 
+            sequences are downsampled. This does not change the dataset size; it only decreases the number of time steps in each sequence.
+            
+            Data downsampling is typically used when the sampling frequency is too high and there are too many time series or the series are too long. Sequence downsampling is 
+            typically used when the sequence length (in units of time) needs to remain large enough to extract meaningful trends and information, but because the sampling 
+            frequency is too high the sequences end up having too many time steps. Sequence downsampling makes sure the time-length of the sequences remains constant while the 
+            number of time steps in each sequence is reduced.
+            
+            For example, let us assume 100 trials of a time-series experiment were performed, each lasting 100 seconds, with a sampling frequency of 1000 Hz. This means there are 
+            a total of 100 K timesteps in each trial, amounting to 10 M time steps (training samples) in total. Let us assume that the sequences that you extract with a sliding 
+            window need to be at least 2 seconds long to be able to extract meaningful information from them. There are two problems here. Firstly, there are too many data points 
+            (10 M) in the training set. Secondly, the sequences will have too many time steps in them (2000) which will make training difficult and memory-intensive. To solve this 
+            problem, we apply a `data_downsampling` rate of 4, reducing the effective sampling frequency to 250 Hz. This reduces the number of data points to 2.5 M.
+            Also, this will mean that our 2-second sequences will have 500 time steps in them. Right now, 2.5 M dataset size is good, and we do not want to reduce it further. 
+            However, especially if the data is smooth enough, 500 time steps in a sequence may be still too high. If we increase the `data_downsampling` rate, dataset size will 
+            also decrease, and we do not want that. Therefore, we simply apply a `sequence_downsampling` rate of 10, which will reduce the number of time steps in each sequence to
+            50, without touching the dataset size, affecting the rate of extracting sequences from the time series, or affecting the time length of the extracted sequences. 
+            Assuming that the data is smooth and 50 timesteps forming a 2-second sequence are enough to extract meaningful information from the data, this is a good solution. 
+            We will eventually have 2.5 M sequences with 50 time steps in each.
             
             Therefore, if the size and/or sampling frequency of the data is too high, data downsampling is preferred.
             However, if the dataset size is fine, but due to the long sequence length or high sampling rate, sequences
             hold too many data points in them and matrices end up being too large for the memory, sequence downsampling 
             is preferred. Sequence downsampling will not touch the size/sampling frequency of the data itself, 
             nor will it touch the true time length of the sequences. It will only make the sequences downsampled 
             and more coarse. Therefore, number of data points in the dataset will remain constant, as will the true 
-            time length of the sequences. However, the number of data points in the sequences will decrease.
+            time length of the sequences. However, the number of time steps in the sequences will decrease.
             
             **IMPORTANT** 
             
             Depending on whether squeezed or unsqueezed data is required (see below), the passed hyperparameter 
             dictionary will be updated as follows:
             
              - If `data_squeezed` is True: The `input_size` and `output_size` hyperparameters will be updated as well as `in_seq_len` and `out_seq_len`.
             This is useful when, e.g., the data will be sent to an ANN that uses 2D tensors as inputs.
             
              - If `data_squeezed` is False: The `in_seq_len` and `out_seq_len` hyperparameters will be updated.
-            This is useful when RNN-based or CNN-based models will be deployed, where inputs are 3D.
+            This is useful when RNN-based or CNN-based models will be deployed, where inputs are 3D. In this case, at the end, `out_features` key will also be updated and
+            multiplied by the `out_seq_len` to get the final output layer width. Thsi is because this class assumes that regardless of input shapes, outputs are always
+            squeezed to 2D tensors. Therefore,  the final output layer width will be `out_features *= out_seq_len`.
             
             ** NOTE ** that in the case of unsqueezed data, the 3D tensors coming from the sliding windows will be of shape 
             (batch size, sequence length, features/channels) which is OK with Keras, but not OK with PyTorch, for instance.
             
             The rest of the arguments of this class are as follows:
                 
             - `subjects_column` (str, optional): Column of the DataFrame holding subject numbers, if any. Defaults to None.
@@ -435,29 +444,29 @@
                     
                     # GENERATE DATASET OBJECT
                     if self.data_squeezed:
                         dataset, self.hparams = make_squeezed_dataset(self.hparams, data_features, y, verbose=False, **kwargs)
                     else:
                         dataset, self.hparams = make_unsqueezed_dataset(self.hparams, data_features, y, verbose=False, **kwargs)
                     
-                    # Get input and output trables   
+                    # Get input and output tables   
                     x_processed = dataset.table_in
                     y_processed = dataset.table_out
                     if verbosity == 2:
                         print("; x: ",x_processed.shape, end="")
                         print(", y: ",y_processed.shape, end="")
                     
                     # POSTPROCESSING
                     if self.input_postprocessor:
                         x_processed = self.input_postprocessor(x_processed)
                     if self.output_postprocessor:
                         y_processed = self.output_postprocessor(y_processed)
                     if verbosity == 2:
-                        print("; x: ",x_processed.shape, end="")
-                        print(", y: ",y_processed.shape, end="")
+                        print("; (post) x: ",x_processed.shape, end="")
+                        print(", (post) y: ",y_processed.shape, end="")
                     
                     # Construct data arrays    
                     if self.return_train_val_test_arrays:
                         x_arrays[subj, ctrl, trial] = x_processed
                         y_arrays[subj, ctrl, trial] = y_processed
                     else:
                         x_arrays[subj, ctrl, trial] = []
@@ -675,41 +684,61 @@
                 These datapoints will be selected randomly out of all the data. The data will be shuffled.
                 If this is a tuple, it should hold the portion, followed by which set it comes from, 
                 'trainset' or 'testset'. If it is a float, it will by default come from test set, if any.
                 If there is no test set applicable according to the settings, training set will be used.
                 If this is a tuple, it should be e.g. [0.2, 'trainset'] or [0.1,'testset'].
             
              
-            ** Description of data downsampling and sequence downsam,pling **
+            ** Description of data downsampling and sequence downsampling **
+            
+            The data downsampling rate downsamples the data when extracting it, so dataset size (number of samples) is divided by the downsampling rate.
+            After the time series is downsampled by the `data_downsampling`, sequences are extracted from it using a sliding window. After the sequences are extracted, they can 
+            still have too many time steps in them especially if the sampling rate was high to begin with. Then, the `sequence_downsampling` is applied, and all the extracted 
+            sequences are downsampled. This does not change the dataset size; it only decreases the number of time steps in each sequence.
+            
+            Data downsampling is typically used when the sampling frequency is too high and there are too many time series or the series are too long. Sequence downsampling is 
+            typically used when the sequence length (in units of time) needs to remain large enough to extract meaningful trends and information, but because the sampling 
+            frequency is too high the sequences end up having too many time steps. Sequence downsampling makes sure the time-length of the sequences remains constant while the 
+            number of time steps in each sequence is reduced.
+            
+            For example, let us assume 100 trials of a time-series experiment were performed, each lasting 100 seconds, with a sampling frequency of 1000 Hz. This means there are 
+            a total of 100 K timesteps in each trial, amounting to 10 M time steps (training samples) in total. Let us assume that the sequences that you extract with a sliding 
+            window need to be at least 2 seconds long to be able to extract meaningful information from them. There are two problems here. Firstly, there are too many data points 
+            (10 M) in the training set. Secondly, the sequences will have too many time steps in them (2000) which will make training difficult and memory-intensive. To solve this 
+            problem, we apply a `data_downsampling` rate of 4, reducing the effective sampling frequency to 250 Hz. This reduces the number of data points to 2.5 M.
+            Also, this will mean that our 2-second sequences will have 500 time steps in them. Right now, 2.5 M dataset size is good, and we do not want to reduce it further. 
+            However, especially if the data is smooth enough, 500 time steps in a sequence may be still too high. If we increase the `data_downsampling` rate, dataset size will 
+            also decrease, and we do not want that. Therefore, we simply apply a `sequence_downsampling` rate of 10, which will reduce the number of time steps in each sequence to
+            50, without touching the dataset size, affecting the rate of extracting sequences from the time series, or affecting the time length of the extracted sequences. 
+            Assuming that the data is smooth and 50 timesteps forming a 2-second sequence are enough to extract meaningful information from the data, this is a good solution. 
+            We will eventually have 2.5 M sequences with 50 time steps in each.
             
-            Note that data downsampling decreases dataset size AND makes sequences more coarsely sampled without
-            changing the true time length of the sequence. Sequence downsampling, on the other hand, does not touch
-            dataset size. It only downsamples the sequences that are already generated from the sliding window.
             Therefore, if the size and/or sampling frequency of the data is too high, data downsampling is preferred.
-            However, if the dataset size/sampling frequency is fine, but due to the high sequence length, sequences
-            hold too many data points in them and matrices end up being too large for the RAM, sequence downsampling 
+            However, if the dataset size is fine, but due to the long sequence length or high sampling rate, sequences
+            hold too many data points in them and matrices end up being too large for the memory, sequence downsampling 
             is preferred. Sequence downsampling will not touch the size/sampling frequency of the data itself, 
             nor will it touch the true time length of the sequences. It will only make the sequences downsampled 
             and more coarse. Therefore, number of data points in the dataset will remain constant, as will the true 
-            time length of the sequences. However, the number of data points in the sequences will decrease.
+            time length of the sequences. However, the number of time steps in the sequences will decrease.
             
             
             
             
             **IMPORTANT** 
             Depending on whether squeezed or unsqueezed data is required (see below), the passed hyperparameter 
             dictionary will be updated as follows:
             
              - If `data_squeezed` is True: The `input_size` and `output_size` hyperparameters will be updated.
-            This is useful when `Keras_ANN` or `Pytorch_ANN` or generally MLP models will be deployed,
+            This is useful when MLP models will be deployed,
             where inputs are 2D tables.
             
              - If `data_squeezed` is False: The `in_seq_len` and `out_seq_len` hyperparameters will be updated.
-            This is useful when `Keras_Seq2Dense` or `Pytorch_Seq2Dense` or generally RNN-based or CNN-based models
-            will be deployed, where inputs are 3D.
+            This is useful when generally RNN-based or CNN-based models
+            will be deployed, where inputs are 3D. In this case, the `out_features` key will also be multiplied by the `out_seq_len` to get the total number of output features.
+            This is because regardless of input shapes, outputs in this function are always assumed to be squeezed. `out_features` is the final output layer width.
             
             
         - `subjects_column` (str, optional): Column of the DataFrame holding subject numbers, if any. Defaults to None.
         - `conditions_column` (str, optional): Column of the DataFrame holding condition numbers. Defaults to None.
         - `trials_column` (str, optional): Column of the DataFrame holding trial numbers, if any. Defaults to None.
             **NOTE**: If any of the above arguments are None, it is assumed only one subject/condition/trial is
             involved in the timeseries experiments.
```

### Comparing `popyrous-0.0.8/popyrous/timeseries/filt.py` & `popyrous-0.0.9/popyrous/timeseries/filt.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/timeseries/metrics.py` & `popyrous-0.0.9/popyrous/timeseries/metrics.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/timeseries/recipe_577504_1.py` & `popyrous-0.0.9/popyrous/timeseries/recipe_577504_1.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/timeseries/sliding_window.py` & `popyrous-0.0.9/popyrous/timeseries/sliding_window.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/web/download.py` & `popyrous-0.0.9/popyrous/web/download.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous/zipfiles/zipfiles.py` & `popyrous-0.0.9/popyrous/zipfiles/zipfiles.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/popyrous.egg-info/PKG-INFO` & `popyrous-0.0.9/popyrous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popyrous
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pouya's Python routines. A collection of useful Python routines for everyday and professional life.
 Home-page: https://github.com/pniaz20/popyrous
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: python,routines,matlab,zipfile,packages,time series,filtering,download,web
 Classifier: Development Status :: 3 - Alpha
@@ -15,19 +15,19 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Popyrous
 
-(Pouya's Python Routines) A collection of useful Python routines for science, research, development, and everyday life.
+(Pouya's Python Routines) A collection of useful and frequently encountered Python routines for (data) science, research, development, and everyday life.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.8  
-Last Update: July 15, 2023
+Version: 0.0.9  
+Last Update: July 16, 2023
 
 This is a collection of Python routines for the following purposes:
 
 - Checking for packages and installing missing ones iwithin scripts without the need for Jupyter and symbols like "!" and "%".
 - Reading and writing `.mat` files coming to/from MathWorks MATLAB software.
 - Building and manipulating time series data using sliding windows, low-pass filtering, etc.
 - Building flexible and easy-to-use datasets for data analysis or machine learning out of structured time series experiments (multiple subjects, conditions, repetitions, etc.).
```

### Comparing `popyrous-0.0.8/popyrous.egg-info/SOURCES.txt` & `popyrous-0.0.9/popyrous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.8/setup.py` & `popyrous-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.0.8' 
+VERSION = '0.0.9' 
 DESCRIPTION = "Pouya's Python routines. A collection of useful Python routines for everyday and professional life."
 
 # Setting up
 setup(
        # the name must match the folder name
         name="popyrous", 
         version=VERSION,
```

