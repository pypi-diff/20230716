# Comparing `tmp/impose-cli-0.3.7.tar.gz` & `tmp/impose-cli-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.3.7.tar", last modified: Sun Jul 16 15:19:37 2023, max compression
+gzip compressed data, was "impose-cli-0.3.8.tar", last modified: Sun Jul 16 17:53:02 2023, max compression
```

## Comparing `impose-cli-0.3.7.tar` & `impose-cli-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 15:19:14.000000 impose-cli-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:19:37.358421 impose-cli-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-16 15:19:14.000000 impose-cli-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:19:37.358421 impose-cli-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-16 15:19:14.000000 impose-cli-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:14.000000 impose-cli-0.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-16 15:19:14.000000 impose-cli-0.3.7/tests/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 17:52:42.000000 impose-cli-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 17:53:02.219831 impose-cli-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-16 17:52:42.000000 impose-cli-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/impose_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 17:53:02.000000 impose-cli-0.3.8/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:53:02.219831 impose-cli-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-16 17:52:42.000000 impose-cli-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:52:42.000000 impose-cli-0.3.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-16 17:52:42.000000 impose-cli-0.3.8/tests/simple.py
```

### Comparing `impose-cli-0.3.7/LICENSE` & `impose-cli-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.7/README.md` & `impose-cli-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.7/impose_cli/_utils.py` & `impose-cli-0.3.8/impose_cli/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,16 @@
         dirs = [os.path.join(root, file) for root, _, files in os.walk(directory) for file in files if
                 file.endswith('.py')]
         return [abspath(join(directory, f)) for f in dirs]
 
     files = find_files()
     meta = produce_module_map(files)
     tree = build_tree(meta)
+    if target is None:
+        tree.root = tree.root.children[0]
     return tree
 
 
 class InterfaceBuilder(object):
     def __init__(self, tree):
         self.tree = tree
         self.root_name = "cli"
```

### Comparing `impose-cli-0.3.7/impose_cli/impose_cli.py` & `impose-cli-0.3.8/impose_cli/impose_cli.py`

 * *Files identical despite different names*

