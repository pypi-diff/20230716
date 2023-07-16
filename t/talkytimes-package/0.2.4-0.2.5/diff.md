# Comparing `tmp/talkytimes_package-0.2.4.tar.gz` & `tmp/talkytimes_package-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.2.4.tar", last modified: Sun Jul 16 08:50:36 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.5.tar", last modified: Sun Jul 16 09:01:49 2023, max compression
```

## Comparing `talkytimes_package-0.2.4.tar` & `talkytimes_package-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.211445 talkytimes_package-0.2.4/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 08:50:36.211445 talkytimes_package-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.4/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 08:50:36.212445 talkytimes_package-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.189445 talkytimes_package-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.197445 talkytimes_package-0.2.4/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.4/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.4/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2343 2023-07-16 08:42:54.000000 talkytimes_package-0.2.4/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.200446 talkytimes_package-0.2.4/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 08:50:33.000000 talkytimes_package-0.2.4/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.4/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.2.4/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.210447 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 09:01:49.389269 talkytimes_package-0.2.5/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 09:01:49.390269 talkytimes_package-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.5/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 09:01:49.391267 talkytimes_package-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:01:49.365268 talkytimes_package-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 09:01:49.373267 talkytimes_package-0.2.5/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.5/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.5/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2276 2023-07-16 09:01:39.000000 talkytimes_package-0.2.5/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:01:49.376267 talkytimes_package-0.2.5/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 09:01:47.000000 talkytimes_package-0.2.5/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.5/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.2.5/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:01:49.388267 talkytimes_package-0.2.5/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 09:01:49.000000 talkytimes_package-0.2.5/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 09:01:49.000000 talkytimes_package-0.2.5/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 09:01:49.000000 talkytimes_package-0.2.5/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 09:01:49.000000 talkytimes_package-0.2.5/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 09:01:49.000000 talkytimes_package-0.2.5/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.2.4/LICENSE` & `talkytimes_package-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.4/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.5/src/dynamodb/dynamodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,17 +52,16 @@
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
         self.table.update_item(
             Key=dict(external_id=external_id),
-            UpdateExpression="set user_info=:user_info",
-            ExpressionAttributeValues={
-                ':user_info': user_info,
+            AttributeUpdates={
+                'user_info': user_info,
             },
             ReturnValues="UPDATED_NEW"
         )
 
     def create_or_update(
         self,
         *,
```

### Comparing `talkytimes_package-0.2.4/src/talkytimes/base.py` & `talkytimes_package-0.2.5/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.4/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.5/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

