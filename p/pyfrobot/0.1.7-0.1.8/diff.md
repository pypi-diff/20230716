# Comparing `tmp/pyfrobot-0.1.7.tar.gz` & `tmp/pyfrobot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfrobot-0.1.7.tar", last modified: Sun Jul 16 09:44:05 2023, max compression
+gzip compressed data, was "pyfrobot-0.1.8.tar", last modified: Sun Jul 16 09:49:39 2023, max compression
```

## Comparing `pyfrobot-0.1.7.tar` & `pyfrobot-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:44:05.535173 pyfrobot-0.1.7/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:44:05.533945 pyfrobot-0.1.7/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)       20 2023-07-16 09:03:31.000000 pyfrobot-0.1.7/README.md
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:44:05.533004 pyfrobot-0.1.7/pyfrobot.egg-info/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:44:05.000000 pyfrobot-0.1.7/pyfrobot.egg-info/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)      177 2023-07-16 09:44:05.000000 pyfrobot-0.1.7/pyfrobot.egg-info/SOURCES.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:44:05.000000 pyfrobot-0.1.7/pyfrobot.egg-info/dependency_links.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       25 2023-07-16 09:44:05.000000 pyfrobot-0.1.7/pyfrobot.egg-info/requires.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:44:05.000000 pyfrobot-0.1.7/pyfrobot.egg-info/top_level.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-07-16 09:44:05.535659 pyfrobot-0.1.7/setup.cfg
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2145 2023-07-16 09:11:32.000000 pyfrobot-0.1.7/setup.py
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:49:39.535664 pyfrobot-0.1.8/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:49:39.535224 pyfrobot-0.1.8/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       20 2023-07-16 09:03:31.000000 pyfrobot-0.1.8/README.md
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:49:39.534426 pyfrobot-0.1.8/pyfrobot.egg-info/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:49:39.000000 pyfrobot-0.1.8/pyfrobot.egg-info/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      177 2023-07-16 09:49:39.000000 pyfrobot-0.1.8/pyfrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:49:39.000000 pyfrobot-0.1.8/pyfrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       25 2023-07-16 09:49:39.000000 pyfrobot-0.1.8/pyfrobot.egg-info/requires.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:49:39.000000 pyfrobot-0.1.8/pyfrobot.egg-info/top_level.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-07-16 09:49:39.535813 pyfrobot-0.1.8/setup.cfg
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2145 2023-07-16 09:11:32.000000 pyfrobot-0.1.8/setup.py
```

### Comparing `pyfrobot-0.1.7/PKG-INFO` & `pyfrobot-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrobot
-Version: 0.1.7
+Version: 0.1.8
 Summary: Descripción de mi librería
 Home-page: https://github.com/tu_usuario/mi_libreria
 Author: alpeza
 Author-email: alvaroperi.06@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrobot-0.1.7/pyfrobot.egg-info/PKG-INFO` & `pyfrobot-0.1.8/pyfrobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrobot
-Version: 0.1.7
+Version: 0.1.8
 Summary: Descripción de mi librería
 Home-page: https://github.com/tu_usuario/mi_libreria
 Author: alpeza
 Author-email: alvaroperi.06@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrobot-0.1.7/setup.py` & `pyfrobot-0.1.8/setup.py`

 * *Files identical despite different names*

