# Comparing `tmp/pyfrobot-0.1.4.tar.gz` & `tmp/pyfrobot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfrobot-0.1.4.tar", last modified: Sun Jul 16 09:17:57 2023, max compression
+gzip compressed data, was "pyfrobot-0.1.5.tar", last modified: Sun Jul 16 09:20:51 2023, max compression
```

## Comparing `pyfrobot-0.1.4.tar` & `pyfrobot-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:17:57.125940 pyfrobot-0.1.4/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:17:57.125325 pyfrobot-0.1.4/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)       20 2023-07-16 09:03:31.000000 pyfrobot-0.1.4/README.md
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:17:57.124616 pyfrobot-0.1.4/pyfrobot.egg-info/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:17:56.000000 pyfrobot-0.1.4/pyfrobot.egg-info/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)      177 2023-07-16 09:17:56.000000 pyfrobot-0.1.4/pyfrobot.egg-info/SOURCES.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:17:56.000000 pyfrobot-0.1.4/pyfrobot.egg-info/dependency_links.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       25 2023-07-16 09:17:56.000000 pyfrobot-0.1.4/pyfrobot.egg-info/requires.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:17:56.000000 pyfrobot-0.1.4/pyfrobot.egg-info/top_level.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-07-16 09:17:57.126096 pyfrobot-0.1.4/setup.cfg
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2145 2023-07-16 09:11:32.000000 pyfrobot-0.1.4/setup.py
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:20:51.832916 pyfrobot-0.1.5/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:20:51.832414 pyfrobot-0.1.5/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       20 2023-07-16 09:03:31.000000 pyfrobot-0.1.5/README.md
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:20:51.831812 pyfrobot-0.1.5/pyfrobot.egg-info/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:20:51.000000 pyfrobot-0.1.5/pyfrobot.egg-info/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      177 2023-07-16 09:20:51.000000 pyfrobot-0.1.5/pyfrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:20:51.000000 pyfrobot-0.1.5/pyfrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       25 2023-07-16 09:20:51.000000 pyfrobot-0.1.5/pyfrobot.egg-info/requires.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:20:51.000000 pyfrobot-0.1.5/pyfrobot.egg-info/top_level.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-07-16 09:20:51.833065 pyfrobot-0.1.5/setup.cfg
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2145 2023-07-16 09:11:32.000000 pyfrobot-0.1.5/setup.py
```

### Comparing `pyfrobot-0.1.4/PKG-INFO` & `pyfrobot-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Descripción de mi librería
 Home-page: https://github.com/tu_usuario/mi_libreria
 Author: alpeza
 Author-email: alvaroperi.06@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrobot-0.1.4/pyfrobot.egg-info/PKG-INFO` & `pyfrobot-0.1.5/pyfrobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Descripción de mi librería
 Home-page: https://github.com/tu_usuario/mi_libreria
 Author: alpeza
 Author-email: alvaroperi.06@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrobot-0.1.4/setup.py` & `pyfrobot-0.1.5/setup.py`

 * *Files identical despite different names*

