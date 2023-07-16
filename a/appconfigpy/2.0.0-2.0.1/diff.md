# Comparing `tmp/appconfigpy-2.0.0.tar.gz` & `tmp/appconfigpy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appconfigpy-2.0.0.tar", last modified: Sat Mar 11 08:26:17 2023, max compression
+gzip compressed data, was "appconfigpy-2.0.1.tar", last modified: Sun Jul 16 10:10:35 2023, max compression
```

## Comparing `appconfigpy-2.0.0.tar` & `appconfigpy-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-03-11 08:26:17.338116 appconfigpy-2.0.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      173 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     4449 2023-03-11 08:26:17.338116 appconfigpy-2.0.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     3014 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-03-11 08:26:17.328116 appconfigpy-2.0.0/appconfigpy/
--rw-r--r--   0 toor      (1000) toor      (1000)      540 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/appconfigpy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/appconfigpy/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6658 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/appconfigpy/_config.py
--rw-r--r--   0 toor      (1000) toor      (1000)       99 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/appconfigpy/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1558 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/appconfigpy/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/appconfigpy/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-03-11 08:26:17.338116 appconfigpy-2.0.0/appconfigpy.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     4449 2023-03-11 08:26:17.000000 appconfigpy-2.0.0/appconfigpy.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      564 2023-03-11 08:26:17.000000 appconfigpy-2.0.0/appconfigpy.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-03-11 08:26:17.000000 appconfigpy-2.0.0/appconfigpy.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2023-03-11 08:26:17.000000 appconfigpy-2.0.0/appconfigpy.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       21 2023-03-11 08:26:17.000000 appconfigpy-2.0.0/appconfigpy.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-03-11 08:26:17.338116 appconfigpy-2.0.0/examples/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/examples/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      686 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/examples/common.py
--rw-r--r--   0 toor      (1000) toor      (1000)      209 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/examples/configure.py
--rw-r--r--   0 toor      (1000) toor      (1000)      302 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/examples/load.py
--rw-r--r--   0 toor      (1000) toor      (1000)      710 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-03-11 08:26:17.338116 appconfigpy-2.0.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        7 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-03-11 08:26:17.338116 appconfigpy-2.0.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2793 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-03-11 08:26:17.338116 appconfigpy-2.0.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)     1875 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/test/test_config_mgr.py
--rw-r--r--   0 toor      (1000) toor      (1000)      530 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/test/test_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)      956 2023-03-11 08:25:47.000000 appconfigpy-2.0.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      173 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     4449 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     3014 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/appconfigpy/
+-rw-r--r--   0 toor      (1000) toor      (1000)      540 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/appconfigpy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/appconfigpy/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6735 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/appconfigpy/_config.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       99 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/appconfigpy/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1558 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/appconfigpy/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/appconfigpy/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/appconfigpy.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4449 2023-07-16 10:10:35.000000 appconfigpy-2.0.1/appconfigpy.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      598 2023-07-16 10:10:35.000000 appconfigpy-2.0.1/appconfigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 10:10:35.000000 appconfigpy-2.0.1/appconfigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 10:10:03.000000 appconfigpy-2.0.1/appconfigpy.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       43 2023-07-16 10:10:35.000000 appconfigpy-2.0.1/appconfigpy.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       21 2023-07-16 10:10:35.000000 appconfigpy-2.0.1/appconfigpy.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/examples/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/examples/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      686 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/examples/common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      209 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/examples/configure.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      302 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/examples/load.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      747 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        7 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2813 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 10:10:35.738878 appconfigpy-2.0.1/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1875 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/test/test_config_mgr.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      530 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/test/test_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      894 2023-07-16 10:09:47.000000 appconfigpy-2.0.1/tox.ini
```

### Comparing `appconfigpy-2.0.0/LICENSE` & `appconfigpy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appconfigpy-2.0.0/PKG-INFO` & `appconfigpy-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appconfigpy
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python library to create/load an application configuration file.
 Home-page: https://github.com/thombashi/appconfigpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/appconfigpy
 Project-URL: Tracker, https://github.com/thombashi/appconfigpy/issues
```

### Comparing `appconfigpy-2.0.0/README.rst` & `appconfigpy-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `appconfigpy-2.0.0/appconfigpy/__init__.py` & `appconfigpy-2.0.1/appconfigpy/__init__.py`

 * *Files identical despite different names*

### Comparing `appconfigpy-2.0.0/appconfigpy/_config.py` & `appconfigpy-2.0.1/appconfigpy/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         return self.__config_filepath
 
     @property
     def config_file_path(self):
         import warnings
 
         warnings.warn(
-            "'config_file_path' property has moved to 'config_filepath'", DeprecationWarning
+            "'config_file_path' property is deprecated and will be removed in the future."
+            " use 'config_filepath' instead.",
+            DeprecationWarning,
         )
 
         return self.__config_filepath
 
     @property
     def exists(self) -> bool:
         return os.path.exists(self.__config_filepath)
```

### Comparing `appconfigpy-2.0.0/appconfigpy/_logger.py` & `appconfigpy-2.0.1/appconfigpy/_logger.py`

 * *Files identical despite different names*

### Comparing `appconfigpy-2.0.0/appconfigpy.egg-info/PKG-INFO` & `appconfigpy-2.0.1/appconfigpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appconfigpy
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python library to create/load an application configuration file.
 Home-page: https://github.com/thombashi/appconfigpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/appconfigpy
 Project-URL: Tracker, https://github.com/thombashi/appconfigpy/issues
```

### Comparing `appconfigpy-2.0.0/appconfigpy.egg-info/SOURCES.txt` & `appconfigpy-2.0.1/appconfigpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 appconfigpy/_config.py
 appconfigpy/_const.py
 appconfigpy/_logger.py
 appconfigpy/py.typed
 appconfigpy.egg-info/PKG-INFO
 appconfigpy.egg-info/SOURCES.txt
 appconfigpy.egg-info/dependency_links.txt
+appconfigpy.egg-info/not-zip-safe
 appconfigpy.egg-info/requires.txt
 appconfigpy.egg-info/top_level.txt
 examples/__init__.py
 examples/common.py
 examples/configure.py
 examples/load.py
 requirements/requirements.txt
```

### Comparing `appconfigpy-2.0.0/examples/common.py` & `appconfigpy-2.0.1/examples/common.py`

 * *Files identical despite different names*

### Comparing `appconfigpy-2.0.0/pyproject.toml` & `appconfigpy-2.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
```

### Comparing `appconfigpy-2.0.0/setup.py` & `appconfigpy-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,8 +77,9 @@
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     cmdclass=get_release_command_class(),
+    zip_safe=False,
 )
```

### Comparing `appconfigpy-2.0.0/test/test_config_mgr.py` & `appconfigpy-2.0.1/test/test_config_mgr.py`

 * *Files identical despite different names*

### Comparing `appconfigpy-2.0.0/test/test_logger.py` & `appconfigpy-2.0.1/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `appconfigpy-2.0.0/tox.ini` & `appconfigpy-2.0.1/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
-    twine check dist/*.whl dist/*.tar.gz
+    python -m build
     python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
@@ -50,12 +50,11 @@
     isort .
     black setup.py test appconfigpy
 
 [testenv:lint]
 skip_install = true
 deps =
     mypy>=1
-    pylama
+    pylama>=8.4.1
 commands =
-    python setup.py check
     pylama
     mypy appconfigpy setup.py
```

