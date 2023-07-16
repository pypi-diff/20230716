# Comparing `tmp/texbuild-0.1.1.tar.gz` & `tmp/texbuild-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texbuild-0.1.1.tar", last modified: Fri Jul 29 23:54:39 2022, max compression
+gzip compressed data, was "texbuild-0.1.2.tar", last modified: Sun Jul 16 18:16:45 2023, max compression
```

## Comparing `texbuild-0.1.1.tar` & `texbuild-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:54:39.795052 texbuild-0.1.1/
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     1075 2022-07-29 23:37:42.000000 texbuild-0.1.1/LICENSE
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     3244 2022-07-29 23:54:39.795052 texbuild-0.1.1/PKG-INFO
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     1464 2022-07-29 23:50:12.000000 texbuild-0.1.1/README.md
--rw-r--r--   0 danielsank (268076) primarygroup (89939)      732 2022-07-29 23:50:46.000000 texbuild-0.1.1/pyproject.toml
--rw-r--r--   0 danielsank (268076) primarygroup (89939)       38 2022-07-29 23:54:39.795052 texbuild-0.1.1/setup.cfg
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:54:39.795052 texbuild-0.1.1/src/
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:54:39.795052 texbuild-0.1.1/src/texbuild/
--rw-r--r--   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:37:42.000000 texbuild-0.1.1/src/texbuild/__init__.py
--rwxr-xr-x   0 danielsank (268076) primarygroup (89939)     8756 2022-07-29 23:37:42.000000 texbuild-0.1.1/src/texbuild/build.py
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:54:39.795052 texbuild-0.1.1/src/texbuild.egg-info/
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     3244 2022-07-29 23:54:39.000000 texbuild-0.1.1/src/texbuild.egg-info/PKG-INFO
--rw-r--r--   0 danielsank (268076) primarygroup (89939)      307 2022-07-29 23:54:39.000000 texbuild-0.1.1/src/texbuild.egg-info/SOURCES.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)        1 2022-07-29 23:54:39.000000 texbuild-0.1.1/src/texbuild.egg-info/dependency_links.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)       49 2022-07-29 23:54:39.000000 texbuild-0.1.1/src/texbuild.egg-info/entry_points.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)       12 2022-07-29 23:54:39.000000 texbuild-0.1.1/src/texbuild.egg-info/requires.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)        9 2022-07-29 23:54:39.000000 texbuild-0.1.1/src/texbuild.egg-info/top_level.txt
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-16 18:16:45.514166 texbuild-0.1.2/
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     1075 2022-07-29 23:37:42.000000 texbuild-0.1.2/LICENSE
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     3244 2023-07-16 18:16:45.514166 texbuild-0.1.2/PKG-INFO
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     1464 2022-07-29 23:50:12.000000 texbuild-0.1.2/README.md
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)      732 2023-07-16 18:10:32.000000 texbuild-0.1.2/pyproject.toml
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)       38 2023-07-16 18:16:45.514166 texbuild-0.1.2/setup.cfg
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-16 18:16:45.514166 texbuild-0.1.2/src/
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-16 18:16:45.514166 texbuild-0.1.2/src/texbuild/
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:37:42.000000 texbuild-0.1.2/src/texbuild/__init__.py
+-rwxr-xr-x   0 danielsank (268076) primarygroup (89939)     8863 2023-07-16 18:08:36.000000 texbuild-0.1.2/src/texbuild/build.py
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-16 18:16:45.514166 texbuild-0.1.2/src/texbuild.egg-info/
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     3244 2023-07-16 18:16:45.000000 texbuild-0.1.2/src/texbuild.egg-info/PKG-INFO
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)      307 2023-07-16 18:16:45.000000 texbuild-0.1.2/src/texbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)        1 2023-07-16 18:16:45.000000 texbuild-0.1.2/src/texbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)       49 2023-07-16 18:16:45.000000 texbuild-0.1.2/src/texbuild.egg-info/entry_points.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)       12 2023-07-16 18:16:45.000000 texbuild-0.1.2/src/texbuild.egg-info/requires.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)        9 2023-07-16 18:16:45.000000 texbuild-0.1.2/src/texbuild.egg-info/top_level.txt
```

### Comparing `texbuild-0.1.1/LICENSE` & `texbuild-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `texbuild-0.1.1/PKG-INFO` & `texbuild-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texbuild
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build system for LaTeX documents.
 Author-email: Daniel Sank <sank.daniel@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Daniel Thomas Sank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `texbuild-0.1.1/README.md` & `texbuild-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `texbuild-0.1.1/pyproject.toml` & `texbuild-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "texbuild"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Daniel Sank", email="sank.daniel@gmail.com" },
 ]
 description = "Build system for LaTeX documents."
 keywords = ["latex"]
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `texbuild-0.1.1/src/texbuild/build.py` & `texbuild-0.1.2/src/texbuild/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import pathlib
 import re
 import shutil
 
 import attrs
 
 
-RE_IMPORTS = re.compile(r'% -- begin imports --\n(.*)% -- end imports --\n', flags=re.DOTALL)
+RE_IMPORTS = re.compile(r'% -- begin imports --\n(.*)% -- end imports --\n', flags=re.DOTALL | re.MULTILINE)
 RE_SINGLE_IMPORT = re.compile(r'% import (.+) as (\w+)')
 RE_EXPORT = re.compile(r'\\label{(.+)} +% export')
-RE_REF = re.compile(r'\\ref{(\w+\.)?(\w+)}{1}')
+RE_REF = re.compile(r'\\ref\{(\w+\.)?([a-zA-Z0-9_:]+)\}', flags=re.MULTILINE)
 RE_PDF = re.compile(r'(?:\\includegraphics|\\quickfig).*{(\w+\.pdf)}')
-RE_TEX_SUBIMPORTLEVEL = re.compile(r'\\subimportlevel{(.+)}{(.+)}{(.+)}')
-RE_TEX_INPUT = re.compile(r'\\input{(.+)}')
+RE_TEX_SUBIMPORTLEVEL = re.compile(r'^\\subimportlevel{(.+)}{(.+)}{(.+)}', flags=re.MULTILINE)
+RE_TEX_INPUT = re.compile(r'^\\input{(.+)}', flags=re.MULTILINE)
 
 
 @contextlib.contextmanager
 def set_directory(path: pathlib.Path):
     origin = pathlib.Path()
     try:
         os.chdir(path)
@@ -42,15 +42,15 @@
     """Find all TeX files included in a single file.
 
     Args:
         file: Path to the file in which we look for other TeX file includes.
 
     Returns a set of paths to included files.
     """
-    with open(file, 'r') as readfile:
+    with open(file.resolve(), 'r') as readfile:
         text = readfile.read()
     paths: Set[pathlib.Path] = set()
 
     result = RE_TEX_SUBIMPORTLEVEL.findall(text)
     for directory, filename, _ in result:
         paths.add(file.parent / directory / filename)
 
@@ -155,15 +155,15 @@
 
     Args:
         file: Path to the TeX file.
         prefix: Prefix to prepend to exported objects.
 
     Returns a Module representing this file.
     """
-    with open(file, 'r') as infile:
+    with open(file.resolve(), 'r') as infile:
         text = infile.read()
     exports = frozenset(Export(label=l) for l in RE_EXPORT.findall(text))
     pdfs = frozenset(RE_PDF.findall(text))
     
     def replace(matcher) -> str:
         if matcher is None:
             raise ValueError
```

### Comparing `texbuild-0.1.1/src/texbuild.egg-info/PKG-INFO` & `texbuild-0.1.2/src/texbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texbuild
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build system for LaTeX documents.
 Author-email: Daniel Sank <sank.daniel@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Daniel Thomas Sank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

