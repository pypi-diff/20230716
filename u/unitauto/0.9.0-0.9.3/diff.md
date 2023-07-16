# Comparing `tmp/unitauto-0.9.0.tar.gz` & `tmp/unitauto-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-oje2c6rl/unitauto-0.9.0.tar", last modified: Sat Jun 24 15:58:55 2023, max compression
+gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-kvrcup18/unitauto-0.9.3.tar", last modified: Sat Jun 24 17:24:48 2023, max compression
```

## Comparing `unitauto-0.9.0.tar` & `unitauto-0.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 15:58:41.000000 unitauto-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 15:58:55.000000 unitauto-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-24 15:58:41.000000 unitauto-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 15:58:41.000000 unitauto-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 15:58:55.000000 unitauto-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20666 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/methodutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 17:24:27.000000 unitauto-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 17:24:48.000000 unitauto-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-24 17:24:27.000000 unitauto-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 17:24:27.000000 unitauto-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 17:24:48.000000 unitauto-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21771 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/methodutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-24 17:24:27.000000 unitauto-0.9.3/unitauto/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 17:24:48.000000 unitauto-0.9.3/unitauto.egg-info/top_level.txt
```

### Comparing `unitauto-0.9.0/LICENSE` & `unitauto-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.0/PKG-INFO` & `unitauto-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.9.0
+Version: 0.9.3
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unitauto-0.9.0/README.md` & `unitauto-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.0/setup.cfg` & `unitauto-0.9.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unitauto
-version = 0.9.0
+version = 0.9.3
 author = TommyLemon
 author_email = tommylemon@qq.com
 description = An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TommyLemon/unitauto-py
 classifiers =
```

### Comparing `unitauto-0.9.0/unitauto/methodutil.py` & `unitauto-0.9.3/unitauto/methodutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -347,15 +347,15 @@
     rt = null
     if return_annotation is not None:
         try:
             rt = return_annotation.__name__
         except Exception as e:
             rt = str(return_annotation)
 
-    if rt == '_empty':
+    if rt in ('_empty', 'POSITIONAL_OR_KEYWORD'):
         rt = null
 
     types = []
     for param in signature.parameters.values():
         a = null if param is None else param.annotation
         n = null
         if a is not None:
@@ -368,18 +368,21 @@
 
     names = [param.name for param in signature.parameters.values()]
     static = is_empty(names) or names[0] != 'self'
     name = func.__name__
     return {
         KEY_STATIC: static,
         'returnType': rt,
+        'genericReturnType': rt,
         KEY_METHOD: name,
         KEY_NAME: name,
-        'types': types if static else types[1:],
-        'names': names if static else names[1:]
+        'parameterTypeList': types if static else types[1:],
+        'genericParameterTypeList': types if static else types[1:],
+        'parameterNameList': names if static else names[1:],
+        'parameterDefaultValueList': null
     }
 
 
 def invoke_method(req: any) -> dict:
     start_time = time.time_ns()
     try:
         if is_str(req):
@@ -461,20 +464,45 @@
 
             func = getattr(instance, method)
 
         start_time = time.time_ns()
         result = func(*ma_values)
         time_detail = get_time_detail(start_time)
 
+        signature = inspect.signature(func)
+        return_annotation = null if signature is None else signature.return_annotation
+        rt = null
+        if return_annotation is not None:
+            try:
+                rt = return_annotation.__name__
+                if rt in ('_empty', 'POSITIONAL_OR_KEYWORD'):
+                    rt = type(result).__name__
+            except Exception as e:
+                print(e)
+                rt = type(result).__name__  # str(return_annotation)
+
+        mas = [null] * mal
+        if mal > 0:  # bug 要及时发现 and size(ma_values) == mal:
+            i = -1
+            for v in ma_values:
+                i += 1
+                t = ma_types[i]
+                mas[i] = {
+                    KEY_TYPE: t.__name__ if t is not None else type(v),
+                    KEY_VALUE: v
+                }
+
         return {
             KEY_LANGUAGE: LANGUAGE,
             KEY_OK: true,
             KEY_CODE: CODE_SUCCESS,
             KEY_MSG: MSG_SUCCESS,
+            KEY_TYPE: rt,
             KEY_RETURN: result,
+            KEY_METHOD_ARGS: mas,
             KEY_TIME_DETAIL: time_detail
         }
     except Exception as e:
         return {
             KEY_LANGUAGE: LANGUAGE,
             KEY_OK: false,
             KEY_CODE: CODE_SERVER_ERROR,
```

### Comparing `unitauto-0.9.0/unitauto/server.py` & `unitauto-0.9.3/unitauto/server.py`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.0/unitauto/test/__init__.py` & `unitauto-0.9.3/unitauto/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.0/unitauto/test/testutil.py` & `unitauto-0.9.3/unitauto/test/testutil.py`

 * *Files identical despite different names*

### Comparing `unitauto-0.9.0/unitauto.egg-info/PKG-INFO` & `unitauto-0.9.3/unitauto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.9.0
+Version: 0.9.3
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

