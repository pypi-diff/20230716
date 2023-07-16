# Comparing `tmp/carica_dynamodb_tools-1.5.tar.gz` & `tmp/carica_dynamodb_tools-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carica_dynamodb_tools-1.5.tar", last modified: Sat Jul 15 19:32:20 2023, max compression
+gzip compressed data, was "carica_dynamodb_tools-1.6.tar", last modified: Sun Jul 16 19:13:14 2023, max compression
```

## Comparing `carica_dynamodb_tools-1.5.tar` & `carica_dynamodb_tools-1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)    11358 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.5/LICENSE
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1395 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/PKG-INFO
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      651 2023-04-08 13:04:58.000000 carica_dynamodb_tools-1.5/README.rst
-drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/carica_dynamodb_tools/
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        0 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/__init__.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)      977 2023-07-15 18:48:48.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/dump.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     6212 2023-07-15 19:24:30.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/dump_s3_export.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     5931 2023-04-08 13:07:12.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/load.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     2085 2023-07-15 19:22:19.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/s3_export.py
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      593 2021-11-16 15:20:28.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/session.py
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      262 2023-07-15 18:48:48.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/utils.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)       20 2023-07-15 19:31:33.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/version.py
-drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1395 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/PKG-INFO
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      590 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        1 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      265 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/entry_points.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       55 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/requires.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       22 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/top_level.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       46 2023-03-02 19:05:06.000000 carica_dynamodb_tools-1.5/pyproject.toml
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       67 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/setup.cfg
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     1784 2023-07-15 19:17:19.000000 carica_dynamodb_tools-1.5/setup.py
+drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-16 19:13:14.555354 carica_dynamodb_tools-1.6/
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)    11358 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.6/LICENSE
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1395 2023-07-16 19:13:14.555354 carica_dynamodb_tools-1.6/PKG-INFO
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      651 2023-04-08 13:04:58.000000 carica_dynamodb_tools-1.6/README.rst
+drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-16 19:13:14.555354 carica_dynamodb_tools-1.6/carica_dynamodb_tools/
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        0 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/__init__.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     1002 2023-07-16 19:12:04.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/dump.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     6237 2023-07-16 19:12:10.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/dump_s3_export.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     5955 2023-07-16 19:12:14.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/load.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     2085 2023-07-15 19:22:19.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/s3_export.py
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      593 2021-11-16 15:20:28.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/session.py
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      261 2023-07-16 19:12:20.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/utils.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)       20 2023-07-16 19:11:13.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools/version.py
+drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-16 19:13:14.555354 carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1395 2023-07-16 19:13:14.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      590 2023-07-16 19:13:14.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        1 2023-07-16 19:13:14.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      265 2023-07-16 19:13:14.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       69 2023-07-16 19:13:14.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/requires.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       22 2023-07-16 19:13:14.000000 carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/top_level.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       46 2023-03-02 19:05:06.000000 carica_dynamodb_tools-1.6/pyproject.toml
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       67 2023-07-16 19:13:14.555354 carica_dynamodb_tools-1.6/setup.cfg
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     1809 2023-07-16 19:04:55.000000 carica_dynamodb_tools-1.6/setup.py
```

### Comparing `carica_dynamodb_tools-1.5/LICENSE` & `carica_dynamodb_tools-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.5/PKG-INFO` & `carica_dynamodb_tools-1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carica_dynamodb_tools
-Version: 1.5
+Version: 1.6
 Summary: Tools to manage DynamoDB tables
 Home-page: https://github.com/caricalabs/carica-dynamodb-tools
 Author: Carica Labs, LLC
 Author-email: info@caricalabs.com
 License: APL 2.0
 Description: carica-dynamodb-tools - Tools to manage DynamoDB tables
         ==================================================================================
```

### Comparing `carica_dynamodb_tools-1.5/README.rst` & `carica_dynamodb_tools-1.6/README.rst`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.5/carica_dynamodb_tools/dump.py` & `carica_dynamodb_tools-1.6/carica_dynamodb_tools/dump.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import json
-
 import click
+import orjson
 import sys
 
 import carica_dynamodb_tools.version
 import carica_dynamodb_tools.version
 from carica_dynamodb_tools.session import boto_session
 from carica_dynamodb_tools.utils import remove_protected_attrs
 
@@ -21,13 +20,13 @@
     """
     session = boto_session(region_name=region)
     client = session.client('dynamodb')
     paginator = client.get_paginator('scan')
     for page in paginator.paginate(TableName=table):
         for item in page['Items']:
             item = remove_protected_attrs(item)
-            json.dump(item, sys.stdout)
-            sys.stdout.write('\n')
+            sys.stdout.buffer.write(orjson.dumps(item))
+            sys.stdout.buffer.write(b'\n')
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `carica_dynamodb_tools-1.5/carica_dynamodb_tools/dump_s3_export.py` & `carica_dynamodb_tools-1.6/carica_dynamodb_tools/dump_s3_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gzip
-import json
 import multiprocessing
 from multiprocessing import Queue
 from typing import Tuple
 
 import click
+import orjson
 import sys
 from botocore.response import StreamingBody
 from click import BadParameter
 
 import carica_dynamodb_tools.version
 import carica_dynamodb_tools.version
 from carica_dynamodb_tools.session import boto_session
@@ -37,15 +37,15 @@
 
     bucket = desc['S3Bucket']
     prefix = desc.get('S3Prefix', '')
     manifest_key = desc['ExportManifest']
 
     # Download the small export manifest JSON file
     resp = s3_client.get_object(Bucket=bucket, Key=f'{prefix}{manifest_key}')
-    manifest = json.loads(resp['Body'].read())
+    manifest = orjson.loads(resp['Body'].read())
     item_count = manifest['itemCount']
     manifest_files_key = manifest['manifestFilesS3Key']
 
     # Open the data items manifest JSON file, but return the response so the caller
     # can stream lines out of it.
     resp = s3_client.get_object(Bucket=bucket, Key=manifest_files_key)
     return bucket, item_count, resp['Body']
@@ -77,20 +77,20 @@
         key = manifest_item['dataFileS3Key']
         etag = manifest_item['etag']
         try:
             resp = s3_client.get_object(Bucket=bucket, Key=key, IfMatch=etag)
             with gzip.open(resp['Body'], 'rt') as data_item_lines:
                 for data_item_line in data_item_lines:
                     # Remove the wrapping "Item" property at the top level
-                    item = json.loads(data_item_line)['Item']
+                    item = orjson.loads(data_item_line)['Item']
                     item = remove_protected_attrs(item)
-                    item_json = json.dumps(item)
+                    item_json = orjson.dumps(item)
                     with print_lock:
-                        sys.stdout.write(item_json)
-                        sys.stdout.write('\n')
+                        sys.stdout.buffer.write(item_json)
+                        sys.stdout.buffer.write(b'\n')
                     with item_total.get_lock():
                         item_total.value += 1
         except Exception as e:
             with error_total.get_lock():
                 error_total.value += 1
             with print_lock:
                 print(
@@ -150,15 +150,15 @@
 
     for p in procs:
         p.start()
 
     # Read manifest items, putting one decoded item into the queue at a time.
     # Put blocks when the queue is full.
     for line in data_manifest_response.iter_lines():
-        manifest_item_q.put(json.loads(line))
+        manifest_item_q.put(orjson.loads(line))
 
     for _ in procs:
         manifest_item_q.put(None)
 
     for p in procs:
         p.join()
```

### Comparing `carica_dynamodb_tools-1.5/carica_dynamodb_tools/load.py` & `carica_dynamodb_tools-1.6/carica_dynamodb_tools/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import json
 import multiprocessing
 import random
-import sys
-import time
 from multiprocessing.queues import Queue
 
 import click
+import orjson
+import sys
+import time
 from botocore.exceptions import ClientError
 from click import BadParameter
 
 import carica_dynamodb_tools.version
 import carica_dynamodb_tools.version
 
 # DynamoDB API limit
@@ -141,15 +141,15 @@
         p.start()
 
     # Read items from stdin, batch them up, and send batches to workers.
     batch = []
     while True:
         line = sys.stdin.readline()
         if line:
-            batch.append(json.loads(line))
+            batch.append(orjson.loads(line))
 
         # Send the batch to the worker when it's full or stdin is closed.
         # We don't worry about checking for total batch size here (in
         # serialized JSON bytes) because we assume DynamoDB would not have
         # supplied records that are too large to load during the dump process.
         if len(batch) == BATCH_MAX_ITEMS or not line:
             batch_q.put(batch)
@@ -167,12 +167,12 @@
     if report:
         with success_total.get_lock(), failure_total.get_lock(), retry_total.get_lock():
             report = {
                 'loaded': success_total.value,
                 'failed': failure_total.value,
                 'retried': retry_total.value,
             }
-        print(json.dumps(report))
+        sys.stdout.buffer.write(orjson.dumps(report))
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `carica_dynamodb_tools-1.5/carica_dynamodb_tools/s3_export.py` & `carica_dynamodb_tools-1.6/carica_dynamodb_tools/s3_export.py`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.5/carica_dynamodb_tools/session.py` & `carica_dynamodb_tools-1.6/carica_dynamodb_tools/session.py`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/PKG-INFO` & `carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carica-dynamodb-tools
-Version: 1.5
+Version: 1.6
 Summary: Tools to manage DynamoDB tables
 Home-page: https://github.com/caricalabs/carica-dynamodb-tools
 Author: Carica Labs, LLC
 Author-email: info@caricalabs.com
 License: APL 2.0
 Description: carica-dynamodb-tools - Tools to manage DynamoDB tables
         ==================================================================================
```

### Comparing `carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/SOURCES.txt` & `carica_dynamodb_tools-1.6/carica_dynamodb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.5/setup.py` & `carica_dynamodb_tools-1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         'Programming Language :: Python :: 3.7',
     ],
     keywords='dynamodb backup restore archive dump load',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     install_requires=[
         'boto3>=1.9.99',
         'click~=8.0',
+        'orjson~=3.9.2',
     ],
     extras_require={
         'dev': ['check-manifest'],
         'test': [],
     },
     package_data={},
     entry_points={
```

