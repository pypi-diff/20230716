# Comparing `tmp/idlerich-0.2.0.tar.gz` & `tmp/idlerich-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idlerich-0.2.0.tar", last modified: Sun Jul 16 21:01:36 2023, max compression
+gzip compressed data, was "idlerich-0.2.1.tar", last modified: Sun Jul 16 21:15:27 2023, max compression
```

## Comparing `idlerich-0.2.0.tar` & `idlerich-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 21:01:36.944076 idlerich-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-07-16 16:33:58.000000 idlerich-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      796 2023-07-16 21:01:36.943076 idlerich-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-07-16 20:59:39.000000 idlerich-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-16 21:01:36.898101 idlerich-0.2.0/idlerich/
--rw-rw-rw-   0        0        0       13 2023-07-16 20:54:31.000000 idlerich-0.2.0/idlerich/__init__.py
--rw-rw-rw-   0        0        0     3364 2023-07-16 20:57:15.000000 idlerich-0.2.0/idlerich/__main__.py
--rw-rw-rw-   0        0        0      151 2023-07-16 21:00:41.000000 idlerich-0.2.0/idlerich/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-16 21:01:36.940080 idlerich-0.2.0/idlerich.egg-info/
--rw-rw-rw-   0        0        0      796 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 21:01:36.945073 idlerich-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-07-16 20:52:35.000000 idlerich-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:15:27.552082 idlerich-0.2.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-16 16:33:58.000000 idlerich-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      822 2023-07-16 21:15:27.552082 idlerich-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-07-16 21:02:38.000000 idlerich-0.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 21:15:27.531095 idlerich-0.2.1/idlerich/
+-rw-rw-rw-   0        0        0       13 2023-07-16 20:54:31.000000 idlerich-0.2.1/idlerich/__init__.py
+-rw-rw-rw-   0        0        0     3364 2023-07-16 20:57:15.000000 idlerich-0.2.1/idlerich/__main__.py
+-rw-rw-rw-   0        0        0      151 2023-07-16 21:14:36.000000 idlerich-0.2.1/idlerich/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:15:27.550083 idlerich-0.2.1/idlerich.egg-info/
+-rw-rw-rw-   0        0        0      822 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 21:15:27.553082 idlerich-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      824 2023-07-16 21:14:16.000000 idlerich-0.2.1/setup.py
```

### Comparing `idlerich-0.2.0/LICENSE` & `idlerich-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idlerich-0.2.0/PKG-INFO` & `idlerich-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlerich
-Version: 0.2.0
+Version: 0.2.1
 Summary: A bootloader that caches and auto-richifies IDLE because I felt lazy.
 Home-page: https://github.com/CuboidRaptor/idlerich
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -17,8 +17,8 @@
 This just literally bootloads IDLE with Rich in it.
 I'm so creative.
 
 WARNING: This package is *extremely* hacky. Do not use it for any sort of stable use.
 -------------------------------------------------------------------------------------
 
 If you still want to, :code:`pip install` and run :code:`python -m idlerich` in console.
-Then, you can just run :code:`idle.pyw` in the idlelib folder.
+Then, you can just run :code:`idle.pyw` in the idlelib folder in idlerich site packages.
```

### Comparing `idlerich-0.2.0/idlerich/__main__.py` & `idlerich-0.2.1/idlerich/__main__.py`

 * *Files identical despite different names*

### Comparing `idlerich-0.2.0/idlerich.egg-info/PKG-INFO` & `idlerich-0.2.1/idlerich.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlerich
-Version: 0.2.0
+Version: 0.2.1
 Summary: A bootloader that caches and auto-richifies IDLE because I felt lazy.
 Home-page: https://github.com/CuboidRaptor/idlerich
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -17,8 +17,8 @@
 This just literally bootloads IDLE with Rich in it.
 I'm so creative.
 
 WARNING: This package is *extremely* hacky. Do not use it for any sort of stable use.
 -------------------------------------------------------------------------------------
 
 If you still want to, :code:`pip install` and run :code:`python -m idlerich` in console.
-Then, you can just run :code:`idle.pyw` in the idlelib folder.
+Then, you can just run :code:`idle.pyw` in the idlelib folder in idlerich site packages.
```

### Comparing `idlerich-0.2.0/setup.py` & `idlerich-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,13 +16,14 @@
     description="A bootloader that caches and auto-richifies IDLE because I felt lazy.",
     url=mdata["__url__"],
     author=mdata["__author__"],
     author_email=mdata["__authoremail__"],
     license="MIT License",
     packages=["idlerich"],
     install_requires=[
-        "rich>=13.0.0a1"
+        "rich>=13.0.0a1",
+        "packaging>=23.0"
     ],
     python_requires=">=3.6",
     long_description=readme,
     long_description_content_type="text/x-rst"
 )
```

