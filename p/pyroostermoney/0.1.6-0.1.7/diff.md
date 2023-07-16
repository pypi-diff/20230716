# Comparing `tmp/pyroostermoney-0.1.6.tar.gz` & `tmp/pyroostermoney-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.6.tar", last modified: Sun Jul 16 21:42:07 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.7.tar", last modified: Sun Jul 16 21:53:27 2023, max compression
```

## Comparing `pyroostermoney-0.1.6.tar` & `pyroostermoney-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.316297 pyroostermoney-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/child/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/child/money_pot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 21:42:07.000000 pyroostermoney-0.1.6/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 21:42:07.320297 pyroostermoney-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 21:41:53.000000 pyroostermoney-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.865571 pyroostermoney-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:53:27.869571 pyroostermoney-0.1.7/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 21:53:27.000000 pyroostermoney-0.1.7/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-16 21:53:27.873571 pyroostermoney-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 21:53:13.000000 pyroostermoney-0.1.7/setup.py
```

### Comparing `pyroostermoney-0.1.6/.github/scripts/release.py` & `pyroostermoney-0.1.7/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/.github/workflows/build.yml` & `pyroostermoney-0.1.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/.gitignore` & `pyroostermoney-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/LICENSE` & `pyroostermoney-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/PKG-INFO` & `pyroostermoney-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.6
+Version: 0.1.7
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.6/pyroostermoney/api.py` & `pyroostermoney-0.1.7/pyroostermoney/api.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/pyroostermoney/child/__init__.py` & `pyroostermoney-0.1.7/pyroostermoney/child/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/pyroostermoney/child/card.py` & `pyroostermoney-0.1.7/pyroostermoney/child/card.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/pyroostermoney/child/money_pot.py` & `pyroostermoney-0.1.7/pyroostermoney/child/money_pot.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/pyroostermoney/const.py` & `pyroostermoney-0.1.7/pyroostermoney/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.1.6"
+VERSION="0.1.7"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
```

### Comparing `pyroostermoney-0.1.6/pyroostermoney/exceptions.py` & `pyroostermoney-0.1.7/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/pyroostermoney/family_account.py` & `pyroostermoney-0.1.7/pyroostermoney/family_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         self.account_number = raw_response["accountNumber"]
         self.sort_code = raw_response["sortCode"]
         self._precision = raw_response["suggestedMonthlyTransfer"]["precision"]
         amount = raw_response["suggestedMonthlyTransfer"]["amount"]
         self.suggested_monthly_transfer = amount / (1 * 10**self._precision)
         self.currency = raw_response["suggestedMonthlyTransfer"]["currency"]
-        self.balance = account_info["familyLedgerBalance"]
+        self.balance = account_info.get("familyLedgerBalance", None)
 
     async def update(self):
         """Updates the FamilyAccount object data."""
         family_account = await self._session.request_handler(
             url=URLS.get("get_family_account"))
         account = await self._session.request_handler(
             url=URLS.get("get_account_info")
```

### Comparing `pyroostermoney-0.1.6/pyroostermoney/roostermoney.py` & `pyroostermoney-0.1.7/pyroostermoney/roostermoney.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.6/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.7/pyroostermoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.6
+Version: 0.1.7
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.6/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.7/pyroostermoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

