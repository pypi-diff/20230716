# Comparing `tmp/climatePy-0.4.31.tar.gz` & `tmp/climatePy-0.4.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.31.tar", last modified: Sat Jul 15 18:33:19 2023, max compression
+gzip compressed data, was "climatePy-0.4.32.tar", last modified: Sun Jul 16 12:54:45 2023, max compression
```

## Comparing `climatePy-0.4.31.tar` & `climatePy-0.4.32.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.469154 climatePy-0.4.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-15 18:33:16.000000 climatePy-0.4.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 18:33:19.469154 climatePy-0.4.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-15 18:33:16.000000 climatePy-0.4.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.425153 climatePy-0.4.31/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    61682 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.425153 climatePy-0.4.31/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.425153 climatePy-0.4.31/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:33:19.469154 climatePy-0.4.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-15 18:33:17.000000 climatePy-0.4.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.469154 climatePy-0.4.31/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:16.000000 climatePy-0.4.31/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-15 18:33:16.000000 climatePy-0.4.31/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-15 18:33:16.000000 climatePy-0.4.31/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.252102 climatePy-0.4.32/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-16 12:54:42.000000 climatePy-0.4.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-16 12:54:45.252102 climatePy-0.4.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-16 12:54:42.000000 climatePy-0.4.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.200102 climatePy-0.4.32/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62112 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.204102 climatePy-0.4.32/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.204102 climatePy-0.4.32/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:54:45.252102 climatePy-0.4.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-16 12:54:44.000000 climatePy-0.4.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.252102 climatePy-0.4.32/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:42.000000 climatePy-0.4.32/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-16 12:54:42.000000 climatePy-0.4.32/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-16 12:54:42.000000 climatePy-0.4.32/tests/test_utils.py
```

### Comparing `climatePy-0.4.31/LICENSE` & `climatePy-0.4.32/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/PKG-INFO` & `climatePy-0.4.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.31
+Version: 0.4.32
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.31/README.md` & `climatePy-0.4.32/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/climatePy/__init__.py` & `climatePy-0.4.32/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/climatePy/_climatepy_filter.py` & `climatePy-0.4.32/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/climatePy/_dap.py` & `climatePy-0.4.32/climatePy/_dap.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,18 +231,24 @@
             
                 ys = [np.argmin(np.abs(Y_coords - out[i].bounds[1])), np.argmin(np.abs(Y_coords - out[i].bounds[3]))]
                 xs = [np.argmin(np.abs(X_coords - out[i].bounds[0])), np.argmin(np.abs(X_coords - out[i].bounds[2]))]
                 
                 catalog.loc[i, 'Y'] = f"[{':1:'.join(map(str, sorted(ys)))}]"
                 catalog.loc[i, 'X'] = f"[{':1:'.join(map(str, sorted(xs)))}]"
 
-                catalog.at[i, 'X1'] = min(X_coords[[i + 1 for i in xs]])
-                catalog.at[i, 'Xn'] = max(X_coords[[i + 1 for i in xs]])
-                catalog.at[i, 'Y1'] = min(Y_coords[[i + 1 for i in ys]])
-                catalog.at[i, 'Yn'] = max(Y_coords[[i + 1 for i in ys]])
+                catalog.at[i, 'X1'] = min(X_coords[[i + 1 if i + 1 < len(X_coords) else i for i in xs]])
+                catalog.at[i, 'Xn'] = max(X_coords[[i + 1 if i + 1 < len(X_coords) else i for i in xs]])
+                catalog.at[i, 'Y1'] = min(Y_coords[[i + 1 if i + 1 < len(Y_coords) else i for i in ys]])
+                catalog.at[i, 'Yn'] = max(Y_coords[[i + 1 if i + 1 < len(Y_coords) else i for i in ys]])
+
+                # catalog.at[i, 'X1'] = min(X_coords[[i + 1 for i in xs]])
+                # catalog.at[i, 'Xn'] = max(X_coords[[i + 1 for i in xs]])
+                # catalog.at[i, 'Y1'] = min(Y_coords[[i + 1 for i in ys]])
+                # catalog.at[i, 'Yn'] = max(Y_coords[[i + 1 for i in ys]])
+
                 catalog.at[i, 'ncols'] = abs(np.diff(xs))[0] + 1
                 catalog.at[i, 'nrows'] = abs(np.diff(ys))[0] + 1
     
     # DIMENSION ORDER STRINGS
     first  = catalog['dim_order'].str[0].fillna('T').values[0]
     second = catalog['dim_order'].str[1].fillna('Y').values[0]
     third  = catalog['dim_order'].str[2].fillna('X').values[0]
```

### Comparing `climatePy-0.4.31/climatePy/_netrc_utils.py` & `climatePy-0.4.32/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/climatePy/_shortcuts.py` & `climatePy-0.4.32/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/climatePy/_utils.py` & `climatePy-0.4.32/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/climatePy/data/catalog.csv` & `climatePy-0.4.32/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.32/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.31
+Version: 0.4.32
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.31/setup.py` & `climatePy-0.4.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.31',
+    version='0.4.32',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.31/tests/test_shortcuts.py` & `climatePy-0.4.32/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.31/tests/test_utils.py` & `climatePy-0.4.32/tests/test_utils.py`

 * *Files identical despite different names*

