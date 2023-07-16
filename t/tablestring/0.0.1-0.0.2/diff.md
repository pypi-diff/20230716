# Comparing `tmp/tablestring-0.0.1.tar.gz` & `tmp/tablestring-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablestring-0.0.1.tar", last modified: Sun Jul 16 12:53:20 2023, max compression
+gzip compressed data, was "tablestring-0.0.2.tar", last modified: Sun Jul 16 13:00:42 2023, max compression
```

## Comparing `tablestring-0.0.1.tar` & `tablestring-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 12:53:20.004551 tablestring-0.0.1/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablestring-0.0.1/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 12:53:20.004551 tablestring-0.0.1/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 tablestring-0.0.1/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-16 12:52:31.000000 tablestring-0.0.1/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 12:53:20.005551 tablestring-0.0.1/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 12:53:20.002551 tablestring-0.0.1/tablestring/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9052 2023-07-16 12:50:48.000000 tablestring-0.0.1/tablestring/TableString.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:29.000000 tablestring-0.0.1/tablestring/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 12:53:20.003551 tablestring-0.0.1/tablestring/chars/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.1/tablestring/chars/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3929 2023-07-16 11:48:00.000000 tablestring-0.0.1/tablestring/chars/border_chars.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 12:53:20.004551 tablestring-0.0.1/tablestring/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.1/tablestring/helpers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1564 2023-07-16 12:10:33.000000 tablestring-0.0.1/tablestring/helpers/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablestring-0.0.1/tablestring/helpers/is_last_element.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2720 2023-07-16 10:57:20.000000 tablestring-0.0.1/tablestring/helpers/row_cross_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      470 2023-07-16 06:06:28.000000 tablestring-0.0.1/tablestring/helpers/row_outer_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1254 2023-07-16 12:11:31.000000 tablestring-0.0.1/tablestring/test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 tablestring-0.0.1/tablestring/type.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 12:53:20.003551 tablestring-0.0.1/tablestring.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 12:53:19.000000 tablestring-0.0.1/tablestring.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      513 2023-07-16 12:53:20.000000 tablestring-0.0.1/tablestring.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 12:53:19.000000 tablestring-0.0.1/tablestring.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       12 2023-07-16 12:53:19.000000 tablestring-0.0.1/tablestring.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.971405 tablestring-0.0.2/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablestring-0.0.2/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:00:42.971405 tablestring-0.0.2/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 tablestring-0.0.2/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-16 13:00:37.000000 tablestring-0.0.2/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 13:00:42.971405 tablestring-0.0.2/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.970405 tablestring-0.0.2/tablestring/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9035 2023-07-16 13:00:28.000000 tablestring-0.0.2/tablestring/TableString.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       49 2023-07-16 13:00:28.000000 tablestring-0.0.2/tablestring/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.970405 tablestring-0.0.2/tablestring/chars/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.2/tablestring/chars/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3929 2023-07-16 11:48:00.000000 tablestring-0.0.2/tablestring/chars/border_chars.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.971405 tablestring-0.0.2/tablestring/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.2/tablestring/helpers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1564 2023-07-16 12:10:33.000000 tablestring-0.0.2/tablestring/helpers/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablestring-0.0.2/tablestring/helpers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2720 2023-07-16 10:57:20.000000 tablestring-0.0.2/tablestring/helpers/row_cross_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      470 2023-07-16 06:06:28.000000 tablestring-0.0.2/tablestring/helpers/row_outer_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1254 2023-07-16 12:11:31.000000 tablestring-0.0.2/tablestring/test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 tablestring-0.0.2/tablestring/type.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.970405 tablestring-0.0.2/tablestring.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      513 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       12 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/top_level.txt
```

### Comparing `tablestring-0.0.1/LICENCE` & `tablestring-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.1/PKG-INFO` & `tablestring-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablestring
-Version: 0.0.1
+Version: 0.0.2
 Summary: An ASCII text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablestring-0.0.1/README.md` & `tablestring-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.1/pyproject.toml` & `tablestring-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablestring"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII text table renderer."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `tablestring-0.0.1/tablestring/TableString.py` & `tablestring-0.0.2/tablestring/TableString.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import math
 import shutil
 from typing import List, Dict
 
-from chars.border_chars import v_line, top_left, top_right, h_line, left_side_matrix, right_side_matrix, cross_matrix, \
-    bottom_left, bottom_right
-from helpers.is_last_element import is_last_element
-from helpers.row_cross_border import row_cross_line
-from helpers.row_outer_border import row_outer_border
+from tablestring.chars.border_chars import v_line, top_left, top_right, bottom_left, bottom_right
+from tablestring.helpers.is_last_element import is_last_element
+from tablestring.helpers.row_cross_border import row_cross_line
+from tablestring.helpers.row_outer_border import row_outer_border
 from tablestring.helpers.cell_string import cell_string_single_line
 from tablestring.type import BorderType, TableFrameColumnDict, TableFrameOption
 
 
 class TableString:
 
     _border: BorderType
```

### Comparing `tablestring-0.0.1/tablestring/chars/border_chars.py` & `tablestring-0.0.2/tablestring/chars/border_chars.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.1/tablestring/helpers/cell_string.py` & `tablestring-0.0.2/tablestring/helpers/cell_string.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.1/tablestring/helpers/row_cross_border.py` & `tablestring-0.0.2/tablestring/helpers/row_cross_border.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.1/tablestring/test.py` & `tablestring-0.0.2/tablestring/test.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.1/tablestring/type.py` & `tablestring-0.0.2/tablestring/type.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.1/tablestring.egg-info/PKG-INFO` & `tablestring-0.0.2/tablestring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablestring
-Version: 0.0.1
+Version: 0.0.2
 Summary: An ASCII text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablestring-0.0.1/tablestring.egg-info/SOURCES.txt` & `tablestring-0.0.2/tablestring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

