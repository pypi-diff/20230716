# Comparing `tmp/adafri-0.0.19.33.tar.gz` & `tmp/adafri-0.0.19.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.33.tar", last modified: Sun Jul 16 01:52:35 2023, max compression
+gzip compressed data, was "adafri-0.0.19.34.tar", last modified: Sun Jul 16 05:23:14 2023, max compression
```

## Comparing `adafri-0.0.19.33.tar` & `adafri-0.0.19.34.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.463683 adafri-0.0.19.33/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 01:52:35.463323 adafri-0.0.19.33/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.437827 adafri-0.0.19.33/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 01:46:28.000000 adafri-0.0.19.33/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.442540 adafri-0.0.19.33/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.33/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.33/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.33/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.443346 adafri-0.0.19.33/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)      137 2023-07-16 01:52:16.000000 adafri-0.0.19.33/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.444233 adafri-0.0.19.33/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.33/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.446623 adafri-0.0.19.33/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.33/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.33/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.33/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.447712 adafri-0.0.19.33/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      314 2023-07-16 01:50:48.000000 adafri-0.0.19.33/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.449337 adafri-0.0.19.33/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.33/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.33/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.450201 adafri-0.0.19.33/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.33/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.450559 adafri-0.0.19.33/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      660 2023-07-16 01:49:50.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.456476 adafri-0.0.19.33/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9475 2023-07-15 08:08:12.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.457610 adafri-0.0.19.33/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)     1907 2023-07-16 01:45:10.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/server/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.459225 adafri-0.0.19.33/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.33/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.33/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.460085 adafri-0.0.19.33/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.33/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.462299 adafri-0.0.19.33/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.33/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.33/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.33/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.440365 adafri-0.0.19.33/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1086 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 01:52:35.463832 adafri-0.0.19.33/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.33/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.407885 adafri-0.0.19.34/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 05:23:14.407231 adafri-0.0.19.34/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.373117 adafri-0.0.19.34/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 05:23:08.000000 adafri-0.0.19.34/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.378164 adafri-0.0.19.34/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.34/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.34/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.34/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.379217 adafri-0.0.19.34/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      137 2023-07-16 01:52:16.000000 adafri-0.0.19.34/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.380398 adafri-0.0.19.34/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.34/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.383714 adafri-0.0.19.34/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.34/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.34/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.34/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.385124 adafri-0.0.19.34/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      314 2023-07-16 01:50:48.000000 adafri-0.0.19.34/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.387051 adafri-0.0.19.34/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.34/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.34/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.388244 adafri-0.0.19.34/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.34/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.388799 adafri-0.0.19.34/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      688 2023-07-16 05:22:32.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.396587 adafri-0.0.19.34/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11644 2023-07-16 05:17:11.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.399142 adafri-0.0.19.34/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      156 2023-07-16 05:21:48.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1463 2023-07-16 05:21:39.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1907 2023-07-16 05:22:43.000000 adafri-0.0.19.34/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.401155 adafri-0.0.19.34/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.34/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.34/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.401801 adafri-0.0.19.34/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.34/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.405427 adafri-0.0.19.34/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.34/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.34/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.34/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 05:23:14.375604 adafri-0.0.19.34/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 05:23:14.000000 adafri-0.0.19.34/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 05:23:14.408146 adafri-0.0.19.34/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.34/setup.py
```

### Comparing `adafri-0.0.19.33/adafri/utils/response.py` & `adafri-0.0.19.34/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/utils/utils.py` & `adafri-0.0.19.34/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/account/models/account.py` & `adafri-0.0.19.34/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.34/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.34/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.34/adafri/v1/auth/oauth/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .models import client
 from .models import client_fields
 from .models.client_fields import (ClientFieldProps, ClientFields)
 from .models.client import (OAuthClient)
 from .models import grant
 from .models import grant_fields
 from .models.grant_fields import (GrantFieldsProps, GrantFields)
-from .models.grant import (OAuthGrant, AuthorizationCodeGrant)
+from .models.grant import (OAuthGrant, AuthorizationCodeGrant, OpenIDCode, OpenIDImplicitGrant, OpenIDHybridGrant)
 from .models import token
 from .models import token_fields
 from .models.token_fields import (TokenFieldsProps, TokenFields)
 from .models.token import (OAuthToken, TokenGenerator, TokenValidator, RefreshTokenGrant, TokenRevocationEndpoint)
-from .server import (authorization, require_oauth,  config_oauth)
+from .server import (server, oidc_server)
```

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.34/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.34/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.34/adafri/v1/auth/oauth/models/token.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,197 @@
-from .....utils import ArrayUtils, DictUtils, Crypto, get_object_model_class, init_class_kwargs
+from .....utils import DictUtils, Crypto, get_object_model_class, pydash, init_class_kwargs
 from ....base.firebase_collection import (FirebaseCollectionBase, getTimestamp)
-from .grant_fields import GrantFields, GrantFieldsProps, STANDARD_FIELDS, GRANT_COLLECTION
+from .token_fields import TokenFields, TokenFieldsProps, STANDARD_FIELDS, TOKEN_COLLECTION
 from .....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
 from typing import Any
 from dataclasses import dataclass
-from authlib.oauth2.rfc6749 import AuthorizationCodeMixin
-from authlib.oauth2.rfc6749 import grants
-from authlib.common.urls import add_params_to_uri
-from authlib.oauth2.rfc6749.util import list_to_scope, scope_to_list
-from authlib.oauth2.rfc6749.errors import AccessDeniedError
 from ....user import User
-import pydash
+from authlib.oauth2.rfc7009 import RevocationEndpoint
+from authlib.oauth2.rfc6750 import BearerTokenValidator
+from authlib.oauth2.rfc6749 import grants
+from authlib.oauth2.rfc6749 import TokenMixin, scope_to_list
+from authlib.oauth2.rfc6750 import BearerTokenGenerator
+from datetime import datetime, timedelta
+import json
+from flask import abort, Response
 
-import os
 @dataclass(init=False)
-class OAuthGrant(AuthorizationCodeMixin, FirebaseCollectionBase):
+class OAuthToken(TokenMixin, FirebaseCollectionBase):
     id: str
-    code: str
-    uid: str
     client_id: str
-    redirect_uri: str
+    uid: str
+    token_type: str
+    access_token: str
+    refresh_token: str
     scopes: list[str]
     scope: str
-    expires: str
-    code_challenge: str
-    code_challenge_method: str
+    expired_at: str
+    expires_in: int
+    revoked: bool
     
-    def __init__(self, grant=None, **kwargs):
-        (cls_object, keys, data_args) = init_class_kwargs(self, grant, STANDARD_FIELDS, GrantFieldsProps, GRANT_COLLECTION, ['id'], **kwargs)
+    def __init__(self, token=None, **kwargs):
+        (cls_object, keys, data_args) = init_class_kwargs(self, token, STANDARD_FIELDS, TokenFieldsProps, TOKEN_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]) 
-        # kwargs['fields'] = STANDARD_FIELDS
-        # kwargs['fields_props'] = GrantFieldsProps
-        # collection_name = getattr(kwargs, 'collection_name', None)
-        # documentId = getattr(cls_object, 'id', None)
-        # if documentId is not None:
-        #     kwargs['documentId'] = documentId;
-        # if collection_name is None:
-        #     kwargs['collection_name'] = GRANT_COLLECTION;
-        
 
 
     @staticmethod
     def generate_model(_key_="default_value"):
         grant = {};
-        props = GrantFieldsProps
+        props = TokenFieldsProps
         for k in DictUtils.get_keys(props):
             grant[k] = props[k][_key_];
         return grant;
 
     @staticmethod
-    def from_dict(grant: Any=None, db=None, collection_name=None) -> 'OAuthGrant':
-        cls_object, keys = get_object_model_class(grant, OAuthGrant, GrantFieldsProps);
-        _client = OAuthGrant(cls_object, db=db, collection_name=collection_name)
+    def from_dict(token: Any=None, db=None, collection_name=None) -> 'OAuthToken':
+        cls_object, keys = get_object_model_class(token, OAuthToken, TokenFieldsProps);
+        _client = OAuthToken(cls_object, db=db, collection_name=collection_name)
         return _client
 
     def query(self, query_params: list, first=False, limit=None):
         query_result = [];
         query_result = self.custom_query(query_params, first=first, limit=limit)
         if bool(query_result):
             if first:
-                return OAuthGrant.from_dict(grant=query_result, db=self.db, collection_name=self.collection_name)
+                return OAuthToken.from_dict(token=query_result, db=self.db, collection_name=self.collection_name)
             else:
                 for doc in query_result:
-                    query_result.append(OAuthGrant.from_dict(client=doc, db=self.db, collection_name=self.collection_name))
+                    query_result.append(OAuthToken.from_dict(token=doc, db=self.db, collection_name=self.collection_name))
                 return query_result
         if first:
                 return None
         return [];
 
-    def get(self) -> 'OAuthGrant':
+    def get(self) -> 'OAuthToken':
         if bool(self.id):
-            doc = self.document_reference(self.id).get();
+            doc = self.document_reference().get();
             if doc.exists is False:
                 return None;
-            return OAuthGrant.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
+            return OAuthToken.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
         if bool(self.client_id):
             return self.query([{"key": "client_id", "comp": "==", "value": self.client_id}])
 
     @staticmethod
     def generate(**kwargs) -> 'ApiResponse':
-        data_dict = DictUtils.pick_fields(kwargs, GrantFields.filtered_keys('mutable', True));
-        authorization_code_model = OAuthGrant.from_dict(DictUtils.merge_dict(data_dict, OAuthGrant.generate_model()));
+        data_dict = DictUtils.pick_fields(kwargs, TokenFields.filtered_keys('mutable', True));
+        token_model = OAuthToken.from_dict(DictUtils.merge_dict(data_dict, OAuthToken.generate_model()));
         
-        if bool(authorization_code_model.to_json()) is False:
+        if bool(token_model.to_json()) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Empty request","INVALID_REQUEST", 1)).to_json()
         
-        if bool(authorization_code_model.code) is False:
+        if bool(token_model.access_token) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
 
-        authorization_code_model.id = Crypto().generate_id(authorization_code_model.code+"~"+authorization_code_model.client_id);
-        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, authorization_code_model, None);
-
-    def get_redirect_uri(self):
-        return self.redirect_uri
+        token_model.id = Crypto().generate_id(token_model.access_token+"~"+token_model.client_id);
+        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, token_model, None);
     
-    def get_scope(self):
-       return self.scope
-    
-    @staticmethod
-    def create(**kwargs):
-        authorization_code = OAuthGrant().generate(**kwargs);
-        if authorization_code.status == ResponseStatus.ERROR:
-            return authorization_code
-        
-        docRef = OAuthGrant(authorization_code.data).document_reference();
+
+    def save(self, token, request):
+        model = {**token, "client_id": request.client.client_id, "uid": request.client.uid, "revoked": False}
+        token_generate = OAuthToken.generate(**model);
+        if token_generate.status == ResponseStatus.ERROR:
+            return token_generate
+        docRef = OAuthToken(token_generate.data.to_json()).document_reference();
         if docRef.get().exists:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {authorization_code.id} already exist","INVALID_REQUEST", 1));
+            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
         
-        authorization_code_model: OAuthGrant = authorization_code.data;
-        docRef.set({**authorization_code_model.to_json(), "createdAt": getTimestamp()}, merge=True);
-        created_campaign = authorization_code_model.get()
-        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_campaign.to_json(), None);
+        token_model: OAuthToken = token_generate.data;
+        docRef.set({**token_model.to_json(), "createdAt": getTimestamp()}, merge=True);
+        created_token = token_model.get()
+        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_token.to_json(), None);
     
     def update(self, data):
         try:
             last_value = self.to_json();
-            filtered_value = pydash.pick(data, GrantFields.filtered_keys('editable', True));
+            filtered_value = pydash.pick(data, TokenFields.filtered_keys('editable', True));
             new_value = DictUtils.merge_dict(filtered_value, self.to_json());
             changed_fields = DictUtils.get_changed_field(last_value, new_value);
             data_update = DictUtils.dict_from_keys(filtered_value, changed_fields);
             if bool(data_update) is False:
                 return None;
             self.document_reference().set(data_update, merge=True)
             return DictUtils.dict_from_keys(self.get().to_json(), changed_fields);
         except Exception as e:
             print(e)
             return None;
     
     def remove(self):
         try:
             if self.id is None:
-                return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Cannot identify Authorization code with id {self.id} to delete","INVALID_REQUEST", 1));
+                return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Cannot identify token with id {self.id} to delete","INVALID_REQUEST", 1));
             deleted = self.document_reference().delete();
-            return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"Authorization code {self.id} deleted"}, None);
+            return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"Token {self.id} deleted"}, None);
         except:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated while removing authorization code with id {self.id}","INVALID_REQUEST", 1));
 
-    
 
-class AuthorizationCodeGrant(grants.AuthorizationCodeGrant):
-    # RESPONSE_TYPES = set({"code"})
-    TOKEN_ENDPOINT_AUTH_METHODS = [
-        'client_secret_basic',
-        'client_secret_post',
-        'none'
-    ]
-    def save_authorization_code(self, code, request):
-        code_challenge = request.data.get('code_challenge')
-        code_challenge_method = request.data.get('code_challenge_method')
-        redirect_uri = request.redirect_uri;
-        if request.args.get("redirect_uri") is not None:
-            redirect_uri = request.args.get("redirect_uri");
-        if redirect_uri is None:
-            default_redirect_uri =os.environ.get('DEFAULT_REDIRECT_URI')
-            redirect_uri = default_redirect_uri
-        model = {
-            "client_id": request.client.client_id,
-            "code": code,
-            "redirect_uri": redirect_uri,
-            "scopes": ArrayUtils.join_string_to_array(request.args.get("scope"), ","),
-            "scope": request.args.get("scope"),
-            "uid": request.user.uid,
-            "code_challenge": code_challenge,
-            "code_challenge_method": code_challenge_method
-        }
-        auth_code_request = OAuthGrant.create(**model)
-        auth_code = auth_code_request.data
-        return auth_code
-
-    
-    def query_authorization_code(self, code, client):
-        query_params = [{"key": GrantFields.code, "comp": "==","value": code}, {"key": GrantFields.client_id, "comp": "==","value": client.client_id}]
-        auth_code = OAuthGrant().query(query_params=query_params, first=True)
-        #if auth_code and not auth_code.is_expired():
-        return auth_code
-
-    def delete_authorization_code(self, authorization_code):
-        remove = OAuthGrant(authorization_code.to_json()).remove()
-        print('removing authorization code', authorization_code.id)
-
-    def authenticate_user(self, authorization_code):
-        print('search', authorization_code)
-        return User({"uid": authorization_code.uid}).get()
-    
-    def create_authorization_response(self, redirect_uri: str, grant_user):
-        if not grant_user:
-            raise AccessDeniedError(state=self.request.state, redirect_uri=redirect_uri)
-
-        self.request.user = grant_user
-        code = self.generate_authorization_code()
-        element = code;
-        element_key = "code";
-
-        self.save_authorization_code(code, self.request)
-        if self.request.response_type=="token":
-            element_key = "access_token"
-            token = self.generate_token(self.request.user, self.request.scope, self.GRANT_TYPE, 3600, True);
-            self.save_token(token);
-            element = token['access_token']
-
-        params = [(element_key, element)]
-        if self.request.state:
-            params.append(('state', self.request.state))
-        uri = add_params_to_uri(redirect_uri, params)
-        headers = [('Location', uri)]
-        return 302, '', headers
+    def is_expired(self):
+        return datetime.fromisoformat(self.expired_at) < datetime.now()
+    
+    def is_revoked(self):
+        return self.revoked
     
+
+class TokenValidator(BearerTokenValidator):
+    def authenticate_token(self, token_string):
+        token_request = OAuthToken().query([{"key":"access_token", "comp": "==", "value": token_string}], True)
+        return token_request
+    
+    def validate_token(self, token, scopes, request):
+        token_scopes = scope_to_list(token.scope);
+        print('token_scopes', token_scopes)
+        print('scopes', scopes)
+        insufficient = self.scope_insufficient(token_scopes, scopes);
+        if insufficient:
+            response = ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Insufficient privilegies","INVALID_REQUEST", 1)).to_json()
+            return abort(Response(response=json.dumps(response), status=401, mimetype='application/json'))        
+        return None
+
+class TokenRevocationEndpoint(RevocationEndpoint):
+    def query_token(self, token, token_type_hint, client):
+        q: list = OAuthToken().query([{"key":"client_id", "comp": "==", "value": client.clent_id}], False)
+        if token_type_hint == 'access_token':
+            return pydash.find(q, lambda x: x.access_token==token);
+        elif token_type_hint == 'refresh_token':
+            return pydash.find(q, lambda x: x.refresh_token==token);
+        # without token_type_hint
+        item = pydash.find(q, lambda x: x.access_token==token);
+        if item:
+            return item
+        return pydash.find(q, lambda x: x.refresh_token==token);
+
+    def revoke_token(self, _token):
+        token = OAuthToken.from_dict(_token);
+        token.revoked = True
+        token.update(_token);
+
+class RefreshTokenGrant(grants.RefreshTokenGrant):
+    def authenticate_refresh_token(self, refresh_token):
+        token = OAuthToken().query([{"key":"refresh_token", "comp": "==", "value": refresh_token}], True);
+        return token;
+        # if token and token.is_refresh_token_active():
+        #     return token
+
+    def authenticate_user(self, credential):
+        return User.get(credential.user_id)
+
+    # def revoke_old_credential(self, credential):
+    #     credential.revoked = True
+    #     db.session.add(credential)
+    #     db.session.commit()
+
+
+DEFAULT_EXPIRES_IN = 3600
+class TokenGenerator(BearerTokenGenerator):
+    @staticmethod
+    def generate(grant_type, client, user=None, scope=None, expires_in=None, include_refresh_token=True):
+        if expires_in is None:
+            expires_in = DEFAULT_EXPIRES_IN
+        expires_at = datetime.now() + timedelta(seconds=DEFAULT_EXPIRES_IN)
+        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": client.uid, 'scope': scope, 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at.isoformat()}
+        access_token = Crypto().generate_token("access_token~"+json.dumps(token));
+        token['access_token'] = access_token;
+        if include_refresh_token:
+            token['refresh_token'] = Crypto().generate_token("refresh_token~"+json.dumps(token));
+        return token
```

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.34/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     client_id = "client_id"
     redirect_uri = "redirect_uri"
     scopes = "scopes"
     scope = "scope"
     expires = "expires"
     code_challenge = "code_challenge"
     code_challenge_method = "code_challenge_method"
+    nonce = "nonce"
 
     @staticmethod
     def keys():
         return DictUtils.get_keys(GrantFieldsProps);
 
     @staticmethod
     def filtered_keys(field, condition=True):
@@ -111,11 +112,20 @@
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
         "default_value": "",
         "pickable": True
+    },
+    GrantFields.nonce: {
+        "type": str,
+        "required": True,
+        "mutable": True,
+        "editable": False,
+        "interactive": True,
+        "default_value": "",
+        "pickable": True
     },
 }
 
 STANDARD_FIELDS = GrantFields.filtered_keys('pickable', True)
```

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.34/adafri/v1/user/models/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,258 @@
-from .....utils import DictUtils, Crypto, get_object_model_class, pydash, init_class_kwargs
-from ....base.firebase_collection import (FirebaseCollectionBase, getTimestamp)
-from .token_fields import TokenFields, TokenFieldsProps, STANDARD_FIELDS, TOKEN_COLLECTION
-from .....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
+from ...base.firebase_collection import FirebaseCollectionBase
+from ....utils import (DictUtils, get_object_model_class, init_class_kwargs)
+from ....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
+from .user_fields import UserFields, UserFieldProps, STANDARD_FIELDS, USERS_COLLECTION
+from typing import List
 from typing import Any
 from dataclasses import dataclass
-from ....user import User
-from authlib.oauth2.rfc7009 import RevocationEndpoint
-from authlib.oauth2.rfc6750 import BearerTokenValidator
-from authlib.oauth2.rfc6749 import grants
-from authlib.oauth2.rfc6749 import TokenMixin, scope_to_list
-from authlib.oauth2.rfc6750 import BearerTokenGenerator
-from datetime import datetime, timedelta
-import json
-from flask import abort, Response
+from firebase_admin import auth as admin_auth
+from firebase_admin.exceptions import FirebaseError
+import pydash
+
+@dataclass
+class Account:
+    canManageClients: bool
+    childs: List[object]
+    currenyCode: str
+    customerId: int
+    dateTimeZone: str
+    name: str
+    testAccount: bool
 
-@dataclass(init=False)
-class OAuthToken(TokenMixin, FirebaseCollectionBase):
+    @staticmethod
+    def from_dict(obj: Any) -> 'Account':
+        _canManageClients = DictUtils.pick(obj, "canManageClients", bool)
+        _childs = [y for y in DictUtils.pick(obj, "childs", list)]
+        _currenyCode = str(DictUtils.pick(obj, "currenyCode", str))
+        _customerId = int(DictUtils.pick(obj, "customerId", int))
+        _dateTimeZone = str(DictUtils.pick(obj, "dateTimeZone",str))
+        _name = str(DictUtils.pick(obj, "name", str))
+        _testAccount = bool(DictUtils.pick(obj, "testAccount", bool))
+        return Account(_canManageClients, _childs, _currenyCode, _customerId, _dateTimeZone, _name, _testAccount)
+
+@dataclass
+class Country:
+    areaCodes: List[object]
+    dialCode: str
+    flagClass: str
+    htmlId: str
+    iso2: str
+    name: str
+    placeHolder: str
+    priority: int
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'Country':
+        _areaCodes = [y for y in DictUtils.pick(obj, "areaCodes", list)]
+        _dialCode = str(DictUtils.pick(obj, "dialCode", str))
+        _flagClass = str(DictUtils.pick(obj, "flagClass",str))
+        _htmlId = str(DictUtils.pick(obj, "htmlId", str))
+        _iso2 = str(DictUtils.pick(obj, "iso2", str))
+        _name = str(DictUtils.pick(obj, "name", str))
+        _placeHolder = str(DictUtils.pick(obj, "placeHolder", str))
+        _priority = int(DictUtils.pick(obj, "priority", int))
+        return Country(_areaCodes, _dialCode, _flagClass, _htmlId, _iso2, _name, _placeHolder, _priority)
+
+@dataclass
+class Credential:
+    refresh_token: str
+    scopes: List[str]
+    token: str
+    token_uri: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'Credential':
+        _refresh_token = str(DictUtils.pick(obj, "refresh_token", str))
+        _scopes = [y for y in DictUtils.pick(obj, "scopes", list)]
+        _token = str(DictUtils.pick(obj, "token", str))
+        _token_uri = str(DictUtils.pick(obj, "token_uri", str))
+        return Credential(_refresh_token, _scopes, _token, _token_uri)
+
+@dataclass
+class DeviceInfo:
+    browser: str
+    browser_version: str
+    device: str
+    os: str
+    os_version: str
+    userAgent: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'DeviceInfo':
+        _browser = str(DictUtils.pick(obj, "browser", str))
+        _browser_version = str(DictUtils.pick(obj, "browser_version", str))
+        _device = str(DictUtils.pick(obj, "device", str))
+        _os = str(DictUtils.pick(obj, "os", str))
+        _os_version = str(DictUtils.pick(obj, "os_version", str))
+        _userAgent = str(DictUtils.pick(obj, "userAgent", str))
+        return DeviceInfo(_browser, _browser_version, _device, _os, _os_version, _userAgent)
+
+@dataclass
+class PartenerData:
+    id: str
+    text: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'PartenerData':
+        _id = str(DictUtils.pick(obj, "id", str))
+        _text = str(DictUtils.pick(obj, "text", str))
+        return PartenerData(_id, _text)
+
+@dataclass
+class PhoneInfo:
+    countryCode: str
+    dialCode: str
+    e164Number: str
+    internationalNumber: str
+    nationalNumber: str
+    number: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'PhoneInfo':
+        _countryCode = str(DictUtils.pick(obj, "countryCode", str))
+        _dialCode = str(DictUtils.pick(obj, "dialCode", str))
+        _e164Number = str(DictUtils.pick(obj, "e164Number", str))
+        _internationalNumber = str(DictUtils.pick(obj, "internationalNumber", str))
+        _nationalNumber = str(DictUtils.pick(obj, "nationalNumber", str))
+        _number = str(DictUtils.pick(obj, "number", str))
+        return PhoneInfo(_countryCode, _dialCode, _e164Number, _internationalNumber, _nationalNumber, _number)
+
+@dataclass
+class PlateformRole:
     id: str
-    client_id: str
+    partenerData: PartenerData
+    text: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'PlateformRole':
+        _id = str(DictUtils.pick(obj, "id", str))
+        _partenerData = PartenerData.from_dict(DictUtils.pick(obj, "partenerData", dict))
+        _text = str(DictUtils.pick(obj, "text", str))
+        return PlateformRole(_id, _partenerData, _text)
+
+
+@dataclass(init=False)
+class User(FirebaseCollectionBase):
+    account_value: int = None;
+    accounts: List[Account]
+    addresse: str
+    auth_code: str
+    authorizedPush: bool
+    country: Country
+    credentials: List[Credential]
+    deviceInfo: DeviceInfo
+    displayName: str
+    email: str
+    entrepriseName: str
+    entrepriseUrl: str
+    first_name: str
+    hasApprouvedPolicy: bool
+    invitedAccounts: List[object]
+    isConnectWithMailAndPassword: bool
+    isCorporate: bool
+    isDesktopDevice: bool
+    isMobile: bool
+    isParticular: bool
+    isTablet: bool
+    last_name: str
+    linkedAccounts: List[object]
+    ownedAccounts: List[object]
+    phoneInfo: PhoneInfo
+    photoURL: str
+    plateformRole: PlateformRole
+    postal: str
+    profileCompleted: bool
+    showPushToken: bool
+    telephone: str
+    token: List[str]
     uid: str
-    token_type: str
-    access_token: str
-    refresh_token: str
-    scopes: list[str]
-    scope: str
-    expired_at: str
-    expires_in: int
-    revoked: bool
+    user_type: str
+    password: str
+    provider: str
     
-    def __init__(self, token=None, **kwargs):
-        (cls_object, keys, data_args) = init_class_kwargs(self, token, STANDARD_FIELDS, TokenFieldsProps, TOKEN_COLLECTION, ['id'], **kwargs)
+    def __init__(self, user, **kwargs):
+        (cls_object, keys, data_args) = init_class_kwargs(self, user, STANDARD_FIELDS, UserFieldProps, USERS_COLLECTION, ['id','uid'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
-            setattr(self, key, cls_object[key]) 
+            setattr(self, key, cls_object[key]);
+    
 
 
     @staticmethod
     def generate_model(_key_="default_value"):
-        grant = {};
-        props = TokenFieldsProps
+        user = {};
+        props = UserFieldProps
         for k in DictUtils.get_keys(props):
-            grant[k] = props[k][_key_];
-        return grant;
+            user[k] = props[k][_key_];
+        return user;
 
     @staticmethod
-    def from_dict(token: Any=None, db=None, collection_name=None) -> 'OAuthToken':
-        cls_object, keys = get_object_model_class(token, OAuthToken, TokenFieldsProps);
-        _client = OAuthToken(cls_object, db=db, collection_name=collection_name)
-        return _client
+    def from_dict(user: Any, db=None, collection_name=USERS_COLLECTION) -> 'User':
+        cls_object, keys = get_object_model_class(user, User, UserFieldProps);
+        _user = User(cls_object, db=db, collection_name=collection_name)
+        return _user
+    
+    def get(self):
+        doc = self.document_reference().get();
+        if doc.exists is False:
+            return None;
+        return User.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
 
     def query(self, query_params: list, first=False, limit=None):
         query_result = [];
         query_result = self.custom_query(query_params, first=first, limit=limit)
         if bool(query_result):
             if first:
-                return OAuthToken.from_dict(token=query_result, db=self.db, collection_name=self.collection_name)
+                return User.from_dict(user=query_result, db=self.db, collection_name=self.collection_name)
             else:
                 for doc in query_result:
-                    query_result.append(OAuthToken.from_dict(token=doc, db=self.db, collection_name=self.collection_name))
+                    query_result.append(User.from_dict(user=doc, db=self.db, collection_name=self.collection_name))
                 return query_result
         if first:
                 return None
         return [];
-
-    def get(self) -> 'OAuthToken':
-        if bool(self.id):
-            doc = self.document_reference().get();
-            if doc.exists is False:
-                return None;
-            return OAuthToken.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
-        if bool(self.client_id):
-            return self.query([{"key": "client_id", "comp": "==", "value": self.client_id}])
-
-    @staticmethod
-    def generate(**kwargs) -> 'ApiResponse':
-        data_dict = DictUtils.pick_fields(kwargs, TokenFields.filtered_keys('mutable', True));
-        token_model = OAuthToken.from_dict(DictUtils.merge_dict(data_dict, OAuthToken.generate_model()));
-        
-        if bool(token_model.to_json()) is False:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Empty request","INVALID_REQUEST", 1)).to_json()
-        
-        if bool(token_model.access_token) is False:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
-
-        token_model.id = Crypto().generate_id(token_model.access_token+"~"+token_model.client_id);
-        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, token_model, None);
-    
-
-    def save(self, token, request):
-        model = {**token, "client_id": request.client.client_id, "uid": request.client.uid, "revoked": False}
-        token_generate = OAuthToken.generate(**model);
-        if token_generate.status == ResponseStatus.ERROR:
-            return token_generate
-        docRef = OAuthToken(token_generate.data.to_json()).document_reference();
-        if docRef.get().exists:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
-        
-        token_model: OAuthToken = token_generate.data;
-        docRef.set({**token_model.to_json(), "createdAt": getTimestamp()}, merge=True);
-        created_token = token_model.get()
-        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_token.to_json(), None);
     
     def update(self, data):
         try:
             last_value = self.to_json();
-            filtered_value = pydash.pick(data, TokenFields.filtered_keys('editable', True));
+            filtered_value = pydash.pick(data, UserFields.filtered_keys('editable', True));
             new_value = DictUtils.merge_dict(filtered_value, self.to_json());
             changed_fields = DictUtils.get_changed_field(last_value, new_value);
             data_update = DictUtils.dict_from_keys(filtered_value, changed_fields);
             if bool(data_update) is False:
                 return None;
             self.document_reference().set(data_update, merge=True)
             return DictUtils.dict_from_keys(self.get().to_json(), changed_fields);
         except Exception as e:
             print(e)
             return None;
-    
-    def remove(self):
+
+    def remove(self, only_mark_as_removed=True):
         try:
             if self.id is None:
-                return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Cannot identify token with id {self.id} to delete","INVALID_REQUEST", 1));
-            deleted = self.document_reference().delete();
-            return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"Token {self.id} deleted"}, None);
+                return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Cannot identify User with id {self.id}","INVALID_REQUEST", 1));
+            if only_mark_as_removed:
+                self.document_reference().set({"is_removed": True})
+            else:
+                self.document_reference().delete();
+            return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"User {self.id} deleted"}, None);
         except:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated while removing authorization code with id {self.id}","INVALID_REQUEST", 1));
 
-
-    def is_expired(self):
-        return datetime.fromisoformat(self.expired_at) < datetime.now()
-    
-    def is_revoked(self):
-        return self.revoked
     
+    def get_firebase_user(self, key: str, value: str) -> 'admin_auth.UserRecord':
+        try:
+            if key == 'email':
+                return admin_auth.get_user_by_email(value)
+            elif key == 'uid':
+                return admin_auth.get_user(value)
+            elif key == 'phone':
+                return admin_auth.get_user_by_phone_number(value)
+        except ValueError as e:
+            raise e
+        except FirebaseError as e:
+            raise e;    
+        except admin_auth.UserNotFoundError as e:
+            raise e;  
+
 
-class TokenValidator(BearerTokenValidator):
-    def authenticate_token(self, token_string):
-        token_request = OAuthToken().query([{"key":"access_token", "comp": "==", "value": token_string}], True)
-        return token_request
-    
-    def validate_token(self, token, scopes, request):
-        token_scopes = scope_to_list(token.scope);
-        print('token_scopes', token_scopes)
-        print('scopes', scopes)
-        insufficient = self.scope_insufficient(token_scopes, scopes);
-        if insufficient:
-            response = ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Insufficient privilegies","INVALID_REQUEST", 1)).to_json()
-            return abort(Response(response=json.dumps(response), status=401, mimetype='application/json'))        
-        return None
-
-class TokenRevocationEndpoint(RevocationEndpoint):
-    def query_token(self, token, token_type_hint, client):
-        q: list = OAuthToken().query([{"key":"client_id", "comp": "==", "value": client.clent_id}], False)
-        if token_type_hint == 'access_token':
-            return pydash.find(q, lambda x: x.access_token==token);
-        elif token_type_hint == 'refresh_token':
-            return pydash.find(q, lambda x: x.refresh_token==token);
-        # without token_type_hint
-        item = pydash.find(q, lambda x: x.access_token==token);
-        if item:
-            return item
-        return pydash.find(q, lambda x: x.refresh_token==token);
-
-    def revoke_token(self, _token):
-        token = OAuthToken.from_dict(_token);
-        token.revoked = True
-        token.update(_token);
-
-class RefreshTokenGrant(grants.RefreshTokenGrant):
-    def authenticate_refresh_token(self, refresh_token):
-        token = OAuthToken().query([{"key":"refresh_token", "comp": "==", "value": refresh_token}], True);
-        return token;
-        # if token and token.is_refresh_token_active():
-        #     return token
-
-    def authenticate_user(self, credential):
-        return User.get(credential.user_id)
-
-    # def revoke_old_credential(self, credential):
-    #     credential.revoked = True
-    #     db.session.add(credential)
-    #     db.session.commit()
-
-
-DEFAULT_EXPIRES_IN = 3600
-class TokenGenerator(BearerTokenGenerator):
-    @staticmethod
-    def generate(grant_type, client, user=None, scope=None, expires_in=None, include_refresh_token=True):
-        if expires_in is None:
-            expires_in = DEFAULT_EXPIRES_IN
-        expires_at = datetime.now() + timedelta(seconds=DEFAULT_EXPIRES_IN)
-        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": client.uid, 'scope': scope, 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at.isoformat()}
-        access_token = Crypto().generate_token("access_token~"+json.dumps(token));
-        token['access_token'] = access_token;
-        if include_refresh_token:
-            token['refresh_token'] = Crypto().generate_token("refresh_token~"+json.dumps(token));
-        return token
```

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.34/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/auth/oauth/server/__init__.py` & `adafri-0.0.19.34/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.34/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.34/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.33/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.34/adafri.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,13 +21,15 @@
 adafri/v1/auth/oauth/models/client.py
 adafri/v1/auth/oauth/models/client_fields.py
 adafri/v1/auth/oauth/models/grant.py
 adafri/v1/auth/oauth/models/grant_fields.py
 adafri/v1/auth/oauth/models/token.py
 adafri/v1/auth/oauth/models/token_fields.py
 adafri/v1/auth/oauth/server/__init__.py
+adafri/v1/auth/oauth/server/oidc_server.py
+adafri/v1/auth/oauth/server/server.py
 adafri/v1/base/__init__.py
 adafri/v1/base/firebase_collection.py
 adafri/v1/user/__init__.py
 adafri/v1/user/models/__init__.py
 adafri/v1/user/models/user.py
 adafri/v1/user/models/user_fields.py
```

### Comparing `adafri-0.0.19.33/setup.py` & `adafri-0.0.19.34/setup.py`

 * *Files identical despite different names*

