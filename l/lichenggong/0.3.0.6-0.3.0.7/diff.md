# Comparing `tmp/lichenggong-0.3.0.6.tar.gz` & `tmp/lichenggong-0.3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.3.0.6.tar", last modified: Sun Jul 16 10:33:52 2023, max compression
+gzip compressed data, was "lichenggong-0.3.0.7.tar", last modified: Sun Jul 16 10:40:31 2023, max compression
```

## Comparing `lichenggong-0.3.0.6.tar` & `lichenggong-0.3.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.527445 lichenggong-0.3.0.6/
--rw-rw-rw-   0        0        0      619 2023-07-16 10:33:52.524445 lichenggong-0.3.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.464442 lichenggong-0.3.0.6/lichenggong.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      624 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:33:52.528451 lichenggong-0.3.0.6/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-07-16 09:34:08.000000 lichenggong-0.3.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.466440 lichenggong-0.3.0.6/ver/
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.485445 lichenggong-0.3.0.6/ver/Noodows/
--rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.6/ver/Noodows/__bios__.py
--rw-rw-rw-   0        0        0     8603 2023-07-16 07:28:02.000000 lichenggong-0.3.0.6/ver/Noodows/__noodows__.py
--rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.6/ver/Noodows/first.txt
--rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.6/ver/Noodows/practice.py
--rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.6/ver/Noodows/update.log
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.492444 lichenggong-0.3.0.6/ver/Noodows/version/
--rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.6/ver/Noodows/version/build_version.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 10:32:43.000000 lichenggong-0.3.0.6/ver/Noodows/version/version.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.442446 lichenggong-0.3.0.6/ver/Program_Files/
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.516445 lichenggong-0.3.0.6/ver/Program_Files/System/
--rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__calc__.py
--rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__logo__.py
--rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__n_time__.py
--rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__start_menu__.py
--rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__thanks__.py
--rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__user__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.521445 lichenggong-0.3.0.6/ver/Program_Files/User/
--rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.6/ver/Program_Files/User/_.py
--rw-rw-rw-   0        0        0        0 2023-07-16 10:28:43.000000 lichenggong-0.3.0.6/ver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.186350 lichenggong-0.3.0.7/
+-rw-rw-rw-   0        0        0      619 2023-07-16 10:40:31.170727 lichenggong-0.3.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.123852 lichenggong-0.3.0.7/lichenggong/
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.155100 lichenggong-0.3.0.7/lichenggong/Noodows/
+-rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.7/lichenggong/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0     8603 2023-07-16 07:28:02.000000 lichenggong-0.3.0.7/lichenggong/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.7/lichenggong/Noodows/first.txt
+-rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.7/lichenggong/Noodows/practice.py
+-rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.7/lichenggong/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.155100 lichenggong-0.3.0.7/lichenggong/Noodows/version/
+-rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.7/lichenggong/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 10:40:26.000000 lichenggong-0.3.0.7/lichenggong/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.123852 lichenggong-0.3.0.7/lichenggong/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.170727 lichenggong-0.3.0.7/lichenggong/Program_Files/System/
+-rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__n_time__.py
+-rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__start_menu__.py
+-rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__user__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.170727 lichenggong-0.3.0.7/lichenggong/Program_Files/User/
+-rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/User/_.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 10:28:43.000000 lichenggong-0.3.0.7/lichenggong/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.139472 lichenggong-0.3.0.7/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-07-16 10:40:30.000000 lichenggong-0.3.0.7/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2023-07-16 10:40:31.000000 lichenggong-0.3.0.7/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:40:30.000000 lichenggong-0.3.0.7/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 10:40:30.000000 lichenggong-0.3.0.7/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:40:31.186350 lichenggong-0.3.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-07-16 10:40:05.000000 lichenggong-0.3.0.7/setup.py
```

### Comparing `lichenggong-0.3.0.6/PKG-INFO` & `lichenggong-0.3.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.6
+Version: 0.3.0.7
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.6/lichenggong.egg-info/PKG-INFO` & `lichenggong-0.3.0.7/lichenggong.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.6
+Version: 0.3.0.7
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.6/setup.py` & `lichenggong-0.3.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # coding=utf-8
 from setuptools import setup
-with open(".\\ver\\Noodows\\version\\version.txt", 'r') as f1:
+with open(".\\lichenggong\\Noodows\\version\\version.txt", 'r') as f1:
     version = f1.readline()
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 setup(
-    packages=['ver','ver.Noodows','ver.Noodows.version','ver.Program_Files.System','ver.Program_Files.User'],
+    packages=['lichenggong',
+              'lichenggong.Noodows',
+              'lichenggong.Noodows.version',
+              'lichenggong.Program_Files.System',
+              'lichenggong.Program_Files.User'],
     name="lichenggong",
     version=version,
     description="python 3   windows 10 (best)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='',
     package_data={'':['*.py','*.txt','*.log']},
```

### Comparing `lichenggong-0.3.0.6/ver/Noodows/__bios__.py` & `lichenggong-0.3.0.7/lichenggong/Noodows/__bios__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.6/ver/Noodows/__noodows__.py` & `lichenggong-0.3.0.7/lichenggong/Noodows/__noodows__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.6/ver/Noodows/update.log` & `lichenggong-0.3.0.7/lichenggong/Noodows/update.log`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.6/ver/Program_Files/System/__calc__.py` & `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__calc__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.6/ver/Program_Files/System/__logo__.py` & `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__logo__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.6/ver/Program_Files/System/__n_time__.py` & `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__n_time__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.6/ver/Program_Files/System/__user__.py` & `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__user__.py`

 * *Files identical despite different names*

