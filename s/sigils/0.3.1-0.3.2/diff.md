# Comparing `tmp/sigils-0.3.1.tar.gz` & `tmp/sigils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigils-0.3.1.tar", last modified: Sun Jul 16 05:21:23 2023, max compression
+gzip compressed data, was "sigils-0.3.2.tar", last modified: Sun Jul 16 05:37:29 2023, max compression
```

## Comparing `sigils-0.3.1.tar` & `sigils-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 05:21:23.668389 sigils-0.3.1/
--rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.1/.gitignore
--rw-rw-rw-   0        0        0     1001 2023-07-16 02:58:04.000000 sigils-0.3.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     4453 2023-07-16 05:21:23.666233 sigils-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3489 2023-07-16 02:50:25.000000 sigils-0.3.1/README.rst
--rw-rw-rw-   0        0        0     1153 2023-07-16 02:57:41.000000 sigils-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 05:21:23.668389 sigils-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 05:21:23.597085 sigils-0.3.1/sigils/
--rw-rw-rw-   0        0        0     7771 2023-07-16 05:07:20.000000 sigils-0.3.1/sigils/__init__.py
--rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.1/sigils/__main__.py
--rw-rw-rw-   0        0        0     2633 2023-07-16 04:32:05.000000 sigils-0.3.1/sigils/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:21:23.661007 sigils-0.3.1/sigils.egg-info/
--rw-rw-rw-   0        0        0     4453 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 05:21:23.000000 sigils-0.3.1/sigils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      437 2023-07-16 03:02:12.000000 sigils-0.3.1/test.json
+drwxrwxrwx   0        0        0        0 2023-07-16 05:37:29.059391 sigils-0.3.2/
+-rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.2/.gitignore
+-rw-rw-rw-   0        0        0     1001 2023-07-16 02:58:04.000000 sigils-0.3.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1084 2023-07-16 05:32:45.000000 sigils-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-07-16 05:37:29.056388 sigils-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2023-07-16 05:35:04.000000 sigils-0.3.2/README.rst
+-rw-rw-rw-   0        0        0     1153 2023-07-16 05:36:19.000000 sigils-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 05:37:29.059391 sigils-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 05:37:28.997863 sigils-0.3.2/sigils/
+-rw-rw-rw-   0        0        0     7771 2023-07-16 05:07:20.000000 sigils-0.3.2/sigils/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.2/sigils/__main__.py
+-rw-rw-rw-   0        0        0     2633 2023-07-16 04:32:05.000000 sigils-0.3.2/sigils/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-16 05:37:29.052388 sigils-0.3.2/sigils.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 05:37:28.000000 sigils-0.3.2/sigils.egg-info/top_level.txt
```

### Comparing `sigils-0.3.1/.gitignore` & `sigils-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sigils-0.3.1/CHANGELOG.md` & `sigils-0.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sigils-0.3.1/README.rst` & `sigils-0.3.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,41 @@
+Metadata-Version: 2.1
+Name: sigils
+Version: 0.3.2
+Summary: Interpolate with %[sigils].
+Author-email: Rafael Jesús Guillén Osorio <arthexis@gmail.com>
+License: MIT
+Project-URL: Source, https://github.com/arthexis/sigils
+Project-URL: Bug-Tracker, https://github.com/arthexis/sigils/issues
+Keywords: utils,sigils,string,text,context
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Software Development :: Pre-processors
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ================
 Sigils
 ================
 
-Sigils is a Python library for powerful and flexible string interpolation.
-
-Overview
-========
-
-Sigils extends Python's built-in string formatting capabilities with additional features like:
-
-- Context-based interpolation: Sigils can be replaced by values from a context, which can be a dictionary or an object.
-- Function execution: If a Sigil's value is a callable function, it can be executed and its return value used in the string.
-- Nested and recursive interpolation: Sigils can be nested within other Sigils, and recursion is handled intelligently.
-- Case-insensitive matching: If a key fails to resolve, a case-insensitive lookup is attempted.
-- Global context: Alongside the context passed for each string, a global context can be maintained and used as a fallback.
+Sigils is a Python library for powerful and flexible string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
 
 Installation
 ============
 
-Sigils can be installed via pip:
+Install Sigils using pip:
 
 .. code-block:: bash
 
     pip install sigils
 
 Usage
 =====
@@ -33,43 +46,50 @@
 
     from sigils import Sigil
 
     context = {"user": {"name": "Alice"}}
     s = Sigil("Hello, %[user.name]!")
     print(s % context)  # Outputs: Hello, Alice!
 
-For more complex uses, such as function execution and nested interpolation, refer to the documentation and example code.
+Sigils can handle function execution and nested interpolation:
 
-Use Cases
-=========
+.. code-block:: python
 
-Sigils can be used in a variety of scenarios:
+    from sigils import Sigil
 
-- **Configuration File Generation**: Generate configuration files for various applications. The context could be loaded from a file or a database, and the output could be written to a config file.
-- **Template Rendering**: Render templates for web pages, emails, or other forms of user-facing content. The context would typically be user data or other dynamic content.
-- **Code Generation**: Generate code, for instance in a code-generation tool or a scaffolding tool.
+    context = {
+        "user": {
+            "name": "Alice",
+            "greet": lambda name: f"Hello, {name}!"
+        }
+    }
+    s = Sigil("%[user.greet:user.name]")
+    print(s % context)  # Outputs: Hello, Alice!
 
-Gotchas
-=======
+Sigils support case-insensitive matching and global context fallback:
 
-- **Execution of Functions**: If the value of a Sigil is a callable function, it will be executed and its return value used in the string. Ensure all function values in your context are safe to execute.
-- **Recursion Depth**: By default, Sigils handles up to 6 levels of nested interpolation. Adjust this limit by passing a different `max_depth` value to the `interpolate` method.
-- **Thread Safety**: The global context in Sigils is thread-safe. However, if you're using mutable objects in your context and you're modifying them from multiple threads, manage thread safety at the application level.
-- **Case-Insensitive Matching**: If a key fails to resolve, a case-insensitive lookup is attempted. This only works if the keys in your context are all unique when lowercased.
+.. code-block:: python
 
+    from sigils import Sigil, Sigil.Context
+
+    global_context = {"greeting": "Hello, world!"}
+    with Sigil.Context(global_context):
+        s = Sigil("%[GREETING]")
+        print(s % {})  # Outputs: Hello, world!
+
+Considerations
+==============
+
+- **Function Execution**: If the value of a Sigil is a callable function, it will be executed and its return value used in the string. Ensure all function values in your context are safe to execute.
+- **Recursion Depth**: Sigils handles up to 6 levels of nested interpolation by default. Adjust this limit by passing a different `max_depth` value to the `interpolate` method.
+- **Thread Safety**: The global context in Sigils is thread-safe. However, if you're using mutable objects in your context and modifying them from multiple threads, manage thread safety at the application level.
+- **Case-Insensitive Matching**: If a key fails to resolve, a case-insensitive lookup is attempted. This only works if the keys in your context are all unique when lowercased.
 
 Performance
 ===========
 
-Sigils has been designed with performance in mind. While the exact performance can vary based on the complexity of your templates and the depth of your context objects, Sigils performs competitively with Python's built-in string formatting in many scenarios.
-
-In a typical use case, with 10000 interpolations of a template with a medium-sized context, Sigils can complete the operation in around 0.02 seconds. For larger templates and contexts, the time increases, but remains within acceptable limits for most applications, including web applications.
-
-Contributing
-============
-
-Contributions to Sigils are welcome! Please refer to the CONTRIBUTING.rst file for guidelines.
+Sigils is designed with performance in mind. In typical use cases, Sigils performs competitively with Python's built-in string formatting.
 
 License
 =======
 
 Sigils is licensed under the MIT License. See the LICENSE file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sigils-0.3.1/pyproject.toml` & `sigils-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigils"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     {name = "Rafael Jesús Guillén Osorio", email = "arthexis@gmail.com"},
 ]
 description = "Interpolate with %[sigils]."
 readme = "README.rst"
 requires-python = ">=3.10"
 keywords = ["utils", "sigils", "string", "text", "context"]
```

### Comparing `sigils-0.3.1/sigils/__init__.py` & `sigils-0.3.2/sigils/__init__.py`

 * *Files identical despite different names*

### Comparing `sigils-0.3.1/sigils/__main__.py` & `sigils-0.3.2/sigils/__main__.py`

 * *Files identical despite different names*

### Comparing `sigils-0.3.1/sigils/tests.py` & `sigils-0.3.2/sigils/tests.py`

 * *Files identical despite different names*

