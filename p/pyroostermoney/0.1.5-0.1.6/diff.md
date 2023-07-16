# Comparing `tmp/pyroostermoney-0.1.5.tar.gz` & `tmp/pyroostermoney-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.5.tar", last modified: Sun Jul 16 15:20:23 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.6.tar", last modified: Sun Jul 16 21:42:07 2023, max compression
```

## Comparing `pyroostermoney-0.1.5.tar` & `pyroostermoney-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.747338 pyroostermoney-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.747338 pyroostermoney-0.1.5/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.751338 pyroostermoney-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.751338 pyroostermoney-0.1.5/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/child/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/child/money_pot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.751338 pyroostermoney-0.1.5/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.316297 pyroostermoney-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/setup.py
```

### Comparing `pyroostermoney-0.1.5/.github/scripts/release.py` & `pyroostermoney-0.1.6/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.5/.github/workflows/build.yml` & `pyroostermoney-0.1.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.5/.gitignore` & `pyroostermoney-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.5/LICENSE` & `pyroostermoney-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.5/PKG-INFO` & `pyroostermoney-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.5
+Version: 0.1.6
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.5/pyroostermoney/api.py` & `pyroostermoney-0.1.6/pyroostermoney/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Rooster Money requests and session handler."""
 
 import json
 import logging
 import base64
+import asyncio
 from datetime import datetime, timedelta
 
 import aiohttp
 
 from .const import HEADERS, BASE_URL, LOGIN_BODY, URLS
 from .exceptions import InvalidAuthError, NotLoggedIn, AuthenticationExpired
 
@@ -42,55 +43,64 @@
 
     def __init__(self, username: str, password: str) -> None:
         self._username = username
         self._password = password
         self._session = None
         self._headers = HEADERS
         self._logged_in = False
+        self._logging_in = asyncio.Lock()
 
     async def async_login(self):
         """Logs into RoosterMoney and starts a new active session."""
-        if self._session is not None:
-            if self._session.get("expiry_time") > datetime.now():
-                _LOGGER.debug("Not logging in again, session already active.")
-                return True
-
-        req_body = LOGIN_BODY
-        req_body["username"] = self._username
-        req_body["password"] = self._password
-        auth = aiohttp.BasicAuth(self._username, self._password)
-
-        if "Authorization" in self._headers:
-            self._headers.pop("Authorization")
-
-        login_response = await self.request_handler(url=URLS.get("login"),
-                                                              body=req_body,
-                                                              auth=auth,
-                                                              headers=self._headers)
-
-        if login_response["status"] == 401:
-            raise InvalidAuthError(self._username, login_response["status"])
-
-        login_response = login_response["response"]
-        token = base64.b64encode(str(self._password[::-1]).encode('utf-8')).decode('utf-8')
-
-        self._session = {
-            "access_token": login_response["tokens"]["access_token"],
-            "refresh_token": login_response["tokens"]["refresh_token"],
-            "token_type": login_response["tokens"]["token_type"],
-            "expiry_time": datetime.now() + timedelta(0, login_response["tokens"]["expires_in"]),
-            "security_code": token
-        }
+        if self._logging_in.locked():
+            _LOGGER.warning("Login already attempting. Only one execution allowed.")
+            while self._logging_in.locked():
+                await asyncio.sleep(1)
+            return True
+
+        async with self._logging_in:
+            if self._session is not None:
+                if self._session.get("expiry_time") > datetime.now():
+                    _LOGGER.debug("Not logging in again, session already active.")
+                    return True
+
+            req_body = LOGIN_BODY
+            req_body["username"] = self._username
+            req_body["password"] = self._password
+            auth = aiohttp.BasicAuth(self._username, self._password)
+
+            if "Authorization" in self._headers:
+                self._headers.pop("Authorization")
+
+            login_response = await self.request_handler(url=URLS.get("login"),
+                                                                body=req_body,
+                                                                auth=auth,
+                                                                headers=self._headers)
+
+            if login_response["status"] == 401:
+                raise InvalidAuthError(self._username, login_response["status"])
+
+            login_response = login_response["response"]
+            token = base64.b64encode(str(self._password[::-1]).encode('utf-8')).decode('utf-8')
+
+            self._session = {
+                "access_token": login_response["tokens"]["access_token"],
+                "refresh_token": login_response["tokens"]["refresh_token"],
+                "token_type": login_response["tokens"]["token_type"],
+                "expiry_time": datetime.now() + timedelta(0,
+                                                          login_response["tokens"]["expires_in"]),
+                "security_code": token
+            }
 
-        token_type = login_response["tokens"]["token_type"]
-        access_token = login_response["tokens"]["access_token"]
+            token_type = login_response["tokens"]["token_type"]
+            access_token = login_response["tokens"]["access_token"]
 
-        self._headers["Authorization"] = f"{token_type} {access_token}"
+            self._headers["Authorization"] = f"{token_type} {access_token}"
 
-        self._logged_in = True
+            self._logged_in = True
 
         return True
 
     async def _internal_request_handler(self,
                                         url,
                                         body=None,
                                         headers=None,
@@ -107,21 +117,20 @@
             if headers is None:
                 headers = self._headers
             return await _post_request(url, body, auth, headers)
         elif self._session is None and self._logged_in is False and auth is None:
             raise NotLoggedIn()
         elif self._session is not None and self._logged_in is False:
             raise RuntimeError("Invalid state. Session data available yet not logged in?")
-
-        # Check if auth has expired
-
-        if login_request:
+        elif self._session["expiry_time"] < datetime.now() and login_request:
             _LOGGER.debug("Login request.")
             return await _post_request(url, body, auth, headers)
 
+        # Check if auth has expired
+
         if self._session["expiry_time"] < datetime.now():
             raise AuthenticationExpired()
 
         if headers is None:
             headers = self._headers
 
         if add_security_token:
```

### Comparing `pyroostermoney-0.1.5/pyroostermoney/child/__init__.py` & `pyroostermoney-0.1.6/pyroostermoney/child/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         self.available_pocket_money = raw_response["availablePocketMoney"]
         self.currency = raw_response["currency"]
         self.first_name = raw_response["firstName"]
         self.surname = raw_response["surname"]
         self.gender = "male" if raw_response["gender"] == 1 else "female"
         self.uses_real_money = True if raw_response["realMoneyStatus"] == 1 else False
         self.user_id = raw_response["userId"]
+        self.profile_image = raw_response["profileImageUrl"]
 
     async def get_active_allowance_period(self):
         """Returns the current active allowance period."""
         allowance_periods = await self._session.request_handler(
             url=URLS.get("get_child_allowance_periods").format(user_id=self.user_id))
         allowance_periods = allowance_periods["response"]
         active_periods = [p for p in allowance_periods
```

### Comparing `pyroostermoney-0.1.5/pyroostermoney/child/card.py` & `pyroostermoney-0.1.6/pyroostermoney/child/card.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.5/pyroostermoney/child/money_pot.py` & `pyroostermoney-0.1.6/pyroostermoney/child/money_pot.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.5/pyroostermoney/const.py` & `pyroostermoney-0.1.6/pyroostermoney/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.1.5"
+VERSION="0.1.6"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
```

### Comparing `pyroostermoney-0.1.5/pyroostermoney/exceptions.py` & `pyroostermoney-0.1.6/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.5/pyroostermoney/family_account.py` & `pyroostermoney-0.1.6/pyroostermoney/family_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,39 @@
 
 from .api import RoosterSession
 from .const import URLS, DEFAULT_BANK_NAME, DEFAULT_BANK_TYPE, CREATE_PAYMENT_BODY, CURRENCY
 
 class FamilyAccount:
     """A family account."""
 
-    def __init__(self, raw_response: dict, session: RoosterSession) -> None:
+    def __init__(self, raw_response: dict, account_info: dict, session: RoosterSession) -> None:
         self._session = session
-        self._parse_response(raw_response)
+        self._parse_response(raw_response, account_info)
 
-    def _parse_response(self, raw_response: dict):
+    def _parse_response(self, raw_response: dict, account_info: dict):
         """Parses the raw response."""
         if "response" in raw_response:
             raw_response = raw_response["response"]
 
         self.account_number = raw_response["accountNumber"]
         self.sort_code = raw_response["sortCode"]
         self._precision = raw_response["suggestedMonthlyTransfer"]["precision"]
         amount = raw_response["suggestedMonthlyTransfer"]["amount"]
         self.suggested_monthly_transfer = amount / (1 * 10**self._precision)
         self.currency = raw_response["suggestedMonthlyTransfer"]["currency"]
+        self.balance = account_info["familyLedgerBalance"]
 
     async def update(self):
         """Updates the FamilyAccount object data."""
-        response = await self._session.request_handler(
+        family_account = await self._session.request_handler(
             url=URLS.get("get_family_account"))
-        self._parse_response(response)
+        account = await self._session.request_handler(
+            url=URLS.get("get_account_info")
+        )
+        self._parse_response(raw_response=family_account, account_info=account)
 
     @property
     def bank_transfer_details(self):
         """Gets the bank transfer details to top up the family account."""
         return {
             "account_number": self.account_number,
             "sort_code": self.sort_code,
```

### Comparing `pyroostermoney-0.1.5/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.6/pyroostermoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.5
+Version: 0.1.6
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.5/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.6/pyroostermoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

