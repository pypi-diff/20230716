# Comparing `tmp/discovery-core-0.2.5.tar.gz` & `tmp/discovery-core-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.5.tar", last modified: Thu Jul 13 23:48:32 2023, max compression
+gzip compressed data, was "discovery-core-0.2.6.tar", last modified: Sun Jul 16 00:03:08 2023, max compression
```

## Comparing `discovery-core-0.2.5.tar` & `discovery-core-0.2.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.066419 discovery-core-0.2.5/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.5/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.5/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-13 23:48:32.066624 discovery-core-0.2.5/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.5/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.047192 discovery-core-0.2.5/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-13 23:48:31.000000 discovery-core-0.2.5/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-13 23:48:31.000000 discovery-core-0.2.5/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-13 23:48:31.000000 discovery-core-0.2.5/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-13 23:48:31.000000 discovery-core-0.2.5/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.047573 discovery-core-0.2.5/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-13 23:40:40.000000 discovery-core-0.2.5/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.050150 discovery-core-0.2.5/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.5/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    22600 2023-07-13 23:44:43.000000 discovery-core-0.2.5/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.052418 discovery-core-0.2.5/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.5/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.5/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.053471 discovery-core-0.2.5/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.5/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.057040 discovery-core-0.2.5/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.5/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.5/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.5/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-13 23:48:32.067397 discovery-core-0.2.5/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.5/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.057971 discovery-core-0.2.5/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.5/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.059752 discovery-core-0.2.5/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.5/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15078 2023-07-13 23:46:04.000000 discovery-core-0.2.5/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.061612 discovery-core-0.2.5/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.5/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.5/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.063325 discovery-core-0.2.5/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.5/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.5/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:48:32.065787 discovery-core-0.2.5/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.5/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.5/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.5/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.929862 discovery-core-0.2.6/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.6/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.6/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-16 00:03:08.930166 discovery-core-0.2.6/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.6/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.908328 discovery-core-0.2.6/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.908677 discovery-core-0.2.6/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-13 23:49:08.000000 discovery-core-0.2.6/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.910804 discovery-core-0.2.6/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.6/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    23605 2023-07-15 23:59:50.000000 discovery-core-0.2.6/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.912785 discovery-core-0.2.6/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.6/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.6/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.913716 discovery-core-0.2.6/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.6/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.917162 discovery-core-0.2.6/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.6/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.6/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.6/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-16 00:03:08.931268 discovery-core-0.2.6/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.6/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.918145 discovery-core-0.2.6/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.6/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.920357 discovery-core-0.2.6/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.6/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15078 2023-07-13 23:46:04.000000 discovery-core-0.2.6/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.923220 discovery-core-0.2.6/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.6/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.6/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.925752 discovery-core-0.2.6/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.6/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.6/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.929010 discovery-core-0.2.6/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.6/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.6/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.5/LICENSE.txt` & `discovery-core-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/PKG-INFO` & `discovery-core-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.5
+Version: 0.2.6
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.5/README.rst` & `discovery-core-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.2.6/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.5
+Version: 0.2.6
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.5/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.2.6/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/ds_core/components/abstract_component.py` & `discovery-core-0.2.6/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/ds_core/components/core_commons.py` & `discovery-core-0.2.6/ds_core/components/core_commons.py`

 * *Files 3% similar despite different names*

```diff
@@ -290,19 +290,26 @@
                     working = True
         return t
 
     @staticmethod
     def table_nest(t: pa.Table) -> list:
         """ turns a flattened table back to a nested pattern """
 
-        def set_dict(tree, vector, value):
-            key = vector[0]
-            tree[key] = value if len(vector) == 1 else set_dict(tree[key] if key in tree else {}, vector[1:], value)
+        def add_leaf(tree, keys, value):
+            key = keys[0]
+            tree[key] = value if len(keys) == 1 else add_leaf(tree[key] if key in tree else {}, keys[1:], value)
             return tree
 
+        def traverse(d, path=[]):
+            if isinstance(d, dict):
+                for (k, v) in d.items():
+                    yield from traverse(v, [*path, k])
+                else:
+                    yield [*path, d]
+
         def set_list(struct, keys, tree):
             for key in tuple(struct.keys()):
                 if isinstance(struct.get(key), dict) and len(struct.get(key)) > 0:
                     keys.append(key)
                     set_list(struct.get(key), keys, tree)
                 if str(key).startswith('nest_list_'):
                     snippet = list([struct.get(key, {})])
@@ -314,23 +321,45 @@
                     snippet = list(struct.values())
                     struct.clear()
                     branch[keys[-1]] = snippet
             if len(keys) > 0:
                 keys.pop()
             return tree
 
-        rtn_lst = []
+        document = []
         for idx in range(t.num_rows):
-            rtn_value = {}
-            for n in t.column_names:
-                values = t.column(n).to_pylist()
-                rtn_value = set_dict(rtn_value, n.split('.'), values[idx])
-            rtn_value = set_list(rtn_value, [], rtn_value)
-            rtn_lst.append(rtn_value)
-        return rtn_lst
+            tree = {}
+            for c in t.column_names:
+                names = c.split('.')
+                # set the branch
+                n = names.pop()
+                branch = {n: t.column(c)[idx].as_py()}
+                _ = (next(traverse(branch)))
+                while names:
+                    n = names.pop()
+                    branch = {n: branch}
+                    _ = (next(traverse(branch)))
+                # branch is correct
+                leaf = branch
+                keys = []
+                sub_leaf = tree
+                while leaf:
+                    key = list(leaf.keys())[0]
+                    keys.append(key)
+                    if key not in sub_leaf.keys():
+                        leaf = leaf.get(key)
+                        break
+                    if tree.keys() is None:
+                        break
+                    leaf = leaf.get(key)
+                    sub_leaf = sub_leaf.get(key)
+                tree = add_leaf(tree, keys, leaf)
+            tree = set_list(tree, [], tree)
+            document.append(tree)
+        return document
 
     @staticmethod
     def column_cast(a: pa.Array, ty: pa.DataType) -> pa.Array:
         """ attempt to cast a pyarrow array to the given type """
         try:
             return a.cast(ty)
         except (ArrowInvalid, ArrowTypeError, ArrowNotImplementedError):
```

### Comparing `discovery-core-0.2.5/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.2.6/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.2.6/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/ds_core/intent/abstract_intent.py` & `discovery-core-0.2.6/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/ds_core/properties/abstract_properties.py` & `discovery-core-0.2.6/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/ds_core/properties/decorator_patterns.py` & `discovery-core-0.2.6/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/ds_core/properties/property_manager.py` & `discovery-core-0.2.6/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/setup.py` & `discovery-core-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/components/abstract_component_test.py` & `discovery-core-0.2.6/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/components/commons_test.py` & `discovery-core-0.2.6/test/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/handlers/connector_contract_test.py` & `discovery-core-0.2.6/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/handlers/handler_factory_test.py` & `discovery-core-0.2.6/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/intent/abstract_intent_test.py` & `discovery-core-0.2.6/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/intent/pyarrow_intent_model.py` & `discovery-core-0.2.6/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.2.6/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.5/test/properties/property_manager_test.py` & `discovery-core-0.2.6/test/properties/property_manager_test.py`

 * *Files identical despite different names*

