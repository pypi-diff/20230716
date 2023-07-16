# Comparing `tmp/financeager-flask-1.0.0.tar.gz` & `tmp/financeager-flask-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financeager-flask-1.0.0.tar", last modified: Tue Apr 25 09:50:38 2023, max compression
+gzip compressed data, was "financeager-flask-1.1.0.tar", last modified: Sun Jul 16 12:18:21 2023, max compression
```

## Comparing `financeager-flask-1.0.0.tar` & `financeager-flask-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.973162 financeager-flask-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.961162 financeager-flask-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.965162 financeager-flask-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-25 09:50:38.969162 financeager-flask-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.965162 financeager-flask-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/examples/fcgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/examples/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.965162 financeager-flask-1.0.0/financeager_flask/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.969162 financeager-flask-1.0.0/financeager_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 09:50:38.973162 financeager-flask-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.969162 financeager-flask-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_fflask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:18:21.297129 financeager-flask-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:18:21.293129 financeager-flask-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:18:21.293129 financeager-flask-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-16 12:18:21.297129 financeager-flask-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:18:21.293129 financeager-flask-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/examples/fcgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/examples/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:18:21.297129 financeager-flask-1.1.0/financeager_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/financeager_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/financeager_flask/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/financeager_flask/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/financeager_flask/httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/financeager_flask/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/financeager_flask/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/financeager_flask/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:18:21.297129 financeager-flask-1.1.0/financeager_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-16 12:18:21.000000 financeager-flask-1.1.0/financeager_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-16 12:18:21.000000 financeager-flask-1.1.0/financeager_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:18:21.000000 financeager-flask-1.1.0/financeager_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-16 12:18:21.000000 financeager-flask-1.1.0/financeager_flask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-16 12:18:21.000000 financeager-flask-1.1.0/financeager_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-16 12:18:21.000000 financeager-flask-1.1.0/financeager_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:18:21.297129 financeager-flask-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:18:21.297129 financeager-flask-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/test/test_fflask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/test/test_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/test/test_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-16 12:17:58.000000 financeager-flask-1.1.0/test/utils.py
```

### Comparing `financeager-flask-1.0.0/.github/workflows/ci.yml` & `financeager-flask-1.1.0/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   # This workflow contains a single job called "build"
   build:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.8, 3.9, "3.10"]
 
     # Steps represent a sequence of tasks that will be executed as part of the job
     steps:
       # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
```

### Comparing `financeager-flask-1.0.0/.github/workflows/release.yml` & `financeager-flask-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/.pre-commit-config.yaml` & `financeager-flask-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/Changelog.md` & `financeager-flask-1.1.0/Changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 
 ## [unreleased]
 ### Added
 ### Changed
 ### Removed
 ### Fixed
 
+## [v1.1.0] - 2023-07-16
+### Removed
+- Support for Python 3.7 is removed.
+### Changed
+- The upstream `financeager` dependency is required as lower than v1.4.0. (#34)
+
 ## [v1.0.0] - 2023-04-25
 ### Removed
 - Support for Python 3.6 is removed.
 ### Changed
 - The upstream `financeager` dependency is required as lower than v1.3.0. (#34)
 - The `setup.py` and `setup.cfg` files are replaced by `pyproject.toml` entirely.
```

### Comparing `financeager-flask-1.0.0/LICENSE` & `financeager-flask-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/Makefile` & `financeager-flask-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/PKG-INFO` & `financeager-flask-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: financeager-flask
-Version: 1.0.0
+Version: 1.1.0
 Summary: Plugin to use flask as backend for financeager
 Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/pylipp/financeager-flask/issues
 Project-URL: Documentation, https://github.com/pylipp/financeager-flask
 Project-URL: Homepage, https://github.com/pylipp/financeager-flask
 Project-URL: Source Code, https://github.com/pylipp/financeager-flask
 Keywords: commandline,finances
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
@@ -32,15 +31,15 @@
 
 # financeager-flask
 
 Plugin that enables you to run [financeager](https://github.com/pylipp/financeager) as a Flask-powered webservice!
 
 ## Installation
 
-`financeager-flask` requires Python 3.7 or higher.
+`financeager-flask` requires Python 3.8 or higher.
 
     pip install financeager-flask
 
 Installation via [`pipx`](https://pipxproject.github.io/pipx/) is recommended:
 
     pipx install financeager
     pipx inject financeager financeager-flask
```

### Comparing `financeager-flask-1.0.0/README.md` & `financeager-flask-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # financeager-flask
 
 Plugin that enables you to run [financeager](https://github.com/pylipp/financeager) as a Flask-powered webservice!
 
 ## Installation
 
-`financeager-flask` requires Python 3.7 or higher.
+`financeager-flask` requires Python 3.8 or higher.
 
     pip install financeager-flask
 
 Installation via [`pipx`](https://pipxproject.github.io/pipx/) is recommended:
 
     pipx install financeager
     pipx inject financeager financeager-flask
```

### Comparing `financeager-flask-1.0.0/examples/fcgi.py` & `financeager-flask-1.1.0/examples/fcgi.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/examples/wsgi.py` & `financeager-flask-1.1.0/examples/wsgi.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/financeager_flask/flask.py` & `financeager-flask-1.1.0/financeager_flask/flask.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/financeager_flask/httprequests.py` & `financeager-flask-1.1.0/financeager_flask/httprequests.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/financeager_flask/main.py` & `financeager-flask-1.1.0/financeager_flask/main.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/financeager_flask/offline.py` & `financeager-flask-1.1.0/financeager_flask/offline.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/financeager_flask/resources.py` & `financeager-flask-1.1.0/financeager_flask/resources.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/financeager_flask.egg-info/PKG-INFO` & `financeager-flask-1.1.0/financeager_flask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: financeager-flask
-Version: 1.0.0
+Version: 1.1.0
 Summary: Plugin to use flask as backend for financeager
 Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/pylipp/financeager-flask/issues
 Project-URL: Documentation, https://github.com/pylipp/financeager-flask
 Project-URL: Homepage, https://github.com/pylipp/financeager-flask
 Project-URL: Source Code, https://github.com/pylipp/financeager-flask
 Keywords: commandline,finances
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
@@ -32,15 +31,15 @@
 
 # financeager-flask
 
 Plugin that enables you to run [financeager](https://github.com/pylipp/financeager) as a Flask-powered webservice!
 
 ## Installation
 
-`financeager-flask` requires Python 3.7 or higher.
+`financeager-flask` requires Python 3.8 or higher.
 
     pip install financeager-flask
 
 Installation via [`pipx`](https://pipxproject.github.io/pipx/) is recommended:
 
     pipx install financeager
     pipx inject financeager financeager-flask
```

### Comparing `financeager-flask-1.0.0/financeager_flask.egg-info/SOURCES.txt` & `financeager-flask-1.1.0/financeager_flask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/pyproject.toml` & `financeager-flask-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -13,48 +13,45 @@
 keywords = [
   "commandline",
   "finances",
 ]
 license = {text = "GPLv3"}
 authors = [{ name = "Philipp Metzner", email = "beth.aleph@yahoo.de" }]
 dependencies = [
-  "financeager>=1.1.0,<1.3.0",
+  "financeager>=1.1.0,<1.4.0",
   "Flask>=1.0.2",
   "Flask-RESTful>=0.3.5",
   "requests>=2.20.0",
-  'importlib-metadata>=1.7.0;python_version<"3.8"',
 ]
 dynamic = [
   "version",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Intended Audience :: End Users/Desktop",
   "Intended Audience :: Other Audience",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: Unix",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Office/Business :: Financial",
   "Topic :: Database",
   "Topic :: Utilities",
 ]
 [project.optional-dependencies]
 develop = [
-  "black==22.10.0",
-  "coverage==6.5",
-  'flake8==6.0.0; python_version >= "3.8"',
-  'flake8==5.0.4; python_version < "3.8"',
-  "flake8-pyproject==1.2.2",
-  "gitlint-core==0.18.0",
-  "isort==5.10.1",
-  "pre-commit==2.20",
+  "black==23.3.0",
+  "coverage==7.2.7",
+  'flake8==6.0.0',
+  "flake8-pyproject==1.2.3",
+  "gitlint-core==0.19.1",
+  'isort==5.12.0',
+  'pre-commit==3.3.3',
 ]
 packaging = [
   "build",
   "twine>=1.11",
 ]
 
 [project.urls]
```

### Comparing `financeager-flask-1.0.0/test/test_cli.py` & `financeager-flask-1.1.0/test/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
             return response
 
         return response
 
 
 @mock.patch("financeager.DATA_DIR", TEST_DATA_DIR)
 class CliFlaskTestCase(CliTestCase):
-
     HOST_IP = "127.0.0.1:5000"
     CONFIG_FILE_CONTENT = """\
 [SERVICE]
 name = flask
 
 [FRONTEND]
 default_category = unspecified
```

### Comparing `financeager-flask-1.0.0/test/test_config.py` & `financeager-flask-1.1.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/test/test_fflask.py` & `financeager-flask-1.1.0/test/test_fflask.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/test/test_httprequests.py` & `financeager-flask-1.1.0/test/test_httprequests.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
                 "timeout": timeout,
             }
         )
 
         with patch(
             "financeager_flask.httprequests.requests.post", side_effect=self.mock_post
         ) as post_patch:
-
             proxy.run("pockets")
 
             url = "{}{}".format(DEFAULT_HOST, POCKETS_TAIL)
             kwargs = {
                 "json": None,
                 "auth": (username, password),
                 "timeout": timeout,
```

### Comparing `financeager-flask-1.0.0/test/test_offline.py` & `financeager-flask-1.1.0/test/test_offline.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-1.0.0/test/utils.py` & `financeager-flask-1.1.0/test/utils.py`

 * *Files identical despite different names*

