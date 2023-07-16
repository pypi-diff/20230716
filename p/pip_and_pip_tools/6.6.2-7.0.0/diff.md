# Comparing `tmp/pip_and_pip_tools-6.6.2.tar.gz` & `tmp/pip_and_pip_tools-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_and_pip_tools-6.6.2.tar", last modified: Fri May 27 18:47:29 2022, max compression
+gzip compressed data, was "pip_and_pip_tools-7.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_and_pip_tools-6.6.2.tar` & `pip_and_pip_tools-7.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      451 2022-05-27 18:47:23.349708 pip_and_pip_tools-6.6.2/.github/workflows/pypi.yml
--rw-r--r--   0        0        0        5 2022-05-27 18:47:23.349708 pip_and_pip_tools-6.6.2/.gitignore
--rw-r--r--   0        0        0      471 2022-05-27 18:47:23.349708 pip_and_pip_tools-6.6.2/LICENSE
--rw-r--r--   0        0        0     1286 2022-05-27 18:47:23.349708 pip_and_pip_tools-6.6.2/README.rst
--rw-r--r--   0        0        0        0 2022-05-27 18:47:23.349708 pip_and_pip_tools-6.6.2/pip_and_pip_tools/__init__.py
--rw-r--r--   0        0        0      467 2022-05-27 18:47:23.349708 pip_and_pip_tools-6.6.2/pyproject.toml
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 pip_and_pip_tools-6.6.2/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-07-16 06:21:41.632027 pip_and_pip_tools-7.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0        5 2023-07-16 06:21:41.632027 pip_and_pip_tools-7.0.0/.gitignore
+-rw-r--r--   0        0        0      471 2023-07-16 06:21:41.632027 pip_and_pip_tools-7.0.0/LICENSE
+-rw-r--r--   0        0        0     1622 2023-07-16 06:21:41.632027 pip_and_pip_tools-7.0.0/README.rst
+-rw-r--r--   0        0        0        0 2023-07-16 06:21:41.632027 pip_and_pip_tools-7.0.0/pip_and_pip_tools/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-16 06:21:41.632027 pip_and_pip_tools-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1985 1970-01-01 00:00:00.000000 pip_and_pip_tools-7.0.0/PKG-INFO
```

### Comparing `pip_and_pip_tools-6.6.2/README.rst` & `pip_and_pip_tools-7.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 =================
 pip and pip-tools
 =================
 
+|pypi-ci|
 
 Purpose
 =======
 
-Occasionally, a new pip__ release is incomatible with the latest existing
+Occasionally, a new pip__ release is incompatible with the latest existing
 `pip-tools`__ release.
 
 The purpose of this package is to make it easy to ensure compatible installations of the two tools.
 
 __ https://github.com/pypa/pip
 __ https://github.com/jazzband/pip-tools
 
@@ -51,7 +52,18 @@
 
 This package is currently maintained by me,
 some guy you don't know.
 
 I am not going to anything malicious with this package,
 but depending on it without verifying its content
 is a risk you should beware.
+
+Usage
+=====
+
+.. code:: console
+
+   $ pip install -U pip pip-tools pip-and-pip-tools
+
+.. |pypi-ci| image:: https://github.com/AndydeCleyre/pip-and-pip-tools/actions/workflows/pypi.yml/badge.svg
+   :alt: Publish to PyPI - GitHub Actions
+   :target: https://github.com/AndydeCleyre/pip-and-pip-tools/actions/workflows/pypi.yml
```

### Comparing `pip_and_pip_tools-6.6.2/PKG-INFO` & `pip_and_pip_tools-7.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: pip_and_pip_tools
-Version: 6.6.2
+Version: 7.0.0
 Summary: Requires compatible installations of pip and pip-tools
 Author: Andy Kluger
 Description-Content-Type: text/x-rst
 Requires-Dist: pip
-Requires-Dist: pip-tools>=6.6.2
+Requires-Dist: pip-tools>=7.0.0
 Requires-Dist: flit<4 ; extra == "dev"
 Project-URL: Home, https://github.com/andydecleyre/pip-and-pip-tools
 Provides-Extra: dev
 
 =================
 pip and pip-tools
 =================
 
+|pypi-ci|
 
 Purpose
 =======
 
-Occasionally, a new pip__ release is incomatible with the latest existing
+Occasionally, a new pip__ release is incompatible with the latest existing
 `pip-tools`__ release.
 
 The purpose of this package is to make it easy to ensure compatible installations of the two tools.
 
 __ https://github.com/pypa/pip
 __ https://github.com/jazzband/pip-tools
 
@@ -64,7 +65,18 @@
 This package is currently maintained by me,
 some guy you don't know.
 
 I am not going to anything malicious with this package,
 but depending on it without verifying its content
 is a risk you should beware.
 
+Usage
+=====
+
+.. code:: console
+
+   $ pip install -U pip pip-tools pip-and-pip-tools
+
+.. |pypi-ci| image:: https://github.com/AndydeCleyre/pip-and-pip-tools/actions/workflows/pypi.yml/badge.svg
+   :alt: Publish to PyPI - GitHub Actions
+   :target: https://github.com/AndydeCleyre/pip-and-pip-tools/actions/workflows/pypi.yml
+
```

