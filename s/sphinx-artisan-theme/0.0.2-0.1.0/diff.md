# Comparing `tmp/sphinx-artisan-theme-0.0.2.tar.gz` & `tmp/sphinx_artisan_theme-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-artisan-theme-0.0.2.tar", max compression
+gzip compressed data, was "sphinx_artisan_theme-0.1.0.tar", max compression
```

## Comparing `sphinx-artisan-theme-0.0.2.tar` & `sphinx_artisan_theme-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      830 2022-06-26 16:33:04.873005 sphinx-artisan-theme-0.0.2/README.md
--rw-r--r--   0        0        0     2306 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2705 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/__init__.py
--rw-r--r--   0        0        0       49 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/ext/__init__.py
--rw-r--r--   0        0        0     4326 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/ext/extract_toc.py
--rw-r--r--   0        0        0     1785 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/ext/remove_sections.py
--rw-r--r--   0        0        0     2888 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/_macros.html
--rw-r--r--   0        0        0     1284 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/domainindex.html
--rw-r--r--   0        0        0      437 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/footer.html
--rw-r--r--   0        0        0     1440 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/genindex.html
--rw-r--r--   0        0        0      767 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/globaltoc.html
--rw-r--r--   0        0        0     1140 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/header.html
--rw-r--r--   0        0        0     1900 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/layout.html
--rw-r--r--   0        0        0      618 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/page.html
--rw-r--r--   0        0        0     1085 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/search-field.html
--rw-r--r--   0        0        0     3017 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/search.html
--rw-r--r--   0        0        0    33691 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/static/theme.css
--rw-r--r--   0        0        0     5187 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/static/theme.src.css
--rw-r--r--   0        0        0     2434 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/tailwind.config.js
--rw-r--r--   0        0        0      114 2022-06-26 16:33:04.877005 sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/theme.conf
--rw-r--r--   0        0        0     1770 1970-01-01 00:00:00.000000 sphinx-artisan-theme-0.0.2/setup.py
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 sphinx-artisan-theme-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      830 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/README.md
+-rw-r--r--   0        0        0     2368 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2705 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/ext/__init__.py
+-rw-r--r--   0        0        0     4326 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/ext/extract_toc.py
+-rw-r--r--   0        0        0     1785 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/ext/remove_sections.py
+-rw-r--r--   0        0        0     2888 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/_macros.html
+-rw-r--r--   0        0        0     1284 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/domainindex.html
+-rw-r--r--   0        0        0      437 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/footer.html
+-rw-r--r--   0        0        0     1440 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/genindex.html
+-rw-r--r--   0        0        0      767 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/globaltoc.html
+-rw-r--r--   0        0        0     1140 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/header.html
+-rw-r--r--   0        0        0     1900 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/layout.html
+-rw-r--r--   0        0        0      618 2023-07-16 21:12:37.418919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/page.html
+-rw-r--r--   0        0        0     1085 2023-07-16 21:12:37.422919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/search-field.html
+-rw-r--r--   0        0        0     3017 2023-07-16 21:12:37.422919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/search.html
+-rw-r--r--   0        0        0    33691 2023-07-16 21:12:37.422919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/static/theme.css
+-rw-r--r--   0        0        0     5187 2023-07-16 21:12:37.422919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/static/theme.src.css
+-rw-r--r--   0        0        0     2434 2023-07-16 21:12:37.422919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/tailwind.config.js
+-rw-r--r--   0        0        0      114 2023-07-16 21:12:37.422919 sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/theme.conf
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 sphinx_artisan_theme-0.1.0/PKG-INFO
```

### Comparing `sphinx-artisan-theme-0.0.2/README.md` & `sphinx_artisan_theme-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/pyproject.toml` & `sphinx_artisan_theme-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "sphinx-artisan-theme"
-version = "0.0.2"
+version = "0.1.0"
 description = ""
 authors = ["Daniel Knell <contact@danielknell.co.uk>"]
 readme = "README.md"
 packages = [{include = "sphinx_artisan_theme", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-Sphinx = "^4.4.0"
+Sphinx = ">=4.4,<7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.1"
 sphinx-autobuild = "^2021.3.14"
-shed = "^0.9.4"
-sphinx-lint = "^0.2"
+shed = ">=0.9.4,<2023.7.0"
+sphinx-lint = ">=0.2,<0.7"
 restructuredtext-lint = "^1.4.0"
-myst-parser = "^0.17.0"
+myst-parser = ">=0.17,<1.1"
 autodocsumm = "^0.2.7"
 pylint = "^2.13.5"
-mypy = "^0.942"
-types-docutils = "^0.18.3"
+mypy = ">=0.942,<1.5"
+types-docutils = ">=0.18.3,<0.21.0"
 types-pkg-resources = "^0.1.3"
-pytest-pylint = "^0.18.0"
-pytest-mypy = "^0.9.1"
+pytest-pylint = ">=0.18,<0.20"
+pytest-mypy = ">=0.9.1,<0.11.0"
 pytest-pydocstyle = "^2.3.0"
-pytest-cov = "^3.0.0"
-typeguard = "^2.13.3"
+pytest-cov = ">=3,<5"
+typeguard = ">=2.13.3,<5.0.0"
 pyenchant = "^3.2.2"
 
 [tool.poetry.plugins."sphinx.html_themes"]
 "sphinx_artisan_theme" = "sphinx_artisan_theme"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/__init__.py` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/ext/extract_toc.py` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/ext/extract_toc.py`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/ext/remove_sections.py` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/ext/remove_sections.py`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/_macros.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/_macros.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/domainindex.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/genindex.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/globaltoc.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/globaltoc.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/header.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/header.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/layout.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/page.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/page.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/search-field.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/search-field.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/search.html` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/static/theme.css` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/static/theme.css`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/static/theme.src.css` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/static/theme.src.css`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/src/sphinx_artisan_theme/themes/artisan/tailwind.config.js` & `sphinx_artisan_theme-0.1.0/src/sphinx_artisan_theme/themes/artisan/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sphinx-artisan-theme-0.0.2/PKG-INFO` & `sphinx_artisan_theme-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: sphinx-artisan-theme
-Version: 0.0.2
+Version: 0.1.0
 Summary: 
 Author: Daniel Knell
 Author-email: contact@danielknell.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Sphinx (>=4.4.0,<5.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Sphinx (>=4.4,<7.0)
 Description-Content-Type: text/markdown
 
 # Artisan Sphinx Theme
 
 <p class="lead">
 An elegant theme designed to style the sphinx documentation for all Artisan of
 Code projects.
```

