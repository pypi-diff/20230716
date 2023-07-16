# Comparing `tmp/poetry-dotenv-plugin-0.1.0a2.tar.gz` & `tmp/poetry_dotenv_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-dotenv-plugin-0.1.0a2.tar", max compression
+gzip compressed data, was "poetry_dotenv_plugin-0.2.0.tar", max compression
```

## Comparing `poetry-dotenv-plugin-0.1.0a2.tar` & `poetry_dotenv_plugin-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,6 @@
--rw-r--r--   0        0        0     1059 2021-05-30 14:29:22.610687 poetry-dotenv-plugin-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     1345 2021-05-30 19:54:33.305121 poetry-dotenv-plugin-0.1.0a2/README.md
--rw-r--r--   0        0        0      181 2021-05-01 14:43:06.093009 poetry-dotenv-plugin-0.1.0a2/poetry_dotenv_plugin/UNKNOWN.egg-info/PKG-INFO
--rw-r--r--   0        0        0      123 2021-05-01 14:43:06.096071 poetry-dotenv-plugin-0.1.0a2/poetry_dotenv_plugin/UNKNOWN.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2021-05-01 14:43:06.093264 poetry-dotenv-plugin-0.1.0a2/poetry_dotenv_plugin/UNKNOWN.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2021-05-01 14:43:06.093552 poetry-dotenv-plugin-0.1.0a2/poetry_dotenv_plugin/UNKNOWN.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2021-04-28 12:44:15.398723 poetry-dotenv-plugin-0.1.0a2/poetry_dotenv_plugin/__init__.py
--rw-r--r--   0        0        0     1030 2021-05-30 13:52:43.390902 poetry-dotenv-plugin-0.1.0a2/poetry_dotenv_plugin/dotenv_plugin.py
--rw-r--r--   0        0        0      965 2021-05-30 19:59:09.280535 poetry-dotenv-plugin-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 poetry-dotenv-plugin-0.1.0a2/setup.py
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 poetry-dotenv-plugin-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-16 11:35:25.397691 poetry_dotenv_plugin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1999 2023-07-16 11:35:25.397691 poetry_dotenv_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 11:35:25.397691 poetry_dotenv_plugin-0.2.0/poetry_dotenv_plugin/__init__.py
+-rw-r--r--   0        0        0     1247 2023-07-16 11:35:25.397691 poetry_dotenv_plugin-0.2.0/poetry_dotenv_plugin/dotenv_plugin.py
+-rw-r--r--   0        0        0      973 2023-07-16 11:35:25.397691 poetry_dotenv_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 poetry_dotenv_plugin-0.2.0/PKG-INFO
```

### Comparing `poetry-dotenv-plugin-0.1.0a2/LICENSE` & `poetry_dotenv_plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-dotenv-plugin-0.1.0a2/README.md` & `poetry_dotenv_plugin-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Poetry Dotenv Plugin
 
+[![CI](https://github.com/mpeteuil/poetry-dotenv-plugin/actions/workflows/build.yml/badge.svg)](https://github.com/mpeteuil/poetry-dotenv-plugin/actions/workflows/build.yml)
+
 A [Poetry](https://python-poetry.org/) plugin that automatically loads environment variables from `.env` files into the environment before poetry commands are run.
 
-Supports Python 3.6+
+Supports Python 3.7+
 
 ```sh
 $ cat .env
 MY_ENV_VAR='Hello World'
 
 $ poetry run python -c 'import os; print(os.environ.get("MY_ENV_VAR"))'
 Hello World
@@ -17,18 +19,24 @@
 ### Origins
 
 Initial implementation based on the event handler application plugin example in the [Poetry docs](https://python-poetry.org/docs/plugins/#event-handler).
 
 ## Install
 
 ```sh
-poetry plugin add poetry-dotenv-plugin
+poetry self add poetry-dotenv-plugin
 ```
 
 ### Coming from Pipenv
 
 If you are transitioning from `pipenv` there shouldn't be much to change with regard to the `.env` loading. If you were a user of [`pipenv`'s environment variables](https://pipenv.pypa.io/en/latest/advanced/#automatic-loading-of-env) to control `.env` loading then you can use the analogous environment variables listed below.
 
 Pipenv env var | Poetry env var
 -------------- | ----------------------
 PIPENV_DOTENV_LOCATION | POETRY_DOTENV_LOCATION
 PIPENV_DONT_LOAD_ENV | POETRY_DONT_LOAD_ENV
+
+### Overriding existing environment variables
+
+By default, this plugin will override existing environment variables. This is because this plugin was built to make onboarding for users coming from `pipenv` as seamless as possible. If you want to prevent existing environment variables from being overridden, you can set the `POETRY_DOTENV_DONT_OVERRIDE` environment variable to `true`.[^1]
+
+[^1]: See [#16](https://github.com/mpeteuil/poetry-dotenv-plugin/pull/16) for background.
```

### Comparing `poetry-dotenv-plugin-0.1.0a2/pyproject.toml` & `poetry_dotenv_plugin-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dotenv-plugin"
-version = "0.1.0a2"
+version = "0.2.0"
 description = "A Poetry plugin to automatically load environment variables from .env files"
 authors = ["Michael Peteuil <michael.peteuil@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "poetry_dotenv_plugin"}]
 homepage = "https://github.com/mpeteuil/poetry-dotenv-plugin"
 repository = "https://github.com/mpeteuil/poetry-dotenv-plugin"
@@ -12,19 +12,19 @@
 classifiers = [
     "Topic :: Software Development",
     "Topic :: System :: Systems Administration",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = ">=3.7,<4"
 poetry = ">=1.2.0a1"
 python-dotenv = ">=0.10.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^6.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."poetry.application.plugin"]
```

### Comparing `poetry-dotenv-plugin-0.1.0a2/PKG-INFO` & `poetry_dotenv_plugin-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: poetry-dotenv-plugin
-Version: 0.1.0a2
+Version: 0.2.0
 Summary: A Poetry plugin to automatically load environment variables from .env files
 Home-page: https://github.com/mpeteuil/poetry-dotenv-plugin
 License: MIT
 Keywords: poetry,poetry-plugin,plugin,dotenv
 Author: Michael Peteuil
 Author-email: michael.peteuil@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Dist: poetry (>=1.2.0a1)
 Requires-Dist: python-dotenv (>=0.10.0)
 Project-URL: Repository, https://github.com/mpeteuil/poetry-dotenv-plugin
 Description-Content-Type: text/markdown
 
 # Poetry Dotenv Plugin
 
+[![CI](https://github.com/mpeteuil/poetry-dotenv-plugin/actions/workflows/build.yml/badge.svg)](https://github.com/mpeteuil/poetry-dotenv-plugin/actions/workflows/build.yml)
+
 A [Poetry](https://python-poetry.org/) plugin that automatically loads environment variables from `.env` files into the environment before poetry commands are run.
 
-Supports Python 3.6+
+Supports Python 3.7+
 
 ```sh
 $ cat .env
 MY_ENV_VAR='Hello World'
 
 $ poetry run python -c 'import os; print(os.environ.get("MY_ENV_VAR"))'
 Hello World
@@ -42,19 +44,25 @@
 ### Origins
 
 Initial implementation based on the event handler application plugin example in the [Poetry docs](https://python-poetry.org/docs/plugins/#event-handler).
 
 ## Install
 
 ```sh
-poetry plugin add poetry-dotenv-plugin
+poetry self add poetry-dotenv-plugin
 ```
 
 ### Coming from Pipenv
 
 If you are transitioning from `pipenv` there shouldn't be much to change with regard to the `.env` loading. If you were a user of [`pipenv`'s environment variables](https://pipenv.pypa.io/en/latest/advanced/#automatic-loading-of-env) to control `.env` loading then you can use the analogous environment variables listed below.
 
 Pipenv env var | Poetry env var
 -------------- | ----------------------
 PIPENV_DOTENV_LOCATION | POETRY_DOTENV_LOCATION
 PIPENV_DONT_LOAD_ENV | POETRY_DONT_LOAD_ENV
 
+### Overriding existing environment variables
+
+By default, this plugin will override existing environment variables. This is because this plugin was built to make onboarding for users coming from `pipenv` as seamless as possible. If you want to prevent existing environment variables from being overridden, you can set the `POETRY_DOTENV_DONT_OVERRIDE` environment variable to `true`.[^1]
+
+[^1]: See [#16](https://github.com/mpeteuil/poetry-dotenv-plugin/pull/16) for background.
+
```

