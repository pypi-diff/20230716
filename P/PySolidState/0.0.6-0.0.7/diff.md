# Comparing `tmp/PySolidState-0.0.6.tar.gz` & `tmp/PySolidState-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.0.6.tar", last modified: Sun Jul 16 01:45:27 2023, max compression
+gzip compressed data, was "PySolidState-0.0.7.tar", last modified: Sun Jul 16 01:48:25 2023, max compression
```

## Comparing `PySolidState-0.0.6.tar` & `PySolidState-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:45:27.644100 PySolidState-0.0.6/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:45:27.642100 PySolidState-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 01:45:27.585100 PySolidState-0.0.6/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.6/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:45:27.639098 PySolidState-0.0.6/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.6/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.6/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.6/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.6/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    16610 2023-07-16 01:44:51.000000 PySolidState-0.0.6/PySolidState/crystal_structure/lattice.py
--rw-rw-rw-   0        0        0     3431 2023-07-08 17:20:16.000000 PySolidState-0.0.6/PySolidState/crystal_structure/lattices.json
-drwxrwxrwx   0        0        0        0 2023-07-16 01:45:27.615102 PySolidState-0.0.6/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:45:27.000000 PySolidState-0.0.6/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-07-16 01:45:27.000000 PySolidState-0.0.6/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:45:27.000000 PySolidState-0.0.6/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 01:45:27.000000 PySolidState-0.0.6/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 01:45:27.000000 PySolidState-0.0.6/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 01:45:27.644100 PySolidState-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1294 2023-07-16 01:44:59.000000 PySolidState-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.887492 PySolidState-0.0.7/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:48:25.886490 PySolidState-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.846495 PySolidState-0.0.7/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.883493 PySolidState-0.0.7/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.7/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.7/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    16610 2023-07-16 01:44:51.000000 PySolidState-0.0.7/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.867492 PySolidState-0.0.7/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 01:48:25.888493 PySolidState-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2023-07-16 01:48:20.000000 PySolidState-0.0.7/setup.py
```

### Comparing `PySolidState-0.0.6/PKG-INFO` & `PySolidState-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.6
+Version: 0.0.7
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.6/PySolidState/crystal_structure/atom.py` & `PySolidState-0.0.7/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.6/PySolidState/crystal_structure/base.py` & `PySolidState-0.0.7/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.6/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.0.7/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.6/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.0.7/PySolidState/crystal_structure/lattice.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.6/PySolidState/crystal_structure/lattices.json` & `PySolidState-0.0.7/PySolidState/crystal_structure/lattices.json`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.6/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.0.7/PySolidState.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.6
+Version: 0.0.7
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.6/setup.py` & `PySolidState-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.0.6",
+    version="0.0.7",
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
     packages=["PySolidState", "PySolidState.crystal_structure"],
     package_data={
-        'PySolidState': ['crystal_structure/lattices.json']
+        'PySolidState': ['PySolidState/crystal_structure/lattices.json']
     },
     include_package_data=True,
     install_requires=["numpy", "matplotlib","mayavi"]
 )
```

