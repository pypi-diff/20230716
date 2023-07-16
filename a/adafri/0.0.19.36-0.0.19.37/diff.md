# Comparing `tmp/adafri-0.0.19.36.tar.gz` & `tmp/adafri-0.0.19.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.36.tar", last modified: Sun Jul 16 06:12:42 2023, max compression
+gzip compressed data, was "adafri-0.0.19.37.tar", last modified: Sun Jul 16 07:54:17 2023, max compression
```

## Comparing `adafri-0.0.19.36.tar` & `adafri-0.0.19.37.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.222560 adafri-0.0.19.36/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 06:12:42.222295 adafri-0.0.19.36/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.201919 adafri-0.0.19.36/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 06:12:32.000000 adafri-0.0.19.36/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.205166 adafri-0.0.19.36/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.36/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.36/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.36/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.205835 adafri-0.0.19.36/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.36/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.206200 adafri-0.0.19.36/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.36/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.208096 adafri-0.0.19.36/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.36/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.36/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.36/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.208959 adafri-0.0.19.36/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.36/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.209950 adafri-0.0.19.36/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.36/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.36/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.210699 adafri-0.0.19.36/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.36/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.211080 adafri-0.0.19.36/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      784 2023-07-16 05:40:08.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.215831 adafri-0.0.19.36/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11644 2023-07-16 05:17:11.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.217739 adafri-0.0.19.36/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1657 2023-07-16 05:38:24.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.36/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.219197 adafri-0.0.19.36/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.36/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.36/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.219549 adafri-0.0.19.36/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.36/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.221420 adafri-0.0.19.36/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.36/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.36/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.36/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 06:12:42.203449 adafri-0.0.19.36/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 06:12:42.000000 adafri-0.0.19.36/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-16 06:12:42.000000 adafri-0.0.19.36/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 06:12:42.000000 adafri-0.0.19.36/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 06:12:42.000000 adafri-0.0.19.36/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 06:12:42.222664 adafri-0.0.19.36/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.36/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.025404 adafri-0.0.19.37/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 07:54:17.025142 adafri-0.0.19.37/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.004167 adafri-0.0.19.37/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 07:54:11.000000 adafri-0.0.19.37/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.007948 adafri-0.0.19.37/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.37/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.37/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.37/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.008723 adafri-0.0.19.37/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.37/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.009377 adafri-0.0.19.37/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.37/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.011397 adafri-0.0.19.37/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.37/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.37/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.37/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.012243 adafri-0.0.19.37/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.37/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.013271 adafri-0.0.19.37/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.37/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.37/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.014257 adafri-0.0.19.37/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.37/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.014562 adafri-0.0.19.37/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-16 07:53:07.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.019059 adafri-0.0.19.37/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    13674 2023-07-16 07:52:25.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.020622 adafri-0.0.19.37/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)      885 2023-07-16 07:54:02.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.37/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.021809 adafri-0.0.19.37/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.37/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.37/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.022230 adafri-0.0.19.37/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.37/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.024356 adafri-0.0.19.37/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.37/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.37/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.37/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 07:54:17.005927 adafri-0.0.19.37/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 07:54:16.000000 adafri-0.0.19.37/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 07:54:17.025513 adafri-0.0.19.37/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.37/setup.py
```

### Comparing `adafri-0.0.19.36/adafri/utils/response.py` & `adafri-0.0.19.37/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/utils/utils.py` & `adafri-0.0.19.37/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/account/models/account.py` & `adafri-0.0.19.37/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.37/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.37/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .models import client
 from .models import client_fields
 from .models.client_fields import (ClientFieldProps, ClientFields)
 from .models.client import (OAuthClient)
 from .models import grant
 from .models import grant_fields
 from .models.grant_fields import (GrantFieldsProps, GrantFields)
-from .models.grant import (OAuthGrant, AuthorizationCodeGrant, OpenIDCode, OpenIDImplicitGrant, OpenIDHybridGrant)
+from .models.grant import (OAuthGrant, AuthorizationCodeGrant, OpenIDCode, OpenIDImplicitGrant, OpenIDHybridGrant, OpenIDAuthorizationCodeGrant)
 from .models import token
 from .models import token_fields
 from .models.token_fields import (TokenFieldsProps, TokenFields)
 from .models.token import (OAuthToken, TokenGenerator, TokenValidator, RefreshTokenGrant, TokenRevocationEndpoint)
 from .server import (oidc_authorization_server, authorization_server, require_oauth, require_oidc_oauth, config_oauth, config_oidc_oauth)
```

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant.py`

 * *Files 11% similar despite different names*

```diff
@@ -245,14 +245,61 @@
         "scope":request.scope,
         "uid": grant_user.id,
         "nonce": nonce,
     }
     auth_code = OAuthGrant.create(**grant)
     return auth_code.data
 
+class OpenIDAuthorizationCodeGrant(grants.AuthorizationCodeGrant):
+    # RESPONSE_TYPES = set({"code"})
+    # TOKEN_ENDPOINT_AUTH_METHODS = [
+    #     'client_secret_basic',
+    #     'client_secret_post',
+    #     'none'
+    # ]
+    def create_authorization_code(self, client, grant_user, request):
+        return create_authorization_code(client, grant_user, request)
+    
+    def parse_authorization_code(self, code, client):
+        query_params = [{"key": GrantFields.code, "comp": "==","value": code}, {"key": GrantFields.client_id, "comp": "==","value": client.client_id}]
+        auth_code = OAuthGrant().query(query_params=query_params, first=True)
+        #if auth_code and not auth_code.is_expired():
+        return auth_code
+
+    def delete_authorization_code(self, authorization_code):
+        remove = OAuthGrant(authorization_code.to_json()).remove()
+        print('removing authorization code', authorization_code.id)
+
+    def authenticate_user(self, authorization_code):
+        print('search', authorization_code)
+        return User({"uid": authorization_code.uid}).get()
+    
+    def create_authorization_response(self, redirect_uri: str, grant_user):
+        if not grant_user:
+            raise AccessDeniedError(state=self.request.state, redirect_uri=redirect_uri)
+
+        self.request.user = grant_user
+        code = self.generate_authorization_code()
+        element = code;
+        element_key = "code";
+
+        self.save_authorization_code(code, self.request)
+        if self.request.response_type=="token":
+            element_key = "access_token"
+            token = self.generate_token(self.request.user, self.request.scope, self.GRANT_TYPE, 3600, True);
+            self.save_token(token);
+            element = token['access_token']
+
+        params = [(element_key, element)]
+        if self.request.state:
+            params.append(('state', self.request.state))
+        uri = add_params_to_uri(redirect_uri, params)
+        headers = [('Location', uri)]
+        return 302, '', headers
+    
 class OpenIDCode(_OpenIDCode):
     def exists_nonce(self, nonce, request):
         return exists_nonce(nonce, request)
 
     def get_jwt_config(self, grant):
         return DUMMY_JWT_CONFIG
```

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.19.37/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.37/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/user/models/user.py` & `adafri-0.0.19.37/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.37/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.37/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.36/setup.py` & `adafri-0.0.19.37/setup.py`

 * *Files identical despite different names*

