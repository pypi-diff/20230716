# Comparing `tmp/miauw-base-service-1.2.3.tar.gz` & `tmp/miauw-base-service-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.2.3.tar", last modified: Sun Jul 16 06:55:02 2023, max compression
+gzip compressed data, was "miauw-base-service-1.2.4.tar", last modified: Sun Jul 16 08:31:41 2023, max compression
```

## Comparing `miauw-base-service-1.2.3.tar` & `miauw-base-service-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:55:02.845054 miauw-base-service-1.2.3/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.3/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:33:12.000000 miauw-base-service-1.2.3/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2157 2023-07-16 06:52:40.000000 miauw-base-service-1.2.3/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 06:55:02.000000 miauw-base-service-1.2.3/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 06:53:27.000000 miauw-base-service-1.2.3/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 06:55:02.848387 miauw-base-service-1.2.3/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 06:53:21.000000 miauw-base-service-1.2.3/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 08:31:41.011596 miauw-base-service-1.2.4/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.2.4/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1874 2023-07-16 06:33:12.000000 miauw-base-service-1.2.4/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2168 2023-07-16 08:29:23.000000 miauw-base-service-1.2.4/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 08:31:41.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 08:31:40.000000 miauw-base-service-1.2.4/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 08:29:37.000000 miauw-base-service-1.2.4/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 08:31:41.014930 miauw-base-service-1.2.4/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 08:29:37.000000 miauw-base-service-1.2.4/setup.py
```

### Comparing `miauw-base-service-1.2.3/base_service/service.py` & `miauw-base-service-1.2.4/base_service/service.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.2.3/base_service/worker.py` & `miauw-base-service-1.2.4/base_service/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             async for message in qi:
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
                         try:
                             data = json.loads(message.body)
                         except json.JSONDecodeError:
-                            data = str(message.body)
+                            data = message.body.decode("utf-8")
                         res = await worker_function(data)
                         await self.ex.publish(
                             aio_pika.Message(
                                 body=json.dumps(res).encode("utf-8"),
                                 correlation_id=message.correlation_id,
                             ),
                             routing_key=message.reply_to,
```

