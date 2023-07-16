# Comparing `tmp/bcamp-dl-1.0.1.tar.gz` & `tmp/bcamp-dl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcamp-dl-1.0.1.tar", last modified: Sat Jul 15 02:43:48 2023, max compression
+gzip compressed data, was "bcamp-dl-1.0.2.tar", last modified: Sun Jul 16 05:01:11 2023, max compression
```

## Comparing `bcamp-dl-1.0.1.tar` & `bcamp-dl-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/templates/pr-build.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/bcamp-dl.sublime-project
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.060310 bcamp-dl-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/src/bcamp_dl/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 02:43:47.000000 bcamp-dl-1.0.1/src/bcamp_dl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/bcamp_dl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:43:31.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.571450 bcamp-dl-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.567450 bcamp-dl-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.567450 bcamp-dl-1.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.567450 bcamp-dl-1.0.2/.github/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/templates/pr-build.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.567450 bcamp-dl-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-16 05:01:11.571450 bcamp-dl-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/bcamp-dl.sublime-project
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 05:01:11.571450 bcamp-dl-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.567450 bcamp-dl-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.567450 bcamp-dl-1.0.2/src/bcamp_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/src/bcamp_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 05:01:11.000000 bcamp-dl-1.0.2/src/bcamp_dl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/src/bcamp_dl/bcamp_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/src/bcamp_dl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 05:00:44.000000 bcamp-dl-1.0.2/src/bcamp_dl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 05:01:11.571450 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-16 05:01:11.000000 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-16 05:01:11.000000 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 05:01:11.000000 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-16 05:01:11.000000 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 05:00:53.000000 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-16 05:01:11.000000 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 05:01:11.000000 bcamp-dl-1.0.2/src/bcamp_dl.egg-info/top_level.txt
```

### Comparing `bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `bcamp-dl-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `bcamp-dl-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/.github/workflows/build.yml` & `bcamp-dl-1.0.2/.github/workflows/build.yml`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 jobs:
   test:
     name: Test
     uses: ./.github/workflows/test.yml
 
   build:
     name: Build
-    if: ${{ github.event_name == 'workflow_dispatch' || github.event.pull_request.merged == true }}
+    if: github.event_name == 'workflow_dispatch' || github.event.pull_request.merged == true || startsWith(github.ref, 'refs/tags/release/')
     needs:
       - test
     runs-on: ubuntu-latest
     environment: build
     permissions:
       id-token: write
       issues: write
@@ -75,21 +75,21 @@
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           print-hash: true
           repository-url: https://test.pypi.org/legacy/
 
       - name: Render PR Template
         id: pr-template
-        if: ${{ github.event_name == 'pull_request_target' }}
+        if: github.event_name == 'pull_request_target'
         uses: chuhlomin/render-template@v1.4
         with:
           template: ./.github/templates/pr-build.md
           vars: |
             version: ${{ steps.version.outputs.version }}
 
       - name: Update PR with Build
-        if: ${{ github.event_name == 'pull_request_target' }}
+        if: github.event_name == 'pull_request_target'
         uses: peter-evans/create-or-update-comment@v3
         with:
           issue-number: ${{ github.event.pull_request.number }}
           body: ${{ steps.pr-template.outputs.result }}
           reactions: rocket
```

### Comparing `bcamp-dl-1.0.1/.github/workflows/release.yml` & `bcamp-dl-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/.github/workflows/test.yml` & `bcamp-dl-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/.gitignore` & `bcamp-dl-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/.pre-commit-config.yaml` & `bcamp-dl-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/LICENSE` & `bcamp-dl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/PKG-INFO` & `bcamp-dl-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcamp-dl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Download your collection from Bandcamp.
 Author-email: ReK42 <ReK42@users.noreply.github.com>
 Maintainer-email: ReK42 <ReK42@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 ReK42
         
@@ -47,40 +47,43 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: build
 License-File: LICENSE
 
 # bcamp-dl
-
-[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
 [![PyPi Version](https://img.shields.io/pypi/v/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
 [![PyPI Status](https://img.shields.io/pypi/status/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
 [![Python Versions](https://img.shields.io/pypi/pyversions/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
 [![Last Commit](https://img.shields.io/github/last-commit/ReK42/bcamp-dl/main?logo=github)](https://github.com/ReK42/bcamp-dl/commits/main)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/ReK42/bcamp-dl/build.yml?logo=github)](https://github.com/ReK42/bcamp-dl/actions)
-[![Linted by Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Linted by Ruff](https://img.shields.io/badge/linting-ruff-purple?logo=ruff&logoColor=white)](https://github.com/astral-sh/ruff)
 [![Code Style by Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Download your collection from Bandcamp.
 
 ## Installation
+Install [Python](https://www.python.org/downloads/), then install `pipx` and use it to install `bcamp-dl`:
 ```sh
+python -m pip install --upgrade pip setuptools pipx
 pipx install bcamp-dl
 ```
 
-For developers: Merged pull requests will automatically create dev builds on [TestPyPI](https://test.pypi.org/project/bcamp-dl)
-
 ## Usage
-```
+To use, login to Bandcamp using one of the supported browsers. All albums in your collection will be downloaded to the output directory, with subfolders, based on the filename format selected. If not specified, the defaults are to use Firefox and download as MP3 V0 to per-artist subfolders in the current directory.
+```sh
 bcamp-dl --browser <BROWSER> --file-format <FORMAT> --directory <DIR> <USERNAME>
 ```
 
 For all options, run `bcamp-dl --help`
 
 ## Development Environment
 ```sh
 git clone https://github.com/ReK42/bcamp-dl.git
 cd bcamp-dl
+python -m venv .env
+source .env/bin/activate
+python -m pip install --upgrade pip setuptools pre-commit
 pre-commit install
 pip install -e .[tests]
 ```
```

### Comparing `bcamp-dl-1.0.1/bcamp-dl.sublime-project` & `bcamp-dl-1.0.2/bcamp-dl.sublime-project`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/pyproject.toml` & `bcamp-dl-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/src/bcamp_dl/bcamp_dl.py` & `bcamp-dl-1.0.2/src/bcamp_dl/bcamp_dl.py`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/src/bcamp_dl/cli.py` & `bcamp-dl-1.0.2/src/bcamp_dl/cli.py`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.1/src/bcamp_dl.egg-info/PKG-INFO` & `bcamp-dl-1.0.2/src/bcamp_dl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcamp-dl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Download your collection from Bandcamp.
 Author-email: ReK42 <ReK42@users.noreply.github.com>
 Maintainer-email: ReK42 <ReK42@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 ReK42
         
@@ -47,40 +47,43 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: build
 License-File: LICENSE
 
 # bcamp-dl
-
-[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
 [![PyPi Version](https://img.shields.io/pypi/v/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
 [![PyPI Status](https://img.shields.io/pypi/status/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
 [![Python Versions](https://img.shields.io/pypi/pyversions/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
 [![Last Commit](https://img.shields.io/github/last-commit/ReK42/bcamp-dl/main?logo=github)](https://github.com/ReK42/bcamp-dl/commits/main)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/ReK42/bcamp-dl/build.yml?logo=github)](https://github.com/ReK42/bcamp-dl/actions)
-[![Linted by Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Linted by Ruff](https://img.shields.io/badge/linting-ruff-purple?logo=ruff&logoColor=white)](https://github.com/astral-sh/ruff)
 [![Code Style by Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Download your collection from Bandcamp.
 
 ## Installation
+Install [Python](https://www.python.org/downloads/), then install `pipx` and use it to install `bcamp-dl`:
 ```sh
+python -m pip install --upgrade pip setuptools pipx
 pipx install bcamp-dl
 ```
 
-For developers: Merged pull requests will automatically create dev builds on [TestPyPI](https://test.pypi.org/project/bcamp-dl)
-
 ## Usage
-```
+To use, login to Bandcamp using one of the supported browsers. All albums in your collection will be downloaded to the output directory, with subfolders, based on the filename format selected. If not specified, the defaults are to use Firefox and download as MP3 V0 to per-artist subfolders in the current directory.
+```sh
 bcamp-dl --browser <BROWSER> --file-format <FORMAT> --directory <DIR> <USERNAME>
 ```
 
 For all options, run `bcamp-dl --help`
 
 ## Development Environment
 ```sh
 git clone https://github.com/ReK42/bcamp-dl.git
 cd bcamp-dl
+python -m venv .env
+source .env/bin/activate
+python -m pip install --upgrade pip setuptools pre-commit
 pre-commit install
 pip install -e .[tests]
 ```
```

### Comparing `bcamp-dl-1.0.1/src/bcamp_dl.egg-info/SOURCES.txt` & `bcamp-dl-1.0.2/src/bcamp_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

