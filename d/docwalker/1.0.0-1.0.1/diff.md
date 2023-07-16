# Comparing `tmp/docwalker-1.0.0.tar.gz` & `tmp/docwalker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docwalker-1.0.0.tar", last modified: Sat Jul 15 21:30:16 2023, max compression
+gzip compressed data, was "docwalker-1.0.1.tar", max compression
```

## Comparing `docwalker-1.0.0.tar` & `docwalker-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 21:30:16.321630 docwalker-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-07-14 00:40:47.000000 docwalker-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       30 2023-07-15 21:05:12.000000 docwalker-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2280 2023-07-15 21:30:16.320630 docwalker-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-07-15 21:08:49.000000 docwalker-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 21:30:16.305624 docwalker-1.0.0/docwalker/
--rw-rw-rw-   0        0        0        0 2023-07-14 01:02:51.000000 docwalker-1.0.0/docwalker/__init__.py
--rw-rw-rw-   0        0        0      328 2023-07-15 21:06:52.000000 docwalker-1.0.0/docwalker/__main__.py
--rw-rw-rw-   0        0        0     2549 2023-07-15 21:08:59.000000 docwalker-1.0.0/docwalker/app.py
--rw-rw-rw-   0        0        0     2029 2023-07-15 21:09:11.000000 docwalker-1.0.0/docwalker/cli.py
--rw-rw-rw-   0        0        0     2236 2023-07-15 04:42:56.000000 docwalker-1.0.0/docwalker/parser.py
-drwxrwxrwx   0        0        0        0 2023-07-15 21:30:16.319629 docwalker-1.0.0/docwalker/styles/
--rw-rw-rw-   0        0        0      200 2023-07-15 20:29:50.000000 docwalker-1.0.0/docwalker/styles/main.css
-drwxrwxrwx   0        0        0        0 2023-07-15 21:30:16.318629 docwalker-1.0.0/docwalker.egg-info/
--rw-rw-rw-   0        0        0     2280 2023-07-15 21:30:16.000000 docwalker-1.0.0/docwalker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-07-15 21:30:16.000000 docwalker-1.0.0/docwalker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 21:30:16.000000 docwalker-1.0.0/docwalker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-15 21:30:16.000000 docwalker-1.0.0/docwalker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-15 21:30:16.000000 docwalker-1.0.0/docwalker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 21:30:16.000000 docwalker-1.0.0/docwalker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1215 2023-07-15 21:28:53.000000 docwalker-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 21:30:16.321630 docwalker-1.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-14 01:02:51.187406 docwalker-1.0.1/docwalker/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-15 21:06:52.667191 docwalker-1.0.1/docwalker/__main__.py
+-rw-r--r--   0        0        0     2549 2023-07-15 21:08:59.854343 docwalker-1.0.1/docwalker/app.py
+-rw-r--r--   0        0        0     2029 2023-07-16 05:47:04.424839 docwalker-1.0.1/docwalker/cli.py
+-rw-r--r--   0        0        0     2236 2023-07-15 04:42:56.411048 docwalker-1.0.1/docwalker/parser.py
+-rw-r--r--   0        0        0      200 2023-07-15 20:29:50.785817 docwalker-1.0.1/docwalker/styles/main.css
+-rw-r--r--   0        0        0     1091 2023-07-14 00:40:47.748612 docwalker-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1226 2023-07-16 05:20:39.834783 docwalker-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1673 2023-07-16 05:45:17.255285 docwalker-1.0.1/README.md
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 docwalker-1.0.1/PKG-INFO
```

### Comparing `docwalker-1.0.0/LICENSE` & `docwalker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docwalker-1.0.0/docwalker/app.py` & `docwalker-1.0.1/docwalker/app.py`

 * *Files identical despite different names*

### Comparing `docwalker-1.0.0/docwalker/cli.py` & `docwalker-1.0.1/docwalker/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 By default, DocWalker creates a local config file, .dwconf, which hosts the
 project-specific configuration.
 """
 
 _default_inline_syntax = "#@"
 _default_block_syntax_start = "/*@"
 _default_block_syntax_end = "@*/"
-_default_listing_syntax_start = "<<<"
-_default_listing_syntax_end = ">>>"
+_default_listing_syntax_start = "#<<"
+_default_listing_syntax_end = "#>>"
 
 _default_config = f"""
 [parser.inline]
 syntax = {_default_inline_syntax}
 
 [parser.block]
 syntax_start = {_default_block_syntax_start}
```

### Comparing `docwalker-1.0.0/docwalker/parser.py` & `docwalker-1.0.1/docwalker/parser.py`

 * *Files identical despite different names*

### Comparing `docwalker-1.0.0/pyproject.toml` & `docwalker-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-[project]
+[tool.poetry]
 name = "docwalker"
-version = "1.0.0"
-description = "Quickly view documentation in source code in a language-agnostic way." 
+version = "1.0.1"
+description = "Quickly view documentation in source code in a language-agnostic way."
+authors = ["Conner Marzen <connermarzen@gmail.com>"]
+license = "MIT"
 readme = "README.md"
-requires-python = ">=3.7"
-license = {file = "LICENSE"}
 keywords = ["tui", "documentation", "viewer"]
-authors = [{name = "Conner Marzen", email = "connermarzen@gmail.com" }]
 classifiers = [
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -19,21 +18,25 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
-dependencies = ["textual"]
-
-[project.optional-dependencies]
-dev = ["textual-dev"]
+packages = [
+    { include = "docwalker" },
+    { include = "docwalker/styles/*.css" },
+]
 
-[project.scripts]
+[tool.poetry.scripts]
 docwalker = "docwalker.__main__:main"
 
-[tool.setuptools.package-data]
-docwalker = ["docwalker/styles/*.css"]
+[tool.poetry.dependencies]
+python = "^3.7"
+textual = "^0.29.0"
+
+[tool.poetry.group.dev.dependencies]
+textual-dev = "^1.0.1"
 
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

