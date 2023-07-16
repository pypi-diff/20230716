# Comparing `tmp/pylint_sarif_unofficial-0.2.0.tar.gz` & `tmp/pylint_sarif_unofficial-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_sarif_unofficial-0.2.0.tar", max compression
+gzip compressed data, was "pylint_sarif_unofficial-0.2.0a0.tar", max compression
```

## Comparing `pylint_sarif_unofficial-0.2.0.tar` & `pylint_sarif_unofficial-0.2.0a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0/LICENSE
--rw-r--r--   0        0        0     2597 2023-07-16 05:19:07.265949 pylint_sarif_unofficial-0.2.0/README.md
--rw-r--r--   0        0        0     1119 2023-07-16 06:06:49.605518 pylint_sarif_unofficial-0.2.0/pyproject.toml
--rw-r--r--   0        0        0   110930 2023-07-15 23:25:17.669142 pylint_sarif_unofficial-0.2.0/sarif-schema.json
--rwxr-xr-x   0        0        0     4060 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0/src/pylint2cso.py
--rwxr-xr-x   0        0        0    13050 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0/src/pylint2sarif.py
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 pylint_sarif_unofficial-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0a0/LICENSE
+-rw-r--r--   0        0        0     2597 2023-07-16 05:19:07.265949 pylint_sarif_unofficial-0.2.0a0/README.md
+-rw-r--r--   0        0        0     1121 2023-07-16 05:19:07.265949 pylint_sarif_unofficial-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0   110930 2023-07-15 23:25:17.669142 pylint_sarif_unofficial-0.2.0a0/sarif-schema.json
+-rwxr-xr-x   0        0        0     4060 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0a0/src/pylint2cso.py
+-rwxr-xr-x   0        0        0    13050 2023-05-07 05:08:52.000000 pylint_sarif_unofficial-0.2.0a0/src/pylint2sarif.py
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 pylint_sarif_unofficial-0.2.0a0/PKG-INFO
```

### Comparing `pylint_sarif_unofficial-0.2.0/LICENSE` & `pylint_sarif_unofficial-0.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0/README.md` & `pylint_sarif_unofficial-0.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0/pyproject.toml` & `pylint_sarif_unofficial-0.2.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-sarif-unofficial"
-version = "0.2.0"
+version = "0.2.0a0"
 description = "Pylint output as SARIF"
 authors = []
 maintainers = ["Eliah Kagan <degeneracypressure@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/EliahKagan/pylint-sarif"
 repository = "https://github.com/EliahKagan/pylint-sarif"
```

### Comparing `pylint_sarif_unofficial-0.2.0/sarif-schema.json` & `pylint_sarif_unofficial-0.2.0a0/sarif-schema.json`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0/src/pylint2cso.py` & `pylint_sarif_unofficial-0.2.0a0/src/pylint2cso.py`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0/src/pylint2sarif.py` & `pylint_sarif_unofficial-0.2.0a0/src/pylint2sarif.py`

 * *Files identical despite different names*

### Comparing `pylint_sarif_unofficial-0.2.0/PKG-INFO` & `pylint_sarif_unofficial-0.2.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-sarif-unofficial
-Version: 0.2.0
+Version: 0.2.0a0
 Summary: Pylint output as SARIF
 Home-page: https://github.com/EliahKagan/pylint-sarif
 License: MIT
 Keywords: pylint,sarif
 Maintainer: Eliah Kagan
 Maintainer-email: degeneracypressure@gmail.com
 Requires-Python: >=3.7,<4.0
```

