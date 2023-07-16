# Comparing `tmp/fa-models-1.0.78.tar.gz` & `tmp/fa-models-1.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.78.tar", last modified: Sun Jul 16 20:02:23 2023, max compression
+gzip compressed data, was "fa-models-1.0.79.tar", last modified: Sun Jul 16 20:16:16 2023, max compression
```

## Comparing `fa-models-1.0.78.tar` & `fa-models-1.0.79.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:02:23.398748 fa-models-1.0.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-16 20:01:52.000000 fa-models-1.0.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.394748 fa-models-1.0.78/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.394748 fa-models-1.0.78/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/famodels/models/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-16 20:02:15.000000 fa-models-1.0.78/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:02:23.398748 fa-models-1.0.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-16 20:01:52.000000 fa-models-1.0.78/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-16 20:01:52.000000 fa-models-1.0.78/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-16 20:01:52.000000 fa-models-1.0.78/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:16:16.906033 fa-models-1.0.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-16 20:15:38.000000 fa-models-1.0.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.902033 fa-models-1.0.79/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.902033 fa-models-1.0.79/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-16 20:16:06.000000 fa-models-1.0.79/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:16:16.906033 fa-models-1.0.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-16 20:15:38.000000 fa-models-1.0.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-16 20:15:38.000000 fa-models-1.0.79/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-16 20:15:38.000000 fa-models-1.0.79/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.78/PKG-INFO` & `fa-models-1.0.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.78
+Version: 1.0.79
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.78/README.md` & `fa-models-1.0.79/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.79/fa_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.78
+Version: 1.0.79
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.78/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.79/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/algorithm.py` & `fa-models-1.0.79/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/investor.py` & `fa-models-1.0.79/famodels/models/investor.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     """Describing the possible states of an Investor. Keep it simple. Also, we added the str to inherit from, so that the ENUM is serializable.         """
     REGISTERED = "registered"
     """When an investor is merely registered, but NOT authenticated with an official document. Registered allows cold trading."""
     QUALIFIED = "qualified"
     """When an investor is identified and authenticated by an offical document and qualified for hot trades. This is the highest state."""
     BANNED = "banned"
     """The investor was deliberatly banned from the system."""
+    DELETED = "deleted"
+    """ This investor is flagged for deletion."""
+
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 key = os.environ.get("ENCRYPTION_KEY").encode()
 ENCRYPTION_KEY = urlsafe_b64encode(sha256(key).digest())
```

### Comparing `fa-models-1.0.78/famodels/models/investor_statement.py` & `fa-models-1.0.79/famodels/models/investor_statement.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/market/public_trade.py` & `fa-models-1.0.79/famodels/models/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/person.py` & `fa-models-1.0.79/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/processed_signal.py` & `fa-models-1.0.79/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/signal_provider.py` & `fa-models-1.0.79/famodels/models/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/trade.py` & `fa-models-1.0.79/famodels/models/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/trading_signal.py` & `fa-models-1.0.79/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/famodels/models/virtual_order.py` & `fa-models-1.0.79/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/pyproject.toml` & `fa-models-1.0.79/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.78"
+version = "1.0.79"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.78"
+current_version = "1.0.79"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.78/setup.py` & `fa-models-1.0.79/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/tests/test_investor.py` & `fa-models-1.0.79/tests/test_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.78/tests/test_processed_trading_signal.py` & `fa-models-1.0.79/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

