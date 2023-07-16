# Comparing `tmp/docstring-generator-0.3.1.tar.gz` & `tmp/docstring-generator-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstring-generator-0.3.1.tar", max compression
+gzip compressed data, was "docstring-generator-0.3.2.tar", max compression
```

## Comparing `docstring-generator-0.3.1.tar` & `docstring-generator-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/LICENSE
--rw-r--r--   0        0        0     1818 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/README.md
--rw-r--r--   0        0        0       89 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/docstring_generator/__init__.py
--rw-r--r--   0        0        0      954 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/docstring_generator/new_gen_docs.py
--rw-r--r--   0        0        0     1177 2023-06-02 09:18:13.630272 docstring-generator-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 docstring-generator-0.3.1/setup.py
--rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 docstring-generator-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-07-16 10:37:12.498159 docstring-generator-0.3.2/README.md
+-rw-r--r--   0        0        0       89 2023-07-16 10:37:12.498159 docstring-generator-0.3.2/docstring_generator/__init__.py
+-rw-r--r--   0        0        0      954 2023-07-16 10:37:12.498159 docstring-generator-0.3.2/docstring_generator/new_gen_docs.py
+-rw-r--r--   0        0        0     1175 2023-07-16 10:37:12.498159 docstring-generator-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 docstring-generator-0.3.2/setup.py
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 docstring-generator-0.3.2/PKG-INFO
```

### Comparing `docstring-generator-0.3.1/docstring_generator/new_gen_docs.py` & `docstring-generator-0.3.2/docstring_generator/new_gen_docs.py`

 * *Files identical despite different names*

### Comparing `docstring-generator-0.3.1/pyproject.toml` & `docstring-generator-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.isort]
 combine_as_imports = true
 line_length = 100
 profile = "black"
 
 [tool.poetry]
 name = "docstring-generator"
-version = "0.3.1"
+version = "0.3.2"
 description = "Auto generate docstring from type-hints."
 authors = ["FelixTheC <felixeisenmenger@gmx.net>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/FelixTheC/docstring_generator"
 packages = [{include = "docstring_generator"}]
 classifiers=[
@@ -30,15 +30,15 @@
 
 [tool.poetry.scripts]
 gendocs_new = "docstring_generator.new_gen_docs:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<=3.11"
 click = "^8.1.3"
-docstring-generator-ext = "^0.0.28"
+docstring-generator-ext = "0.0.*"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 isort = "^5.10.1"
 pytest = "^7.1.3"
 
 [build-system]
```

