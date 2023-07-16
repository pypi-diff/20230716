# Comparing `tmp/scrapypi-0.0.1.tar.gz` & `tmp/scrapypi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapypi-0.0.1.tar", last modified: Sun Jul 16 20:58:04 2023, max compression
+gzip compressed data, was "scrapypi-0.0.2.tar", last modified: Sun Jul 16 21:05:41 2023, max compression
```

## Comparing `scrapypi-0.0.1.tar` & `scrapypi-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 20:58:04.881128 scrapypi-0.0.1/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       99 2023-07-16 19:56:56.000000 scrapypi-0.0.1/CHANGELOG.md
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1065 2023-07-16 19:52:15.000000 scrapypi-0.0.1/LICENCE.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.1/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      719 2023-07-16 20:58:04.881128 scrapypi-0.0.1/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       84 2023-07-16 20:57:10.000000 scrapypi-0.0.1/README.md
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 20:58:04.877128 scrapypi-0.0.1/scrapypi/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       21 2023-07-16 20:26:59.000000 scrapypi-0.0.1/scrapypi/__init__.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1131 2023-07-16 20:14:05.000000 scrapypi-0.0.1/scrapypi/scrapypi.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 20:58:04.881128 scrapypi-0.0.1/scrapypi.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      719 2023-07-16 20:58:04.000000 scrapypi-0.0.1/scrapypi.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      291 2023-07-16 20:58:04.000000 scrapypi-0.0.1/scrapypi.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-16 20:58:04.000000 scrapypi-0.0.1/scrapypi.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-16 20:58:04.000000 scrapypi-0.0.1/scrapypi.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        5 2023-07-16 20:58:04.000000 scrapypi-0.0.1/scrapypi.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        9 2023-07-16 20:58:04.000000 scrapypi-0.0.1/scrapypi.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-16 20:58:04.881128 scrapypi-0.0.1/setup.cfg
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1225 2023-07-16 20:56:11.000000 scrapypi-0.0.1/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 21:05:41.638242 scrapypi-0.0.2/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      173 2023-07-16 21:04:21.000000 scrapypi-0.0.2/CHANGELOG.md
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1065 2023-07-16 19:52:15.000000 scrapypi-0.0.2/LICENCE.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.2/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      793 2023-07-16 21:05:41.638242 scrapypi-0.0.2/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       84 2023-07-16 20:57:10.000000 scrapypi-0.0.2/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 21:05:41.634242 scrapypi-0.0.2/scrapypi/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       23 2023-07-16 21:01:59.000000 scrapypi-0.0.2/scrapypi/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1131 2023-07-16 20:14:05.000000 scrapypi-0.0.2/scrapypi/scrapypi.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 21:05:41.638242 scrapypi-0.0.2/scrapypi.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      793 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      291 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        5 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        9 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-16 21:05:41.638242 scrapypi-0.0.2/setup.cfg
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1225 2023-07-16 21:03:40.000000 scrapypi-0.0.2/setup.py
```

### Comparing `scrapypi-0.0.1/LICENCE.txt` & `scrapypi-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.1/PKG-INFO` & `scrapypi-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get PyPi Package information.
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: pypi,information,package,module,stats,info,scrape
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -20,7 +20,11 @@
 
 
 # **:- Change Log -:**
 
 > **0.0.1** -- [ 16 JULY 2023 ]  
 > [ NOTICE ]  
 > [ ! ] - Initial Release
+
+> **0.0.2** -- [ 16 JULY 2023 ]  
+> [ FIXED ]  
+> [ + ] - Import and Run
```

### Comparing `scrapypi-0.0.1/scrapypi/scrapypi.py` & `scrapypi-0.0.2/scrapypi/scrapypi.py`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.1/scrapypi.egg-info/PKG-INFO` & `scrapypi-0.0.2/scrapypi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get PyPi Package information.
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: pypi,information,package,module,stats,info,scrape
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -20,7 +20,11 @@
 
 
 # **:- Change Log -:**
 
 > **0.0.1** -- [ 16 JULY 2023 ]  
 > [ NOTICE ]  
 > [ ! ] - Initial Release
+
+> **0.0.2** -- [ 16 JULY 2023 ]  
+> [ FIXED ]  
+> [ + ] - Import and Run
```

### Comparing `scrapypi-0.0.1/setup.py` & `scrapypi-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Get PyPi Package information.'
 KEYWORDS = ['pypi', 'information', 'package', 'module', 'stats', 'info', 'scrape']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
```

