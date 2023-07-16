# Comparing `tmp/pymetard-0.0.1.tar.gz` & `tmp/pymetard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetard-0.0.1.tar", last modified: Fri Jul 14 07:52:10 2023, max compression
+gzip compressed data, was "pymetard-0.0.2.tar", last modified: Sun Jul 16 14:57:40 2023, max compression
```

## Comparing `pymetard-0.0.1.tar` & `pymetard-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:52:10.050366 pymetard-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-14 07:51:59.000000 pymetard-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-14 07:52:10.050366 pymetard-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 07:51:59.000000 pymetard-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:52:10.050366 pymetard-0.0.1/pymetard/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:52:10.050366 pymetard-0.0.1/pymetard/metar/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/metar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/metar/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/metar/meteo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/metar/station.py
--rw-r--r--   0 runner    (1001) docker     (123)   814165 2023-07-14 07:51:59.000000 pymetard-0.0.1/pymetard/metar/stations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:52:10.050366 pymetard-0.0.1/pymetard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-14 07:52:10.000000 pymetard-0.0.1/pymetard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-14 07:52:10.000000 pymetard-0.0.1/pymetard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:52:10.000000 pymetard-0.0.1/pymetard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 07:52:10.000000 pymetard-0.0.1/pymetard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-14 07:52:10.000000 pymetard-0.0.1/pymetard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 07:52:10.000000 pymetard-0.0.1/pymetard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 07:51:59.000000 pymetard-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:52:10.050366 pymetard-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-14 07:51:59.000000 pymetard-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:52:10.050366 pymetard-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:51:59.000000 pymetard-0.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:52:10.050366 pymetard-0.0.1/tests/pymetard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:51:59.000000 pymetard-0.0.1/tests/pymetard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:52:10.050366 pymetard-0.0.1/tests/pymetard/metar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:51:59.000000 pymetard-0.0.1/tests/pymetard/metar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-14 07:51:59.000000 pymetard-0.0.1/tests/pymetard/metar/test_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 14:57:31.000000 pymetard-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-16 14:57:40.773644 pymetard-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-16 14:57:31.000000 pymetard-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.769643 pymetard-0.0.2/pymetard/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/pymetard/metar/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/meteo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)   814165 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/stations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.769643 pymetard-0.0.2/pymetard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 14:57:31.000000 pymetard-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 14:57:40.773644 pymetard-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-16 14:57:31.000000 pymetard-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/tests/pymetard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/pymetard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/tests/pymetard/metar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/pymetard/metar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/pymetard/metar/test_station.py
```

### Comparing `pymetard-0.0.1/LICENSE` & `pymetard-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.1/pymetard/cli.py` & `pymetard-0.0.2/pymetard/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,15 +112,19 @@
         target_dir=data_workspace,
     )
 
     CHUNK_SIZE = 500
     N = math.ceil(len(stations.keys()) / CHUNK_SIZE)
 
     _start = start
-    if start.day == end.day:
+    if all([
+        _start.year == end.year,
+        _start.month == end.month,
+        _start.day == end.day,
+    ]):
         _end = end
     else:
         _end = datetime(
             year=_start.year,
             month=_start.month,
             day=_start.day,
             hour=23,
@@ -135,15 +139,19 @@
                 end_datetime=_end,
             ):
                 time.sleep(10)
             logger.info(f"Range {_start} to {_end}")
             logger.info(f"Downloaded {int(1+i/CHUNK_SIZE)}/{N}")
             time.sleep(10)
         _start = _end + timedelta(minutes=1)
-        if _start.day == end.day:
+        if all([
+            _start.year == end.year,
+            _start.month == end.month,
+            _start.day == end.day,
+        ]):
             _end = end
         else:
             _end = datetime(
                 year=_start.year,
                 month=_start.month,
                 day=_start.day,
                 hour=23,
```

### Comparing `pymetard-0.0.1/pymetard/metar/downloader.py` & `pymetard-0.0.2/pymetard/metar/downloader.py`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.1/pymetard/metar/station.py` & `pymetard-0.0.2/pymetard/metar/station.py`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.1/pymetard/metar/stations.txt` & `pymetard-0.0.2/pymetard/metar/stations.txt`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.1/pymetard.egg-info/SOURCES.txt` & `pymetard-0.0.2/pymetard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.1/setup.py` & `pymetard-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 
 import setuptools
 
 
-CLIENT_VERSION = "0.0.1"
+CLIENT_VERSION = "0.0.2"
 PACKAGE_NAME = "pymetard"
 
 try:
     with io.open("README.md", encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = ""
```

### Comparing `pymetard-0.0.1/tests/pymetard/metar/test_station.py` & `pymetard-0.0.2/tests/pymetard/metar/test_station.py`

 * *Files identical despite different names*

