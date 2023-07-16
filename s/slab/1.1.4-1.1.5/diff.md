# Comparing `tmp/slab-1.1.4.tar.gz` & `tmp/slab-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slab-1.1.4.tar", last modified: Sun Jul 16 11:42:46 2023, max compression
+gzip compressed data, was "slab-1.1.5.tar", last modified: Sun Jul 16 17:44:53 2023, max compression
```

## Comparing `slab-1.1.4.tar` & `slab-1.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-16 11:42:36.000000 slab-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-16 11:42:36.000000 slab-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-07-16 11:42:46.724534 slab-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-16 11:42:36.000000 slab-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:42:46.724534 slab-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-16 11:42:36.000000 slab-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-16 11:42:36.000000 slab-1.1.4/slab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28795 2023-07-16 11:42:36.000000 slab-1.1.4/slab/binaural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab/data/
--rw-r--r--   0 runner    (1001) docker     (123)   670746 2023-07-16 11:42:36.000000 slab-1.1.4/slab/data/mit_kemar_normal_pinna.bz2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:36.000000 slab-1.1.4/slab/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-16 11:42:36.000000 slab-1.1.4/slab/experiments/motion_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-16 11:42:36.000000 slab-1.1.4/slab/experiments/room_voice_interference.py
--rw-r--r--   0 runner    (1001) docker     (123)    29833 2023-07-16 11:42:36.000000 slab-1.1.4/slab/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51148 2023-07-16 11:42:36.000000 slab-1.1.4/slab/hrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)    58405 2023-07-16 11:42:36.000000 slab-1.1.4/slab/psychoacoustics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-07-16 11:42:36.000000 slab-1.1.4/slab/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)    72821 2023-07-16 11:42:36.000000 slab-1.1.4/slab/sound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:44:53.391598 slab-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-16 17:44:40.000000 slab-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-16 17:44:40.000000 slab-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-07-16 17:44:53.391598 slab-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-16 17:44:40.000000 slab-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:44:53.391598 slab-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-16 17:44:40.000000 slab-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:44:53.387598 slab-1.1.5/slab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-16 17:44:40.000000 slab-1.1.5/slab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28795 2023-07-16 17:44:40.000000 slab-1.1.5/slab/binaural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:44:53.387598 slab-1.1.5/slab/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   670746 2023-07-16 17:44:40.000000 slab-1.1.5/slab/data/mit_kemar_normal_pinna.bz2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:44:53.387598 slab-1.1.5/slab/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:44:40.000000 slab-1.1.5/slab/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-16 17:44:40.000000 slab-1.1.5/slab/experiments/motion_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-16 17:44:40.000000 slab-1.1.5/slab/experiments/room_voice_interference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29833 2023-07-16 17:44:40.000000 slab-1.1.5/slab/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51148 2023-07-16 17:44:40.000000 slab-1.1.5/slab/hrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58405 2023-07-16 17:44:40.000000 slab-1.1.5/slab/psychoacoustics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-07-16 17:44:40.000000 slab-1.1.5/slab/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72821 2023-07-16 17:44:40.000000 slab-1.1.5/slab/sound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:44:53.387598 slab-1.1.5/slab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-07-16 17:44:53.000000 slab-1.1.5/slab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-16 17:44:53.000000 slab-1.1.5/slab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:44:53.000000 slab-1.1.5/slab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:44:53.000000 slab-1.1.5/slab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 17:44:53.000000 slab-1.1.5/slab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 17:44:53.000000 slab-1.1.5/slab.egg-info/top_level.txt
```

### Comparing `slab-1.1.4/LICENSE` & `slab-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/PKG-INFO` & `slab-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slab
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tools for generating and manipulating digital signals, particularly sounds.
 Home-page: http://github.com/DrMarc/slab.git
 Author: Marc Schoenwiesner
 Author-email: marc.schoenwiesner@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `slab-1.1.4/README.md` & `slab-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/setup.py` & `slab-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/__init__.py` & `slab-1.1.5/slab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import os
 import pathlib
 
-__version__ = '1.1.4'
+__version__ = '1.1.5'
 
 # The variable _in_notebook is used to enable audio playing in Jupiter notebooks
 # and on Google colab (see slab.sound.play())
 try:
     shell = get_ipython().__class__.__module__
     if 'terminal' in shell:
         _in_notebook = False
```

### Comparing `slab-1.1.4/slab/binaural.py` & `slab-1.1.5/slab/binaural.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/data/mit_kemar_normal_pinna.bz2` & `slab-1.1.5/slab/data/mit_kemar_normal_pinna.bz2`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/experiments/motion_speed.py` & `slab-1.1.5/slab/experiments/motion_speed.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/experiments/room_voice_interference.py` & `slab-1.1.5/slab/experiments/room_voice_interference.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/filter.py` & `slab-1.1.5/slab/filter.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/hrtf.py` & `slab-1.1.5/slab/hrtf.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/psychoacoustics.py` & `slab-1.1.5/slab/psychoacoustics.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/signal.py` & `slab-1.1.5/slab/signal.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab/sound.py` & `slab-1.1.5/slab/sound.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.4/slab.egg-info/PKG-INFO` & `slab-1.1.5/slab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slab
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tools for generating and manipulating digital signals, particularly sounds.
 Home-page: http://github.com/DrMarc/slab.git
 Author: Marc Schoenwiesner
 Author-email: marc.schoenwiesner@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

