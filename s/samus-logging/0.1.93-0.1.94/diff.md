# Comparing `tmp/samus-logging-0.1.93.tar.gz` & `tmp/samus-logging-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.93.tar", last modified: Sun Jul 16 18:11:48 2023, max compression
+gzip compressed data, was "samus-logging-0.1.94.tar", last modified: Sun Jul 16 18:15:53 2023, max compression
```

## Comparing `samus-logging-0.1.93.tar` & `samus-logging-0.1.94.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:11:48.251634 samus-logging-0.1.93/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.93/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:11:48.251634 samus-logging-0.1.93/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)       49 2023-07-10 16:43:05.000000 samus-logging-0.1.93/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:11:48.247635 samus-logging-0.1.93/samus_logging/
--rw-rw-r--   0 samu      (1000) samu      (1000)       57 2023-07-16 18:11:47.000000 samus-logging-0.1.93/samus_logging/__init__.py
--rw-rw-r--   0 samu      (1000) samu      (1000)      482 2023-07-10 15:52:51.000000 samus-logging-0.1.93/samus_logging/level_filter.py
--rw-rw-r--   0 samu      (1000) samu      (1000)     4654 2023-07-16 18:07:01.000000 samus-logging-0.1.93/samus_logging/samus_logging.py
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:11:48.251634 samus-logging-0.1.93/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:11:48.000000 samus-logging-0.1.93/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-16 18:11:48.000000 samus-logging-0.1.93/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-16 18:11:48.000000 samus-logging-0.1.93/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-16 18:11:48.000000 samus-logging-0.1.93/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-16 18:11:48.000000 samus-logging-0.1.93/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-16 18:11:48.251634 samus-logging-0.1.93/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)     1286 2023-07-10 17:23:15.000000 samus-logging-0.1.93/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:15:53.918986 samus-logging-0.1.94/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.94/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:15:53.914986 samus-logging-0.1.94/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)       49 2023-07-10 16:43:05.000000 samus-logging-0.1.94/README.md
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:15:53.914986 samus-logging-0.1.94/samus_logging/
+-rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-16 18:14:00.000000 samus-logging-0.1.94/samus_logging/__init__.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)      482 2023-07-10 15:52:51.000000 samus-logging-0.1.94/samus_logging/level_filter.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)     4667 2023-07-16 18:14:15.000000 samus-logging-0.1.94/samus_logging/samus_logging.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:15:53.914986 samus-logging-0.1.94/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/top_level.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-16 18:15:53.918986 samus-logging-0.1.94/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)     1286 2023-07-10 17:23:15.000000 samus-logging-0.1.94/setup.py
```

### Comparing `samus-logging-0.1.93/PKG-INFO` & `samus-logging-0.1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.93
+Version: 0.1.94
 Summary: A minimal Logging-controller.
 Home-page: https://github.com/samuscodes/Samus-Logging
 Author: Samu Rabin
 Author-email: samus_codes@samusoft.net
 Maintainer: Samu Rabin
 Maintainer-email: samus_codes@samusoft.net
 License: UNKNOWN
```

### Comparing `samus-logging-0.1.93/samus_logging/samus_logging.py` & `samus-logging-0.1.94/samus_logging/samus_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from .level_filter import LevelFilter
+from samus_logging.level_filter import LevelFilter
 from pathlib import Path
 import os
 
 
 class Samus_Logging:
     """A minimal Logging-controller."""
```

### Comparing `samus-logging-0.1.93/samus_logging.egg-info/PKG-INFO` & `samus-logging-0.1.94/samus_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.93
+Version: 0.1.94
 Summary: A minimal Logging-controller.
 Home-page: https://github.com/samuscodes/Samus-Logging
 Author: Samu Rabin
 Author-email: samus_codes@samusoft.net
 Maintainer: Samu Rabin
 Maintainer-email: samus_codes@samusoft.net
 License: UNKNOWN
```

### Comparing `samus-logging-0.1.93/setup.py` & `samus-logging-0.1.94/setup.py`

 * *Files identical despite different names*

