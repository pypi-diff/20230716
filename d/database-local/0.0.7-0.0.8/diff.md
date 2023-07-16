# Comparing `tmp/database-local-0.0.7.tar.gz` & `tmp/database-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-local-0.0.7.tar", last modified: Sun Jul 16 17:16:16 2023, max compression
+gzip compressed data, was "database-local-0.0.8.tar", last modified: Sun Jul 16 19:32:21 2023, max compression
```

## Comparing `database-local-0.0.7.tar` & `database-local-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:16:16.885925 database-local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:15:50.000000 database-local-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 17:16:16.885925 database-local-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:16:16.885925 database-local-0.0.7/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:15:50.000000 database-local-0.0.7/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-16 17:15:50.000000 database-local-0.0.7/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:16:16.885925 database-local-0.0.7/database_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 17:16:16.000000 database-local-0.0.7/database_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 17:15:50.000000 database-local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:16:16.885925 database-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 17:15:50.000000 database-local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:21.736246 database-local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:00.000000 database-local-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 19:32:21.736246 database-local-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:21.736246 database-local-0.0.8/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:00.000000 database-local-0.0.8/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-16 19:32:00.000000 database-local-0.0.8/circles_local_database_python/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:32:21.736246 database-local-0.0.8/database_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 19:32:21.000000 database-local-0.0.8/database_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 19:32:00.000000 database-local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 19:32:21.736246 database-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 19:32:00.000000 database-local-0.0.8/setup.py
```

### Comparing `database-local-0.0.7/circles_local_database_python/database.py` & `database-local-0.0.8/circles_local_database_python/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class database():
     
     def connect_to_database(self):
         try:
             host=os.getenv("RDS_HOSTNAME")
             user=os.getenv("RDS_USERNAME")
-            local_logger.start("database-without-orm-local-python-package database.connect_to_database() "+" host= "+host+" user= "+user)
+            local_logger.start("database-without-orm-local-python-package database.connect_to_database() "+"host= "+host+" user= "+user)
             mydb = mysql.connector.connect(
             host=os.getenv("RDS_HOSTNAME"),
             user=os.getenv("RDS_USERNAME"),
             password=os.getenv("RDS_PASSWORD")
         )
             local_logger.end("database-without-orm-local-python-package database.connect_to_database()")
             return mydb
```

### Comparing `database-local-0.0.7/setup.py` & `database-local-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
      name='database-local',  
-     version='0.0.7',
+     version='0.0.8',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Database Python",
      long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

