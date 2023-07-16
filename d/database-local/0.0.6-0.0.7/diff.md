# Comparing `tmp/database-local-0.0.6.tar.gz` & `tmp/database-local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-local-0.0.6.tar", last modified: Wed May 24 02:36:51 2023, max compression
+gzip compressed data, was "database-local-0.0.7.tar", last modified: Sun Jul 16 17:16:16 2023, max compression
```

## Comparing `database-local-0.0.6.tar` & `database-local-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:36:51.441883 database-local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:36:39.000000 database-local-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 02:36:51.441883 database-local-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:36:51.441883 database-local-0.0.6/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:36:39.000000 database-local-0.0.6/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 02:36:39.000000 database-local-0.0.6/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:36:51.441883 database-local-0.0.6/database_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 02:36:51.000000 database-local-0.0.6/database_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 02:36:51.000000 database-local-0.0.6/database_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:36:51.000000 database-local-0.0.6/database_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-24 02:36:51.000000 database-local-0.0.6/database_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 02:36:39.000000 database-local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:36:51.441883 database-local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-24 02:36:39.000000 database-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:16:16.885925 database-local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:15:50.000000 database-local-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 17:16:16.885925 database-local-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:16:16.885925 database-local-0.0.7/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:15:50.000000 database-local-0.0.7/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-16 17:15:50.000000 database-local-0.0.7/circles_local_database_python/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:16:16.885925 database-local-0.0.7/database_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 17:15:50.000000 database-local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:16:16.885925 database-local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 17:15:50.000000 database-local-0.0.7/setup.py
```

### Comparing `database-local-0.0.6/setup.py` & `database-local-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
      name='database-local',  
-     version='0.0.6',
+     version='0.0.7',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Database Python",
      long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

