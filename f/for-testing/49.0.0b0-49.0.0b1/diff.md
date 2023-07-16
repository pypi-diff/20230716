# Comparing `tmp/for-testing-49.0.0b0.tar.gz` & `tmp/for-testing-49.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-yj_mq3hi/for-testing-49.0.0b0.tar", last modified: Sun Jul 16 11:13:49 2023, max compression
+gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-ypgp8rtq/for-testing-49.0.0b1.tar", last modified: Sun Jul 16 11:25:54 2023, max compression
```

## Comparing `for-testing-49.0.0b0.tar` & `for-testing-49.0.0b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 11:13:42.000000 for-testing-49.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/for_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/for_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/for_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/for_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/for_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/for_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-16 11:13:43.000000 for-testing-49.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:13:49.000000 for-testing-49.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 11:25:44.000000 for-testing-49.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/for_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/for_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/for_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/for_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/for_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/for_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-16 11:25:45.000000 for-testing-49.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:25:54.000000 for-testing-49.0.0b1/setup.cfg
```

### Comparing `for-testing-49.0.0b0/pyproject.toml` & `for-testing-49.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "for-testing"
-version = "49.0.0b"
+version = "49.0.0b1"
 description = "foo"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "ascacascascdac@acacascaiuvbasceav.ascaeavav"},
 ]
```

