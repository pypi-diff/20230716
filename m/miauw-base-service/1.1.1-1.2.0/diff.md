# Comparing `tmp/miauw-base-service-1.1.1.tar.gz` & `tmp/miauw-base-service-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.1.1.tar", last modified: Sat Jul 15 16:10:34 2023, max compression
+gzip compressed data, was "miauw-base-service-1.2.0.tar", last modified: Sun Jul 16 06:12:18 2023, max compression
```

## Comparing `miauw-base-service-1.1.1.tar` & `miauw-base-service-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 16:10:34.851368 miauw-base-service-1.1.1/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 16:10:34.848034 miauw-base-service-1.1.1/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 16:10:34.848034 miauw-base-service-1.1.1/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.1.1/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2026 2023-07-15 15:57:46.000000 miauw-base-service-1.1.1/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1997 2023-07-15 16:03:21.000000 miauw-base-service-1.1.1/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 16:10:34.848034 miauw-base-service-1.1.1/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 16:05:44.000000 miauw-base-service-1.1.1/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-15 16:10:34.851368 miauw-base-service-1.1.1/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-15 16:05:48.000000 miauw-base-service-1.1.1/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.0/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:01:40.000000 miauw-base-service-1.2.0/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2144 2023-07-16 06:06:59.000000 miauw-base-service-1.2.0/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:07:28.000000 miauw-base-service-1.2.0/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 06:07:28.000000 miauw-base-service-1.2.0/setup.py
```

### Comparing `miauw-base-service-1.1.1/base_service/service.py` & `miauw-base-service-1.2.0/base_service/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from base_service import RabbitMQWorker
 from collections import defaultdict
 import asyncio
 import typing
 import logging
 
+
 class BaseService:
     """creates the base service class"""
-    def __init__(self, name: str, url: str, logfile: str = None, worker_log: bool = True):
+
+    def __init__(
+        self, name: str, url: str, logfile: str = None, worker_log: bool = True
+    ):
         self.worker = RabbitMQWorker(url)
         self.events: list[str] = []
-        self.m: dict[str, typing.Callable[[typing.Any], typing.Awaitable[typing.Any]]] = defaultdict()
+        self.m: dict[
+            str, typing.Callable[[typing.Any], typing.Awaitable[typing.Any]]
+        ] = defaultdict()
         self.name = name
         # logging
         self.logger = logging.getLogger(name)
         self.log_formatter = logging.Formatter("[%(asctime)s] - %(name)s - %(message)s")
         self.log_filehandler = logging.FileHandler(logfile or "service.log")
         self.log_streamhandler = logging.StreamHandler()
         self.logger.setLevel(logging.DEBUG)
@@ -26,22 +32,20 @@
 
     def start(self):
         """starts the service"""
         self.logger.info("starting")
         loop = asyncio.get_event_loop()
         for ev in self.events:
             self.logger.info(f"listening for event '{ev}'")
-        loop.run_until_complete(asyncio.gather(*[self.worker.listen(k,v) for k,v in self.m.items()]))
-
-
-    def add_event_handler(self, event: str, handler: typing.Callable[[typing.Any], typing.Awaitable[typing.Any]]) -> None:
-        """adds a new event handler for service"""
-        self.logger.debug(f"add handler {handler} for event '{event}'")
-        self.events.append(event)
-        self.m[event] = handler
-
+        loop.run_until_complete(
+            asyncio.gather(*[self.worker.listen(k, v) for k, v in self.m.items()])
+        )
 
     def event(self, event: str):
         """adds a new event handler for event"""
+
         def wrapper(handler: typing.Callable[[dict], typing.Awaitable[dict]]):
-            self.add_event_handler(event, handler)
+            self.logger.debug(f"add handler {handler} for event '{event}'")
+            self.events.append(event)
+            self.m[event] = handler
+
         return wrapper
```

### Comparing `miauw-base-service-1.1.1/base_service/worker.py` & `miauw-base-service-1.2.0/base_service/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Callable, Awaitable, Any
 import aio_pika
 import json
 import asyncio
-
+import traceback
+import os
 
 class RabbitMQWorker:
     """RabbitMQ Base Worker Class"""
 
     def __init__(self, url: str):
         self.connection = None
         self.url: str = url
@@ -45,7 +46,9 @@
                                 body=json.dumps(res).encode("utf-8"),
                                 correlation_id=message.correlation_id,
                             ),
                             routing_key=message.reply_to,
                         )
                 except Exception as e:
                     print("[!] Exception: ", e)
+                    if os.getenv("SERVICE_TRACEBACK") == "active":
+                        print(traceback.format_exc())
```

