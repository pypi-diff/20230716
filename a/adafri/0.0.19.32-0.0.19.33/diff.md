# Comparing `tmp/adafri-0.0.19.32.tar.gz` & `tmp/adafri-0.0.19.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.32.tar", last modified: Sat Jul 15 08:15:26 2023, max compression
+gzip compressed data, was "adafri-0.0.19.33.tar", last modified: Sun Jul 16 01:52:35 2023, max compression
```

## Comparing `adafri-0.0.19.32.tar` & `adafri-0.0.19.33.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.683614 adafri-0.0.19.32/
--rw-r--r--   0 ibrahima   (502) staff       (20)      496 2023-07-15 08:15:26.683107 adafri-0.0.19.32/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.653950 adafri-0.0.19.32/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.19.32/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.659134 adafri-0.0.19.32/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.32/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.32/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.32/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.659885 adafri-0.0.19.32/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.19.32/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.660713 adafri-0.0.19.32/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.32/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.663115 adafri-0.0.19.32/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.32/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.32/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.32/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.663982 adafri-0.0.19.32/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.19.32/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.665668 adafri-0.0.19.32/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.32/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.32/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.666569 adafri-0.0.19.32/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.32/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.666874 adafri-0.0.19.32/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.673697 adafri-0.0.19.32/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9475 2023-07-15 08:08:12.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:15:04.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.675707 adafri-0.0.19.32/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.32/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.32/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.676403 adafri-0.0.19.32/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.32/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.681695 adafri-0.0.19.32/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.32/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.32/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.32/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.656699 adafri-0.0.19.32/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      496 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-15 08:15:26.683843 adafri-0.0.19.32/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1010 2023-07-15 08:15:20.000000 adafri-0.0.19.32/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.463683 adafri-0.0.19.33/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 01:52:35.463323 adafri-0.0.19.33/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.437827 adafri-0.0.19.33/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-16 01:46:28.000000 adafri-0.0.19.33/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.442540 adafri-0.0.19.33/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.33/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.33/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.33/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.443346 adafri-0.0.19.33/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      137 2023-07-16 01:52:16.000000 adafri-0.0.19.33/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.444233 adafri-0.0.19.33/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.33/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.446623 adafri-0.0.19.33/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.33/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.33/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.33/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.447712 adafri-0.0.19.33/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      314 2023-07-16 01:50:48.000000 adafri-0.0.19.33/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.449337 adafri-0.0.19.33/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.33/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.33/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.450201 adafri-0.0.19.33/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.33/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.450559 adafri-0.0.19.33/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      660 2023-07-16 01:49:50.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.456476 adafri-0.0.19.33/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9475 2023-07-15 08:08:12.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.457610 adafri-0.0.19.33/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1907 2023-07-16 01:45:10.000000 adafri-0.0.19.33/adafri/v1/auth/oauth/server/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.459225 adafri-0.0.19.33/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.33/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.33/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.460085 adafri-0.0.19.33/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.33/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.462299 adafri-0.0.19.33/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.33/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.33/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.33/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-16 01:52:35.440365 adafri-0.0.19.33/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1086 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-16 01:52:35.000000 adafri-0.0.19.33/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-16 01:52:35.463832 adafri-0.0.19.33/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.33/setup.py
```

### Comparing `adafri-0.0.19.32/adafri/utils/response.py` & `adafri-0.0.19.33/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/utils/utils.py` & `adafri-0.0.19.33/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/account/models/account.py` & `adafri-0.0.19.33/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.33/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.33/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.33/adafri/v1/auth/oauth/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 from .models import grant
 from .models import grant_fields
 from .models.grant_fields import (GrantFieldsProps, GrantFields)
 from .models.grant import (OAuthGrant, AuthorizationCodeGrant)
 from .models import token
 from .models import token_fields
 from .models.token_fields import (TokenFieldsProps, TokenFields)
-from .models.token import (OAuthToken, TokenGenerator, TokenValidator, RefreshTokenGrant, TokenRevocationEndpoint)
+from .models.token import (OAuthToken, TokenGenerator, TokenValidator, RefreshTokenGrant, TokenRevocationEndpoint)
+from .server import (authorization, require_oauth,  config_oauth)
```

### Comparing `adafri-0.0.19.32/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.33/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.33/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.33/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.33/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.33/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.33/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/user/models/user.py` & `adafri-0.0.19.33/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.33/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.32/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.33/adafri.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 adafri/v1/auth/oauth/models/__init__.py
 adafri/v1/auth/oauth/models/client.py
 adafri/v1/auth/oauth/models/client_fields.py
 adafri/v1/auth/oauth/models/grant.py
 adafri/v1/auth/oauth/models/grant_fields.py
 adafri/v1/auth/oauth/models/token.py
 adafri/v1/auth/oauth/models/token_fields.py
+adafri/v1/auth/oauth/server/__init__.py
 adafri/v1/base/__init__.py
 adafri/v1/base/firebase_collection.py
 adafri/v1/user/__init__.py
 adafri/v1/user/models/__init__.py
 adafri/v1/user/models/user.py
 adafri/v1/user/models/user_fields.py
```

### Comparing `adafri-0.0.19.32/setup.py` & `adafri-0.0.19.33/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from setuptools import setup, find_packages
-
-VERSION = '0.0.19.32' 
+from adafri import __version__
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module helper'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri", 
-        version=VERSION,
+        version=__version__,
         author="Ibrahima Touré",
         author_email="ibrahima.toure.dev@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=[], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
-        keywords=['python', 'first package'],
-        classifiers= [
-            "Development Status :: 3 - Alpha",
-            "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
-            "Programming Language :: Python :: 3",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
-        ]
+        keywords=[],
+        classifiers= []
 )
```

