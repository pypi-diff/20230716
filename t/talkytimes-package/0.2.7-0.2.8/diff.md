# Comparing `tmp/talkytimes_package-0.2.7.tar.gz` & `tmp/talkytimes_package-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.2.7.tar", last modified: Sun Jul 16 09:12:27 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.8.tar", last modified: Sun Jul 16 09:19:07 2023, max compression
```

## Comparing `talkytimes_package-0.2.7.tar` & `talkytimes_package-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:27.571871 talkytimes_package-0.2.7/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.7/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 09:12:27.571871 talkytimes_package-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.7/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 09:12:27.573871 talkytimes_package-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:27.549815 talkytimes_package-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:27.557817 talkytimes_package-0.2.7/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.7/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.7/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2381 2023-07-16 09:12:12.000000 talkytimes_package-0.2.7/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:27.560871 talkytimes_package-0.2.7/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 09:12:26.000000 talkytimes_package-0.2.7/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.7/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.2.7/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:27.570870 talkytimes_package-0.2.7/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 09:12:27.000000 talkytimes_package-0.2.7/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 09:12:27.000000 talkytimes_package-0.2.7/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 09:12:27.000000 talkytimes_package-0.2.7/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 09:12:27.000000 talkytimes_package-0.2.7/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 09:12:27.000000 talkytimes_package-0.2.7/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.843856 talkytimes_package-0.2.8/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 09:19:07.843856 talkytimes_package-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.8/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 09:19:07.845864 talkytimes_package-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.819857 talkytimes_package-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.826855 talkytimes_package-0.2.8/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.8/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.8/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2418 2023-07-16 09:18:45.000000 talkytimes_package-0.2.8/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.829855 talkytimes_package-0.2.8/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 09:19:05.000000 talkytimes_package-0.2.8/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.8/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.2.8/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:19:07.843856 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 09:19:07.000000 talkytimes_package-0.2.8/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.2.7/LICENSE` & `talkytimes_package-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.7/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.8/src/dynamodb/dynamodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,17 @@
                 emails=emails
             )
         )
         self.table.update_item(
             Key=dict(external_id=external_id),
             UpdateExpression='SET #user_info = :user_info',
             ExpressionAttributeNames={'#user_info': 'user_info'},
-            ExpressionAttributeValues={':user_info': user_info},
+            ExpressionAttributeValues={':user_info': {
+                "S": user_info
+            }},
             ReturnValues="UPDATED_NEW"
         )
 
     def create_or_update(
         self,
         *,
         external_id: str,
```

### Comparing `talkytimes_package-0.2.7/src/talkytimes/base.py` & `talkytimes_package-0.2.8/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.7/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.8/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

