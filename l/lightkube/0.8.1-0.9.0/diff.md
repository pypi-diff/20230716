# Comparing `tmp/lightkube-0.8.1.tar.gz` & `tmp/lightkube-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lightkube-0.8.1.tar", last modified: Thu Oct 14 07:23:10 2021, max compression
+gzip compressed data, was "dist/lightkube-0.9.0.tar", last modified: Sun Nov 21 10:47:09 2021, max compression
```

## Comparing `lightkube-0.8.1.tar` & `lightkube-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 tribulat   (502) staff       (20)        0 2021-10-14 07:23:10.000000 lightkube-0.8.1/
--rw-r--r--   0 tribulat   (502) staff       (20)     1095 2020-12-22 16:57:17.000000 lightkube-0.8.1/LICENSE
--rw-r--r--   0 tribulat   (502) staff       (20)     5370 2021-10-14 07:23:10.000000 lightkube-0.8.1/PKG-INFO
--rw-r--r--   0 tribulat   (502) staff       (20)     3635 2021-08-06 20:30:00.000000 lightkube-0.8.1/README.md
-drwxr-xr-x   0 tribulat   (502) staff       (20)        0 2021-10-14 07:23:10.000000 lightkube-0.8.1/lightkube/
--rw-r--r--   0 tribulat   (502) staff       (20)      211 2021-05-13 09:26:55.000000 lightkube-0.8.1/lightkube/__init__.py
--rw-r--r--   0 tribulat   (502) staff       (20)     4307 2021-07-28 14:52:43.000000 lightkube-0.8.1/lightkube/codecs.py
-drwxr-xr-x   0 tribulat   (502) staff       (20)        0 2021-10-14 07:23:10.000000 lightkube-0.8.1/lightkube/config/
--rw-r--r--   0 tribulat   (502) staff       (20)     4608 2021-08-06 20:30:00.000000 lightkube-0.8.1/lightkube/config/client_adapter.py
--rw-r--r--   0 tribulat   (502) staff       (20)     8571 2020-12-22 16:57:17.000000 lightkube-0.8.1/lightkube/config/kubeconfig.py
--rw-r--r--   0 tribulat   (502) staff       (20)     1909 2020-12-22 16:57:17.000000 lightkube-0.8.1/lightkube/config/models.py
-drwxr-xr-x   0 tribulat   (502) staff       (20)        0 2021-10-14 07:23:10.000000 lightkube-0.8.1/lightkube/core/
--rw-r--r--   0 tribulat   (502) staff       (20)    25573 2021-08-06 20:30:00.000000 lightkube-0.8.1/lightkube/core/client.py
--rw-r--r--   0 tribulat   (502) staff       (20)     4771 2020-09-12 12:12:05.000000 lightkube-0.8.1/lightkube/core/dataclasses_dict.py
--rw-r--r--   0 tribulat   (502) staff       (20)      575 2021-08-06 20:30:00.000000 lightkube-0.8.1/lightkube/core/exceptions.py
--rw-r--r--   0 tribulat   (502) staff       (20)    10665 2021-10-14 07:20:25.000000 lightkube-0.8.1/lightkube/core/generic_client.py
--rw-r--r--   0 tribulat   (502) staff       (20)      436 2020-08-29 15:14:53.000000 lightkube-0.8.1/lightkube/core/internal_models.py
--rw-r--r--   0 tribulat   (502) staff       (20)      312 2021-01-08 18:34:16.000000 lightkube-0.8.1/lightkube/core/internal_resources.py
--rw-r--r--   0 tribulat   (502) staff       (20)      655 2020-09-16 19:56:42.000000 lightkube-0.8.1/lightkube/core/resource.py
--rw-r--r--   0 tribulat   (502) staff       (20)     1171 2020-09-26 08:37:29.000000 lightkube-0.8.1/lightkube/core/selector.py
--rw-r--r--   0 tribulat   (502) staff       (20)      594 2020-08-29 15:14:53.000000 lightkube-0.8.1/lightkube/core/typing_extra.py
--rw-r--r--   0 tribulat   (502) staff       (20)     5569 2021-05-13 09:26:55.000000 lightkube-0.8.1/lightkube/generic_resource.py
--rw-r--r--   0 tribulat   (502) staff       (20)     1154 2020-09-04 20:09:59.000000 lightkube-0.8.1/lightkube/operators.py
--rw-r--r--   0 tribulat   (502) staff       (20)      832 2020-09-16 20:25:19.000000 lightkube-0.8.1/lightkube/types.py
-drwxr-xr-x   0 tribulat   (502) staff       (20)        0 2021-10-14 07:23:10.000000 lightkube-0.8.1/lightkube.egg-info/
--rw-r--r--   0 tribulat   (502) staff       (20)     5370 2021-10-14 07:23:09.000000 lightkube-0.8.1/lightkube.egg-info/PKG-INFO
--rw-r--r--   0 tribulat   (502) staff       (20)      675 2021-10-14 07:23:09.000000 lightkube-0.8.1/lightkube.egg-info/SOURCES.txt
--rw-r--r--   0 tribulat   (502) staff       (20)        1 2021-10-14 07:23:09.000000 lightkube-0.8.1/lightkube.egg-info/dependency_links.txt
--rw-r--r--   0 tribulat   (502) staff       (20)      121 2021-10-14 07:23:09.000000 lightkube-0.8.1/lightkube.egg-info/requires.txt
--rw-r--r--   0 tribulat   (502) staff       (20)       10 2021-10-14 07:23:09.000000 lightkube-0.8.1/lightkube.egg-info/top_level.txt
--rw-r--r--   0 tribulat   (502) staff       (20)       38 2021-10-14 07:23:10.000000 lightkube-0.8.1/setup.cfg
--rw-r--r--   0 tribulat   (502) staff       (20)     1105 2021-10-14 07:21:01.000000 lightkube-0.8.1/setup.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2021-11-21 10:47:09.000000 lightkube-0.9.0/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1095 2020-12-22 16:57:17.000000 lightkube-0.9.0/LICENSE
+-rw-r--r--   0 tribulat   (501) staff       (20)     5370 2021-11-21 10:47:09.000000 lightkube-0.9.0/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)     3635 2021-08-06 20:30:00.000000 lightkube-0.9.0/README.md
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2021-11-21 10:47:09.000000 lightkube-0.9.0/lightkube/
+-rw-r--r--   0 tribulat   (501) staff       (20)      211 2021-05-13 09:26:55.000000 lightkube-0.9.0/lightkube/__init__.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     4307 2021-07-28 14:52:43.000000 lightkube-0.9.0/lightkube/codecs.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2021-11-21 10:47:09.000000 lightkube-0.9.0/lightkube/config/
+-rw-r--r--   0 tribulat   (501) staff       (20)     4608 2021-08-06 20:30:00.000000 lightkube-0.9.0/lightkube/config/client_adapter.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     8571 2020-12-22 16:57:17.000000 lightkube-0.9.0/lightkube/config/kubeconfig.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1909 2020-12-22 16:57:17.000000 lightkube-0.9.0/lightkube/config/models.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2021-11-21 10:47:09.000000 lightkube-0.9.0/lightkube/core/
+-rw-r--r--   0 tribulat   (501) staff       (20)    29975 2021-11-21 10:36:29.000000 lightkube-0.9.0/lightkube/core/client.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     4771 2020-09-12 12:12:05.000000 lightkube-0.9.0/lightkube/core/dataclasses_dict.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1122 2021-11-21 10:36:29.000000 lightkube-0.9.0/lightkube/core/exceptions.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10665 2021-10-14 07:20:25.000000 lightkube-0.9.0/lightkube/core/generic_client.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      436 2020-08-29 15:14:53.000000 lightkube-0.9.0/lightkube/core/internal_models.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      312 2021-01-08 18:34:16.000000 lightkube-0.9.0/lightkube/core/internal_resources.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      655 2020-09-16 19:56:42.000000 lightkube-0.9.0/lightkube/core/resource.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1171 2020-09-26 08:37:29.000000 lightkube-0.9.0/lightkube/core/selector.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      594 2020-08-29 15:14:53.000000 lightkube-0.9.0/lightkube/core/typing_extra.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5569 2021-05-13 09:26:55.000000 lightkube-0.9.0/lightkube/generic_resource.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1154 2020-09-04 20:09:59.000000 lightkube-0.9.0/lightkube/operators.py
+-rw-r--r--   0 tribulat   (501) staff       (20)        0 2020-12-22 16:57:17.000000 lightkube-0.9.0/lightkube/py.typed
+-rw-r--r--   0 tribulat   (501) staff       (20)      832 2020-09-16 20:25:19.000000 lightkube-0.9.0/lightkube/types.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2021-11-21 10:47:09.000000 lightkube-0.9.0/lightkube.egg-info/
+-rw-r--r--   0 tribulat   (501) staff       (20)     5370 2021-11-21 10:47:08.000000 lightkube-0.9.0/lightkube.egg-info/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)      694 2021-11-21 10:47:08.000000 lightkube-0.9.0/lightkube.egg-info/SOURCES.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)        1 2021-11-21 10:47:08.000000 lightkube-0.9.0/lightkube.egg-info/dependency_links.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)      121 2021-11-21 10:47:08.000000 lightkube-0.9.0/lightkube.egg-info/requires.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       10 2021-11-21 10:47:08.000000 lightkube-0.9.0/lightkube.egg-info/top_level.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       38 2021-11-21 10:47:09.000000 lightkube-0.9.0/setup.cfg
+-rw-r--r--   0 tribulat   (501) staff       (20)     1151 2021-11-21 10:44:48.000000 lightkube-0.9.0/setup.py
```

### Comparing `lightkube-0.8.1/LICENSE` & `lightkube-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/PKG-INFO` & `lightkube-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube
-Version: 0.8.1
+Version: 0.9.0
 Summary: Lightweight kubernetes client library
 Home-page: https://github.com/gtsystem/lightkube
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: MIT
 Description: # lightkube
```

### Comparing `lightkube-0.8.1/README.md` & `lightkube-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/codecs.py` & `lightkube-0.9.0/lightkube/codecs.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/config/client_adapter.py` & `lightkube-0.9.0/lightkube/config/client_adapter.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/config/kubeconfig.py` & `lightkube-0.9.0/lightkube/config/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/config/models.py` & `lightkube-0.9.0/lightkube/config/models.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/core/client.py` & `lightkube-0.9.0/lightkube/core/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Type, Iterator, TypeVar, Union, overload, Dict, Tuple, List, Iterable, AsyncIterable
 import httpx
 from ..config.kubeconfig import SingleConfig, KubeConfig
 from .. import operators
 from ..core import resource as r
 from .generic_client import GenericSyncClient, GenericAsyncClient
+from ..core.exceptions import ConditionError, ObjectDeleted
 from ..types import OnErrorHandler, PatchType, on_error_raise
 from .internal_resources import core_v1
 from .selector import build_selector
 
 NamespacedResource = TypeVar('NamespacedResource', bound=r.NamespacedResource)
 GlobalResource = TypeVar('GlobalResource', bound=r.GlobalResource)
 GlobalSubResource = TypeVar('GlobalSubResource', bound=r.GlobalSubResource)
@@ -173,14 +174,84 @@
                 'labelSelector': build_selector(labels) if labels else None,
                 'fieldSelector': build_selector(fields, for_fields=True) if fields else None
             }
         )
         return self._client.watch(br, on_error=on_error)
 
     @overload
+    def wait(
+        self,
+        res: Type[GlobalResource],
+        name: str,
+        *,
+        for_conditions: Iterable[str],
+        raise_for_conditions: Iterable[str] = (),
+    ) -> GlobalResource:
+        ...
+
+    @overload
+    def wait(
+        self,
+        res: Type[AllNamespacedResource],
+        name: str,
+        *,
+        for_conditions: Iterable[str],
+        namespace: str = None,
+        raise_for_conditions: Iterable[str] = (),
+    ) -> AllNamespacedResource:
+        ...
+
+    def wait(
+        self,
+        res,
+        name: str,
+        *,
+        for_conditions: Iterable[str],
+        namespace=None,
+        raise_for_conditions: Iterable[str] = (),
+    ):
+        """Waits for specified conditions.
+
+        **parameters**
+
+        * **res** - Resource kind.
+        * **name** - Name of resource to wait for.
+        * **for_conditions** - Condition types that are considered a success and will end the wait.
+        * **namespace** - *(optional)* Name of the namespace containing the object (Only for namespaced resources).
+        * **raise_for_conditions** - *(optional)* Condition types that are considered failures and will exit the wait early.
+        """
+
+        kind = r.api_info(res).plural
+        full_name = f'{kind}/{name}'
+
+        for_conditions = list(for_conditions)
+        raise_for_conditions = list(raise_for_conditions)
+
+        for op, obj in self.watch(res, namespace=namespace, fields={'metadata.name': name}):
+            if obj.status is None:
+                continue
+
+            if op == "DELETED":
+                raise ObjectDeleted(full_name)
+
+            try:
+                status = obj.status.to_dict()
+            except AttributeError:
+                status = obj.status
+
+            conditions = [c for c in status.get('conditions', []) if c['status'] == 'True']
+            if any(c['type'] in for_conditions for c in conditions):
+                return obj
+
+            failures = [c for c in conditions if c['type'] in raise_for_conditions]
+
+            if failures:
+                raise ConditionError(full_name, [f.get('message', f['type']) for f in failures])
+
+    @overload
     def patch(self, res: Type[GlobalSubResource], name: str,
               obj: Union[GlobalSubResource, Dict, List], *,
               patch_type: PatchType = PatchType.STRATEGIC) -> GlobalSubResource:
         ...
 
     @overload
     def patch(self, res: Type[GlobalResource], name: str,
@@ -444,14 +515,84 @@
                 'labelSelector': build_selector(labels) if labels else None,
                 'fieldSelector': build_selector(fields, for_fields=True) if fields else None
             }
         )
         return self._client.watch(br, on_error=on_error)
 
     @overload
+    async def wait(
+        self,
+        res: Type[GlobalResource],
+        name: str,
+        *,
+        for_conditions: Iterable[str],
+        raise_for_conditions: Iterable[str] = (),
+    ) -> GlobalResource:
+        ...
+
+    @overload
+    async def wait(
+        self,
+        res: Type[AllNamespacedResource],
+        name: str,
+        *,
+        for_conditions: Iterable[str],
+        namespace: str = None,
+        raise_for_conditions: Iterable[str] = (),
+    ) -> AllNamespacedResource:
+        ...
+
+    async def wait(
+        self,
+        res,
+        name: str,
+        *,
+        for_conditions: Iterable[str],
+        namespace=None,
+        raise_for_conditions: Iterable[str] = (),
+    ):
+        """Waits for specified conditions.
+
+        **parameters**
+
+        * **res** - Resource kind.
+        * **name** - Name of resource to wait for.
+        * **for_conditions** - Condition types that are considered a success and will end the wait.
+        * **namespace** - *(optional)* Name of the namespace containing the object (Only for namespaced resources).
+        * **raise_for_conditions** - *(optional)* Condition types that are considered failures and will exit the wait early.
+        """
+
+        kind = r.api_info(res).plural
+        full_name = f'{kind}/{name}'
+
+        for_conditions = list(for_conditions)
+        raise_for_conditions = list(raise_for_conditions)
+
+        async for op, obj in self.watch(res, namespace=namespace, fields={'metadata.name': name}):
+            if obj.status is None:
+                continue
+
+            if op == "DELETED":
+                raise ObjectDeleted(full_name)
+
+            try:
+                status = obj.status.to_dict()
+            except AttributeError:
+                status = obj.status
+
+            conditions = [c for c in status.get('conditions', []) if c['status'] == 'True']
+            if any(c['type'] in for_conditions for c in conditions):
+                return obj
+
+            failures = [c for c in conditions if c['type'] in raise_for_conditions]
+
+            if failures:
+                raise ConditionError(full_name, [f.get('message', f['type']) for f in failures])
+
+    @overload
     async def patch(self, res: Type[GlobalSubResource], name: str,
               obj: Union[GlobalSubResource, Dict, List], *,
               patch_type: PatchType = PatchType.STRATEGIC) -> GlobalSubResource:
         ...
 
     @overload
     async def patch(self, res: Type[GlobalResource], name: str,
```

### Comparing `lightkube-0.8.1/lightkube/core/dataclasses_dict.py` & `lightkube-0.9.0/lightkube/core/dataclasses_dict.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/core/exceptions.py` & `lightkube-0.9.0/lightkube/core/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,7 +22,33 @@
         super().__init__(self.status.message, request=request, response=response)
 
 
 class LoadResourceError(Exception):
     """
     Error in loading a resource
     """
+
+
+class ObjectDeleted(Exception):
+    """
+    Object was unexpectedly deleted
+    """
+
+    def __init__(self, name):
+        self.name = name
+
+    def __str__(self):
+        return f"{self.name} was unexpectedly deleted"
+
+
+class ConditionError(Exception):
+    """
+    Object is in specified bad condition
+    """
+
+    def __init__(self, name, messages):
+        self.name = name
+        self.messages = messages
+
+    def __str__(self):
+        messages = '; '.join(self.messages)
+        return f'{self.name} has failure condition(s): {messages}'
```

### Comparing `lightkube-0.8.1/lightkube/core/generic_client.py` & `lightkube-0.9.0/lightkube/core/generic_client.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/core/resource.py` & `lightkube-0.9.0/lightkube/core/resource.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/core/selector.py` & `lightkube-0.9.0/lightkube/core/selector.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/core/typing_extra.py` & `lightkube-0.9.0/lightkube/core/typing_extra.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/generic_resource.py` & `lightkube-0.9.0/lightkube/generic_resource.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/operators.py` & `lightkube-0.9.0/lightkube/operators.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube/types.py` & `lightkube-0.9.0/lightkube/types.py`

 * *Files identical despite different names*

### Comparing `lightkube-0.8.1/lightkube.egg-info/PKG-INFO` & `lightkube-0.9.0/lightkube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube
-Version: 0.8.1
+Version: 0.9.0
 Summary: Lightweight kubernetes client library
 Home-page: https://github.com/gtsystem/lightkube
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: MIT
 Description: # lightkube
```

### Comparing `lightkube-0.8.1/lightkube.egg-info/SOURCES.txt` & `lightkube-0.9.0/lightkube.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 lightkube/__init__.py
 lightkube/codecs.py
 lightkube/generic_resource.py
 lightkube/operators.py
+lightkube/py.typed
 lightkube/types.py
 lightkube.egg-info/PKG-INFO
 lightkube.egg-info/SOURCES.txt
 lightkube.egg-info/dependency_links.txt
 lightkube.egg-info/requires.txt
 lightkube.egg-info/top_level.txt
 lightkube/config/client_adapter.py
```

### Comparing `lightkube-0.8.1/setup.py` & `lightkube-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name='lightkube',
-    version="0.8.1",
+    version="0.9.0",
     description='Lightweight kubernetes client library',
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author='Giuseppe Tribulato',
     author_email='gtsystem@gmail.com',
     license='MIT',
     url='https://github.com/gtsystem/lightkube',
     packages=['lightkube', 'lightkube.config', 'lightkube.core'],
+    package_data={'lightkube': ['py.typed']},
     install_requires=[
         'lightkube-models >= 1.15.12.0',
         'httpx >= 0.20.0',
         'PyYAML',
         'backports-datetime-fromisoformat;python_version<"3.7"',
         'dataclasses;python_version<"3.7"'
     ],
```

