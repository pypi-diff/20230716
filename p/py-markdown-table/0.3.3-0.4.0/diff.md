# Comparing `tmp/py-markdown-table-0.3.3.tar.gz` & `tmp/py-markdown-table-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-markdown-table-0.3.3.tar", last modified: Wed Aug 17 19:51:03 2022, max compression
+gzip compressed data, was "py-markdown-table-0.4.0.tar", last modified: Sun Jul 16 10:57:11 2023, max compression
```

## Comparing `py-markdown-table-0.3.3.tar` & `py-markdown-table-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-17 19:51:03.454298 py-markdown-table-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2022-08-17 19:50:47.000000 py-markdown-table-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     8822 2022-08-17 19:51:03.454298 py-markdown-table-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8384 2022-08-17 19:50:47.000000 py-markdown-table-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-17 19:51:03.454298 py-markdown-table-0.3.3/markdownTable/
--rw-r--r--   0 runner    (1001) docker     (116)     2528 2022-08-17 19:50:47.000000 py-markdown-table-0.3.3/markdownTable/__gendesc__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9392 2022-08-17 19:50:47.000000 py-markdown-table-0.3.3/markdownTable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-17 19:51:03.454298 py-markdown-table-0.3.3/py_markdown_table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8822 2022-08-17 19:51:03.000000 py-markdown-table-0.3.3/py_markdown_table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      245 2022-08-17 19:51:03.000000 py-markdown-table-0.3.3/py_markdown_table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-17 19:51:03.000000 py-markdown-table-0.3.3/py_markdown_table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-08-17 19:51:03.000000 py-markdown-table-0.3.3/py_markdown_table.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-08-17 19:51:03.454298 py-markdown-table-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      657 2022-08-17 19:50:47.000000 py-markdown-table-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 10:57:11.527527 py-markdown-table-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    25100 2023-07-16 10:57:11.523527 py-markdown-table-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24647 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 10:57:11.519528 py-markdown-table-0.4.0/markdownTable/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/markdownTable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 10:57:11.523527 py-markdown-table-0.4.0/py_markdown_table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/py_markdown_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27988 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/py_markdown_table/markdown_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/py_markdown_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 10:57:11.523527 py-markdown-table-0.4.0/py_markdown_table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25100 2023-07-16 10:57:11.000000 py-markdown-table-0.4.0/py_markdown_table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-16 10:57:11.000000 py-markdown-table-0.4.0/py_markdown_table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-16 10:57:11.000000 py-markdown-table-0.4.0/py_markdown_table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-16 10:57:11.000000 py-markdown-table-0.4.0/py_markdown_table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-16 10:57:11.000000 py-markdown-table-0.4.0/py_markdown_table.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-16 10:57:11.527527 py-markdown-table-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 10:57:11.523527 py-markdown-table-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12174 2023-07-16 10:56:59.000000 py-markdown-table-0.4.0/tests/tests.py
```

### Comparing `py-markdown-table-0.3.3/LICENSE` & `py-markdown-table-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-markdown-table-0.3.3/setup.py` & `py-markdown-table-0.4.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import setuptools
+from setuptools import setup,find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-setuptools.setup(
+setup(
     name="py-markdown-table",
-    version="0.3.3",
+    version="0.4.0",
     author="hvalev",
-    description="A package used to generate basic markdown tables from a list of dicts",
+    description="Package that generates markdown tables from a list of dicts",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/hvalev/markdownTable",
-    packages=['markdownTable'],
+    url="https://github.com/hvalev/py-markdown-table",
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
+    extras_require={"dev": ["pytest", "pytest-cov", "pylint", "black"]},
 )
```

