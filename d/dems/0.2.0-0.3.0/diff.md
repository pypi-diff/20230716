# Comparing `tmp/dems-0.2.0.tar.gz` & `tmp/dems-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dems-0.2.0.tar", max compression
+gzip compressed data, was "dems-0.3.0.tar", max compression
```

## Comparing `dems-0.2.0.tar` & `dems-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-18 12:33:28.758332 dems-0.2.0/LICENSE
--rw-r--r--   0        0        0       31 2023-04-18 12:33:28.758332 dems-0.2.0/README.md
--rw-r--r--   0        0        0       94 2023-04-18 12:33:28.758332 dems-0.2.0/dems/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-18 12:33:28.758332 dems-0.2.0/dems/d1.py
--rw-r--r--   0        0        0     6975 2023-04-18 12:33:28.758332 dems-0.2.0/dems/d2.py
--rw-r--r--   0        0        0        0 2023-04-18 12:33:28.758332 dems-0.2.0/dems/py.typed
--rw-r--r--   0        0        0      509 2023-04-18 12:33:28.758332 dems-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 dems-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-16 10:46:07.957393 dems-0.3.0/LICENSE
+-rw-r--r--   0        0        0      664 2023-07-16 10:46:07.957393 dems-0.3.0/README.md
+-rw-r--r--   0        0        0       94 2023-07-16 10:46:07.957393 dems-0.3.0/dems/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-16 10:46:07.957393 dems-0.3.0/dems/d1.py
+-rw-r--r--   0        0        0     6975 2023-07-16 10:46:07.957393 dems-0.3.0/dems/d2.py
+-rw-r--r--   0        0        0        0 2023-07-16 10:46:07.957393 dems-0.3.0/dems/py.typed
+-rw-r--r--   0        0        0      499 2023-07-16 10:46:07.957393 dems-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 dems-0.3.0/PKG-INFO
```

### Comparing `dems-0.2.0/LICENSE` & `dems-0.3.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 DESHIMA
+Copyright (c) 2022-2023 Akio Taniguchi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dems-0.2.0/dems/d1.py` & `dems-0.3.0/dems/d1.py`

 * *Files identical despite different names*

### Comparing `dems-0.2.0/dems/d2.py` & `dems-0.3.0/dems/d2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # constants
 ASTE_ITRS_COORDS = (
     +2230817.2140945992,
     -5440188.022176585,
     -2475718.801708271,
 )
-DEMS_VERSION = "v0.2.0"
+DEMS_VERSION = "v0.3.0"
 DMERGE_VERSION = "v1.0.0"
 
 
 @dataclass
 class Data_:
     data: Data[Tuple[Ti, Ch], Any]
     long_name: Attr[str] = "Data values"
```

