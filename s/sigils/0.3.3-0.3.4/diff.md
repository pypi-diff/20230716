# Comparing `tmp/sigils-0.3.3.tar.gz` & `tmp/sigils-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigils-0.3.3.tar", last modified: Sun Jul 16 06:05:23 2023, max compression
+gzip compressed data, was "sigils-0.3.4.tar", last modified: Sun Jul 16 06:24:33 2023, max compression
```

## Comparing `sigils-0.3.3.tar` & `sigils-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:05:23.155058 sigils-0.3.3/
--rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.3/.gitignore
--rw-rw-rw-   0        0        0     1001 2023-07-16 02:58:04.000000 sigils-0.3.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1084 2023-07-16 05:32:45.000000 sigils-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     4199 2023-07-16 06:05:23.153065 sigils-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3212 2023-07-16 06:04:34.000000 sigils-0.3.3/README.rst
--rw-rw-rw-   0        0        0     1153 2023-07-16 05:39:22.000000 sigils-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 06:05:23.156064 sigils-0.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 06:05:23.086428 sigils-0.3.3/sigils/
--rw-rw-rw-   0        0        0     8015 2023-07-16 06:03:15.000000 sigils-0.3.3/sigils/__init__.py
--rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.3/sigils/__main__.py
--rw-rw-rw-   0        0        0     2631 2023-07-16 06:03:48.000000 sigils-0.3.3/sigils/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:05:23.149058 sigils-0.3.3/sigils.egg-info/
--rw-rw-rw-   0        0        0     4199 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-16 06:05:23.000000 sigils-0.3.3/sigils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 06:05:22.000000 sigils-0.3.3/sigils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:24:33.526569 sigils-0.3.4/
+-rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.4/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-07-16 06:22:50.000000 sigils-0.3.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1084 2023-07-16 05:32:45.000000 sigils-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     4249 2023-07-16 06:24:33.524572 sigils-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3212 2023-07-16 06:04:34.000000 sigils-0.3.4/README.rst
+-rw-rw-rw-   0        0        0     1198 2023-07-16 06:21:43.000000 sigils-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 06:24:33.526569 sigils-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 06:24:33.443528 sigils-0.3.4/sigils/
+-rw-rw-rw-   0        0        0     8015 2023-07-16 06:03:15.000000 sigils-0.3.4/sigils/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.4/sigils/__main__.py
+-rw-rw-rw-   0        0        0     2631 2023-07-16 06:03:48.000000 sigils-0.3.4/sigils/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:24:33.519568 sigils-0.3.4/sigils.egg-info/
+-rw-rw-rw-   0        0        0     4249 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       75 2023-07-16 06:21:28.000000 sigils-0.3.4/test.json
```

### Comparing `sigils-0.3.3/.gitignore` & `sigils-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sigils-0.3.3/CHANGELOG.md` & `sigils-0.3.4/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Release Notes
 =============
 
+0.3.4 (2023-07-16)
+-------------------
+
+Restore backwards compatibility with Python 3.9.
+
 0.3.1 (2023-07-15)
 -------------------
 
 Complete revamp and simplification of the library.
 
 Sigils now use the following syntax:
```

### Comparing `sigils-0.3.3/LICENSE` & `sigils-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sigils-0.3.3/PKG-INFO` & `sigils-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigils
-Version: 0.3.3
+Version: 0.3.4
 Summary: Interpolate with %[sigils].
 Author-email: Rafael Jesús Guillén Osorio <arthexis@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/arthexis/sigils
 Project-URL: Bug-Tracker, https://github.com/arthexis/sigils/issues
 Keywords: utils,sigils,string,text,context
 Classifier: Development Status :: 3 - Alpha
@@ -12,17 +12,18 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 Sigils
 ================
```

### Comparing `sigils-0.3.3/README.rst` & `sigils-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `sigils-0.3.3/pyproject.toml` & `sigils-0.3.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigils"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
     {name = "Rafael Jesús Guillén Osorio", email = "arthexis@gmail.com"},
 ]
 description = "Interpolate with %[sigils]."
 readme = "README.rst"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 keywords = ["utils", "sigils", "string", "text", "context"]
 license = {text = "MIT"}
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Libraries',
     'Topic :: Text Processing :: Markup',
     'Topic :: Software Development :: Pre-processors',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Environment :: Console',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 dependencies = [
 ]
 
 [project.urls]
```

### Comparing `sigils-0.3.3/sigils/__init__.py` & `sigils-0.3.4/sigils/__init__.py`

 * *Files identical despite different names*

### Comparing `sigils-0.3.3/sigils/__main__.py` & `sigils-0.3.4/sigils/__main__.py`

 * *Files identical despite different names*

### Comparing `sigils-0.3.3/sigils/tests.py` & `sigils-0.3.4/sigils/tests.py`

 * *Files identical despite different names*

### Comparing `sigils-0.3.3/sigils.egg-info/PKG-INFO` & `sigils-0.3.4/sigils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigils
-Version: 0.3.3
+Version: 0.3.4
 Summary: Interpolate with %[sigils].
 Author-email: Rafael Jesús Guillén Osorio <arthexis@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/arthexis/sigils
 Project-URL: Bug-Tracker, https://github.com/arthexis/sigils/issues
 Keywords: utils,sigils,string,text,context
 Classifier: Development Status :: 3 - Alpha
@@ -12,17 +12,18 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 Sigils
 ================
```

