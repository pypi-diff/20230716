# Comparing `tmp/DataProperty-1.0.0.tar.gz` & `tmp/DataProperty-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataProperty-1.0.0.tar", last modified: Sun Jun 25 01:23:32 2023, max compression
+gzip compressed data, was "DataProperty-1.0.1.tar", last modified: Sun Jul 16 12:48:40 2023, max compression
```

## Comparing `DataProperty-1.0.0.tar` & `DataProperty-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.687040 DataProperty-1.0.0/DataProperty.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    11239 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1262 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 01:23:00.000000 DataProperty-1.0.0/DataProperty.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      138 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-06-25 01:22:45.000000 DataProperty-1.0.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      223 2023-06-25 01:22:45.000000 DataProperty-1.0.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    11239 2023-06-25 01:23:32.697040 DataProperty-1.0.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     9792 2023-06-25 01:22:45.000000 DataProperty-1.0.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/dataproperty/
--rw-r--r--   0 toor      (1000) toor      (1000)     1262 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      535 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_align.py
--rw-r--r--   0 toor      (1000) toor      (1000)      833 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_align_getter.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2478 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_base.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11654 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_column.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1915 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3767 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_container.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3269 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_converter.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11174 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_dataproperty.py
--rw-r--r--   0 toor      (1000) toor      (1000)    25832 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_extractor.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2936 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_formatter.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3115 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_function.py
--rw-r--r--   0 toor      (1000) toor      (1000)      626 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_interface.py
--rw-r--r--   0 toor      (1000) toor      (1000)      114 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_line_break.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5433 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_preprocessor.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/dataproperty/logger/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/logger/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      442 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/logger/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1071 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/logger/_null_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/py.typed
--rw-r--r--   0 toor      (1000) toor      (1000)     1403 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/typing.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/misc/
--rw-r--r--   0 toor      (1000) toor      (1000)       47 2023-06-25 01:22:45.000000 DataProperty-1.0.0/misc/summary.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1186 2023-06-25 01:22:45.000000 DataProperty-1.0.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       24 2023-06-25 01:22:45.000000 DataProperty-1.0.0/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-06-25 01:22:45.000000 DataProperty-1.0.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       52 2023-06-25 01:22:45.000000 DataProperty-1.0.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-25 01:23:32.697040 DataProperty-1.0.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2881 2023-06-25 01:22:45.000000 DataProperty-1.0.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      259 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1748 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_align_getter.py
--rw-r--r--   0 toor      (1000) toor      (1000)    23178 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_column_dataproperty.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4175 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_container.py
--rw-r--r--   0 toor      (1000) toor      (1000)    26293 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_dataproperty.py
--rw-r--r--   0 toor      (1000) toor      (1000)    31362 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_extractor.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2727 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_formatter.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4806 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_function.py
--rw-r--r--   0 toor      (1000) toor      (1000)      559 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2573 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_preprocessor.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1162 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_str_function.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1312 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_typing.py
--rw-r--r--   0 toor      (1000) toor      (1000)      982 2023-06-25 01:22:45.000000 DataProperty-1.0.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 12:48:40.896043 DataProperty-1.0.1/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 12:48:40.886043 DataProperty-1.0.1/DataProperty.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11217 2023-07-16 12:48:40.000000 DataProperty-1.0.1/DataProperty.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1262 2023-07-16 12:48:40.000000 DataProperty-1.0.1/DataProperty.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 12:48:40.000000 DataProperty-1.0.1/DataProperty.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 12:48:06.000000 DataProperty-1.0.1/DataProperty.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      138 2023-07-16 12:48:40.000000 DataProperty-1.0.1/DataProperty.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-07-16 12:48:40.000000 DataProperty-1.0.1/DataProperty.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-07-16 12:47:51.000000 DataProperty-1.0.1/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      223 2023-07-16 12:47:51.000000 DataProperty-1.0.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11217 2023-07-16 12:48:40.896043 DataProperty-1.0.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     9770 2023-07-16 12:47:51.000000 DataProperty-1.0.1/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 12:48:40.886043 DataProperty-1.0.1/dataproperty/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1308 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      535 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_align.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      833 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_align_getter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2514 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11653 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_column.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1915 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5130 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_container.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3269 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_converter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11321 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_dataproperty.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    25899 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_extractor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3000 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_formatter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3115 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      626 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      114 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_line_break.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5467 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/_preprocessor.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 12:48:40.886043 DataProperty-1.0.1/dataproperty/logger/
+-rw-r--r--   0 toor      (1000) toor      (1000)       88 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/logger/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      442 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/logger/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1071 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/logger/_null_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/py.typed
+-rw-r--r--   0 toor      (1000) toor      (1000)     1403 2023-07-16 12:47:51.000000 DataProperty-1.0.1/dataproperty/typing.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 12:48:40.886043 DataProperty-1.0.1/misc/
+-rw-r--r--   0 toor      (1000) toor      (1000)       47 2023-07-16 12:47:51.000000 DataProperty-1.0.1/misc/summary.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1186 2023-07-16 12:47:51.000000 DataProperty-1.0.1/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 12:48:40.886043 DataProperty-1.0.1/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       24 2023-07-16 12:47:51.000000 DataProperty-1.0.1/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-07-16 12:47:51.000000 DataProperty-1.0.1/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       52 2023-07-16 12:47:51.000000 DataProperty-1.0.1/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-16 12:48:40.896043 DataProperty-1.0.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2881 2023-07-16 12:47:51.000000 DataProperty-1.0.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 12:48:40.896043 DataProperty-1.0.1/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      259 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1748 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_align_getter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    23178 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_column_dataproperty.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4175 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_container.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    26293 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_dataproperty.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    31362 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_extractor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2727 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_formatter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4806 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      559 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2573 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_preprocessor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1162 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_str_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1312 2023-07-16 12:47:51.000000 DataProperty-1.0.1/test/test_typing.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      956 2023-07-16 12:47:51.000000 DataProperty-1.0.1/tox.ini
```

### Comparing `DataProperty-1.0.0/DataProperty.egg-info/PKG-INFO` & `DataProperty-1.0.1/DataProperty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataProperty
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for extract property from data.
 Home-page: https://github.com/thombashi/DataProperty
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 Maintainer: Tsuyoshi Hombashi
 Maintainer-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
@@ -54,16 +54,16 @@
    :target: https://pypi.org/project/DataProperty
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/implementation/DataProperty.svg
     :target: https://pypi.org/project/DataProperty
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml
+.. image:: https://github.com/thombashi/DataProperty/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/DataProperty/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/DataProperty/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/DataProperty?branch=master
     :alt: Test coverage
 
 .. image:: https://github.com/thombashi/DataProperty/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `DataProperty-1.0.0/DataProperty.egg-info/SOURCES.txt` & `DataProperty-1.0.1/DataProperty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/LICENSE` & `DataProperty-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/PKG-INFO` & `DataProperty-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataProperty
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for extract property from data.
 Home-page: https://github.com/thombashi/DataProperty
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 Maintainer: Tsuyoshi Hombashi
 Maintainer-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
@@ -54,16 +54,16 @@
    :target: https://pypi.org/project/DataProperty
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/implementation/DataProperty.svg
     :target: https://pypi.org/project/DataProperty
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml
+.. image:: https://github.com/thombashi/DataProperty/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/DataProperty/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/DataProperty/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/DataProperty?branch=master
     :alt: Test coverage
 
 .. image:: https://github.com/thombashi/DataProperty/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `DataProperty-1.0.0/README.rst` & `DataProperty-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
    :target: https://pypi.org/project/DataProperty
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/implementation/DataProperty.svg
     :target: https://pypi.org/project/DataProperty
     :alt: Supported Python implementations
 
-.. image:: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml
+.. image:: https://github.com/thombashi/DataProperty/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/DataProperty/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/DataProperty/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/DataProperty?branch=master
     :alt: Test coverage
 
 .. image:: https://github.com/thombashi/DataProperty/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `DataProperty-1.0.0/dataproperty/__init__.py` & `DataProperty-1.0.1/dataproperty/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from .__version__ import __author__, __copyright__, __email__, __license__, __version__
 from ._align import Align
 from ._align_getter import align_getter
 from ._column import ColumnDataProperty
 from ._common import MAX_STRICT_LEVEL_MAP, MIN_STRICT_LEVEL_MAP, NOT_QUOTING_FLAGS, DefaultValue
 from ._container import MinMaxContainer
 from ._dataproperty import DataProperty
-from ._extractor import DataPropertyExtractor, MatrixFormatting
+from ._extractor import DataPropertyExtractor, DataPropertyMatrix, MatrixFormatting
 from ._formatter import Format
 from ._function import calc_ascii_char_width, get_integer_digit, get_number_of_digit
 from ._line_break import LineBreakHandling
 from ._preprocessor import Preprocessor
 from .logger import set_logger
 
 
 __all__ = (
     "Align",
     "align_getter",
     "ColumnDataProperty",
     "DataProperty",
     "DataPropertyExtractor",
+    "DataPropertyMatrix",
     "Format",
     "LineBreakHandling",
     "MatrixFormatting",
     "MinMaxContainer",
     "Preprocessor",
     "calc_ascii_char_width",
     "get_integer_digit",
```

### Comparing `DataProperty-1.0.0/dataproperty/_align.py` & `DataProperty-1.0.1/dataproperty/_align.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/dataproperty/_align_getter.py` & `DataProperty-1.0.1/dataproperty/_align_getter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/dataproperty/_base.py` & `DataProperty-1.0.1/dataproperty/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Type
+from typing import Dict, Optional, Type
 
 from typepy import (
     Bool,
     DateTime,
     Dictionary,
     Infinity,
     Integer,
@@ -27,15 +27,15 @@
         "_decimal_places",
         "_east_asian_ambiguous_width",
         "_formatter",
         "_typecode",
         "__format_str",
     )
 
-    __TYPE_CLASS_TABLE = {
+    __TYPE_CLASS_TABLE: Dict[Typecode, AbstractType] = {
         Typecode.BOOL: Bool,
         Typecode.DATETIME: DateTime,
         Typecode.DICTIONARY: Dictionary,
         Typecode.INTEGER: Integer,
         Typecode.INFINITY: Infinity,
         Typecode.IP_ADDRESS: IpAddress,
         Typecode.LIST: List,
```

### Comparing `DataProperty-1.0.0/dataproperty/_column.py` & `DataProperty-1.0.1/dataproperty/_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         self.__update_ascii_char_width()
 
     def merge(self, column_dp: "ColumnDataProperty") -> None:
         self.__typecode_bitmap |= column_dp.typecode.value
         self.__calc_typecode_from_bitmap()
 
         self.__minmax_integer_digits.merge(column_dp.minmax_integer_digits)
-        self.__minmax_decimal_places.update(column_dp.minmax_decimal_places)
+        self.__minmax_decimal_places.merge(column_dp.minmax_decimal_places)
         self.__update_decimal_places()
 
         self.__minmax_additional_format_len.merge(column_dp.minmax_additional_format_len)
 
         self.__body_ascii_char_width = max(self.__body_ascii_char_width, column_dp.ascii_char_width)
         self.__update_ascii_char_width()
 
@@ -270,15 +270,15 @@
 
         return max(width_list)
 
     def __calc_decimal_places(self) -> Optional[int]:
         if self.minmax_decimal_places.max_value is None:
             return None
 
-        return int(min(self.__max_precision, self.minmax_decimal_places.max_value))
+        return min(self.__max_precision, int(self.minmax_decimal_places.max_value))
 
     def __get_tostring_format(self, value_dp: DataProperty) -> str:
         if self.typecode == Typecode.STRING:
             return self.__format_map.get(value_dp.typecode, "{:s}")
 
         return self.__format_map.get(self.typecode, "{:s}")
```

### Comparing `DataProperty-1.0.0/dataproperty/_common.py` & `DataProperty-1.0.1/dataproperty/_common.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/dataproperty/_converter.py` & `DataProperty-1.0.1/dataproperty/_converter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/dataproperty/_dataproperty.py` & `DataProperty-1.0.1/dataproperty/_dataproperty.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,23 +94,29 @@
 
         if no_ansi_escape_data is None or len(data) == len(no_ansi_escape_data):
             self.__no_ansi_escape_data: Optional[DataProperty] = None
         else:
             self.__no_ansi_escape_data = DataProperty(no_ansi_escape_data, float_type=float_type)
 
     def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, DataProperty):
+            return False
+
         if self.typecode != other.typecode:
             return False
 
         if self.typecode == Typecode.NAN:
             return True
 
         return self.data == other.data
 
     def __ne__(self, other: Any) -> bool:
+        if not isinstance(other, DataProperty):
+            return True
+
         if self.typecode != other.typecode:
             return True
 
         if self.typecode == Typecode.NAN:
             return False
 
         return self.data != other.data
```

### Comparing `DataProperty-1.0.0/dataproperty/_extractor.py` & `DataProperty-1.0.1/dataproperty/_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     TransFunc,
     TypeHint,
     TypeValueMap,
     normalize_type_hint,
 )
 
 
-DataPropertyMatrix = Sequence[Sequence[DataProperty]]
+DataPropertyMatrix = List[List[DataProperty]]
 
 
 @enum.unique
 class MatrixFormatting(enum.Enum):
     # raise exception if the matrix is not properly formatted
     EXCEPTION = 1 << 1
 
@@ -488,15 +488,15 @@
         self.__update_dp_converter()
         logger.debug(f"max_workers={self.max_workers}, preprocessor={self.__preprocessor}")
 
         value_matrix = self.__strip_data_matrix(value_matrix)
 
         if self.__is_dp_matrix(value_matrix):
             logger.debug("already a dataproperty matrix")
-            return value_matrix
+            return value_matrix  # type: ignore
 
         if self.max_workers <= 1:
             return self.__to_dp_matrix_st(value_matrix)
 
         return self.__to_dp_matrix_mt(value_matrix)
 
     def to_header_dp_list(self) -> List[DataProperty]:
@@ -508,15 +508,15 @@
         return self._to_dp_list(
             self.headers,
             type_hint=String,
             preprocessor=preprocessor,
             strict_level_map=MIN_STRICT_LEVEL_MAP,
         )
 
-    def update_preprocessor(self, **kwargs) -> bool:
+    def update_preprocessor(self, **kwargs: Any) -> bool:
         is_updated = self.__preprocessor.update(**kwargs)
         self.__update_dp_converter()
 
         return is_updated
 
     def update_strict_level_map(self, value: StrictLevelMap) -> bool:
         org = copy.deepcopy(self.__strict_level_map)
@@ -638,15 +638,15 @@
             east_asian_ambiguous_width=self.east_asian_ambiguous_width,
         )
 
         return self.__dp_converter.convert(value_dp)
 
     def __to_dp_matrix_st(self, value_matrix: Sequence[Sequence[Any]]) -> DataPropertyMatrix:
         return list(
-            zip(
+            zip(  # type: ignore
                 *(
                     _to_dp_list_helper(
                         self,
                         col_idx,
                         values,
                         self.__get_col_type_hint(col_idx),
                         self.__preprocessor,
@@ -674,15 +674,17 @@
                 for col_idx, values in enumerate(zip(*value_matrix))
             ]
 
             for future in futures.as_completed(future_list):
                 col_idx, value_dp_list = future.result()
                 col_data_map[col_idx] = value_dp_list
 
-        return list(zip(*(col_data_map[col_idx] for col_idx in sorted(col_data_map))))
+        return list(
+            zip(*(col_data_map[col_idx] for col_idx in sorted(col_data_map)))  # type: ignore
+        )
 
     def _to_dp_list(
         self,
         data_list: Sequence[Any],
         type_hint: TypeHint = None,
         preprocessor: Optional[Preprocessor] = None,
         strict_level_map: Optional[StrictLevelMap] = None,
```

### Comparing `DataProperty-1.0.0/dataproperty/_formatter.py` & `DataProperty-1.0.1/dataproperty/_formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 from decimal import Decimal
-from typing import Optional, Union
+from typing import Dict, Optional, Union
 
 from typepy import Nan, Typecode
 
 
 DecimalPlaces = Union[float, Decimal]
 
 
@@ -12,15 +12,15 @@
     NONE = 0
     THOUSAND_SEPARATOR = 1
 
 
 class Formatter:
     __slots__ = ("__is_formatting_float", "__format_flags", "__datetime_format_str")
 
-    _BLANK_CURLY_BRACES_FORMAT_MAP = {
+    _BLANK_CURLY_BRACES_FORMAT_MAP: Dict[Typecode, str] = {
         Typecode.NONE: "{}",
         Typecode.IP_ADDRESS: "{}",
         Typecode.BOOL: "{}",
         Typecode.DICTIONARY: "{}",
         Typecode.LIST: "{}",
     }
 
@@ -34,15 +34,17 @@
             self.__format_flags = format_flags
         else:
             self.__format_flags = Format.NONE
 
         self.__datetime_format_str = datetime_format_str
         self.__is_formatting_float = is_formatting_float
 
-    def make_format_map(self, decimal_places: Optional[DecimalPlaces] = None):
+    def make_format_map(
+        self, decimal_places: Optional[DecimalPlaces] = None
+    ) -> Dict[Typecode, str]:
         format_map = copy.copy(self._BLANK_CURLY_BRACES_FORMAT_MAP)
         format_map.update(
             {
                 Typecode.INTEGER: self.make_format_str(Typecode.INTEGER),
                 Typecode.REAL_NUMBER: self.make_format_str(Typecode.REAL_NUMBER, decimal_places),
                 Typecode.INFINITY: self.make_format_str(Typecode.INFINITY),
                 Typecode.NAN: self.make_format_str(Typecode.NAN),
```

### Comparing `DataProperty-1.0.0/dataproperty/_function.py` & `DataProperty-1.0.1/dataproperty/_function.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/dataproperty/_interface.py` & `DataProperty-1.0.1/dataproperty/_interface.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/dataproperty/_preprocessor.py` & `DataProperty-1.0.1/dataproperty/_preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,30 +66,30 @@
 
     def preprocess(self, data: Any) -> Tuple:
         data, no_ansi_escape_data = self.__preprocess_string(
             self.__preprocess_data(data, self.strip_str),
         )
         return (data, no_ansi_escape_data)
 
-    def update(self, **kwargs) -> bool:
+    def update(self, **kwargs: Any) -> bool:
         is_updated = False
 
         for key, value in kwargs.items():
             if not hasattr(self, key):
                 continue
 
             if getattr(self, key) == value:
                 continue
 
             setattr(self, key, value)
             is_updated = True
 
         return is_updated
 
-    def __preprocess_string(self, raw_data: Any):
+    def __preprocess_string(self, raw_data: Any) -> Tuple[Any, Optional[str]]:
         data = raw_data
 
         if not isinstance(data, str):
             return (data, None)
 
         if self.replace_tabs_with_spaces:
             try:
```

### Comparing `DataProperty-1.0.0/dataproperty/logger/_null_logger.py` & `DataProperty-1.0.1/dataproperty/logger/_null_logger.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/dataproperty/typing.py` & `DataProperty-1.0.1/dataproperty/typing.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/pyproject.toml` & `DataProperty-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/setup.py` & `DataProperty-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_align_getter.py` & `DataProperty-1.0.1/test/test_align_getter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_column_dataproperty.py` & `DataProperty-1.0.1/test/test_column_dataproperty.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_container.py` & `DataProperty-1.0.1/test/test_container.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_dataproperty.py` & `DataProperty-1.0.1/test/test_dataproperty.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_extractor.py` & `DataProperty-1.0.1/test/test_extractor.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_formatter.py` & `DataProperty-1.0.1/test/test_formatter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_function.py` & `DataProperty-1.0.1/test/test_function.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_logger.py` & `DataProperty-1.0.1/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_preprocessor.py` & `DataProperty-1.0.1/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_str_function.py` & `DataProperty-1.0.1/test/test_str_function.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/test/test_typing.py` & `DataProperty-1.0.1/test/test_typing.py`

 * *Files identical despite different names*

### Comparing `DataProperty-1.0.0/tox.ini` & `DataProperty-1.0.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -53,11 +53,10 @@
 [testenv:lint]
 skip_install = true
 deps =
     codespell>=2
     mypy>=1
     pylama>=8.4.1
 commands =
-    python setup.py check
     -codespell -q2 dataproperty examples test README.rst
     mypy dataproperty
     pylama
```

