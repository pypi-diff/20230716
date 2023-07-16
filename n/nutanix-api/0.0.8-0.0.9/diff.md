# Comparing `tmp/nutanix-api-0.0.8.tar.gz` & `tmp/nutanix-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutanix-api-0.0.8.tar", last modified: Fri Aug  5 08:32:39 2022, max compression
+gzip compressed data, was "nutanix-api-0.0.9.tar", last modified: Fri Aug  5 10:14:25 2022, max compression
```

## Comparing `nutanix-api-0.0.8.tar` & `nutanix-api-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:32:39.487253 nutanix-api-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-08-05 08:32:39.487253 nutanix-api-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 08:32:39.487253 nutanix-api-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:32:39.483253 nutanix-api-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:32:39.487253 nutanix-api-0.0.8/src/nutanix_api/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/src/nutanix_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/src/nutanix_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/src/nutanix_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/src/nutanix_api/api_object.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/src/nutanix_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/src/nutanix_api/nutanix_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/src/nutanix_api/nutanix_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:32:39.487253 nutanix-api-0.0.8/src/nutanix_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-08-05 08:32:39.000000 nutanix-api-0.0.8/src/nutanix_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-08-05 08:32:39.000000 nutanix-api-0.0.8/src/nutanix_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 08:32:39.000000 nutanix-api-0.0.8/src/nutanix_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-05 08:32:39.000000 nutanix-api-0.0.8/src/nutanix_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-05 08:32:39.000000 nutanix-api-0.0.8/src/nutanix_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-05 08:32:16.000000 nutanix-api-0.0.8/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-05 08:32:39.000000 nutanix-api-0.0.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:14:25.431207 nutanix-api-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-08-05 10:14:25.431207 nutanix-api-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 10:14:25.431207 nutanix-api-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:14:25.431207 nutanix-api-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:14:25.431207 nutanix-api-0.0.9/src/nutanix_api/
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/src/nutanix_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/src/nutanix_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/src/nutanix_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/src/nutanix_api/api_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/src/nutanix_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/src/nutanix_api/nutanix_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/src/nutanix_api/nutanix_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:14:25.431207 nutanix-api-0.0.9/src/nutanix_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-08-05 10:14:25.000000 nutanix-api-0.0.9/src/nutanix_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-08-05 10:14:25.000000 nutanix-api-0.0.9/src/nutanix_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 10:14:25.000000 nutanix-api-0.0.9/src/nutanix_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-05 10:14:25.000000 nutanix-api-0.0.9/src/nutanix_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-05 10:14:25.000000 nutanix-api-0.0.9/src/nutanix_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-05 10:14:05.000000 nutanix-api-0.0.9/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-05 10:14:25.000000 nutanix-api-0.0.9/version.txt
```

### Comparing `nutanix-api-0.0.8/LICENSE` & `nutanix-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nutanix-api-0.0.8/PKG-INFO` & `nutanix-api-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutanix-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for interact with v3 Nutanix API
 Home-page: https://github.com/eliorerz/nutanix_api
 Author: Elior Erez
 Author-email: elior123@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nutanix-api-0.0.8/README.md` & `nutanix-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nutanix-api-0.0.8/setup.py` & `nutanix-api-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `nutanix-api-0.0.8/src/nutanix_api/api_client.py` & `nutanix-api-0.0.9/src/nutanix_api/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import warnings
 from http import HTTPStatus
 from typing import Any, Callable, Dict, Union
 
 import requests
 from requests import Session
-from urllib3.exceptions import InsecureRequestWarning, RequestError
+from urllib3.exceptions import InsecureRequestWarning
+
+from .exceptions import RequestError
 
 
 class NutanixSession:
     HEADERS = {"Content-Type": "application/json", "charset": "utf-8"}
 
     def __init__(self, username: str, password: str, insecure: bool = True):
         session = requests.Session()
@@ -29,24 +31,25 @@
 
         self._session.close()
         return self
 
 
 class NutanixApiClient:
     URL_FORMAT = "https://{address}:{port}/api/nutanix/v3/"  # noqa FS003
+    DEFAULT_REQUEST_TIMEOUT = 60
 
     def __init__(self, username: str, password: str, port: Union[str, int], address: str):
         self._username = username
         self._password = password
         self._port = int(port)
         self._url = self.URL_FORMAT.format(address=address, port=port)
 
     @classmethod
-    def _request(cls, url: str, method: Callable, body: Dict[str, Any] = None):
-        server_response = method(url) if body is None else method(url, json=body)
+    def _request(cls, url: str, method: Callable, body: Dict[str, Any] = None, timeout=DEFAULT_REQUEST_TIMEOUT):
+        server_response = method(url, timeout=timeout) if body is None else method(url, json=body)
         if server_response.status_code != HTTPStatus.OK and server_response.status_code != HTTPStatus.ACCEPTED:
             raise RequestError(server_response.json())
 
         return server_response.json()
 
     def GET(self, relative_url: str) -> Union[Dict[str, Any], None]:  # noqa
         with NutanixSession(self._username, self._password) as session:
```

### Comparing `nutanix-api-0.0.8/src/nutanix_api/api_object.py` & `nutanix-api-0.0.9/src/nutanix_api/api_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,7 +84,16 @@
 
     def load(self, uuid: str) -> "ApiObject":
         vm = self.get(self._api_client, uuid)
         self._spec = vm.spec
         self._metadata = vm.metadata
         self._status = vm.status
         return self
+
+    @classmethod
+    def get_from_info(cls, api_client: NutanixApiClient, info: Dict[str, Any]) -> "ApiObject":
+        return cls(
+            api_client,
+            status=info.get("status", {}),
+            spec=info.get("spec", {}),
+            metadata=info.get("metadata", {}),
+        )
```

### Comparing `nutanix-api-0.0.8/src/nutanix_api/nutanix_cluster.py` & `nutanix-api-0.0.9/src/nutanix_api/nutanix_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,14 @@
         super().__init__(
             api_client,
             ClusterStatus(kwargs.get("status", {})),
             ClusterSpec(kwargs.get("spec", {})),
             ClusterMetadata(kwargs.get("metadata", {})),
         )
 
-        super().__init__(api_client, kwargs.get("status", {}), kwargs.get("spec", {}), kwargs.get("metadata", {}))
-
     @property
     def external_ip(self) -> str:
         return self.spec.external_ip
 
     @property
     def external_subnet(self) -> str:
         return self.spec.external_subnet
@@ -72,18 +70,13 @@
     @property
     def internal_subnet(self) -> str:
         return self.spec.internal_subnet
 
     @classmethod
     def get(cls, api_client: NutanixApiClient, uuid: str) -> "NutanixCluster":
         cluster_info = api_client.GET(f"/clusters/{uuid}")
-        return NutanixCluster(
-            api_client,
-            status=ClusterStatus(cluster_info.get("status", {})),
-            spec=ClusterSpec(cluster_info.get("spec", {})),
-            metadata=ClusterMetadata(cluster_info.get("metadata", {})),
-        )
+        return cls.get_from_info(api_client, cluster_info)
 
     @classmethod
     def list_clusters(cls, api_client: NutanixApiClient) -> List["NutanixCluster"]:
         clusters = api_client.POST("/clusters/list")
-        return [NutanixCluster(api_client, **cluster_info) for cluster_info in clusters["entities"]]
+        return [cls.get_from_info(api_client, cluster_info) for cluster_info in clusters["entities"]]
```

### Comparing `nutanix-api-0.0.8/src/nutanix_api/nutanix_vm.py` & `nutanix-api-0.0.9/src/nutanix_api/nutanix_vm.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,25 +109,20 @@
 
     @property
     def ip_addresses(self) -> List[str]:
         return self.spec.ip_endpoint_list
 
     @classmethod
     def list_vms(cls, api_client: NutanixApiClient) -> List["NutanixVM"]:
-        return [NutanixVM(api_client, **vm_info) for vm_info in api_client.POST("/vms/list")["entities"]]
+        return [cls.get_from_info(api_client, vm_info) for vm_info in api_client.POST("/vms/list")["entities"]]
 
     @classmethod
     def get(cls, api_client: NutanixApiClient, uuid: str) -> "NutanixVM":
         vm_info = api_client.GET(f"/vms/{uuid}")
-        return NutanixVM(
-            api_client,
-            status=VMStatus(vm_info.get("status", {})),
-            spec=VMSpec(vm_info.get("spec", {})),
-            metadata=VMMetadata(vm_info.get("metadata", {})),
-        )
+        return cls.get_from_info(api_client, vm_info)
 
     @classmethod
     def set_vms_power_state(cls, api_client: NutanixApiClient, uuid: str, state: PowerState):
         vm = cls.get(uuid)
         vm.power_state = state.value
 
         vm_info = vm.get_info()
```

### Comparing `nutanix-api-0.0.8/src/nutanix_api.egg-info/PKG-INFO` & `nutanix-api-0.0.9/src/nutanix_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutanix-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for interact with v3 Nutanix API
 Home-page: https://github.com/eliorerz/nutanix_api
 Author: Elior Erez
 Author-email: elior123@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

