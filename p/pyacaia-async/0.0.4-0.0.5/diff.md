# Comparing `tmp/pyacaia_async-0.0.4.tar.gz` & `tmp/pyacaia_async-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacaia_async-0.0.4.tar", last modified: Sat Jul 15 09:41:28 2023, max compression
+gzip compressed data, was "pyacaia_async-0.0.5.tar", last modified: Sun Jul 16 06:09:07 2023, max compression
```

## Comparing `pyacaia_async-0.0.4.tar` & `pyacaia_async-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/pyacaia_async/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/acaiascale.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/pyacaia_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/pyacaia_async/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/acaiascale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/pyacaia_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/setup.py
```

### Comparing `pyacaia_async-0.0.4/LICENSE` & `pyacaia_async-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.4/PKG-INFO` & `pyacaia_async-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia_async
-Version: 0.0.4
+Version: 0.0.5
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -40,13 +40,13 @@
 In that callback you will either receive objects of type `Message` or `Settings`. A sample notification handler can look like this and can also be found in `decode.py`
 
 ```python
 def notification_handler(sender, data) -> None:
     msg = decode(data)[0]
     if isinstance(msg, Settings):
         print(f"Battery: {msg.battery}")
-        print(f"Unit: {msg.unit}")
+        print(f"Unit: {msg.units}")
     elif isinstance(msg, Message):
         print(f"Weight: {msg.value}")
 
 scale = await AcaiaScale.create(mac=address, callback=notification_handler)
 ```
```

### Comparing `pyacaia_async-0.0.4/README.md` & `pyacaia_async-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 In that callback you will either receive objects of type `Message` or `Settings`. A sample notification handler can look like this and can also be found in `decode.py`
 
 ```python
 def notification_handler(sender, data) -> None:
     msg = decode(data)[0]
     if isinstance(msg, Settings):
         print(f"Battery: {msg.battery}")
-        print(f"Unit: {msg.unit}")
+        print(f"Unit: {msg.units}")
     elif isinstance(msg, Message):
         print(f"Weight: {msg.value}")
 
 scale = await AcaiaScale.create(mac=address, callback=notification_handler)
 ```
```

### Comparing `pyacaia_async-0.0.4/pyacaia_async/acaiascale.py` & `pyacaia_async-0.0.5/pyacaia_async/acaiascale.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,27 +160,27 @@
 
         await self._queue.put((
                 DEFAULT_CHAR_ID,
                 self.msg_types["notificationRequest"]
         ))
 
 
-    async def _send_heartbeats(self) -> None:
+    async def _send_heartbeats(self, interval:int=HEARTBEAT_INTERVAL) -> None:
         """ Task to send heartbeats in the background. """
         while True:
             try:
                 if not self._connected or self._disconnecting:
                     return
                 
                 _LOGGER.debug("Sending heartbeat.")
                 await self._queue.put((
                         DEFAULT_CHAR_ID, 
                         self.msg_types["heartbeat"]
                     ))
-                await asyncio.sleep(HEARTBEAT_INTERVAL)
+                await asyncio.sleep(interval)
             except asyncio.CancelledError:
                 return
             except Exception as ex:
                 _LOGGER.debug("Error sending heartbeat: %s", ex)
                 return
 
     async def disconnect(self) -> None:
```

### Comparing `pyacaia_async-0.0.4/pyacaia_async/decode.py` & `pyacaia_async-0.0.5/pyacaia_async/decode.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.4/pyacaia_async/helpers.py` & `pyacaia_async-0.0.5/pyacaia_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.4/pyacaia_async.egg-info/PKG-INFO` & `pyacaia_async-0.0.5/pyacaia_async.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia-async
-Version: 0.0.4
+Version: 0.0.5
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -40,13 +40,13 @@
 In that callback you will either receive objects of type `Message` or `Settings`. A sample notification handler can look like this and can also be found in `decode.py`
 
 ```python
 def notification_handler(sender, data) -> None:
     msg = decode(data)[0]
     if isinstance(msg, Settings):
         print(f"Battery: {msg.battery}")
-        print(f"Unit: {msg.unit}")
+        print(f"Unit: {msg.units}")
     elif isinstance(msg, Message):
         print(f"Weight: {msg.value}")
 
 scale = await AcaiaScale.create(mac=address, callback=notification_handler)
 ```
```

### Comparing `pyacaia_async-0.0.4/setup.py` & `pyacaia_async-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="pyacaia_async",
-    version="0.0.4",
+    version="0.0.5",
     description="An async implementation of PyAcaia",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pyacaia_async",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

