# Comparing `tmp/sphinxcontrib-xlsxtable-1.0.0.tar.gz` & `tmp/sphinxcontrib-xlsxtable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sphinxcontrib-xlsxtable-1.0.0.tar", last modified: Sun Jul 19 12:54:46 2020, max compression
+gzip compressed data, was "sphinxcontrib-xlsxtable-1.1.0.tar", last modified: Sun Jul 16 12:03:14 2023, max compression
```

## Comparing `sphinxcontrib-xlsxtable-1.0.0.tar` & `sphinxcontrib-xlsxtable-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/
--rw-rw-rw-   0        0        0      593 2020-07-19 12:53:29.000000 sphinxcontrib-xlsxtable-1.0.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1087 2020-03-03 12:57:07.000000 sphinxcontrib-xlsxtable-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       54 2020-03-11 14:09:26.000000 sphinxcontrib-xlsxtable-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5873 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3307 2020-07-19 07:45:18.000000 sphinxcontrib-xlsxtable-1.0.0/README.rst
--rw-rw-rw-   0        0        0       83 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1401 2020-07-19 12:53:29.000000 sphinxcontrib-xlsxtable-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/
--rw-rw-rw-   0        0        0      380 2020-03-08 01:51:57.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/
--rw-rw-rw-   0        0        0      151 2020-03-29 11:12:05.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/__init__.py
--rw-rw-rw-   0        0        0       55 2020-03-29 11:12:05.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/__main__.py
--rw-rw-rw-   0        0        0     8710 2020-07-19 08:09:34.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/xlsx2gridtable.py
--rw-rw-rw-   0        0        0     2381 2020-07-19 12:53:29.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/xlsxtable.py
-drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/
--rw-rw-rw-   0        0        0     5873 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      589 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        2 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/test/
--rw-rw-rw-   0        0        0     4518 2020-07-19 08:14:11.000000 sphinxcontrib-xlsxtable-1.0.0/test/test.py
+drwxr-xr-x   0 ayataka    (501) staff       (20)        0 2023-07-16 12:03:14.113070 sphinxcontrib-xlsxtable-1.1.0/
+-rw-r--r--   0 ayataka    (501) staff       (20)      660 2023-07-16 11:44:29.000000 sphinxcontrib-xlsxtable-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 ayataka    (501) staff       (20)     1066 2023-03-25 08:49:09.000000 sphinxcontrib-xlsxtable-1.1.0/LICENSE
+-rw-r--r--   0 ayataka    (501) staff       (20)       51 2023-03-25 08:49:09.000000 sphinxcontrib-xlsxtable-1.1.0/MANIFEST.in
+-rw-r--r--   0 ayataka    (501) staff       (20)     4562 2023-07-16 12:03:14.113167 sphinxcontrib-xlsxtable-1.1.0/PKG-INFO
+-rw-r--r--   0 ayataka    (501) staff       (20)     3682 2023-07-16 11:44:29.000000 sphinxcontrib-xlsxtable-1.1.0/README.rst
+-rw-r--r--   0 ayataka    (501) staff       (20)       76 2023-07-16 12:03:14.113703 sphinxcontrib-xlsxtable-1.1.0/setup.cfg
+-rw-r--r--   0 ayataka    (501) staff       (20)     1358 2023-07-16 11:44:29.000000 sphinxcontrib-xlsxtable-1.1.0/setup.py
+drwxr-xr-x   0 ayataka    (501) staff       (20)        0 2023-07-16 12:03:14.107650 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/
+-rw-r--r--   0 ayataka    (501) staff       (20)      366 2023-03-25 08:49:09.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/__init__.py
+drwxr-xr-x   0 ayataka    (501) staff       (20)        0 2023-07-16 12:03:14.109063 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/
+-rw-r--r--   0 ayataka    (501) staff       (20)      143 2023-05-28 13:12:42.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/__init__.py
+-rw-r--r--   0 ayataka    (501) staff       (20)       52 2023-03-25 08:49:09.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/__main__.py
+drwxr-xr-x   0 ayataka    (501) staff       (20)        0 2023-07-16 12:03:14.110057 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/workbook/
+-rw-r--r--   0 ayataka    (501) staff       (20)        0 2023-07-16 06:47:10.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/workbook/__init__.py
+-rw-r--r--   0 ayataka    (501) staff       (20)     8770 2023-07-16 06:47:10.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/workbook/workbook.py
+-rw-r--r--   0 ayataka    (501) staff       (20)    10403 2023-07-16 06:47:10.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/xlsx2gridtable.py
+-rw-r--r--   0 ayataka    (501) staff       (20)     2221 2023-07-16 11:44:29.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/xlsxtable.py
+drwxr-xr-x   0 ayataka    (501) staff       (20)        0 2023-07-16 12:03:14.112454 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/
+-rw-r--r--   0 ayataka    (501) staff       (20)     4562 2023-07-16 12:03:14.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/PKG-INFO
+-rw-r--r--   0 ayataka    (501) staff       (20)      679 2023-07-16 12:03:14.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt
+-rw-r--r--   0 ayataka    (501) staff       (20)        1 2023-07-16 12:03:14.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/dependency_links.txt
+-rw-r--r--   0 ayataka    (501) staff       (20)       14 2023-07-16 12:03:14.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/namespace_packages.txt
+-rw-r--r--   0 ayataka    (501) staff       (20)        1 2023-07-16 12:03:14.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/not-zip-safe
+-rw-r--r--   0 ayataka    (501) staff       (20)       30 2023-07-16 12:03:14.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/requires.txt
+-rw-r--r--   0 ayataka    (501) staff       (20)       14 2023-07-16 12:03:14.000000 sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/top_level.txt
+drwxr-xr-x   0 ayataka    (501) staff       (20)        0 2023-07-16 12:03:14.112644 sphinxcontrib-xlsxtable-1.1.0/test/
+-rw-r--r--   0 ayataka    (501) staff       (20)     5667 2023-07-16 06:47:10.000000 sphinxcontrib-xlsxtable-1.1.0/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sphinxcontrib-xlsxtable-1.0.0/CHANGELOG.rst` & `sphinxcontrib-xlsxtable-1.1.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.1.0 (2023-07-16)
+------------------
+
+- Support embedded images
+
+
 1.0.0 (2020-07-19)
 ------------------
 
 - Add ``start-column`` option
 - Add ``include-rows`` and ``exclude-rows`` optionals
 - Add ``include-columns`` and ``exclude-columns`` optional
```

### Comparing `sphinxcontrib-xlsxtable-1.0.0/README.rst` & `sphinxcontrib-xlsxtable-1.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 A sphinx extension for making table from Excel file.
 
 - Depends on `OpenPyXL <https://openpyxl.readthedocs.io/en/stable/>`__
 
   - Supports xlsx file
 
 - Supports merged cell
+- Supports images
 - Supports Japanese
 
 This extension **generates a grid table string internally** from Excel file.
 
 
 Install and Set up
 ==================
@@ -176,11 +177,19 @@
    | A3 |       | C3:D3          |
    +----+-------+-------+--------+
    | A4 | B4    | C4    | - D4-1 |
    |    |       |       | - D4-2 |
    +----+-------+-------+--------+
 
 
+Links
+=====
+
+- `sphinxcontrib-xlsxtableの解説 <https://kkayataka.hatenablog.com/entry/2020/03/14/140305>`__
+- `sphinxcontrib-xlsxtableのモジュール実行 <https://kkayataka.hatenablog.com/entry/2020/04/11/173717>`__
+- `sphinxcontrib-xlsxtableに行・列指定オプションを追加 <https://kkayataka.hatenablog.com/entry/2020/07/25/131440>`__
+
+
 LICENSE
 =======
 
 - MIT
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sphinxcontrib-xlsxtable-1.0.0/setup.py` & `sphinxcontrib-xlsxtable-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# -*- coding: utf-8 -*-
-
-from setuptools import setup, find_packages
-
-long_desc = ''
-with open("README.rst", "r") as fh:
-    long_desc = fh.read()
-
-setup(
-    name='sphinxcontrib-xlsxtable',
-    version='1.0.0',
-    url='https://github.com/kkAyataka/sphinxcontrib-xlsxtable',
-    download_url='http://pypi.python.org/pypi/sphinxcontrib-xlsxtable',
-    license='MIT',
-    author='kkAyataka',
-    author_email='kk.ayataka@gmail.com',
-    description='A sphinx extension for making table from Excel file',
-    long_description=long_desc,
-    long_description_content_type='text/x-rst',
-    zip_safe=False,
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Console',
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.0',
-        'Framework :: Sphinx :: Extension',
-        'Topic :: Documentation',
-        'Topic :: Utilities',
-    ],
-    platforms='any',
-    packages=find_packages(exclude=['test', 'test.*']),
-    include_package_data=True,
-    install_requires=[
-        'Sphinx >= 2.0.0',
-        'openpyxl >= 3.0.0',
-    ],
-    namespace_packages=['sphinxcontrib'],
-    test_suite='test',
-)
+# -*- coding: utf-8 -*-
+
+from setuptools import setup, find_packages
+
+long_desc = ''
+with open("README.rst", "r") as fh:
+    long_desc = fh.read()
+
+setup(
+    name='sphinxcontrib-xlsxtable',
+    version='1.1.0',
+    url='https://github.com/kkAyataka/sphinxcontrib-xlsxtable',
+    download_url='http://pypi.python.org/pypi/sphinxcontrib-xlsxtable',
+    license='MIT',
+    author='kkAyataka',
+    author_email='kk.ayataka@gmail.com',
+    description='A sphinx extension for making table from Excel file',
+    long_description=long_desc,
+    long_description_content_type='text/x-rst',
+    zip_safe=False,
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Environment :: Console',
+        'Environment :: Web Environment',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.0',
+        'Framework :: Sphinx :: Extension',
+        'Topic :: Documentation',
+        'Topic :: Utilities',
+    ],
+    platforms='any',
+    packages=find_packages(exclude=['test', 'test.*']),
+    include_package_data=True,
+    install_requires=[
+        'Sphinx >= 2.0.0',
+        'openpyxl >= 3.0.0',
+    ],
+    namespace_packages=['sphinxcontrib'],
+    test_suite='test',
+)
```

### Comparing `sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/xlsxtable.py` & `sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib/xlsxtable/xlsxtable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,66 @@
-import os
-from docutils import nodes
-from docutils.parsers.rst import directives
-from docutils.statemachine import ViewList
-
-from openpyxl import Workbook
-from openpyxl import load_workbook
-from openpyxl.cell.cell import MergedCell
-
-from .xlsx2gridtable import gen_reST_grid_table_lines
-
-
-class XlsxTable(directives.tables.RSTTable):
-    has_content = True
-
-    optional_arguments = 1
-    option_spec = {
-        'file': directives.path,
-        'header-rows': directives.positive_int,
-        'start-row': directives.positive_int,
-        'start-column': directives.positive_int,
-        'include-rows': directives.unchanged,
-        'exclude-rows': directives.unchanged,
-        'include-columns': directives.unchanged,
-        'exclude-columns': directives.unchanged,
-        'sheet': directives.unchanged,
-    }
-
-    def run(self):
-        filepath = self.options.get('file', '')
-        header_rows = self.options.get('header-rows', 0)
-        sheet = self.options.get('sheet', None)
-        start_row = self.options.get('start-row', 1)
-        start_column = self.options.get('start-column', 1)
-        include_rows = self.options.get('include-rows', None)
-        exclude_rows = self.options.get('exclude-rows', None)
-        include_columns = self.options.get('include-columns', None)
-        exclude_columns = self.options.get('exclude-columns', None)
-
-        rst_dir = os.path.dirname(os.path.abspath(self.state.document.current_source))
-        filepath = os.path.normpath(os.path.join(rst_dir, filepath))
-
-        lines = gen_reST_grid_table_lines(
-            filepath,
-            header_rows,
-            sheet,
-            start_row,
-            start_column,
-            include_rows, exclude_rows,
-            include_columns, exclude_columns)
-        node = nodes.Element(rawsource='\n'.join(lines))
-
-        title, messages = self.make_title()
-
-        self.content = ViewList(lines, self.content.source)
-        self.state.nested_parse(self.content, self.content_offset, node)
-        table_node = node[0]
-        if title:
-            table_node.insert(0, title)
-
-        return [table_node] + messages
-
-def setup(app):
-    app.add_directive("xlsx-table", XlsxTable)
-
-    return {
-        'version': '1.0.0',
-        'parallel_read_safe': True,
-        'parallel_write_safe': True,
-    }
+import os
+from docutils import nodes
+from docutils.parsers.rst import directives
+from docutils.statemachine import ViewList
+
+from xlsxtable.xlsx2gridtable import gen_reST_grid_table_lines
+
+class XlsxTable(directives.tables.RSTTable):
+    has_content = True
+
+    optional_arguments = 1
+    option_spec = {
+        'file': directives.path,
+        'header-rows': directives.positive_int,
+        'start-row': directives.positive_int,
+        'start-column': directives.positive_int,
+        'include-rows': directives.unchanged,
+        'exclude-rows': directives.unchanged,
+        'include-columns': directives.unchanged,
+        'exclude-columns': directives.unchanged,
+        'sheet': directives.unchanged,
+    }
+
+    def run(self):
+        file = self.options.get('file', '')
+        header_rows = self.options.get('header-rows', 0)
+        sheet = self.options.get('sheet', None)
+        start_row = self.options.get('start-row', 1)
+        start_column = self.options.get('start-column', 1)
+        include_rows = self.options.get('include-rows', None)
+        exclude_rows = self.options.get('exclude-rows', None)
+        include_columns = self.options.get('include-columns', None)
+        exclude_columns = self.options.get('exclude-columns', None)
+
+        rst_dir = os.path.dirname(os.path.abspath(self.state.document.current_source))
+        fullpath = os.path.normpath(os.path.join(rst_dir, file))
+
+        lines = gen_reST_grid_table_lines(
+            file,
+            fullpath,
+            header_rows,
+            sheet,
+            start_row,
+            start_column,
+            include_rows, exclude_rows,
+            include_columns, exclude_columns)
+        node = nodes.Element(rawsource='\n'.join(lines))
+
+        title, messages = self.make_title()
+
+        self.content = ViewList(lines, self.content.source)
+        self.state.nested_parse(self.content, self.content_offset, node)
+        table_node = node[0]
+        if title:
+            table_node.insert(0, title)
+
+        return [table_node] + messages
+
+def setup(app):
+    app.add_directive("xlsx-table", XlsxTable)
+
+    return {
+        'version': '1.1.0',
+        'parallel_read_safe': True,
+        'parallel_write_safe': True,
+    }
```

### Comparing `sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt` & `sphinxcontrib-xlsxtable-1.1.0/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 setup.cfg
 setup.py
 sphinxcontrib/__init__.py
 sphinxcontrib/xlsxtable/__init__.py
 sphinxcontrib/xlsxtable/__main__.py
 sphinxcontrib/xlsxtable/xlsx2gridtable.py
 sphinxcontrib/xlsxtable/xlsxtable.py
+sphinxcontrib/xlsxtable/workbook/__init__.py
+sphinxcontrib/xlsxtable/workbook/workbook.py
 sphinxcontrib_xlsxtable.egg-info/PKG-INFO
 sphinxcontrib_xlsxtable.egg-info/SOURCES.txt
 sphinxcontrib_xlsxtable.egg-info/dependency_links.txt
 sphinxcontrib_xlsxtable.egg-info/namespace_packages.txt
 sphinxcontrib_xlsxtable.egg-info/not-zip-safe
 sphinxcontrib_xlsxtable.egg-info/requires.txt
 sphinxcontrib_xlsxtable.egg-info/top_level.txt
```

