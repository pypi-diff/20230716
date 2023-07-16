# Comparing `tmp/Numkdoc-0.4.1.tar.gz` & `tmp/Numkdoc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Numkdoc-0.4.1.tar", last modified: Mon Feb  7 23:30:22 2022, max compression
+gzip compressed data, was "Numkdoc-0.4.2.tar", last modified: Sun Jul 16 21:21:32 2023, max compression
```

## Comparing `Numkdoc-0.4.1.tar` & `Numkdoc-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 23:30:22.198674 Numkdoc-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-02-07 23:30:13.000000 Numkdoc-0.4.1/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 23:30:22.194674 Numkdoc-0.4.1/Numkdoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-02-07 23:30:22.000000 Numkdoc-0.4.1/Numkdoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-02-07 23:30:22.000000 Numkdoc-0.4.1/Numkdoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 23:30:22.000000 Numkdoc-0.4.1/Numkdoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-02-07 23:30:22.000000 Numkdoc-0.4.1/Numkdoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-07 23:30:22.000000 Numkdoc-0.4.1/Numkdoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-07 23:30:22.000000 Numkdoc-0.4.1/Numkdoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-02-07 23:30:22.198674 Numkdoc-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-02-07 23:30:13.000000 Numkdoc-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 23:30:22.198674 Numkdoc-0.4.1/numkdoc/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-02-07 23:30:13.000000 Numkdoc-0.4.1/numkdoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-02-07 23:30:13.000000 Numkdoc-0.4.1/numkdoc/numkdoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6664 2022-02-07 23:30:13.000000 Numkdoc-0.4.1/numkdoc/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-02-07 23:30:13.000000 Numkdoc-0.4.1/numkdoc/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-02-07 23:30:22.198674 Numkdoc-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-02-07 23:30:13.000000 Numkdoc-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:32.354642 Numkdoc-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 21:21:16.000000 Numkdoc-0.4.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:32.354642 Numkdoc-0.4.2/Numkdoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-16 21:21:32.000000 Numkdoc-0.4.2/Numkdoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-16 21:21:32.000000 Numkdoc-0.4.2/Numkdoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:21:32.000000 Numkdoc-0.4.2/Numkdoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-16 21:21:32.000000 Numkdoc-0.4.2/Numkdoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 21:21:32.000000 Numkdoc-0.4.2/Numkdoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 21:21:32.000000 Numkdoc-0.4.2/Numkdoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-16 21:21:32.354642 Numkdoc-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-16 21:21:16.000000 Numkdoc-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:32.354642 Numkdoc-0.4.2/numkdoc/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 21:21:16.000000 Numkdoc-0.4.2/numkdoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-16 21:21:16.000000 Numkdoc-0.4.2/numkdoc/numkdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-16 21:21:16.000000 Numkdoc-0.4.2/numkdoc/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-16 21:21:16.000000 Numkdoc-0.4.2/numkdoc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-16 21:21:32.358642 Numkdoc-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-16 21:21:16.000000 Numkdoc-0.4.2/setup.py
```

### Comparing `Numkdoc-0.4.1/LICENSE.txt` & `Numkdoc-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Numkdoc-0.4.1/Numkdoc.egg-info/PKG-INFO` & `Numkdoc-0.4.2/Numkdoc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: Numkdoc
-Version: 0.4.1
+Version: 0.4.2
 Summary: Mkdoc plugin to autodoc your numpy docstring
 Home-page: https://github.com/napolar/numkdoc
 Author: Thomas FEL
 Author-email: thomas.fel@protonmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -55,9 +54,7 @@
 
 [...]
 
 {{ src.module.Class }}
 
 [...]
 ```
-
-
```

### Comparing `Numkdoc-0.4.1/PKG-INFO` & `Numkdoc-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: Numkdoc
-Version: 0.4.1
+Version: 0.4.2
 Summary: Mkdoc plugin to autodoc your numpy docstring
 Home-page: https://github.com/napolar/numkdoc
 Author: Thomas FEL
 Author-email: thomas.fel@protonmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -55,9 +54,7 @@
 
 [...]
 
 {{ src.module.Class }}
 
 [...]
 ```
-
-
```

### Comparing `Numkdoc-0.4.1/README.md` & `Numkdoc-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `Numkdoc-0.4.1/numkdoc/numkdoc.py` & `Numkdoc-0.4.2/numkdoc/numkdoc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 from numkdoc.utils import REPLACES
-import os
 import re
 import inspect
 from importlib import import_module
 
 from mkdocs.plugins import BasePlugin
 
-from .parser import parse_class
+from .parser import parse_class, parse_method
 
 
 class Numkdoc(BasePlugin):
     # caching classes to markdown for fast hot_reload
-    _cache = {}
+    _class_cache = {}
+    _function_cache = {}
 
     def on_page_markdown(self, markdown, **kwargs):
         """hook triggering before converting markdown to html"""
 
-        # get the current directory
-        cwd = os.getcwd()
-
         # check the documentation for all the call to a class
         # e.g {{ module.submodule.ClassName }} will render the document of 'ClassName'
         classes_to_load = re.findall('{{(.+?)}}', markdown)
 
         # sanity check
         if len(classes_to_load) == 0:
             return markdown
 
         for class_string in classes_to_load:
             directory = class_string.split('.')[:-1]
             class_name = class_string.split('.')[-1]
 
-            if class_name not in self._cache:
+            if class_name not in self._class_cache and class_name not in self._function_cache:
                 # loading the module
                 try:
                     module = import_module(str.join('.', directory))
                 except:
                     raise ValueError(f"Cant load module {class_string}.")
 
                 # parse and store all the classes in the module
                 for name, data in inspect.getmembers(module, inspect.isclass):
-                    if name not in self._cache:
+                    if name not in self._class_cache:
                         document = parse_class(data)
                         for old, new in REPLACES:
                             document = document.replace(old, new)
-                        self._cache[name] = document
-                        
-            # replace the call with the documentation of the class            
-            markdown = markdown.replace(
-                "{{"+class_string+"}}", self._cache[class_name])
+                        self._class_cache[name] = document
+
+                # parse and store all the functions in the module
+                for name, data in inspect.getmembers(module, inspect.isfunction):
+                    if name not in self._function_cache:
+                        print('trying to parse function', name, 'with data', data)
+                        document = parse_method(data)
+                        for old, new in REPLACES:
+                            document = document.replace(old, new)
+                        self._function_cache[name] = document
+
+            # replace the call with the documentation of the class
+            if class_name in self._class_cache:
+                markdown = markdown.replace(
+                    "{{"+class_string+"}}", self._class_cache[class_name])
+            elif class_name in self._function_cache:
+                markdown = markdown.replace(
+                    "{{"+class_string+"}}", self._function_cache[class_name])
+            else:
+                raise ValueError(f"Class {class_string} not found.")
 
         return markdown
```

### Comparing `Numkdoc-0.4.1/numkdoc/parser.py` & `Numkdoc-0.4.2/numkdoc/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,31 +87,31 @@
     markdown = ""
 
     try:
         # sanity check
         method_name = method.__name__
         method_name = "\_\_init__" if method_name == '__init__' else method_name
 
-        signature = f"{method_name}" 
+        signature = f"{method_name}"
         parameters = str(inspect.signature(method))
         first_line_padding = len(method_name.replace('\\', ''))
 
         accumulator = ""
         for p_id, p in enumerate(re.split(r',(?![^\[]*[\]])', parameters)):
             if p_id > 0 and (('[' in p and ']' not in p) or ('(' in p and ')' not in p)):
                 accumulator += p + ","
                 continue
-            
+
             line = parameter_signature(accumulator + p)
             padding = WHITE_SPACE*first_line_padding if p_id > 0 else ""
             signature += padding + line + ",<br>"
             accumulator = ""
         signature = signature[:-5]
 
-        markdown += f"{heading(CLASS_METHOD_HEADING, signature, method_name)} {lb} {lb}"     
+        markdown += f"{heading(CLASS_METHOD_HEADING, signature, method_name)} {lb} {lb}"
     except:
         raise
         warnings.warn(f"No Signature found for method {method}.")
 
     return markdown
 
 
@@ -129,15 +129,15 @@
     # keeps the line break in the documentation only when there is a period before
     line = "<p>"
     for chunk in param.desc:
         if line[-1] != '.':
             line += f" {chunk}"
         else:
             line += f"</p><p> {chunk}"
-    
+
     line += "</p>"
 
     return line
 
 
 def parse_parameters(doc, method=None):
     markdown = ""
@@ -181,44 +181,50 @@
                 if '->' in str(signature):
                     ret_type = str(signature).split('->')[-1].strip()
                     ret = ret._replace(type = ret_type)
 
             markdown += parameter_line(ret)
 
     except:
-        raise
         warnings.warn(f"No return found for {doc._f.__name__}.")
 
     return markdown
 
 
+def parse_method(method):
+    markdown = ""
+    # check if the func is wrapped (decorator)
+    if hasattr(method, "__closure__") and method.__closure__ is not None:
+        wrapped_method = extract_wrapped(method)
+        method = method if wrapped_method is None else wrapped_method
+
+    method_doc = FunctionDoc(method)
+    markdown += parse_signature(method)
+    markdown += parse_summary(method_doc)
+    markdown += parse_parameters(method_doc, method)
+    markdown += parse_returns(method_doc, method)
+    markdown += flb
+
+    return markdown
+
+
 def parse_methods(class_object, doc):
     markdown = ""
 
     # avoid private and builtin methods
     methods = [m for m in dir(class_object) if should_parse_method(class_object, m)]
-    
+
     # sanity check
     if len(methods) > 0:
         markdown += f"{lb * 2}"
 
         for method_key in methods:
             try:
                 method = getattr(class_object, method_key)
-
-                # check if the func is wrapped (decorator)
-                if hasattr(method, "__closure__") and method.__closure__ is not None:
-                    wrapped_method = extract_wrapped(method)
-                    method = method if wrapped_method is None else wrapped_method
-
-                method_doc = FunctionDoc(method)
-                markdown += parse_signature(method)
-                markdown += parse_summary(method_doc)
-                markdown += parse_parameters(method_doc, method)
-                markdown += parse_returns(method_doc, method)
-                markdown += flb
+                markdown += parse_method(method)
             except:
-                raise
                 warnings.warn(
                     f"Skip parsing method {class_object.__name__}.{method}.")
 
     return markdown
+
+
```

### Comparing `Numkdoc-0.4.1/numkdoc/utils.py` & `Numkdoc-0.4.2/numkdoc/utils.py`

 * *Files identical despite different names*

### Comparing `Numkdoc-0.4.1/setup.py` & `Numkdoc-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 
 setup(
     name='Numkdoc',
     packages=['numkdoc'],
-    version='0.4.1',
+    version='0.4.2',
     license='MIT',
 
     description='Mkdoc plugin to autodoc your numpy docstring',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
 
     author='Thomas FEL',
```

