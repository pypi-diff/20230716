# Comparing `tmp/inventree-kom2-1.1a1.tar.gz` & `tmp/inventree-kom2-1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/inventree-kom2/inventree-kom2/dist/.tmp-cai_abeg/inventree-kom2-1.1a1.tar", last modified: Wed May 31 21:26:58 2023, max compression
+gzip compressed data, was "/home/runner/work/inventree-kom2/inventree-kom2/dist/.tmp-pb18k75r/inventree-kom2-1.1a2.tar", last modified: Wed May 31 21:43:12 2023, max compression
```

## Comparing `inventree-kom2-1.1a1.tar` & `inventree-kom2-1.1a2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/src/inventree_kom2/KiCadClasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/src/inventree_kom2/Kom2Plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/src/inventree_kom2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-31 21:42:57.000000 inventree-kom2-1.1a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-31 21:42:57.000000 inventree-kom2-1.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 21:42:57.000000 inventree-kom2-1.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-31 21:42:57.000000 inventree-kom2-1.1a2/src/inventree_kom2/KiCadClasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-31 21:42:57.000000 inventree-kom2-1.1a2/src/inventree_kom2/Kom2Plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-31 21:42:57.000000 inventree-kom2-1.1a2/src/inventree_kom2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2/templates/inventree_kom2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-31 21:42:57.000000 inventree-kom2-1.1a2/src/inventree_kom2/templates/inventree_kom2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 21:43:12.000000 inventree-kom2-1.1a2/src/inventree_kom2.egg-info/top_level.txt
```

### Comparing `inventree-kom2-1.1a1/PKG-INFO` & `inventree-kom2-1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-kom2
-Version: 1.1a1
+Version: 1.1a2
 Summary: Use InvenTree with KiCad
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-kom2
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-kom2/issues
 Keywords: inventree,inventree-plugin,inventree-kom2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inventree-kom2-1.1a1/README.md` & `inventree-kom2-1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `inventree-kom2-1.1a1/pyproject.toml` & `inventree-kom2-1.1a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel", "pyyaml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inventree-kom2"
-version =  "1.1a1"
+version =  "1.1a2"
 description="Use InvenTree with KiCad"
 readme = "README.md"
 license = {text = "MIT license"}
 keywords = ["inventree", "inventree-plugin", "inventree-kom2"]
 authors = [
     {name = "Matthias Mair", email =  "code@mjmair.com"}
 ]
```

### Comparing `inventree-kom2-1.1a1/src/inventree_kom2/KiCadClasses.py` & `inventree-kom2-1.1a2/src/inventree_kom2/KiCadClasses.py`

 * *Files identical despite different names*

### Comparing `inventree-kom2-1.1a1/src/inventree_kom2/Kom2Plugin.py` & `inventree-kom2-1.1a2/src/inventree_kom2/Kom2Plugin.py`

 * *Files identical despite different names*

### Comparing `inventree-kom2-1.1a1/src/inventree_kom2.egg-info/PKG-INFO` & `inventree-kom2-1.1a2/src/inventree_kom2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-kom2
-Version: 1.1a1
+Version: 1.1a2
 Summary: Use InvenTree with KiCad
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-kom2
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-kom2/issues
 Keywords: inventree,inventree-plugin,inventree-kom2
 Classifier: Programming Language :: Python :: 3
```

