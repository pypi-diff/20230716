# Comparing `tmp/talkytimes_package-0.2.2.tar.gz` & `tmp/talkytimes_package-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.2.2.tar", last modified: Sun Jul 16 08:33:41 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.3.tar", last modified: Sun Jul 16 08:46:28 2023, max compression
```

## Comparing `talkytimes_package-0.2.2.tar` & `talkytimes_package-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:33:41.002037 talkytimes_package-0.2.2/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 08:33:41.002037 talkytimes_package-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.2/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 08:33:41.003041 talkytimes_package-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:33:40.980038 talkytimes_package-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 08:33:40.988040 talkytimes_package-0.2.2/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.2/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.2/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2321 2023-07-16 08:28:00.000000 talkytimes_package-0.2.2/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:33:40.990038 talkytimes_package-0.2.2/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 08:33:08.000000 talkytimes_package-0.2.2/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.2/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3956 2023-07-16 08:32:47.000000 talkytimes_package-0.2.2/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:33:41.001037 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.471886 talkytimes_package-0.2.3/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:46:28.472886 talkytimes_package-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.3/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 08:46:28.473886 talkytimes_package-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.443880 talkytimes_package-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.451882 talkytimes_package-0.2.3/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.3/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.3/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2343 2023-07-16 08:42:54.000000 talkytimes_package-0.2.3/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.453880 talkytimes_package-0.2.3/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 08:46:22.000000 talkytimes_package-0.2.3/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.3/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3956 2023-07-16 08:32:47.000000 talkytimes_package-0.2.3/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.470881 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.2.2/LICENSE` & `talkytimes_package-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.2/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.3/src/dynamodb/dynamodb.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         external_id: str,
         status: str,
         messages: Optional[str] = "0",
         emails: Optional[str] = "0"
     ) -> Any:
         data = dict(
             external_id=external_id,
-            value=json.dumps(
+            user_info=json.dumps(
                 dict(
                     status=status,
                     messages=messages,
                     emails=emails
                 )
             )
         )
@@ -43,26 +43,26 @@
         self,
         *,
         external_id: str,
         status: str,
         messages: Optional[str] = "0",
         emails: Optional[str] = "0"
     ) -> None:
-        others = json.dumps(
+        user_info = json.dumps(
             dict(
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
         self.table.update_item(
             Key=dict(external_id=external_id),
-            UpdateExpression="set value=:value",
+            UpdateExpression="set user_info=:user_info",
             ExpressionAttributeValues={
-                ':value': others,
+                ':user_info': user_info,
             },
             ReturnValues="UPDATED_NEW"
         )
 
     def create_or_update(
         self,
         *,
```

### Comparing `talkytimes_package-0.2.2/src/talkytimes/base.py` & `talkytimes_package-0.2.3/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.2/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.3/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

