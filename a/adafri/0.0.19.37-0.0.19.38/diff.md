# Comparing `tmp/adafri-0.0.19.37.tar.gz` & `tmp/adafri-0.0.19.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.37.tar", last modified: Sun Jul 16 07:54:17 2023, max compression
+gzip compressed data, was "adafri-0.0.19.38.tar", last modified: Sun Jul 16 08:00:18 2023, max compression
```

## Comparing `adafri-0.0.19.37.tar` & `adafri-0.0.19.38.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.025404 adafri-0.0.19.37/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 07:54:17.025142 adafri-0.0.19.37/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.004167 adafri-0.0.19.37/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 07:54:11.000000 adafri-0.0.19.37/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.007948 adafri-0.0.19.37/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.37/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.37/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.37/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.008723 adafri-0.0.19.37/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.37/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.009377 adafri-0.0.19.37/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.37/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.011397 adafri-0.0.19.37/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.37/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.37/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.37/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.012243 adafri-0.0.19.37/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.37/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.013271 adafri-0.0.19.37/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.37/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.37/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.014257 adafri-0.0.19.37/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.37/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.014562 adafri-0.0.19.37/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-16 07:53:07.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.019059 adafri-0.0.19.37/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    13674 2023-07-16 07:52:25.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.020622 adafri-0.0.19.37/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)      885 2023-07-16 07:54:02.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.021809 adafri-0.0.19.37/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.37/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.37/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.022230 adafri-0.0.19.37/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.37/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.024356 adafri-0.0.19.37/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.37/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.37/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.37/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.005927 adafri-0.0.19.37/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 07:54:17.025513 adafri-0.0.19.37/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.37/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.831407 adafri-0.0.19.38/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 08:00:18.831112 adafri-0.0.19.38/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.809896 adafri-0.0.19.38/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 08:00:12.000000 adafri-0.0.19.38/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.813339 adafri-0.0.19.38/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.38/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.38/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.38/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.814136 adafri-0.0.19.38/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.38/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.814822 adafri-0.0.19.38/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.38/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.816914 adafri-0.0.19.38/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.38/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.38/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.38/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.817662 adafri-0.0.19.38/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.38/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.818785 adafri-0.0.19.38/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.38/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.38/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.819446 adafri-0.0.19.38/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.38/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.819748 adafri-0.0.19.38/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-16 07:53:07.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.824239 adafri-0.0.19.38/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15172 2023-07-16 08:00:04.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.826207 adafri-0.0.19.38/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)      885 2023-07-16 07:54:02.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.38/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.827675 adafri-0.0.19.38/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.38/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.38/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.828288 adafri-0.0.19.38/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.38/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.830366 adafri-0.0.19.38/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.38/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.38/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.38/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 08:00:18.811578 adafri-0.0.19.38/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 08:00:18.000000 adafri-0.0.19.38/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-16 08:00:18.000000 adafri-0.0.19.38/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 08:00:18.000000 adafri-0.0.19.38/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 08:00:18.000000 adafri-0.0.19.38/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 08:00:18.831520 adafri-0.0.19.38/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.38/setup.py
```

### Comparing `adafri-0.0.19.37/adafri/utils/response.py` & `adafri-0.0.19.38/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/utils/utils.py` & `adafri-0.0.19.38/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/account/models/account.py` & `adafri-0.0.19.38/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.38/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.38/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/models/grant.py`

 * *Files 4% similar despite different names*

```diff
@@ -252,23 +252,54 @@
 class OpenIDAuthorizationCodeGrant(grants.AuthorizationCodeGrant):
     # RESPONSE_TYPES = set({"code"})
     # TOKEN_ENDPOINT_AUTH_METHODS = [
     #     'client_secret_basic',
     #     'client_secret_post',
     #     'none'
     # ]
+    def save_authorization_code(self, code, request):
+        code_challenge = request.data.get('code_challenge')
+        code_challenge_method = request.data.get('code_challenge_method')
+        redirect_uri = request.redirect_uri;
+        nonce = request.data.get('nonce')
+        if request.args.get("redirect_uri") is not None:
+            redirect_uri = request.args.get("redirect_uri");
+        if redirect_uri is None:
+            default_redirect_uri =os.environ.get('DEFAULT_REDIRECT_URI')
+            redirect_uri = default_redirect_uri
+        model = {
+            "client_id": request.client.client_id,
+            "code": code,
+            "redirect_uri": redirect_uri,
+            "scopes": ArrayUtils.join_string_to_array(request.args.get("scope"), ","),
+            "scope": request.args.get("scope"),
+            "uid": request.user.uid,
+            "code_challenge": code_challenge,
+            "code_challenge_method": code_challenge_method,
+            "nonce": nonce,
+        }
+        auth_code_request = OAuthGrant.create(**model)
+        auth_code = auth_code_request.data
+        return auth_code
+    
     def create_authorization_code(self, client, grant_user, request):
         return create_authorization_code(client, grant_user, request)
     
     def parse_authorization_code(self, code, client):
         query_params = [{"key": GrantFields.code, "comp": "==","value": code}, {"key": GrantFields.client_id, "comp": "==","value": client.client_id}]
         auth_code = OAuthGrant().query(query_params=query_params, first=True)
         #if auth_code and not auth_code.is_expired():
         return auth_code
-
+   
+    def query_authorization_code(self, code, client):
+        query_params = [{"key": GrantFields.code, "comp": "==","value": code}, {"key": GrantFields.client_id, "comp": "==","value": client.client_id}]
+        auth_code = OAuthGrant().query(query_params=query_params, first=True)
+        #if auth_code and not auth_code.is_expired():
+        return auth_code
+    
     def delete_authorization_code(self, authorization_code):
         remove = OAuthGrant(authorization_code.to_json()).remove()
         print('removing authorization code', authorization_code.id)
 
     def authenticate_user(self, authorization_code):
         print('search', authorization_code)
         return User({"uid": authorization_code.uid}).get()
```

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.19.38/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.38/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/user/models/user.py` & `adafri-0.0.19.38/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.38/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.38/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.37/setup.py` & `adafri-0.0.19.38/setup.py`

 * *Files identical despite different names*

