# Comparing `tmp/string-data-algorithms-0.1.1.tar.gz` & `tmp/string-data-algorithms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string-data-algorithms-0.1.1.tar", last modified: Wed Jul  5 23:53:20 2023, max compression
+gzip compressed data, was "string-data-algorithms-0.1.3.tar", last modified: Sun Jul 16 20:34:05 2023, max compression
```

## Comparing `string-data-algorithms-0.1.1.tar` & `string-data-algorithms-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:53:20.383634 string-data-algorithms-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-05 23:53:20.383634 string-data-algorithms-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:53:20.383634 string-data-algorithms-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-05 23:53:19.000000 string-data-algorithms-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:53:20.383634 string-data-algorithms-0.1.1/string_data_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:53:05.000000 string-data-algorithms-0.1.1/string_data_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-05 23:53:05.000000 string-data-algorithms-0.1.1/string_data_algorithms/string_data_manipulators.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-05 23:53:05.000000 string-data-algorithms-0.1.1/string_data_algorithms/test_string_data_manipulators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:53:20.383634 string-data-algorithms-0.1.1/string_data_algorithms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-05 23:53:20.000000 string-data-algorithms-0.1.1/string_data_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-05 23:53:20.000000 string-data-algorithms-0.1.1/string_data_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:53:20.000000 string-data-algorithms-0.1.1/string_data_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 23:53:20.000000 string-data-algorithms-0.1.1/string_data_algorithms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:34:05.468745 string-data-algorithms-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 20:34:05.468745 string-data-algorithms-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:34:05.468745 string-data-algorithms-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-16 20:34:04.000000 string-data-algorithms-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:34:05.468745 string-data-algorithms-0.1.3/string_data_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:33:50.000000 string-data-algorithms-0.1.3/string_data_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-16 20:33:50.000000 string-data-algorithms-0.1.3/string_data_algorithms/string_data_manipulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-16 20:33:50.000000 string-data-algorithms-0.1.3/string_data_algorithms/test_string_data_manipulators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:34:05.468745 string-data-algorithms-0.1.3/string_data_algorithms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 20:34:05.000000 string-data-algorithms-0.1.3/string_data_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-16 20:34:05.000000 string-data-algorithms-0.1.3/string_data_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:34:05.000000 string-data-algorithms-0.1.3/string_data_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 20:34:05.000000 string-data-algorithms-0.1.3/string_data_algorithms.egg-info/top_level.txt
```

### Comparing `string-data-algorithms-0.1.1/string_data_algorithms/string_data_manipulators.py` & `string-data-algorithms-0.1.3/string_data_algorithms/string_data_manipulators.py`

 * *Files identical despite different names*

### Comparing `string-data-algorithms-0.1.1/string_data_algorithms/test_string_data_manipulators.py` & `string-data-algorithms-0.1.3/string_data_algorithms/test_string_data_manipulators.py`

 * *Files identical despite different names*

