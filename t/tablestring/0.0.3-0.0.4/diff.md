# Comparing `tmp/tablestring-0.0.3.tar.gz` & `tmp/tablestring-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablestring-0.0.3.tar", last modified: Sun Jul 16 13:03:49 2023, max compression
+gzip compressed data, was "tablestring-0.0.4.tar", last modified: Sun Jul 16 13:11:12 2023, max compression
```

## Comparing `tablestring-0.0.3.tar` & `tablestring-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.522923 tablestring-0.0.3/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablestring-0.0.3/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:03:49.521923 tablestring-0.0.3/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 tablestring-0.0.3/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-16 13:03:30.000000 tablestring-0.0.3/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 13:03:49.522923 tablestring-0.0.3/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.518923 tablestring-0.0.3/tablestring/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9035 2023-07-16 13:00:28.000000 tablestring-0.0.3/tablestring/TableString.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       49 2023-07-16 13:00:28.000000 tablestring-0.0.3/tablestring/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.520923 tablestring-0.0.3/tablestring/chars/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.3/tablestring/chars/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3929 2023-07-16 11:48:00.000000 tablestring-0.0.3/tablestring/chars/border_chars.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.521923 tablestring-0.0.3/tablestring/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.3/tablestring/helpers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1564 2023-07-16 12:10:33.000000 tablestring-0.0.3/tablestring/helpers/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablestring-0.0.3/tablestring/helpers/is_last_element.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2744 2023-07-16 13:03:12.000000 tablestring-0.0.3/tablestring/helpers/row_cross_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      494 2023-07-16 13:03:15.000000 tablestring-0.0.3/tablestring/helpers/row_outer_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1254 2023-07-16 12:11:31.000000 tablestring-0.0.3/tablestring/test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 tablestring-0.0.3/tablestring/type.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:03:49.519923 tablestring-0.0.3/tablestring.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      513 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       12 2023-07-16 13:03:49.000000 tablestring-0.0.3/tablestring.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:11:12.691799 tablestring-0.0.4/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablestring-0.0.4/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:11:12.691799 tablestring-0.0.4/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 tablestring-0.0.4/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-16 13:11:01.000000 tablestring-0.0.4/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 13:11:12.691799 tablestring-0.0.4/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:11:12.690799 tablestring-0.0.4/tablestring/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9035 2023-07-16 13:00:28.000000 tablestring-0.0.4/tablestring/TableString.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       49 2023-07-16 13:00:28.000000 tablestring-0.0.4/tablestring/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:11:12.690799 tablestring-0.0.4/tablestring/chars/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.4/tablestring/chars/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3935 2023-07-16 13:10:40.000000 tablestring-0.0.4/tablestring/chars/border_chars.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:11:12.691799 tablestring-0.0.4/tablestring/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablestring-0.0.4/tablestring/helpers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1564 2023-07-16 12:10:33.000000 tablestring-0.0.4/tablestring/helpers/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablestring-0.0.4/tablestring/helpers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2744 2023-07-16 13:03:12.000000 tablestring-0.0.4/tablestring/helpers/row_cross_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      494 2023-07-16 13:03:15.000000 tablestring-0.0.4/tablestring/helpers/row_outer_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1256 2023-07-16 13:06:30.000000 tablestring-0.0.4/tablestring/test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 tablestring-0.0.4/tablestring/type.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 13:11:12.690799 tablestring-0.0.4/tablestring.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 13:11:12.000000 tablestring-0.0.4/tablestring.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      513 2023-07-16 13:11:12.000000 tablestring-0.0.4/tablestring.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 13:11:12.000000 tablestring-0.0.4/tablestring.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       12 2023-07-16 13:11:12.000000 tablestring-0.0.4/tablestring.egg-info/top_level.txt
```

### Comparing `tablestring-0.0.3/LICENCE` & `tablestring-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.3/PKG-INFO` & `tablestring-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablestring
-Version: 0.0.3
+Version: 0.0.4
 Summary: An ASCII text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablestring-0.0.3/README.md` & `tablestring-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.3/pyproject.toml` & `tablestring-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablestring"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII text table renderer."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `tablestring-0.0.3/tablestring/TableString.py` & `tablestring-0.0.4/tablestring/TableString.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.3/tablestring/chars/border_chars.py` & `tablestring-0.0.4/tablestring/chars/border_chars.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,17 +124,17 @@
             "thick": "╦",
             "double": "╦"
         }
     },
     "thin": {
         "blank": {
             "blank": " ",
-            "thin": " ",
-            "thick": " ",
-            "double": " "
+            "thin": "│",
+            "thick": "┃",
+            "double": "║"
         },
         "thin": {
             "blank": "┴",
             "thin": "┼",
             "thick": "╁",
             "double": "╁"
         },
```

### Comparing `tablestring-0.0.3/tablestring/helpers/cell_string.py` & `tablestring-0.0.4/tablestring/helpers/cell_string.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.3/tablestring/helpers/row_cross_border.py` & `tablestring-0.0.4/tablestring/helpers/row_cross_border.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.3/tablestring/test.py` & `tablestring-0.0.4/tablestring/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tablestring.TableString import TableString
 
 
-x = TableString(width=150, border="thick")
+x = TableString(width=150, border="double")
 
 column_list = [
     {
         "key": "Key One",
         "width":  20
     },
     {
@@ -35,15 +35,15 @@
         "Key Three": "Blah s.kflsdjlsdkjflsdkjf;lskdjf;lkdjfls;kdjfl;skdjfsl;kdjflds;kfjsl;kdjfl;sdkjflsd;kjf;slkdjf;sdlkjf"
 
     },
 ]
 
 options = {
     "header_base_divider": "thick",
-    "row_line_divider": "none",
+    "row_line_divider": "blank",
     "column_divider": "thin",
     "header_column_divider": "none",
     "frame_base_divider": "thick",
     # "header_align": "center"
 }
 
 x.add_table_frame(column_list, row_list, options)
```

### Comparing `tablestring-0.0.3/tablestring/type.py` & `tablestring-0.0.4/tablestring/type.py`

 * *Files identical despite different names*

### Comparing `tablestring-0.0.3/tablestring.egg-info/PKG-INFO` & `tablestring-0.0.4/tablestring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablestring
-Version: 0.0.3
+Version: 0.0.4
 Summary: An ASCII text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablestring-0.0.3/tablestring.egg-info/SOURCES.txt` & `tablestring-0.0.4/tablestring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

