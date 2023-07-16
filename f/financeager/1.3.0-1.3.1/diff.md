# Comparing `tmp/financeager-1.3.0.tar.gz` & `tmp/financeager-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financeager-1.3.0.tar", last modified: Thu May  4 22:06:12 2023, max compression
+gzip compressed data, was "financeager-1.3.1.tar", last modified: Sun Jul 16 11:56:38 2023, max compression
```

## Comparing `financeager-1.3.0.tar` & `financeager-1.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:06:12.071500 financeager-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:06:12.063499 financeager-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-04 22:05:45.000000 financeager-1.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:06:12.067500 financeager-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-04 22:05:45.000000 financeager-1.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-04 22:05:45.000000 financeager-1.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-04 22:05:45.000000 financeager-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-04 22:05:45.000000 financeager-1.3.0/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-04 22:05:45.000000 financeager-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-04 22:05:45.000000 financeager-1.3.0/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-04 22:05:45.000000 financeager-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 22:05:45.000000 financeager-1.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-05-04 22:06:12.071500 financeager-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13432 2023-05-04 22:05:45.000000 financeager-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:06:12.067500 financeager-1.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   214498 2023-05-04 22:05:45.000000 financeager-1.3.0/examples/quickstart.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:06:12.067500 financeager-1.3.0/financeager/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/entries.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-04 22:05:45.000000 financeager-1.3.0/financeager/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:06:12.067500 financeager-1.3.0/financeager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-05-04 22:06:12.000000 financeager-1.3.0/financeager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-04 22:06:12.000000 financeager-1.3.0/financeager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:06:12.000000 financeager-1.3.0/financeager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 22:06:12.000000 financeager-1.3.0/financeager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-04 22:06:12.000000 financeager-1.3.0/financeager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 22:06:12.000000 financeager-1.3.0/financeager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-04 22:05:45.000000 financeager-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 22:06:12.071500 financeager-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:06:12.071500 financeager-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:05:45.000000 financeager-1.3.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-05-04 22:05:45.000000 financeager-1.3.0/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-04 22:05:45.000000 financeager-1.3.0/test/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-04 22:05:45.000000 financeager-1.3.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-04 22:05:45.000000 financeager-1.3.0/test/test_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-04 22:05:45.000000 financeager-1.3.0/test/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23123 2023-05-04 22:05:45.000000 financeager-1.3.0/test/test_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-05-04 22:05:45.000000 financeager-1.3.0/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:38.605405 financeager-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:38.597405 financeager-1.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-16 11:56:10.000000 financeager-1.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:38.601405 financeager-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-16 11:56:10.000000 financeager-1.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-16 11:56:10.000000 financeager-1.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-16 11:56:10.000000 financeager-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-16 11:56:10.000000 financeager-1.3.1/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-16 11:56:10.000000 financeager-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-16 11:56:10.000000 financeager-1.3.1/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-16 11:56:10.000000 financeager-1.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-16 11:56:10.000000 financeager-1.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-07-16 11:56:38.605405 financeager-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13432 2023-07-16 11:56:10.000000 financeager-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:38.601405 financeager-1.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   214498 2023-07-16 11:56:10.000000 financeager-1.3.1/examples/quickstart.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:38.601405 financeager-1.3.1/financeager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-16 11:56:10.000000 financeager-1.3.1/financeager/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:38.605405 financeager-1.3.1/financeager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-07-16 11:56:38.000000 financeager-1.3.1/financeager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-16 11:56:38.000000 financeager-1.3.1/financeager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:56:38.000000 financeager-1.3.1/financeager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 11:56:38.000000 financeager-1.3.1/financeager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 11:56:38.000000 financeager-1.3.1/financeager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 11:56:38.000000 financeager-1.3.1/financeager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-16 11:56:10.000000 financeager-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:56:38.605405 financeager-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:38.605405 financeager-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 11:56:10.000000 financeager-1.3.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-07-16 11:56:10.000000 financeager-1.3.1/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-16 11:56:10.000000 financeager-1.3.1/test/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-16 11:56:10.000000 financeager-1.3.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-16 11:56:10.000000 financeager-1.3.1/test/test_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-16 11:56:10.000000 financeager-1.3.1/test/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23123 2023-07-16 11:56:10.000000 financeager-1.3.1/test/test_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-16 11:56:10.000000 financeager-1.3.1/test/test_server.py
```

### Comparing `financeager-1.3.0/.github/workflows/ci.yml` & `financeager-1.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/.github/workflows/release.yml` & `financeager-1.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/.pre-commit-config.yaml` & `financeager-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/Changelog.md` & `financeager-1.3.1/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 ## [unreleased]
 ### Added
 ### Changed
 ### Fixed
 ### Removed
 ### Deprecated
 
+## [v1.3.1] - 2023-07-16
+### Changed
+- Update dependencies `rich` and `tinydb`. (#169,#170)
+
 ## [v1.3.0] - 2023-05-05
 ### Changed
 - Update dependencies `rich` and `argcomplete`. (#161,#163)
 ### Removed
 - Support for Python 3.7 is removed.
 
 ## [v1.2.1] - 2023-04-03
```

### Comparing `financeager-1.3.0/LICENSE.md` & `financeager-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/Makefile` & `financeager-1.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/PKG-INFO` & `financeager-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financeager
-Version: 1.3.0
+Version: 1.3.1
 Summary: command line tool for organizing finances
 Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/pylipp/financeager/issues
 Project-URL: Documentation, https://github.com/pylipp/financeager
 Project-URL: Homepage, https://github.com/pylipp/financeager
 Project-URL: Source Code, https://github.com/pylipp/financeager
```

### Comparing `financeager-1.3.0/README.md` & `financeager-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/examples/quickstart.svg` & `financeager-1.3.1/examples/quickstart.svg`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/__init__.py` & `financeager-1.3.1/financeager/__init__.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/cli.py` & `financeager-1.3.1/financeager/cli.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/clients.py` & `financeager-1.3.1/financeager/clients.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/config.py` & `financeager-1.3.1/financeager/config.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/entries.py` & `financeager-1.3.1/financeager/entries.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/exceptions.py` & `financeager-1.3.1/financeager/exceptions.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/listing.py` & `financeager-1.3.1/financeager/listing.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/localserver.py` & `financeager-1.3.1/financeager/localserver.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/plugin.py` & `financeager-1.3.1/financeager/plugin.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/pocket.py` & `financeager-1.3.1/financeager/pocket.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/rich.py` & `financeager-1.3.1/financeager/rich.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager/server.py` & `financeager-1.3.1/financeager/server.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/financeager.egg-info/PKG-INFO` & `financeager-1.3.1/financeager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financeager
-Version: 1.3.0
+Version: 1.3.1
 Summary: command line tool for organizing finances
 Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/pylipp/financeager/issues
 Project-URL: Documentation, https://github.com/pylipp/financeager
 Project-URL: Homepage, https://github.com/pylipp/financeager
 Project-URL: Source Code, https://github.com/pylipp/financeager
```

### Comparing `financeager-1.3.0/financeager.egg-info/SOURCES.txt` & `financeager-1.3.1/financeager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/pyproject.toml` & `financeager-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 license = {text = "GPLv3"}
 authors = [{ name = "Philipp Metzner", email = "beth.aleph@yahoo.de" }]
 dependencies = [
   "appdirs==1.4.4",
   "argcomplete==3.0.8",
   "marshmallow==3.19.0",
   "python-dateutil==2.8.2",
-  "rich==13.3.5",
-  "tinydb==4.7.1",
+  "rich==13.4.2",
+  "tinydb==4.8.0",
 ]
 dynamic = [
   "version",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
@@ -41,20 +41,20 @@
   "Topic :: Office/Business :: Financial",
   "Topic :: Database",
   "Topic :: Utilities",
 ]
 [project.optional-dependencies]
 develop = [
   "black==23.3.0",
-  "coverage==7.2.5",
+  "coverage==7.2.7",
   'flake8==6.0.0',
   "flake8-pyproject==1.2.3",
   "gitlint-core==0.19.1",
   'isort==5.12.0',
-  'pre-commit==3.3.0',
+  'pre-commit==3.3.3',
 ]
 packaging = [
   "build",
   "twine>=1.11",
 ]
 
 [project.urls]
```

### Comparing `financeager-1.3.0/test/test_cli.py` & `financeager-1.3.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/test/test_clients.py` & `financeager-1.3.1/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/test/test_config.py` & `financeager-1.3.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/test/test_entries.py` & `financeager-1.3.1/test/test_entries.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/test/test_listing.py` & `financeager-1.3.1/test/test_listing.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/test/test_pocket.py` & `financeager-1.3.1/test/test_pocket.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.0/test/test_server.py` & `financeager-1.3.1/test/test_server.py`

 * *Files identical despite different names*

