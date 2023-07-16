# Comparing `tmp/aioabcpapi-2.0.5.tar.gz` & `tmp/aioabcpapi-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-2.0.5.tar", last modified: Sat Jul 15 20:06:51 2023, max compression
+gzip compressed data, was "aioabcpapi-2.0.6.tar", last modified: Sun Jul 16 18:03:00 2023, max compression
```

## Comparing `aioabcpapi-2.0.5.tar` & `aioabcpapi-2.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.484546 aioabcpapi-2.0.5/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.5/LICENSE
--rw-rw-rw-   0        0        0     5371 2023-07-15 20:06:51.485547 aioabcpapi-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.400529 aioabcpapi-2.0.5/aioabcpapi/
--rw-rw-rw-   0        0        0      530 2023-07-15 20:06:01.000000 aioabcpapi-2.0.5/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.5/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    20655 2023-07-15 19:33:16.000000 aioabcpapi-2.0.5/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.5/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.444536 aioabcpapi-2.0.5/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.5/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   114141 2023-07-15 20:04:31.000000 aioabcpapi-2.0.5/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.5/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.5/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.5/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.453539 aioabcpapi-2.0.5/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.5/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   126277 2023-07-15 18:59:44.000000 aioabcpapi-2.0.5/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.5/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    47055 2023-07-15 18:54:00.000000 aioabcpapi-2.0.5/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.468541 aioabcpapi-2.0.5/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.5/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.5/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.5/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.419534 aioabcpapi-2.0.5/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5371 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-07-15 20:06:51.487549 aioabcpapi-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-07-15 20:06:01.000000 aioabcpapi-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.482545 aioabcpapi-2.0.5/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.5/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:03:00.829148 aioabcpapi-2.0.6/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5371 2023-07-16 18:03:00.829148 aioabcpapi-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 18:03:00.716123 aioabcpapi-2.0.6/aioabcpapi/
+-rw-rw-rw-   0        0        0      530 2023-07-16 18:01:38.000000 aioabcpapi-2.0.6/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.6/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    20655 2023-07-15 19:33:16.000000 aioabcpapi-2.0.6/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.6/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:03:00.782138 aioabcpapi-2.0.6/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.6/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   114141 2023-07-15 20:04:31.000000 aioabcpapi-2.0.6/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.6/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.6/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.6/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:03:00.796143 aioabcpapi-2.0.6/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.6/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   126500 2023-07-16 12:15:07.000000 aioabcpapi-2.0.6/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.6/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    47189 2023-07-16 10:26:02.000000 aioabcpapi-2.0.6/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:03:00.814143 aioabcpapi-2.0.6/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.6/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.6/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.6/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:03:00.745129 aioabcpapi-2.0.6/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5371 2023-07-16 18:03:00.000000 aioabcpapi-2.0.6/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-07-16 18:03:00.000000 aioabcpapi-2.0.6/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 18:03:00.000000 aioabcpapi-2.0.6/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-16 18:03:00.000000 aioabcpapi-2.0.6/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-07-16 18:03:00.000000 aioabcpapi-2.0.6/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-07-16 18:03:00.836149 aioabcpapi-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-07-16 18:01:38.000000 aioabcpapi-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:03:00.827147 aioabcpapi-2.0.6/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.6/test/test_payload.py
```

### Comparing `aioabcpapi-2.0.5/LICENSE` & `aioabcpapi-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/PKG-INFO` & `aioabcpapi-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.5
+Version: 2.0.6
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.5/README.md` & `aioabcpapi-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/__init__.py` & `aioabcpapi-2.0.6/aioabcpapi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,9 +5,9 @@
                          AbcpParameterRequired, TeaPot)
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 
 __author__ = 'bl4ckm45k'
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 __email__ = 'nonpowa@gmail.com'
```

### Comparing `aioabcpapi-2.0.5/aioabcpapi/abcp.py` & `aioabcpapi-2.0.6/aioabcpapi/abcp.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/api.py` & `aioabcpapi-2.0.6/aioabcpapi/api.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/base.py` & `aioabcpapi-2.0.6/aioabcpapi/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/cp/admin.py` & `aioabcpapi-2.0.6/aioabcpapi/cp/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/cp/client.py` & `aioabcpapi-2.0.6/aioabcpapi/cp/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/exceptions.py` & `aioabcpapi-2.0.6/aioabcpapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/ts/admin.py` & `aioabcpapi-2.0.6/aioabcpapi/ts/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,14 +705,15 @@
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.TsAdmin.DistributorOwners.DISTRIBUTOR_OWNERS, payload)
 
 
 class Orders:
     def __init__(self, base: BaseAbcp):
         self._base = base
+        self.messages = Messages(base)
 
     class _FieldsChecker:
         fields = ["deliveries", "agreement", "tags", "posInfo", "amounts"]
 
     async def create(self, client_id: Union[str, int], number: Union[int, str] = None,
                      agreement_id: Union[int, str] = None,
                      create_time: Union[datetime, str] = None, manager_id: Union[int, str] = None,
@@ -1197,14 +1198,15 @@
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.TsAdmin.Cart.TRANSFER, payload, True)
 
 
 class Positions:
     def __init__(self, base: BaseAbcp):
         self._base = base
+        self.messages = PositionsMessages(base)
 
     class _FieldsChecker:
         additional_info = ["reserv", "product", "orderPicking",
                            "customerComplaintPoses", "supplierOrder", "grPosition",
                            "order", "delivery", "tags", "unpaidAmount"]
         statuses = ["prepayment", "canceled", "new",
                     "supOrder", "supOrderCanceled", "reservation",
@@ -2001,33 +2003,33 @@
         return await self._base.request(_Methods.TsAdmin.PaymentMethods.METHODS_LIST, payload)
 
 
 class Agreements:
     def __init__(self, base: BaseAbcp):
         self._base = base
 
-    async def get_list(self, contractor_ids: Union[int, List[int]] = None,
-                       contractor_requisite_ids: Union[int, List[int]] = None,
-                       shop_requisite_ids: Union[int, List[int]] = None,
+    async def get_list(self, contractor_ids: Union[int, str, List[int]] = None,
+                       contractor_requisite_ids: Union[int, str, List[int]] = None,
+                       shop_requisite_ids: Union[int, str, List[int]] = None,
                        is_active: bool = None, is_delete: bool = None, is_default: bool = None,
                        agreement_type: int = None, relation_type: int = None,
                        number: str = None, currency: str = None,
                        date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
                        credit_limit: Union[float, int] = None,
                        limit: int = None, skip: int = None):
         if isinstance(date_start, datetime):
             date_start = generate(date_start.replace(tzinfo=pytz.utc))
         if isinstance(date_end, datetime):
             date_end = generate(date_end.replace(tzinfo=pytz.utc))
 
-        if isinstance(contractor_ids, int):
+        if isinstance(contractor_ids, int) or isinstance(contractor_ids, str):
             contractor_ids = [contractor_ids]
-        if isinstance(contractor_requisite_ids, int):
+        if isinstance(contractor_requisite_ids, int) or isinstance(contractor_requisite_ids, str):
             contractor_requisite_ids = [contractor_requisite_ids]
-        if isinstance(shop_requisite_ids, int):
+        if isinstance(shop_requisite_ids, int) or isinstance(shop_requisite_ids, str):
             shop_requisite_ids = [shop_requisite_ids]
 
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.TsAdmin.Agreements.get_list, payload)
 
 
 class LegalPersons:
```

### Comparing `aioabcpapi-2.0.5/aioabcpapi/ts/base.py` & `aioabcpapi-2.0.6/aioabcpapi/ts/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/ts/client.py` & `aioabcpapi-2.0.6/aioabcpapi/ts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,30 +710,30 @@
         return await self._base.request(_Methods.TsClient.Positions.MASS_CANCEL, payload, True)
 
 
 class Agreements:
     def __init__(self, base: BaseAbcp):
         self._base = base
 
-    async def get_list(self, contractor_ids: Union[int, List[int]] = None,
-                       contractor_requisite_ids: Union[int, List[int]] = None,
-                       shop_requisite_ids: Union[int, List[int]] = None,
+    async def get_list(self, contractor_ids: Union[int, str, List[int]] = None,
+                       contractor_requisite_ids: Union[int, str, List[int]] = None,
+                       shop_requisite_ids: Union[int, str, List[int]] = None,
                        is_active: bool = None, is_delete: bool = None, is_default: bool = None,
                        agreement_type: int = None, relation_type: int = None,
                        number: str = None, currency: str = None,
                        date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
                        credit_limit: Union[float, int] = None,
                        limit: int = None, skip: int = None):
         if isinstance(date_start, datetime):
             date_start = generate(date_start.replace(tzinfo=pytz.utc))
         if isinstance(date_end, datetime):
             date_end = generate(date_end.replace(tzinfo=pytz.utc))
 
-        if isinstance(contractor_ids, int):
+        if isinstance(contractor_ids, int) or isinstance(contractor_ids, str):
             contractor_ids = [contractor_ids]
-        if isinstance(contractor_requisite_ids, int):
+        if isinstance(contractor_requisite_ids, int) or isinstance(contractor_requisite_ids, str):
             contractor_requisite_ids = [contractor_requisite_ids]
-        if isinstance(shop_requisite_ids, int):
+        if isinstance(shop_requisite_ids, int) or isinstance(shop_requisite_ids, str):
             shop_requisite_ids = [shop_requisite_ids]
 
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.TsClient.Agreements.get_list, payload)
```

### Comparing `aioabcpapi-2.0.5/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-2.0.6/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi/utils/payload.py` & `aioabcpapi-2.0.6/aioabcpapi/utils/payload.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-2.0.6/aioabcpapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.5
+Version: 2.0.6
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.5/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-2.0.6/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.5/setup.py` & `aioabcpapi-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 requirements = ["aiohttp>=3.8.3", "certifi>=2022.12.7", "ujson>=5.7.0", "pytz>=2022.7.1", "pyrfc3339"]
 setup(
     name='aioabcpapi',
-    version='2.0.5',
+    version='2.0.6',
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Async library for ABCP API',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/aioabcpapi",
     license="MIT",
     packages=['aioabcpapi', 'aioabcpapi/cp', 'aioabcpapi/ts', 'aioabcpapi/utils'],
```

### Comparing `aioabcpapi-2.0.5/test/test_payload.py` & `aioabcpapi-2.0.6/test/test_payload.py`

 * *Files identical despite different names*

