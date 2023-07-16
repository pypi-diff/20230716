# Comparing `tmp/PySolidState-0.0.4.tar.gz` & `tmp/PySolidState-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.0.4.tar", last modified: Sun Jul 16 01:34:28 2023, max compression
+gzip compressed data, was "PySolidState-0.0.5.tar", last modified: Sun Jul 16 01:40:45 2023, max compression
```

## Comparing `PySolidState-0.0.4.tar` & `PySolidState-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.362966 PySolidState-0.0.4/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:34:28.361967 PySolidState-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.319967 PySolidState-0.0.4/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.4/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.358969 PySolidState-0.0.4/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.4/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.4/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.4/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.4/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    16586 2023-07-16 00:26:58.000000 PySolidState-0.0.4/PySolidState/crystal_structure/lattice.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:34:28.345968 PySolidState-0.0.4/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-07-16 01:34:28.000000 PySolidState-0.0.4/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 01:34:27.000000 PySolidState-0.0.4/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 01:34:28.363969 PySolidState-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-07-16 01:34:20.000000 PySolidState-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:40:45.803956 PySolidState-0.0.5/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:40:45.802955 PySolidState-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 01:40:45.751961 PySolidState-0.0.5/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.5/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:40:45.800959 PySolidState-0.0.5/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.5/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.5/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.5/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.5/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    16586 2023-07-16 00:26:58.000000 PySolidState-0.0.5/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-08 17:20:16.000000 PySolidState-0.0.5/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-16 01:40:45.782959 PySolidState-0.0.5/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-16 01:40:45.000000 PySolidState-0.0.5/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-07-16 01:40:45.000000 PySolidState-0.0.5/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:40:45.000000 PySolidState-0.0.5/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 01:40:45.000000 PySolidState-0.0.5/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 01:40:45.000000 PySolidState-0.0.5/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 01:40:45.803956 PySolidState-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2023-07-16 01:40:35.000000 PySolidState-0.0.5/setup.py
```

### Comparing `PySolidState-0.0.4/PKG-INFO` & `PySolidState-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.4
+Version: 0.0.5
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.4/PySolidState/crystal_structure/atom.py` & `PySolidState-0.0.5/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.4/PySolidState/crystal_structure/base.py` & `PySolidState-0.0.5/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.4/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.0.5/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.4/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.0.5/PySolidState/crystal_structure/lattice.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.4/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.0.5/PySolidState.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.4
+Version: 0.0.5
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.4/setup.py` & `PySolidState-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.0.04",
+    version="0.0.05",
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
+    package_data={
+        'PySolidState': ['crystal_structure/lattices.json']
+    },
     include_package_data=True,
     install_requires=["numpy", "matplotlib","mayavi"]
 )
```

