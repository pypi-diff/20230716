# Comparing `tmp/alfen_eve_modbus_tcp-0.0.1.tar.gz` & `tmp/alfen_eve_modbus_tcp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfen_eve_modbus_tcp-0.0.1.tar", last modified: Sun Jul 16 14:15:04 2023, max compression
+gzip compressed data, was "alfen_eve_modbus_tcp-0.0.2.tar", last modified: Sun Jul 16 15:22:37 2023, max compression
```

## Comparing `alfen_eve_modbus_tcp-0.0.1.tar` & `alfen_eve_modbus_tcp-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.1/LICENSE
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-15 21:37:45.000000 alfen_eve_modbus_tcp-0.0.1/README.md
--rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/setup.cfg
--rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.1/setup.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/src/
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp/
--rw-rw-r--   0 luc       (1000) luc       (1000)    22838 2023-07-16 12:34:44.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp/__init__.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/requires.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 15:22:37.799304 alfen_eve_modbus_tcp-0.0.2/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.2/LICENSE
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-16 15:22:37.799304 alfen_eve_modbus_tcp-0.0.2/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-15 21:37:45.000000 alfen_eve_modbus_tcp-0.0.2/README.md
+-rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-07-16 15:22:37.803304 alfen_eve_modbus_tcp-0.0.2/setup.cfg
+-rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.2/setup.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 15:22:37.799304 alfen_eve_modbus_tcp-0.0.2/src/
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 15:22:37.799304 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    22838 2023-07-16 12:34:44.000000 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp/__init__.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 15:22:37.799304 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp.egg-info/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-16 15:22:37.000000 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-07-16 15:22:37.000000 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-16 15:22:37.000000 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-07-16 15:22:37.000000 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp.egg-info/requires.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-07-16 15:22:37.000000 alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/LICENSE` & `alfen_eve_modbus_tcp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.1/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: alfen_eve_modbus_tcp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # alfen_eve_modbus_tcp
 
 alfen_eve_modbus_tcp is a python library that collects data from Alfen Eve Car Chargers over Modbus TCP.
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/README.md` & `alfen_eve_modbus_tcp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.1/setup.cfg` & `alfen_eve_modbus_tcp-0.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alfen_eve_modbus_tcp
-version = 0.0.1
+version = 0.0.2
 author = nessnaj
 description = Alfen Eve Car Charger parser library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/nessnaj/alfen_eve_modbus_tcp
 project_urls = 
@@ -19,15 +19,15 @@
 	License :: OSI Approved :: MIT License
 
 [options]
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
-python_requires = >= 3.8
+python_requires = >= 3.7
 install_requires = 
 	pymodbus >= 3.0.0
 	pyserial-asyncio >= 0.6.0
 
 [options.packages.find]
 where = src
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp/__init__.py` & `alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.2/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: alfen-eve-modbus-tcp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # alfen_eve_modbus_tcp
 
 alfen_eve_modbus_tcp is a python library that collects data from Alfen Eve Car Chargers over Modbus TCP.
```

