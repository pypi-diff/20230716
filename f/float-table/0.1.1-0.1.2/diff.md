# Comparing `tmp/float_table-0.1.1.tar.gz` & `tmp/float_table-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "float_table-0.1.1.tar", max compression
+gzip compressed data, was "float_table-0.1.2.tar", max compression
```

## Comparing `float_table-0.1.1.tar` & `float_table-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.1/README.md
--rw-r--r--   0        0        0      111 2023-07-16 16:20:05.485577 float_table-0.1.1/float_table/__init__.py
--rw-r--r--   0        0        0     2615 2023-07-16 19:15:13.862085 float_table-0.1.1/float_table/fmt.py
--rw-r--r--   0        0        0      833 2023-07-16 19:42:42.165695 float_table-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2320 2023-07-16 19:42:06.993525 float_table-0.1.1/tests/test.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 float_table-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.2/README.md
+-rw-r--r--   0        0        0      111 2023-07-16 16:20:05.485577 float_table-0.1.2/float_table/__init__.py
+-rw-r--r--   0        0        0     2615 2023-07-16 19:15:13.862085 float_table-0.1.2/float_table/fmt.py
+-rw-r--r--   0        0        0      824 2023-07-16 19:54:21.394980 float_table-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2320 2023-07-16 19:42:06.993525 float_table-0.1.2/tests/test.py
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.2/PKG-INFO
```

### Comparing `float_table-0.1.1/float_table/fmt.py` & `float_table-0.1.2/float_table/fmt.py`

 * *Files identical despite different names*

### Comparing `float_table-0.1.1/pyproject.toml` & `float_table-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool]
 [tool.poetry]
 name = "float-table"
-version = "0.1.1"
+version = "0.1.2"
 homepage = "https://github.com/tadamcz/float-table"
 description = "Top-level package for float-table."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
 ]
 packages = [
     { include = "float_table" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4"
-numpy = "^1.25.1"
-pandas = "^2.0.3"
+python = ">=3.8,<4"
+numpy = "^1"
+pandas = "^2"
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "*"
 coverage = "*"
 pytest = ">=7.2.0"
 pytest-pycharm = "*"
 sigfig = "*"
```

### Comparing `float_table-0.1.1/tests/test.py` & `float_table-0.1.2/tests/test.py`

 * *Files identical despite different names*

