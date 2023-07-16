# Comparing `tmp/FinanceTrackerCLI-1.3.0.1.tar.gz` & `tmp/FinanceTrackerCLI-1.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinanceTrackerCLI-1.3.0.1.tar", last modified: Sun Jul 16 17:47:21 2023, max compression
+gzip compressed data, was "FinanceTrackerCLI-1.3.0.2.tar", last modified: Sun Jul 16 17:50:36 2023, max compression
```

## Comparing `FinanceTrackerCLI-1.3.0.1.tar` & `FinanceTrackerCLI-1.3.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:47:21.568671 FinanceTrackerCLI-1.3.0.1/
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.3.0.1/LICENSE
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:47:21.568578 FinanceTrackerCLI-1.3.0.1/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      292 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.1/README.md
--rw-r--r--   0 vladkobranov   (501) staff       (20)      124 2023-07-16 16:47:26.000000 FinanceTrackerCLI-1.3.0.1/pyproject.toml
--rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-16 17:47:21.568701 FinanceTrackerCLI-1.3.0.1/setup.cfg
--rw-r--r--   0 vladkobranov   (501) staff       (20)      704 2023-07-16 17:47:17.000000 FinanceTrackerCLI-1.3.0.1/setup.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:47:21.566312 FinanceTrackerCLI-1.3.0.1/src/
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:47:21.566988 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      299 2023-07-16 17:41:57.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/__init__.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3144 2023-07-16 15:56:56.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/finance_tracker.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:47:21.568433 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      616 2023-07-16 17:45:33.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/__init__.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/grouped_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/input_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/local_convertor.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/search_by_month_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/show_all_delete_string.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/terminal_name.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     2536 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/text_prompts.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:47:21.567512 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:47:21.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      708 2023-07-16 17:47:21.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/SOURCES.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 17:47:21.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/dependency_links.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 17:47:21.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/requires.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 17:47:21.000000 FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/top_level.txt
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:50:36.823446 FinanceTrackerCLI-1.3.0.2/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.3.0.2/LICENSE
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:50:36.823349 FinanceTrackerCLI-1.3.0.2/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      292 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.2/README.md
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      124 2023-07-16 16:47:26.000000 FinanceTrackerCLI-1.3.0.2/pyproject.toml
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-16 17:50:36.823490 FinanceTrackerCLI-1.3.0.2/setup.cfg
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      704 2023-07-16 17:50:32.000000 FinanceTrackerCLI-1.3.0.2/setup.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:50:36.821019 FinanceTrackerCLI-1.3.0.2/src/
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:50:36.821726 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      299 2023-07-16 17:41:57.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/__init__.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3710 2023-07-16 17:50:32.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/finance_tracker.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:50:36.823195 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      616 2023-07-16 17:45:33.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/__init__.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/grouped_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/input_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/local_convertor.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/search_by_month_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/show_all_delete_string.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/terminal_name.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     2536 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/text_prompts.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 17:50:36.822268 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 17:50:36.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      708 2023-07-16 17:50:36.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 17:50:36.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 17:50:36.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/requires.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 17:50:36.000000 FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/top_level.txt
```

### Comparing `FinanceTrackerCLI-1.3.0.1/LICENSE` & `FinanceTrackerCLI-1.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/PKG-INFO` & `FinanceTrackerCLI-1.3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinanceTrackerCLI
-Version: 1.3.0.1
+Version: 1.3.0.2
 Summary: Finance tracker CLI app
 Home-page: https://github.com/VladimirKobranov/FinanceTrackerCLI
 Author: Vladimir Kobranov
 Author-email: josephclturok@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `FinanceTrackerCLI-1.3.0.1/setup.py` & `FinanceTrackerCLI-1.3.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FinanceTrackerCLI',
-    version='1.3.0.1',
+    version='1.3.0.2',
     author='Vladimir Kobranov',
     author_email='josephclturok@gmail.com',
     description='Finance tracker CLI app',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VladimirKobranov/FinanceTrackerCLI',
     classifiers=[
```

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/finance_tracker.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/finance_tracker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import json
 import os
 import os.path
 
-from logic.grouped_data import grouped_final
-from logic.input_data import input_string
-from logic.local_convertor import local_convertor
-from logic.search_by_month_data import search_by_month
-from logic.show_all_delete_string import delete_string
-from logic.terminal_name import set_terminal_title, get_terminal_title
-from logic.text_prompts import mainMessage, helpMessage, creditsMessage, availableCurrencies, currency_list
+# from logic.grouped_data import grouped_final
+# from logic.input_data import input_string
+# from logic.local_convertor import local_convertor
+# from logic.search_by_month_data import search_by_month
+# from logic.show_all_delete_string import delete_string
+# from logic.terminal_name import set_terminal_title, get_terminal_title
+# from logic.text_prompts import mainMessage, helpMessage, creditsMessage, availableCurrencies, currency_list
+from FinanceTrackerCLI.logic.grouped_data import grouped_final
+from FinanceTrackerCLI.logic.input_data import input_string
+from FinanceTrackerCLI.logic.local_convertor import local_convertor
+from FinanceTrackerCLI.logic.search_by_month_data import search_by_month
+from FinanceTrackerCLI.logic.show_all_delete_string import delete_string
+from FinanceTrackerCLI.logic.terminal_name import set_terminal_title, get_terminal_title
+from FinanceTrackerCLI.logic.text_prompts import mainMessage, helpMessage, creditsMessage, availableCurrencies, currency_list
 
 new_title = 'Finance tracker'
 original_title = get_terminal_title()
 set_terminal_title(new_title)
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 file_path = os.path.join(current_dir, "data/FinanceList.json")
```

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/__init__.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/grouped_data.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/grouped_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/input_data.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/input_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/local_convertor.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/local_convertor.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/search_by_month_data.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/search_by_month_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/show_all_delete_string.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/show_all_delete_string.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/terminal_name.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/terminal_name.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI/logic/text_prompts.py` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI/logic/text_prompts.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/PKG-INFO` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinanceTrackerCLI
-Version: 1.3.0.1
+Version: 1.3.0.2
 Summary: Finance tracker CLI app
 Home-page: https://github.com/VladimirKobranov/FinanceTrackerCLI
 Author: Vladimir Kobranov
 Author-email: josephclturok@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `FinanceTrackerCLI-1.3.0.1/src/FinanceTrackerCLI.egg-info/SOURCES.txt` & `FinanceTrackerCLI-1.3.0.2/src/FinanceTrackerCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

