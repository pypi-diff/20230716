# Comparing `tmp/miauw-base-service-1.7.2.tar.gz` & `tmp/miauw-base-service-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.7.2.tar", last modified: Sun Jul 16 14:32:47 2023, max compression
+gzip compressed data, was "miauw-base-service-1.8.0.tar", last modified: Sun Jul 16 15:16:58 2023, max compression
```

## Comparing `miauw-base-service-1.7.2.tar` & `miauw-base-service-1.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 14:32:47.791130 miauw-base-service-1.7.2/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.7.2/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.7.2/base_service/email_worker.py
--rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.7.2/base_service/exceptions.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2134 2023-07-16 14:27:13.000000 miauw-base-service-1.7.2/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2317 2023-07-16 14:32:21.000000 miauw-base-service-1.7.2/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      360 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 14:32:21.000000 miauw-base-service-1.7.2/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 14:32:21.000000 miauw-base-service-1.7.2/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 15:16:58.571073 miauw-base-service-1.8.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 15:16:58.571073 miauw-base-service-1.8.0/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 15:16:58.567740 miauw-base-service-1.8.0/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.8.0/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.8.0/base_service/email_worker.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.8.0/base_service/exceptions.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2226 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2715 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 15:16:58.567740 miauw-base-service-1.8.0/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      360 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 15:16:58.571073 miauw-base-service-1.8.0/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/setup.py
```

### Comparing `miauw-base-service-1.7.2/base_service/email_worker.py` & `miauw-base-service-1.8.0/base_service/email_worker.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.7.2/base_service/exceptions.py` & `miauw-base-service-1.8.0/base_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.7.2/base_service/service.py` & `miauw-base-service-1.8.0/base_service/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         if not url:
             raise Exception("No URL provided and env var 'RABBITMQ_URL' is empty.")
         self.worker = RabbitMQWorker(url)
         self.emailer = EMailWorker(url)
         self.events: list[str] = []
         self.m: dict[
             str, typing.Callable[[typing.Any], typing.Awaitable[typing.Any]]
-        ] = defaultdict()
+        ] = defaultdict(rpc={}, basic={})
         self.name = name
         # logging
         self.logger = logging.getLogger(name)
         self.log_formatter = logging.Formatter("[%(asctime)s] - %(name)s - %(message)s")
         self.log_filehandler = logging.FileHandler(logfile or "service.log")
         self.log_streamhandler = logging.StreamHandler()
         self.logger.setLevel(logging.DEBUG)
@@ -37,19 +37,18 @@
     def start(self):
         """starts the service"""
         self.logger.info("starting")
         loop = asyncio.get_event_loop()
         for ev in self.events:
             self.logger.info(f"listening for event '{ev}'")
         loop.run_until_complete(
-            asyncio.gather(*[self.worker.listen(k, v) for k, v in self.m.items()])
+            asyncio.gather(*[self.worker.listen(event, handler) for a in self.m.values() for event, handler in a.items()])
         )
 
-    def event(self, event: str):
+    def event(self, event: str, event_type: str = "rpc"):
         """adds a new event handler for event"""
 
         def wrapper(handler: typing.Callable[[dict], typing.Awaitable[dict]]):
             self.logger.debug(f"add handler {handler} for event '{event}'")
             self.events.append(event)
-            self.m[event] = handler
-
+            self.m[event_type][event] = handler
         return wrapper
```

### Comparing `miauw-base-service-1.7.2/base_service/worker.py` & `miauw-base-service-1.8.0/base_service/worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Callable, Awaitable, Any
 import aio_pika
 import json
 import asyncio
 import traceback
 import os
 
+
 class RabbitMQWorker:
     """RabbitMQ Base Worker Class"""
 
     def __init__(self, url: str):
         self.connection = None
         self.url: str = url
         self.channel: aio_pika.abc.AbstractChannel = None
@@ -26,33 +27,43 @@
         try:
             data = json.loads(message.body)
         except json.JSONDecodeError:
             data = message.body.decode("utf-8")
         await self.ex.publish(aio_pika.Message(data), routing_key=queue_name)
 
     async def listen(
-        self, queue_name: str, worker_function: Callable[[Any], Awaitable[Any]]
+        self,
+        queue_name: str,
+        worker_function: Callable[[Any], Awaitable[Any]]
     ):
         await self.setup()
         queue = await self.channel.declare_queue(queue_name)
         async with queue.iterator() as qi:
             message: aio_pika.abc.AbstractMessage
             async for message in qi:
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
                         try:
                             data = json.loads(message.body)
                         except json.JSONDecodeError:
                             data = message.body.decode("utf-8")
                         res = await worker_function(data)
+                        return
                         await self.ex.publish(
                             aio_pika.Message(
                                 body=json.dumps(res).encode("utf-8"),
                                 correlation_id=message.correlation_id,
                             ),
                             routing_key=message.reply_to,
                         )
                 except Exception as e:
-                    print("[!] Exception: ", e)
-                    if os.getenv("SERVICE_TRACEBACK") == "active":
-                        print(traceback.format_exc())
+                    if isinstance(e, AssertionError):
+                        try:
+                            data = json.loads(message.body)
+                        except json.JSONDecodeError:
+                            data = message.body.decode("utf-8")
+                        await worker_function(data)
+                    else:
+                        print("[!] Exception: ", e)
+                        if os.getenv("SERVICE_TRACEBACK") == "active":
+                            print(traceback.format_exc())
```

