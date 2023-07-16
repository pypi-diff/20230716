# Comparing `tmp/pyracer-1.0.1.tar.gz` & `tmp/pyracer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracer-1.0.1.tar", last modified: Sun Jul 16 15:52:10 2023, max compression
+gzip compressed data, was "pyracer-1.0.2.tar", last modified: Sun Jul 16 21:10:09 2023, max compression
```

## Comparing `pyracer-1.0.1.tar` & `pyracer-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:52:10.535327 pyracer-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-16 15:52:00.000000 pyracer-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-16 15:52:10.535327 pyracer-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:52:10.531326 pyracer-1.0.1/RACER/
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/RACER.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 15:52:00.000000 pyracer-1.0.1/RACER/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-16 15:52:00.000000 pyracer-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:52:10.531326 pyracer-1.0.1/pyracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 15:52:10.000000 pyracer-1.0.1/pyracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:52:10.535327 pyracer-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-16 15:52:00.000000 pyracer-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:10:09.352467 pyracer-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-16 21:09:59.000000 pyracer-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-16 21:10:09.352467 pyracer-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:10:09.352467 pyracer-1.0.2/RACER/
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-07-16 21:09:59.000000 pyracer-1.0.2/RACER/RACER.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 21:09:59.000000 pyracer-1.0.2/RACER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-16 21:09:59.000000 pyracer-1.0.2/RACER/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 21:09:59.000000 pyracer-1.0.2/RACER/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-16 21:09:59.000000 pyracer-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:10:09.352467 pyracer-1.0.2/pyracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-16 21:10:09.000000 pyracer-1.0.2/pyracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 21:10:09.000000 pyracer-1.0.2/pyracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:10:09.000000 pyracer-1.0.2/pyracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 21:10:09.000000 pyracer-1.0.2/pyracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 21:10:09.000000 pyracer-1.0.2/pyracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 21:10:09.352467 pyracer-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-16 21:09:59.000000 pyracer-1.0.2/setup.py
```

### Comparing `pyracer-1.0.1/LICENSE` & `pyracer-1.0.2/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Adversarian
+Copyright (c) 2023 Arian Tashakkor, Mohammad Safaiyan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyracer-1.0.1/PKG-INFO` & `pyracer-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.0.1/RACER/RACER.py` & `pyracer-1.0.2/RACER/RACER.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,17 +363,17 @@
         self._extants_if = new_extants_if
 
     def _finalize_rules(self) -> None:
         """Removes redundant rules to form the final ruleset"""
         temp_rules_if = self._final_rules_if
         temp_rules_then = self._final_rules_then
         temp_rules_fitnesses = self._fitnesses
-        for i in range(len(temp_rules_if) - 1):
+        for i in range(len(temp_rules_if) - 2):
             mask = np.ones(len(temp_rules_if), dtype=bool)
-            covered = self._covered(temp_rules_if[i], temp_rules_if[i + 1 :])
+            covered = self._covered(temp_rules_if[i + 1 :], temp_rules_if[i])
             mask[i+1:][covered] = False
             temp_rules_if, temp_rules_then, temp_rules_fitnesses = (
                 temp_rules_if[mask], temp_rules_then[mask], temp_rules_fitnesses[mask]
             )
 
         self._final_rules_if, self._final_rules_then, self._fitnesses = (
             temp_rules_if,
```

### Comparing `pyracer-1.0.1/RACER/preprocessing.py` & `pyracer-1.0.2/RACER/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyracer-1.0.1/pyracer.egg-info/PKG-INFO` & `pyracer-1.0.2/pyracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.0.1/setup.py` & `pyracer-1.0.2/setup.py`

 * *Files identical despite different names*

