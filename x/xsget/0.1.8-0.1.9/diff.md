# Comparing `tmp/xsget-0.1.8.tar.gz` & `tmp/xsget-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsget-0.1.8.tar", last modified: Sun Apr 16 04:35:30 2023, max compression
+gzip compressed data, was "xsget-0.1.9.tar", last modified: Sun May 28 12:58:21 2023, max compression
```

## Comparing `xsget-0.1.8.tar` & `xsget-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      104 2023-03-18 10:31:29.623190 xsget-0.1.8/.coveragerc
--rw-r--r--   0        0        0     1919 2023-03-24 14:01:29.280123 xsget-0.1.8/.gitignore
--rw-r--r--   0        0        0     2607 2023-04-15 13:24:35.236799 xsget-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       36 2023-04-05 23:46:00.757628 xsget-0.1.8/.python-version
--rw-r--r--   0        0        0     4120 2023-04-16 04:34:20.701509 xsget-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     1590 2023-04-14 14:54:29.535457 xsget-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2022-09-03 12:07:10.610397 xsget-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     5145 2023-03-20 15:47:55.552686 xsget-0.1.8/README.md
--rw-r--r--   0        0        0      782 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/Makefile
--rw-r--r--   0        0        0      804 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    63990 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/_static/logo.png
--rw-r--r--   0        0        0     2473 2022-09-28 15:08:05.153213 xsget-0.1.8/docs/source/conf.py
--rw-r--r--   0        0        0      202 2022-05-06 12:58:04.555971 xsget-0.1.8/docs/source/index.rst
--rw-r--r--   0        0        0      533 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/xsget.rst
--rw-r--r--   0        0        0      471 2022-07-16 05:50:26.995584 xsget-0.1.8/docs/source/xstxt.md
--rw-r--r--   0        0        0      426 2023-03-24 23:09:21.188668 xsget-0.1.8/locales/en/LC_MESSAGES/xstxt.mo
--rw-r--r--   0        0        0      616 2023-03-06 13:28:02.776464 xsget-0.1.8/locales/en/LC_MESSAGES/xstxt.po
--rw-r--r--   0        0        0      571 2023-03-25 09:30:21.493991 xsget-0.1.8/locales/xstxt.pot
--rw-r--r--   0        0        0      427 2023-03-24 23:09:21.192668 xsget-0.1.8/locales/zh/LC_MESSAGES/xstxt.mo
--rw-r--r--   0        0        0      617 2023-03-06 13:28:02.776464 xsget-0.1.8/locales/zh/LC_MESSAGES/xstxt.po
--rw-r--r--   0        0        0     2998 2023-04-08 06:52:10.846647 xsget-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-15 14:02:04.220660 xsget-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      257 2022-06-04 02:46:26.216686 xsget-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     4863 2023-04-08 07:01:14.579946 xsget-0.1.8/tests/test_xsget.py
--rw-r--r--   0        0        0     8758 2023-03-21 13:38:27.613019 xsget-0.1.8/tests/test_xstxt.py
--rw-r--r--   0        0        0     4295 2023-04-16 04:34:33.621575 xsget-0.1.8/xsget/__init__.py
--rw-r--r--   0        0        0      355 2022-07-01 22:44:04.742450 xsget-0.1.8/xsget/book.py
--rw-r--r--   0        0        0      920 2023-02-28 09:58:00.269999 xsget-0.1.8/xsget/chapter.py
--rw-r--r--   0        0        0    13457 2023-04-14 14:01:38.733820 xsget-0.1.8/xsget/xsget.py
--rw-r--r--   0        0        0     1526 2022-12-27 10:58:29.556852 xsget-0.1.8/xsget/xsget.toml
--rw-r--r--   0        0        0    17162 2023-04-06 23:39:41.532743 xsget-0.1.8/xsget/xstxt.py
--rw-r--r--   0        0        0     3408 2023-02-01 09:54:23.862432 xsget-0.1.8/xsget/xstxt.toml
--rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 xsget-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      104 2023-04-24 07:55:55.261518 xsget-0.1.9/.coveragerc
+-rw-r--r--   0        0        0     1919 2023-04-24 07:55:55.261518 xsget-0.1.9/.gitignore
+-rw-r--r--   0        0        0     2616 2023-05-25 12:25:29.332269 xsget-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       36 2023-04-24 07:55:55.265518 xsget-0.1.9/.python-version
+-rw-r--r--   0        0        0     4514 2023-05-28 12:53:38.296373 xsget-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1775 2023-05-25 12:03:46.447169 xsget-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2022-09-02 14:41:24.441841 xsget-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     5363 2023-05-25 12:27:25.777401 xsget-0.1.9/README.md
+-rw-r--r--   0        0        0      782 2022-04-13 01:07:39.320671 xsget-0.1.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-03-14 14:02:55.911550 xsget-0.1.9/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-04-24 07:28:20.840663 xsget-0.1.9/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-04-24 07:28:20.828663 xsget-0.1.9/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-04-24 07:28:20.832663 xsget-0.1.9/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-04-24 07:28:20.832663 xsget-0.1.9/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    63990 2022-03-14 14:52:13.993170 xsget-0.1.9/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     2473 2022-09-30 16:51:41.686428 xsget-0.1.9/docs/source/conf.py
+-rw-r--r--   0        0        0      202 2022-05-02 09:01:13.307163 xsget-0.1.9/docs/source/index.rst
+-rw-r--r--   0        0        0      533 2022-03-31 15:53:59.135397 xsget-0.1.9/docs/source/xsget.rst
+-rw-r--r--   0        0        0      471 2022-07-13 14:43:57.947353 xsget-0.1.9/docs/source/xstxt.md
+-rw-r--r--   0        0        0      426 2023-04-24 07:55:55.265518 xsget-0.1.9/locales/en/LC_MESSAGES/xstxt.mo
+-rw-r--r--   0        0        0      616 2023-04-24 07:55:55.265518 xsget-0.1.9/locales/en/LC_MESSAGES/xstxt.po
+-rw-r--r--   0        0        0      571 2023-04-24 07:55:55.265518 xsget-0.1.9/locales/xstxt.pot
+-rw-r--r--   0        0        0      427 2023-04-24 07:55:55.265518 xsget-0.1.9/locales/zh/LC_MESSAGES/xstxt.mo
+-rw-r--r--   0        0        0      617 2023-04-24 07:55:55.265518 xsget-0.1.9/locales/zh/LC_MESSAGES/xstxt.po
+-rw-r--r--   0        0        0     3242 2023-05-14 13:49:38.620824 xsget-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-14 15:34:15.808734 xsget-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      257 2022-05-26 14:21:34.585186 xsget-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     4896 2023-05-12 11:45:34.186967 xsget-0.1.9/tests/test_xsget.py
+-rw-r--r--   0        0        0     8758 2023-04-24 07:55:55.265518 xsget-0.1.9/tests/test_xstxt.py
+-rw-r--r--   0        0        0     4296 2023-05-28 12:54:08.392896 xsget-0.1.9/xsget/__init__.py
+-rw-r--r--   0        0        0      355 2022-05-15 09:21:27.338663 xsget-0.1.9/xsget/book.py
+-rw-r--r--   0        0        0      920 2023-04-24 07:55:55.265518 xsget-0.1.9/xsget/chapter.py
+-rw-r--r--   0        0        0    13513 2023-05-12 11:45:34.186967 xsget-0.1.9/xsget/xsget.py
+-rw-r--r--   0        0        0     1526 2022-10-13 15:56:17.544266 xsget-0.1.9/xsget/xsget.toml
+-rw-r--r--   0        0        0    18535 2023-05-28 12:38:45.569705 xsget-0.1.9/xsget/xstxt.py
+-rw-r--r--   0        0        0     3408 2023-04-24 07:55:55.269518 xsget-0.1.9/xsget/xstxt.toml
+-rw-r--r--   0        0        0     7854 1970-01-01 00:00:00.000000 xsget-0.1.9/PKG-INFO
```

### Comparing `xsget-0.1.8/.gitignore` & `xsget-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/.pre-commit-config.yaml` & `xsget-0.1.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
       - id: trailing-whitespace
       - id: end-of-file-fixer
         exclude: "locales/.*$"
       - id: check-yaml
       - id: check-toml
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.13
     hooks:
       - id: validate-pyproject
         name: validate pyproject
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
 
   - repo: https://github.com/pycqa/isort
     rev: 5.11.5
     hooks:
       - id: isort
@@ -50,15 +50,15 @@
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==22.8.0
 
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.2
+    rev: v2.1.1
     hooks:
       - id: autoflake
         args:
           - --in-place
           - --remove-unused-variables
           - --remove-all-unused-imports
         language: python
@@ -95,13 +95,13 @@
           - xsget
           - tests
           - --py-version=3.7
           - --disable=R0801,W0612
           - --unsafe-load-any-extension=y
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         exclude: docs/
         additional_dependencies:
           - types-aiofiles
```

### Comparing `xsget-0.1.8/CHANGELOG.md` & `xsget-0.1.9/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,33 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.1.9 - 2023-05-28
+
+### Added
+
+- Add watching mode, `-m` or `--monitor` for `xstxt` to regenerate the content
+  from html files
+
+### Changed
+
+- Update project classifiers and dependencies
+- Run test randomly by default
+- Update PyPi's classifiers
+
+### Fixed
+
+- Fix session not closed during test
+- Resolve raising generic exception
+- Use `pip install -e` to install local development copy
+
 ## v0.1.8 - 2023-04-16
 
 ### Added
 
 - Add multiprocessor support for `pytest`
 
 ### Changed
```

### Comparing `xsget-0.1.8/CONTRIBUTING.md` & `xsget-0.1.9/CONTRIBUTING.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 pyenv install 3.10.11
 pyenv install 3.11.3
 ```
 
 Install and upgrade required Python packages:
 
 ```console
-python -m pip install --upgrade pip flit tox tox-pyenv pylint pre-commit
+python -m pip install --upgrade pip flit pytest pylint pre-commit playwright "tox<4" tox-pyenv
 ```
 
 Clone repository from GitHub and setting up the development environment:
 
 ```console
 git clone https://github.com/kianmeng/xsget
 cd xsget
-flit install --symlink
+python -m pip install -e .
 playwright install
 ```
 
 Show all available tox tasks:
 
 ```console
 $ tox -av
@@ -79,7 +79,12 @@
 Push to the branch:
 
 ```console
 git push origin my-new-feature
 ```
 
 Create new Pull Request in GitHub.
+
+## License
+
+By contributing to xsget, you agree that your contributions will be licensed
+under the LICENSE.md file in the root directory of this source tree.
```

### Comparing `xsget-0.1.8/LICENSE.md` & `xsget-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/README.md` & `xsget-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # xsget
 
 Console tools to download online novel and convert to text file.
 
 ## Installation
 
-Stable version From PyPI:
+Stable version From PyPI using `pipx`:
 
 ```console
-python3 -m pip install xsget
+pipx install xsget playwright
+playwright install
+```
+
+Stable version From PyPI using `pip`:
+
+```console
+python3 -m pip install xsget playwright
 playwright install
 ```
 
 Latest development version from GitHub:
 
 ```console
 python3 -m pip install -e git+https://github.com/kianmeng/xsget.git
@@ -48,41 +55,42 @@
   -r, --refresh
         refresh the index page
   -t, --test
         show extracted urls without crawling
   -b, --browser
         crawl by actual browser (default: 'False')
   -bs SESSION, --browser-session SESSION
-        set the number of browser session (default: 5)
+        set the number of browser session (default: 2)
   -bd DELAY, --browser-delay DELAY
         set the second to wait for page to load in browser (default: 0)
   -d, --debug
         show debugging log and stacktrace
   -h, --help
         show this help message and exit
   -V, --version
         show program's version number and exit
 
 examples:
   xsget http://localhost
   xsget http://localhost/page[1-100].html
+  xsget -g -l "a" -p "id" http://localhost
 ```
 
 ## xstxt
 
 ```console
 xstxt -h
 ```
 
 ```console
 usage: xstxt [-pt CSS_PATH] [-pb CSS_PATH] [-la LANGUAGE] [-ps SEPARATOR]
              [-rh REGEX REGEX] [-rt REGEX REGEX] [-bt TITLE] [-ba AUTHOR]
              [-ic INDENT_CHARS] [-fw] [-oi] [-i GLOB_PATTERN]
              [-e GLOB_PATTERN] [-l TOTAL_FILES] [-w WIDTH] [-o FILENAME]
-             [-g [FILENAME] | -c [FILENAME]] [-wf] [-d] [-h] [-V]
+             [-g [FILENAME] | -c [FILENAME]] [-m] [-d] [-h] [-V]
 
 xstxt is a cli app that extract content from HTML to text file.
   website: https://github.com/kianmeng/xsget
   issues: https://github.com/kianmeng/xsget/issues
 
 optional arguments:
   -pt CSS_PATH, --title-css-path CSS_PATH
@@ -117,26 +125,26 @@
         set the line width for wrapping (default: 0, 0 to disable)
   -o FILENAME, --output FILENAME
         set output txt file name (default: 'book.txt')
   -g [FILENAME], --generate-config-file [FILENAME]
         generate config file from options (default: 'xstxt.toml')
   -c [FILENAME], --config-file [FILENAME]
         load config from file (default: 'xstxt.toml')
-  -wf, --watch-files
-        enable watch on file changes
+  -m, --monitor
+        monitor config file changes and re-run when needed
   -d, --debug
         show debugging log and stacktrace
   -h, --help
         show this help message and exit
   -V, --version
         show program's version number and exit
 
 examples:
-  xstxt -i *.html
-  xstxt -oi -i *.html
+  xstxt --input *.html
+  xstxt --output-individual-file --input *.html
 ```
 
 ## Copyright and License
 
 Copyright (C) 2021,2022,2023 Kian-Meng Ang
 
 This program is free software: you can redistribute it and/or modify it under
```

### Comparing `xsget-0.1.8/docs/Makefile` & `xsget-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/docs/make.bat` & `xsget-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/docs/source/_static/logo.png` & `xsget-0.1.9/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/docs/source/conf.py` & `xsget-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/docs/source/xsget.rst` & `xsget-0.1.9/docs/source/xsget.rst`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/locales/en/LC_MESSAGES/xstxt.po` & `xsget-0.1.9/locales/en/LC_MESSAGES/xstxt.po`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/locales/xstxt.pot` & `xsget-0.1.9/locales/xstxt.pot`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/locales/zh/LC_MESSAGES/xstxt.po` & `xsget-0.1.9/locales/zh/LC_MESSAGES/xstxt.po`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/pyproject.toml` & `xsget-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,80 +10,87 @@
 license = {file = "LICENSE.md"}
 authors = [{name = "Kian-Meng, Ang", email = "kianmeng@cpan.org"}]
 requires-python = ">=3.7"
 dependencies = [
   "aiofiles",
   "aiohttp",
   "bs4",
+  "cssselect",
   "lxml",
   "natsort",
   "playwright",
   "regex",
   "tomlkit",
   "user_agent",
-  "cssselect",
+  "watchdog",
 ]
 dynamic = [
   "description",
   "version",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+    "Natural Language :: Chinese (Simplified)",
+    "Natural Language :: Chinese (Traditional)",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python",
+    "Topic :: Text Processing :: Filters",
     "Topic :: Text Processing :: General",
     "Topic :: Text Processing :: Markup :: HTML",
+    "Topic :: Text Processing",
 ]
 [project.optional-dependencies]
 dev = [
   "black",
   "isort",
+  "line-profiler",
   "pre-commit",
-  "tox<4",
   "tox-pyenv",
-  "line-profiler",
+  "tox<4",
 ]
 doc = [
   "myst_parser",
   "sphinx",
+  "sphinx-autodoc-typehints",
   "sphinx_autobuild",
   "sphinx_copybutton",
-  "sphinx-autodoc-typehints",
 ]
 test = [
   "aioresponses",
   "playwright",
   "pytest",
   "pytest-asyncio",
   "pytest-console-scripts",
   "pytest-cov",
-  "pytest-xdist",
   "pytest-mock",
   "pytest-playwright",
+  "pytest-randomly",
+  "pytest-xdist",
   "types-aiofiles",
 ]
 
 [project.urls]
 Issues = "https://github.com/kianmeng/xsget/issues"
 Source = "https://github.com/kianmeng/xsget"
 
 [project.scripts]
 xsget = "xsget.xsget:cli"
 xstxt = "xsget.xstxt:cli"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-vv -s -q -x"
-asyncio_mode = "strict"
+asyncio_mode = "auto"
 script_launch_mode = "subprocess"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
 envlist = py3{7,8,9,10,11}
@@ -93,15 +100,15 @@
 deps = .[test]
 commands = pytest --numprocesses auto --hide-run-results
 
 [testenv:cover]
 description = generate code coverage report in html
 basepython = python3.11
 deps = .[test]
-commands = pytest --numprocesses auto --cov=xsget --cov-report term-missing --cov-report html {toxinidir}/tests
+commands = pytest --numprocesses auto --cov=xsget --ctov-report term-missing --cov-report html {toxinidir}/tests
 
 [testenv:doc]
 description = generate sphinx documentation in html
 basepython = python3.11
 deps = .[doc]
 commands = sphinx-build {toxinidir}/docs/source/ {toxinidir}/docs/_build/html
```

### Comparing `xsget-0.1.8/tests/test_xsget.py` & `xsget-0.1.9/tests/test_xsget.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         assert log in ret.stdout
 
 
 def test_raise_exception_for_invalid_range_in_url(script_runner):
     ret = script_runner.run(*argv(f"xsget -d -t {DEFAULT_URL}/[2-1].html"))
     logs = [
         "ERROR: xsget.xsget: error: invalid url range, start: 2, end: 1",
-        "Exception: invalid url range, start: 2, end: 1",
+        "RuntimeError: invalid url range, start: 2, end: 1",
     ]
     for log in logs:
         assert log in ret.stdout
 
 
 def test_generating_default_config_file(script_runner):
     ret = script_runner.run(*argv(f"xsget {DEFAULT_URL} -g"))
@@ -147,18 +147,19 @@
 def test_user_agent():
     user_agent = http_headers()["User-Agent"]
     assert "Mozilla/5.0" in user_agent
 
 
 async def test_fetch_url_by_aiohttp(tmpdir):
     session = aiohttp.ClientSession()
-
     with aioresponses() as mocked:
         config = argparse.Namespace(url_param_as_filename="")
         mocked.get(DEFAULT_URL, status=200, body="test")
 
         resp = await fetch_url_by_aiohttp(session, DEFAULT_URL, config)
         assert resp.status == 200
         mocked.assert_called_once_with(DEFAULT_URL)
 
         with open(Path(tmpdir, "index.html"), encoding="utf8") as file:
             assert file.read() == "test"
+
+        await session.close()
```

### Comparing `xsget-0.1.8/tests/test_xstxt.py` & `xsget-0.1.9/tests/test_xstxt.py`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/xsget/__init__.py` & `xsget-0.1.9/xsget/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from datetime import datetime as dt
 from importlib.resources import read_text
 from pathlib import Path
 from typing import Dict
 
 import tomlkit
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 _logger = logging.getLogger(__name__)
 
 
 class ConfigFileCorruptedError(Exception):
     """Config file corrupted after reading."""
 
@@ -68,14 +68,15 @@
 
     return config
 
 
 def _load_config(parsed_args: Namespace, app: str) -> Dict:
     """Load the config from command line options or from config file."""
     config_file = parsed_args.config
+
     with open(config_file, "r", encoding="utf8") as file:
         toml = tomlkit.load(file)
 
         if len(toml) == 0:
             raise ConfigFileCorruptedError(
                 f"Corrupted config file: {config_file}"
             )
```

### Comparing `xsget-0.1.8/xsget/chapter.py` & `xsget-0.1.9/xsget/chapter.py`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/xsget/xsget.py` & `xsget-0.1.9/xsget/xsget.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     # Log as error instead of raising exception as we want to continue with
     # other downloads.
     except aiohttp.ClientResponseError as error:
         _logger.error("error: %s", error)
 
     except aiohttp.client_exceptions.InvalidURL as error:
-        raise Exception(f"invalid url: {error}") from error
+        raise RuntimeError(f"invalid url: {error}") from error
 
 
 async def fetch_url_by_browser(
     session: Any, url: str, config: argparse.Namespace
 ) -> None:
     """Fetch and save a single URL asynchronously.
 
@@ -162,15 +162,15 @@
 
     # Log as error instead of raising exception as we want to continue with
     # other downloads.
     except aiohttp.ClientResponseError as error:
         _logger.error(error)
 
     except aiohttp.client_exceptions.InvalidURL as error:
-        raise Exception(f"invalid url: {error}") from error
+        raise RuntimeError(f"invalid url: {error}") from error
 
 
 async def fetch_urls(burls: List, config: argparse.Namespace) -> None:
     """Batch fetch and save multiple URLS asynchronously.
 
     Args:
         burls (list): A list of URL to be fetched
@@ -409,15 +409,17 @@
     match = re.search(range_re, config.url)
     if match:
         urls = []
         start = int(match.group(1))
         end = int(match.group(2))
 
         if start > end:
-            raise Exception(f"invalid url range, start: {start}, end: {end}")
+            raise RuntimeError(
+                f"invalid url range, start: {start}, end: {end}"
+            )
 
         for sequence in range(start, end + 1):
             url = config.url.replace(match.group(0), str(sequence))
             urls.append(url)
         burls = [urls]
     else:
         filename = url_to_filename(config.url, config.url_param_as_filename)
@@ -436,15 +438,15 @@
         for urls in burls:
             for url in urls:
                 _logger.info("Found url: %s", url)
     else:
         asyncio.run(fetch_urls(burls, config), debug=config.debug)
 
 
-def main(args: Sequence[str]) -> None:
+def main(args: Optional[Sequence[str]] = None) -> None:
     """Run the main program flow."""
     config = argparse.Namespace(debug=True)
     try:
         parser = build_parser(args)
         parsed_args = parser.parse_args(args)
 
         setup_logging(parsed_args.debug)
```

### Comparing `xsget-0.1.8/xsget/xsget.toml` & `xsget-0.1.9/xsget/xsget.toml`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/xsget/xstxt.py` & `xsget-0.1.9/xsget/xstxt.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,23 +27,26 @@
 from pathlib import Path
 from typing import Callable, List, Optional, Sequence
 
 import aiofiles
 import regex as re
 from bs4 import BeautifulSoup, UnicodeDammit
 from natsort import natsorted
+from watchdog.events import FileSystemEventHandler
+from watchdog.observers import Observer
 
 from xsget import __version__, load_or_create_config, setup_logging
 from xsget.book import Book
 from xsget.chapter import Chapter
 
 __usages__ = """
 examples:
   xstxt --input *.html
   xstxt --output-individual-file --input *.html
+  xstxt --config --monitor
 
 """
 
 # Unicode integer in hexadecimal for these characters.
 FULLWIDTH_EXCLAMATION_MARK = 0xFF01
 EXCLAMATION_MARK = 0x21
 TILDE = 0x7E
@@ -53,17 +56,33 @@
 #
 # See Halfwidth and Fullwidth Forms in Unicode (https://w.wiki/66Ps) and
 # Unicode block (https://w.wiki/66Pt).
 HALFWIDTH_FULLWIDTH_MAP = {}
 for hwi, fwi in enumerate(range(EXCLAMATION_MARK, TILDE + 1)):
     HALFWIDTH_FULLWIDTH_MAP[fwi] = FULLWIDTH_EXCLAMATION_MARK + hwi
 
+DEFAULT_CONFIG_FILE = "xstxt.toml"
+
 _logger = logging.getLogger(__name__)
 
 
+class MyHandler(FileSystemEventHandler):
+    """Custom event handler for monitoring changes in config file."""
+
+    def __init__(self, config):
+        """Constructor."""
+        self.config = config
+
+    def on_modified(self, event):
+        """Re-generate the book when config file updated."""
+        if event.src_path.endswith(DEFAULT_CONFIG_FILE):
+            config = _load_config(["-c", self.config.config])
+            asyncio.run(gen_book(config), debug=config.debug)
+
+
 def get_html_files(
     inputs: List[str], limit: int, excludes: List[str]
 ) -> List[str]:
     """Get the list of HTML files or file for cleansing and extracting.
 
     Args:
         inputs (List[str]): Glob-like pattern for selecting HTML files
@@ -500,34 +519,43 @@
     group = parser.add_mutually_exclusive_group()
 
     group.add_argument(
         "-g",
         "--generate-config-file",
         nargs="?",
         default=False,
-        const="xstxt.toml",
+        const=DEFAULT_CONFIG_FILE,
         dest="gen_config",
         help="generate config file from options (default: '%(const)s')",
         type=str,
         metavar="FILENAME",
     )
 
     group.add_argument(
         "-c",
         "--config-file",
         nargs="?",
         default=False,
-        const="xstxt.toml",
+        const=DEFAULT_CONFIG_FILE,
         dest="config",
         help="load config from file (default: '%(const)s')",
         type=str,
         metavar="FILENAME",
     )
 
     parser.add_argument(
+        "-m",
+        "--monitor",
+        default=False,
+        action="store_true",
+        dest="monitor",
+        help="monitor config file changes and re-run when needed",
+    )
+
+    parser.add_argument(
         "-d",
         "--debug",
         default=False,
         action="store_true",
         dest="debug",
         help="show debugging log and stacktrace",
     )
@@ -544,31 +572,48 @@
     return parser
 
 
 def main(args: Optional[Sequence[str]] = None) -> None:
     """Run the main program flow."""
     config = argparse.Namespace(debug=True)
     try:
-        parser = build_parser()
-        parsed_args = parser.parse_args(args)
-
-        setup_logging(parsed_args.debug)
-
-        config_from_file = load_or_create_config(parsed_args, "xstxt")
-        parser.set_defaults(**config_from_file)
-        config = parser.parse_args()
-
+        config = _load_config(args)
+        _logger.debug(config)
         asyncio.run(gen_book(config), debug=config.debug)
+        if config.monitor:
+            _logger.info("Running in monitor mode")
+            event_handler = MyHandler(config)
+            observer = Observer()
+            observer.schedule(event_handler, path=".")
+            observer.start()
+
+            while observer.is_alive():
+                observer.join(1)
     except Exception as error:
         _logger.error(
             "error: %s",
             getattr(error, "message", str(error)),
             exc_info=getattr(config, "debug", True),
         )
         raise SystemExit(1) from None
+    finally:
+        observer.stop()
+        observer.join()
+
+
+def _load_config(args: Optional[Sequence[str]] = None) -> argparse.Namespace:
+    parser = build_parser()
+    parsed_args = parser.parse_args(args)
+
+    setup_logging(parsed_args.debug)
+
+    config_from_file = load_or_create_config(parsed_args, "xstxt")
+    parser.set_defaults(**config_from_file)
+    config = parser.parse_args()
+    return config
 
 
 def _load_translation(config: argparse.Namespace) -> Callable:
     localedir = Path(Path(__file__).parent.parent, "locales")
     translation = gettext.translation(
         "xstxt", localedir=localedir, languages=[config.language]
     )
```

### Comparing `xsget-0.1.8/xsget/xstxt.toml` & `xsget-0.1.9/xsget/xstxt.toml`

 * *Files identical despite different names*

### Comparing `xsget-0.1.8/PKG-INFO` & `xsget-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,86 @@
 Metadata-Version: 2.1
 Name: xsget
-Version: 0.1.8
+Version: 0.1.9
 Summary: Console tools to download online novel and convert to text file.
 Author-email: "Kian-Meng, Ang" <kianmeng@cpan.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python
+Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Text Processing
 Requires-Dist: aiofiles
 Requires-Dist: aiohttp
 Requires-Dist: bs4
+Requires-Dist: cssselect
 Requires-Dist: lxml
 Requires-Dist: natsort
 Requires-Dist: playwright
 Requires-Dist: regex
 Requires-Dist: tomlkit
 Requires-Dist: user_agent
-Requires-Dist: cssselect
+Requires-Dist: watchdog
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
+Requires-Dist: line-profiler ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: tox<4 ; extra == "dev"
 Requires-Dist: tox-pyenv ; extra == "dev"
-Requires-Dist: line-profiler ; extra == "dev"
+Requires-Dist: tox<4 ; extra == "dev"
 Requires-Dist: myst_parser ; extra == "doc"
 Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints ; extra == "doc"
 Requires-Dist: sphinx_autobuild ; extra == "doc"
 Requires-Dist: sphinx_copybutton ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints ; extra == "doc"
 Requires-Dist: aioresponses ; extra == "test"
 Requires-Dist: playwright ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-console-scripts ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: pytest-playwright ; extra == "test"
+Requires-Dist: pytest-randomly ; extra == "test"
+Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: types-aiofiles ; extra == "test"
 Project-URL: Issues, https://github.com/kianmeng/xsget/issues
 Project-URL: Source, https://github.com/kianmeng/xsget
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 
 # xsget
 
 Console tools to download online novel and convert to text file.
 
 ## Installation
 
-Stable version From PyPI:
+Stable version From PyPI using `pipx`:
+
+```console
+pipx install xsget playwright
+playwright install
+```
+
+Stable version From PyPI using `pip`:
 
 ```console
-python3 -m pip install xsget
+python3 -m pip install xsget playwright
 playwright install
 ```
 
 Latest development version from GitHub:
 
 ```console
 python3 -m pip install -e git+https://github.com/kianmeng/xsget.git
@@ -103,41 +117,42 @@
   -r, --refresh
         refresh the index page
   -t, --test
         show extracted urls without crawling
   -b, --browser
         crawl by actual browser (default: 'False')
   -bs SESSION, --browser-session SESSION
-        set the number of browser session (default: 5)
+        set the number of browser session (default: 2)
   -bd DELAY, --browser-delay DELAY
         set the second to wait for page to load in browser (default: 0)
   -d, --debug
         show debugging log and stacktrace
   -h, --help
         show this help message and exit
   -V, --version
         show program's version number and exit
 
 examples:
   xsget http://localhost
   xsget http://localhost/page[1-100].html
+  xsget -g -l "a" -p "id" http://localhost
 ```
 
 ## xstxt
 
 ```console
 xstxt -h
 ```
 
 ```console
 usage: xstxt [-pt CSS_PATH] [-pb CSS_PATH] [-la LANGUAGE] [-ps SEPARATOR]
              [-rh REGEX REGEX] [-rt REGEX REGEX] [-bt TITLE] [-ba AUTHOR]
              [-ic INDENT_CHARS] [-fw] [-oi] [-i GLOB_PATTERN]
              [-e GLOB_PATTERN] [-l TOTAL_FILES] [-w WIDTH] [-o FILENAME]
-             [-g [FILENAME] | -c [FILENAME]] [-wf] [-d] [-h] [-V]
+             [-g [FILENAME] | -c [FILENAME]] [-m] [-d] [-h] [-V]
 
 xstxt is a cli app that extract content from HTML to text file.
   website: https://github.com/kianmeng/xsget
   issues: https://github.com/kianmeng/xsget/issues
 
 optional arguments:
   -pt CSS_PATH, --title-css-path CSS_PATH
@@ -172,26 +187,26 @@
         set the line width for wrapping (default: 0, 0 to disable)
   -o FILENAME, --output FILENAME
         set output txt file name (default: 'book.txt')
   -g [FILENAME], --generate-config-file [FILENAME]
         generate config file from options (default: 'xstxt.toml')
   -c [FILENAME], --config-file [FILENAME]
         load config from file (default: 'xstxt.toml')
-  -wf, --watch-files
-        enable watch on file changes
+  -m, --monitor
+        monitor config file changes and re-run when needed
   -d, --debug
         show debugging log and stacktrace
   -h, --help
         show this help message and exit
   -V, --version
         show program's version number and exit
 
 examples:
-  xstxt -i *.html
-  xstxt -oi -i *.html
+  xstxt --input *.html
+  xstxt --output-individual-file --input *.html
 ```
 
 ## Copyright and License
 
 Copyright (C) 2021,2022,2023 Kian-Meng Ang
 
 This program is free software: you can redistribute it and/or modify it under
```

