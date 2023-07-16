# Comparing `tmp/mylatextable-0.0.1.tar.gz` & `tmp/mylatextable-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mylatextable-0.0.1.tar", last modified: Fri Jun  9 13:48:48 2023, max compression
+gzip compressed data, was "mylatextable-0.0.2.tar", last modified: Sun Jul 16 19:46:16 2023, max compression
```

## Comparing `mylatextable-0.0.1.tar` & `mylatextable-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-09 13:48:48.033031 mylatextable-0.0.1/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1060 2023-05-20 16:37:14.000000 mylatextable-0.0.1/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)     2357 2023-06-09 13:48:48.033031 mylatextable-0.0.1/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      456 2023-05-20 18:09:38.000000 mylatextable-0.0.1/README.md
--rw-rw-r--   0 peter     (1000) peter     (1000)      909 2023-05-20 16:34:32.000000 mylatextable-0.0.1/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-09 13:48:48.033031 mylatextable-0.0.1/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-09 13:48:48.029031 mylatextable-0.0.1/src/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-09 13:48:48.033031 mylatextable-0.0.1/src/mylatextable/
--rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-05-20 19:09:36.000000 mylatextable-0.0.1/src/mylatextable/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1559 2023-05-20 18:59:27.000000 mylatextable-0.0.1/src/mylatextable/my_latex_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2099 2023-05-20 19:16:21.000000 mylatextable-0.0.1/src/mylatextable/my_long_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2152 2023-05-20 21:06:07.000000 mylatextable-0.0.1/src/mylatextable/my_table.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-09 13:48:48.033031 mylatextable-0.0.1/src/mylatextable.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2357 2023-06-09 13:48:48.000000 mylatextable-0.0.1/src/mylatextable.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      319 2023-06-09 13:48:48.000000 mylatextable-0.0.1/src/mylatextable.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-09 13:48:48.000000 mylatextable-0.0.1/src/mylatextable.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       13 2023-06-09 13:48:48.000000 mylatextable-0.0.1/src/mylatextable.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-16 19:46:16.644183 mylatextable-0.0.2/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1060 2023-05-20 16:37:14.000000 mylatextable-0.0.2/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2603 2023-07-16 19:46:16.644183 mylatextable-0.0.2/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      701 2023-06-09 13:52:41.000000 mylatextable-0.0.2/README.md
+-rw-rw-r--   0 peter     (1000) peter     (1000)      909 2023-07-16 19:46:07.000000 mylatextable-0.0.2/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-16 19:46:16.644183 mylatextable-0.0.2/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-16 19:46:16.640183 mylatextable-0.0.2/src/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-16 19:46:16.644183 mylatextable-0.0.2/src/mylatextable/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-05-20 19:09:36.000000 mylatextable-0.0.2/src/mylatextable/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1717 2023-07-16 19:43:37.000000 mylatextable-0.0.2/src/mylatextable/my_latex_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2099 2023-05-20 19:16:21.000000 mylatextable-0.0.2/src/mylatextable/my_long_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2152 2023-07-16 19:45:01.000000 mylatextable-0.0.2/src/mylatextable/my_table.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-16 19:46:16.644183 mylatextable-0.0.2/src/mylatextable.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2603 2023-07-16 19:46:16.000000 mylatextable-0.0.2/src/mylatextable.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      319 2023-07-16 19:46:16.000000 mylatextable-0.0.2/src/mylatextable.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-16 19:46:16.000000 mylatextable-0.0.2/src/mylatextable.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       13 2023-07-16 19:46:16.000000 mylatextable-0.0.2/src/mylatextable.egg-info/top_level.txt
```

### Comparing `mylatextable-0.0.1/LICENSE` & `mylatextable-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mylatextable-0.0.1/PKG-INFO` & `mylatextable-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mylatextable
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quickly generate LaTeX tables
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: Copyright (c) 2023 Peter N. Robinson
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -45,7 +45,19 @@
 header = [...] # Define header fields
 table = MyLatexTable(header_fields=header, use_booktabs=True)
 rows = .... # create a list of rows according to your logic
 for row in rows:
     table.add_row(row)
 print(table.get_latex()) # display LaTeX code
 ```
+
+
+
+### Release
+To release a new version, update the version number in pyproject.toml and enter the following commands.
+
+```
+python -m build .
+python -m twine upload dist/*
+```
+
+This package is available at https://pypi.org/project/mylatextable/.
```

### Comparing `mylatextable-0.0.1/pyproject.toml` & `mylatextable-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 ["src"]
 
 
 [project]
 name = "mylatextable"
-version = "0.0.1"
+version = "0.0.2"
 requires-python = ">=3.5"
 description = "Quickly generate LaTeX tables"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `mylatextable-0.0.1/src/mylatextable/my_latex_table.py` & `mylatextable-0.0.2/src/mylatextable/my_latex_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,28 @@
         self._hlines = self._header()
         self._flines = self._footer()
         
         
     def _header(self) -> None:
         hlines = []
         hlines.append("\\begin{table}")
+        hlines.append("\\centering")
         hlines.append("\\begin{tabular}" + "{" + self._header_field_formats + "}")
         if self._use_booktabs:
             hlines.append("\\toprule")
         else:
             hlines.append("\\hline")
         header = []
         for h in self._header_fields:
             header.append("\\textbf{" + h +"}")
         hlines.append(" & ".join(header) + "\\\\")
+        if self._use_booktabs:
+            hlines.append("\\midrule")
+        else:
+            hlines.append("\\hline")
         return hlines
     
     def _footer(self) -> None:
         flines = []
         if self._use_booktabs:
             flines.append("\\bottomrule")
         else:
```

### Comparing `mylatextable-0.0.1/src/mylatextable/my_long_table.py` & `mylatextable-0.0.2/src/mylatextable/my_long_table.py`

 * *Files identical despite different names*

### Comparing `mylatextable-0.0.1/src/mylatextable/my_table.py` & `mylatextable-0.0.2/src/mylatextable/my_table.py`

 * *Files identical despite different names*

### Comparing `mylatextable-0.0.1/src/mylatextable.egg-info/PKG-INFO` & `mylatextable-0.0.2/src/mylatextable.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mylatextable
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quickly generate LaTeX tables
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: Copyright (c) 2023 Peter N. Robinson
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -45,7 +45,19 @@
 header = [...] # Define header fields
 table = MyLatexTable(header_fields=header, use_booktabs=True)
 rows = .... # create a list of rows according to your logic
 for row in rows:
     table.add_row(row)
 print(table.get_latex()) # display LaTeX code
 ```
+
+
+
+### Release
+To release a new version, update the version number in pyproject.toml and enter the following commands.
+
+```
+python -m build .
+python -m twine upload dist/*
+```
+
+This package is available at https://pypi.org/project/mylatextable/.
```

