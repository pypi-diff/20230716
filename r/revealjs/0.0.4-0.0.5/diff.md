# Comparing `tmp/revealjs-0.0.4.tar.gz` & `tmp/revealjs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revealjs-0.0.4.tar", last modified: Sun Jul 16 04:41:56 2023, max compression
+gzip compressed data, was "revealjs-0.0.5.tar", last modified: Sun Jul 16 04:56:02 2023, max compression
```

## Comparing `revealjs-0.0.4.tar` & `revealjs-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:41:56.128527 revealjs-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 04:41:56.128527 revealjs-0.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:41:56.124527 revealjs-0.0.4/revealjs/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-16 04:40:54.000000 revealjs-0.0.4/revealjs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      136 2023-07-16 04:40:54.000000 revealjs-0.0.4/revealjs/interface.py
--rw-rw-r--   0 root         (0) root         (0)    17532 2023-07-16 04:40:54.000000 revealjs-0.0.4/revealjs/reveal_js.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:41:56.128527 revealjs-0.0.4/revealjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 04:41:56.000000 revealjs-0.0.4/revealjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2023-07-16 04:41:56.000000 revealjs-0.0.4/revealjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 04:41:56.000000 revealjs-0.0.4/revealjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 04:41:56.000000 revealjs-0.0.4/revealjs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-16 04:41:56.000000 revealjs-0.0.4/revealjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 04:41:56.000000 revealjs-0.0.4/revealjs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 04:41:56.128527 revealjs-0.0.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      506 2023-07-16 04:36:12.000000 revealjs-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:56:02.690019 revealjs-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 04:56:02.690019 revealjs-0.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:56:02.690019 revealjs-0.0.5/revealjs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      136 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/interface.py
+-rw-rw-r--   0 root         (0) root         (0)    17532 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/reveal_js.py
+-rw-rw-r--   0 root         (0) root         (0)     4504 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/slide.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:56:02.690019 revealjs-0.0.5/revealjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 04:56:02.690019 revealjs-0.0.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      553 2023-07-16 04:53:24.000000 revealjs-0.0.5/setup.py
```

### Comparing `revealjs-0.0.4/PKG-INFO` & `revealjs-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.4
+Version: 0.0.5
 Summary: Reveal.js Presentation Builder Inspired By revealjs
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

### Comparing `revealjs-0.0.4/README.md` & `revealjs-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.4/revealjs/reveal_js.py` & `revealjs-0.0.5/revealjs/reveal_js.py`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.4/revealjs.egg-info/PKG-INFO` & `revealjs-0.0.5/revealjs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.4
+Version: 0.0.5
 Summary: Reveal.js Presentation Builder Inspired By revealjs
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

