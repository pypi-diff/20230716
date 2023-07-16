# Comparing `tmp/impose-cli-0.3.6.tar.gz` & `tmp/impose-cli-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.3.6.tar", last modified: Sun Jul 16 15:05:10 2023, max compression
+gzip compressed data, was "impose-cli-0.3.7.tar", last modified: Sun Jul 16 15:19:37 2023, max compression
```

## Comparing `impose-cli-0.3.6.tar` & `impose-cli-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 15:04:50.000000 impose-cli-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:05:10.484569 impose-cli-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-16 15:04:50.000000 impose-cli-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:05:10.484569 impose-cli-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-16 15:04:50.000000 impose-cli-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:04:50.000000 impose-cli-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-16 15:04:50.000000 impose-cli-0.3.6/tests/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 15:19:14.000000 impose-cli-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:19:37.358421 impose-cli-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-16 15:19:14.000000 impose-cli-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-16 15:19:14.000000 impose-cli-0.3.7/impose_cli/impose_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 15:19:37.000000 impose-cli-0.3.7/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:19:37.358421 impose-cli-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-16 15:19:14.000000 impose-cli-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:37.358421 impose-cli-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:19:14.000000 impose-cli-0.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-16 15:19:14.000000 impose-cli-0.3.7/tests/simple.py
```

### Comparing `impose-cli-0.3.6/LICENSE` & `impose-cli-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.6/README.md` & `impose-cli-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.6/impose_cli/_utils.py` & `impose-cli-0.3.7/impose_cli/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     tree = build_tree(meta)
     return tree
 
 
 class InterfaceBuilder(object):
     def __init__(self, tree):
         self.tree = tree
+        self.root_name = "cli"
 
     def dfs(self):
         self.initialize_root()
         root = self.tree.root
         for function in root.functions:
             self.handle_vertex(root, function)
         root.alter_children(type(self).handle_edge)
@@ -212,15 +213,15 @@
 
     def run(self):
         self.tree.root.external_object()
 
 
 class CLIInterfaceBuilder(InterfaceBuilder):
     def initialize_root(self):
-        name = "cli" if self.tree.root.name == "" and self.root_name is None else self.root_name
+        name = "cli" if self.tree.root.name == "" or self.tree.root.name is None else self.root_name
         self.tree.root.external_object = click.Group(name=name)
 
     @staticmethod
     def handle_vertex(node, function):
         command = click.Command(
             name=function.name.replace("_", "-"),
             callback=function.reference,
```

### Comparing `impose-cli-0.3.6/impose_cli/impose_cli.py` & `impose-cli-0.3.7/impose_cli/impose_cli.py`

 * *Files identical despite different names*

