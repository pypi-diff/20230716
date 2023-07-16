# Comparing `tmp/sigils-0.3.2.tar.gz` & `tmp/sigils-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigils-0.3.2.tar", last modified: Sun Jul 16 05:37:29 2023, max compression
+gzip compressed data, was "sigils-0.3.3.tar", last modified: Sun Jul 16 06:05:23 2023, max compression
```

## Comparing `sigils-0.3.2.tar` & `sigils-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 05:37:29.059391 sigils-0.3.2/
--rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.2/.gitignore
--rw-rw-rw-   0        0        0     1001 2023-07-16 02:58:04.000000 sigils-0.3.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1084 2023-07-16 05:32:45.000000 sigils-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-07-16 05:37:29.056388 sigils-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2417 2023-07-16 05:35:04.000000 sigils-0.3.2/README.rst
--rw-rw-rw-   0        0        0     1153 2023-07-16 05:36:19.000000 sigils-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 05:37:29.059391 sigils-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 05:37:28.997863 sigils-0.3.2/sigils/
--rw-rw-rw-   0        0        0     7771 2023-07-16 05:07:20.000000 sigils-0.3.2/sigils/__init__.py
--rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.2/sigils/__main__.py
--rw-rw-rw-   0        0        0     2633 2023-07-16 04:32:05.000000 sigils-0.3.2/sigils/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:37:29.052388 sigils-0.3.2/sigils.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:05:23.155058 sigils-0.3.3/
+-rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.3/.gitignore
+-rw-rw-rw-   0        0        0     1001 2023-07-16 02:58:04.000000 sigils-0.3.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1084 2023-07-16 05:32:45.000000 sigils-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     4199 2023-07-16 06:05:23.153065 sigils-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3212 2023-07-16 06:04:34.000000 sigils-0.3.3/README.rst
+-rw-rw-rw-   0        0        0     1153 2023-07-16 05:39:22.000000 sigils-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 06:05:23.156064 sigils-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 06:05:23.086428 sigils-0.3.3/sigils/
+-rw-rw-rw-   0        0        0     8015 2023-07-16 06:03:15.000000 sigils-0.3.3/sigils/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.3/sigils/__main__.py
+-rw-rw-rw-   0        0        0     2631 2023-07-16 06:03:48.000000 sigils-0.3.3/sigils/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:05:23.149058 sigils-0.3.3/sigils.egg-info/
+-rw-rw-rw-   0        0        0     4199 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-16 06:05:23.000000 sigils-0.3.3/sigils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/top_level.txt
```

### Comparing `sigils-0.3.2/.gitignore` & `sigils-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sigils-0.3.2/CHANGELOG.md` & `sigils-0.3.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sigils-0.3.2/LICENSE` & `sigils-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sigils-0.3.2/PKG-INFO` & `sigils-0.3.3/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,16 @@
-Metadata-Version: 2.1
-Name: sigils
-Version: 0.3.2
-Summary: Interpolate with %[sigils].
-Author-email: Rafael Jesús Guillén Osorio <arthexis@gmail.com>
-License: MIT
-Project-URL: Source, https://github.com/arthexis/sigils
-Project-URL: Bug-Tracker, https://github.com/arthexis/sigils/issues
-Keywords: utils,sigils,string,text,context
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Text Processing :: Markup
-Classifier: Topic :: Software Development :: Pre-processors
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ================
 Sigils
 ================
 
-Sigils is a Python library for powerful and flexible string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
+"An inscribed or painted symbol considered to have magical power."
+
+Sigils is a Python library for magic and string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
+
+Any Python object can be provided as context, including nested dictionaries, lists, and functions. Sigils can be used directly from Python or from the command line. Sigils is thread-safe and has no dependencies outside of the Python standard library.
 
 Installation
 ============
 
 Install Sigils using pip:
 
 .. code-block:: bash
@@ -58,28 +38,43 @@
 
     context = {
         "user": {
             "name": "Alice",
             "greet": lambda name: f"Hello, {name}!"
         }
     }
+    
     s = Sigil("%[user.greet:user.name]")
     print(s % context)  # Outputs: Hello, Alice!
 
+    s = Sigil("%[user.greet:%%user.name]")
+    print(s % context)  # Outputs: Hello, %user.name! %user.name is treated as a literal value
+
 Sigils support case-insensitive matching and global context fallback:
 
 .. code-block:: python
 
     from sigils import Sigil, Sigil.Context
 
     global_context = {"greeting": "Hello, world!"}
     with Sigil.Context(global_context):
         s = Sigil("%[GREETING]")
         print(s % {})  # Outputs: Hello, world!
 
+Command-Line Usage
+==================
+
+Sigils can be used directly from the command line. Here's an example:
+
+.. code-block:: bash
+
+    sigils "Hello, %[user.name]!" -c context.json
+
+In this example, "context.json" is a JSON file with a structure like {"user": {"name": "Alice"}}. The command will output: "Hello, Alice!".
+
 Considerations
 ==============
 
 - **Function Execution**: If the value of a Sigil is a callable function, it will be executed and its return value used in the string. Ensure all function values in your context are safe to execute.
 - **Recursion Depth**: Sigils handles up to 6 levels of nested interpolation by default. Adjust this limit by passing a different `max_depth` value to the `interpolate` method.
 - **Thread Safety**: The global context in Sigils is thread-safe. However, if you're using mutable objects in your context and modifying them from multiple threads, manage thread safety at the application level.
 - **Case-Insensitive Matching**: If a key fails to resolve, a case-insensitive lookup is attempted. This only works if the keys in your context are all unique when lowercased.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sigils-0.3.2/pyproject.toml` & `sigils-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigils"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     {name = "Rafael Jesús Guillén Osorio", email = "arthexis@gmail.com"},
 ]
 description = "Interpolate with %[sigils]."
 readme = "README.rst"
 requires-python = ">=3.10"
 keywords = ["utils", "sigils", "string", "text", "context"]
```

### Comparing `sigils-0.3.2/sigils/__init__.py` & `sigils-0.3.3/sigils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,31 +45,37 @@
             keys = match.split('.')
             value = context
             function_args = []
             try:
                 for i, key in enumerate(keys):
                     if ':' in key:
                         key, *function_args = key.split(':')
-                    if isinstance(value, dict):
+                    literal = False
+                    if key.startswith('%'):
+                        key = key[1:]
+                        literal = True
+                    if literal:
+                        temp = key
+                    elif isinstance(value, dict):
                         temp = value.get(key)
                     elif isinstance(value, list) and key.isdigit():
                         temp = value[int(key)]
                     else:
                         temp = None
-                    if temp is None and '-' in key:
+                    if temp is None and '-' in key and not literal:
                         temp = value.get(key.replace('-', '_')) if isinstance(value, dict) else None
-                    if temp is None and hasattr(value, key):
+                    if temp is None and hasattr(value, key) and not literal:
                         temp = getattr(value, key)
-                    if temp is None and '-' in key and hasattr(value, key.replace('-', '_')):
+                    if temp is None and '-' in key and hasattr(value, key.replace('-', '_')) and not literal:
                         temp = getattr(value, key.replace('-', '_'))
                     if temp is not None:
                         value = temp
                         if callable(value) and execute:
                             if function_args:
-                                resolved_function_args = [Sigil(f'%[{arg[1:]}]').interpolate(context) if arg.startswith('%') else arg for arg in function_args]
+                                resolved_function_args = [Sigil(f'%[{arg}]').interpolate(context) for arg in function_args]
                                 value = value(*resolved_function_args)
                             else:
                                 value = value()
                     else:
                         value = None
                         break
             except (TypeError, AttributeError):
```

### Comparing `sigils-0.3.2/sigils/__main__.py` & `sigils-0.3.3/sigils/__main__.py`

 * *Files identical despite different names*

### Comparing `sigils-0.3.2/sigils/tests.py` & `sigils-0.3.3/sigils/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         self.assertEqual(s % self.context, "Number: 2")
 
     def test_callable_interpolation(self):
         s = Sigil("%[callable]")
         self.assertEqual(s % self.context, "Hello, World!")
 
     def test_callable_with_args_interpolation(self):
-        s = Sigil("%[callable_with_args:%name]")
+        s = Sigil("%[callable_with_args:name]")
         self.assertEqual(s % self.context, "Hello, Alice!")
 
     def test_callable_with_literal_args(self):
-        s = Sigil("%[callable_with_args:name]")
+        s = Sigil("%[callable_with_args:%name]")
         self.assertEqual(s % self.context, "Hello, name!")
 
     def test_sigils(self):
         s = Sigil("Hello, %[name]!")
         self.assertEqual(s.sigils(self.context), {"name": "Alice"})
 
     def test_recursive_interpolation(self):
@@ -61,18 +61,18 @@
             {"name": "Bob", "email": "bob@example.com"}
         ]
         s = Sigil("User: %[users.0.name], Email: %[users.0.email]")
         self.assertEqual(s % self.context, "User: Alice, Email: alice@example.com")
 
     def test_nested_callable_with_args_interpolation(self):
         self.context['nested']['callable_with_args'] = lambda x: f"Hello, {x}!"
-        s = Sigil("Message: %[nested.callable_with_args:%name]")
+        s = Sigil("Message: %[nested.callable_with_args:name]")
         self.assertEqual(s % self.context, "Message: Hello, Alice!")
 
     def test_recursive_callable(self):
-        s = Sigil("Message: %[recursive:%name]")
+        s = Sigil("Message: %[recursive:name]")
         self.assertEqual(s % self.context, "Message: Hello, Alice!")
 
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `sigils-0.3.2/sigils.egg-info/PKG-INFO` & `sigils-0.3.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigils
-Version: 0.3.2
+Version: 0.3.3
 Summary: Interpolate with %[sigils].
 Author-email: Rafael Jesús Guillén Osorio <arthexis@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/arthexis/sigils
 Project-URL: Bug-Tracker, https://github.com/arthexis/sigils/issues
 Keywords: utils,sigils,string,text,context
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,19 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 Sigils
 ================
 
-Sigils is a Python library for powerful and flexible string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
+"An inscribed or painted symbol considered to have magical power."
+
+Sigils is a Python library for magic and string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
+
+Any Python object can be provided as context, including nested dictionaries, lists, and functions. Sigils can be used directly from Python or from the command line. Sigils is thread-safe and has no dependencies outside of the Python standard library.
 
 Installation
 ============
 
 Install Sigils using pip:
 
 .. code-block:: bash
@@ -58,28 +62,43 @@
 
     context = {
         "user": {
             "name": "Alice",
             "greet": lambda name: f"Hello, {name}!"
         }
     }
+    
     s = Sigil("%[user.greet:user.name]")
     print(s % context)  # Outputs: Hello, Alice!
 
+    s = Sigil("%[user.greet:%%user.name]")
+    print(s % context)  # Outputs: Hello, %user.name! %user.name is treated as a literal value
+
 Sigils support case-insensitive matching and global context fallback:
 
 .. code-block:: python
 
     from sigils import Sigil, Sigil.Context
 
     global_context = {"greeting": "Hello, world!"}
     with Sigil.Context(global_context):
         s = Sigil("%[GREETING]")
         print(s % {})  # Outputs: Hello, world!
 
+Command-Line Usage
+==================
+
+Sigils can be used directly from the command line. Here's an example:
+
+.. code-block:: bash
+
+    sigils "Hello, %[user.name]!" -c context.json
+
+In this example, "context.json" is a JSON file with a structure like {"user": {"name": "Alice"}}. The command will output: "Hello, Alice!".
+
 Considerations
 ==============
 
 - **Function Execution**: If the value of a Sigil is a callable function, it will be executed and its return value used in the string. Ensure all function values in your context are safe to execute.
 - **Recursion Depth**: Sigils handles up to 6 levels of nested interpolation by default. Adjust this limit by passing a different `max_depth` value to the `interpolate` method.
 - **Thread Safety**: The global context in Sigils is thread-safe. However, if you're using mutable objects in your context and modifying them from multiple threads, manage thread safety at the application level.
 - **Case-Insensitive Matching**: If a key fails to resolve, a case-insensitive lookup is attempted. This only works if the keys in your context are all unique when lowercased.
```

