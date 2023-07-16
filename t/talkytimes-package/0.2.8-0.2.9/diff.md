# Comparing `tmp/talkytimes_package-0.2.8.tar.gz` & `tmp/talkytimes_package-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.2.8.tar", last modified: Sun Jul 16 09:19:07 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.9.tar", last modified: Sun Jul 16 09:27:06 2023, max compression
```

## Comparing `talkytimes_package-0.2.8.tar` & `talkytimes_package-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.843856 talkytimes_package-0.2.8/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 09:19:07.843856 talkytimes_package-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.8/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 09:19:07.845864 talkytimes_package-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.819857 talkytimes_package-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.826855 talkytimes_package-0.2.8/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.8/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.8/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2418 2023-07-16 09:18:45.000000 talkytimes_package-0.2.8/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.829855 talkytimes_package-0.2.8/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 09:19:05.000000 talkytimes_package-0.2.8/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.8/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.2.8/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.843856 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 09:27:06.455334 talkytimes_package-0.2.9/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 09:27:06.456333 talkytimes_package-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.9/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 09:27:06.457337 talkytimes_package-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:27:06.433334 talkytimes_package-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 09:27:06.441334 talkytimes_package-0.2.9/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.9/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.9/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2561 2023-07-16 09:26:39.000000 talkytimes_package-0.2.9/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:27:06.444333 talkytimes_package-0.2.9/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 09:27:04.000000 talkytimes_package-0.2.9/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.9/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.2.9/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:27:06.455334 talkytimes_package-0.2.9/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 09:27:06.000000 talkytimes_package-0.2.9/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 09:27:06.000000 talkytimes_package-0.2.9/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 09:27:06.000000 talkytimes_package-0.2.9/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 09:27:06.000000 talkytimes_package-0.2.9/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 09:27:06.000000 talkytimes_package-0.2.9/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.2.8/LICENSE` & `talkytimes_package-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.8/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.9/src/dynamodb/dynamodb.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,21 +51,30 @@
             dict(
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
         self.table.update_item(
-            Key=dict(external_id=external_id),
+            ExpressionAttributeNames={
+                '#user_info': 'user_info'
+            },
+            ExpressionAttributeValues={
+                ':user_info': {
+                    'S': user_info,
+                }
+            },
+            Key={
+                'external_id': {
+                    'S': external_id,
+                },
+            },
+            ReturnValues='ALL_NEW',
             UpdateExpression='SET #user_info = :user_info',
-            ExpressionAttributeNames={'#user_info': 'user_info'},
-            ExpressionAttributeValues={':user_info': {
-                "S": user_info
-            }},
-            ReturnValues="UPDATED_NEW"
+
         )
 
     def create_or_update(
         self,
         *,
         external_id: str,
         status: str,
```

### Comparing `talkytimes_package-0.2.8/src/talkytimes/base.py` & `talkytimes_package-0.2.9/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.8/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.9/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

