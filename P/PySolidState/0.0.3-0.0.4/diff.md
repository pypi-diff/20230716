# Comparing `tmp/PySolidState-0.0.3.tar.gz` & `tmp/PySolidState-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.0.3.tar", last modified: Sun Jul 16 01:28:37 2023, max compression
+gzip compressed data, was "PySolidState-0.0.4.tar", last modified: Sun Jul 16 01:34:28 2023, max compression
```

## Comparing `PySolidState-0.0.3.tar` & `PySolidState-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:28:37.224844 PySolidState-0.0.3/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:28:37.223844 PySolidState-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 01:28:37.189844 PySolidState-0.0.3/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.3/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:28:37.220863 PySolidState-0.0.3/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-07-16 01:28:37.000000 PySolidState-0.0.3/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 01:28:36.000000 PySolidState-0.0.3/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 01:28:37.224844 PySolidState-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1172 2023-07-16 01:28:19.000000 PySolidState-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.362966 PySolidState-0.0.4/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:34:28.361967 PySolidState-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.319967 PySolidState-0.0.4/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.4/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.358969 PySolidState-0.0.4/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.4/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.4/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.4/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.4/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    16586 2023-07-16 00:26:58.000000 PySolidState-0.0.4/PySolidState/crystal_structure/lattice.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.345968 PySolidState-0.0.4/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-07-16 01:34:28.000000 PySolidState-0.0.4/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 01:34:28.363969 PySolidState-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2023-07-16 01:34:20.000000 PySolidState-0.0.4/setup.py
```

### Comparing `PySolidState-0.0.3/PKG-INFO` & `PySolidState-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.3
+Version: 0.0.4
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.3/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.0.4/PySolidState.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.3
+Version: 0.0.4
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.3/setup.py` & `PySolidState-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.0.03",
+    version="0.0.04",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe",
     author_email="makesens19@gmail.com",
     license="GNU General Public License v3.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
-    packages=["PySolidState"],
+    packages=["PySolidState", "PySolidState.crystal_structure"],
     include_package_data=True,
     install_requires=["numpy", "matplotlib","mayavi"]
 )
```

