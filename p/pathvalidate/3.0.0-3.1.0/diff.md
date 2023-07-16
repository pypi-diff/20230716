# Comparing `tmp/pathvalidate-3.0.0.tar.gz` & `tmp/pathvalidate-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathvalidate-3.0.0.tar", last modified: Mon May 22 14:16:00 2023, max compression
+gzip compressed data, was "pathvalidate-3.1.0.tar", last modified: Sun Jul 16 02:56:50 2023, max compression
```

## Comparing `pathvalidate-3.0.0.tar` & `pathvalidate-3.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    11160 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     9413 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/docs/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/docs/pages/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/docs/pages/introduction/
--rw-r--r--   0 toor      (1000) toor      (1000)       97 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/docs/pages/introduction/summary.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/pathvalidate/
--rw-r--r--   0 toor      (1000) toor      (1000)     1926 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6041 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_base.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3351 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)      523 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)    14841 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_filename.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16234 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_filepath.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1203 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_ltsv.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2326 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_symbol.py
--rw-r--r--   0 toor      (1000) toor      (1000)      180 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_types.py
--rw-r--r--   0 toor      (1000) toor      (1000)      970 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/argparse.py
--rw-r--r--   0 toor      (1000) toor      (1000)      960 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/click.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5313 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)      441 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/handler.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/pathvalidate.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    11160 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      965 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-22 14:15:27.000000 pathvalidate-3.0.0/pathvalidate.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      136 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1251 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       39 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      121 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2894 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1875 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4270 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_argparse.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2325 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_click.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1569 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)      297 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_error.py
--rw-r--r--   0 toor      (1000) toor      (1000)    22640 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_filename.py
--rw-r--r--   0 toor      (1000) toor      (1000)    30287 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_filepath.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2500 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_ltsv.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4342 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_symbol.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1505 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.991691 pathvalidate-3.1.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11173 2023-07-16 02:56:49.991691 pathvalidate-3.1.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     9455 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.981691 pathvalidate-3.1.0/docs/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.981691 pathvalidate-3.1.0/docs/pages/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.981691 pathvalidate-3.1.0/docs/pages/introduction/
+-rw-r--r--   0 toor      (1000) toor      (1000)       97 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/docs/pages/introduction/summary.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.981691 pathvalidate-3.1.0/pathvalidate/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1926 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6041 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3363 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      686 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14897 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_filename.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16387 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_filepath.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1203 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_ltsv.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2326 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_symbol.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      180 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/_types.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      970 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/argparse.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      960 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/click.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6441 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      441 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/handler.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pathvalidate/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.981691 pathvalidate-3.1.0/pathvalidate.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11173 2023-07-16 02:56:49.000000 pathvalidate-3.1.0/pathvalidate.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      965 2023-07-16 02:56:49.000000 pathvalidate-3.1.0/pathvalidate.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 02:56:49.000000 pathvalidate-3.1.0/pathvalidate.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 02:56:27.000000 pathvalidate-3.1.0/pathvalidate.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      190 2023-07-16 02:56:49.000000 pathvalidate-3.1.0/pathvalidate.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-07-16 02:56:49.000000 pathvalidate-3.1.0/pathvalidate.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1288 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.981691 pathvalidate-3.1.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       46 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      121 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-16 02:56:49.991691 pathvalidate-3.1.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     3029 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:49.991691 pathvalidate-3.1.0/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1875 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4270 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_argparse.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2325 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_click.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1569 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1384 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    23234 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_filename.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    30197 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_filepath.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2500 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_ltsv.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4342 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/test/test_symbol.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1596 2023-07-16 02:56:17.000000 pathvalidate-3.1.0/tox.ini
```

### Comparing `pathvalidate-3.0.0/LICENSE` & `pathvalidate-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/PKG-INFO` & `pathvalidate-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathvalidate
-Version: 3.0.0
+Version: 3.1.0
 Summary: pathvalidate is a Python library to sanitize/validate a string such as filenames/file-paths/etc.
 Home-page: https://github.com/thombashi/pathvalidate
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://pathvalidate.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/pathvalidate
@@ -13,29 +13,29 @@
 Keywords: file,path,validation,validator,sanitization,sanitizer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **pathvalidate**
    :backlinks: top
    :depth: 2
 
@@ -74,15 +74,15 @@
 Features
 ---------
 - Sanitize/Validate a string as a:
     - file name
     - file path
 - file name/path argument validator/sanitizer for ``argparse`` and ``click``
 - Multi platform support:
-    - sanitize/validate file names/paths for a specific platform (``Linux``/``Windows``/``macOS``/``Posix``) or ``universal`` (platform independent)
+    - sanitize/validate file names/paths for a specific platform (``Linux``/``Windows``/``macOS``/``POSIX``) or ``universal`` (platform independent)
 - Multibyte character support
 
 Examples
 ==========
 Sanitize a filename
 ---------------------
 :Sample Code:
@@ -143,17 +143,17 @@
             validate_filename("COM1")
         except ValidationError as e:
             print(f"{e}\n", file=sys.stderr)
 
 :Output:
     .. code-block::
 
-        invalid char found: invalids=(':', '*', '/', '"', '?', '>', '|', '<'), value='fi:l*e/p"a?t>h|.t<xt', reason=INVALID_CHARACTER, target-platform=Windows
+        [PV1100] invalid characters found: target-platform=universal, description=invalids=('/'), value='fi:l*e/p"a?t>h|.t<xt'
 
-        'COM1' is a reserved name, reason=RESERVED_NAME, target-platform=universal
+        [PV1002] found a reserved name by a platform: 'COM1' is a reserved name, target-platform=universal, reusable_name=False
 
 Check a filename
 ------------------
 :Sample Code:
     .. code-block:: python
 
         from pathvalidate import is_valid_filename, sanitize_filename
@@ -167,48 +167,48 @@
 :Output:
     .. code-block::
 
         is_valid_filename('fi:l*e/p"a?t>h|.t<xt') return False
 
         is_valid_filename('filepath.txt') return True
 
-filename/filepath validator for argparse
-------------------------------------------
+filename/filepath validator for ``argparse``
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         from argparse import ArgumentParser
 
         from pathvalidate.argparse import validate_filename_arg, validate_filepath_arg
 
         parser = ArgumentParser()
-        parser.add_argument("--filepath", type=validate_filepath_arg)
         parser.add_argument("--filename", type=validate_filename_arg)
+        parser.add_argument("--filepath", type=validate_filepath_arg)
         options = parser.parse_args()
 
         if options.filename:
-            print("filename: {}".format(options.filename))
+            print(f"filename: {options.filename}")
 
         if options.filepath:
-            print("filepath: {}".format(options.filepath))
+            print(f"filepath: {options.filepath}")
 
 :Output:
     .. code-block::
 
         $ ./examples/argparse_validate.py --filename eg
         filename: eg
-        $ ./examples/argparse_validate.py --filepath e?g
-        usage: argparse_validate.py [-h] [--filepath FILEPATH] [--filename FILENAME]
-        argparse_validate.py: error: argument --filepath: invalid char found: invalids=('?'), value='e?g', reason=INVALID_CHARACTER, target-platform=Windows
+        $ ./examples/argparse_validate.py --filename e?g
+        usage: argparse_validate.py [-h] [--filename FILENAME] [--filepath FILEPATH]
+        argparse_validate.py: error: argument --filename: [PV1100] invalid characters found: invalids=(':'), value='e:g', target-platform=Windows
 
 .. note::
     ``validate_filepath_arg`` consider ``platform`` as of ``"auto"`` if the input is an absolute file path.
 
-filename/filepath sanitizer for argparse
-------------------------------------------
+filename/filepath sanitizer for ``argparse``
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         from argparse import ArgumentParser
 
         from pathvalidate.argparse import sanitize_filename_arg, sanitize_filepath_arg
 
@@ -229,65 +229,66 @@
 
         $ ./examples/argparse_sanitize.py --filename e/g
         filename: eg
 
 .. note::
     ``sanitize_filepath_arg`` is set platform as ``"auto"``.
 
-filename/filepath validator for click
----------------------------------------
+filename/filepath validator for ``click``
+-------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import click
 
         from pathvalidate.click import validate_filename_arg, validate_filepath_arg
 
 
         @click.command()
         @click.option("--filename", callback=validate_filename_arg)
         @click.option("--filepath", callback=validate_filepath_arg)
-        def cli(filename, filepath):
+        def cli(filename: str, filepath: str) -> None:
             if filename:
-                click.echo("filename: {}".format(filename))
+                click.echo(f"filename: {filename}")
             if filepath:
-                click.echo("filepath: {}".format(filepath))
+                click.echo(f"filepath: {filepath}")
 
 
         if __name__ == "__main__":
             cli()
 
 :Output:
     .. code-block::
 
         $ ./examples/click_validate.py --filename ab
         filename: ab
         $ ./examples/click_validate.py --filepath e?g
         Usage: click_validate.py [OPTIONS]
+        Try 'click_validate.py --help' for help.
 
-        Error: Invalid value for "--filepath": invalid char found: invalids=('?'), value='e?g', reason=INVALID_CHARACTER, target-platform=Windows
+        Error: Invalid value for '--filename': [PV1100] invalid characters found: invalids=('?'), value='e?g', target-platform=Windows
 
-filename/filepath sanitizer for click
----------------------------------------
+filename/filepath sanitizer for ``click``
+-------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import click
 
         from pathvalidate.click import sanitize_filename_arg, sanitize_filepath_arg
 
 
         @click.command()
         @click.option("--filename", callback=sanitize_filename_arg)
         @click.option("--filepath", callback=sanitize_filepath_arg)
         def cli(filename, filepath):
             if filename:
-                click.echo("filename: {}".format(filename))
+                click.echo(f"filename: {filename}")
             if filepath:
-                click.echo("filepath: {}".format(filepath))
+                click.echo(f"filepath: {filepath}")
 
 
         if __name__ == "__main__":
             cli()
 
 :Output:
     .. code-block::
@@ -321,15 +322,15 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-pathvalidate
 
 
 Dependencies
 ============
-Python 3.6+
+Python 3.7+
 no external dependencies.
 
 Documentation
 ===============
 https://pathvalidate.rtfd.io/
 
 Sponsors
```

### Comparing `pathvalidate-3.0.0/README.rst` & `pathvalidate-3.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 Features
 ---------
 - Sanitize/Validate a string as a:
     - file name
     - file path
 - file name/path argument validator/sanitizer for ``argparse`` and ``click``
 - Multi platform support:
-    - sanitize/validate file names/paths for a specific platform (``Linux``/``Windows``/``macOS``/``Posix``) or ``universal`` (platform independent)
+    - sanitize/validate file names/paths for a specific platform (``Linux``/``Windows``/``macOS``/``POSIX``) or ``universal`` (platform independent)
 - Multibyte character support
 
 Examples
 ==========
 Sanitize a filename
 ---------------------
 :Sample Code:
@@ -106,17 +106,17 @@
             validate_filename("COM1")
         except ValidationError as e:
             print(f"{e}\n", file=sys.stderr)
 
 :Output:
     .. code-block::
 
-        invalid char found: invalids=(':', '*', '/', '"', '?', '>', '|', '<'), value='fi:l*e/p"a?t>h|.t<xt', reason=INVALID_CHARACTER, target-platform=Windows
+        [PV1100] invalid characters found: target-platform=universal, description=invalids=('/'), value='fi:l*e/p"a?t>h|.t<xt'
 
-        'COM1' is a reserved name, reason=RESERVED_NAME, target-platform=universal
+        [PV1002] found a reserved name by a platform: 'COM1' is a reserved name, target-platform=universal, reusable_name=False
 
 Check a filename
 ------------------
 :Sample Code:
     .. code-block:: python
 
         from pathvalidate import is_valid_filename, sanitize_filename
@@ -130,48 +130,48 @@
 :Output:
     .. code-block::
 
         is_valid_filename('fi:l*e/p"a?t>h|.t<xt') return False
 
         is_valid_filename('filepath.txt') return True
 
-filename/filepath validator for argparse
-------------------------------------------
+filename/filepath validator for ``argparse``
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         from argparse import ArgumentParser
 
         from pathvalidate.argparse import validate_filename_arg, validate_filepath_arg
 
         parser = ArgumentParser()
-        parser.add_argument("--filepath", type=validate_filepath_arg)
         parser.add_argument("--filename", type=validate_filename_arg)
+        parser.add_argument("--filepath", type=validate_filepath_arg)
         options = parser.parse_args()
 
         if options.filename:
-            print("filename: {}".format(options.filename))
+            print(f"filename: {options.filename}")
 
         if options.filepath:
-            print("filepath: {}".format(options.filepath))
+            print(f"filepath: {options.filepath}")
 
 :Output:
     .. code-block::
 
         $ ./examples/argparse_validate.py --filename eg
         filename: eg
-        $ ./examples/argparse_validate.py --filepath e?g
-        usage: argparse_validate.py [-h] [--filepath FILEPATH] [--filename FILENAME]
-        argparse_validate.py: error: argument --filepath: invalid char found: invalids=('?'), value='e?g', reason=INVALID_CHARACTER, target-platform=Windows
+        $ ./examples/argparse_validate.py --filename e?g
+        usage: argparse_validate.py [-h] [--filename FILENAME] [--filepath FILEPATH]
+        argparse_validate.py: error: argument --filename: [PV1100] invalid characters found: invalids=(':'), value='e:g', target-platform=Windows
 
 .. note::
     ``validate_filepath_arg`` consider ``platform`` as of ``"auto"`` if the input is an absolute file path.
 
-filename/filepath sanitizer for argparse
-------------------------------------------
+filename/filepath sanitizer for ``argparse``
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         from argparse import ArgumentParser
 
         from pathvalidate.argparse import sanitize_filename_arg, sanitize_filepath_arg
 
@@ -192,65 +192,66 @@
 
         $ ./examples/argparse_sanitize.py --filename e/g
         filename: eg
 
 .. note::
     ``sanitize_filepath_arg`` is set platform as ``"auto"``.
 
-filename/filepath validator for click
----------------------------------------
+filename/filepath validator for ``click``
+-------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import click
 
         from pathvalidate.click import validate_filename_arg, validate_filepath_arg
 
 
         @click.command()
         @click.option("--filename", callback=validate_filename_arg)
         @click.option("--filepath", callback=validate_filepath_arg)
-        def cli(filename, filepath):
+        def cli(filename: str, filepath: str) -> None:
             if filename:
-                click.echo("filename: {}".format(filename))
+                click.echo(f"filename: {filename}")
             if filepath:
-                click.echo("filepath: {}".format(filepath))
+                click.echo(f"filepath: {filepath}")
 
 
         if __name__ == "__main__":
             cli()
 
 :Output:
     .. code-block::
 
         $ ./examples/click_validate.py --filename ab
         filename: ab
         $ ./examples/click_validate.py --filepath e?g
         Usage: click_validate.py [OPTIONS]
+        Try 'click_validate.py --help' for help.
 
-        Error: Invalid value for "--filepath": invalid char found: invalids=('?'), value='e?g', reason=INVALID_CHARACTER, target-platform=Windows
+        Error: Invalid value for '--filename': [PV1100] invalid characters found: invalids=('?'), value='e?g', target-platform=Windows
 
-filename/filepath sanitizer for click
----------------------------------------
+filename/filepath sanitizer for ``click``
+-------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import click
 
         from pathvalidate.click import sanitize_filename_arg, sanitize_filepath_arg
 
 
         @click.command()
         @click.option("--filename", callback=sanitize_filename_arg)
         @click.option("--filepath", callback=sanitize_filepath_arg)
         def cli(filename, filepath):
             if filename:
-                click.echo("filename: {}".format(filename))
+                click.echo(f"filename: {filename}")
             if filepath:
-                click.echo("filepath: {}".format(filepath))
+                click.echo(f"filepath: {filepath}")
 
 
         if __name__ == "__main__":
             cli()
 
 :Output:
     .. code-block::
@@ -284,15 +285,15 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-pathvalidate
 
 
 Dependencies
 ============
-Python 3.6+
+Python 3.7+
 no external dependencies.
 
 Documentation
 ===============
 https://pathvalidate.rtfd.io/
 
 Sponsors
```

### Comparing `pathvalidate-3.0.0/pathvalidate/__init__.py` & `pathvalidate-3.1.0/pathvalidate/__init__.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/pathvalidate/_base.py` & `pathvalidate-3.1.0/pathvalidate/_base.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/pathvalidate/_common.py` & `pathvalidate-3.1.0/pathvalidate/_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import platform
 import re
 import string
-from pathlib import Path
+from pathlib import PurePath
 from typing import Any, List, Optional
 
 from ._const import Platform
 from ._types import PathType, PlatformType
 
 
 _re_whitespaces = re.compile(r"^[\s]+$")
 
 
 def validate_pathtype(
     text: PathType, allow_whitespaces: bool = False, error_msg: Optional[str] = None
 ) -> None:
     from .error import ErrorReason, ValidationError
 
-    if _is_not_null_string(text) or isinstance(text, Path):
+    if _is_not_null_string(text) or isinstance(text, PurePath):
         return
 
     if allow_whitespaces and _re_whitespaces.search(str(text)):
         return
 
     if is_null_string(text):
         raise ValidationError(reason=ErrorReason.NULL_NAME)
 
     raise TypeError(f"text must be a string: actual={type(text)}")
 
 
 def to_str(name: PathType) -> str:
-    if isinstance(name, Path):
+    if isinstance(name, PurePath):
         return str(name)
 
     return name
 
 
 def is_null_string(value: Any) -> bool:
     if value is None:
```

### Comparing `pathvalidate-3.0.0/pathvalidate/_const.py` & `pathvalidate-3.1.0/pathvalidate/_const.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,13 +21,20 @@
     "$ObjId",
     "$Reparse",
 )  # Only in root directory
 
 
 @enum.unique
 class Platform(enum.Enum):
+    """
+    Platform specifier enumeration.
+    """
+
+    #: POSIX compatible platform.
     POSIX = "POSIX"
+
+    #: platform independent. note that absolute paths cannot specify this.
     UNIVERSAL = "universal"
 
     LINUX = "Linux"
     WINDOWS = "Windows"
     MACOS = "macOS"
```

### Comparing `pathvalidate-3.0.0/pathvalidate/_filename.py` & `pathvalidate-3.1.0/pathvalidate/_filename.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import itertools
 import ntpath
 import posixpath
 import re
-from pathlib import Path
+from pathlib import Path, PurePath
 from typing import Optional, Pattern, Tuple
 
 from ._base import AbstractSanitizer, AbstractValidator, BaseFile, BaseValidator
 from ._common import findall_to_str, to_str, validate_pathtype
 from ._const import DEFAULT_MIN_LEN, INVALID_CHAR_ERR_MSG_TMPL, Platform
 from ._types import PathType, PlatformType
 from .error import ErrorReason, InvalidCharError, ValidationError
@@ -60,15 +60,15 @@
         self._sanitize_regexp = self._get_sanitize_regexp()
 
     def sanitize(self, value: PathType, replacement_text: str = "") -> PathType:
         try:
             validate_pathtype(value, allow_whitespaces=not self._is_windows(include_universal=True))
         except ValidationError as e:
             if e.reason == ErrorReason.NULL_NAME:
-                if isinstance(value, Path):
+                if isinstance(value, PurePath):
                     raise
 
                 return self._null_value_handler(e)
             raise
 
         sanitized_filename = self._sanitize_regexp.sub(replacement_text, str(value))
         sanitized_filename = sanitized_filename[: self.max_len]
@@ -99,15 +99,15 @@
             except ValidationError as e:
                 raise ValidationError(
                     description=str(e),
                     reason=ErrorReason.INVALID_AFTER_SANITIZE,
                     platform=self.platform,
                 )
 
-        if isinstance(value, Path):
+        if isinstance(value, PurePath):
             return Path(sanitized_filename)
 
         return sanitized_filename
 
     def _get_sanitize_regexp(self) -> Pattern[str]:
         if self._is_windows(include_universal=True):
             return _RE_INVALID_WIN_FILENAME
@@ -182,19 +182,18 @@
                 [
                     f"filename is too short: expected>={self.min_len:d} bytes, actual={byte_ct:d} bytes"
                 ],
                 **err_kwargs,
             )
 
         self._validate_reserved_keywords(unicode_filename)
+        self.__validate_universal_filename(unicode_filename)
 
         if self._is_windows(include_universal=True):
             self.__validate_win_filename(unicode_filename)
-        else:
-            self.__validate_unix_filename(unicode_filename)
 
     def validate_abspath(self, value: str) -> None:
         err = ValidationError(
             description=f"found an absolute path ({value}), expected a filename",
             platform=self.platform,
             reason=ErrorReason.FOUND_ABS_PATH,
         )
@@ -202,21 +201,22 @@
         if self._is_windows(include_universal=True):
             if ntpath.isabs(value):
                 raise err
 
         if posixpath.isabs(value):
             raise err
 
-    def __validate_unix_filename(self, unicode_filename: str) -> None:
+    def __validate_universal_filename(self, unicode_filename: str) -> None:
         match = _RE_INVALID_FILENAME.findall(unicode_filename)
         if match:
             raise InvalidCharError(
                 INVALID_CHAR_ERR_MSG_TMPL.format(
                     invalid=findall_to_str(match), value=repr(unicode_filename)
-                )
+                ),
+                platform=Platform.UNIVERSAL,
             )
 
     def __validate_win_filename(self, unicode_filename: str) -> None:
         match = _RE_INVALID_WIN_FILENAME.findall(unicode_filename)
         if match:
             raise InvalidCharError(
                 INVALID_CHAR_ERR_MSG_TMPL.format(
```

### Comparing `pathvalidate-3.0.0/pathvalidate/_filepath.py` & `pathvalidate-3.1.0/pathvalidate/_filepath.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import ntpath
 import os.path
 import posixpath
 import re
-from pathlib import Path
+from pathlib import Path, PurePath
 from typing import List, Optional, Pattern, Tuple
 
 from ._base import AbstractSanitizer, AbstractValidator, BaseFile, BaseValidator
 from ._common import findall_to_str, to_str, validate_pathtype
 from ._const import _NTFS_RESERVED_FILE_NAMES, DEFAULT_MIN_LEN, INVALID_CHAR_ERR_MSG_TMPL, Platform
 from ._filename import FileNameSanitizer, FileNameValidator
 from ._types import PathType, PlatformType
@@ -71,15 +71,15 @@
             self.__split_drive = posixpath.splitdrive
 
     def sanitize(self, value: PathType, replacement_text: str = "") -> PathType:
         try:
             validate_pathtype(value, allow_whitespaces=not self._is_windows(include_universal=True))
         except ValidationError as e:
             if e.reason == ErrorReason.NULL_NAME:
-                if isinstance(value, Path):
+                if isinstance(value, PurePath):
                     raise
 
                 return self._null_value_handler(e)
             raise
 
         unicode_filepath = to_str(value)
 
@@ -113,15 +113,15 @@
         except ValidationError as e:
             if e.reason == ErrorReason.NULL_NAME:
                 sanitized_path = self._null_value_handler(e)
 
         if self._validate_after_sanitize:
             self._validator.validate(sanitized_path)
 
-        if isinstance(value, Path):
+        if isinstance(value, PurePath):
             return Path(sanitized_path)
 
         return sanitized_path
 
     def _get_sanitize_regexp(self) -> Pattern[str]:
         if self._is_windows(include_universal=True):
             return _RE_INVALID_WIN_PATH
@@ -299,35 +299,35 @@
     max_len: Optional[int] = None,
     fs_encoding: Optional[str] = None,
     check_reserved: bool = True,
 ) -> None:
     """Verifying whether the ``file_path`` is a valid file path or not.
 
     Args:
-        file_path:
-            File path to validate.
-        platform:
+        file_path (PathType):
+            File path to be validated.
+        platform (Optional[PlatformType], optional):
             Target platform name of the file path.
 
             .. include:: platform.txt
-        min_len:
+        min_len (int, optional):
             Minimum byte length of the ``file_path``. The value must be greater or equal to one.
             Defaults to ``1``.
-        max_len:
+        max_len (Optional[int], optional):
             Maximum byte length of the ``file_path``. If the value is |None| or minus,
             automatically determined by the ``platform``:
 
                 - ``Linux``: 4096
                 - ``macOS``: 1024
                 - ``Windows``: 260
                 - ``universal``: 260
-        fs_encoding:
+        fs_encoding (Optional[str], optional):
             Filesystem encoding that used to calculate the byte length of the file path.
             If |None|, get the value from the execution environment.
-        check_reserved:
+        check_reserved (bool, optional):
             If |True|, check reserved names of the ``platform``.
 
     Raises:
         ValidationError (ErrorReason.INVALID_CHARACTER):
             If the ``file_path`` includes invalid char(s):
             |invalid_file_path_chars|.
             The following characters are also invalid for Windows platforms:
```

### Comparing `pathvalidate-3.0.0/pathvalidate/_ltsv.py` & `pathvalidate-3.1.0/pathvalidate/_ltsv.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/pathvalidate/_symbol.py` & `pathvalidate-3.1.0/pathvalidate/_symbol.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/pathvalidate/argparse.py` & `pathvalidate-3.1.0/pathvalidate/argparse.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/pathvalidate/click.py` & `pathvalidate-3.1.0/pathvalidate/click.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/pathvalidate.egg-info/PKG-INFO` & `pathvalidate-3.1.0/pathvalidate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathvalidate
-Version: 3.0.0
+Version: 3.1.0
 Summary: pathvalidate is a Python library to sanitize/validate a string such as filenames/file-paths/etc.
 Home-page: https://github.com/thombashi/pathvalidate
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://pathvalidate.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/pathvalidate
@@ -13,29 +13,29 @@
 Keywords: file,path,validation,validator,sanitization,sanitizer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **pathvalidate**
    :backlinks: top
    :depth: 2
 
@@ -74,15 +74,15 @@
 Features
 ---------
 - Sanitize/Validate a string as a:
     - file name
     - file path
 - file name/path argument validator/sanitizer for ``argparse`` and ``click``
 - Multi platform support:
-    - sanitize/validate file names/paths for a specific platform (``Linux``/``Windows``/``macOS``/``Posix``) or ``universal`` (platform independent)
+    - sanitize/validate file names/paths for a specific platform (``Linux``/``Windows``/``macOS``/``POSIX``) or ``universal`` (platform independent)
 - Multibyte character support
 
 Examples
 ==========
 Sanitize a filename
 ---------------------
 :Sample Code:
@@ -143,17 +143,17 @@
             validate_filename("COM1")
         except ValidationError as e:
             print(f"{e}\n", file=sys.stderr)
 
 :Output:
     .. code-block::
 
-        invalid char found: invalids=(':', '*', '/', '"', '?', '>', '|', '<'), value='fi:l*e/p"a?t>h|.t<xt', reason=INVALID_CHARACTER, target-platform=Windows
+        [PV1100] invalid characters found: target-platform=universal, description=invalids=('/'), value='fi:l*e/p"a?t>h|.t<xt'
 
-        'COM1' is a reserved name, reason=RESERVED_NAME, target-platform=universal
+        [PV1002] found a reserved name by a platform: 'COM1' is a reserved name, target-platform=universal, reusable_name=False
 
 Check a filename
 ------------------
 :Sample Code:
     .. code-block:: python
 
         from pathvalidate import is_valid_filename, sanitize_filename
@@ -167,48 +167,48 @@
 :Output:
     .. code-block::
 
         is_valid_filename('fi:l*e/p"a?t>h|.t<xt') return False
 
         is_valid_filename('filepath.txt') return True
 
-filename/filepath validator for argparse
-------------------------------------------
+filename/filepath validator for ``argparse``
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         from argparse import ArgumentParser
 
         from pathvalidate.argparse import validate_filename_arg, validate_filepath_arg
 
         parser = ArgumentParser()
-        parser.add_argument("--filepath", type=validate_filepath_arg)
         parser.add_argument("--filename", type=validate_filename_arg)
+        parser.add_argument("--filepath", type=validate_filepath_arg)
         options = parser.parse_args()
 
         if options.filename:
-            print("filename: {}".format(options.filename))
+            print(f"filename: {options.filename}")
 
         if options.filepath:
-            print("filepath: {}".format(options.filepath))
+            print(f"filepath: {options.filepath}")
 
 :Output:
     .. code-block::
 
         $ ./examples/argparse_validate.py --filename eg
         filename: eg
-        $ ./examples/argparse_validate.py --filepath e?g
-        usage: argparse_validate.py [-h] [--filepath FILEPATH] [--filename FILENAME]
-        argparse_validate.py: error: argument --filepath: invalid char found: invalids=('?'), value='e?g', reason=INVALID_CHARACTER, target-platform=Windows
+        $ ./examples/argparse_validate.py --filename e?g
+        usage: argparse_validate.py [-h] [--filename FILENAME] [--filepath FILEPATH]
+        argparse_validate.py: error: argument --filename: [PV1100] invalid characters found: invalids=(':'), value='e:g', target-platform=Windows
 
 .. note::
     ``validate_filepath_arg`` consider ``platform`` as of ``"auto"`` if the input is an absolute file path.
 
-filename/filepath sanitizer for argparse
-------------------------------------------
+filename/filepath sanitizer for ``argparse``
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         from argparse import ArgumentParser
 
         from pathvalidate.argparse import sanitize_filename_arg, sanitize_filepath_arg
 
@@ -229,65 +229,66 @@
 
         $ ./examples/argparse_sanitize.py --filename e/g
         filename: eg
 
 .. note::
     ``sanitize_filepath_arg`` is set platform as ``"auto"``.
 
-filename/filepath validator for click
----------------------------------------
+filename/filepath validator for ``click``
+-------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import click
 
         from pathvalidate.click import validate_filename_arg, validate_filepath_arg
 
 
         @click.command()
         @click.option("--filename", callback=validate_filename_arg)
         @click.option("--filepath", callback=validate_filepath_arg)
-        def cli(filename, filepath):
+        def cli(filename: str, filepath: str) -> None:
             if filename:
-                click.echo("filename: {}".format(filename))
+                click.echo(f"filename: {filename}")
             if filepath:
-                click.echo("filepath: {}".format(filepath))
+                click.echo(f"filepath: {filepath}")
 
 
         if __name__ == "__main__":
             cli()
 
 :Output:
     .. code-block::
 
         $ ./examples/click_validate.py --filename ab
         filename: ab
         $ ./examples/click_validate.py --filepath e?g
         Usage: click_validate.py [OPTIONS]
+        Try 'click_validate.py --help' for help.
 
-        Error: Invalid value for "--filepath": invalid char found: invalids=('?'), value='e?g', reason=INVALID_CHARACTER, target-platform=Windows
+        Error: Invalid value for '--filename': [PV1100] invalid characters found: invalids=('?'), value='e?g', target-platform=Windows
 
-filename/filepath sanitizer for click
----------------------------------------
+filename/filepath sanitizer for ``click``
+-------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import click
 
         from pathvalidate.click import sanitize_filename_arg, sanitize_filepath_arg
 
 
         @click.command()
         @click.option("--filename", callback=sanitize_filename_arg)
         @click.option("--filepath", callback=sanitize_filepath_arg)
         def cli(filename, filepath):
             if filename:
-                click.echo("filename: {}".format(filename))
+                click.echo(f"filename: {filename}")
             if filepath:
-                click.echo("filepath: {}".format(filepath))
+                click.echo(f"filepath: {filepath}")
 
 
         if __name__ == "__main__":
             cli()
 
 :Output:
     .. code-block::
@@ -321,15 +322,15 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-pathvalidate
 
 
 Dependencies
 ============
-Python 3.6+
+Python 3.7+
 no external dependencies.
 
 Documentation
 ===============
 https://pathvalidate.rtfd.io/
 
 Sponsors
```

### Comparing `pathvalidate-3.0.0/pathvalidate.egg-info/SOURCES.txt` & `pathvalidate-3.1.0/pathvalidate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/pyproject.toml` & `pathvalidate-3.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

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
@@ -54,15 +55,15 @@
     'abstractproperty',
     'abstractclassmethod',
     'warnings.warn',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `pathvalidate-3.0.0/setup.py` & `pathvalidate-3.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
 with open(os.path.join("docs", "pages", "introduction", "summary.txt"), encoding=ENCODING) as f:
     summary = f.read().strip()
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
+with open(os.path.join(REQUIREMENT_DIR, "docs_requirements.txt")) as f:
+    docs_requires = [line.strip() for line in f if line.strip()]
+
 setuptools.setup(
     name=MODULE_NAME,
     version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description=summary,
@@ -53,24 +56,26 @@
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Documentation": f"https://{MODULE_NAME:s}.rtfd.io/",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
         "Changlog": f"{REPOSITORY_URL:s}/releases",
     },
-    python_requires=">=3.6",
-    extras_require={"test": TESTS_REQUIRES},
+    python_requires=">=3.7",
+    extras_require={
+        "docs": docs_requires,
+        "test": TESTS_REQUIRES,
+    },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `pathvalidate-3.0.0/test/_common.py` & `pathvalidate-3.1.0/test/_common.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/test/test_argparse.py` & `pathvalidate-3.1.0/test/test_argparse.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/test/test_click.py` & `pathvalidate-3.1.0/test/test_click.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/test/test_common.py` & `pathvalidate-3.1.0/test/test_common.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/test/test_filename.py` & `pathvalidate-3.1.0/test/test_filename.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import platform as m_platform
 import random
 import sys
 from collections import OrderedDict
 from itertools import chain, product
-from pathlib import Path
+from pathlib import Path, PurePosixPath, PureWindowsPath
 
 import pytest
 from allpairspy import AllPairs
 
 from pathvalidate import (
     ErrorReason,
     Platform,
@@ -287,14 +287,29 @@
             validate_filename(value, platform)
         assert e.value.reason == ErrorReason.INVALID_CHARACTER
         assert not is_valid_filename(value, platform=platform)
 
     @pytest.mark.parametrize(
         ["value", "platform"],
         [
+            ["a/b", Platform.UNIVERSAL],
+            ["a*b", Platform.WINDOWS],
+            [PurePosixPath("a/b"), Platform.UNIVERSAL],
+            [PureWindowsPath("a/b"), Platform.WINDOWS],
+        ],
+    )
+    def test_exception_invalid_char_specific_target_platform(self, value, platform):
+        with pytest.raises(ValidationError) as e:
+            validate_filename(value, platform)
+        assert e.value.reason == ErrorReason.INVALID_CHARACTER
+        assert e.value.platform == platform
+
+    @pytest.mark.parametrize(
+        ["value", "platform"],
+        [
             ["{0}{1}{0}".format(randstr(64), invalid_c), platform]
             for invalid_c, platform in product(
                 set(INVALID_WIN_PATH_CHARS).difference(
                     set(INVALID_PATH_CHARS + INVALID_FILENAME_CHARS + unprintable_ascii_chars)
                 ),
                 ["windows", "universal"],
             )
@@ -636,15 +651,15 @@
     )
     def test_exception_invalid_after_sanitize(self, platform, value):
         kwargs = {
             "platform": platform,
             "replacement_text": "",
             "validate_after_sanitize": False,
         }
-        print("'{}'".format(sanitize_filename(value, **kwargs)), file=sys.stderr)
+        print(f"'{sanitize_filename(value, **kwargs)}'", file=sys.stderr)
         kwargs["validate_after_sanitize"] = True
 
         with pytest.raises(ValidationError) as e:
             sanitize_filename(value, **kwargs)
         assert e.value.reason == ErrorReason.INVALID_AFTER_SANITIZE
 
     @pytest.mark.parametrize(
```

### Comparing `pathvalidate-3.0.0/test/test_filepath.py` & `pathvalidate-3.1.0/test/test_filepath.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,15 +821,14 @@
             ),
             file=sys.stderr,
         )
         with pytest.raises(ValidationError) as e:
             sanitize_filepath(value, platform=platform, validate_after_sanitize=True)
         assert e.value.reason == ErrorReason.INVALID_AFTER_SANITIZE
 
-    @pytest.mark.skipif(sys.version_info < (3, 6), reason="requires python3.6 or higher")
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             [1, TypeError],
             [True, TypeError],
             [nan, TypeError],
             [inf, TypeError],
```

### Comparing `pathvalidate-3.0.0/test/test_ltsv.py` & `pathvalidate-3.1.0/test/test_ltsv.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/test/test_symbol.py` & `pathvalidate-3.1.0/test/test_symbol.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-3.0.0/tox.ini` & `pathvalidate-3.1.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{36,37,38,39,310,311}
+    py{37,38,39,310,311}
     pypy3
     build
     cov
     docs
     fmt
     lint
     readme
@@ -17,20 +17,20 @@
 allowlist_externals =
     pytest
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
@@ -41,18 +41,18 @@
 deps =
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:docs]
-deps =
-    -r{toxinidir}/requirements/docs_requirements.txt
+extras =
+    docs
 commands =
-    python setup.py build_sphinx --source-dir=docs/ --build-dir=docs/_build --all-files
+    sphinx-build docs/ docs/_build
 
 [testenv:fmt]
 skip_install = true
 deps =
     autoflake>=2
     black>=23.1
     isort>=5
@@ -65,19 +65,30 @@
 skip_install = true
 deps =
     codespell>=2
     mypy>=1
     pylama>=8.4.1
     types-click
 commands =
-    python setup.py check
     mypy pathvalidate setup.py
     codespell pathvalidate docs/pages examples test -q2 --check-filenames
     pylama pathvalidate test setup.py
 
+[testenv:lint-examples]
+skip_install = true
+changedir = examples
+deps =
+    jupyter
+    mypy>=1
+    pathvalidate>=3
+    types-click
+commands =
+    jupyter nbconvert pathvalidate_examples.ipynb --to python
+    mypy pathvalidate_examples.py --strict
+
 [testenv:readme]
 skip_install = true
 changedir = docs
 deps =
     readmemaker>=1.1.0
 commands =
     python make_readme.py
```

