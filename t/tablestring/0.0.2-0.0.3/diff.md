# Comparing `tmp/tablestring-0.0.2.tar.gz` & `tmp/tablestring-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablestring-0.0.2.tar", last modified: Sun Jul 16 13:00:42 2023, max compression
+gzip compressed data, was "tablestring-0.0.3.tar", last modified: Sun Jul 16 13:03:49 2023, max compression
```

## Comparing `tablestring-0.0.2.tar` & `tablestring-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.971405 tablestring-0.0.2/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablestring-0.0.2/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:00:42.971405 tablestring-0.0.2/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 tablestring-0.0.2/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-16 13:00:37.000000 tablestring-0.0.2/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 13:00:42.971405 tablestring-0.0.2/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.970405 tablestring-0.0.2/tablestring/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9035 2023-07-16 13:00:28.000000 tablestring-0.0.2/tablestring/TableString.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       49 2023-07-16 13:00:28.000000 tablestring-0.0.2/tablestring/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.970405 tablestring-0.0.2/tablestring/chars/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.2/tablestring/chars/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3929 2023-07-16 11:48:00.000000 tablestring-0.0.2/tablestring/chars/border_chars.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.971405 tablestring-0.0.2/tablestring/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.2/tablestring/helpers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1564 2023-07-16 12:10:33.000000 tablestring-0.0.2/tablestring/helpers/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablestring-0.0.2/tablestring/helpers/is_last_element.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2720 2023-07-16 10:57:20.000000 tablestring-0.0.2/tablestring/helpers/row_cross_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      470 2023-07-16 06:06:28.000000 tablestring-0.0.2/tablestring/helpers/row_outer_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1254 2023-07-16 12:11:31.000000 tablestring-0.0.2/tablestring/test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 tablestring-0.0.2/tablestring/type.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:00:42.970405 tablestring-0.0.2/tablestring.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      513 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       12 2023-07-16 13:00:42.000000 tablestring-0.0.2/tablestring.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.522923 tablestring-0.0.3/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablestring-0.0.3/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:03:49.521923 tablestring-0.0.3/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 tablestring-0.0.3/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-16 13:03:30.000000 tablestring-0.0.3/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 13:03:49.522923 tablestring-0.0.3/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.518923 tablestring-0.0.3/tablestring/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9035 2023-07-16 13:00:28.000000 tablestring-0.0.3/tablestring/TableString.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       49 2023-07-16 13:00:28.000000 tablestring-0.0.3/tablestring/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.520923 tablestring-0.0.3/tablestring/chars/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.3/tablestring/chars/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3929 2023-07-16 11:48:00.000000 tablestring-0.0.3/tablestring/chars/border_chars.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.521923 tablestring-0.0.3/tablestring/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.3/tablestring/helpers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1564 2023-07-16 12:10:33.000000 tablestring-0.0.3/tablestring/helpers/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablestring-0.0.3/tablestring/helpers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2744 2023-07-16 13:03:12.000000 tablestring-0.0.3/tablestring/helpers/row_cross_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      494 2023-07-16 13:03:15.000000 tablestring-0.0.3/tablestring/helpers/row_outer_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1254 2023-07-16 12:11:31.000000 tablestring-0.0.3/tablestring/test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 tablestring-0.0.3/tablestring/type.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.519923 tablestring-0.0.3/tablestring.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      513 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       12 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/top_level.txt
```

### Comparing `tablestring-0.0.2/LICENCE` & `tablestring-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.2/PKG-INFO` & `tablestring-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablestring
-Version: 0.0.2
+Version: 0.0.3
 Summary: An ASCII text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablestring-0.0.2/README.md` & `tablestring-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.2/pyproject.toml` & `tablestring-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablestring"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII text table renderer."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `tablestring-0.0.2/tablestring/TableString.py` & `tablestring-0.0.3/tablestring/TableString.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.2/tablestring/chars/border_chars.py` & `tablestring-0.0.3/tablestring/chars/border_chars.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.2/tablestring/helpers/cell_string.py` & `tablestring-0.0.3/tablestring/helpers/cell_string.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.2/tablestring/helpers/row_cross_border.py` & `tablestring-0.0.3/tablestring/helpers/row_cross_border.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from chars.border_chars import cross_matrix, h_line
-from type import BorderType
+from tablestring.chars.border_chars import cross_matrix, h_line
+from tablestring.type import BorderType
 
 
 def row_cross_line(divider: BorderType, v_line_list_top: list, v_line_list_bottom: list) -> str:
 
     """
     :param divider: BorderType
     :param v_line_list_top: [[col_width, BorderType]]
```

### Comparing `tablestring-0.0.2/tablestring/test.py` & `tablestring-0.0.3/tablestring/test.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.2/tablestring/type.py` & `tablestring-0.0.3/tablestring/type.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.2/tablestring.egg-info/PKG-INFO` & `tablestring-0.0.3/tablestring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablestring
-Version: 0.0.2
+Version: 0.0.3
 Summary: An ASCII text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablestring-0.0.2/tablestring.egg-info/SOURCES.txt` & `tablestring-0.0.3/tablestring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

