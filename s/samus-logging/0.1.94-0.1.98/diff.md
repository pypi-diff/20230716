# Comparing `tmp/samus-logging-0.1.94.tar.gz` & `tmp/samus-logging-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.94.tar", last modified: Sun Jul 16 18:15:53 2023, max compression
+gzip compressed data, was "samus-logging-0.1.98.tar", last modified: Sun Jul 16 18:23:24 2023, max compression
```

## Comparing `samus-logging-0.1.94.tar` & `samus-logging-0.1.98.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:15:53.918986 samus-logging-0.1.94/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.94/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:15:53.914986 samus-logging-0.1.94/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)       49 2023-07-10 16:43:05.000000 samus-logging-0.1.94/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:15:53.914986 samus-logging-0.1.94/samus_logging/
--rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-16 18:14:00.000000 samus-logging-0.1.94/samus_logging/__init__.py
--rw-rw-r--   0 samu      (1000) samu      (1000)      482 2023-07-10 15:52:51.000000 samus-logging-0.1.94/samus_logging/level_filter.py
--rw-rw-r--   0 samu      (1000) samu      (1000)     4667 2023-07-16 18:14:15.000000 samus-logging-0.1.94/samus_logging/samus_logging.py
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:15:53.914986 samus-logging-0.1.94/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-16 18:15:53.000000 samus-logging-0.1.94/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-16 18:15:53.918986 samus-logging-0.1.94/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)     1286 2023-07-10 17:23:15.000000 samus-logging-0.1.94/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:23:24.013116 samus-logging-0.1.98/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.98/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:23:24.013116 samus-logging-0.1.98/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)       49 2023-07-10 16:43:05.000000 samus-logging-0.1.98/README.md
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:23:24.013116 samus-logging-0.1.98/samus_logging/
+-rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-16 18:22:12.000000 samus-logging-0.1.98/samus_logging/__init__.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)      482 2023-07-10 15:52:51.000000 samus-logging-0.1.98/samus_logging/level_filter.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)     4667 2023-07-16 18:22:16.000000 samus-logging-0.1.98/samus_logging/samus_logging.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-16 18:23:24.013116 samus-logging-0.1.98/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)      775 2023-07-16 18:23:23.000000 samus-logging-0.1.98/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-16 18:23:23.000000 samus-logging-0.1.98/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-16 18:23:23.000000 samus-logging-0.1.98/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-16 18:23:23.000000 samus-logging-0.1.98/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-16 18:23:23.000000 samus-logging-0.1.98/samus_logging.egg-info/top_level.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-16 18:23:24.013116 samus-logging-0.1.98/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)     1286 2023-07-10 17:23:15.000000 samus-logging-0.1.98/setup.py
```

### Comparing `samus-logging-0.1.94/PKG-INFO` & `samus-logging-0.1.98/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.94
+Version: 0.1.98
 Summary: A minimal Logging-controller.
 Home-page: https://github.com/samuscodes/Samus-Logging
 Author: Samu Rabin
 Author-email: samus_codes@samusoft.net
 Maintainer: Samu Rabin
 Maintainer-email: samus_codes@samusoft.net
 License: UNKNOWN
```

### Comparing `samus-logging-0.1.94/samus_logging/samus_logging.py` & `samus-logging-0.1.98/samus_logging/samus_logging.py`

 * *Files identical despite different names*

### Comparing `samus-logging-0.1.94/samus_logging.egg-info/PKG-INFO` & `samus-logging-0.1.98/samus_logging.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.94
+Version: 0.1.98
 Summary: A minimal Logging-controller.
 Home-page: https://github.com/samuscodes/Samus-Logging
 Author: Samu Rabin
 Author-email: samus_codes@samusoft.net
 Maintainer: Samu Rabin
 Maintainer-email: samus_codes@samusoft.net
 License: UNKNOWN
```

### Comparing `samus-logging-0.1.94/setup.py` & `samus-logging-0.1.98/setup.py`

 * *Files identical despite different names*

