# Comparing `tmp/adafri-0.0.19.34.tar.gz` & `tmp/adafri-0.0.19.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.34.tar", last modified: Sun Jul 16 05:23:14 2023, max compression
+gzip compressed data, was "adafri-0.0.19.35.tar", last modified: Sun Jul 16 05:40:51 2023, max compression
```

## Comparing `adafri-0.0.19.34.tar` & `adafri-0.0.19.35.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.407885 adafri-0.0.19.34/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 05:23:14.407231 adafri-0.0.19.34/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.373117 adafri-0.0.19.34/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 05:23:08.000000 adafri-0.0.19.34/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.378164 adafri-0.0.19.34/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.34/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.34/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.34/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.379217 adafri-0.0.19.34/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)      137 2023-07-16 01:52:16.000000 adafri-0.0.19.34/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.380398 adafri-0.0.19.34/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.34/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.383714 adafri-0.0.19.34/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.34/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.34/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.34/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.385124 adafri-0.0.19.34/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      314 2023-07-16 01:50:48.000000 adafri-0.0.19.34/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.387051 adafri-0.0.19.34/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.34/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.34/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.388244 adafri-0.0.19.34/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.34/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.388799 adafri-0.0.19.34/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      688 2023-07-16 05:22:32.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.396587 adafri-0.0.19.34/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11644 2023-07-16 05:17:11.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.399142 adafri-0.0.19.34/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      156 2023-07-16 05:21:48.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1463 2023-07-16 05:21:39.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1907 2023-07-16 05:22:43.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.401155 adafri-0.0.19.34/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.34/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.34/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.401801 adafri-0.0.19.34/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.34/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.405427 adafri-0.0.19.34/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.34/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.34/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.34/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.375604 adafri-0.0.19.34/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 05:23:14.408146 adafri-0.0.19.34/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.34/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.620585 adafri-0.0.19.35/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 05:40:51.620312 adafri-0.0.19.35/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.598178 adafri-0.0.19.35/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 05:40:47.000000 adafri-0.0.19.35/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.601594 adafri-0.0.19.35/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.35/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.35/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.35/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.602287 adafri-0.0.19.35/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      137 2023-07-16 01:52:16.000000 adafri-0.0.19.35/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.602954 adafri-0.0.19.35/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.35/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.605004 adafri-0.0.19.35/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.35/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.35/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.35/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.605877 adafri-0.0.19.35/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.35/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.607131 adafri-0.0.19.35/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.35/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.35/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.607972 adafri-0.0.19.35/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.35/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.608288 adafri-0.0.19.35/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      784 2023-07-16 05:40:08.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.613404 adafri-0.0.19.35/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11644 2023-07-16 05:17:11.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.615419 adafri-0.0.19.35/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1657 2023-07-16 05:38:24.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.35/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.616848 adafri-0.0.19.35/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.35/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.35/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.617683 adafri-0.0.19.35/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.35/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.619433 adafri-0.0.19.35/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.35/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.35/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.35/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:40:51.599857 adafri-0.0.19.35/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 05:40:51.000000 adafri-0.0.19.35/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-16 05:40:51.000000 adafri-0.0.19.35/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 05:40:51.000000 adafri-0.0.19.35/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 05:40:51.000000 adafri-0.0.19.35/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 05:40:51.620700 adafri-0.0.19.35/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.35/setup.py
```

### Comparing `adafri-0.0.19.34/adafri/utils/response.py` & `adafri-0.0.19.35/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/utils/utils.py` & `adafri-0.0.19.35/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/account/models/account.py` & `adafri-0.0.19.35/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.35/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.35/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,22 +18,24 @@
     def authenticate_client(self, request, methods, endpoint='token'):
         return super().authenticate_client(request, methods, endpoint)
     
     def handle_error_response(self, request, error):
         return self.handle_response(*error(self.get_error_uri(request, error)))
     
 
-oidc_server_authorization = AuthServer(
-    query_client=OAuthClient().get_by_client_id,
-    save_token=OAuthToken().save,
-)
-
+# oidc_authorization_server = AuthServer(
+#     query_client=OAuthClient().get_by_client_id,
+#     save_token=OAuthToken().save,
+# )
+oidc_authorization_server = AuthorizationServer()
 require_oidc_oauth = ResourceProtector()
 
 def config_oidc_oauth(app):
-    oidc_server_authorization.init_app(app)
-    oidc_server_authorization.register_grant(AuthCodeGrant, [
+    oidc_authorization_server.query_client = OAuthClient().get_by_client_id
+    oidc_authorization_server.save_token = OAuthToken().save
+    oidc_authorization_server.init_app(app)
+    oidc_authorization_server.register_grant(AuthCodeGrant, [
         OpenIDCode(require_nonce=True),
     ])
-    oidc_server_authorization.register_grant(OpenIDImplicitGrant)
-    oidc_server_authorization.register_grant(OpenIDHybridGrant)
+    oidc_authorization_server.register_grant(OpenIDImplicitGrant)
+    oidc_authorization_server.register_grant(OpenIDHybridGrant)
     require_oidc_oauth.register_token_validator(TokenValidator())
```

### Comparing `adafri-0.0.19.34/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.19.35/adafri/v1/auth/oauth/server/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,32 +18,36 @@
     def authenticate_client(self, request, methods, endpoint='token'):
         return super().authenticate_client(request, methods, endpoint)
     
     def handle_error_response(self, request, error):
         return self.handle_response(*error(self.get_error_uri(request, error)))
     
 
-authorization = AuthServer(
-    query_client=OAuthClient().get_by_client_id,
-    save_token=OAuthToken().save,
-)
+# authorization_server = AuthServer(
+#     query_client=OAuthClient().get_by_client_id,
+#     save_token=OAuthToken().save,
+# )
+authorization_server = AuthorizationServer()
+require_oauth = ResourceProtector()
 
 require_oauth = ResourceProtector()
 
 def config_oauth(app):
-    authorization.init_app(app)
+    authorization_server.query_client = OAuthClient().get_by_client_id
+    authorization_server.save_token = OAuthToken().save
+    authorization_server.init_app(app)
     
-    authorization.register_grant(grants.ImplicitGrant)
-    #authorization.register_grant(AccessTokenGrant, [CodeChallenge(required=True)])
-    authorization.register_grant(grants.ClientCredentialsGrant)
-    authorization.register_grant(AuthCodeGrant, [CodeChallenge(required=True)])
+    authorization_server.register_grant(grants.ImplicitGrant)
+    #authorization_server.register_grant(AccessTokenGrant, [CodeChallenge(required=True)])
+    authorization_server.register_grant(grants.ClientCredentialsGrant)
+    authorization_server.register_grant(AuthCodeGrant, [CodeChallenge(required=True)])
     
-    # authorization.register_grant(PasswordGrant)
-    authorization.register_grant(RefreshTokenGrant)
+    # authorization_server.register_grant(PasswordGrant)
+    authorization_server.register_grant(RefreshTokenGrant)
     # support revocation
     # revocation_cls = create_revocation_endpoint()
-    authorization.register_endpoint(TokenRevocationEndpoint)
-    # authorization.register_token_generator("default", TokenGenerator.generate)
-    # authorization.register_token_generator("client_credentials", TokenGenerator.generate)
+    authorization_server.register_endpoint(TokenRevocationEndpoint)
+    # authorization_server.register_token_generator("default", TokenGenerator.generate)
+    # authorization_server.register_token_generator("client_credentials", TokenGenerator.generate)
     # protect resource
     #bearer_cls = create_bearer_token_validator(TokenValidator)
     require_oauth.register_token_validator(TokenValidator())
```

### Comparing `adafri-0.0.19.34/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.35/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/user/models/user.py` & `adafri-0.0.19.35/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.35/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.35/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.34/setup.py` & `adafri-0.0.19.35/setup.py`

 * *Files identical despite different names*

