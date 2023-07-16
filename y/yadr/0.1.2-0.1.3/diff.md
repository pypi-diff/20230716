# Comparing `tmp/yadr-0.1.2.tar.gz` & `tmp/yadr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadr-0.1.2.tar", last modified: Sat Apr 15 23:19:14 2023, max compression
+gzip compressed data, was "yadr-0.1.3.tar", last modified: Sun Jul 16 15:24:52 2023, max compression
```

## Comparing `yadr-0.1.2.tar` & `yadr-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.911226 yadr-0.1.2/
--rw-r--r--   0 pji        (501) staff       (20)     1069 2021-11-15 07:15:50.000000 yadr-0.1.2/LICENSE
--rw-r--r--   0 pji        (501) staff       (20)     4177 2023-04-15 23:19:14.911427 yadr-0.1.2/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     3703 2023-04-12 13:04:13.000000 yadr-0.1.2/README.rst
--rw-r--r--   0 pji        (501) staff       (20)       90 2021-12-01 13:26:36.000000 yadr-0.1.2/pyproject.toml
--rw-r--r--   0 pji        (501) staff       (20)      812 2023-04-15 23:19:14.912532 yadr-0.1.2/setup.cfg
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.903863 yadr-0.1.2/tests/
--rw-r--r--   0 pji        (501) staff       (20)     1524 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_encoder.py
--rw-r--r--   0 pji        (501) staff       (20)    26052 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_lex.py
--rw-r--r--   0 pji        (501) staff       (20)     8452 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_maps.py
--rw-r--r--   0 pji        (501) staff       (20)    10646 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_operator.py
--rw-r--r--   0 pji        (501) staff       (20)    19434 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_parser.py
--rw-r--r--   0 pji        (501) staff       (20)     3717 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_yadr.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.899067 yadr-0.1.2/yadr/
--rw-r--r--   0 pji        (501) staff       (20)      128 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/__init__.py
--rw-r--r--   0 pji        (501) staff       (20)      163 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/__main__.py
--rw-r--r--   0 pji        (501) staff       (20)    17602 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/base.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.899588 yadr-0.1.2/yadr/data/
--rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-30 15:19:28.000000 yadr-0.1.2/yadr/data/__init__.py
--rw-r--r--   0 pji        (501) staff       (20)      904 2021-11-30 13:16:10.000000 yadr-0.1.2/yadr/data/dice_maps.yadn
--rw-r--r--   0 pji        (501) staff       (20)     1688 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/encode.py
--rw-r--r--   0 pji        (501) staff       (20)    11664 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/lex.py
--rw-r--r--   0 pji        (501) staff       (20)     7743 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/maps.py
--rw-r--r--   0 pji        (501) staff       (20)     3586 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/model.py
--rw-r--r--   0 pji        (501) staff       (20)     6784 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/operator.py
--rw-r--r--   0 pji        (501) staff       (20)    13348 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/parser.py
--rw-r--r--   0 pji        (501) staff       (20)     3587 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/pools.py
--rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-31 13:18:36.000000 yadr-0.1.2/yadr/py.typed
--rw-r--r--   0 pji        (501) staff       (20)     5460 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/yadr.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.910709 yadr-0.1.2/yadr.egg-info/
--rw-r--r--   0 pji        (501) staff       (20)     4177 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)      553 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/SOURCES.txt
--rw-r--r--   0 pji        (501) staff       (20)        1 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/dependency_links.txt
--rw-r--r--   0 pji        (501) staff       (20)        1 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/not-zip-safe
--rw-r--r--   0 pji        (501) staff       (20)        5 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/top_level.txt
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-07-16 15:24:52.126561 yadr-0.1.3/
+-rw-r--r--   0 pji        (501) staff       (20)     1069 2021-11-15 07:15:50.000000 yadr-0.1.3/LICENSE
+-rw-r--r--   0 pji        (501) staff       (20)     4177 2023-07-16 15:24:52.126704 yadr-0.1.3/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     3703 2023-04-15 23:35:36.000000 yadr-0.1.3/README.rst
+-rw-r--r--   0 pji        (501) staff       (20)       90 2021-12-01 13:26:36.000000 yadr-0.1.3/pyproject.toml
+-rw-r--r--   0 pji        (501) staff       (20)      827 2023-07-16 15:24:52.127355 yadr-0.1.3/setup.cfg
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-07-16 15:24:52.124066 yadr-0.1.3/tests/
+-rw-r--r--   0 pji        (501) staff       (20)     1524 2023-07-16 15:22:55.000000 yadr-0.1.3/tests/test_encoder.py
+-rw-r--r--   0 pji        (501) staff       (20)    26052 2023-07-16 15:22:55.000000 yadr-0.1.3/tests/test_lex.py
+-rw-r--r--   0 pji        (501) staff       (20)     8452 2023-07-16 15:22:55.000000 yadr-0.1.3/tests/test_maps.py
+-rw-r--r--   0 pji        (501) staff       (20)    10646 2023-07-16 15:22:55.000000 yadr-0.1.3/tests/test_operator.py
+-rw-r--r--   0 pji        (501) staff       (20)    19434 2023-07-16 15:22:55.000000 yadr-0.1.3/tests/test_parser.py
+-rw-r--r--   0 pji        (501) staff       (20)     3717 2023-07-16 15:22:55.000000 yadr-0.1.3/tests/test_yadr.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-07-16 15:24:52.118112 yadr-0.1.3/yadr/
+-rw-r--r--   0 pji        (501) staff       (20)      128 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/__init__.py
+-rw-r--r--   0 pji        (501) staff       (20)      163 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/__main__.py
+-rw-r--r--   0 pji        (501) staff       (20)    17602 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/base.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-07-16 15:24:52.118993 yadr-0.1.3/yadr/data/
+-rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-30 15:19:28.000000 yadr-0.1.3/yadr/data/__init__.py
+-rw-r--r--   0 pji        (501) staff       (20)      904 2021-11-30 13:16:10.000000 yadr-0.1.3/yadr/data/dice_maps.yadn
+-rw-r--r--   0 pji        (501) staff       (20)     1688 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/encode.py
+-rw-r--r--   0 pji        (501) staff       (20)    11664 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/lex.py
+-rw-r--r--   0 pji        (501) staff       (20)     7743 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/maps.py
+-rw-r--r--   0 pji        (501) staff       (20)     3586 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/model.py
+-rw-r--r--   0 pji        (501) staff       (20)    16360 2023-07-16 15:23:56.000000 yadr-0.1.3/yadr/operator.py
+-rw-r--r--   0 pji        (501) staff       (20)    14054 2023-07-16 15:23:56.000000 yadr-0.1.3/yadr/parser.py
+-rw-r--r--   0 pji        (501) staff       (20)     3587 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/pools.py
+-rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-31 13:18:36.000000 yadr-0.1.3/yadr/py.typed
+-rw-r--r--   0 pji        (501) staff       (20)     5460 2023-07-16 15:22:55.000000 yadr-0.1.3/yadr/yadr.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-07-16 15:24:52.126328 yadr-0.1.3/yadr.egg-info/
+-rw-r--r--   0 pji        (501) staff       (20)     4177 2023-07-16 15:24:52.000000 yadr-0.1.3/yadr.egg-info/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)      553 2023-07-16 15:24:52.000000 yadr-0.1.3/yadr.egg-info/SOURCES.txt
+-rw-r--r--   0 pji        (501) staff       (20)        1 2023-07-16 15:24:52.000000 yadr-0.1.3/yadr.egg-info/dependency_links.txt
+-rw-r--r--   0 pji        (501) staff       (20)        1 2023-07-16 15:24:51.000000 yadr-0.1.3/yadr.egg-info/not-zip-safe
+-rw-r--r--   0 pji        (501) staff       (20)        5 2023-07-16 15:24:52.000000 yadr-0.1.3/yadr.egg-info/top_level.txt
```

### Comparing `yadr-0.1.2/LICENSE` & `yadr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/PKG-INFO` & `yadr-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Yet another dice roller for Python.
 Home-page: https://github.com/pji/yadr
 Author: Paul J. Iutzi
 Author-email: pji@mac.com
 Project-URL: Bug Tracker, https://github.com/pji/yadr/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yadr-0.1.2/README.rst` & `yadr-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/setup.cfg` & `yadr-0.1.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [pycodestyle]
 quiet = 1
 ignore = E231,W503
 
 [precommit]
 doctest_modules = yadr.yadr
+	yadr.operator
 python_files = *
 	yadr/*
 	examples/*
 	tests/*
 rst_files = *
 	docs/*
 unit_tests = tests
 
 [metadata]
 name = yadr
-version = 0.1.2
+version = 0.1.3
 author = Paul J. Iutzi
 author_email = pji@mac.com
 description = Yet another dice roller for Python.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pji/yadr
 project_urls =
```

### Comparing `yadr-0.1.2/tests/test_encoder.py` & `yadr-0.1.3/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/tests/test_lex.py` & `yadr-0.1.3/tests/test_lex.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/tests/test_maps.py` & `yadr-0.1.3/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/tests/test_operator.py` & `yadr-0.1.3/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/tests/test_parser.py` & `yadr-0.1.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/tests/test_yadr.py` & `yadr-0.1.3/tests/test_yadr.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/base.py` & `yadr-0.1.3/yadr/base.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/data/dice_maps.yadn` & `yadr-0.1.3/yadr/data/dice_maps.yadn`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/encode.py` & `yadr-0.1.3/yadr/encode.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/lex.py` & `yadr-0.1.3/yadr/lex.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/maps.py` & `yadr-0.1.3/yadr/maps.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/model.py` & `yadr-0.1.3/yadr/model.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/parser.py` & `yadr-0.1.3/yadr/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,20 +121,21 @@
 
         # Compute the value of the tokens that are higher in the
         # order of operations than this tree and on the right-side
         # of this expression.
         right = self.right.compute()
 
         # Determine the operation to run.
-        yo.ops_by_symbol['m'] = self._map_result
         try:
-            op = yo.ops_by_symbol[self.value]
-        except IndexError:
-            msg = f'Operator not recognized: {self.value}.'
-            raise ValueError(msg)
+            op = yo.ops[self.value]
+        except KeyError:
+            if self.value != 'm':
+                msg = f'Operator not recognized: {self.value}.'
+                raise ValueError(msg)
+            op = self._map_result
 
         # Perform the operation on the left and right values,
         # returning the result.
         return op(left, right)
 
     def _map_result(
         self, result: int | tuple[int, ...],
@@ -183,23 +184,54 @@
             return self.value
 
         # Compute the result of any children.
         child = self.child.compute()
 
         # Determine the operation to perform.
         if self.kind in op_tokens:
-            op = yo.ops_by_symbol[self.value]
+            op = yo.ops[self.value]
 
         # Perform the operation and return the result.
         return op(child)
 
 
 # Parser class.
 class Parser:
-    """A state machine for parsing :ref:`YADN`."""
+    """A state machine for parsing :ref:`YADN`.
+
+    How Parsing Works
+    =================
+    Essentially, parsing turns an ordered list of tokens into a
+    tree structure for execution. For example, let's say we have
+    the :ref:`YADN` expression::
+
+        3 * ( 4 - 2 )
+
+    That is lexed into the tokens::
+
+        Token(NUMBER, 3)
+        Token(MD_OPERATOR, '*')
+        Token(GROUP_OPEN, '(')
+        Token(NUMBER, 4)
+        Token(AS_OPERATOR, '-')
+        Token(NUMBER, 2)
+        Token(GROUP_CLOSE, ')')
+
+    Which is then parsed into the tree::
+
+            *
+           / \\
+          -   3
+         / \\
+        4   2
+
+    Where each token ends up in each tree is dependent on the
+    :ref:`ops_order` defined by :ref:`YADN`.
+
+    """
     def __init__(self) -> None:
         self.dice_map: dict[str, DiceMapping] = dict()
         self.top_rule = self._map_operator
 
     # Public method.
     def parse(
         self,
```

### Comparing `yadr-0.1.2/yadr/pools.py` & `yadr-0.1.3/yadr/pools.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr/yadr.py` & `yadr-0.1.3/yadr/yadr.py`

 * *Files identical despite different names*

### Comparing `yadr-0.1.2/yadr.egg-info/PKG-INFO` & `yadr-0.1.3/yadr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Yet another dice roller for Python.
 Home-page: https://github.com/pji/yadr
 Author: Paul J. Iutzi
 Author-email: pji@mac.com
 Project-URL: Bug Tracker, https://github.com/pji/yadr/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yadr-0.1.2/yadr.egg-info/SOURCES.txt` & `yadr-0.1.3/yadr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

