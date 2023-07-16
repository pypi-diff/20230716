# Comparing `tmp/labeva-2.1.0a2.dev1.tar.gz` & `tmp/labeva-2.1.0a3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeva-2.1.0a2.dev1.tar", max compression
+gzip compressed data, was "labeva-2.1.0a3.dev1.tar", max compression
```

## Comparing `labeva-2.1.0a2.dev1.tar` & `labeva-2.1.0a3.dev1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0    32473 2023-07-14 05:45:23.392204 labeva-2.1.0a2.dev1/LICENSE
--rwxr-xr-x   0        0        0     1248 2023-07-14 05:45:23.424469 labeva-2.1.0a2.dev1/README.md
--rwxr-xr-x   0        0        0     2757 2023-07-14 06:41:04.643432 labeva-2.1.0a2.dev1/pyproject.toml
--rwxr-xr-x   0        0        0      108 2023-07-14 05:45:23.732933 labeva-2.1.0a2.dev1/src/labeva/__init__.py
--rwxr-xr-x   0        0        0       25 2023-07-14 06:41:04.531522 labeva-2.1.0a2.dev1/src/labeva/__version__.py
--rwxr-xr-x   0        0        0     1295 2023-07-14 05:45:23.823030 labeva-2.1.0a2.dev1/src/labeva/fit.py
--rwxr-xr-x   0        0        0     2130 2023-07-14 06:38:56.962991 labeva-2.1.0a2.dev1/src/labeva/func.py
--rwxr-xr-x   0        0        0     3176 2023-07-14 05:45:23.924147 labeva-2.1.0a2.dev1/src/labeva/math.py
--rwxr-xr-x   0        0        0     5769 2023-07-14 05:45:23.974761 labeva-2.1.0a2.dev1/src/labeva/plot.py
--rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 labeva-2.1.0a2.dev1/PKG-INFO
+-rwxr-xr-x   0        0        0    32473 2023-07-14 05:45:23.392204 labeva-2.1.0a3.dev1/LICENSE
+-rwxr-xr-x   0        0        0     1248 2023-07-14 05:45:23.424469 labeva-2.1.0a3.dev1/README.md
+-rwxr-xr-x   0        0        0     2757 2023-07-16 09:03:42.967102 labeva-2.1.0a3.dev1/pyproject.toml
+-rwxr-xr-x   0        0        0      108 2023-07-14 05:45:23.732933 labeva-2.1.0a3.dev1/src/labeva/__init__.py
+-rwxr-xr-x   0        0        0       25 2023-07-16 09:03:42.926616 labeva-2.1.0a3.dev1/src/labeva/__version__.py
+-rwxr-xr-x   0        0        0     1295 2023-07-14 05:45:23.823030 labeva-2.1.0a3.dev1/src/labeva/fit.py
+-rwxr-xr-x   0        0        0     2130 2023-07-14 06:38:56.962991 labeva-2.1.0a3.dev1/src/labeva/func.py
+-rwxr-xr-x   0        0        0     3176 2023-07-14 05:45:23.924147 labeva-2.1.0a3.dev1/src/labeva/math.py
+-rwxr-xr-x   0        0        0     5895 2023-07-16 08:57:48.658469 labeva-2.1.0a3.dev1/src/labeva/plot.py
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 labeva-2.1.0a3.dev1/PKG-INFO
```

### Comparing `labeva-2.1.0a2.dev1/LICENSE` & `labeva-2.1.0a3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `labeva-2.1.0a2.dev1/README.md` & `labeva-2.1.0a3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `labeva-2.1.0a2.dev1/pyproject.toml` & `labeva-2.1.0a3.dev1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labeva"
-version = "2.1.0a2.dev1"
+version = "2.1.0a3.dev1"
 description = "ETs Laboratory Evaluation Suit"
 authors = ["Erik Thiel <erik.thiel@students.uni-mainz.de>"]
 license = "GPLv3+"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `labeva-2.1.0a2.dev1/src/labeva/fit.py` & `labeva-2.1.0a3.dev1/src/labeva/fit.py`

 * *Files identical despite different names*

### Comparing `labeva-2.1.0a2.dev1/src/labeva/func.py` & `labeva-2.1.0a3.dev1/src/labeva/func.py`

 * *Files identical despite different names*

### Comparing `labeva-2.1.0a2.dev1/src/labeva/math.py` & `labeva-2.1.0a3.dev1/src/labeva/math.py`

 * *Files identical despite different names*

### Comparing `labeva-2.1.0a2.dev1/src/labeva/plot.py` & `labeva-2.1.0a3.dev1/src/labeva/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,17 +194,19 @@
         capthick: error bar cap thickness
         **kwargs: other valid `plt.errorbar` parameters can be provided
 
     Returns:
         Dictionary with parameters
     """
     dct = {}
-    for key, value in locals().values():
+    for key, value in locals().items():
         if value is not None:
             dct[key] = value
+    dct.update(dct["kwargs"])
+    del dct["dct"], dct["kwargs"]
     return dct
 
 
 def args_plt(
     *, ls: str = "dashed", color: str = FIGURE_COLOR, **kwargs: str | int
 ) -> dict[str, str | int]:
     """
@@ -219,11 +221,13 @@
         color: line color
         **kwargs: other valid `plt.plot` parameters can be provided
 
     Returns:
         Dictionary with parameters
     """
     dct = {}
-    for key, value in locals().values():
+    for key, value in locals().items():
         if value is not None:
             dct[key] = value
+    dct.update(dct["kwargs"])
+    del dct["dct"], dct["kwargs"]
     return dct
```

### Comparing `labeva-2.1.0a2.dev1/PKG-INFO` & `labeva-2.1.0a3.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeva
-Version: 2.1.0a2.dev1
+Version: 2.1.0a3.dev1
 Summary: ETs Laboratory Evaluation Suit
 Home-page: https://github.com/et15/labeva
 License: GPLv3+
 Author: Erik Thiel
 Author-email: erik.thiel@students.uni-mainz.de
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
```

