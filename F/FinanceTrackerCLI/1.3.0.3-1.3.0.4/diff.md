# Comparing `tmp/FinanceTrackerCLI-1.3.0.3.tar.gz` & `tmp/FinanceTrackerCLI-1.3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinanceTrackerCLI-1.3.0.3.tar", last modified: Sun Jul 16 17:53:18 2023, max compression
+gzip compressed data, was "FinanceTrackerCLI-1.3.0.4.tar", last modified: Sun Jul 16 17:55:04 2023, max compression
```

## Comparing `FinanceTrackerCLI-1.3.0.3.tar` & `FinanceTrackerCLI-1.3.0.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:53:18.808964 FinanceTrackerCLI-1.3.0.3/
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.3.0.3/LICENSE
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:53:18.808868 FinanceTrackerCLI-1.3.0.3/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      292 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.3/README.md
--rw-r--r--   0 vladkobranov   (501) staff       (20)      124 2023-07-16 16:47:26.000000 FinanceTrackerCLI-1.3.0.3/pyproject.toml
--rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-16 17:53:18.809001 FinanceTrackerCLI-1.3.0.3/setup.cfg
--rw-r--r--   0 vladkobranov   (501) staff       (20)      704 2023-07-16 17:53:14.000000 FinanceTrackerCLI-1.3.0.3/setup.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:53:18.806562 FinanceTrackerCLI-1.3.0.3/src/
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:53:18.807253 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      299 2023-07-16 17:41:57.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/__init__.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3710 2023-07-16 17:50:32.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/finance_tracker.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:53:18.808720 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      616 2023-07-16 17:52:50.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/__init__.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/grouped_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/input_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/local_convertor.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/search_by_month_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/show_all_delete_string.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/terminal_name.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     2536 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/text_prompts.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:53:18.807782 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:53:18.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      708 2023-07-16 17:53:18.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/SOURCES.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 17:53:18.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/dependency_links.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 17:53:18.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/requires.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 17:53:18.000000 FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/top_level.txt
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:55:04.742777 FinanceTrackerCLI-1.3.0.4/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.3.0.4/LICENSE
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:55:04.742679 FinanceTrackerCLI-1.3.0.4/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      292 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.4/README.md
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      124 2023-07-16 16:47:26.000000 FinanceTrackerCLI-1.3.0.4/pyproject.toml
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-16 17:55:04.742814 FinanceTrackerCLI-1.3.0.4/setup.cfg
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      704 2023-07-16 17:54:58.000000 FinanceTrackerCLI-1.3.0.4/setup.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:55:04.740484 FinanceTrackerCLI-1.3.0.4/src/
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:55:04.741082 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3710 2023-07-16 17:50:32.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/finance_tracker.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:55:04.742524 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      616 2023-07-16 17:52:50.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/__init__.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/grouped_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/input_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/local_convertor.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/search_by_month_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/show_all_delete_string.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/terminal_name.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     2536 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/text_prompts.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:55:04.741620 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:55:04.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      674 2023-07-16 17:55:04.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 17:55:04.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 17:55:04.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/requires.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 17:55:04.000000 FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/top_level.txt
```

### Comparing `FinanceTrackerCLI-1.3.0.3/LICENSE` & `FinanceTrackerCLI-1.3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/PKG-INFO` & `FinanceTrackerCLI-1.3.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinanceTrackerCLI
-Version: 1.3.0.3
+Version: 1.3.0.4
 Summary: Finance tracker CLI app
 Home-page: https://github.com/VladimirKobranov/FinanceTrackerCLI
 Author: Vladimir Kobranov
 Author-email: josephclturok@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `FinanceTrackerCLI-1.3.0.3/setup.py` & `FinanceTrackerCLI-1.3.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FinanceTrackerCLI',
-    version='1.3.0.3',
+    version='1.3.0.4',
     author='Vladimir Kobranov',
     author_email='josephclturok@gmail.com',
     description='Finance tracker CLI app',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VladimirKobranov/FinanceTrackerCLI',
     classifiers=[
```

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/finance_tracker.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/finance_tracker.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/__init__.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/grouped_data.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/grouped_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/input_data.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/input_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/local_convertor.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/local_convertor.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/search_by_month_data.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/search_by_month_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/show_all_delete_string.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/show_all_delete_string.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/terminal_name.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/terminal_name.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI/logic/text_prompts.py` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI/logic/text_prompts.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/PKG-INFO` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinanceTrackerCLI
-Version: 1.3.0.3
+Version: 1.3.0.4
 Summary: Finance tracker CLI app
 Home-page: https://github.com/VladimirKobranov/FinanceTrackerCLI
 Author: Vladimir Kobranov
 Author-email: josephclturok@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `FinanceTrackerCLI-1.3.0.3/src/FinanceTrackerCLI.egg-info/SOURCES.txt` & `FinanceTrackerCLI-1.3.0.4/src/FinanceTrackerCLI.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-src/FinanceTrackerCLI/__init__.py
 src/FinanceTrackerCLI/finance_tracker.py
 src/FinanceTrackerCLI.egg-info/PKG-INFO
 src/FinanceTrackerCLI.egg-info/SOURCES.txt
 src/FinanceTrackerCLI.egg-info/dependency_links.txt
 src/FinanceTrackerCLI.egg-info/requires.txt
 src/FinanceTrackerCLI.egg-info/top_level.txt
 src/FinanceTrackerCLI/logic/__init__.py
```

