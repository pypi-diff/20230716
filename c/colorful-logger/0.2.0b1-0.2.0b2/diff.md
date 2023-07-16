# Comparing `tmp/colorful-logger-0.2.0b1.tar.gz` & `tmp/colorful-logger-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful-logger-0.2.0b1.tar", last modified: Thu Apr  6 09:06:55 2023, max compression
+gzip compressed data, was "colorful-logger-0.2.0b2.tar", last modified: Sun Jul 16 01:06:29 2023, max compression
```

## Comparing `colorful-logger-0.2.0b1.tar` & `colorful-logger-0.2.0b2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:06:55.258862 colorful-logger-0.2.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:06:55.254862 colorful-logger-0.2.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:06:55.254862 colorful-logger-0.2.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-06 09:06:55.258862 colorful-logger-0.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/README.zh_CN.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:06:55.258862 colorful-logger-0.2.0b1/colorful_logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/colorful_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/colorful_logger/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/colorful_logger/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/colorful_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/colorful_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/colorful_logger/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/colorful_logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-06 09:06:55.000000 colorful-logger-0.2.0b1/colorful_logger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:06:55.258862 colorful-logger-0.2.0b1/colorful_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-06 09:06:55.000000 colorful-logger-0.2.0b1/colorful_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-06 09:06:55.000000 colorful-logger-0.2.0b1/colorful_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:06:55.000000 colorful-logger-0.2.0b1/colorful_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 09:06:55.000000 colorful-logger-0.2.0b1/colorful_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 09:06:55.000000 colorful-logger-0.2.0b1/colorful_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-06 09:06:41.000000 colorful-logger-0.2.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 09:06:55.258862 colorful-logger-0.2.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.175374 colorful-logger-0.2.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/README.zh_CN.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/colorful_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/colorful_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/setup.cfg
```

### Comparing `colorful-logger-0.2.0b1/.github/workflows/publish.yaml` & `colorful-logger-0.2.0b2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/.gitignore` & `colorful-logger-0.2.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/LICENSE` & `colorful-logger-0.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/PKG-INFO` & `colorful-logger-0.2.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-logger
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: A colorful logger for python3.
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `colorful-logger-0.2.0b1/README.md` & `colorful-logger-0.2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/README.zh_CN.md` & `colorful-logger-0.2.0b2/README.zh_CN.md`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/colorful_logger/__init__.py` & `colorful-logger-0.2.0b2/colorful_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/colorful_logger/consts.py` & `colorful-logger-0.2.0b2/colorful_logger/consts.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/colorful_logger/formatter.py` & `colorful-logger-0.2.0b2/colorful_logger/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Author:      thepoy
-# @Email:       thepoy@163.com
-# @File Name:   formatter.py
-# @Created At:  2021-05-21 13:53:40
-# @Modified At: 2023-03-06 21:22:14
-# @Modified By: thepoy
 
 import sys
 import os
 import json
 
 from datetime import datetime
 from logging import Formatter, LogRecord
@@ -200,15 +194,15 @@
             kwargs[k] = str(v)
 
         if self.to_file:
             log_map = {
                 "level": record.levelname,
                 "time": self.__time(record),
                 "message": msg,
-                **record.kwargs,
+                **kwargs,
                 "caller": f"{self.__file_path(record)}{self.__line_number(record)}",
             }
 
             return json.dumps(log_map)
 
         for k, v in record.kwargs.items():
             if k in ("err", "error"):
```

### Comparing `colorful-logger-0.2.0b1/colorful_logger/handlers.py` & `colorful-logger-0.2.0b2/colorful_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/colorful_logger/logger.py` & `colorful-logger-0.2.0b2/colorful_logger/logger.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b1/colorful_logger.egg-info/PKG-INFO` & `colorful-logger-0.2.0b2/colorful_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-logger
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: A colorful logger for python3.
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `colorful-logger-0.2.0b1/pyproject.toml` & `colorful-logger-0.2.0b2/pyproject.toml`

 * *Files identical despite different names*

