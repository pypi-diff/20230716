# Comparing `tmp/sigils-0.2.8.tar.gz` & `tmp/sigils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigils-0.2.8.tar", last modified: Wed Mar 15 01:45:33 2023, max compression
+gzip compressed data, was "sigils-0.3.1.tar", last modified: Sun Jul 16 05:21:23 2023, max compression
```

## Comparing `sigils-0.2.8.tar` & `sigils-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.762987 sigils-0.2.8/
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.615388 sigils-0.2.8/.github/
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.647410 sigils-0.2.8/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      872 2023-03-08 18:03:31.000000 sigils-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      337 2023-03-06 18:49:20.000000 sigils-0.2.8/.github/ISSUE_TEMPLATE/standard-feature-request.md
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.649404 sigils-0.2.8/.github/workflows/
--rw-rw-rw-   0        0        0       84 2023-03-09 14:32:40.000000 sigils-0.2.8/.github/workflows/tests.yml
--rw-rw-rw-   0        0        0     1848 2021-03-21 06:16:52.000000 sigils-0.2.8/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.651409 sigils-0.2.8/.vscode/
--rw-rw-rw-   0        0        0      129 2023-02-04 01:12:09.000000 sigils-0.2.8/.vscode/settings.json
--rw-rw-rw-   0        0        0      567 2023-03-15 01:30:01.000000 sigils-0.2.8/CHANGELOG.md
--rw-rw-rw-   0        0        0    21090 2023-03-15 01:45:33.761986 sigils-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    19948 2023-03-08 21:41:38.000000 sigils-0.2.8/README.rst
--rw-rw-rw-   0        0        0     1485 2023-03-15 01:45:27.000000 sigils-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       73 2023-03-08 22:05:02.000000 sigils-0.2.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 01:45:33.763989 sigils-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.671463 sigils-0.2.8/sigils/
--rw-rw-rw-   0        0        0      116 2023-03-05 22:42:40.000000 sigils-0.2.8/sigils/__init__.py
--rw-rw-rw-   0        0        0       33 2023-01-30 04:10:42.000000 sigils-0.2.8/sigils/__main__.py
--rw-rw-rw-   0        0        0     2051 2023-03-09 15:10:31.000000 sigils-0.2.8/sigils/cli.py
--rw-rw-rw-   0        0        0     9256 2023-03-09 16:54:24.000000 sigils-0.2.8/sigils/contexts.py
--rw-rw-rw-   0        0        0      297 2023-03-08 03:11:15.000000 sigils-0.2.8/sigils/errors.py
--rw-rw-rw-   0        0        0     7166 2023-03-08 17:43:19.000000 sigils-0.2.8/sigils/parser.py
--rw-rw-rw-   0        0        0     1427 2023-03-08 23:23:15.000000 sigils-0.2.8/sigils/sigils.py
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.740474 sigils-0.2.8/sigils/tests/
--rw-rw-rw-   0        0        0        0 2023-01-30 00:31:30.000000 sigils-0.2.8/sigils/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.759988 sigils-0.2.8/sigils/tests/data/
--rw-rw-rw-   0        0        0       50 2023-03-08 22:22:18.000000 sigils-0.2.8/sigils/tests/data/context.ini
--rw-rw-rw-   0        0        0       59 2023-03-08 22:12:55.000000 sigils-0.2.8/sigils/tests/data/context.json
--rw-rw-rw-   0        0        0       64 2023-03-08 22:23:34.000000 sigils-0.2.8/sigils/tests/data/context.py
--rw-rw-rw-   0        0        0       43 2023-03-08 22:22:54.000000 sigils-0.2.8/sigils/tests/data/context.toml
--rw-rw-rw-   0        0        0       35 2023-03-08 22:21:27.000000 sigils-0.2.8/sigils/tests/data/context.yaml
--rw-rw-rw-   0        0        0     2183 2023-03-09 16:50:03.000000 sigils-0.2.8/sigils/tests/data/event.json
--rw-rw-rw-   0        0        0       68 2023-03-08 02:53:12.000000 sigils-0.2.8/sigils/tests/data/sample3.txt
--rw-rw-rw-   0        0        0       38 2023-03-04 20:32:43.000000 sigils-0.2.8/sigils/tests/data/settings.ini
--rw-rw-rw-   0        0        0      573 2023-03-08 17:56:52.000000 sigils-0.2.8/sigils/tests/test_cli.py
--rw-rw-rw-   0        0        0     4133 2023-03-08 20:49:29.000000 sigils-0.2.8/sigils/tests/test_context.py
--rw-rw-rw-   0        0        0     2316 2023-03-08 20:49:29.000000 sigils-0.2.8/sigils/tests/test_models.py
--rw-rw-rw-   0        0        0     1452 2023-03-08 20:34:33.000000 sigils-0.2.8/sigils/tests/test_parser.py
--rw-rw-rw-   0        0        0      958 2023-03-05 21:02:23.000000 sigils-0.2.8/sigils/tests/test_sysenv.py
--rw-rw-rw-   0        0        0     4303 2023-03-08 20:49:29.000000 sigils-0.2.8/sigils/tests/test_tools.py
--rw-rw-rw-   0        0        0     6401 2023-03-15 01:29:24.000000 sigils-0.2.8/sigils/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-15 01:45:33.719457 sigils-0.2.8/sigils.egg-info/
--rw-rw-rw-   0        0        0    21090 2023-03-15 01:45:33.000000 sigils-0.2.8/sigils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-03-15 01:45:33.000000 sigils-0.2.8/sigils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 01:45:33.000000 sigils-0.2.8/sigils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-03-15 01:45:33.000000 sigils-0.2.8/sigils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-03-15 01:45:33.000000 sigils-0.2.8/sigils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-15 01:45:33.000000 sigils-0.2.8/sigils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      220 2023-03-09 14:26:31.000000 sigils-0.2.8/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-16 05:21:23.668389 sigils-0.3.1/
+-rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.1/.gitignore
+-rw-rw-rw-   0        0        0     1001 2023-07-16 02:58:04.000000 sigils-0.3.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     4453 2023-07-16 05:21:23.666233 sigils-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3489 2023-07-16 02:50:25.000000 sigils-0.3.1/README.rst
+-rw-rw-rw-   0        0        0     1153 2023-07-16 02:57:41.000000 sigils-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 05:21:23.668389 sigils-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 05:21:23.597085 sigils-0.3.1/sigils/
+-rw-rw-rw-   0        0        0     7771 2023-07-16 05:07:20.000000 sigils-0.3.1/sigils/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.1/sigils/__main__.py
+-rw-rw-rw-   0        0        0     2633 2023-07-16 04:32:05.000000 sigils-0.3.1/sigils/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-16 05:21:23.661007 sigils-0.3.1/sigils.egg-info/
+-rw-rw-rw-   0        0        0     4453 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      437 2023-07-16 03:02:12.000000 sigils-0.3.1/test.json
```

### Comparing `sigils-0.2.8/.gitignore` & `sigils-0.3.1/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -118,8 +118,11 @@
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
-.pyre/
+.pyre/
+
+# json test fixtures
+.json
```

### Comparing `sigils-0.2.8/pyproject.toml` & `sigils-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,39 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigils"
-version = "0.2.8"
+version = "0.3.1"
 authors = [
     {name = "Rafael Jesús Guillén Osorio", email = "arthexis@gmail.com"},
 ]
-description = "Manage context-less text with [[SIGILS]]."
+description = "Interpolate with %[sigils]."
 readme = "README.rst"
-requires-python = ">=3.9"
-keywords = ["utils", "sigils", "string", "text", "magic", "context"]
+requires-python = ">=3.10"
+keywords = ["utils", "sigils", "string", "text", "context"]
 license = {text = "MIT"}
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Libraries',
-    'Topic :: Software Development :: Embedded Systems',
     'Topic :: Text Processing :: Markup',
     'Topic :: Software Development :: Pre-processors',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Environment :: Console',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 dependencies = [
-    'lark',
-    'lark-parser',
-    'click',
-    'pyyaml',
 ]
 
 [project.urls]
 Source = "https://github.com/arthexis/sigils"
 Bug-Tracker = "https://github.com/arthexis/sigils/issues"
 
-[project.optional-dependencies]
-django = [
-    "Django>=3.2"
-]
-dev = [
-    "pytest", 
-    "pytest-cov", 
-    "python-dotenv",
-    "tox",
-]
 
 [project.scripts]
-sigils = "sigils.cli:main"
+sigils = "sigils.__main__:main"
```

