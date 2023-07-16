# Comparing `tmp/srai-core-0.4.0.tar.gz` & `tmp/srai-core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-core-0.4.0.tar", last modified: Sun Jul 16 08:32:17 2023, max compression
+gzip compressed data, was "srai-core-0.4.1.tar", last modified: Sun Jul 16 08:56:35 2023, max compression
```

## Comparing `srai-core-0.4.0.tar` & `srai-core-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:32:17.526181 srai-core-0.4.0/
--rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0       24 2023-07-15 08:05:50.000000 srai-core-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      767 2023-07-16 08:32:17.526181 srai-core-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 07:25:20.000000 srai-core-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-07-16 08:32:17.528174 srai-core-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-16 08:28:50.000000 srai-core-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:32:17.498175 srai-core-0.4.0/srai_core/
--rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.4.0/srai_core/__init__.py
--rw-rw-rw-   0        0        0      538 2023-07-16 08:31:22.000000 srai-core-0.4.0/srai_core/file_store.py
--rw-rw-rw-   0        0        0      466 2023-07-16 08:28:25.000000 srai-core-0.4.0/srai_core/file_store_disk.py
--rw-rw-rw-   0        0        0     1296 2023-07-16 08:31:12.000000 srai-core-0.4.0/srai_core/jsondict_store.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:32:17.525192 srai-core-0.4.0/srai_core.egg-info/
--rw-rw-rw-   0        0        0      767 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:56:35.505848 srai-core-0.4.1/
+-rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       24 2023-07-15 08:05:50.000000 srai-core-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      767 2023-07-16 08:56:35.505848 srai-core-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 07:25:20.000000 srai-core-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-16 08:56:35.507848 srai-core-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-16 08:55:28.000000 srai-core-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:56:35.487835 srai-core-0.4.1/srai_core/
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.4.1/srai_core/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-07-16 08:31:22.000000 srai-core-0.4.1/srai_core/file_store.py
+-rw-rw-rw-   0        0        0      500 2023-07-16 08:56:01.000000 srai-core-0.4.1/srai_core/file_store_disk.py
+-rw-rw-rw-   0        0        0     1296 2023-07-16 08:31:12.000000 srai-core-0.4.1/srai_core/jsondict_store.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:56:35.503833 srai-core-0.4.1/srai_core.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-07-16 08:56:35.000000 srai-core-0.4.1/srai_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-16 08:56:35.000000 srai-core-0.4.1/srai_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:56:35.000000 srai-core-0.4.1/srai_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-16 08:56:35.000000 srai-core-0.4.1/srai_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 08:56:35.000000 srai-core-0.4.1/srai_core.egg-info/top_level.txt
```

### Comparing `srai-core-0.4.0/LICENSE.txt` & `srai-core-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srai-core-0.4.0/PKG-INFO` & `srai-core-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library core functions used in other SRAI libraries.
 Home-page: https://github.com/southriverai/srai-core
 Download-URL: https://github.com/southriverai/srai-core/archive/v_01.tar.gz
 Author: Jaap Oosterbroek
 Author-email: jaap.oosterbroek@southriverai.com
 License: MIT
 Keywords: SRAI,TOOLS
```

### Comparing `srai-core-0.4.0/setup.py` & `srai-core-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="srai-core",
     packages=find_packages(),
-    version="0.4.0",
+    version="0.4.1",
     license="MIT",
     package_data={},
     python_requires=">=3.5",
     install_requires=requirements,
     author="Jaap Oosterbroek",
     author_email="jaap.oosterbroek@southriverai.com",
     description="A library core functions used in other SRAI libraries.",
```

### Comparing `srai-core-0.4.0/srai_core/file_store.py` & `srai-core-0.4.1/srai_core/file_store.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.4.0/srai_core/jsondict_store.py` & `srai-core-0.4.1/srai_core/jsondict_store.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.4.0/srai_core.egg-info/PKG-INFO` & `srai-core-0.4.1/srai_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library core functions used in other SRAI libraries.
 Home-page: https://github.com/southriverai/srai-core
 Download-URL: https://github.com/southriverai/srai-core/archive/v_01.tar.gz
 Author: Jaap Oosterbroek
 Author-email: jaap.oosterbroek@southriverai.com
 License: MIT
 Keywords: SRAI,TOOLS
```

