# Comparing `tmp/symbex-1.1.tar.gz` & `tmp/symbex-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-1.1.tar", last modified: Sun Jul 16 01:13:26 2023, max compression
+gzip compressed data, was "symbex-1.2.tar", last modified: Sun Jul 16 16:55:50 2023, max compression
```

## Comparing `symbex-1.1.tar` & `symbex-1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.089621 symbex-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 01:13:12.000000 symbex-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-16 01:13:26.089621 symbex-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-07-16 01:13:12.000000 symbex-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 01:13:26.089621 symbex-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-16 01:13:12.000000 symbex-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.085621 symbex-1.1/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:12.000000 symbex-1.1/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-16 01:13:12.000000 symbex-1.1/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-07-16 01:13:12.000000 symbex-1.1/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-16 01:13:12.000000 symbex-1.1/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.085621 symbex-1.1/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.085621 symbex-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.441049 symbex-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 16:55:34.000000 symbex-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-16 16:55:50.441049 symbex-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-16 16:55:34.000000 symbex-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:55:50.441049 symbex-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-16 16:55:34.000000 symbex-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.437049 symbex-1.2/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:34.000000 symbex-1.2/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-16 16:55:34.000000 symbex-1.2/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-16 16:55:34.000000 symbex-1.2/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-16 16:55:34.000000 symbex-1.2/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.441049 symbex-1.2/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.441049 symbex-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_symbols.py
```

### Comparing `symbex-1.1/LICENSE` & `symbex-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-1.1/PKG-INFO` & `symbex-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 1.1
+Version: 1.2
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -108,14 +108,15 @@
 In addition to searching for symbols, you can apply filters to the results.
 
 The following filters are available:
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
+- `--unasync` - only non-async functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 - `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
@@ -401,24 +402,15 @@
 You can use this in CI to guard against things like functions being added without documentation:
 
 ```bash
 symbex --function --undocumented --check
 ```
 This will fail silently but set a `1` exit code if there are any undocumented functions.
 
-## Using in CI
-
-The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
-
-You can use this in CI to guard against things like functions being added without documentation:
-
-```bash
-symbex --function --undocumented --check
-```
-This will fail silently but set a `1` exit code if there are any undocumented functions.
+`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols.
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -483,16 +475,17 @@
   -n, --no-file              Don't include the # File: comments in the output
   -i, --imports              Show 'from x import y' lines for imported symbols
   -m, --module TEXT          Modules to search within
   --sys-path TEXT            Calculate imports relative to these on sys.path
   --docs, --docstrings       Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
-  --async                    Filter async functions
   --function                 Filter functions
+  --async                    Filter async functions
+  --unasync                  Filter non-async functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
```

### Comparing `symbex-1.1/README.md` & `symbex-1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 In addition to searching for symbols, you can apply filters to the results.
 
 The following filters are available:
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
+- `--unasync` - only non-async functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 - `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
@@ -386,24 +387,15 @@
 You can use this in CI to guard against things like functions being added without documentation:
 
 ```bash
 symbex --function --undocumented --check
 ```
 This will fail silently but set a `1` exit code if there are any undocumented functions.
 
-## Using in CI
-
-The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
-
-You can use this in CI to guard against things like functions being added without documentation:
-
-```bash
-symbex --function --undocumented --check
-```
-This will fail silently but set a `1` exit code if there are any undocumented functions.
+`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols.
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -468,16 +460,17 @@
   -n, --no-file              Don't include the # File: comments in the output
   -i, --imports              Show 'from x import y' lines for imported symbols
   -m, --module TEXT          Modules to search within
   --sys-path TEXT            Calculate imports relative to these on sys.path
   --docs, --docstrings       Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
-  --async                    Filter async functions
   --function                 Filter functions
+  --async                    Filter async functions
+  --unasync                  Filter non-async functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
```

### Comparing `symbex-1.1/setup.py` & `symbex-1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "1.1"
+VERSION = "1.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-1.1/symbex/cli.py` & `symbex-1.2/symbex/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,29 @@
 )
 @click.option(
     "--silent",
     is_flag=True,
     help="Silently ignore Python files with parse errors",
 )
 @click.option(
+    "--function",
+    is_flag=True,
+    help="Filter functions",
+)
+@click.option(
     "async_",
     "--async",
     is_flag=True,
     help="Filter async functions",
 )
 @click.option(
-    "--function",
+    "unasync",
+    "--unasync",
     is_flag=True,
-    help="Filter functions",
+    help="Filter non-async functions",
 )
 @click.option(
     "class_",
     "--class",
     is_flag=True,
     help="Filter classes",
 )
@@ -158,16 +164,17 @@
     no_file,
     imports,
     modules,
     sys_paths,
     docs,
     count,
     silent,
-    async_,
     function,
+    async_,
+    unasync,
     class_,
     documented,
     undocumented,
     typed,
     untyped,
     partially_typed,
     fully_typed,
@@ -265,14 +272,15 @@
         signatures = True
     # Show --help if no filter options are provided:
     if not any(
         [
             symbols,
             signatures,
             async_,
+            unasync,
             function,
             class_,
             documented,
             undocumented,
             typed,
             untyped,
             partially_typed,
@@ -295,14 +303,15 @@
         no_file = True
     # Default to '*' if --signatures or filters are provided without symbols
     if (
         any(
             [
                 signatures,
                 async_,
+                unasync,
                 function,
                 class_,
                 documented,
                 undocumented,
                 typed,
                 untyped,
                 partially_typed,
@@ -329,14 +338,15 @@
                 if path.is_file():
                     yield path
 
     # If any --filters were supplied, handle them:
     if any(
         [
             async_,
+            unasync,
             function,
             class_,
             documented,
             undocumented,
             typed,
             untyped,
             partially_typed,
@@ -349,14 +359,16 @@
             # Filters must ALL match
             if async_ and not isinstance(node, ast.AsyncFunctionDef):
                 return False
             if function and not isinstance(
                 node, (ast.FunctionDef, ast.AsyncFunctionDef)
             ):
                 return False
+            if unasync and not isinstance(node, ast.FunctionDef):
+                return False
             if class_ and not isinstance(node, ast.ClassDef):
                 return False
             if documented and not ast.get_docstring(node):
                 return False
             if undocumented and ast.get_docstring(node):
                 return False
             summary = type_summary(node)
```

### Comparing `symbex-1.1/symbex/lib.py` & `symbex-1.2/symbex/lib.py`

 * *Files identical despite different names*

### Comparing `symbex-1.1/symbex.egg-info/PKG-INFO` & `symbex-1.2/symbex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 1.1
+Version: 1.2
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -108,14 +108,15 @@
 In addition to searching for symbols, you can apply filters to the results.
 
 The following filters are available:
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
+- `--unasync` - only non-async functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 - `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
@@ -401,24 +402,15 @@
 You can use this in CI to guard against things like functions being added without documentation:
 
 ```bash
 symbex --function --undocumented --check
 ```
 This will fail silently but set a `1` exit code if there are any undocumented functions.
 
-## Using in CI
-
-The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
-
-You can use this in CI to guard against things like functions being added without documentation:
-
-```bash
-symbex --function --undocumented --check
-```
-This will fail silently but set a `1` exit code if there are any undocumented functions.
+`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols.
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -483,16 +475,17 @@
   -n, --no-file              Don't include the # File: comments in the output
   -i, --imports              Show 'from x import y' lines for imported symbols
   -m, --module TEXT          Modules to search within
   --sys-path TEXT            Calculate imports relative to these on sys.path
   --docs, --docstrings       Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
-  --async                    Filter async functions
   --function                 Filter functions
+  --async                    Filter async functions
+  --unasync                  Filter non-async functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
```

### Comparing `symbex-1.1/tests/test_filters.py` & `symbex-1.2/tests/test_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,35 @@
         (
             ["--async"],
             [
                 "async def async_func",
                 "async def async_func_fully_typed",
             ],
         ),
+        (
+            ["--unasync"],
+            [
+                "def func_no_args",
+                "def func_positional_args",
+                "def func_default_args",
+                "def func_arbitrary_positional_args",
+                "def func_arbitrary_keyword_args",
+                "def func_arbitrary_args",
+                "def func_positional_only_args",
+                "def func_keyword_only_args",
+                "def func_type_annotations",
+                "def function_with_non_pep_0484_annotation",
+                "def complex_annotations",
+                "def func_fully_typed",
+                "def func_partially_typed",
+                "def func_partially_typed_no_typed_return",
+                "def func_partially_typed_only_typed_return",
+                "def func_typed_no_params",
+            ],
+        ),
         # This doesn't make sense, so should return []
         (
             ["--async", "--class"],
             [],
         ),
         # Various typing options
         (
```

### Comparing `symbex-1.1/tests/test_imports.py` & `symbex-1.2/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `symbex-1.1/tests/test_replace.py` & `symbex-1.2/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `symbex-1.1/tests/test_symbex.py` & `symbex-1.2/tests/test_symbex.py`

 * *Files identical despite different names*

### Comparing `symbex-1.1/tests/test_symbols.py` & `symbex-1.2/tests/test_symbols.py`

 * *Files identical despite different names*

