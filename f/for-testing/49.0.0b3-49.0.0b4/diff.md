# Comparing `tmp/for-testing-49.0.0b3.tar.gz` & `tmp/for-testing-49.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-jfgkp4ob/for-testing-49.0.0b3.tar", last modified: Sun Jul 16 11:45:04 2023, max compression
+gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-4agmfn_c/for-testing-49.0.0b4.tar", last modified: Sun Jul 16 11:48:24 2023, max compression
```

## Comparing `for-testing-49.0.0b3.tar` & `for-testing-49.0.0b4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 11:44:58.000000 for-testing-49.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/for_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/for_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/for_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/for_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/for_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/for_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-16 11:44:58.000000 for-testing-49.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:45:04.000000 for-testing-49.0.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 11:48:16.000000 for-testing-49.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/for_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/for_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/for_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/for_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/for_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/for_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-16 11:48:16.000000 for-testing-49.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:48:24.000000 for-testing-49.0.0b4/setup.cfg
```

### Comparing `for-testing-49.0.0b3/pyproject.toml` & `for-testing-49.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "for-testing"
-version = "49.0.0b3"
+version = "49.0.0b4"
 description = "foo"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "ascacascascdac@acacascaiuvbasceav.ascaeavav"},
 ]
```

