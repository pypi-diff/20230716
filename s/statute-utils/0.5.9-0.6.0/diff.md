# Comparing `tmp/statute_utils-0.5.9.tar.gz` & `tmp/statute_utils-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.5.9.tar", max compression
+gzip compressed data, was "statute_utils-0.6.0.tar", max compression
```

## Comparing `statute_utils-0.5.9.tar` & `statute_utils-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.9/LICENSE
--rw-r--r--   0        0        0     3593 2023-07-14 16:18:39.431381 statute_utils-0.5.9/README.md
--rw-r--r--   0        0        0     1314 2023-07-14 18:33:12.450876 statute_utils-0.5.9/pyproject.toml
--rw-r--r--   0        0        0      678 2023-07-14 16:17:42.904400 statute_utils-0.5.9/statute_utils/__init__.py
--rw-r--r--   0        0        0      460 2023-07-14 10:30:59.403468 statute_utils-0.5.9/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-14 14:09:59.832215 statute_utils-0.5.9/statute_utils/components/builder.py
--rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.5.9/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.9/statute_utils/components/short.py
--rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.9/statute_utils/components/utils.py
--rw-r--r--   0        0        0     3963 2023-07-14 16:17:14.380273 statute_utils-0.5.9/statute_utils/display.py
--rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.9/statute_utils/main.py
--rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.9/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.9/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.9/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.9/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.9/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.9/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.9/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.9/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0       85 2023-07-14 18:33:02.453752 statute_utils-0.5.9/statute_utils/templates/branch.html
--rw-r--r--   0        0        0     1114 2023-07-14 18:24:17.829710 statute_utils-0.5.9/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     2224 2023-07-14 18:27:08.881995 statute_utils-0.5.9/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     6519 2023-07-14 12:30:11.704539 statute_utils-0.5.9/statute_utils/tree.py
--rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 statute_utils-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2640 2023-07-16 05:44:56.640061 statute_utils-0.6.0/README.md
+-rw-r--r--   0        0        0     1357 2023-07-16 05:42:45.235534 statute_utils-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      817 2023-07-16 07:43:47.611153 statute_utils-0.6.0/statute_utils/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.0/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     5976 2023-07-16 05:09:00.421516 statute_utils-0.6.0/statute_utils/components/branch.py
+-rw-r--r--   0        0        0     8323 2023-07-16 08:01:53.752165 statute_utils-0.6.0/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.6.0/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.0/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.0/statute_utils/components/utils.py
+-rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.6.0/statute_utils/main.py
+-rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.6.0/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.0/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.0/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.0/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.0/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.0/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.0/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.0/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6537 2023-07-16 06:04:54.216686 statute_utils-0.6.0/statute_utils/statute.py
+-rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.0/statute_utils/templater.py
+-rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.0/statute_utils/templates/crumbs.html
+-rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.0/statute_utils/templates/paragraph.html
+-rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.0/statute_utils/templates/subtree.html
+-rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.0/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     2416 2023-07-16 08:50:40.061466 statute_utils-0.6.0/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 statute_utils-0.6.0/PKG-INFO
```

### Comparing `statute_utils-0.5.9/LICENSE` & `statute_utils-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/README.md` & `statute_utils-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: statute-utils
+Version: 0.6.0
+Summary: Philippine statutory law pattern matching and unit retrieval.
+Home-page: https://lawsql.com
+Author: Marcelino G. Veloso III
+Author-email: contact@mv3.dev
+Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Legal Industry
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
+Requires-Dist: markdown (>=3.4.3,<4.0.0)
+Requires-Dist: python-slugify (>=8.0,<9.0)
+Requires-Dist: sqlite-utils (>=3.33,<4.0)
+Project-URL: Documentation, https://justmars.github.io/statute-utils
+Project-URL: Repository, https://github.com/justmars/statute-utils
+Description-Content-Type: text/markdown
+
 # statute-utils
 
 ![Github CI](https://github.com/justmars/statute-utils/actions/workflows/main.yml/badge.svg)
 
 Philippine statutory law pattern matching and unit retrieval; utilized in [LawSQL dataset](https://lawsql.com).
 
 ## Documentation
@@ -53,20 +77,14 @@
 >>> db = Database('db.sqlite')
 >>> db["statutes"].insert(Statute.from_file(f).make_row())
 # this will contain an 'html' column containing a semantic tree structure that can be styled via css
 ```
 
 ### Copy html/css files
 
-are found in `statute_utils/templates/statute.html`.
-
-The present module has a directory for `statute_utils/templates/`:
-
-It contains:
-
 1. `tree.html` - Tree-building macros (which can be used for creating an html tree to represent the statute)
 2. `tree.css` - Sample css rulesets to use for the tree generated with the macros
 
 Copy files to the Jinja environment where these can be reused:
 
 ```text
 - /app
@@ -110,29 +128,9 @@
 
 When datasette is served with:
 
 ```jinja
 datasette serve db.sqlite --plugins-dir=app/plugins/ {# plus the other arguments #}...
 ```
 
-It becomes possible to use custom functions and filters found in `tree.py` likeso:
+It becomes possible to use custom functions and filters found in `tree.py`.
 
-```py title="datasette/plugins/tree.py"
-from datasette import hookimpl
-from statute_utils.display import from_json, is_hidden, is_excluded, from_mp, try_short, set_mp_slug, is_par, md_to_html, build_branch, crumb, tree_helpers
-
-@hookimpl
-def prepare_jinja2_environment(env): # custom filters can be used in datasette pages
-  env.filters["from_json"] = from_json
-  env.filters["is_hidden"] = is_hidden
-  env.filters["is_excluded"] = is_excluded
-  env.filters["from_mp"] = from_mp
-  env.filters["try_short"] = try_short
-  env.filters["set_mp_slug"] = set_mp_slug
-  env.filters["is_par"] = is_par
-  env.filters["md_to_html"] = md_to_html
-  env.filters["crumb"] = crumb
-
-@hookimpl
-def prepare_connection(conn): # custom function can be used in sqlite
-    conn.create_function("build_branch", 1, build_branch)
-```
```

### Comparing `statute_utils-0.5.9/pyproject.toml` & `statute_utils-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.5.9"
+version = "0.6.0"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
@@ -17,14 +17,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-slugify = "^8.0"
 sqlite-utils = "^3.33"
 markdown = "^3.4.3"
 jinja2 = "^3.1.2"
+beautifulsoup4 = "^4.12.2"
+lxml = "^4.9.3"
 
 [tool.poetry.group.dev.dependencies]
 python-frontmatter = "^1.0.0" # for testing local decisions
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
 types-python-slugify = "^5.0"
```

### Comparing `statute_utils-0.5.9/statute_utils/__init__.py` & `statute_utils-0.6.0/statute_utils/components/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from .components import (
-    StatuteSerialCategory,
-    StatuteTitle,
-    StatuteTitleCategory,
-    add_blg,
-    add_num,
-    create_fts_snippet_column,
-    create_unit_heading,
+from .branch import make_branch, make_branch_json_array, set_node_ids, walk
+from .builder import (
+    TREE_FILTERS,
+    crumb,
     from_json,
     from_mp,
     is_excluded,
+    is_first_par,
     is_hidden,
     is_par,
-    ltr,
+    md_to_html,
+    paragrapher,
     set_mp_slug,
     try_short,
 )
-from .display import build_branch, make_statute_string, tree_helpers
-from .main import (
-    CountedStatute,
-    extract_named_rules,
-    extract_rule,
-    extract_rules,
-    extract_serial_rules,
+from .category import StatuteSerialCategory, StatuteTitle, StatuteTitleCategory
+from .utils import (
+    NON_ACT_INDICATORS,
+    add_blg,
+    add_num,
+    create_fts_snippet_column,
+    create_unit_heading,
+    get_regexes,
+    limited_acts,
+    ltr,
+    make_regex_readable,
+    not_prefixed_by_any,
 )
-from .models import Rule, create_db
-from .models_names import STYLES_NAMED, NamedPattern
-from .models_serials import STYLES_SERIAL, SerialPattern
-from .tree import STATUTE_DIR, Statute
```

### Comparing `statute_utils-0.5.9/statute_utils/components/category.py` & `statute_utils-0.6.0/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/components/short.py` & `statute_utils-0.6.0/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/main.py` & `statute_utils-0.6.0/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/models.py` & `statute_utils-0.6.0/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/models_names.py` & `statute_utils-0.6.0/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/models_serials.py` & `statute_utils-0.6.0/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/recipes/digits.py` & `statute_utils-0.6.0/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/recipes/spain.py` & `statute_utils-0.6.0/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.9/statute_utils/templates/tree.css` & `statute_utils-0.6.0/statute_utils/templates/tree.css`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-article > header > hgroup > h3.crumbs {
+span.crumbs {
   display: flex;
   flex-direction: row-reverse;
   flex-wrap: wrap-reverse;
   justify-content: start;
 
   & span:not(:last-child):before {
     content: ", "
   }
 }
 
 section.tree {
   & ul {
-    padding-left: 0px; /* No indent */
+    padding-left: 0px; /* No top-level indention */
 
     @media (min-width: 640px) {
       & li {
-        padding-left: 0.7rem; /* Indent since > small screens */
+        padding-left: 0.7rem; /* Indention if > small screens */
       }
 
       & li[data-par="true"] {
-        padding-left: 0px; /* No indent even if > small screens */
+        padding-left: 0px; /* No indention for data-par even if > small screens */
       }
     }
   }
 
   & li {
     list-style-type: none;
     margin-bottom: 0.25em;
```

### Comparing `statute_utils-0.5.9/statute_utils/tree.py` & `statute_utils-0.6.0/statute_utils/statute.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     StatuteSerialCategory,
     StatuteTitle,
     create_fts_snippet_column,
     create_unit_heading,
     set_node_ids,
     walk,
 )
-from .display import create_html_tree
 from .models import STATUTE_DIR, Rule
+from .templater import html_tree_from_hierarchy
 
 
 class Statute(NamedTuple):
     """A instance is dependent on a statute path from a fixed
     `STATUTE_DIR`. The shape of the Python object will be different
     from the shape of the dumpable `.yml` export."""
 
@@ -73,15 +73,15 @@
         return {
             "id": self.slug,
             "cat": self.rule.cat.value,
             "num": self.rule.num,
             "date": self.date,
             "variant": self.variant,
             "units": units,
-            "html": create_html_tree(units),
+            "html": html_tree_from_hierarchy(units),
         }
 
     @classmethod
     def flatten_units(
         cls, statute_id: str, units: list[dict[str, Any]], heading: str = ""
     ) -> Iterator[dict[str, str | None]]:
         """Recursive flattening of tree structure where each material path
```

