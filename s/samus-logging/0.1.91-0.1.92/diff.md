# Comparing `tmp/samus-logging-0.1.91.tar.gz` & `tmp/samus-logging-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.91.tar", last modified: Mon Jul 10 16:38:48 2023, max compression
+gzip compressed data, was "samus-logging-0.1.92.tar", last modified: Sun Jul 16 17:57:01 2023, max compression
```

## Comparing `samus-logging-0.1.91.tar` & `samus-logging-0.1.92.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-10 16:38:48.156048 samus-logging-0.1.91/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.91/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      745 2023-07-10 16:38:48.156048 samus-logging-0.1.91/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-07-08 10:45:11.000000 samus-logging-0.1.91/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-10 16:38:48.156048 samus-logging-0.1.91/samus_logging/
--rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-08 08:29:30.000000 samus-logging-0.1.91/samus_logging/__init__.py
--rw-rw-r--   0 samu      (1000) samu      (1000)      482 2023-07-10 15:52:51.000000 samus-logging-0.1.91/samus_logging/level_filter.py
--rw-rw-r--   0 samu      (1000) samu      (1000)     4667 2023-07-10 16:00:59.000000 samus-logging-0.1.91/samus_logging/samus_logging.py
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-10 16:38:48.156048 samus-logging-0.1.91/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      745 2023-07-10 16:38:48.000000 samus-logging-0.1.91/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-10 16:38:48.000000 samus-logging-0.1.91/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-10 16:38:48.000000 samus-logging-0.1.91/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-10 16:38:48.000000 samus-logging-0.1.91/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-10 16:38:48.000000 samus-logging-0.1.91/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-10 16:38:48.156048 samus-logging-0.1.91/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)     1298 2023-07-10 16:35:43.000000 samus-logging-0.1.91/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 17:57:01.342150 samus-logging-0.1.92/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.92/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 17:57:01.338150 samus-logging-0.1.92/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)       49 2023-07-10 16:43:05.000000 samus-logging-0.1.92/README.md
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 17:57:01.338150 samus-logging-0.1.92/samus_logging/
+-rw-rw-r--   0 samu      (1000) samu      (1000)       69 2023-07-16 17:55:05.000000 samus-logging-0.1.92/samus_logging/__init__.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)      482 2023-07-10 15:52:51.000000 samus-logging-0.1.92/samus_logging/level_filter.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)     4653 2023-07-16 17:56:34.000000 samus-logging-0.1.92/samus_logging/samus_logging.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 17:57:01.338150 samus-logging-0.1.92/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 17:57:01.000000 samus-logging-0.1.92/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-16 17:57:01.000000 samus-logging-0.1.92/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-16 17:57:01.000000 samus-logging-0.1.92/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-16 17:57:01.000000 samus-logging-0.1.92/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-16 17:57:01.000000 samus-logging-0.1.92/samus_logging.egg-info/top_level.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-16 17:57:01.342150 samus-logging-0.1.92/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)     1286 2023-07-10 17:23:15.000000 samus-logging-0.1.92/setup.py
```

### Comparing `samus-logging-0.1.91/PKG-INFO` & `samus-logging-0.1.92/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.91
+Version: 0.1.92
 Summary: A minimal Logging-controller.
-Home-page: https://github.com/MarblesTheMadOne/Samus-Logging
+Home-page: https://github.com/samuscodes/Samus-Logging
 Author: Samu Rabin
 Author-email: samus_codes@samusoft.net
 Maintainer: Samu Rabin
 Maintainer-email: samus_codes@samusoft.net
 License: UNKNOWN
-Download-URL: https://github.com/MarblesTheMadOne/Samus-Logging
+Download-URL: https://github.com/samuscodes/Samus-Logging
 Keywords: python,logging,logger,minimal
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-UNKNOWN
+![Dependency Diagramm](plantuml/dependencies.png)
```

### Comparing `samus-logging-0.1.91/samus_logging/samus_logging.py` & `samus-logging-0.1.92/samus_logging/samus_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from samus_logging.level_filter import LevelFilter
+from level_filter import LevelFilter
 from pathlib import Path
 import os
 
 
 class Samus_Logging:
     """A minimal Logging-controller."""
```

### Comparing `samus-logging-0.1.91/samus_logging.egg-info/PKG-INFO` & `samus-logging-0.1.92/samus_logging.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.91
+Version: 0.1.92
 Summary: A minimal Logging-controller.
-Home-page: https://github.com/MarblesTheMadOne/Samus-Logging
+Home-page: https://github.com/samuscodes/Samus-Logging
 Author: Samu Rabin
 Author-email: samus_codes@samusoft.net
 Maintainer: Samu Rabin
 Maintainer-email: samus_codes@samusoft.net
 License: UNKNOWN
-Download-URL: https://github.com/MarblesTheMadOne/Samus-Logging
+Download-URL: https://github.com/samuscodes/Samus-Logging
 Keywords: python,logging,logger,minimal
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-UNKNOWN
+![Dependency Diagramm](plantuml/dependencies.png)
```

### Comparing `samus-logging-0.1.91/setup.py` & `samus-logging-0.1.92/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     description='A minimal Logging-controller.',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     author='Samu Rabin',
     author_email='samus_codes@samusoft.net',
     maintainer='Samu Rabin',
     maintainer_email='samus_codes@samusoft.net',
-    url='https://github.com/MarblesTheMadOne/Samus-Logging',
-    download_url='https://github.com/MarblesTheMadOne/Samus-Logging',
+    url='https://github.com/samuscodes/Samus-Logging',
+    download_url='https://github.com/samuscodes/Samus-Logging',
     keywords=['python', 'logging', 'logger', 'minimal'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
```

