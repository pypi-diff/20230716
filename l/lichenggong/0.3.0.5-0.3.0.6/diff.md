# Comparing `tmp/lichenggong-0.3.0.5.tar.gz` & `tmp/lichenggong-0.3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.3.0.5.tar", last modified: Sun Jul 16 09:34:52 2023, max compression
+gzip compressed data, was "lichenggong-0.3.0.6.tar", last modified: Sun Jul 16 10:33:52 2023, max compression
```

## Comparing `lichenggong-0.3.0.5.tar` & `lichenggong-0.3.0.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/
--rw-rw-rw-   0        0        0      619 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.404236 lichenggong-0.3.0.5/lichenggong.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-07-16 09:34:08.000000 lichenggong-0.3.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.388613 lichenggong-0.3.0.5/ver/
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.404236 lichenggong-0.3.0.5/ver/Noodows/
--rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.5/ver/Noodows/__bios__.py
--rw-rw-rw-   0        0        0     8603 2023-07-16 07:28:02.000000 lichenggong-0.3.0.5/ver/Noodows/__noodows__.py
--rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.5/ver/Noodows/first.txt
--rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.5/ver/Noodows/practice.py
--rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.5/ver/Noodows/update.log
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.435485 lichenggong-0.3.0.5/ver/Noodows/version/
--rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.5/ver/Noodows/version/build_version.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 09:34:47.000000 lichenggong-0.3.0.5/ver/Noodows/version/version.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.388613 lichenggong-0.3.0.5/ver/Program_Files/
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/ver/Program_Files/System/
--rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__calc__.py
--rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__logo__.py
--rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__n_time__.py
--rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__start_menu__.py
--rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__thanks__.py
--rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__user__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/ver/Program_Files/User/
--rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.5/ver/Program_Files/User/_.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.527445 lichenggong-0.3.0.6/
+-rw-rw-rw-   0        0        0      619 2023-07-16 10:33:52.524445 lichenggong-0.3.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.464442 lichenggong-0.3.0.6/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      624 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-16 10:33:52.000000 lichenggong-0.3.0.6/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:33:52.528451 lichenggong-0.3.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      795 2023-07-16 09:34:08.000000 lichenggong-0.3.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.466440 lichenggong-0.3.0.6/ver/
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.485445 lichenggong-0.3.0.6/ver/Noodows/
+-rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.6/ver/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0     8603 2023-07-16 07:28:02.000000 lichenggong-0.3.0.6/ver/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.6/ver/Noodows/first.txt
+-rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.6/ver/Noodows/practice.py
+-rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.6/ver/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.492444 lichenggong-0.3.0.6/ver/Noodows/version/
+-rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.6/ver/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 10:32:43.000000 lichenggong-0.3.0.6/ver/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.442446 lichenggong-0.3.0.6/ver/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.516445 lichenggong-0.3.0.6/ver/Program_Files/System/
+-rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__n_time__.py
+-rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__start_menu__.py
+-rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.6/ver/Program_Files/System/__user__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:33:52.521445 lichenggong-0.3.0.6/ver/Program_Files/User/
+-rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.6/ver/Program_Files/User/_.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 10:28:43.000000 lichenggong-0.3.0.6/ver/__init__.py
```

### Comparing `lichenggong-0.3.0.5/PKG-INFO` & `lichenggong-0.3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.5
+Version: 0.3.0.6
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.5/lichenggong.egg-info/PKG-INFO` & `lichenggong-0.3.0.6/lichenggong.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.5
+Version: 0.3.0.6
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.5/lichenggong.egg-info/SOURCES.txt` & `lichenggong-0.3.0.6/lichenggong.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 lichenggong.egg-info/PKG-INFO
 lichenggong.egg-info/SOURCES.txt
 lichenggong.egg-info/dependency_links.txt
 lichenggong.egg-info/top_level.txt
+ver/__init__.py
 ver/Noodows/__bios__.py
 ver/Noodows/__noodows__.py
 ver/Noodows/first.txt
 ver/Noodows/practice.py
 ver/Noodows/update.log
 ver/Noodows/version/build_version.txt
 ver/Noodows/version/version.txt
```

### Comparing `lichenggong-0.3.0.5/setup.py` & `lichenggong-0.3.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.5/ver/Noodows/__bios__.py` & `lichenggong-0.3.0.6/ver/Noodows/__bios__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.5/ver/Noodows/__noodows__.py` & `lichenggong-0.3.0.6/ver/Noodows/__noodows__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.5/ver/Noodows/update.log` & `lichenggong-0.3.0.6/ver/Noodows/update.log`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.5/ver/Program_Files/System/__calc__.py` & `lichenggong-0.3.0.6/ver/Program_Files/System/__calc__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.5/ver/Program_Files/System/__logo__.py` & `lichenggong-0.3.0.6/ver/Program_Files/System/__logo__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.5/ver/Program_Files/System/__n_time__.py` & `lichenggong-0.3.0.6/ver/Program_Files/System/__n_time__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.5/ver/Program_Files/System/__user__.py` & `lichenggong-0.3.0.6/ver/Program_Files/System/__user__.py`

 * *Files identical despite different names*

