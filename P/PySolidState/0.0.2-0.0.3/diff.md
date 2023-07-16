# Comparing `tmp/PySolidState-0.0.2.tar.gz` & `tmp/PySolidState-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.0.2.tar", last modified: Sun Jul 16 01:21:02 2023, max compression
+gzip compressed data, was "PySolidState-0.0.3.tar", last modified: Sun Jul 16 01:28:37 2023, max compression
```

## Comparing `PySolidState-0.0.2.tar` & `PySolidState-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:21:02.700678 PySolidState-0.0.2/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:21:02.699676 PySolidState-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 01:21:02.695672 PySolidState-0.0.2/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:21:01.000000 PySolidState-0.0.2/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-07-16 01:21:02.000000 PySolidState-0.0.2/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:21:01.000000 PySolidState-0.0.2/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 01:21:01.000000 PySolidState-0.0.2/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 01:21:01.000000 PySolidState-0.0.2/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 01:21:02.700678 PySolidState-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1172 2023-07-16 01:19:26.000000 PySolidState-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:28:37.224844 PySolidState-0.0.3/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:28:37.223844 PySolidState-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 01:28:37.189844 PySolidState-0.0.3/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.3/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:28:37.220863 PySolidState-0.0.3/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-16 01:28:37.000000 PySolidState-0.0.3/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 01:28:37.224844 PySolidState-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1172 2023-07-16 01:28:19.000000 PySolidState-0.0.3/setup.py
```

### Comparing `PySolidState-0.0.2/PKG-INFO` & `PySolidState-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.2
+Version: 0.0.3
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.2/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.0.3/PySolidState.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.2
+Version: 0.0.3
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.2/setup.py` & `PySolidState-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.0.02",
+    version="0.0.03",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe",
     author_email="makesens19@gmail.com",
     license="GNU General Public License v3.0",
```

