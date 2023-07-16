# Comparing `tmp/atro-pyrsync-0.0.7.tar.gz` & `tmp/atro_pyrsync-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pyrsync-0.0.7.tar", last modified: Sun Jun 25 09:33:07 2023, max compression
+gzip compressed data, was "atro_pyrsync-0.0.8.tar", max compression
```

## Comparing `atro-pyrsync-0.0.7.tar` & `atro_pyrsync-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyrsync-0.0.7/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      236 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)       11 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        8 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/pyrsync/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1418 2023-06-25 09:32:47.000000 atro-pyrsync-0.0.7/pyrsync/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       72 2023-06-24 20:11:31.000000 atro-pyrsync-0.0.7/pyrsync/helpers.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)      904 2023-06-25 09:32:28.000000 atro-pyrsync-0.0.7/setup.py
+-rw-r--r--   0        0        0        0 2023-06-17 12:33:58.233092 atro_pyrsync-0.0.8/README.md
+-rw-r--r--   0        0        0     1418 2023-06-25 09:32:47.679795 atro_pyrsync-0.0.8/atro_pyrsync/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-24 20:11:31.873997 atro_pyrsync-0.0.8/atro_pyrsync/helpers.py
+-rw-r--r--   0        0        0      327 2023-07-16 21:25:50.253799 atro_pyrsync-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 atro_pyrsync-0.0.8/PKG-INFO
```

### Comparing `atro-pyrsync-0.0.7/pyrsync/__init__.py` & `atro_pyrsync-0.0.8/atro_pyrsync/__init__.py`

 * *Files identical despite different names*

