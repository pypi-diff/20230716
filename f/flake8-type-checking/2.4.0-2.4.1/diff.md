# Comparing `tmp/flake8_type_checking-2.4.0.tar.gz` & `tmp/flake8_type_checking-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_type_checking-2.4.0.tar", max compression
+gzip compressed data, was "flake8_type_checking-2.4.1.tar", max compression
```

## Comparing `flake8_type_checking-2.4.0.tar` & `flake8_type_checking-2.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1520 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/LICENSE
--rw-r--r--   0        0        0    12763 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/README.md
--rw-r--r--   0        0        0        0 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/flake8_type_checking/__init__.py
--rw-r--r--   0        0        0    43847 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/flake8_type_checking/checker.py
--rw-r--r--   0        0        0     1274 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/flake8_type_checking/constants.py
--rw-r--r--   0        0        0     5279 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/flake8_type_checking/plugin.py
--rw-r--r--   0        0        0        0 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/flake8_type_checking/py.typed
--rw-r--r--   0        0        0      621 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/flake8_type_checking/types.py
--rw-r--r--   0        0        0     2009 2023-03-28 07:09:04.489580 flake8_type_checking-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    14269 1970-01-01 00:00:00.000000 flake8_type_checking-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/LICENSE
+-rw-r--r--   0        0        0    12763 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/flake8_type_checking/__init__.py
+-rw-r--r--   0        0        0    45082 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/flake8_type_checking/checker.py
+-rw-r--r--   0        0        0     1274 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/flake8_type_checking/constants.py
+-rw-r--r--   0        0        0     5279 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/flake8_type_checking/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/flake8_type_checking/py.typed
+-rw-r--r--   0        0        0      621 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/flake8_type_checking/types.py
+-rw-r--r--   0        0        0     2009 2023-07-16 09:07:18.560279 flake8_type_checking-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0    14067 1970-01-01 00:00:00.000000 flake8_type_checking-2.4.1/PKG-INFO
```

### Comparing `flake8_type_checking-2.4.0/LICENSE` & `flake8_type_checking-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.4.0/README.md` & `flake8_type_checking-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.4.0/flake8_type_checking/checker.py` & `flake8_type_checking-2.4.1/flake8_type_checking/checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -481,14 +481,47 @@
             and (node.id == 'TYPE_CHECKING')
             # True for `typing.TYPE_CHECKING` or `T.TYPE_CHECKING`
             or (hasattr(node, 'attr') and node.attr == 'TYPE_CHECKING')
             # True for `from typing import TYPE_CHECKING as TC\nTC`
             or (self.type_checking_alias is not None and hasattr(node, 'id') and (node.id == self.type_checking_alias))
         )
 
+    def is_type_checking_true(self, node: ast.Compare) -> bool:
+        """
+        Check whether the node matches `if TYPE_CHECKING is True`.
+
+        An ast.Compare node has a `left`, `ops`, and `comparators` attribute.
+
+        Here we want to check whether our node corresponds to
+
+            `if TYPE_CHECKING is True`
+                    ^         ^    ^
+        left _______|        ops   |____ comparators
+        """
+        # Left side should be a TYPE_CHECKING block
+        is_type_checking_block = hasattr(node, 'left') and self.is_type_checking(node.left)
+        if not is_type_checking_block:
+            return False
+
+        # Operator should be `is`
+        operator_is_is = len(node.ops) == 1 and isinstance(node.ops[0], ast.Is)
+        if not operator_is_is:
+            return False
+
+        # Right side should be `True`
+        right_side_is_true = (
+            len(node.comparators) == 1
+            and isinstance(node.comparators[0], ast.Constant)
+            and node.comparators[0].value is True
+        )
+        if not right_side_is_true:
+            return False
+
+        return True
+
     def is_true_when_type_checking(self, node: ast.AST) -> bool | Literal['TYPE_CHECKING']:
         """Determine if the node evaluates to True when TYPE_CHECKING is True.
 
         This handles simple boolean logic where the values can be statically determined.
         If a value is dynamic (e.g. a reference or a function call) we assume it may be False.
 
         Returns True if the statement is always True,
@@ -511,14 +544,16 @@
                 return 'TYPE_CHECKING' if has_type_checking else any_others_true
             elif isinstance(node.op, ast.And) and all_others_true:
                 # At least one of the conditions must be TYPE_CHECKING, and all others must be True
                 return 'TYPE_CHECKING' if has_type_checking else False
         elif isinstance(node, ast.Constant):
             with suppress(Exception):
                 return bool(literal_eval(node))
+        elif isinstance(node, ast.Compare) and self.is_type_checking_true(node):
+            return 'TYPE_CHECKING'
         return False
 
     def visit_If(self, node: ast.If) -> Any:
         """Look for a TYPE_CHECKING block."""
         type_checking_condition = self.is_true_when_type_checking(node.test) == 'TYPE_CHECKING'
 
         # If it is, note down the line-number-range where the type-checking block exists
```

### Comparing `flake8_type_checking-2.4.0/flake8_type_checking/constants.py` & `flake8_type_checking-2.4.1/flake8_type_checking/constants.py`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.4.0/flake8_type_checking/plugin.py` & `flake8_type_checking-2.4.1/flake8_type_checking/plugin.py`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.4.0/flake8_type_checking/types.py` & `flake8_type_checking-2.4.1/flake8_type_checking/types.py`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.4.0/pyproject.toml` & `flake8_type_checking-2.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'flake8-type-checking'
-version = "2.4.0"
+version = "2.4.1"
 description = 'A flake8 plugin for managing type-checking imports & forward references'
 homepage = 'https://github.com/snok'
 repository = 'https://github.com/snok/flake8-type-checking'
 authors = ['Sondre Lillebø Gundersen <sondrelg@live.no>']
 license = 'BSD-3-Clause'
 readme = 'README.md'
 keywords = ['flake8', 'plugin', 'linting', 'type hint', 'typing', 'imports']
```

### Comparing `flake8_type_checking-2.4.0/PKG-INFO` & `flake8_type_checking-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-type-checking
-Version: 2.4.0
+Version: 2.4.1
 Summary: A flake8 plugin for managing type-checking imports & forward references
 Home-page: https://github.com/snok
 License: BSD-3-Clause
 Keywords: flake8,plugin,linting,type hint,typing,imports
 Author: Sondre Lillebø Gundersen
 Author-email: sondrelg@live.no
 Requires-Python: >=3.8
@@ -15,19 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Dist: astor ; python_version < "3.9"
 Requires-Dist: classify-imports
 Requires-Dist: flake8
 Project-URL: Repository, https://github.com/snok/flake8-type-checking
 Project-URL: Releases, https://github.com/snok/flake8-type-checking/releases
```

