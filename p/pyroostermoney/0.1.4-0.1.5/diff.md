# Comparing `tmp/pyroostermoney-0.1.4.tar.gz` & `tmp/pyroostermoney-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.4.tar", last modified: Sun Jul 16 11:01:52 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.5.tar", last modified: Sun Jul 16 15:20:23 2023, max compression
```

## Comparing `pyroostermoney-0.1.4.tar` & `pyroostermoney-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.747338 pyroostermoney-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.747338 pyroostermoney-0.1.5/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.751338 pyroostermoney-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.751338 pyroostermoney-0.1.5/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:20:23.751338 pyroostermoney-0.1.5/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 15:20:23.000000 pyroostermoney-0.1.5/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 15:20:23.755338 pyroostermoney-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 15:20:12.000000 pyroostermoney-0.1.5/setup.py
```

### Comparing `pyroostermoney-0.1.4/.github/scripts/release.py` & `pyroostermoney-0.1.5/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.4/.github/workflows/build.yml` & `pyroostermoney-0.1.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.4/.gitignore` & `pyroostermoney-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.4/LICENSE` & `pyroostermoney-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.4/PKG-INFO` & `pyroostermoney-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.4
+Version: 0.1.5
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.4/pyroostermoney/api.py` & `pyroostermoney-0.1.5/pyroostermoney/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Rooster Money requests and session handler."""
 
 import json
 import logging
+import base64
 from datetime import datetime, timedelta
 
 import aiohttp
 
 from .const import HEADERS, BASE_URL, LOGIN_BODY, URLS
 from .exceptions import InvalidAuthError, NotLoggedIn, AuthenticationExpired
 
@@ -66,20 +67,22 @@
                                                               auth=auth,
                                                               headers=self._headers)
 
         if login_response["status"] == 401:
             raise InvalidAuthError(self._username, login_response["status"])
 
         login_response = login_response["response"]
+        token = base64.b64encode(str(self._password[::-1]).encode('utf-8')).decode('utf-8')
 
         self._session = {
             "access_token": login_response["tokens"]["access_token"],
             "refresh_token": login_response["tokens"]["refresh_token"],
             "token_type": login_response["tokens"]["token_type"],
-            "expiry_time": datetime.now() + timedelta(0, login_response["tokens"]["expires_in"])
+            "expiry_time": datetime.now() + timedelta(0, login_response["tokens"]["expires_in"]),
+            "security_code": token
         }
 
         token_type = login_response["tokens"]["token_type"]
         access_token = login_response["tokens"]["access_token"]
 
         self._headers["Authorization"] = f"{token_type} {access_token}"
 
@@ -89,16 +92,18 @@
 
     async def _internal_request_handler(self,
                                         url,
                                         body=None,
                                         headers=None,
                                         auth=None,
                                         method="GET",
-                                        login_request=False):
+                                        login_request=False,
+                                        add_security_token=False):
         """Handles all incoming requests to make sure that the session is active."""
+
         if self._session is None and self._logged_in:
             raise RuntimeError("Invalid state. Missing session data yet currently logged in?")
         elif self._session is None and self._logged_in is False and auth is not None:
             _LOGGER.info("Not logged in, trying now.")
             if headers is None:
                 headers = self._headers
             return await _post_request(url, body, auth, headers)
@@ -115,45 +120,48 @@
 
         if self._session["expiry_time"] < datetime.now():
             raise AuthenticationExpired()
 
         if headers is None:
             headers = self._headers
 
+        if add_security_token:
+            headers["securitytoken"] = self._session["security_code"]
+
         if method == "GET":
             return await _fetch_request(url, headers=headers)
         elif method == "POST":
             return await _post_request(url, body=body, headers=headers)
         else:
             raise ValueError("Invalid type argument.")
 
     async def request_handler(self,
                                         url,
                                         body=None,
                                         headers=None,
                                         auth=None,
                                         method="GET",
-                                        login_request=False):
+                                        login_request=False,
+                                        add_security_token=False):
         """Public calls for the private _internal_request_handler."""
         try:
             return await self._internal_request_handler(
                 url=url,
                 body=body,
                 headers=headers,
                 auth=auth,
                 method=method,
-                login_request=login_request
+                login_request=login_request,
+                add_security_token=add_security_token
             )
         except AuthenticationExpired:
             await self.async_login()
             return await self._internal_request_handler(
                 url=url,
                 body=body,
                 headers=headers,
                 auth=auth,
                 method=method,
                 login_request=login_request
             )
-        except NotLoggedIn:
-            raise NotLoggedIn()
-        except Exception as err:
-            _LOGGER.error(err)
+        except NotLoggedIn as exc:
+            raise NotLoggedIn() from exc
```

### Comparing `pyroostermoney-0.1.4/pyroostermoney/child/__init__.py` & `pyroostermoney-0.1.5/pyroostermoney/child/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """Defines some standard values for a Natwest Rooster Money child."""
 
 import asyncio
 import datetime
 
 from pyroostermoney.const import URLS
 from pyroostermoney.api import RoosterSession
+from .money_pot import Pot, convert_response as MoneyPotConverter
+from .card import Card
 
 class ChildAccount:
     """The child account."""
 
     def __init__(self, raw_response: dict, session: RoosterSession) -> None:
         self._parse_response(raw_response)
         self._session = session
+        self.pots: list[Pot] = []
+        self.card: Card = None
+
+    async def perform_init(self):
+        """Performs init for some internal async props."""
+        await self.get_pocket_money()
+        await self.get_card_details()
 
     async def update(self):
         """Updates the cached data for this child."""
         response = await self._session.request_handler(
             url=URLS.get("get_child").format(user_id=self.user_id))
         self._parse_response(response)
+        await self.get_pocket_money()
 
     def _parse_response(self, raw_response:dict):
         """Parses the raw_response into this object"""
         if "response" in raw_response:
             raw_response = raw_response["response"]
         self.interest_rate = raw_response["interestRate"]
         self.available_pocket_money = raw_response["availablePocketMoney"]
@@ -67,21 +77,34 @@
 
     async def get_pocket_money(self):
         """Gets pocket money"""
         url = URLS.get("get_child_pocket_money").format(
             user_id=self.user_id
         )
         response = await self._session.request_handler(url)
+        self.pots: list[Pot] = MoneyPotConverter(response["response"])
 
         return response["response"]
 
     async def special_get_pocket_money(self):
         """Same as get_pocket_money yet parses the response and provides a basic dict."""
         pocket_money = await self.get_pocket_money()
 
         return {
             "total": pocket_money["walletTotal"],
             "available": pocket_money["availablePocketMoney"],
             "spend": pocket_money["pocketMoneyAmount"],
             "save": pocket_money["safeTotal"],
             "give": pocket_money["giveAmount"]
         }
+
+    async def get_card_details(self):
+        """Returns the card details for the child."""
+        card_details = await self._session.request_handler(
+            URLS.get("get_child_card_details").format(
+                user_id=self.user_id
+            )
+        )
+
+        self.card = Card(card_details["response"], self.user_id, self._session)
+        await self.card.init_card_pin()
+        return self.card
```

### Comparing `pyroostermoney-0.1.4/pyroostermoney/const.py` & `pyroostermoney-0.1.5/pyroostermoney/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,43 @@
+# pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.1.4"
+VERSION="0.1.5"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
 DEFAULT_BANK_NAME="Rooster Money"
 DEFAULT_BANK_TYPE="Business"
 MOBILE_APP_VERSION="10.3.1"
 
+SAVINGS_POT_ID="savings"
+SPEND_POT_ID="spend"
+GIVE_POT_ID="give"
+GOAL_POT_ID="goal"
+
 URLS = {
     "login": "api/v1/parent",
     "get_account_info": "api/parent",
     "get_child": "api/parent/child/{user_id}",
     "get_child_allowance_periods": "api/parent/child/{user_id}/allowance-periods",
     "get_top_up_methods": "api/parent/acquirer/topup/methods?currency={currency}",
     "get_available_cards": "api/parent/acquirer/cards",
     "get_family_account": "api/parent/family/account",
     "get_child_pocket_money": "api/parent/child/{user_id}/pocketmoney",
     "get_child_allowance_period_jobs": "api/parent/child/{user_id}/allowance-periods/{allowance_period_id}",
     "get_master_jobs": "api/parent/master-jobs",
     "get_child_spend_history": "api/parent/child/{user_id}/spendHistory?count={count}",
-    "create_payment": "api/parent/acquirer/create-payment"
+    "create_payment": "api/parent/acquirer/create-payment",
+    "get_child_card_details": "api/parent/child/{user_id}/card/details",
+    "get_child_card_pin": "api/parent/child/{user_id}/cards/{card_id}/pin",
+    "get_family_account_cards": "api/parent/family/cards"
 }
 
 HEADERS = {
     "content-type": "application/json",
     "accept": "application/json"
 }
```

### Comparing `pyroostermoney-0.1.4/pyroostermoney/exceptions.py` & `pyroostermoney-0.1.5/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.4/pyroostermoney/family_account.py` & `pyroostermoney-0.1.5/pyroostermoney/family_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=fixme
 """Defines the class for the family account."""
 
 from .api import RoosterSession
 from .const import URLS, DEFAULT_BANK_NAME, DEFAULT_BANK_TYPE, CREATE_PAYMENT_BODY, CURRENCY
 
 class FamilyAccount:
     """A family account."""
```

### Comparing `pyroostermoney-0.1.4/pyroostermoney/roostermoney.py` & `pyroostermoney-0.1.5/pyroostermoney/roostermoney.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,32 @@
 
     async def get_children(self) -> list[ChildAccount]:
         """Returns a list of available children."""
         account_info = await self.get_account_info()
         children = account_info["response"]["children"]
         output = []
         for child in children:
-            output.append(ChildAccount(child, self))
+            child = ChildAccount(child, self)
+            await child.perform_init() # calling this will init some extra props.
+            output.append(child)
         return output
 
     async def get_account_info(self) -> dict:
         """Returns the account info for the current user."""
         return await self.request_handler(url=URLS.get("get_account_info"))
 
     async def get_child_account(self, user_id) -> ChildAccount:
         """Fetches and returns a given child account details."""
         response = await self.request_handler(
             url=URLS.get("get_child").format(user_id=user_id))
 
-        return ChildAccount(response, self)
+        child = ChildAccount(response, self)
+        await child.perform_init()
+
+        return child
 
     async def get_master_job_list(self):
         """Gets master job list (/parent/master-jobs)"""
         response = await self.request_handler(
             url=URLS.get("get_master_job_list")
         )
```

### Comparing `pyroostermoney-0.1.4/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.5/pyroostermoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.4
+Version: 0.1.5
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.4/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.5/pyroostermoney.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 pyroostermoney/family_account.py
 pyroostermoney/roostermoney.py
 pyroostermoney.egg-info/PKG-INFO
 pyroostermoney.egg-info/SOURCES.txt
 pyroostermoney.egg-info/dependency_links.txt
 pyroostermoney.egg-info/requires.txt
 pyroostermoney.egg-info/top_level.txt
-pyroostermoney/child/__init__.py
+pyroostermoney/child/__init__.py
+pyroostermoney/child/card.py
+pyroostermoney/child/money_pot.py
```

