# Comparing `tmp/types-aiobotocore-dynamodb-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-dynamodb-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post1.tar", last modified: Sat Jul 15 06:45:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post2.tar", last modified: Sun Jul 16 12:49:57 2023, max compression
```

## Comparing `types-aiobotocore-dynamodb-2.5.2.post1.tar` & `types-aiobotocore-dynamodb-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-15 06:32:45.000000 types-aiobotocore-dynamodb-2.5.2.post1/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29459 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27884 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-07-15 06:44:52.000000 types-aiobotocore-dynamodb-2.5.2.post1/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1813 2023-07-15 06:32:46.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1812 2023-07-15 06:32:46.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    56380 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    56311 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12866 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12864 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8705 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8698 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:32:46.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28868 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28840 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   151413 2023-07-15 06:44:58.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   151276 2023-07-15 06:44:56.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2442 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2440 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29459 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1002 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29495 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27920 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1813 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1812 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    56380 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    56311 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12866 2023-07-16 12:49:26.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12864 2023-07-16 12:49:26.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8705 2023-07-16 12:47:34.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8698 2023-07-16 12:47:34.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29455 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29426 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   151607 2023-07-16 12:49:30.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   151470 2023-07-16 12:49:28.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2442 2023-07-16 12:47:35.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2440 2023-07-16 12:47:34.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29495 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1002 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/LICENSE` & `types-aiobotocore-dynamodb-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.2.post1
+Version: 2.5.2.post2
 Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
@@ -576,14 +576,15 @@
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
     StreamSpecificationOutputTypeDef,
     StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
+    TableBatchWriterRequestTypeDef,
     TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
     ArchivalSummaryTableResponseMetadataTypeDef,
     BillingModeSummaryTableResponseMetadataTypeDef,
     DescribeLimitsOutputTypeDef,
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/README.md` & `types-aiobotocore-dynamodb-2.5.2.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -543,14 +543,15 @@
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
     StreamSpecificationOutputTypeDef,
     StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
+    TableBatchWriterRequestTypeDef,
     TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
     ArchivalSummaryTableResponseMetadataTypeDef,
     BillingModeSummaryTableResponseMetadataTypeDef,
     DescribeLimitsOutputTypeDef,
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/setup.py` & `types-aiobotocore-dynamodb-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodb",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder"
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.pyi` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__main__.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post2\nBuilder"
         " version: 7.15.0\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.pyi` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.pyi` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.pyi` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,26 @@
         resource: DynamoDBServiceResource
 
         my_table: dynamodb_resources.Table = resource.Table(...)
 ```
 """
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, AsyncIterator, Awaitable, List, Mapping, NoReturn, Sequence, Set, Union
+from typing import (
+    Any,
+    AsyncIterator,
+    Awaitable,
+    List,
+    Mapping,
+    NoReturn,
+    Optional,
+    Sequence,
+    Set,
+    Union,
+)
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
@@ -73,17 +84,17 @@
     TableClassSummaryTableResponseMetadataTypeDef,
     TagServiceResourceTypeDef,
     UpdateItemOutputTableTypeDef,
     WriteRequestServiceResourceTypeDef,
 )
 
 try:
-    from aioboto3.dynamodb.table import CustomTableResource
+    from aioboto3.dynamodb.table import BatchWriter
 except (ModuleNotFoundError, ImportError):
-    from builtins import object as CustomTableResource
+    from builtins import object as BatchWriter
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
     from aioboto3.resources.collection import AIOResourceCollection
 except (ModuleNotFoundError, ImportError):
@@ -162,15 +173,15 @@
         A generator which yields Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#serviceresourcetablescollection)
         """
 
 
-class Table(AIOBoto3ServiceResource, CustomTableResource):
+class Table(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#table)
     """
 
     attribute_definitions: Awaitable[List[AttributeDefinitionTableOutputTypeDef]]
     table_name: Awaitable[str]
@@ -193,14 +204,27 @@
     restore_summary: Awaitable[RestoreSummaryTableResponseMetadataTypeDef]
     sse_description: Awaitable[SSEDescriptionTableResponseMetadataTypeDef]
     archival_summary: Awaitable[ArchivalSummaryTableResponseMetadataTypeDef]
     table_class_summary: Awaitable[TableClassSummaryTableResponseMetadataTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
 
+    def batch_writer(
+        self,
+        overwrite_by_pkeys: Optional[List[str]] = ...,
+        flush_amount: int = ...,
+        on_exit_loop_sleep: int = ...,
+    ) -> BatchWriter:
+        """
+        Create a batch writer object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
+        """
+
     async def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.pyi` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,26 @@
         resource: DynamoDBServiceResource
 
         my_table: dynamodb_resources.Table = resource.Table(...)
 ```
 """
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, AsyncIterator, Awaitable, List, Mapping, NoReturn, Sequence, Set, Union
+from typing import (
+    Any,
+    AsyncIterator,
+    Awaitable,
+    List,
+    Mapping,
+    NoReturn,
+    Optional,
+    Sequence,
+    Set,
+    Union,
+)
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
@@ -73,17 +84,17 @@
     TableClassSummaryTableResponseMetadataTypeDef,
     TagServiceResourceTypeDef,
     UpdateItemOutputTableTypeDef,
     WriteRequestServiceResourceTypeDef,
 )
 
 try:
-    from aioboto3.dynamodb.table import CustomTableResource
+    from aioboto3.dynamodb.table import BatchWriter
 except (ModuleNotFoundError, ImportError):
-    from builtins import object as CustomTableResource
+    from builtins import object as BatchWriter
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
     from aioboto3.resources.collection import AIOResourceCollection
 except (ModuleNotFoundError, ImportError):
@@ -153,15 +164,15 @@
         """
         A generator which yields Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#serviceresourcetablescollection)
         """
 
-class Table(AIOBoto3ServiceResource, CustomTableResource):
+class Table(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#table)
     """
 
     attribute_definitions: Awaitable[List[AttributeDefinitionTableOutputTypeDef]]
     table_name: Awaitable[str]
@@ -184,14 +195,26 @@
     restore_summary: Awaitable[RestoreSummaryTableResponseMetadataTypeDef]
     sse_description: Awaitable[SSEDescriptionTableResponseMetadataTypeDef]
     archival_summary: Awaitable[ArchivalSummaryTableResponseMetadataTypeDef]
     table_class_summary: Awaitable[TableClassSummaryTableResponseMetadataTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
 
+    def batch_writer(
+        self,
+        overwrite_by_pkeys: Optional[List[str]] = ...,
+        flush_amount: int = ...,
+        on_exit_loop_sleep: int = ...,
+    ) -> BatchWriter:
+        """
+        Create a batch writer object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
+        """
     async def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,15 @@
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
     "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
     "StreamSpecificationOutputTypeDef",
     "StreamSpecificationTableOutputTypeDef",
     "StreamSpecificationTableTypeDef",
+    "TableBatchWriterRequestTypeDef",
     "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
     "ArchivalSummaryTableResponseMetadataTypeDef",
     "BillingModeSummaryTableResponseMetadataTypeDef",
     "DescribeLimitsOutputTypeDef",
@@ -1736,14 +1737,22 @@
 
 class StreamSpecificationTableTypeDef(
     _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
 ):
     pass
 
 
+TableBatchWriterRequestTypeDef = TypedDict(
+    "TableBatchWriterRequestTypeDef",
+    {
+        "overwrite_by_pkeys": List[str],
+    },
+    total=False,
+)
+
 TimeToLiveSpecificationOutputTypeDef = TypedDict(
     "TimeToLiveSpecificationOutputTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.pyi` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
     "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
     "StreamSpecificationOutputTypeDef",
     "StreamSpecificationTableOutputTypeDef",
     "StreamSpecificationTableTypeDef",
+    "TableBatchWriterRequestTypeDef",
     "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
     "ArchivalSummaryTableResponseMetadataTypeDef",
     "BillingModeSummaryTableResponseMetadataTypeDef",
     "DescribeLimitsOutputTypeDef",
@@ -1713,14 +1714,22 @@
 )
 
 class StreamSpecificationTableTypeDef(
     _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
 ):
     pass
 
+TableBatchWriterRequestTypeDef = TypedDict(
+    "TableBatchWriterRequestTypeDef",
+    {
+        "overwrite_by_pkeys": List[str],
+    },
+    total=False,
+)
+
 TimeToLiveSpecificationOutputTypeDef = TypedDict(
     "TimeToLiveSpecificationOutputTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.py` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.pyi` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.2.post1
+Version: 2.5.2.post2
 Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
@@ -576,14 +576,15 @@
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
     StreamSpecificationOutputTypeDef,
     StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
+    TableBatchWriterRequestTypeDef,
     TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
     ArchivalSummaryTableResponseMetadataTypeDef,
     BillingModeSummaryTableResponseMetadataTypeDef,
     DescribeLimitsOutputTypeDef,
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

