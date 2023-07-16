# Comparing `tmp/database-local-0.0.8.tar.gz` & `tmp/database-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-local-0.0.8.tar", last modified: Sun Jul 16 19:32:21 2023, max compression
+gzip compressed data, was "database-local-0.0.9.tar", last modified: Sun Jul 16 20:49:47 2023, max compression
```

## Comparing `database-local-0.0.8.tar` & `database-local-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:21.736246 database-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:00.000000 database-local-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 19:32:21.736246 database-local-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:21.736246 database-local-0.0.8/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:00.000000 database-local-0.0.8/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-16 19:32:00.000000 database-local-0.0.8/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:21.736246 database-local-0.0.8/database_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 19:32:00.000000 database-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 19:32:21.736246 database-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 19:32:00.000000 database-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:49:47.184871 database-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:49:26.000000 database-local-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 20:49:47.184871 database-local-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:49:47.184871 database-local-0.0.9/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:49:26.000000 database-local-0.0.9/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-16 20:49:26.000000 database-local-0.0.9/circles_local_database_python/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:49:47.184871 database-local-0.0.9/database_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 20:49:47.000000 database-local-0.0.9/database_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 20:49:47.000000 database-local-0.0.9/database_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:49:47.000000 database-local-0.0.9/database_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 20:49:47.000000 database-local-0.0.9/database_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 20:49:26.000000 database-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:49:47.184871 database-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 20:49:26.000000 database-local-0.0.9/setup.py
```

### Comparing `database-local-0.0.8/circles_local_database_python/database.py` & `database-local-0.0.9/circles_local_database_python/database.py`

 * *Files identical despite different names*

### Comparing `database-local-0.0.8/setup.py` & `database-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
      name='database-local',  
-     version='0.0.8',
+     version='0.0.9',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Database Python",
      long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

