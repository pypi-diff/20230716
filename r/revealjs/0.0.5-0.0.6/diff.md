# Comparing `tmp/revealjs-0.0.5.tar.gz` & `tmp/revealjs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revealjs-0.0.5.tar", last modified: Sun Jul 16 04:56:02 2023, max compression
+gzip compressed data, was "revealjs-0.0.6.tar", last modified: Sun Jul 16 05:10:35 2023, max compression
```

## Comparing `revealjs-0.0.5.tar` & `revealjs-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:56:02.690019 revealjs-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 04:56:02.690019 revealjs-0.0.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:56:02.690019 revealjs-0.0.5/revealjs/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      136 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/interface.py
--rw-rw-r--   0 root         (0) root         (0)    17532 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/reveal_js.py
--rw-rw-r--   0 root         (0) root         (0)     4504 2023-07-16 04:40:54.000000 revealjs-0.0.5/revealjs/slide.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 04:56:02.690019 revealjs-0.0.5/revealjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 04:56:02.000000 revealjs-0.0.5/revealjs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 04:56:02.690019 revealjs-0.0.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      553 2023-07-16 04:53:24.000000 revealjs-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:10:35.054742 revealjs-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 05:10:35.054742 revealjs-0.0.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:10:35.054742 revealjs-0.0.6/revealjs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-16 04:40:54.000000 revealjs-0.0.6/revealjs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      136 2023-07-16 04:40:54.000000 revealjs-0.0.6/revealjs/interface.py
+-rw-rw-r--   0 root         (0) root         (0)    17532 2023-07-16 04:40:54.000000 revealjs-0.0.6/revealjs/reveal_js.py
+-rw-rw-r--   0 root         (0) root         (0)     4504 2023-07-16 04:40:54.000000 revealjs-0.0.6/revealjs/slide.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:10:35.054742 revealjs-0.0.6/revealjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 05:10:35.000000 revealjs-0.0.6/revealjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-16 05:10:35.000000 revealjs-0.0.6/revealjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 05:10:35.000000 revealjs-0.0.6/revealjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 05:10:35.000000 revealjs-0.0.6/revealjs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-16 05:10:35.000000 revealjs-0.0.6/revealjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 05:10:35.000000 revealjs-0.0.6/revealjs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 05:10:35.054742 revealjs-0.0.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      562 2023-07-16 05:03:01.000000 revealjs-0.0.6/setup.py
```

### Comparing `revealjs-0.0.5/PKG-INFO` & `revealjs-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Reveal.js Presentation Builder Inspired By revealjs
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

### Comparing `revealjs-0.0.5/README.md` & `revealjs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.5/revealjs/reveal_js.py` & `revealjs-0.0.6/revealjs/reveal_js.py`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.5/revealjs/slide.adoc` & `revealjs-0.0.6/revealjs/slide.adoc`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.5/revealjs.egg-info/PKG-INFO` & `revealjs-0.0.6/revealjs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Reveal.js Presentation Builder Inspired By revealjs
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

### Comparing `revealjs-0.0.5/setup.py` & `revealjs-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     long_description = fd.read()
 
 setup(
     **data,
     long_description=long_description,
     packages=["revealjs"],
     py_modules=["revealjs.reveal_js", "revealjs.interface"],
-    package_data={"revealjs": ["slide.adoc"]},
+    data_files=[("revealjs", ["revealjs/slide.adoc"])],
     entry_points={
         "console_scripts": ["reveal_js = revealjs.reveal_js:main"],
     },
     install_requires=[i.strip() for i in open("requirements.txt").readlines()],
 )
```

