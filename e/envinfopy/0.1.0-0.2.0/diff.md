# Comparing `tmp/envinfopy-0.1.0.tar.gz` & `tmp/envinfopy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envinfopy-0.1.0.tar", last modified: Sat Jun 17 16:19:40 2023, max compression
+gzip compressed data, was "envinfopy-0.2.0.tar", last modified: Sun Jul 16 15:33:14 2023, max compression
```

## Comparing `envinfopy-0.1.0.tar` & `envinfopy-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:13:59.000000 envinfopy-0.1.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      222 2021-03-20 04:13:59.000000 envinfopy-0.1.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5190 2023-06-17 16:19:40.261482 envinfopy-0.1.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     3600 2023-06-17 15:53:45.000000 envinfopy-0.1.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/envinfopy/
--rw-r--r--   0 toor      (1000) toor      (1000)     5568 2023-06-17 11:43:43.000000 envinfopy-0.1.0/envinfopy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-06-17 11:04:59.000000 envinfopy-0.1.0/envinfopy/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-17 11:46:07.000000 envinfopy-0.1.0/envinfopy/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      392 2023-06-17 11:40:05.000000 envinfopy-0.1.0/envinfopy/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:13:59.000000 envinfopy-0.1.0/envinfopy/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/envinfopy.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5190 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      471 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-17 16:19:21.000000 envinfopy-0.1.0/envinfopy.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      314 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       10 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1205 2023-06-17 09:03:58.000000 envinfopy-0.1.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:13:59.000000 envinfopy-0.1.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       79 2023-06-17 05:03:58.000000 envinfopy-0.1.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-17 16:19:40.261482 envinfopy-0.1.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     3121 2023-06-17 15:49:42.000000 envinfopy-0.1.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)      878 2023-06-17 04:56:36.000000 envinfopy-0.1.0/tests/test_cli.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3747 2023-06-17 10:04:15.000000 envinfopy-0.1.0/tests/test_envinfo.py
--rw-r--r--   0 toor      (1000) toor      (1000)      954 2023-06-17 16:19:08.000000 envinfopy-0.1.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:33:14.648679 envinfopy-0.2.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:13:59.000000 envinfopy-0.2.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      222 2021-03-20 04:13:59.000000 envinfopy-0.2.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     5190 2023-07-16 15:33:14.648679 envinfopy-0.2.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     3600 2023-06-17 15:53:45.000000 envinfopy-0.2.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:33:14.638679 envinfopy-0.2.0/envinfopy/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5658 2023-07-16 15:21:28.000000 envinfopy-0.2.0/envinfopy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-06-17 11:04:59.000000 envinfopy-0.2.0/envinfopy/__main__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-16 14:32:56.000000 envinfopy-0.2.0/envinfopy/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      392 2023-06-17 11:40:05.000000 envinfopy-0.2.0/envinfopy/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:13:59.000000 envinfopy-0.2.0/envinfopy/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:33:14.648679 envinfopy-0.2.0/envinfopy.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5190 2023-07-16 15:33:14.000000 envinfopy-0.2.0/envinfopy.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      471 2023-07-16 15:33:14.000000 envinfopy-0.2.0/envinfopy.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 15:33:14.000000 envinfopy-0.2.0/envinfopy.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 15:32:51.000000 envinfopy-0.2.0/envinfopy.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      367 2023-07-16 15:33:14.000000 envinfopy-0.2.0/envinfopy.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       10 2023-07-16 15:33:14.000000 envinfopy-0.2.0/envinfopy.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1205 2023-06-17 09:03:58.000000 envinfopy-0.2.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:33:14.648679 envinfopy-0.2.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-07-16 15:21:40.000000 envinfopy-0.2.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       79 2023-07-16 15:06:56.000000 envinfopy-0.2.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-16 15:33:14.648679 envinfopy-0.2.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     3121 2023-06-17 15:49:42.000000 envinfopy-0.2.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:33:14.648679 envinfopy-0.2.0/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)      878 2023-06-17 04:56:36.000000 envinfopy-0.2.0/tests/test_cli.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3747 2023-06-17 10:04:15.000000 envinfopy-0.2.0/tests/test_envinfo.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      928 2023-06-25 12:47:38.000000 envinfopy-0.2.0/tox.ini
```

### Comparing `envinfopy-0.1.0/LICENSE` & `envinfopy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `envinfopy-0.1.0/PKG-INFO` & `envinfopy-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envinfopy
-Version: 0.1.0
+Version: 0.2.0
 Summary: envinfopy is a Python Library to get execution environment information.
 Home-page: https://github.com/thombashi/envinfopy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/envinfopy
 Project-URL: Tracker, https://github.com/thombashi/envinfopy/issues
```

### Comparing `envinfopy-0.1.0/README.rst` & `envinfopy-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `envinfopy-0.1.0/envinfopy/__init__.py` & `envinfopy-0.2.0/envinfopy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 import os
 import platform
 import re
 import sys
 from collections import OrderedDict, namedtuple
 from typing import Dict, Mapping, Optional, Sequence
 
-import pkg_resources
+
+try:
+    from importlib.metadata import PackageNotFoundError, version
+except ImportError:
+    from importlib_metadata import PackageNotFoundError, version
 
 from .__version__ import __author__, __copyright__, __email__, __license__, __version__
 from ._const import CGROUP_RPOC, Key, OutputFormat
 
 
 __all__ = (
     "__author__",
@@ -102,16 +106,16 @@
         return envinfo
 
     for pkg in packages:
         if not pkg:
             continue
 
         try:
-            envinfo[pkg] = pkg_resources.get_distribution(pkg).version
-        except pkg_resources.DistributionNotFound:
+            envinfo[pkg] = version(pkg)
+        except PackageNotFoundError:
             envinfo[pkg] = "not installed"
 
     return envinfo
 
 
 def _pop_basic_envinfo(envinfo: Dict[str, str]) -> BasicEnvInfo:
     return BasicEnvInfo(
```

### Comparing `envinfopy-0.1.0/envinfopy/__main__.py` & `envinfopy-0.2.0/envinfopy/__main__.py`

 * *Files identical despite different names*

### Comparing `envinfopy-0.1.0/envinfopy.egg-info/PKG-INFO` & `envinfopy-0.2.0/envinfopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envinfopy
-Version: 0.1.0
+Version: 0.2.0
 Summary: envinfopy is a Python Library to get execution environment information.
 Home-page: https://github.com/thombashi/envinfopy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/envinfopy
 Project-URL: Tracker, https://github.com/thombashi/envinfopy/issues
```

### Comparing `envinfopy-0.1.0/pyproject.toml` & `envinfopy-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `envinfopy-0.1.0/setup.py` & `envinfopy-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `envinfopy-0.1.0/tests/test_cli.py` & `envinfopy-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `envinfopy-0.1.0/tests/test_envinfo.py` & `envinfopy-0.2.0/tests/test_envinfo.py`

 * *Files identical despite different names*

### Comparing `envinfopy-0.1.0/tox.ini` & `envinfopy-0.2.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -55,10 +55,9 @@
 skip_install = true
 deps =
     mypy>=1
     pylama>=8.4.1
     types-pkg_resources
     types-setuptools
 commands =
-    python setup.py check
     mypy envinfopy setup.py
     pylama
```

