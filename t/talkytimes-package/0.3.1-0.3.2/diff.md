# Comparing `tmp/talkytimes_package-0.3.1.tar.gz` & `tmp/talkytimes_package-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.3.1.tar", last modified: Sun Jul 16 16:02:13 2023, max compression
+gzip compressed data, was "talkytimes_package-0.3.2.tar", last modified: Sun Jul 16 17:01:00 2023, max compression
```

## Comparing `talkytimes_package-0.3.1.tar` & `talkytimes_package-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 16:02:13.290888 talkytimes_package-0.3.1/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 16:02:13.290888 talkytimes_package-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.1/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 16:02:13.295890 talkytimes_package-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:02:13.265886 talkytimes_package-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 16:02:13.273883 talkytimes_package-0.3.1/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.1/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.1/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2375 2023-07-16 16:01:43.000000 talkytimes_package-0.3.1/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:02:13.276885 talkytimes_package-0.3.1/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 16:02:09.000000 talkytimes_package-0.3.1/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.1/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.3.1/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:02:13.289888 talkytimes_package-0.3.1/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 16:02:13.000000 talkytimes_package-0.3.1/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 16:02:13.000000 talkytimes_package-0.3.1/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 16:02:13.000000 talkytimes_package-0.3.1/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 16:02:13.000000 talkytimes_package-0.3.1/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 16:02:13.000000 talkytimes_package-0.3.1/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 17:01:00.713402 talkytimes_package-0.3.2/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 17:01:00.713402 talkytimes_package-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.2/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 17:01:00.714402 talkytimes_package-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:01:00.685322 talkytimes_package-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 17:01:00.694322 talkytimes_package-0.3.2/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.2/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.2/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2551 2023-07-16 17:00:36.000000 talkytimes_package-0.3.2/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:01:00.697402 talkytimes_package-0.3.2/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 17:00:57.000000 talkytimes_package-0.3.2/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.2/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.3.2/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:01:00.712402 talkytimes_package-0.3.2/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 17:01:00.000000 talkytimes_package-0.3.2/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 17:01:00.000000 talkytimes_package-0.3.2/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 17:01:00.000000 talkytimes_package-0.3.2/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 17:01:00.000000 talkytimes_package-0.3.2/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 17:01:00.000000 talkytimes_package-0.3.2/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.3.1/LICENSE` & `talkytimes_package-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.1/src/dynamodb/dynamodb.py` & `talkytimes_package-0.3.2/src/dynamodb/dynamodb.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,23 +51,29 @@
             dict(
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
         self.table.update_item(
+            ExpressionAttributeNames={
+                '#UI': 'user_info',
+            },
+            ExpressionAttributeValues={
+                ':user_info': {
+                    'S': user_info,
+                },
+            },
             Key={
-                "external_id": {
-                    "S": external_id
+                'external_id': {
+                    'S': external_id,
                 }
             },
-            UpdateExpression="SET user_info = :val1",
-            ExpressionAttributeValues={
-                ":val1": {"S": user_info}
-            }
+            ReturnValues='UPDATED_NEW',
+            UpdateExpression='SET #UI = :user_info',
         )
 
     def create_or_update(
         self,
         *,
         external_id: str,
         status: str,
```

### Comparing `talkytimes_package-0.3.1/src/talkytimes/base.py` & `talkytimes_package-0.3.2/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.1/src/talkytimes/talkytimes.py` & `talkytimes_package-0.3.2/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

