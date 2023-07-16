# Comparing `tmp/pyfrobot-0.1.0.tar.gz` & `tmp/pyfrobot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfrobot-0.1.0.tar", last modified: Sun Jul 16 08:42:06 2023, max compression
+gzip compressed data, was "pyfrobot-0.1.1.tar", last modified: Sun Jul 16 09:11:37 2023, max compression
```

## Comparing `pyfrobot-0.1.0.tar` & `pyfrobot-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 08:42:06.411941 pyfrobot-0.1.0/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      591 2023-07-16 08:42:06.411123 pyfrobot-0.1.0/PKG-INFO
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 08:42:06.410375 pyfrobot-0.1.0/pyfrobot.egg-info/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      591 2023-07-16 08:42:05.000000 pyfrobot-0.1.0/pyfrobot.egg-info/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)      136 2023-07-16 08:42:06.000000 pyfrobot-0.1.0/pyfrobot.egg-info/SOURCES.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 08:42:05.000000 pyfrobot-0.1.0/pyfrobot.egg-info/dependency_links.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 08:42:05.000000 pyfrobot-0.1.0/pyfrobot.egg-info/top_level.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-07-16 08:42:06.412050 pyfrobot-0.1.0/setup.cfg
--rw-r--r--   0 alvaroperis   (501) staff       (20)      765 2023-07-16 08:41:38.000000 pyfrobot-0.1.0/setup.py
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:11:37.365913 pyfrobot-0.1.1/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:11:37.365377 pyfrobot-0.1.1/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       20 2023-07-16 09:03:31.000000 pyfrobot-0.1.1/README.md
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-07-16 09:11:37.364579 pyfrobot-0.1.1/pyfrobot.egg-info/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      557 2023-07-16 09:11:36.000000 pyfrobot-0.1.1/pyfrobot.egg-info/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      177 2023-07-16 09:11:37.000000 pyfrobot-0.1.1/pyfrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:11:36.000000 pyfrobot-0.1.1/pyfrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       25 2023-07-16 09:11:36.000000 pyfrobot-0.1.1/pyfrobot.egg-info/requires.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-07-16 09:11:36.000000 pyfrobot-0.1.1/pyfrobot.egg-info/top_level.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-07-16 09:11:37.366084 pyfrobot-0.1.1/setup.cfg
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2145 2023-07-16 09:11:32.000000 pyfrobot-0.1.1/setup.py
```

### Comparing `pyfrobot-0.1.0/PKG-INFO` & `pyfrobot-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfrobot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Descripción de mi librería
 Home-page: https://github.com/tu_usuario/mi_libreria
 Author: alpeza
 Author-email: alvaroperi.06@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-Texto largo con información detallada de la librería
+# Py Framework Robot
```

### Comparing `pyfrobot-0.1.0/pyfrobot.egg-info/PKG-INFO` & `pyfrobot-0.1.1/pyfrobot.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfrobot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Descripción de mi librería
 Home-page: https://github.com/tu_usuario/mi_libreria
 Author: alpeza
 Author-email: alvaroperi.06@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-Texto largo con información detallada de la librería
+# Py Framework Robot
```

