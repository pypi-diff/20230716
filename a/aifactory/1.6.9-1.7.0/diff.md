# Comparing `tmp/aifactory-1.6.9.tar.gz` & `tmp/aifactory-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.6.9.tar", last modified: Fri Apr  7 08:24:30 2023, max compression
+gzip compressed data, was "aifactory-1.7.0.tar", last modified: Sun Jul 16 02:36:32 2023, max compression
```

## Comparing `aifactory-1.6.9.tar` & `aifactory-1.7.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-04-07 08:24:30.810726 aifactory-1.6.9/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-04-07 08:24:30.810568 aifactory-1.6.9/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-04-07 08:24:30.809061 aifactory-1.6.9/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2022-08-02 00:40:18.000000 aifactory-1.6.9/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2022-11-14 05:11:27.000000 aifactory-1.6.9/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2022-11-14 05:11:05.000000 aifactory-1.6.9/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-03-30 07:01:37.000000 aifactory-1.6.9/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2022-11-05 14:24:05.000000 aifactory-1.6.9/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)     3630 2023-04-07 08:24:18.000000 aifactory-1.6.9/aifactory/score.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-04-07 08:24:30.810348 aifactory-1.6.9/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-04-07 08:24:30.000000 aifactory-1.6.9/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      289 2023-04-07 08:24:30.000000 aifactory-1.6.9/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-04-07 08:24:30.000000 aifactory-1.6.9/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-04-07 08:24:30.000000 aifactory-1.6.9/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-04-07 08:24:30.000000 aifactory-1.6.9/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-04-07 08:24:30.811018 aifactory-1.6.9/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-04-07 08:23:50.000000 aifactory-1.6.9/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 02:36:32.786422 aifactory-1.7.0/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 02:36:32.786210 aifactory-1.7.0/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 02:36:32.784138 aifactory-1.7.0/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)     7471 2023-07-16 02:30:23.000000 aifactory-1.7.0/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 02:36:32.785639 aifactory-1.7.0/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-16 02:36:32.786502 aifactory-1.7.0/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-16 01:38:33.000000 aifactory-1.7.0/setup.py
```

### Comparing `aifactory-1.6.9/aifactory/api.py` & `aifactory-1.7.0/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.6.9/aifactory/demo.py` & `aifactory-1.7.0/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.6.9/aifactory/grade.py` & `aifactory-1.7.0/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.6.9/aifactory/make_zip.py` & `aifactory-1.7.0/aifactory/make_zip.py`

 * *Files identical despite different names*

