# Comparing `tmp/atro_pylog-0.2.0.tar.gz` & `tmp/atro_pylog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_pylog-0.2.0.tar", max compression
+gzip compressed data, was "atro_pylog-0.2.1.tar", max compression
```

## Comparing `atro_pylog-0.2.0.tar` & `atro_pylog-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1717 2023-07-11 20:05:26.775535 atro_pylog-0.2.0/atro_pylog/__init__.py
--rw-r--r--   0        0        0     1050 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/level.py
--rw-r--r--   0        0        0      363 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/logger_type.py
--rw-r--r--   0        0        0     1096 2023-07-11 19:59:20.704545 atro_pylog-0.2.0/atro_pylog/opentelemetry_setup.py
--rw-r--r--   0        0        0      127 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/rich_setup.py
--rw-r--r--   0        0        0      649 2023-07-11 19:45:01.356569 atro_pylog-0.2.0/atro_pylog/settings.py
--rw-r--r--   0        0        0      636 2023-07-11 20:05:06.008434 atro_pylog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 atro_pylog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1717 2023-07-11 20:05:26.775535 atro_pylog-0.2.1/atro_pylog/__init__.py
+-rw-r--r--   0        0        0     1050 2023-07-11 19:45:01.356569 atro_pylog-0.2.1/atro_pylog/level.py
+-rw-r--r--   0        0        0      363 2023-07-11 19:45:01.356569 atro_pylog-0.2.1/atro_pylog/logger_type.py
+-rw-r--r--   0        0        0     1096 2023-07-11 19:59:20.704545 atro_pylog-0.2.1/atro_pylog/opentelemetry_setup.py
+-rw-r--r--   0        0        0      127 2023-07-11 19:45:01.356569 atro_pylog-0.2.1/atro_pylog/rich_setup.py
+-rw-r--r--   0        0        0      865 2023-07-16 20:46:20.949079 atro_pylog-0.2.1/atro_pylog/settings.py
+-rw-r--r--   0        0        0      636 2023-07-16 20:46:28.832573 atro_pylog-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 atro_pylog-0.2.1/PKG-INFO
```

### Comparing `atro_pylog-0.2.0/atro_pylog/__init__.py` & `atro_pylog-0.2.1/atro_pylog/__init__.py`

 * *Files identical despite different names*

### Comparing `atro_pylog-0.2.0/atro_pylog/level.py` & `atro_pylog-0.2.1/atro_pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro_pylog-0.2.0/atro_pylog/opentelemetry_setup.py` & `atro_pylog-0.2.1/atro_pylog/opentelemetry_setup.py`

 * *Files identical despite different names*

### Comparing `atro_pylog-0.2.0/pyproject.toml` & `atro_pylog-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "atro-pylog"
-version = "0.2.0"
+version = "0.2.1"
 description = "A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging)."
 authors = ["Atropos <pypi.rising@atro.xyz>"]
 packages = [{ include = "atro_pylog" }]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 rich = "*"
```

### Comparing `atro_pylog-0.2.0/PKG-INFO` & `atro_pylog-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

