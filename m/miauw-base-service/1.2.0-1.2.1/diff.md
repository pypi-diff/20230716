# Comparing `tmp/miauw-base-service-1.2.0.tar.gz` & `tmp/miauw-base-service-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.2.0.tar", last modified: Sun Jul 16 06:12:18 2023, max compression
+gzip compressed data, was "miauw-base-service-1.2.1.tar", last modified: Sun Jul 16 06:36:38 2023, max compression
```

## Comparing `miauw-base-service-1.2.0.tar` & `miauw-base-service-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.0/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:01:40.000000 miauw-base-service-1.2.0/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2144 2023-07-16 06:06:59.000000 miauw-base-service-1.2.0/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 06:12:18.000000 miauw-base-service-1.2.0/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:07:28.000000 miauw-base-service-1.2.0/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 06:12:18.725108 miauw-base-service-1.2.0/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 06:07:28.000000 miauw-base-service-1.2.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:36:38.365077 miauw-base-service-1.2.1/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:36:38.365077 miauw-base-service-1.2.1/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:36:38.365077 miauw-base-service-1.2.1/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.1/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:33:12.000000 miauw-base-service-1.2.1/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2152 2023-07-16 06:33:12.000000 miauw-base-service-1.2.1/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:36:38.365077 miauw-base-service-1.2.1/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:36:38.000000 miauw-base-service-1.2.1/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:36:38.000000 miauw-base-service-1.2.1/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 06:36:38.000000 miauw-base-service-1.2.1/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 06:36:38.000000 miauw-base-service-1.2.1/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 06:36:38.000000 miauw-base-service-1.2.1/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:33:12.000000 miauw-base-service-1.2.1/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 06:36:38.365077 miauw-base-service-1.2.1/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 06:33:12.000000 miauw-base-service-1.2.1/setup.py
```

### Comparing `miauw-base-service-1.2.0/base_service/service.py` & `miauw-base-service-1.2.1/base_service/service.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.2.0/base_service/worker.py` & `miauw-base-service-1.2.1/base_service/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         queue = await self.channel.declare_queue(queue_name)
         async with queue.iterator() as qi:
             message: aio_pika.abc.AbstractMessage
             async for message in qi:
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
-                        if type(data) is dict:
+                        if type(message.body) is dict:
                             data = json.loads(message.body)
                         else:
                             data = str(data)
                         res = await worker_function(data)
                         await self.ex.publish(
                             aio_pika.Message(
                                 body=json.dumps(res).encode("utf-8"),
```

