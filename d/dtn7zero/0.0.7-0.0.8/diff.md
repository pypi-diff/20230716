# Comparing `tmp/dtn7zero-0.0.7.tar.gz` & `tmp/dtn7zero-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\dtn7zero\dist\.tmp-akzhq7gz\dtn7zero-0.0.7.tar", last modified: Thu Jul  6 13:00:37 2023, max compression
+gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\dtn7zero\dist\.tmp-2oy1uzw1\dtn7zero-0.0.8.tar", last modified: Sun Jul 16 12:06:01 2023, max compression
```

## Comparing `dtn7zero-0.0.7.tar` & `dtn7zero-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/
--rw-rw-rw-   0        0        0    35184 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/LICENSE
--rw-rw-rw-   0        0        0    10795 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    10470 2023-07-06 11:54:34.000000 dtn7zero-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/
--rw-rw-rw-   0        0        0      261 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/dtn7zero/__init__.py
--rw-rw-rw-   0        0        0     9886 2023-07-03 16:30:35.000000 dtn7zero-0.0.7/dtn7zero/api.py
--rw-rw-rw-   0        0        0    21220 2023-07-03 15:37:31.000000 dtn7zero-0.0.7/dtn7zero/bundle_protocol_agent.py
--rw-rw-rw-   0        0        0     2673 2023-07-03 16:28:59.000000 dtn7zero-0.0.7/dtn7zero/configuration.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/
--rw-rw-rw-   0        0        0      939 2023-06-21 11:49:23.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/__init__.py
--rw-rw-rw-   0        0        0     3311 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
--rw-rw-rw-   0        0        0     2124 2023-06-21 12:09:12.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/espnow_cla.py
--rw-rw-rw-   0        0        0    12993 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/mtcp.py
--rw-rw-rw-   0        0        0     2435 2023-07-06 12:35:47.000000 dtn7zero-0.0.7/dtn7zero/data.py
--rw-rw-rw-   0        0        0     7620 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/endpoints.py
--rw-rw-rw-   0        0        0    14821 2023-07-06 12:35:49.000000 dtn7zero-0.0.7/dtn7zero/ipnd.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/routers/
--rw-rw-rw-   0        0        0     3133 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/routers/__init__.py
--rw-rw-rw-   0        0        0     5115 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/routers/simple_epidemic_router.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/storage/
--rw-rw-rw-   0        0        0     1402 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/dtn7zero/storage/__init__.py
--rw-rw-rw-   0        0        0     2910 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/storage/simple_in_memory_storage.py
--rw-rw-rw-   0        0        0     4769 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/utility.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/
--rw-rw-rw-   0        0        0    10795 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      654 2023-07-06 11:59:17.000000 dtn7zero-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/test/
--rw-rw-rw-   0        0        0      960 2023-07-03 16:32:09.000000 dtn7zero-0.0.7/test/test-api-background.py
--rw-rw-rw-   0        0        0      698 2023-07-03 16:32:30.000000 dtn7zero-0.0.7/test/test-api-ping.py
--rw-rw-rw-   0        0        0      567 2023-07-03 16:32:43.000000 dtn7zero-0.0.7/test/test-api-pong.py
--rw-rw-rw-   0        0        0      903 2023-07-03 16:32:56.000000 dtn7zero-0.0.7/test/test-api-synchronous.py
--rw-rw-rw-   0        0        0     1940 2023-07-03 16:33:17.000000 dtn7zero-0.0.7/test/test-bundle-protocol-agent-receiver.py
--rw-rw-rw-   0        0        0     2091 2023-07-03 16:33:34.000000 dtn7zero-0.0.7/test/test-bundle-protocol-agent-sender.py
--rw-rw-rw-   0        0        0     1454 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/test/test-bundle-protocol-agent.py
--rw-rw-rw-   0        0        0     1711 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-bundle-serialization.py
--rw-rw-rw-   0        0        0    15498 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-bundle-size.py
--rw-rw-rw-   0        0        0     1745 2023-07-03 16:34:44.000000 dtn7zero-0.0.7/test/test-dtn7rs-rest-cla.py
--rw-rw-rw-   0        0        0     2049 2023-07-05 14:49:44.000000 dtn7zero-0.0.7/test/test-espnow-receiver.py
--rw-rw-rw-   0        0        0     2348 2023-07-05 14:49:40.000000 dtn7zero-0.0.7/test/test-espnow-sender.py
--rw-rw-rw-   0        0        0     1236 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-ipnd.py
--rw-rw-rw-   0        0        0     2114 2023-07-05 13:52:56.000000 dtn7zero-0.0.7/test/test-mtcp-intermediate.py
--rw-rw-rw-   0        0        0     2315 2023-07-03 16:37:33.000000 dtn7zero-0.0.7/test/test-mtcp-receiver.py
--rw-rw-rw-   0        0        0     2618 2023-07-03 16:37:33.000000 dtn7zero-0.0.7/test/test-mtcp-sender.py
--rw-rw-rw-   0        0        0     5282 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-py-dtn7-functionality.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/
+-rw-rw-rw-   0        0        0    35184 2023-04-28 22:29:12.000000 dtn7zero-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0    10795 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10470 2023-07-06 11:54:34.000000 dtn7zero-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero/
+-rw-rw-rw-   0        0        0      261 2023-04-28 22:29:12.000000 dtn7zero-0.0.8/dtn7zero/__init__.py
+-rw-rw-rw-   0        0        0     9886 2023-07-03 16:30:35.000000 dtn7zero-0.0.8/dtn7zero/api.py
+-rw-rw-rw-   0        0        0    21336 2023-07-10 14:15:57.000000 dtn7zero-0.0.8/dtn7zero/bundle_protocol_agent.py
+-rw-rw-rw-   0        0        0     2719 2023-07-10 13:01:33.000000 dtn7zero-0.0.8/dtn7zero/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/
+-rw-rw-rw-   0        0        0      939 2023-06-21 11:49:23.000000 dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/__init__.py
+-rw-rw-rw-   0        0        0     3311 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
+-rw-rw-rw-   0        0        0     2124 2023-07-10 14:54:52.000000 dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/espnow_cla.py
+-rw-rw-rw-   0        0        0    12993 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/mtcp.py
+-rw-rw-rw-   0        0        0     2435 2023-07-06 12:35:47.000000 dtn7zero-0.0.8/dtn7zero/data.py
+-rw-rw-rw-   0        0        0     7620 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/dtn7zero/endpoints.py
+-rw-rw-rw-   0        0        0    14825 2023-07-10 14:19:41.000000 dtn7zero-0.0.8/dtn7zero/ipnd.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero/routers/
+-rw-rw-rw-   0        0        0     3133 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/dtn7zero/routers/__init__.py
+-rw-rw-rw-   0        0        0     5115 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/dtn7zero/routers/simple_epidemic_router.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero/storage/
+-rw-rw-rw-   0        0        0     1402 2023-04-28 22:29:12.000000 dtn7zero-0.0.8/dtn7zero/storage/__init__.py
+-rw-rw-rw-   0        0        0     2910 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/dtn7zero/storage/simple_in_memory_storage.py
+-rw-rw-rw-   0        0        0     4769 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/dtn7zero/utility.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero.egg-info/
+-rw-rw-rw-   0        0        0    10795 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/dtn7zero.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      654 2023-07-16 12:04:33.000000 dtn7zero-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 12:06:01.000000 dtn7zero-0.0.8/test/
+-rw-rw-rw-   0        0        0      960 2023-07-03 16:32:09.000000 dtn7zero-0.0.8/test/test-api-background.py
+-rw-rw-rw-   0        0        0      698 2023-07-03 16:32:30.000000 dtn7zero-0.0.8/test/test-api-ping.py
+-rw-rw-rw-   0        0        0      567 2023-07-03 16:32:43.000000 dtn7zero-0.0.8/test/test-api-pong.py
+-rw-rw-rw-   0        0        0      903 2023-07-03 16:32:56.000000 dtn7zero-0.0.8/test/test-api-synchronous.py
+-rw-rw-rw-   0        0        0     1940 2023-07-03 16:33:17.000000 dtn7zero-0.0.8/test/test-bundle-protocol-agent-receiver.py
+-rw-rw-rw-   0        0        0     2091 2023-07-03 16:33:34.000000 dtn7zero-0.0.8/test/test-bundle-protocol-agent-sender.py
+-rw-rw-rw-   0        0        0     1454 2023-06-23 13:58:42.000000 dtn7zero-0.0.8/test/test-bundle-protocol-agent.py
+-rw-rw-rw-   0        0        0     1711 2023-04-28 22:29:12.000000 dtn7zero-0.0.8/test/test-bundle-serialization.py
+-rw-rw-rw-   0        0        0    15498 2023-04-28 22:29:12.000000 dtn7zero-0.0.8/test/test-bundle-size.py
+-rw-rw-rw-   0        0        0     1745 2023-07-03 16:34:44.000000 dtn7zero-0.0.8/test/test-dtn7rs-rest-cla.py
+-rw-rw-rw-   0        0        0     2049 2023-07-05 14:49:44.000000 dtn7zero-0.0.8/test/test-espnow-receiver.py
+-rw-rw-rw-   0        0        0     2348 2023-07-05 14:49:40.000000 dtn7zero-0.0.8/test/test-espnow-sender.py
+-rw-rw-rw-   0        0        0     1236 2023-04-28 22:29:12.000000 dtn7zero-0.0.8/test/test-ipnd.py
+-rw-rw-rw-   0        0        0     2114 2023-07-05 13:52:56.000000 dtn7zero-0.0.8/test/test-mtcp-intermediate.py
+-rw-rw-rw-   0        0        0     2315 2023-07-03 16:37:33.000000 dtn7zero-0.0.8/test/test-mtcp-receiver.py
+-rw-rw-rw-   0        0        0     2618 2023-07-03 16:37:33.000000 dtn7zero-0.0.8/test/test-mtcp-sender.py
+-rw-rw-rw-   0        0        0     5282 2023-04-28 22:29:12.000000 dtn7zero-0.0.8/test/test-py-dtn7-functionality.py
```

### Comparing `dtn7zero-0.0.7/LICENSE` & `dtn7zero-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/PKG-INFO` & `dtn7zero-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.7
+Version: 0.0.8
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/dtn7/dtn7zero
 Project-URL: Repository, https://github.com/dtn7/dtn7zero
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dtn7zero-0.0.7/README.md` & `dtn7zero-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/api.py` & `dtn7zero-0.0.8/dtn7zero/api.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/bundle_protocol_agent.py` & `dtn7zero-0.0.8/dtn7zero/bundle_protocol_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,24 +31,26 @@
         self.local_registered_endpoints: Dict[str, List[_LocalEndpoint]] = {}
 
         self.local_bundle_dispatch_queue: List[BundleInformation] = []  # this pipeline-stage is needed to prevent infinite-recursion if two local endpoints answer each other on every reception-callback
         self.storage_retry_generator = None
         self.router_poll_generator = None
 
         # on micropython we need to handle wireless connections manually
-        if RUNNING_MICROPYTHON and not isconnected():
-            connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
+        if RUNNING_MICROPYTHON and CONFIGURATION.MICROPYTHON_CHECK_WIFI:
+            if not isconnected():
+                connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
 
         scheme_encoded, node_encoded = PrimaryBlock.from_full_uri(full_node_uri)
         self.ipnd = IPND(scheme_encoded, node_encoded, storage)
 
     def update(self):
         # on micropython we need to handle wireless connections manually
-        if RUNNING_MICROPYTHON and not isconnected():
-            connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
+        if RUNNING_MICROPYTHON and CONFIGURATION.MICROPYTHON_CHECK_WIFI:
+            if not isconnected():
+                connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
 
         # update discovery
         self.ipnd.update()
 
         # process stored/delayed bundle
         if self.storage_retry_generator is None:
             self.storage_retry_generator = self.storage.get_bundles_to_retry()
```

### Comparing `dtn7zero-0.0.7/dtn7zero/configuration.py` & `dtn7zero-0.0.8/dtn7zero/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         self.IPND: _SubConfigurationIPND = _SubConfigurationIPND()
         self.MTCP: _SubConfigurationMTCP = _SubConfigurationMTCP()
         self.PORT: _SubConfigurationPORT = _SubConfigurationPORT()
 
         self.SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO = 3
         self.SOCKET_RECEIVE_BUFFER_SIZE = 512
 
+        self.MICROPYTHON_CHECK_WIFI = True
+
         if RUNNING_MICROPYTHON:
             self.SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES = 7  # experimental setting
             self.SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS = 18  # experimental setting
         else:
             self.SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES = 10000
             self.SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS = 100000
```

### Comparing `dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/__init__.py` & `dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py` & `dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/espnow_cla.py` & `dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/espnow_cla.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/mtcp.py` & `dtn7zero-0.0.8/dtn7zero/convergence_layer_adapters/mtcp.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/data.py` & `dtn7zero-0.0.8/dtn7zero/data.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/endpoints.py` & `dtn7zero-0.0.8/dtn7zero/endpoints.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/ipnd.py` & `dtn7zero-0.0.8/dtn7zero/ipnd.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         if CONFIGURATION.IPND.INTERFACE_WHITELIST:
             raise Exception("IPND interface whitelist is not supported on Micropython, list: {}".format(CONFIGURATION.IPND.INTERFACE_WHITELIST))
 
         address, subnet, _, _ = wlan.ifconfig()
 
         if address == '0.0.0.0':
             warning('wlan is not connected, cannot form broadcast address')
-            return []
+            return [], []
 
         return [build_broadcast_ipv4_address(address, subnet)], [address]
 
     @staticmethod
     def get_cpython_ipv4_broadcast_addresses() -> (list, list):
         broadcast_addresses = []
         own_addresses = []
```

### Comparing `dtn7zero-0.0.7/dtn7zero/routers/__init__.py` & `dtn7zero-0.0.8/dtn7zero/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/routers/simple_epidemic_router.py` & `dtn7zero-0.0.8/dtn7zero/routers/simple_epidemic_router.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/storage/__init__.py` & `dtn7zero-0.0.8/dtn7zero/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/storage/simple_in_memory_storage.py` & `dtn7zero-0.0.8/dtn7zero/storage/simple_in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero/utility.py` & `dtn7zero-0.0.8/dtn7zero/utility.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/dtn7zero.egg-info/PKG-INFO` & `dtn7zero-0.0.8/dtn7zero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.7
+Version: 0.0.8
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/dtn7/dtn7zero
 Project-URL: Repository, https://github.com/dtn7/dtn7zero
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dtn7zero-0.0.7/dtn7zero.egg-info/SOURCES.txt` & `dtn7zero-0.0.8/dtn7zero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/pyproject.toml` & `dtn7zero-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtn7zero"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name = "Lukas Holst", email = "lh700@proton.me"},
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "AGPL-3.0"}
 dependencies = [
     "requests >= 2.27.1",
     "cbor2",
     "netifaces",
-    "py-dtn7 >= 0.3.0a1"
+    "py-dtn7 == 0.3.0b1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dtn7/dtn7zero"
 "Repository" = "https://github.com/dtn7/dtn7zero"
 
 [tool.setuptools]
```

### Comparing `dtn7zero-0.0.7/test/test-api-background.py` & `dtn7zero-0.0.8/test/test-api-background.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-api-ping.py` & `dtn7zero-0.0.8/test/test-api-ping.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-api-pong.py` & `dtn7zero-0.0.8/test/test-api-pong.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-api-synchronous.py` & `dtn7zero-0.0.8/test/test-api-synchronous.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-bundle-protocol-agent-receiver.py` & `dtn7zero-0.0.8/test/test-bundle-protocol-agent-receiver.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-bundle-protocol-agent-sender.py` & `dtn7zero-0.0.8/test/test-bundle-protocol-agent-sender.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-bundle-protocol-agent.py` & `dtn7zero-0.0.8/test/test-bundle-protocol-agent.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-bundle-serialization.py` & `dtn7zero-0.0.8/test/test-bundle-serialization.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-bundle-size.py` & `dtn7zero-0.0.8/test/test-bundle-size.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-dtn7rs-rest-cla.py` & `dtn7zero-0.0.8/test/test-dtn7rs-rest-cla.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-espnow-receiver.py` & `dtn7zero-0.0.8/test/test-espnow-receiver.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-espnow-sender.py` & `dtn7zero-0.0.8/test/test-espnow-sender.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-ipnd.py` & `dtn7zero-0.0.8/test/test-ipnd.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-mtcp-intermediate.py` & `dtn7zero-0.0.8/test/test-mtcp-intermediate.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-mtcp-receiver.py` & `dtn7zero-0.0.8/test/test-mtcp-receiver.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-mtcp-sender.py` & `dtn7zero-0.0.8/test/test-mtcp-sender.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.7/test/test-py-dtn7-functionality.py` & `dtn7zero-0.0.8/test/test-py-dtn7-functionality.py`

 * *Files identical despite different names*

