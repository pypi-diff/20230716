# Comparing `tmp/pyccolo-0.0.8.tar.gz` & `tmp/pyccolo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyccolo-0.0.8.tar", last modified: Mon Jan 24 07:18:53 2022, max compression
+gzip compressed data, was "pyccolo-0.0.9.tar", last modified: Tue Jan 25 02:39:05 2022, max compression
```

## Comparing `pyccolo-0.0.8.tar` & `pyccolo-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-24 07:18:53.431381 pyccolo-0.0.8/
--rw-r--r--   0 smacke     (501) staff       (20)     1062 2022-01-24 07:12:06.000000 pyccolo-0.0.8/HISTORY.rst
--rw-r--r--   0 smacke     (501) staff       (20)       97 2021-12-15 06:38:18.000000 pyccolo-0.0.8/MANIFEST.in
--rw-r--r--   0 smacke     (501) staff       (20)    14822 2022-01-24 07:18:53.431597 pyccolo-0.0.8/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)    12024 2022-01-24 07:15:25.000000 pyccolo-0.0.8/README.md
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-24 07:18:53.432689 pyccolo-0.0.8/pyccolo/
--rw-r--r--   0 smacke     (501) staff       (20)     7693 2022-01-23 19:42:21.000000 pyccolo-0.0.8/pyccolo/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)     2064 2022-01-19 18:49:37.000000 pyccolo-0.0.8/pyccolo/__main__.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-24 07:18:53.426174 pyccolo-0.0.8/pyccolo/_fast/
--rw-r--r--   0 smacke     (501) staff       (20)      299 2022-01-09 05:06:32.000000 pyccolo-0.0.8/pyccolo/_fast/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)     1949 2022-01-16 21:07:28.000000 pyccolo-0.0.8/pyccolo/_fast/fast_ast.py
--rw-r--r--   0 smacke     (501) staff       (20)     3110 2022-01-21 18:35:45.000000 pyccolo-0.0.8/pyccolo/_fast/misc_ast_utils.py
--rw-r--r--   0 smacke     (501) staff       (20)      497 2022-01-24 07:18:53.432752 pyccolo-0.0.8/pyccolo/_version.py
--rw-r--r--   0 smacke     (501) staff       (20)     4816 2022-01-23 19:40:35.000000 pyccolo-0.0.8/pyccolo/ast_rewriter.py
--rw-r--r--   0 smacke     (501) staff       (20)     2371 2022-01-24 02:53:27.000000 pyccolo-0.0.8/pyccolo/emit_event.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-24 07:18:53.428074 pyccolo-0.0.8/pyccolo/examples/
--rw-r--r--   0 smacke     (501) staff       (20)      266 2022-01-24 01:55:49.000000 pyccolo-0.0.8/pyccolo/examples/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)     4468 2022-01-19 18:43:32.000000 pyccolo-0.0.8/pyccolo/examples/coverage.py
--rw-r--r--   0 smacke     (501) staff       (20)      900 2022-01-16 20:33:10.000000 pyccolo-0.0.8/pyccolo/examples/null_coalesce.py
--rw-r--r--   0 smacke     (501) staff       (20)     3090 2022-01-24 07:02:19.000000 pyccolo-0.0.8/pyccolo/examples/quasiquote.py
--rw-r--r--   0 smacke     (501) staff       (20)     1937 2022-01-24 07:14:44.000000 pyccolo-0.0.8/pyccolo/examples/quick_lambda.py
--rw-r--r--   0 smacke     (501) staff       (20)    28524 2022-01-23 19:40:44.000000 pyccolo-0.0.8/pyccolo/expr_rewriter.py
--rw-r--r--   0 smacke     (501) staff       (20)      362 2022-01-10 04:52:28.000000 pyccolo-0.0.8/pyccolo/extra_builtins.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-24 07:18:53.428431 pyccolo-0.0.8/pyccolo/fast/
--rw-r--r--   0 smacke     (501) staff       (20)      615 2022-01-09 05:06:32.000000 pyccolo-0.0.8/pyccolo/fast/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)     5782 2022-01-18 05:53:56.000000 pyccolo-0.0.8/pyccolo/import_hooks.py
--rw-r--r--   0 smacke     (501) staff       (20)    10430 2022-01-21 18:35:45.000000 pyccolo-0.0.8/pyccolo/stmt_inserter.py
--rw-r--r--   0 smacke     (501) staff       (20)     6887 2022-01-23 01:41:56.000000 pyccolo-0.0.8/pyccolo/stmt_mapper.py
--rw-r--r--   0 smacke     (501) staff       (20)     4142 2022-01-17 16:48:06.000000 pyccolo-0.0.8/pyccolo/syntax_augmentation.py
--rw-r--r--   0 smacke     (501) staff       (20)     5036 2022-01-24 02:49:07.000000 pyccolo-0.0.8/pyccolo/trace_events.py
--rw-r--r--   0 smacke     (501) staff       (20)     4060 2022-01-18 06:12:02.000000 pyccolo-0.0.8/pyccolo/trace_stack.py
--rw-r--r--   0 smacke     (501) staff       (20)    29431 2022-01-24 07:04:39.000000 pyccolo-0.0.8/pyccolo/tracer.py
--rw-r--r--   0 smacke     (501) staff       (20)      202 2022-01-09 05:06:32.000000 pyccolo-0.0.8/pyccolo/utils.py
--rw-r--r--   0 smacke     (501) staff       (20)      520 2022-01-09 05:06:32.000000 pyccolo-0.0.8/pyccolo/version.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-24 07:18:53.424893 pyccolo-0.0.8/pyccolo.egg-info/
--rw-r--r--   0 smacke     (501) staff       (20)    14822 2022-01-24 07:18:53.000000 pyccolo-0.0.8/pyccolo.egg-info/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)     1158 2022-01-24 07:18:53.000000 pyccolo-0.0.8/pyccolo.egg-info/SOURCES.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2022-01-24 07:18:53.000000 pyccolo-0.0.8/pyccolo.egg-info/dependency_links.txt
--rw-r--r--   0 smacke     (501) staff       (20)       79 2022-01-24 07:18:53.000000 pyccolo-0.0.8/pyccolo.egg-info/entry_points.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2022-01-24 07:18:53.000000 pyccolo-0.0.8/pyccolo.egg-info/not-zip-safe
--rw-r--r--   0 smacke     (501) staff       (20)       15 2022-01-24 07:18:53.000000 pyccolo-0.0.8/pyccolo.egg-info/requires.txt
--rw-r--r--   0 smacke     (501) staff       (20)        8 2022-01-24 07:18:53.000000 pyccolo-0.0.8/pyccolo.egg-info/top_level.txt
--rw-r--r--   0 smacke     (501) staff       (20)      124 2022-01-17 17:32:20.000000 pyccolo-0.0.8/pyproject.toml
--rw-r--r--   0 smacke     (501) staff       (20)       15 2022-01-09 05:06:32.000000 pyccolo-0.0.8/requirements.txt
--rw-r--r--   0 smacke     (501) staff       (20)      572 2022-01-24 07:18:53.432381 pyccolo-0.0.8/setup.cfg
--rw-r--r--   0 smacke     (501) staff       (20)     1657 2022-01-16 19:43:43.000000 pyccolo-0.0.8/setup.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-24 07:18:53.431044 pyccolo-0.0.8/test/
--rw-r--r--   0 smacke     (501) staff       (20)    18097 2022-01-24 07:05:40.000000 pyccolo-0.0.8/test/test_handlers.py
--rw-r--r--   0 smacke     (501) staff       (20)      469 2022-01-17 17:27:15.000000 pyccolo-0.0.8/test/test_import_hooks.py
--rw-r--r--   0 smacke     (501) staff       (20)     1399 2022-01-19 18:49:37.000000 pyccolo-0.0.8/test/test_instrumented_functions.py
--rw-r--r--   0 smacke     (501) staff       (20)     1296 2022-01-09 05:06:32.000000 pyccolo-0.0.8/test/test_no_prints.py
--rw-r--r--   0 smacke     (501) staff       (20)      612 2022-01-20 06:53:39.000000 pyccolo-0.0.8/test/test_script_entrypoint.py
--rw-r--r--   0 smacke     (501) staff       (20)     5943 2022-01-18 06:11:41.000000 pyccolo-0.0.8/test/test_stack.py
--rw-r--r--   0 smacke     (501) staff       (20)     4475 2022-01-22 05:03:41.000000 pyccolo-0.0.8/test/test_syntax_augmentation.py
--rw-r--r--   0 smacke     (501) staff       (20)    19800 2022-01-22 01:58:37.000000 pyccolo-0.0.8/test/test_trace_events.py
--rw-r--r--   0 smacke     (501) staff       (20)    70144 2021-12-27 22:22:54.000000 pyccolo-0.0.8/versioneer.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-25 02:39:05.730584 pyccolo-0.0.9/
+-rw-r--r--   0 smacke     (501) staff       (20)     1133 2022-01-25 02:32:31.000000 pyccolo-0.0.9/HISTORY.rst
+-rw-r--r--   0 smacke     (501) staff       (20)       97 2021-12-15 06:38:18.000000 pyccolo-0.0.9/MANIFEST.in
+-rw-r--r--   0 smacke     (501) staff       (20)    14820 2022-01-25 02:39:05.730802 pyccolo-0.0.9/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)    12022 2022-01-25 02:32:31.000000 pyccolo-0.0.9/README.md
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-25 02:39:05.731855 pyccolo-0.0.9/pyccolo/
+-rw-r--r--   0 smacke     (501) staff       (20)     7693 2022-01-23 19:42:21.000000 pyccolo-0.0.9/pyccolo/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)     2064 2022-01-19 18:49:37.000000 pyccolo-0.0.9/pyccolo/__main__.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-25 02:39:05.719078 pyccolo-0.0.9/pyccolo/_fast/
+-rw-r--r--   0 smacke     (501) staff       (20)      299 2022-01-09 05:06:32.000000 pyccolo-0.0.9/pyccolo/_fast/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1949 2022-01-16 21:07:28.000000 pyccolo-0.0.9/pyccolo/_fast/fast_ast.py
+-rw-r--r--   0 smacke     (501) staff       (20)     3110 2022-01-21 18:35:45.000000 pyccolo-0.0.9/pyccolo/_fast/misc_ast_utils.py
+-rw-r--r--   0 smacke     (501) staff       (20)      497 2022-01-25 02:39:05.731920 pyccolo-0.0.9/pyccolo/_version.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4827 2022-01-25 02:32:31.000000 pyccolo-0.0.9/pyccolo/ast_rewriter.py
+-rw-r--r--   0 smacke     (501) staff       (20)     2519 2022-01-25 02:32:31.000000 pyccolo-0.0.9/pyccolo/emit_event.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-25 02:39:05.723180 pyccolo-0.0.9/pyccolo/examples/
+-rw-r--r--   0 smacke     (501) staff       (20)      266 2022-01-24 01:55:49.000000 pyccolo-0.0.9/pyccolo/examples/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4468 2022-01-19 18:43:32.000000 pyccolo-0.0.9/pyccolo/examples/coverage.py
+-rw-r--r--   0 smacke     (501) staff       (20)      900 2022-01-16 20:33:10.000000 pyccolo-0.0.9/pyccolo/examples/null_coalesce.py
+-rw-r--r--   0 smacke     (501) staff       (20)     3070 2022-01-25 02:32:31.000000 pyccolo-0.0.9/pyccolo/examples/quasiquote.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1894 2022-01-25 02:32:31.000000 pyccolo-0.0.9/pyccolo/examples/quick_lambda.py
+-rw-r--r--   0 smacke     (501) staff       (20)    28524 2022-01-23 19:40:44.000000 pyccolo-0.0.9/pyccolo/expr_rewriter.py
+-rw-r--r--   0 smacke     (501) staff       (20)      362 2022-01-10 04:52:28.000000 pyccolo-0.0.9/pyccolo/extra_builtins.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-25 02:39:05.723930 pyccolo-0.0.9/pyccolo/fast/
+-rw-r--r--   0 smacke     (501) staff       (20)      615 2022-01-09 05:06:32.000000 pyccolo-0.0.9/pyccolo/fast/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)     5782 2022-01-18 05:53:56.000000 pyccolo-0.0.9/pyccolo/import_hooks.py
+-rw-r--r--   0 smacke     (501) staff       (20)    10430 2022-01-21 18:35:45.000000 pyccolo-0.0.9/pyccolo/stmt_inserter.py
+-rw-r--r--   0 smacke     (501) staff       (20)     6887 2022-01-23 01:41:56.000000 pyccolo-0.0.9/pyccolo/stmt_mapper.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4142 2022-01-24 21:13:25.000000 pyccolo-0.0.9/pyccolo/syntax_augmentation.py
+-rw-r--r--   0 smacke     (501) staff       (20)     5036 2022-01-24 02:49:07.000000 pyccolo-0.0.9/pyccolo/trace_events.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4060 2022-01-24 21:10:21.000000 pyccolo-0.0.9/pyccolo/trace_stack.py
+-rw-r--r--   0 smacke     (501) staff       (20)    29718 2022-01-25 02:32:31.000000 pyccolo-0.0.9/pyccolo/tracer.py
+-rw-r--r--   0 smacke     (501) staff       (20)      202 2022-01-09 05:06:32.000000 pyccolo-0.0.9/pyccolo/utils.py
+-rw-r--r--   0 smacke     (501) staff       (20)      520 2022-01-09 05:06:32.000000 pyccolo-0.0.9/pyccolo/version.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-25 02:39:05.717309 pyccolo-0.0.9/pyccolo.egg-info/
+-rw-r--r--   0 smacke     (501) staff       (20)    14820 2022-01-25 02:39:05.000000 pyccolo-0.0.9/pyccolo.egg-info/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)     1158 2022-01-25 02:39:05.000000 pyccolo-0.0.9/pyccolo.egg-info/SOURCES.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2022-01-25 02:39:05.000000 pyccolo-0.0.9/pyccolo.egg-info/dependency_links.txt
+-rw-r--r--   0 smacke     (501) staff       (20)       79 2022-01-25 02:39:05.000000 pyccolo-0.0.9/pyccolo.egg-info/entry_points.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2022-01-25 02:39:05.000000 pyccolo-0.0.9/pyccolo.egg-info/not-zip-safe
+-rw-r--r--   0 smacke     (501) staff       (20)       15 2022-01-25 02:39:05.000000 pyccolo-0.0.9/pyccolo.egg-info/requires.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        8 2022-01-25 02:39:05.000000 pyccolo-0.0.9/pyccolo.egg-info/top_level.txt
+-rw-r--r--   0 smacke     (501) staff       (20)      124 2022-01-17 17:32:20.000000 pyccolo-0.0.9/pyproject.toml
+-rw-r--r--   0 smacke     (501) staff       (20)       15 2022-01-09 05:06:32.000000 pyccolo-0.0.9/requirements.txt
+-rw-r--r--   0 smacke     (501) staff       (20)      572 2022-01-25 02:39:05.731522 pyccolo-0.0.9/setup.cfg
+-rw-r--r--   0 smacke     (501) staff       (20)     1657 2022-01-16 19:43:43.000000 pyccolo-0.0.9/setup.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-01-25 02:39:05.729709 pyccolo-0.0.9/test/
+-rw-r--r--   0 smacke     (501) staff       (20)    18097 2022-01-24 07:05:40.000000 pyccolo-0.0.9/test/test_handlers.py
+-rw-r--r--   0 smacke     (501) staff       (20)      469 2022-01-17 17:27:15.000000 pyccolo-0.0.9/test/test_import_hooks.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1399 2022-01-19 18:49:37.000000 pyccolo-0.0.9/test/test_instrumented_functions.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1296 2022-01-09 05:06:32.000000 pyccolo-0.0.9/test/test_no_prints.py
+-rw-r--r--   0 smacke     (501) staff       (20)      612 2022-01-20 06:53:39.000000 pyccolo-0.0.9/test/test_script_entrypoint.py
+-rw-r--r--   0 smacke     (501) staff       (20)     5943 2022-01-18 06:11:41.000000 pyccolo-0.0.9/test/test_stack.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4475 2022-01-22 05:03:41.000000 pyccolo-0.0.9/test/test_syntax_augmentation.py
+-rw-r--r--   0 smacke     (501) staff       (20)    19800 2022-01-22 01:58:37.000000 pyccolo-0.0.9/test/test_trace_events.py
+-rw-r--r--   0 smacke     (501) staff       (20)    70144 2021-12-27 22:22:54.000000 pyccolo-0.0.9/versioneer.py
```

### Comparing `pyccolo-0.0.8/HISTORY.rst` & `pyccolo-0.0.9/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 History
 =======
 
+0.0.9 (2022-01-24)
+------------------
+* Allow per-handler reentrancy;
+
 0.0.8 (2022-01-23)
 ------------------
 * Add eval helper;
 * Add syntactic macro examples (quasiquotes and quick lambdas);
 * Add support for conditional handlers;
 
 0.0.7 (2022-01-06)
```

### Comparing `pyccolo-0.0.8/PKG-INFO` & `pyccolo-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyccolo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Embedded instrumentation for Python.
 Home-page: https://github.com/smacke/pyccolo
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: BSD-3-Clause
 Description: Pyccolo
         =======
@@ -25,15 +25,15 @@
         multiple versions of Python (3.6 to 3.10), with few exceptions. Portability
         across versions is accomplished by embedding instrumentation at the level of
         source code (as opposed to bytecode-level instrumentation).
         
         Pyccolo can be used (and has been used) to implement various kinds of dynamic analysis
         tools and other instrumentation:
         - Code coverage (see [pyccolo/examples/coverage.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/coverage.py))
-        - Syntactic macros such as quasiquotes (like [MacroPy's](https://macropy3.readthedocs.io/en/latest/reference.html#quasiquote) or quick lambdas; see [pyccolo/examples/quasiquote.py)](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quasiquote.py) and [pyccolo/examples/quick_lambda.py)](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quick_lambda.py))
+        - Syntactic macros such as quasiquotes (like [MacroPy's](https://macropy3.readthedocs.io/en/latest/reference.html#quasiquote)) or quick lambdas; see [pyccolo/examples/quasiquote.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quasiquote.py) and [pyccolo/examples/quick_lambda.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quick_lambda.py)
         - Syntax-augmented Python (3.8 and up, see [pyccolo/examples/null_coalesce.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/null_coalesce.py))
         - Dynamic dataflow analysis performed by [nbsafety](https://github.com/nbsafety-project/nbsafety)
         - Tools to find unused imports at runtime (candidates for lazy importing)
         - Tools to uncover [semantic memory leaks](http://ithare.com/java-vs-c-trading-ub-for-semantic-memory-leaks-same-problem-different-punishment-for-failure/)
         - \<Your tool here!>
         
         ## Install
```

### Comparing `pyccolo-0.0.8/README.md` & `pyccolo-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 multiple versions of Python (3.6 to 3.10), with few exceptions. Portability
 across versions is accomplished by embedding instrumentation at the level of
 source code (as opposed to bytecode-level instrumentation).
 
 Pyccolo can be used (and has been used) to implement various kinds of dynamic analysis
 tools and other instrumentation:
 - Code coverage (see [pyccolo/examples/coverage.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/coverage.py))
-- Syntactic macros such as quasiquotes (like [MacroPy's](https://macropy3.readthedocs.io/en/latest/reference.html#quasiquote) or quick lambdas; see [pyccolo/examples/quasiquote.py)](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quasiquote.py) and [pyccolo/examples/quick_lambda.py)](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quick_lambda.py))
+- Syntactic macros such as quasiquotes (like [MacroPy's](https://macropy3.readthedocs.io/en/latest/reference.html#quasiquote)) or quick lambdas; see [pyccolo/examples/quasiquote.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quasiquote.py) and [pyccolo/examples/quick_lambda.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quick_lambda.py)
 - Syntax-augmented Python (3.8 and up, see [pyccolo/examples/null_coalesce.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/null_coalesce.py))
 - Dynamic dataflow analysis performed by [nbsafety](https://github.com/nbsafety-project/nbsafety)
 - Tools to find unused imports at runtime (candidates for lazy importing)
 - Tools to uncover [semantic memory leaks](http://ithare.com/java-vs-c-trading-ub-for-semantic-memory-leaks-same-problem-different-punishment-for-failure/)
 - \<Your tool here!>
 
 ## Install
```

### Comparing `pyccolo-0.0.8/pyccolo/__init__.py` & `pyccolo-0.0.9/pyccolo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/__main__.py` & `pyccolo-0.0.9/pyccolo/__main__.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/_fast/fast_ast.py` & `pyccolo-0.0.9/pyccolo/_fast/fast_ast.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/_fast/misc_ast_utils.py` & `pyccolo-0.0.9/pyccolo/_fast/misc_ast_utils.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/ast_rewriter.py` & `pyccolo-0.0.9/pyccolo/ast_rewriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,17 @@
         for tracer in self._tracers:
             for evt in tracer.events_with_registered_handlers:
                 if self._path is not None and not tracer._file_passes_filter_impl(
                     evt.value, self._path
                 ):
                     continue
                 handler_data = tracer._event_handlers.get(
-                    evt, [(None, False, lambda *_: True)]
+                    evt, [(None, False, False, lambda *_: True)]
                 )
-                for _, use_raw_node_id, raw_condition in handler_data:
+                for _, use_raw_node_id, __, raw_condition in handler_data:
                     condition: CONDITION = self._make_condition(
                         use_raw_node_id, raw_condition
                     )
                     raw_handler_conditions_by_event[evt].append(condition)
         handler_condition_by_event: DefaultDict[TraceEvent, CONDITION] = defaultdict(
             lambda: (lambda *_: False)
         )
```

### Comparing `pyccolo-0.0.8/pyccolo/emit_event.py` & `pyccolo-0.0.9/pyccolo/emit_event.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,34 +36,39 @@
     else:
         return ret
 
 
 def _emit_event(event, node_id, **kwargs):
     global _allow_event_handling
     global _allow_reentrant_event_handling
-    if not _allow_event_handling and not _allow_reentrant_event_handling:
-        return _make_ret(event, kwargs.get("ret", None))
     frame = sys._getframe().f_back
     if frame.f_code.co_filename == __file__:
         # weird shit happens if we instrument this file, so exclude it.
         return _make_ret(event, kwargs.get("ret", None))
     orig_allow_event_handling = _allow_event_handling
     orig_allow_reentrant_event_handling = _allow_reentrant_event_handling
     try:
         is_reentrant = not _allow_event_handling
+        reentrant_handlers_only = is_reentrant and not _allow_reentrant_event_handling
         _allow_event_handling = False
         _allow_reentrant_event_handling = False
         for tracer in _TRACER_STACK:
             if tracer._file_passes_filter_impl(
                 event, frame.f_code.co_filename, is_reentrant=is_reentrant
             ):
                 try:
                     _allow_reentrant_event_handling = (
                         orig_allow_reentrant_event_handling
                     )
-                    kwargs["ret"] = tracer._emit_event(event, node_id, frame, **kwargs)
+                    kwargs["ret"] = tracer._emit_event(
+                        event,
+                        node_id,
+                        frame,
+                        reentrant_handlers_only=reentrant_handlers_only,
+                        **kwargs,
+                    )
                 finally:
                     _allow_reentrant_event_handling = False
     finally:
         _allow_event_handling = orig_allow_event_handling
         _allow_reentrant_event_handling = orig_allow_reentrant_event_handling
     return _make_ret(event, kwargs.get("ret", None))
```

### Comparing `pyccolo-0.0.8/pyccolo/examples/coverage.py` & `pyccolo-0.0.9/pyccolo/examples/coverage.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/examples/null_coalesce.py` & `pyccolo-0.0.9/pyccolo/examples/null_coalesce.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/examples/quasiquote.py` & `pyccolo-0.0.9/pyccolo/examples/quasiquote.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,43 +62,41 @@
     def exit_tracing_hook(self) -> None:
         import builtins
 
         for macro in self.macros:
             if hasattr(builtins, macro):
                 delattr(builtins, macro)
 
-    @pyc.before_subscript_slice(when=is_macro("q"))
+    @pyc.before_subscript_slice(when=is_macro("q"), reentrant=True)
     def quote_handler(self, _ret, node, frame, *_, **__):
         to_visit = node.slice
         if isinstance(node.slice, ast.Index):
             to_visit = to_visit.value
         return lambda: _QuasiquoteTransformer(frame.f_globals, frame.f_locals).visit(
             copy.deepcopy(to_visit)
         )
 
-    @pyc.after_subscript_slice(when=is_macro("u"))
+    @pyc.after_subscript_slice(when=is_macro("u"), reentrant=True)
     def unquote_handler(self, ret, *_, **__):
-        with pyc.allow_reentrant_event_handling():
-            return pyc.eval(f"q[{repr(ret)}]")
+        return pyc.eval(f"q[{repr(ret)}]")
 
-    @pyc.after_subscript_slice(when=is_macro("name"))
+    @pyc.after_subscript_slice(when=is_macro("name"), reentrant=True)
     def name_handler(self, ret, *_, **__):
         assert isinstance(ret, str)
-        with pyc.allow_reentrant_event_handling():
-            return pyc.eval(f"q[{ret}]")
+        return pyc.eval(f"q[{ret}]")
 
-    @pyc.after_subscript_slice(when=is_macro("ast_literal"))
+    @pyc.after_subscript_slice(when=is_macro("ast_literal"), reentrant=True)
     def ast_literal_handler(self, ret, *_, **__):
         # technically we could get away without even having this handler
         assert isinstance(ret, ast.AST)
         return ret
 
-    @pyc.after_subscript_slice(when=is_macro("ast_list"))
+    @pyc.after_subscript_slice(when=is_macro("ast_list"), reentrant=True)
     def ast_list_handler(self, ret, *_, **__):
         return ast.List(elts=list(ret))
 
     def is_any_macro(self, node):
         return any(is_macro(m)(node) for m in self.macros)
 
-    @pyc.before_subscript_load(when=is_any_macro)
-    def load_macro_result(self, _ret, node, *_, **__):
+    @pyc.before_subscript_load(when=is_any_macro, reentrant=True)
+    def load_macro_result(self, _ret, *_, **__):
         return _identity_subscript
```

### Comparing `pyccolo-0.0.8/pyccolo/examples/quick_lambda.py` & `pyccolo-0.0.9/pyccolo/examples/quick_lambda.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,23 +36,22 @@
 
 class QuickLambdaTracer(Quasiquoter):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.macros.add("f")
         self._arg_replacer = _ArgReplacer()
 
-    @pyc.before_subscript_slice(when=is_macro("f"))
+    @pyc.before_subscript_slice(when=is_macro("f"), reentrant=True)
     def handle_quick_lambda(self, _ret, node, frame, *_, **__):
         orig_ctr = self._arg_replacer.ctr
         orig_lambda_body = node.slice
         if isinstance(node.slice, ast.Index):
             orig_lambda_body = orig_lambda_body.value
         lambda_body = self._arg_replacer.visit(  # noqa: F841
             copy.deepcopy(orig_lambda_body)
         )
         num_lambda_args = self._arg_replacer.ctr - orig_ctr
         lambda_args = ", ".join(
             f"_{arg_idx}" for arg_idx in range(orig_ctr, orig_ctr + num_lambda_args)
         )
-        with pyc.allow_reentrant_event_handling():
-            ast_lambda = pyc.eval(f"q[lambda {lambda_args}: ast_literal[lambda_body]]")
-            return lambda: pyc.eval(ast_lambda, frame.f_globals, frame.f_locals)
+        ast_lambda = pyc.eval(f"q[lambda {lambda_args}: ast_literal[lambda_body]]")
+        return lambda: pyc.eval(ast_lambda, frame.f_globals, frame.f_locals)
```

### Comparing `pyccolo-0.0.8/pyccolo/expr_rewriter.py` & `pyccolo-0.0.9/pyccolo/expr_rewriter.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/fast/__init__.py` & `pyccolo-0.0.9/pyccolo/fast/__init__.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/import_hooks.py` & `pyccolo-0.0.9/pyccolo/import_hooks.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/stmt_inserter.py` & `pyccolo-0.0.9/pyccolo/stmt_inserter.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/stmt_mapper.py` & `pyccolo-0.0.9/pyccolo/stmt_mapper.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/syntax_augmentation.py` & `pyccolo-0.0.9/pyccolo/syntax_augmentation.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/trace_events.py` & `pyccolo-0.0.9/pyccolo/trace_events.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/trace_stack.py` & `pyccolo-0.0.9/pyccolo/trace_stack.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo/tracer.py` & `pyccolo-0.0.9/pyccolo/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     def __call__(cls, *args, **kwargs):
         obj = MetaHasTraits.__call__(cls, *args, **kwargs)
         obj._post_init_hook_end()
         return obj
 
 
-_HANDLER_DATA_T = Tuple[Callable[..., Any], bool, Callable[..., bool]]
+_HANDLER_DATA_T = Tuple[Callable[..., Any], bool, bool, Callable[..., bool]]
 
 
 class _InternalBaseTracer(metaclass=MetaTracerStateMachine):
     ast_rewriter_cls = AstRewriter
     defined_file = ""
 
     _MANAGER_CLASS_REGISTERED = False
@@ -244,23 +244,29 @@
         return False
 
     def _emit_event(
         self,
         evt: Union[str, TraceEvent],
         node_id: Optional[int],
         frame: FrameType,
+        reentrant_handlers_only: bool = False,
         **kwargs: Any,
     ):
         try:
             if self._is_tracing_hard_disabled:
                 return kwargs.get("ret", None)
             event = evt if isinstance(evt, TraceEvent) else TraceEvent(evt)
-            for handler, use_raw_node_id, condition in self._event_handlers.get(
-                event, []
-            ):
+            for (
+                handler,
+                use_raw_node_id,
+                reentrant,
+                condition,
+            ) in self._event_handlers.get(event, []):
+                if reentrant_handlers_only and not reentrant:
+                    continue
                 old_ret = kwargs.pop("ret", None)
                 try:
                     node_id_or_node = (
                         node_id
                         if use_raw_node_id
                         else self.ast_node_by_id.get(node_id, None)
                     )
@@ -720,29 +726,30 @@
 
 
 def register_handler(
     event: Union[
         Union[TraceEvent, Type[ast.AST]], Tuple[Union[TraceEvent, Type[ast.AST]], ...]
     ],
     use_raw_node_id: bool = False,
+    reentrant: bool = False,
     when: Optional[Callable[..., bool]] = None,
 ):
     events = event if isinstance(event, tuple) else (event,)
     when = (lambda *_: True) if when is None else when
 
     if TraceEvent.opcode in events and sys.version_info < (3, 7):
         raise ValueError("can't trace opcodes on Python < 3.7")
 
     def _inner_registrar(handler):
         for evt in events:
             _InternalBaseTracer.EVENT_HANDLERS_PENDING_REGISTRATION[
                 AST_TO_EVENT_MAPPING[evt]
                 if type(evt) is type and issubclass(evt, ast.AST)
                 else evt
-            ].append((handler, use_raw_node_id, when))
+            ].append((handler, use_raw_node_id, reentrant, when))
         return handler
 
     return _inner_registrar
 
 
 def __event_call__(self, handler=None, **kwargs):
     if handler is None:
@@ -791,17 +798,18 @@
         self._saved_slice: Optional[Any] = None
 
     @register_raw_handler(
         (
             TraceEvent.before_subscript_load,
             TraceEvent.before_subscript_store,
             TraceEvent.before_subscript_del,
-        )
+        ),
+        reentrant=True,
     )
     def _save_slice_for_later(self, *_, attr_or_subscript: Any, **__):
         self._saved_slice = attr_or_subscript
 
-    @register_raw_handler(TraceEvent._load_saved_slice)
+    @register_raw_handler(TraceEvent._load_saved_slice, reentrant=True)
     def _load_saved_slice(self, *_, **__):
         ret = self._saved_slice
         self._saved_slice = None
         return ret
```

### Comparing `pyccolo-0.0.8/pyccolo/version.py` & `pyccolo-0.0.9/pyccolo/version.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/pyccolo.egg-info/PKG-INFO` & `pyccolo-0.0.9/pyccolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyccolo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Embedded instrumentation for Python.
 Home-page: https://github.com/smacke/pyccolo
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: BSD-3-Clause
 Description: Pyccolo
         =======
@@ -25,15 +25,15 @@
         multiple versions of Python (3.6 to 3.10), with few exceptions. Portability
         across versions is accomplished by embedding instrumentation at the level of
         source code (as opposed to bytecode-level instrumentation).
         
         Pyccolo can be used (and has been used) to implement various kinds of dynamic analysis
         tools and other instrumentation:
         - Code coverage (see [pyccolo/examples/coverage.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/coverage.py))
-        - Syntactic macros such as quasiquotes (like [MacroPy's](https://macropy3.readthedocs.io/en/latest/reference.html#quasiquote) or quick lambdas; see [pyccolo/examples/quasiquote.py)](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quasiquote.py) and [pyccolo/examples/quick_lambda.py)](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quick_lambda.py))
+        - Syntactic macros such as quasiquotes (like [MacroPy's](https://macropy3.readthedocs.io/en/latest/reference.html#quasiquote)) or quick lambdas; see [pyccolo/examples/quasiquote.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quasiquote.py) and [pyccolo/examples/quick_lambda.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/quick_lambda.py)
         - Syntax-augmented Python (3.8 and up, see [pyccolo/examples/null_coalesce.py](https://github.com/smacke/pyccolo/blob/master/pyccolo/examples/null_coalesce.py))
         - Dynamic dataflow analysis performed by [nbsafety](https://github.com/nbsafety-project/nbsafety)
         - Tools to find unused imports at runtime (candidates for lazy importing)
         - Tools to uncover [semantic memory leaks](http://ithare.com/java-vs-c-trading-ub-for-semantic-memory-leaks-same-problem-different-punishment-for-failure/)
         - \<Your tool here!>
         
         ## Install
```

### Comparing `pyccolo-0.0.8/pyccolo.egg-info/SOURCES.txt` & `pyccolo-0.0.9/pyccolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/setup.cfg` & `pyccolo-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/setup.py` & `pyccolo-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/test/test_handlers.py` & `pyccolo-0.0.9/test/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/test/test_instrumented_functions.py` & `pyccolo-0.0.9/test/test_instrumented_functions.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/test/test_no_prints.py` & `pyccolo-0.0.9/test/test_no_prints.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/test/test_script_entrypoint.py` & `pyccolo-0.0.9/test/test_script_entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/test/test_stack.py` & `pyccolo-0.0.9/test/test_stack.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/test/test_syntax_augmentation.py` & `pyccolo-0.0.9/test/test_syntax_augmentation.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/test/test_trace_events.py` & `pyccolo-0.0.9/test/test_trace_events.py`

 * *Files identical despite different names*

### Comparing `pyccolo-0.0.8/versioneer.py` & `pyccolo-0.0.9/versioneer.py`

 * *Files identical despite different names*

