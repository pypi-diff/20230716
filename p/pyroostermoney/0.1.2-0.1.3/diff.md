# Comparing `tmp/pyroostermoney-0.1.2.tar.gz` & `tmp/pyroostermoney-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.2.tar", last modified: Sat Jul 15 22:22:38 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.3.tar", last modified: Sat Jul 15 22:55:34 2023, max compression
```

## Comparing `pyroostermoney-0.1.2.tar` & `pyroostermoney-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.584741 pyroostermoney-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.005233 pyroostermoney-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.009233 pyroostermoney-0.1.3/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.009233 pyroostermoney-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.009233 pyroostermoney-0.1.3/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-15 22:55:34.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/setup.py
```

### Comparing `pyroostermoney-0.1.2/.github/scripts/release.py` & `pyroostermoney-0.1.3/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/.github/workflows/build.yml` & `pyroostermoney-0.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/.gitignore` & `pyroostermoney-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/LICENSE` & `pyroostermoney-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/PKG-INFO` & `pyroostermoney-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.2
+Version: 0.1.3
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.2/pyroostermoney/api.py` & `pyroostermoney-0.1.3/pyroostermoney/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         req_body = LOGIN_BODY
         req_body["username"] = self._username
         req_body["password"] = self._password
         auth = aiohttp.BasicAuth(self._username, self._password)
 
         login_response = await self.internal_request_handler(url=URLS.get("login"),
                                                               body=req_body,
-                                                              auth=auth)
+                                                              auth=auth,
+                                                              headers=HEADERS)
 
         if login_response["status"] == 401:
             raise InvalidAuthError(self._username, login_response["status"])
 
         login_response = login_response["response"]
 
         self._session = {
@@ -85,15 +86,17 @@
                                         auth=None,
                                         method="GET"):
         """Handles all incoming requests to make sure that the session is active."""
         if self._session is None and self._logged_in:
             raise RuntimeError("Invalid state. Missing session data yet currently logged in?")
         elif self._session is None and self._logged_in is False and auth is not None:
             _LOGGER.info("Not logged in, trying now.")
-            return await _post_request(url, body, auth, self._headers)
+            if headers is None:
+                headers = self._headers
+            return await _post_request(url, body, auth, headers)
         elif self._session is None and self._logged_in is False and auth is None:
             raise NotLoggedIn()
         elif self._session is not None and self._logged_in is False:
             raise RuntimeError("Invalid state. Session data available yet not logged in?")
 
         # Check if auth has expired
```

### Comparing `pyroostermoney-0.1.2/pyroostermoney/child/__init__.py` & `pyroostermoney-0.1.3/pyroostermoney/child/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/pyroostermoney/const.py` & `pyroostermoney-0.1.3/pyroostermoney/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Static Rooster Money variables"""
 
-VERSION="0.1.2"
+VERSION="0.1.3"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
```

### Comparing `pyroostermoney-0.1.2/pyroostermoney/exceptions.py` & `pyroostermoney-0.1.3/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/pyroostermoney/family_account.py` & `pyroostermoney-0.1.3/pyroostermoney/family_account.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/pyroostermoney/roostermoney.py` & `pyroostermoney-0.1.3/pyroostermoney/roostermoney.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.2/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.3/pyroostermoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.2
+Version: 0.1.3
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.2/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.3/pyroostermoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

