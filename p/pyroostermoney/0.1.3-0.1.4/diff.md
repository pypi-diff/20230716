# Comparing `tmp/pyroostermoney-0.1.3.tar.gz` & `tmp/pyroostermoney-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.3.tar", last modified: Sat Jul 15 22:55:34 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.4.tar", last modified: Sun Jul 16 11:01:52 2023, max compression
```

## Comparing `pyroostermoney-0.1.3.tar` & `pyroostermoney-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.005233 pyroostermoney-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.009233 pyroostermoney-0.1.3/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.009233 pyroostermoney-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.009233 pyroostermoney-0.1.3/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-15 22:55:34.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 22:55:33.000000 pyroostermoney-0.1.3/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 22:55:34.013233 pyroostermoney-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 22:55:21.000000 pyroostermoney-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.201471 pyroostermoney-0.1.4/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 11:01:52.000000 pyroostermoney-0.1.4/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 11:01:52.205472 pyroostermoney-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 11:01:41.000000 pyroostermoney-0.1.4/setup.py
```

### Comparing `pyroostermoney-0.1.3/.github/scripts/release.py` & `pyroostermoney-0.1.4/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.3/.github/workflows/build.yml` & `pyroostermoney-0.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.3/.gitignore` & `pyroostermoney-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.3/LICENSE` & `pyroostermoney-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.3/PKG-INFO` & `pyroostermoney-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.3
+Version: 0.1.4
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.3/pyroostermoney/api.py` & `pyroostermoney-0.1.4/pyroostermoney/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,23 +44,31 @@
         self._password = password
         self._session = None
         self._headers = HEADERS
         self._logged_in = False
 
     async def async_login(self):
         """Logs into RoosterMoney and starts a new active session."""
+        if self._session is not None:
+            if self._session.get("expiry_time") > datetime.now():
+                _LOGGER.debug("Not logging in again, session already active.")
+                return True
+
         req_body = LOGIN_BODY
         req_body["username"] = self._username
         req_body["password"] = self._password
         auth = aiohttp.BasicAuth(self._username, self._password)
 
-        login_response = await self.internal_request_handler(url=URLS.get("login"),
+        if "Authorization" in self._headers:
+            self._headers.pop("Authorization")
+
+        login_response = await self.request_handler(url=URLS.get("login"),
                                                               body=req_body,
                                                               auth=auth,
-                                                              headers=HEADERS)
+                                                              headers=self._headers)
 
         if login_response["status"] == 401:
             raise InvalidAuthError(self._username, login_response["status"])
 
         login_response = login_response["response"]
 
         self._session = {
@@ -75,20 +83,21 @@
 
         self._headers["Authorization"] = f"{token_type} {access_token}"
 
         self._logged_in = True
 
         return True
 
-    async def internal_request_handler(self,
+    async def _internal_request_handler(self,
                                         url,
                                         body=None,
                                         headers=None,
                                         auth=None,
-                                        method="GET"):
+                                        method="GET",
+                                        login_request=False):
         """Handles all incoming requests to make sure that the session is active."""
         if self._session is None and self._logged_in:
             raise RuntimeError("Invalid state. Missing session data yet currently logged in?")
         elif self._session is None and self._logged_in is False and auth is not None:
             _LOGGER.info("Not logged in, trying now.")
             if headers is None:
                 headers = self._headers
@@ -96,19 +105,55 @@
         elif self._session is None and self._logged_in is False and auth is None:
             raise NotLoggedIn()
         elif self._session is not None and self._logged_in is False:
             raise RuntimeError("Invalid state. Session data available yet not logged in?")
 
         # Check if auth has expired
 
+        if login_request:
+            _LOGGER.debug("Login request.")
+            return await _post_request(url, body, auth, headers)
+
         if self._session["expiry_time"] < datetime.now():
             raise AuthenticationExpired()
 
         if headers is None:
             headers = self._headers
 
         if method == "GET":
             return await _fetch_request(url, headers=headers)
         elif method == "POST":
             return await _post_request(url, body=body, headers=headers)
         else:
             raise ValueError("Invalid type argument.")
+
+    async def request_handler(self,
+                                        url,
+                                        body=None,
+                                        headers=None,
+                                        auth=None,
+                                        method="GET",
+                                        login_request=False):
+        """Public calls for the private _internal_request_handler."""
+        try:
+            return await self._internal_request_handler(
+                url=url,
+                body=body,
+                headers=headers,
+                auth=auth,
+                method=method,
+                login_request=login_request
+            )
+        except AuthenticationExpired:
+            await self.async_login()
+            return await self._internal_request_handler(
+                url=url,
+                body=body,
+                headers=headers,
+                auth=auth,
+                method=method,
+                login_request=login_request
+            )
+        except NotLoggedIn:
+            raise NotLoggedIn()
+        except Exception as err:
+            _LOGGER.error(err)
```

### Comparing `pyroostermoney-0.1.3/pyroostermoney/child/__init__.py` & `pyroostermoney-0.1.4/pyroostermoney/child/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     def __init__(self, raw_response: dict, session: RoosterSession) -> None:
         self._parse_response(raw_response)
         self._session = session
 
     async def update(self):
         """Updates the cached data for this child."""
-        response = await self._session.internal_request_handler(
+        response = await self._session.request_handler(
             url=URLS.get("get_child").format(user_id=self.user_id))
         self._parse_response(response)
 
     def _parse_response(self, raw_response:dict):
         """Parses the raw_response into this object"""
         if "response" in raw_response:
             raw_response = raw_response["response"]
@@ -30,15 +30,15 @@
         self.surname = raw_response["surname"]
         self.gender = "male" if raw_response["gender"] == 1 else "female"
         self.uses_real_money = True if raw_response["realMoneyStatus"] == 1 else False
         self.user_id = raw_response["userId"]
 
     async def get_active_allowance_period(self):
         """Returns the current active allowance period."""
-        allowance_periods = await self._session.internal_request_handler(
+        allowance_periods = await self._session.request_handler(
             url=URLS.get("get_child_allowance_periods").format(user_id=self.user_id))
         allowance_periods = allowance_periods["response"]
         active_periods = [p for p in allowance_periods
                           if datetime.datetime.strptime(p["startDate"], "%Y-%m-%d").date() <=
                           datetime.date.today() <=
                           datetime.datetime.strptime(p["endDate"], "%Y-%m-%d").date()]
         if len(active_periods) != 1:
@@ -47,34 +47,34 @@
 
     async def get_spend_history(self, count=10):
         """Gets the spend history"""
         url = URLS.get("get_child_spend_history").format(
             user_id=self.user_id,
             count=count
         )
-        response = await self._session.internal_request_handler(url=url)
+        response = await self._session.request_handler(url=url)
 
         return response["response"]
 
     async def get_allowance_period_jobs(self, allowance_period_id):
         """Gets jobs for a given allowance period"""
         url = URLS.get("get_child_allowance_period_jobs").format(
             user_id=self.user_id,
             allowance_period_id=allowance_period_id
         )
-        response = await self._session.internal_request_handler(url)
+        response = await self._session.request_handler(url)
 
         return response["response"]
 
     async def get_pocket_money(self):
         """Gets pocket money"""
         url = URLS.get("get_child_pocket_money").format(
             user_id=self.user_id
         )
-        response = await self._session.internal_request_handler(url)
+        response = await self._session.request_handler(url)
 
         return response["response"]
 
     async def special_get_pocket_money(self):
         """Same as get_pocket_money yet parses the response and provides a basic dict."""
         pocket_money = await self.get_pocket_money()
```

### Comparing `pyroostermoney-0.1.3/pyroostermoney/const.py` & `pyroostermoney-0.1.4/pyroostermoney/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Static Rooster Money variables"""
 
-VERSION="0.1.3"
+VERSION="0.1.4"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
```

### Comparing `pyroostermoney-0.1.3/pyroostermoney/exceptions.py` & `pyroostermoney-0.1.4/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.3/pyroostermoney/family_account.py` & `pyroostermoney-0.1.4/pyroostermoney/family_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._precision = raw_response["suggestedMonthlyTransfer"]["precision"]
         amount = raw_response["suggestedMonthlyTransfer"]["amount"]
         self.suggested_monthly_transfer = amount / (1 * 10**self._precision)
         self.currency = raw_response["suggestedMonthlyTransfer"]["currency"]
 
     async def update(self):
         """Updates the FamilyAccount object data."""
-        response = await self._session.internal_request_handler(
+        response = await self._session.request_handler(
             url=URLS.get("get_family_account"))
         self._parse_response(response)
 
     @property
     def bank_transfer_details(self):
         """Gets the bank transfer details to top up the family account."""
         return {
@@ -51,35 +51,35 @@
         request_body["paymentMethod"]["encryptedCardNumber"] = card_number
         request_body["paymentMethod"]["encryptedExpiryMonth"] = expiry_month
         request_body["paymentMethod"]["encryptedExpiryYear"] = expiry_year
         request_body["paymentMethod"]["encryptedSecurityCode"] = security_code
         request_body["paymentMethod"]["holderName"] = holder_name
         ## TODO request_body["shopperEmail"] = self.account_info.email
 
-        response = await self._session.internal_request_handler(
+        response = await self._session.request_handler(
             url=URLS.get("create_payment"),
             body=request_body,
             method="POST"
         )
 
         return response["response"]
 
     async def get_available_cards(self):
         """Gets available top up payment cards"""
-        response = await self._session.internal_request_handler(
+        response = await self._session.request_handler(
             url=URLS.get("get_available_cards")
         )
 
         return response["response"]
 
     async def get_top_up_methods(self, currency=None):
         """Gets available top up methods for the family account."""
         if currency is None:
             currency=CURRENCY
 
-        response = await self._session.internal_request_handler(
+        response = await self._session.request_handler(
             url=URLS.get("get_top_up_methods").format(
                 currency=currency
             )
         )
 
         return response["response"]
```

### Comparing `pyroostermoney-0.1.3/pyroostermoney/roostermoney.py` & `pyroostermoney-0.1.4/pyroostermoney/roostermoney.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,31 +25,31 @@
         output = []
         for child in children:
             output.append(ChildAccount(child, self))
         return output
 
     async def get_account_info(self) -> dict:
         """Returns the account info for the current user."""
-        return await self.internal_request_handler(url=URLS.get("get_account_info"))
+        return await self.request_handler(url=URLS.get("get_account_info"))
 
     async def get_child_account(self, user_id) -> ChildAccount:
         """Fetches and returns a given child account details."""
-        response = await self.internal_request_handler(
+        response = await self.request_handler(
             url=URLS.get("get_child").format(user_id=user_id))
 
         return ChildAccount(response, self)
 
     async def get_master_job_list(self):
         """Gets master job list (/parent/master-jobs)"""
-        response = await self.internal_request_handler(
+        response = await self.request_handler(
             url=URLS.get("get_master_job_list")
         )
 
         return response
 
     async def get_family_account(self) -> FamilyAccount:
         """Gets family account details (/parent/family/account)"""
-        response = await self.internal_request_handler(
+        response = await self.request_handler(
             url=URLS.get("get_family_account")
         )
 
         return FamilyAccount(response["response"], self)
```

### Comparing `pyroostermoney-0.1.3/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.4/pyroostermoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.3
+Version: 0.1.4
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.3/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.4/pyroostermoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

