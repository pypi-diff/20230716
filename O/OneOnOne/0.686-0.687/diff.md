# Comparing `tmp/OneOnOne-0.686.tar.gz` & `tmp/OneOnOne-0.687.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.686.tar", last modified: Sat Jul 15 11:13:11 2023, max compression
+gzip compressed data, was "OneOnOne-0.687.tar", last modified: Sun Jul 16 10:49:06 2023, max compression
```

## Comparing `OneOnOne-0.686.tar` & `OneOnOne-0.687.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-15 11:13:11.879034 OneOnOne-0.686/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.686/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-15 11:13:11.874533 OneOnOne-0.686/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    35653 2023-07-15 11:12:22.000000 OneOnOne-0.686/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.686/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.686/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.686/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.686/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-15 11:13:11.877633 OneOnOne-0.686/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      114 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-15 11:13:11.878352 OneOnOne-0.686/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.686/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-15 11:13:11.879239 OneOnOne-0.686/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1909 2023-07-15 11:12:34.000000 OneOnOne-0.686/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-16 10:49:06.641290 OneOnOne-0.687/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.687/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-16 10:49:06.637849 OneOnOne-0.687/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    35736 2023-07-16 10:47:32.000000 OneOnOne-0.687/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.687/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.687/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.687/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.687/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-16 10:49:06.639896 OneOnOne-0.687/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-16 10:49:06.000000 OneOnOne-0.687/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-16 10:49:06.000000 OneOnOne-0.687/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-16 10:49:06.000000 OneOnOne-0.687/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      114 2023-07-16 10:49:06.000000 OneOnOne-0.687/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-16 10:49:06.000000 OneOnOne-0.687/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-16 10:49:06.640785 OneOnOne-0.687/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.687/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-16 10:49:06.641400 OneOnOne-0.687/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1909 2023-07-16 10:48:54.000000 OneOnOne-0.687/setup.py
```

### Comparing `OneOnOne-0.686/LICENSE` & `OneOnOne-0.687/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.686/OneOnOne/__init__.py` & `OneOnOne-0.687/OneOnOne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,22 @@
 from sklearn import preprocessing
 from sklearn.utils import shuffle
 
 from tqdm import keras
 import urllib.request
 import urllib
 import pkgutil
-# from urllib.request import urlretrieve
-# from urllib import urlretrieve
+import requests, zipfile
+from io import BytesIO
+from googleapiclient.discovery import build
+from google_auth_oauthlib.flow import InstalledAppFlow
+from google.auth.transport.requests import Request
+from googleapiclient.http import MediaIoBaseDownload, MediaFileUpload
+# from googledrivedownloader import GoogleDriveDownloader as gdd
+
 class PretrainedModel:
     def __init__(self, model_type="resnet50", dataset="cifar10", samplingtype="none"):
 
         self.model_type=model_type
         self.dataset=dataset
         self.samplingtype=samplingtype
 
@@ -50,21 +56,18 @@
             self.samplingtype="none"
 
         if self.samplingtype=="none" or self.samplingtype=="None":
             self.path=os.getcwd()+f'/models_to_load/{self.model_type}_{self.dataset}'
         else:
             self.path=os.getcwd()+f'/models_to_load/{self.model_type}_{self.dataset}_{self.samplingtype}'
 
-        self.model=urllib.request.urlretrieve('https://github.com/sohini-bhattacharya/OneOnOne/blob/master/saved_models/resnet50_cifar10_none.zip',f"{self.path}_none_webzip")
         self.model=load_model(self.path)
         self.model.summary()
 
 
-
-
 class Classification:
     def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
 
         self.model_type = model_type
         self.date=datetime.datetime.now()
         self.dataset=dataset
         self.shuffle_bool = shuffle
```

### Comparing `OneOnOne-0.686/OneOnOne/classes.py` & `OneOnOne-0.687/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.686/OneOnOne/classification.py` & `OneOnOne-0.687/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.686/OneOnOne/contextdecider.py` & `OneOnOne-0.687/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.686/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.687/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.686
+Version: 0.687
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.686/PKG-INFO` & `OneOnOne-0.687/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.686
+Version: 0.687
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.686/README.md` & `OneOnOne-0.687/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.686/setup.py` & `OneOnOne-0.687/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.686
+VERSION=0.687
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

