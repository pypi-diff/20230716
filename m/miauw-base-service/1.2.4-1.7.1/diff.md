# Comparing `tmp/miauw-base-service-1.2.4.tar.gz` & `tmp/miauw-base-service-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.2.4.tar", last modified: Sun Jul 16 08:31:41 2023, max compression
+gzip compressed data, was "miauw-base-service-1.7.1.tar", last modified: Sun Jul 16 11:48:03 2023, max compression
```

## Comparing `miauw-base-service-1.2.4.tar` & `miauw-base-service-1.7.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 08:31:41.011596 miauw-base-service-1.2.4/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.4/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:33:12.000000 miauw-base-service-1.2.4/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2168 2023-07-16 08:29:23.000000 miauw-base-service-1.2.4/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 08:31:41.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 08:29:37.000000 miauw-base-service-1.2.4/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 08:29:37.000000 miauw-base-service-1.2.4/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/email_worker.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/exceptions.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2134 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2168 2023-07-16 08:29:23.000000 miauw-base-service-1.7.1/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      360 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/setup.py
```

### Comparing `miauw-base-service-1.2.4/base_service/service.py` & `miauw-base-service-1.7.1/base_service/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from base_service import RabbitMQWorker
+from base_service.email_worker import EmailTemplates, EMailWorker
+from base_service.worker import RabbitMQWorker
 from collections import defaultdict
 import asyncio
 import typing
 import logging
-
+import os
 
 class BaseService:
     """creates the base service class"""
 
     def __init__(
-        self, name: str, url: str, logfile: str = None, worker_log: bool = True
+        self, name: str, url: str | None= os.getenv("RABBITMQ_URL"), logfile: str = None, worker_log: bool = True
     ):
+        if not url:
+            raise Exception("No URL provided and env var 'RABBITMQ_URL' is empty.")
         self.worker = RabbitMQWorker(url)
+        self.emailer = EMailWorker(url)
         self.events: list[str] = []
         self.m: dict[
             str, typing.Callable[[typing.Any], typing.Awaitable[typing.Any]]
         ] = defaultdict()
         self.name = name
         # logging
         self.logger = logging.getLogger(name)
```

### Comparing `miauw-base-service-1.2.4/base_service/worker.py` & `miauw-base-service-1.7.1/base_service/worker.py`

 * *Files identical despite different names*

