# Comparing `tmp/impose-cli-0.3.5.tar.gz` & `tmp/impose-cli-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.3.5.tar", last modified: Wed Jul 12 07:55:50 2023, max compression
+gzip compressed data, was "impose-cli-0.3.6.tar", last modified: Sun Jul 16 15:05:10 2023, max compression
```

## Comparing `impose-cli-0.3.5.tar` & `impose-cli-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 07:55:29.000000 impose-cli-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 07:55:50.342055 impose-cli-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-12 07:55:29.000000 impose-cli-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 07:55:50.342055 impose-cli-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-12 07:55:29.000000 impose-cli-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:29.000000 impose-cli-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 07:55:29.000000 impose-cli-0.3.5/tests/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 15:04:50.000000 impose-cli-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:05:10.484569 impose-cli-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-16 15:04:50.000000 impose-cli-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-16 15:04:50.000000 impose-cli-0.3.6/impose_cli/impose_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 15:05:10.000000 impose-cli-0.3.6/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:05:10.484569 impose-cli-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-16 15:04:50.000000 impose-cli-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:05:10.484569 impose-cli-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:04:50.000000 impose-cli-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-16 15:04:50.000000 impose-cli-0.3.6/tests/simple.py
```

### Comparing `impose-cli-0.3.5/LICENSE` & `impose-cli-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.5/README.md` & `impose-cli-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.5/impose_cli/_utils.py` & `impose-cli-0.3.6/impose_cli/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -181,25 +181,20 @@
         dirs = [os.path.join(root, file) for root, _, files in os.walk(directory) for file in files if
                 file.endswith('.py')]
         return [abspath(join(directory, f)) for f in dirs]
 
     files = find_files()
     meta = produce_module_map(files)
     tree = build_tree(meta)
-    if len(tree.root.children) == 1 and not len(tree.root.functions) and (tree.root.name == "" or tree.root.name is None):
-        tree.root = tree.root.children[0]
-        tree.root.root = True
     return tree
 
 
 class InterfaceBuilder(object):
-    def __init__(self, tree, root_name: str, config: dict = None):
+    def __init__(self, tree):
         self.tree = tree
-        self.config = config
-        self.root_name = root_name
 
     def dfs(self):
         self.initialize_root()
         root = self.tree.root
         for function in root.functions:
             self.handle_vertex(root, function)
         root.alter_children(type(self).handle_edge)
@@ -256,18 +251,18 @@
         if node is not None and node.children is not None and len(node.children) > 0:
             node.alter_children(CLIInterfaceBuilder.handle_edge)
 
     def run(self):
         self.tree.root.external_object()
 
 
-def _get_interface_builder(tree, interface_type, root_name, config, return_before_executing):
+def _get_interface_builder(tree, interface_type, return_before_executing):
     builder_name = "{}InterfaceBuilder".format(interface_type.upper())
     if builder_name in globals():
-        builder = globals()[builder_name](tree, root_name, config)
+        builder = globals()[builder_name](tree)
         builder.dfs()
         if return_before_executing:
             return builder.tree.root.external_object
         else:
             builder.run()
     else:
         raise InterfaceNotImplementedError(interface_type)
```

### Comparing `impose-cli-0.3.5/impose_cli/impose_cli.py` & `impose-cli-0.3.6/impose_cli/impose_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ._utils import parse_nodes, _get_interface_builder
-from inspect import stack, getframeinfo, currentframe
+from inspect import stack
 
 
-def impose_cli(target: str = None, launch_type: str = "cli", launch_specific_configs: dict = {},
-               return_before_executing: bool = False, root_name: str = "cli", build_cache: bool = True):
+def impose_cli(target: str = None, launch_type: str = "cli",
+               return_before_executing: bool = False):
     """
     The entrypoint for building a suite of CLI commands / API endpoints.
     :param launch_specific_configs:
     :param target: Can be used to specify the relative path of a directory which will contain all commands / endpoints.
     :param launch_type: CLI or API.
     :param return_before_executing: Return the produced object before executing.
     :param build_cache: If cache should be built. This could be problematic for larger applications.
     :return:
     """
     entry = stack()[1].filename
     tree = parse_nodes(entry, target)
-    return _get_interface_builder(tree, launch_type, root_name, launch_specific_configs, return_before_executing)
+    return _get_interface_builder(tree, launch_type, return_before_executing)
```

