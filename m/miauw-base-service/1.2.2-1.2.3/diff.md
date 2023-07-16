# Comparing `tmp/miauw-base-service-1.2.2.tar.gz` & `tmp/miauw-base-service-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.2.2.tar", last modified: Sun Jul 16 06:40:29 2023, max compression
+gzip compressed data, was "miauw-base-service-1.2.3.tar", last modified: Sun Jul 16 06:55:02 2023, max compression
```

## Comparing `miauw-base-service-1.2.2.tar` & `miauw-base-service-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:40:29.691739 miauw-base-service-1.2.2/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:40:29.688406 miauw-base-service-1.2.2/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:40:29.688406 miauw-base-service-1.2.2/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.2/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:33:12.000000 miauw-base-service-1.2.2/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2160 2023-07-16 06:39:24.000000 miauw-base-service-1.2.2/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:40:29.688406 miauw-base-service-1.2.2/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:40:29.000000 miauw-base-service-1.2.2/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:40:29.000000 miauw-base-service-1.2.2/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 06:40:29.000000 miauw-base-service-1.2.2/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 06:40:29.000000 miauw-base-service-1.2.2/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 06:40:29.000000 miauw-base-service-1.2.2/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:39:35.000000 miauw-base-service-1.2.2/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 06:40:29.691739 miauw-base-service-1.2.2/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 06:39:47.000000 miauw-base-service-1.2.2/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:55:02.845054 miauw-base-service-1.2.3/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.3/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:33:12.000000 miauw-base-service-1.2.3/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2157 2023-07-16 06:52:40.000000 miauw-base-service-1.2.3/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:53:27.000000 miauw-base-service-1.2.3/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 06:53:21.000000 miauw-base-service-1.2.3/setup.py
```

### Comparing `miauw-base-service-1.2.2/base_service/service.py` & `miauw-base-service-1.2.3/base_service/service.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.2.2/base_service/worker.py` & `miauw-base-service-1.2.3/base_service/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         queue = await self.channel.declare_queue(queue_name)
         async with queue.iterator() as qi:
             message: aio_pika.abc.AbstractMessage
             async for message in qi:
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
-                        if type(message.body) is dict:
+                        try:
                             data = json.loads(message.body)
-                        else:
+                        except json.JSONDecodeError:
                             data = str(message.body)
                         res = await worker_function(data)
                         await self.ex.publish(
                             aio_pika.Message(
                                 body=json.dumps(res).encode("utf-8"),
                                 correlation_id=message.correlation_id,
                             ),
```

