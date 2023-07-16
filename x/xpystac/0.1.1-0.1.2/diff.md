# Comparing `tmp/xpystac-0.1.1.tar.gz` & `tmp/xpystac-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpystac-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xpystac-0.1.2.tar", last modified: Sun Jul 16 16:39:16 2023, max compression
```

## Comparing `xpystac-0.1.1.tar` & `xpystac-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,36 @@
--rw-r--r--   0        0        0     2041 2023-06-14 19:41:11.943981 xpystac-0.1.1/README.md
--rw-r--r--   0        0        0      682 2023-06-14 19:41:11.943981 xpystac-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/__init__.py
--rw-r--r--   0        0        0     2513 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/core.py
--rw-r--r--   0        0        0        0 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/py.typed
--rw-r--r--   0        0        0      235 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/utils.py
--rw-r--r--   0        0        0      754 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/xarray_plugin.py
--rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 xpystac-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.533505 xpystac-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.529505 xpystac-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.529505 xpystac-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-16 16:39:05.000000 xpystac-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-16 16:39:05.000000 xpystac-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 16:39:05.000000 xpystac-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-16 16:39:05.000000 xpystac-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-16 16:39:05.000000 xpystac-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-16 16:39:16.533505 xpystac-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-16 16:39:05.000000 xpystac-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-16 16:39:05.000000 xpystac-0.1.2/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-16 16:39:05.000000 xpystac-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-16 16:39:16.533505 xpystac-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.529505 xpystac-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:05.000000 xpystac-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.529505 xpystac-0.1.2/tests/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.533505 xpystac-0.1.2/tests/cassettes/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-07-16 16:39:05.000000 xpystac-0.1.2/tests/cassettes/fixtures/simple_reference_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-16 16:39:05.000000 xpystac-0.1.2/tests/cassettes/fixtures/simple_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-07-16 16:39:05.000000 xpystac-0.1.2/tests/cassettes/fixtures/simple_zarr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-16 16:39:05.000000 xpystac-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-16 16:39:05.000000 xpystac-0.1.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-16 16:39:05.000000 xpystac-0.1.2/tests/test_xarray_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.533505 xpystac-0.1.2/xpystac/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-16 16:39:05.000000 xpystac-0.1.2/xpystac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-16 16:39:05.000000 xpystac-0.1.2/xpystac/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:05.000000 xpystac-0.1.2/xpystac/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-16 16:39:05.000000 xpystac-0.1.2/xpystac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-16 16:39:05.000000 xpystac-0.1.2/xpystac/xarray_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:39:16.533505 xpystac-0.1.2/xpystac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-16 16:39:16.000000 xpystac-0.1.2/xpystac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 16:39:16.000000 xpystac-0.1.2/xpystac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:39:16.000000 xpystac-0.1.2/xpystac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-16 16:39:16.000000 xpystac-0.1.2/xpystac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 16:39:16.000000 xpystac-0.1.2/xpystac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 16:39:16.000000 xpystac-0.1.2/xpystac.egg-info/top_level.txt
```

### Comparing `xpystac-0.1.1/README.md` & `xpystac-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xpystac-0.1.1/xpystac/core.py` & `xpystac-0.1.2/xpystac/core.py`

 * *Files identical despite different names*

### Comparing `xpystac-0.1.1/xpystac/xarray_plugin.py` & `xpystac-0.1.2/xpystac/xarray_plugin.py`

 * *Files identical despite different names*

### Comparing `xpystac-0.1.1/PKG-INFO` & `xpystac-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: xpystac
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extend xarray.open_dataset to accept pystac objects
 Author-email: Julia Signell <jsignell@element84.com>
+License: MIT
+Project-URL: Home, https://github.com/stac-utils/xpystac
+Project-URL: Repository, https://github.com/stac-utils/xpystac
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: xarray
-Requires-Dist: pystac>=1.0.0b3
-Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
 Provides-Extra: dev
+License-File: LICENSE
 
 # xpystac
 xpystac provides the glue that allows `xarray.open_dataset` to accept pystac objects.
 
 The goal is that as long as this library is in your env, you should never need to think about it.
 
 ## Example
@@ -87,8 +87,7 @@
 When you call ``xarray.open_dataset(object, engine="stac")`` this library maps that open call to the correct library.
 Depending on the ``type`` of ``object`` that might be [stackstac](https://github.com/gjoseph92/stackstac)
 or back to ``xarray.open_dataset`` itself but with the engine and other options pulled from the pystac object.
 
 ## Prior Art
 
 This work is inspired by https://github.com/TomAugspurger/staccontainers and the discussion in https://github.com/stac-utils/pystac/issues/846
-
```

