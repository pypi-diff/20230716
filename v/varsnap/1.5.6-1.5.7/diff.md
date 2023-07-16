# Comparing `tmp/varsnap-1.5.6.tar.gz` & `tmp/varsnap-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varsnap-1.5.6.tar", last modified: Fri Mar 31 06:44:58 2023, max compression
+gzip compressed data, was "varsnap-1.5.7.tar", last modified: Sun Jul 16 06:48:59 2023, max compression
```

## Comparing `varsnap-1.5.6.tar` & `varsnap-1.5.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 06:44:58.830414 varsnap-1.5.6/
--rw-r--r--   0 root         (0) root         (0)     6938 2023-03-31 06:43:53.000000 varsnap-1.5.6/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-31 06:43:53.000000 varsnap-1.5.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3068 2023-03-31 06:44:58.830414 varsnap-1.5.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2337 2023-03-31 06:43:53.000000 varsnap-1.5.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 06:44:58.830414 varsnap-1.5.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-03-31 06:43:53.000000 varsnap-1.5.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 06:44:58.830414 varsnap-1.5.6/varsnap/
--rw-r--r--   0 root         (0) root         (0)      132 2023-03-31 06:43:53.000000 varsnap-1.5.6/varsnap/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-31 06:43:53.000000 varsnap-1.5.6/varsnap/__version__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-03-31 06:43:53.000000 varsnap-1.5.6/varsnap/assert_generator.py
--rw-r--r--   0 root         (0) root         (0)    16216 2023-03-31 06:43:53.000000 varsnap-1.5.6/varsnap/core.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 06:43:53.000000 varsnap-1.5.6/varsnap/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 06:44:58.830414 varsnap-1.5.6/varsnap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3068 2023-03-31 06:44:58.000000 varsnap-1.5.6/varsnap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2023-03-31 06:44:58.000000 varsnap-1.5.6/varsnap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 06:44:58.000000 varsnap-1.5.6/varsnap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 06:44:58.000000 varsnap-1.5.6/varsnap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-31 06:44:58.000000 varsnap-1.5.6/varsnap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 06:48:59.868223 varsnap-1.5.7/
+-rw-r--r--   0 root         (0) root         (0)     7078 2023-07-16 06:48:21.000000 varsnap-1.5.7/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-16 06:48:21.000000 varsnap-1.5.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3068 2023-07-16 06:48:59.868223 varsnap-1.5.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-16 06:48:21.000000 varsnap-1.5.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-07-16 06:48:21.000000 varsnap-1.5.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 06:48:59.868223 varsnap-1.5.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-07-16 06:48:21.000000 varsnap-1.5.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 06:48:59.868223 varsnap-1.5.7/varsnap/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-16 06:48:21.000000 varsnap-1.5.7/varsnap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-16 06:48:21.000000 varsnap-1.5.7/varsnap/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-07-16 06:48:21.000000 varsnap-1.5.7/varsnap/assert_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16239 2023-07-16 06:48:21.000000 varsnap-1.5.7/varsnap/core.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-16 06:48:21.000000 varsnap-1.5.7/varsnap/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 06:48:59.868223 varsnap-1.5.7/varsnap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3068 2023-07-16 06:48:59.000000 varsnap-1.5.7/varsnap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-16 06:48:59.000000 varsnap-1.5.7/varsnap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 06:48:59.000000 varsnap-1.5.7/varsnap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 06:48:59.000000 varsnap-1.5.7/varsnap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-16 06:48:59.000000 varsnap-1.5.7/varsnap.egg-info/top_level.txt
```

### Comparing `varsnap-1.5.6/CHANGELOG.md` & `varsnap-1.5.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+1.5.7 (2023-07-15)
+------------------
+
+ - Mior code cleanup
+ - Update dependencies
+ - Switch from flake8 to ruff
+ - Set up pyproject.toml
+
+
 1.5.6 (2023-03-30)
 ------------------
 
  - Update dependencies
  - Update CI
```

### Comparing `varsnap-1.5.6/PKG-INFO` & `varsnap-1.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varsnap
-Version: 1.5.6
+Version: 1.5.7
 Summary: Varsnap
 Home-page: https://www.varsnap.com/
 Author: Varsnap
 Author-email: admin@varsnap.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `varsnap-1.5.6/README.md` & `varsnap-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `varsnap-1.5.6/setup.py` & `varsnap-1.5.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,14 +55,12 @@
     install_requires=[
         'requests>=2.0,<3.0',
         'dill>=0.3.1.1,<0.4.0',
     ],
 
     test_suite="varsnap.tests",
 
-    # testing requires flake8 and coverage but they're listed separately
-    # because they need to wrap setup.py
     extras_require={
         'dev': [],
         'test': [],
     },
 )
```

### Comparing `varsnap-1.5.6/varsnap/assert_generator.py` & `varsnap-1.5.7/varsnap/assert_generator.py`

 * *Files identical despite different names*

### Comparing `varsnap-1.5.6/varsnap/core.py` & `varsnap-1.5.7/varsnap/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         ]
     ) -> str:
         data = Producer.normalize_data(data)
         try:
             pickle_data = pickle.dumps(data)
         except Exception as e:
             if type(e) in PICKLE_ERRORS:
-                raise SerializeError(e)
+                raise SerializeError(e) from e
             raise
         serialized_data = base64.b64encode(pickle_data).decode('utf-8')
         return serialized_data
 
     @staticmethod
     def serialize_formatted(
         data: Union[
@@ -313,15 +313,15 @@
     @staticmethod
     def deserialize(data: str) -> Any:
         decoded_data = base64.b64decode(data.encode('utf-8'))
         try:
             deserialized_data = pickle.loads(decoded_data)
         except Exception as e:
             if type(e) in UNPICKLE_ERRORS:
-                raise DeserializeError(e)
+                raise DeserializeError(e) from e
             raise
         return deserialized_data
 
     def consume(self, trial_group: TrialGroup) -> list[Trial]:
         if not Consumer.is_enabled():
             return []
         data = {
@@ -476,20 +476,20 @@
         if exception:
             report.append(('Local exception:', limit_string(exception)))
         report.append(('Matching outputs:', str(matches)))
         return report
 
 
 def varsnap(
-    orig_func: Union[TargetFunction, staticmethod[Any]]
+    orig_func: Union[TargetFunction, staticmethod[Any, Any]]
 ) -> TargetFunction:
     try:
         # Have this operate on the actual function in case it is wrapping a
         # staticmethod object
-        func = getattr(orig_func, '__func__')
+        func = orig_func.__func__  # type: ignore
     except AttributeError:
         func = orig_func
 
     producer = Producer(func)
     Consumer(func)
 
     def magic(*args: Any, **kwargs: Any) -> Any:
```

### Comparing `varsnap-1.5.6/varsnap.egg-info/PKG-INFO` & `varsnap-1.5.7/varsnap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varsnap
-Version: 1.5.6
+Version: 1.5.7
 Summary: Varsnap
 Home-page: https://www.varsnap.com/
 Author: Varsnap
 Author-email: admin@varsnap.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

