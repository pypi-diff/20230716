# Comparing `tmp/symbex-1.0.tar.gz` & `tmp/symbex-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-1.0.tar", last modified: Thu Jun 29 18:31:56 2023, max compression
+gzip compressed data, was "symbex-1.1.tar", last modified: Sun Jul 16 01:13:26 2023, max compression
```

## Comparing `symbex-1.0.tar` & `symbex-1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.649236 symbex-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 18:31:42.000000 symbex-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-29 18:31:56.649236 symbex-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-06-29 18:31:42.000000 symbex-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:31:56.649236 symbex-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-29 18:31:42.000000 symbex-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.645236 symbex-1.0/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:42.000000 symbex-1.0/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 18:31:42.000000 symbex-1.0/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-06-29 18:31:42.000000 symbex-1.0/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-29 18:31:42.000000 symbex-1.0/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.645236 symbex-1.0/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.645236 symbex-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.089621 symbex-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 01:13:12.000000 symbex-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-16 01:13:26.089621 symbex-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-07-16 01:13:12.000000 symbex-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 01:13:26.089621 symbex-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-16 01:13:12.000000 symbex-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.085621 symbex-1.1/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:12.000000 symbex-1.1/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-16 01:13:12.000000 symbex-1.1/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-07-16 01:13:12.000000 symbex-1.1/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-16 01:13:12.000000 symbex-1.1/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.085621 symbex-1.1/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 01:13:26.000000 symbex-1.1/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:13:26.085621 symbex-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-16 01:13:12.000000 symbex-1.1/tests/test_symbols.py
```

### Comparing `symbex-1.0/LICENSE` & `symbex-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-1.0/PKG-INFO` & `symbex-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 1.0
+Version: 1.1
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -184,48 +184,48 @@
 runner = CliRunner()
 result = runner.invoke(cli, ["-s", "-f", str(path / "lib.py")])
 cog.out(
     "```python\n{}\n```\n".format(sorted_chunks(result.output))
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 106
+# File: symbex/lib.py Line: 107
 def function_definition(function_node: AST)
 
 # File: symbex/lib.py Line: 13
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 174
+# File: symbex/lib.py Line: 175
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 208
+# File: symbex/lib.py Line: 209
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 226
+# File: symbex/lib.py Line: 227
 def read_file(path)
 
-# File: symbex/lib.py Line: 252
+# File: symbex/lib.py Line: 253
 class TypeSummary
 
-# File: symbex/lib.py Line: 257
+# File: symbex/lib.py Line: 258
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 303
+# File: symbex/lib.py Line: 304
 def quoted_string(s)
 
-# File: symbex/lib.py Line: 314
+# File: symbex/lib.py Line: 315
 def import_line_for_function(function_name: str, filepath: str, possible_root_dirs: List[str]) -> str
 
 # File: symbex/lib.py Line: 37
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
 # File: symbex/lib.py Line: 71
 def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
 
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
 To include estimated import paths, such as `# from symbex.lib import match`, use `--imports`. These will be calculated relative to the directory you specified, or you can pass one or more `--sys-path` options to request that imports are calculated relative to those directories as if they were on `sys.path`:
 
@@ -238,15 +238,15 @@
     "--imports", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
 ])
 cog.out(
     "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 # from symbex.lib import match
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 To suppress the `# File: ...` comments, use `--no-file` or `-n`.
 
 So to both show import paths and suppress File comments, use `-in` as a shortcut:
@@ -276,15 +276,15 @@
 <!-- [[[cog
 result = runner.invoke(cli, ["match", "--docstrings", "-f", str(path / "lib.py")])
 cog.out(
     "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 def match(name: str, symbols: Iterable[str]) -> bool
     "Returns True if name matches any of the symbols, resolving wildcards"
 ```
 <!-- [[[end]]] -->
 
 ## Counting symbols
 
@@ -331,37 +331,94 @@
 ```bash
 echo "def second_function(a, b):
     # This is a replacement implementation
     return a + b + 3
 " | symbex second_function --replace
 ```
 The result will be an updated-in-place `my_code.py` containing the following:
+
 ```python
 def first_function():
     # This will be ignored
     pass
 
 def second_function(a, b):
     # This is a replacement implementation
     return a + b + 3
 ```
 This feature should be used with care! I recommend only using this feature against code that is already checked into Git, so you can review changes it makes using `git diff` and revert them using `git checkout my_code.py`.
 
-You can use this with `llm` like so:
+## Replacing a matched symbol by running a command
+
+The `--rexec COMMAND` option can be used to replace a single matched symbol by running a command and using its output.
+
+The command will be run with the matched symbol's definition piped to its standard input. The output of that command will be used as the replacement text.
+
+Here's an example that uses `sed` to add a `# ` to the beginning of each matching line, effectively commenting out the matched function:
 
 ```bash
-symbex second_function -n \
-  | llm --system 'add type hints, remove docstring' \
-  | symbex second_function --replace
+symbex first_function --rexec "sed 's/^/# /'"
 ```
-When I ran this the result was a `second_function` definition like this:
+This modified the first function in place to look like this:
+```python
+# def first_function():
+#    # This will be ignored
+#    pass
+```
+A much more exciting example uses LLM. This example will use the `gpt-3.5-turbo` model to add type hints and generate a docstring:
+
+```bash
+symbex second_function \
+  --rexec "llm --system 'add type hints and a docstring'"
+```
+I ran this against this code:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function(a, b):
+    return a + b + 3
+```
+And the second function was updated in place to look like this:
 ```python
 def second_function(a: int, b: int) -> int:
+    """
+    Returns the sum of two integers (a and b) plus 3.
+
+    Parameters:
+    a (int): The first integer.
+    b (int): The second integer.
+
+    Returns:
+    int: The sum of a and b plus 3.
+    """
     return a + b + 3
 ```
+## Using in CI
+
+The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
+
+You can use this in CI to guard against things like functions being added without documentation:
+
+```bash
+symbex --function --undocumented --check
+```
+This will fail silently but set a `1` exit code if there are any undocumented functions.
+
+## Using in CI
+
+The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
+
+You can use this in CI to guard against things like functions being added without documentation:
+
+```bash
+symbex --function --undocumented --check
+```
+This will fail silently but set a `1` exit code if there are any undocumented functions.
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -436,15 +493,17 @@
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
+  --check                    Exit with non-zero code if any matches found
   --replace                  Replace matching symbol with text from stdin
+  --rexec TEXT               Replace with the result of piping to this tool
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-1.0/README.md` & `symbex-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -169,48 +169,48 @@
 runner = CliRunner()
 result = runner.invoke(cli, ["-s", "-f", str(path / "lib.py")])
 cog.out(
     "```python\n{}\n```\n".format(sorted_chunks(result.output))
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 106
+# File: symbex/lib.py Line: 107
 def function_definition(function_node: AST)
 
 # File: symbex/lib.py Line: 13
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 174
+# File: symbex/lib.py Line: 175
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 208
+# File: symbex/lib.py Line: 209
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 226
+# File: symbex/lib.py Line: 227
 def read_file(path)
 
-# File: symbex/lib.py Line: 252
+# File: symbex/lib.py Line: 253
 class TypeSummary
 
-# File: symbex/lib.py Line: 257
+# File: symbex/lib.py Line: 258
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 303
+# File: symbex/lib.py Line: 304
 def quoted_string(s)
 
-# File: symbex/lib.py Line: 314
+# File: symbex/lib.py Line: 315
 def import_line_for_function(function_name: str, filepath: str, possible_root_dirs: List[str]) -> str
 
 # File: symbex/lib.py Line: 37
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
 # File: symbex/lib.py Line: 71
 def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
 
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
 To include estimated import paths, such as `# from symbex.lib import match`, use `--imports`. These will be calculated relative to the directory you specified, or you can pass one or more `--sys-path` options to request that imports are calculated relative to those directories as if they were on `sys.path`:
 
@@ -223,15 +223,15 @@
     "--imports", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
 ])
 cog.out(
     "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 # from symbex.lib import match
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 To suppress the `# File: ...` comments, use `--no-file` or `-n`.
 
 So to both show import paths and suppress File comments, use `-in` as a shortcut:
@@ -261,15 +261,15 @@
 <!-- [[[cog
 result = runner.invoke(cli, ["match", "--docstrings", "-f", str(path / "lib.py")])
 cog.out(
     "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 def match(name: str, symbols: Iterable[str]) -> bool
     "Returns True if name matches any of the symbols, resolving wildcards"
 ```
 <!-- [[[end]]] -->
 
 ## Counting symbols
 
@@ -316,37 +316,94 @@
 ```bash
 echo "def second_function(a, b):
     # This is a replacement implementation
     return a + b + 3
 " | symbex second_function --replace
 ```
 The result will be an updated-in-place `my_code.py` containing the following:
+
 ```python
 def first_function():
     # This will be ignored
     pass
 
 def second_function(a, b):
     # This is a replacement implementation
     return a + b + 3
 ```
 This feature should be used with care! I recommend only using this feature against code that is already checked into Git, so you can review changes it makes using `git diff` and revert them using `git checkout my_code.py`.
 
-You can use this with `llm` like so:
+## Replacing a matched symbol by running a command
+
+The `--rexec COMMAND` option can be used to replace a single matched symbol by running a command and using its output.
+
+The command will be run with the matched symbol's definition piped to its standard input. The output of that command will be used as the replacement text.
+
+Here's an example that uses `sed` to add a `# ` to the beginning of each matching line, effectively commenting out the matched function:
 
 ```bash
-symbex second_function -n \
-  | llm --system 'add type hints, remove docstring' \
-  | symbex second_function --replace
+symbex first_function --rexec "sed 's/^/# /'"
 ```
-When I ran this the result was a `second_function` definition like this:
+This modified the first function in place to look like this:
+```python
+# def first_function():
+#    # This will be ignored
+#    pass
+```
+A much more exciting example uses LLM. This example will use the `gpt-3.5-turbo` model to add type hints and generate a docstring:
+
+```bash
+symbex second_function \
+  --rexec "llm --system 'add type hints and a docstring'"
+```
+I ran this against this code:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function(a, b):
+    return a + b + 3
+```
+And the second function was updated in place to look like this:
 ```python
 def second_function(a: int, b: int) -> int:
+    """
+    Returns the sum of two integers (a and b) plus 3.
+
+    Parameters:
+    a (int): The first integer.
+    b (int): The second integer.
+
+    Returns:
+    int: The sum of a and b plus 3.
+    """
     return a + b + 3
 ```
+## Using in CI
+
+The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
+
+You can use this in CI to guard against things like functions being added without documentation:
+
+```bash
+symbex --function --undocumented --check
+```
+This will fail silently but set a `1` exit code if there are any undocumented functions.
+
+## Using in CI
+
+The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
+
+You can use this in CI to guard against things like functions being added without documentation:
+
+```bash
+symbex --function --undocumented --check
+```
+This will fail silently but set a `1` exit code if there are any undocumented functions.
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -421,15 +478,17 @@
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
+  --check                    Exit with non-zero code if any matches found
   --replace                  Replace matching symbol with text from stdin
+  --rexec TEXT               Replace with the result of piping to this tool
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-1.0/setup.py` & `symbex-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "1.0"
+VERSION = "1.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -28,10 +28,10 @@
     version=VERSION,
     packages=["symbex"],
     entry_points="""
         [console_scripts]
         symbex=symbex.cli:cli
     """,
     install_requires=["click"],
-    extras_require={"test": ["pytest", "pytest-icdiff", "cogapp", "PyYAML"]},
+    extras_require={"test": ["pytest", "pytest-icdiff", "cogapp", "PyYAML", "ruff"]},
     python_requires=">=3.8",
 )
```

### Comparing `symbex-1.0/symbex/cli.py` & `symbex-1.1/symbex/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 import click
 import importlib
 import inspect
 import pathlib
 import site
+import subprocess
 import sys
 
 from .lib import (
     code_for_node,
     find_symbol_nodes,
     import_line_for_function,
     read_file,
@@ -135,18 +136,22 @@
 )
 @click.option(
     "--no-init",
     is_flag=True,
     help="Filter to exclude any __init__ methods",
 )
 @click.option(
+    "--check", is_flag=True, help="Exit with non-zero code if any matches found"
+)
+@click.option(
     "--replace",
     is_flag=True,
     help="Replace matching symbol with text from stdin",
 )
+@click.option("--rexec", help="Replace with the result of piping to this tool")
 def cli(
     symbols,
     files,
     directories,
     stdlib,
     excludes,
     signatures,
@@ -163,15 +168,17 @@
     documented,
     undocumented,
     typed,
     untyped,
     partially_typed,
     fully_typed,
     no_init,
+    check,
     replace,
+    rexec,
 ):
     """
     Find symbols in Python code and print the code for them.
 
     Example usage:
 
     \b
@@ -228,15 +235,15 @@
             try:
                 mod = importlib.import_module(module)
                 mod_path = pathlib.Path(inspect.getfile(mod))
                 if mod_path.stem == "__init__":
                     module_dirs.append(mod_path.parent)
                 else:
                     module_files.append(mod_path)
-            except ModuleNotFoundError as ex:
+            except ModuleNotFoundError:
                 raise click.ClickException("Module not found: {}".format(module))
         directories = [*directories, *module_dirs]
         files = [*files, *module_files]
         if module_dirs or module_files:
             if not symbols:
                 symbols = ["*"]
             site_packages_dirs = site.getsitepackages()
@@ -274,14 +281,18 @@
             modules,
         ]
     ):
         ctx = click.get_current_context()
         click.echo(ctx.get_help())
         ctx.exit()
 
+    if rexec:
+        replace = True
+        no_file = True
+
     if replace and signatures:
         raise click.ClickException("--replace cannot be used with --signatures")
     if replace:
         no_file = True
     # Default to '*' if --signatures or filters are provided without symbols
     if (
         any(
@@ -314,18 +325,14 @@
             for path in pathlib.Path(directory).rglob("*.py"):
                 # Skip if path is inside any of 'excludes'
                 if any(is_subpath(path, exclude) for exclude in excludes):
                     continue
                 if path.is_file():
                     yield path
 
-    # Filter symbols by type
-    def filter(node: ast.AST) -> bool:
-        return True
-
     # If any --filters were supplied, handle them:
     if any(
         [
             async_,
             function,
             class_,
             documented,
@@ -333,15 +340,15 @@
             typed,
             untyped,
             partially_typed,
             fully_typed,
             no_init,
         ]
     ):
-
+        # Return just nodes matching filters
         def filter(node: ast.AST) -> bool:
             # Filters must ALL match
             if async_ and not isinstance(node, ast.AsyncFunctionDef):
                 return False
             if function and not isinstance(
                 node, (ast.FunctionDef, ast.AsyncFunctionDef)
             ):
@@ -367,14 +374,19 @@
                 return False
             if no_init and node.name == "__init__":
                 return False
             if fully_typed and not summary.fully:
                 return False
             return True
 
+    else:
+        # All nodes are allowed
+        def filter(node: ast.AST) -> bool:
+            return True
+
     pwd = pathlib.Path(".").resolve()
     num_matches = 0
     replace_matches = []
     for file in iterate_files():
         try:
             code = read_file(file)
         except UnicodeDecodeError as ex:
@@ -386,17 +398,18 @@
         except SyntaxError as ex:
             if not silent:
                 click.secho(f"# Syntax error in {file}: {ex}", err=True, fg="yellow")
             continue
         for node, class_name in nodes:
             if not filter(node):
                 continue
-            if count:
+            if count or check:
                 num_matches += 1
-                continue
+                if count or not signatures:
+                    continue
             # If file is within pwd, print relative path
             if pwd in file.resolve().parents:
                 path = file.resolve().relative_to(pwd)
             else:
                 # else print absolute path
                 path = file.resolve()
             snippet, line_no = code_for_node(code, node, class_name, signatures, docs)
@@ -420,32 +433,53 @@
                     )
                 click.echo("# " + import_line)
             click.echo(snippet)
             click.echo()
     if count:
         click.echo(num_matches)
 
+    if check and num_matches > 0:
+        sys.exit(1)
+
     if replace:
         # Only works if we got a single match
         if len(replace_matches) != 1:
             raise click.ClickException(
                 "--replace only works with a single match, got {}".format(
                     len(replace_matches)
                 )
             )
         filepath, to_replace = replace_matches[0][:2]
-        if sys.stdin.isatty():
-            raise click.ClickException(
-                "--replace only works with text piped to it on stdin"
+        if rexec:
+            # Run to_replace through that command
+            p = subprocess.Popen(
+                rexec,
+                stdin=subprocess.PIPE,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                shell=True,
             )
-        new_lines = sys.stdin.readlines()
-        # Check if any lines were read
-        if len(new_lines) == 0:
-            raise click.ClickException("No input for --replace found on stdin")
-        replacement = "".join(new_lines)
+            stdout, stderr = p.communicate(input=to_replace.encode())
+            if p.returncode != 0:
+                raise click.ClickException(
+                    f"Command '{rexec}' failed with exit code {p.returncode}"
+                    f", stderr: {stderr.decode()}"
+                )
+
+            replacement = stdout.decode()
+        else:
+            if sys.stdin.isatty():
+                raise click.ClickException(
+                    "--replace only works with text piped to it on stdin"
+                )
+            new_lines = sys.stdin.readlines()
+            # Check if any lines were read
+            if len(new_lines) == 0:
+                raise click.ClickException("No input for --replace found on stdin")
+            replacement = "".join(new_lines)
         old = filepath.read_text("utf-8")
         new = old.replace(to_replace, replacement)
         filepath.write_text(new, "utf-8")
 
 
 def is_subpath(path: pathlib.Path, parent: pathlib.Path) -> bool:
     try:
```

### Comparing `symbex-1.0/symbex/lib.py` & `symbex-1.1/symbex/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,16 @@
 def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str:
     if not docstrings:
         return definition
     docstring = ast.get_docstring(node)
     if not docstring:
         return definition
     docstring = quoted_string(docstring)
-    return f"{definition}\n{textwrap.indent(docstring, '        ' if is_method else '    ')}"
+    wrapped = textwrap.indent(docstring, "        " if is_method else "    ")
+    return f"{definition}\n{wrapped}"
 
 
 def match(name: str, symbols: Iterable[str]) -> bool:
     "Returns True if name matches any of the symbols, resolving wildcards"
     if name is None:
         return False
     for search in symbols:
```

### Comparing `symbex-1.0/symbex.egg-info/PKG-INFO` & `symbex-1.1/symbex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 1.0
+Version: 1.1
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -184,48 +184,48 @@
 runner = CliRunner()
 result = runner.invoke(cli, ["-s", "-f", str(path / "lib.py")])
 cog.out(
     "```python\n{}\n```\n".format(sorted_chunks(result.output))
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 106
+# File: symbex/lib.py Line: 107
 def function_definition(function_node: AST)
 
 # File: symbex/lib.py Line: 13
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 174
+# File: symbex/lib.py Line: 175
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 208
+# File: symbex/lib.py Line: 209
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 226
+# File: symbex/lib.py Line: 227
 def read_file(path)
 
-# File: symbex/lib.py Line: 252
+# File: symbex/lib.py Line: 253
 class TypeSummary
 
-# File: symbex/lib.py Line: 257
+# File: symbex/lib.py Line: 258
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 303
+# File: symbex/lib.py Line: 304
 def quoted_string(s)
 
-# File: symbex/lib.py Line: 314
+# File: symbex/lib.py Line: 315
 def import_line_for_function(function_name: str, filepath: str, possible_root_dirs: List[str]) -> str
 
 # File: symbex/lib.py Line: 37
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
 # File: symbex/lib.py Line: 71
 def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
 
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
 To include estimated import paths, such as `# from symbex.lib import match`, use `--imports`. These will be calculated relative to the directory you specified, or you can pass one or more `--sys-path` options to request that imports are calculated relative to those directories as if they were on `sys.path`:
 
@@ -238,15 +238,15 @@
     "--imports", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
 ])
 cog.out(
     "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 # from symbex.lib import match
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 To suppress the `# File: ...` comments, use `--no-file` or `-n`.
 
 So to both show import paths and suppress File comments, use `-in` as a shortcut:
@@ -276,15 +276,15 @@
 <!-- [[[cog
 result = runner.invoke(cli, ["match", "--docstrings", "-f", str(path / "lib.py")])
 cog.out(
     "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 81
+# File: symbex/lib.py Line: 82
 def match(name: str, symbols: Iterable[str]) -> bool
     "Returns True if name matches any of the symbols, resolving wildcards"
 ```
 <!-- [[[end]]] -->
 
 ## Counting symbols
 
@@ -331,37 +331,94 @@
 ```bash
 echo "def second_function(a, b):
     # This is a replacement implementation
     return a + b + 3
 " | symbex second_function --replace
 ```
 The result will be an updated-in-place `my_code.py` containing the following:
+
 ```python
 def first_function():
     # This will be ignored
     pass
 
 def second_function(a, b):
     # This is a replacement implementation
     return a + b + 3
 ```
 This feature should be used with care! I recommend only using this feature against code that is already checked into Git, so you can review changes it makes using `git diff` and revert them using `git checkout my_code.py`.
 
-You can use this with `llm` like so:
+## Replacing a matched symbol by running a command
+
+The `--rexec COMMAND` option can be used to replace a single matched symbol by running a command and using its output.
+
+The command will be run with the matched symbol's definition piped to its standard input. The output of that command will be used as the replacement text.
+
+Here's an example that uses `sed` to add a `# ` to the beginning of each matching line, effectively commenting out the matched function:
 
 ```bash
-symbex second_function -n \
-  | llm --system 'add type hints, remove docstring' \
-  | symbex second_function --replace
+symbex first_function --rexec "sed 's/^/# /'"
 ```
-When I ran this the result was a `second_function` definition like this:
+This modified the first function in place to look like this:
+```python
+# def first_function():
+#    # This will be ignored
+#    pass
+```
+A much more exciting example uses LLM. This example will use the `gpt-3.5-turbo` model to add type hints and generate a docstring:
+
+```bash
+symbex second_function \
+  --rexec "llm --system 'add type hints and a docstring'"
+```
+I ran this against this code:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function(a, b):
+    return a + b + 3
+```
+And the second function was updated in place to look like this:
 ```python
 def second_function(a: int, b: int) -> int:
+    """
+    Returns the sum of two integers (a and b) plus 3.
+
+    Parameters:
+    a (int): The first integer.
+    b (int): The second integer.
+
+    Returns:
+    int: The sum of a and b plus 3.
+    """
     return a + b + 3
 ```
+## Using in CI
+
+The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
+
+You can use this in CI to guard against things like functions being added without documentation:
+
+```bash
+symbex --function --undocumented --check
+```
+This will fail silently but set a `1` exit code if there are any undocumented functions.
+
+## Using in CI
+
+The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
+
+You can use this in CI to guard against things like functions being added without documentation:
+
+```bash
+symbex --function --undocumented --check
+```
+This will fail silently but set a `1` exit code if there are any undocumented functions.
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -436,15 +493,17 @@
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
+  --check                    Exit with non-zero code if any matches found
   --replace                  Replace matching symbol with text from stdin
+  --rexec TEXT               Replace with the result of piping to this tool
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-1.0/tests/test_filters.py` & `symbex-1.1/tests/test_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,7 +206,18 @@
     result2 = runner.invoke(
         cli,
         full_args + ["--count"],
         catch_exceptions=False,
     )
     assert result2.exit_code == 0
     assert result2.stdout.strip() == str(expected_count)
+
+    # And the --check option
+    result3 = runner.invoke(
+        cli,
+        full_args + ["--check"],
+        catch_exceptions=False,
+    )
+    if expected:
+        assert result3.exit_code == 1
+    else:
+        assert result3.exit_code == 0
```

### Comparing `symbex-1.0/tests/test_imports.py` & `symbex-1.1/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `symbex-1.0/tests/test_symbex.py` & `symbex-1.1/tests/test_symbex.py`

 * *Files identical despite different names*

### Comparing `symbex-1.0/tests/test_symbols.py` & `symbex-1.1/tests/test_symbols.py`

 * *Files identical despite different names*

