# Comparing `tmp/spacetraders_sdk-2.0.2.tar.gz` & `tmp/spacetraders_sdk-2.0.3.tar.gz`

## Comparing `spacetraders_sdk-2.0.2.tar` & `spacetraders_sdk-2.0.3.tar`

### file list

```diff
@@ -1,7 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.2/src/spacetraders_sdk/__init.py__
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.2/src/spacetraders_sdk/example.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.2/.gitignore
--rw-r--r--   0        0        0    18429 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.2/LICENSE
--rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.2/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/__init.py__
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/a_star.py
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/api.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/constants.py
+-rw-r--r--   0        0        0    16678 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/enums.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/helper.py
+-rw-r--r--   0        0        0    21396 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/objects.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/ratelimit.py
+-rw-r--r--   0        0        0    80955 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/sdk.py
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/src/spacetraders_sdk/st_db.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/.gitignore
+-rw-r--r--   0        0        0    18429 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/LICENSE
+-rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/README.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 spacetraders_sdk-2.0.3/PKG-INFO
```

### Comparing `spacetraders_sdk-2.0.2/.gitignore` & `spacetraders_sdk-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spacetraders_sdk-2.0.2/LICENSE` & `spacetraders_sdk-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetraders_sdk-2.0.2/README.md` & `spacetraders_sdk-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders_sdk-2.0.2/PKG-INFO` & `spacetraders_sdk-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders_sdk
-Version: 2.0.2
+Version: 2.0.3
 Summary: A python sdk for the SpaceTradersAPI game
 Project-URL: Homepage, https://github.com/feba66/spacetraders-sdk-v2
 Project-URL: Bug Tracker, https://github.com/feba66/spacetraders-sdk-v2/issues
 Author-email: Felix Baumkötter <feba@feba66.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

