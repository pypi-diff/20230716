# Comparing `tmp/docstring_generator_ext-0.0.28.tar.gz` & `tmp/docstring_generator_ext-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstring_generator_ext-0.0.28.tar", last modified: Fri Jun  2 08:53:06 2023, max compression
+gzip compressed data, was "docstring_generator_ext-0.0.31.tar", last modified: Sun Jul 16 10:08:49 2023, max compression
```

## Comparing `docstring_generator_ext-0.0.28.tar` & `docstring_generator_ext-0.0.31.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/
--rw-rw-r--   0 felix     (1000) felix     (1000)      902 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/PKG-INFO
--rw-rw-r--   0 felix     (1000) felix     (1000)      212 2023-06-02 07:53:42.000000 docstring_generator_ext-0.0.28/README.md
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/
--rw-rw-r--   0 felix     (1000) felix     (1000)      902 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1000) felix     (1000)      361 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-06-02 08:16:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/not-zip-safe
--rw-rw-r--   0 felix     (1000) felix     (1000)       15 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/requires.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)       24 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/top_level.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)      864 2023-06-02 07:55:25.000000 docstring_generator_ext-0.0.28/pyproject.toml
--rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/setup.cfg
--rw-rw-r--   0 felix     (1000) felix     (1000)     1959 2023-06-02 08:53:01.000000 docstring_generator_ext-0.0.28/setup.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/src/
--rw-rw-r--   0 felix     (1000) felix     (1000)    17478 2023-06-02 07:53:42.000000 docstring_generator_ext-0.0.28/src/docstringFormat.cpp
--rw-rw-r--   0 felix     (1000) felix     (1000)    16324 2023-06-02 08:40:40.000000 docstring_generator_ext-0.0.28/src/docstringFormat.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:08:49.441046 docstring_generator_ext-0.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-16 10:08:49.441046 docstring_generator_ext-0.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-16 10:08:38.000000 docstring_generator_ext-0.0.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:08:49.441046 docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-16 10:08:49.000000 docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-16 10:08:49.000000 docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 10:08:49.000000 docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 10:08:49.000000 docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 10:08:49.000000 docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 10:08:49.000000 docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-16 10:08:38.000000 docstring_generator_ext-0.0.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 10:08:49.441046 docstring_generator_ext-0.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-16 10:08:38.000000 docstring_generator_ext-0.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:08:49.441046 docstring_generator_ext-0.0.31/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    33538 2023-07-16 10:08:38.000000 docstring_generator_ext-0.0.31/src/docstringFormat.cpp
```

### Comparing `docstring_generator_ext-0.0.28/PKG-INFO` & `docstring_generator_ext-0.0.31/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: docstring_generator_ext
-Version: 0.0.28
+Version: 0.0.31
 Summary: Generate Docstrings with type-hint information
 Home-page: https://github.com/FelixTheC/docstring_generator
 Author: FelixTheC
 Author-email: fberndt87@gmail.com
 License: MIT
-Description: #### Versioning
-        - For the versions available, see the tags on this repository.
-        
-        ### Authors
-        - Felix Eisenmenger
-        
-        ### License
-        - This project is licensed under the MIT License - see the LICENSE.md file for details
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Typing :: Typed
-Requires-Python: <=3.11
+Requires-Python: <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
+
+#### Versioning
+- For the versions available, see the tags on this repository.
+
+### Authors
+- Felix Eisenmenger
+
+### License
+- This project is licensed under the MIT License - see the LICENSE.md file for details
```

### Comparing `docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/PKG-INFO` & `docstring_generator_ext-0.0.31/docstring_generator_ext.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: docstring-generator-ext
-Version: 0.0.28
+Version: 0.0.31
 Summary: Generate Docstrings with type-hint information
 Home-page: https://github.com/FelixTheC/docstring_generator
 Author: FelixTheC
 Author-email: fberndt87@gmail.com
 License: MIT
-Description: #### Versioning
-        - For the versions available, see the tags on this repository.
-        
-        ### Authors
-        - Felix Eisenmenger
-        
-        ### License
-        - This project is licensed under the MIT License - see the LICENSE.md file for details
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Typing :: Typed
-Requires-Python: <=3.11
+Requires-Python: <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
+
+#### Versioning
+- For the versions available, see the tags on this repository.
+
+### Authors
+- Felix Eisenmenger
+
+### License
+- This project is licensed under the MIT License - see the LICENSE.md file for details
```

### Comparing `docstring_generator_ext-0.0.28/setup.py` & `docstring_generator_ext-0.0.31/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 # Available at setup time due to pyproject.toml
 import pathlib
-from glob import glob
 
 from pybind11.setup_helpers import Pybind11Extension, build_ext
-from setuptools import find_packages, setup
+from setuptools import setup
 
-__version__ = "0.0.28"
+__version__ = "0.0.31"
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/python_example/pull/53)
 
-
-class CustomBuildExt(build_ext):
-    def run(self):
-        # Include additional header file directories
-        self.include_dirs.append('src/docstringFormat.hpp')
-        super().run()
-
-
 ext_modules = [
     Pybind11Extension(
         "docstring_generator_ext",
         [
             "src/docstringFormat.cpp",
         ],
     ),
@@ -54,11 +45,11 @@
         "Topic :: Software Development :: Documentation",
         "Typing :: Typed",
     ],
     ext_modules=ext_modules,
     extras_require={"test": "pytest"},
     # Currently, build_ext only provides an optional "highest supported C++
     # level" feature, but in the future it may provide more features.
-    cmdclass={"build_ext": CustomBuildExt},
+    cmdclass={"build_ext": build_ext},
     zip_safe=False,
-    python_requires="<=3.11",
+    python_requires="<3.12",
 )
```

