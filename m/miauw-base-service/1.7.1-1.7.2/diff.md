# Comparing `tmp/miauw-base-service-1.7.1.tar.gz` & `tmp/miauw-base-service-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.7.1.tar", last modified: Sun Jul 16 11:48:03 2023, max compression
+gzip compressed data, was "miauw-base-service-1.7.2.tar", last modified: Sun Jul 16 14:32:47 2023, max compression
```

## Comparing `miauw-base-service-1.7.1.tar` & `miauw-base-service-1.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/email_worker.py
--rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/exceptions.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2134 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2168 2023-07-16 08:29:23.000000 miauw-base-service-1.7.1/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      360 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 11:48:03.000000 miauw-base-service-1.7.1/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 11:48:03.698009 miauw-base-service-1.7.1/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 11:46:05.000000 miauw-base-service-1.7.1/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 14:32:47.791130 miauw-base-service-1.7.2/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.7.2/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.7.2/base_service/email_worker.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.7.2/base_service/exceptions.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2134 2023-07-16 14:27:13.000000 miauw-base-service-1.7.2/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2317 2023-07-16 14:32:21.000000 miauw-base-service-1.7.2/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      360 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 14:32:47.000000 miauw-base-service-1.7.2/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 14:32:21.000000 miauw-base-service-1.7.2/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 14:32:47.794463 miauw-base-service-1.7.2/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 14:32:21.000000 miauw-base-service-1.7.2/setup.py
```

### Comparing `miauw-base-service-1.7.1/base_service/email_worker.py` & `miauw-base-service-1.7.2/base_service/email_worker.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.7.1/base_service/exceptions.py` & `miauw-base-service-1.7.2/base_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.7.1/base_service/service.py` & `miauw-base-service-1.7.2/base_service/service.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.7.1/base_service/worker.py` & `miauw-base-service-1.7.2/base_service/worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,20 @@
     async def setup(self, chan_id: int | None = None) -> "RabbitMQWorker":
         """setup worker"""
         self.connection = await aio_pika.connect(self.url)
         self.channel = await self.connection.channel(channel_number=chan_id)
         self.ex = self.channel.default_exchange
         return self
 
-    async def send_basic(self, queue_name: str, data: bytes) -> None:
+    async def send(self, queue_name: str, data: dict | str | bytes) -> None:
         """sends something to queue"""
+        try:
+            data = json.loads(message.body)
+        except json.JSONDecodeError:
+            data = message.body.decode("utf-8")
         await self.ex.publish(aio_pika.Message(data), routing_key=queue_name)
 
     async def listen(
         self, queue_name: str, worker_function: Callable[[Any], Awaitable[Any]]
     ):
         await self.setup()
         queue = await self.channel.declare_queue(queue_name)
```

