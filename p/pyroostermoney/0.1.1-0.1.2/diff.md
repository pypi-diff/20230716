# Comparing `tmp/pyroostermoney-0.1.1.tar.gz` & `tmp/pyroostermoney-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.1.tar", last modified: Sat Jul 15 21:49:56 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.2.tar", last modified: Sat Jul 15 22:22:38 2023, max compression
```

## Comparing `pyroostermoney-0.1.1.tar` & `pyroostermoney-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:49:56.389661 pyroostermoney-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 21:49:56.389661 pyroostermoney-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.584741 pyroostermoney-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 22:22:38.000000 pyroostermoney-0.1.2/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 22:22:38.588741 pyroostermoney-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 22:22:21.000000 pyroostermoney-0.1.2/setup.py
```

### Comparing `pyroostermoney-0.1.1/.github/scripts/release.py` & `pyroostermoney-0.1.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.1/.github/workflows/build.yml` & `pyroostermoney-0.1.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.1/.gitignore` & `pyroostermoney-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.1/LICENSE` & `pyroostermoney-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.1/PKG-INFO` & `pyroostermoney-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.1
+Version: 0.1.2
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.1/pyroostermoney/api.py` & `pyroostermoney-0.1.2/pyroostermoney/api.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.1/pyroostermoney/child/__init__.py` & `pyroostermoney-0.1.2/pyroostermoney/child/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 """Defines some standard values for a Natwest Rooster Money child."""
 
+import asyncio
 import datetime
 
 from pyroostermoney.const import URLS
 from pyroostermoney.api import RoosterSession
 
 class ChildAccount:
     """The child account."""
 
     def __init__(self, raw_response: dict, session: RoosterSession) -> None:
+        self._parse_response(raw_response)
+        self._session = session
+
+    async def update(self):
+        """Updates the cached data for this child."""
+        response = await self._session.internal_request_handler(
+            url=URLS.get("get_child").format(user_id=self.user_id))
+        self._parse_response(response)
+
+    def _parse_response(self, raw_response:dict):
+        """Parses the raw_response into this object"""
         if "response" in raw_response:
             raw_response = raw_response["response"]
         self.interest_rate = raw_response["interestRate"]
         self.available_pocket_money = raw_response["availablePocketMoney"]
         self.currency = raw_response["currency"]
         self.first_name = raw_response["firstName"]
         self.surname = raw_response["surname"]
         self.gender = "male" if raw_response["gender"] == 1 else "female"
         self.uses_real_money = True if raw_response["realMoneyStatus"] == 1 else False
         self.user_id = raw_response["userId"]
-        self._session = session
 
     async def get_active_allowance_period(self):
         """Returns the current active allowance period."""
         allowance_periods = await self._session.internal_request_handler(
             url=URLS.get("get_child_allowance_periods").format(user_id=self.user_id))
         allowance_periods = allowance_periods["response"]
         active_periods = [p for p in allowance_periods
```

### Comparing `pyroostermoney-0.1.1/pyroostermoney/const.py` & `pyroostermoney-0.1.2/pyroostermoney/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Static Rooster Money variables"""
 
-VERSION="0.1.1"
+VERSION="0.1.2"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
```

### Comparing `pyroostermoney-0.1.1/pyroostermoney/exceptions.py` & `pyroostermoney-0.1.2/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.1/pyroostermoney/roostermoney.py` & `pyroostermoney-0.1.2/pyroostermoney/family_account.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,43 @@
-"""The RoosterMoney integration."""
+"""Defines the class for the family account."""
 
-import logging
-
-from .const import URLS, CREATE_PAYMENT_BODY, CURRENCY, DEFAULT_BANK_NAME, DEFAULT_BANK_TYPE
-from .child import ChildAccount
 from .api import RoosterSession
+from .const import URLS, DEFAULT_BANK_NAME, DEFAULT_BANK_TYPE, CREATE_PAYMENT_BODY, CURRENCY
 
-_LOGGER = logging.getLogger(__name__)
-
-class RoosterMoney(RoosterSession):
-    """The RoosterMoney module."""
-
-    def __init__(self, username: str, password: str) -> None:
-        super().__init__(
-            username=username,
-            password=password
-        )
-
-    async def get_children(self) -> list[ChildAccount]:
-        """Returns a list of available children."""
-        account_info = await self.get_account_info()
-        children = account_info["response"]["children"]
-        output = []
-        for child in children:
-            output.append(ChildAccount(child, self))
-        return output
-
-    async def get_account_info(self) -> dict:
-        """Returns the account info for the current user."""
-        return await self.internal_request_handler(url=URLS.get("get_account_info"))
-
-    async def get_child_account(self, user_id) -> ChildAccount:
-        """Fetches and returns a given child account details."""
-        response = await self.internal_request_handler(
-            url=URLS.get("get_child").format(user_id=user_id))
-
-        return ChildAccount(response, self)
-
-    async def get_master_job_list(self):
-        """Gets master job list (/parent/master-jobs)"""
-        response = await self.internal_request_handler(
-            url=URLS.get("get_master_job_list")
-        )
-
-        return response
+class FamilyAccount:
+    """A family account."""
 
-    async def get_top_up_methods(self, currency=None):
-        """Gets available top up methods for the family account."""
-        if currency is None:
-            currency=CURRENCY
-
-        response = await self.internal_request_handler(
-            url=URLS.get("get_top_up_methods").format(
-                currency=currency
-            )
-        )
-
-        return response["response"]
-
-    async def get_available_cards(self):
-        """Gets available top up payment cards"""
-        response = await self.internal_request_handler(
-            url=URLS.get("get_available_cards")
-        )
-
-        return response["response"]
-
-    async def get_family_account(self):
-        """Gets family account details (/parent/family/account)"""
-        response = await self.internal_request_handler(
-            url=URLS.get("get_family_account")
-        )
-
-        return response["response"]
-
-    async def get_bank_transfer_account_details(self):
-        """Returns bank account details to add money to the family account."""
-        account = await self.get_family_account()
+    def __init__(self, raw_response: dict, session: RoosterSession) -> None:
+        self._session = session
+        self._parse_response(raw_response)
+
+    def _parse_response(self, raw_response: dict):
+        """Parses the raw response."""
+        if "response" in raw_response:
+            raw_response = raw_response["response"]
+
+        self.account_number = raw_response["accountNumber"]
+        self.sort_code = raw_response["sortCode"]
+        self._precision = raw_response["suggestedMonthlyTransfer"]["precision"]
+        amount = raw_response["suggestedMonthlyTransfer"]["amount"]
+        self.suggested_monthly_transfer = amount / (1 * 10**self._precision)
+        self.currency = raw_response["suggestedMonthlyTransfer"]["currency"]
+
+    async def update(self):
+        """Updates the FamilyAccount object data."""
+        response = await self._session.internal_request_handler(
+            url=URLS.get("get_family_account"))
+        self._parse_response(response)
+
+    @property
+    def bank_transfer_details(self):
+        """Gets the bank transfer details to top up the family account."""
         return {
-            "account_number": account["accountNumber"],
-            "sort_code": account["sortCode"],
+            "account_number": self.account_number,
+            "sort_code": self.sort_code,
             "type": DEFAULT_BANK_TYPE,
             "name": DEFAULT_BANK_NAME
         }
 
     async def create_payment(self,
                              value: float,
                              card_number,
@@ -97,14 +51,35 @@
         request_body["paymentMethod"]["encryptedCardNumber"] = card_number
         request_body["paymentMethod"]["encryptedExpiryMonth"] = expiry_month
         request_body["paymentMethod"]["encryptedExpiryYear"] = expiry_year
         request_body["paymentMethod"]["encryptedSecurityCode"] = security_code
         request_body["paymentMethod"]["holderName"] = holder_name
         ## TODO request_body["shopperEmail"] = self.account_info.email
 
-        response = await self.internal_request_handler(
+        response = await self._session.internal_request_handler(
             url=URLS.get("create_payment"),
             body=request_body,
             method="POST"
         )
 
         return response["response"]
+
+    async def get_available_cards(self):
+        """Gets available top up payment cards"""
+        response = await self._session.internal_request_handler(
+            url=URLS.get("get_available_cards")
+        )
+
+        return response["response"]
+
+    async def get_top_up_methods(self, currency=None):
+        """Gets available top up methods for the family account."""
+        if currency is None:
+            currency=CURRENCY
+
+        response = await self._session.internal_request_handler(
+            url=URLS.get("get_top_up_methods").format(
+                currency=currency
+            )
+        )
+
+        return response["response"]
```

### Comparing `pyroostermoney-0.1.1/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.2/pyroostermoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.1
+Version: 0.1.2
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.1/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.2/pyroostermoney.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .github/workflows/build.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 pyroostermoney/__init__.py
 pyroostermoney/api.py
 pyroostermoney/const.py
 pyroostermoney/exceptions.py
+pyroostermoney/family_account.py
 pyroostermoney/roostermoney.py
 pyroostermoney.egg-info/PKG-INFO
 pyroostermoney.egg-info/SOURCES.txt
 pyroostermoney.egg-info/dependency_links.txt
 pyroostermoney.egg-info/requires.txt
 pyroostermoney.egg-info/top_level.txt
 pyroostermoney/child/__init__.py
```

