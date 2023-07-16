# Comparing `tmp/lichenggong-0.3.0.7.tar.gz` & `tmp/lichenggong-0.3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.3.0.7.tar", last modified: Sun Jul 16 10:40:31 2023, max compression
+gzip compressed data, was "lichenggong-0.3.0.8.tar", last modified: Sun Jul 16 10:49:00 2023, max compression
```

## Comparing `lichenggong-0.3.0.7.tar` & `lichenggong-0.3.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.186350 lichenggong-0.3.0.7/
--rw-rw-rw-   0        0        0      619 2023-07-16 10:40:31.170727 lichenggong-0.3.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.123852 lichenggong-0.3.0.7/lichenggong/
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.155100 lichenggong-0.3.0.7/lichenggong/Noodows/
--rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.7/lichenggong/Noodows/__bios__.py
--rw-rw-rw-   0        0        0     8603 2023-07-16 07:28:02.000000 lichenggong-0.3.0.7/lichenggong/Noodows/__noodows__.py
--rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.7/lichenggong/Noodows/first.txt
--rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.7/lichenggong/Noodows/practice.py
--rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.7/lichenggong/Noodows/update.log
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.155100 lichenggong-0.3.0.7/lichenggong/Noodows/version/
--rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.7/lichenggong/Noodows/version/build_version.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 10:40:26.000000 lichenggong-0.3.0.7/lichenggong/Noodows/version/version.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.123852 lichenggong-0.3.0.7/lichenggong/Program_Files/
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.170727 lichenggong-0.3.0.7/lichenggong/Program_Files/System/
--rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__calc__.py
--rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__logo__.py
--rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__n_time__.py
--rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__start_menu__.py
--rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__thanks__.py
--rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/System/__user__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.170727 lichenggong-0.3.0.7/lichenggong/Program_Files/User/
--rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.7/lichenggong/Program_Files/User/_.py
--rw-rw-rw-   0        0        0        0 2023-07-16 10:28:43.000000 lichenggong-0.3.0.7/lichenggong/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:40:31.139472 lichenggong-0.3.0.7/lichenggong.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-16 10:40:30.000000 lichenggong-0.3.0.7/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-07-16 10:40:31.000000 lichenggong-0.3.0.7/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:40:30.000000 lichenggong-0.3.0.7/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 10:40:30.000000 lichenggong-0.3.0.7/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:40:31.186350 lichenggong-0.3.0.7/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-16 10:40:05.000000 lichenggong-0.3.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.507216 lichenggong-0.3.0.8/
+-rw-rw-rw-   0        0        0      619 2023-07-16 10:49:00.506216 lichenggong-0.3.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.458215 lichenggong-0.3.0.8/lichenggong/
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.479211 lichenggong-0.3.0.8/lichenggong/Noodows/
+-rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.8/lichenggong/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0     8609 2023-07-16 10:48:26.000000 lichenggong-0.3.0.8/lichenggong/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.8/lichenggong/Noodows/first.txt
+-rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.8/lichenggong/Noodows/practice.py
+-rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.8/lichenggong/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.484211 lichenggong-0.3.0.8/lichenggong/Noodows/version/
+-rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.8/lichenggong/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 10:48:54.000000 lichenggong-0.3.0.8/lichenggong/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.452210 lichenggong-0.3.0.8/lichenggong/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.501212 lichenggong-0.3.0.8/lichenggong/Program_Files/System/
+-rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__n_time__.py
+-rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__start_menu__.py
+-rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__user__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.503213 lichenggong-0.3.0.8/lichenggong/Program_Files/User/
+-rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/User/_.py
+-rw-rw-rw-   0        0        0      144 2023-07-16 10:48:26.000000 lichenggong-0.3.0.8/lichenggong/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.467215 lichenggong-0.3.0.8/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:49:00.508214 lichenggong-0.3.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-07-16 10:40:05.000000 lichenggong-0.3.0.8/setup.py
```

### Comparing `lichenggong-0.3.0.7/PKG-INFO` & `lichenggong-0.3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.7
+Version: 0.3.0.8
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.7/lichenggong/Noodows/__bios__.py` & `lichenggong-0.3.0.8/lichenggong/Noodows/__bios__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.7/lichenggong/Noodows/__noodows__.py` & `lichenggong-0.3.0.8/lichenggong/Noodows/__noodows__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 sys.path.append('../Program_Files/User')
 
 
 # import some modules
 
 # 优雅
 
-def start():
+def __n_start__():
     def __first_choose__():
         with open('first.txt', 'r') as Fir:
                 firs = Fir.readline()
         if firs == 'True':
             __user__.First(0)
             firs = 'False'
             with open('first.txt', "w", encoding="utf-8") as Fir:
```

### Comparing `lichenggong-0.3.0.7/lichenggong/Noodows/update.log` & `lichenggong-0.3.0.8/lichenggong/Noodows/update.log`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__calc__.py` & `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__calc__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__logo__.py` & `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__logo__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__n_time__.py` & `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__n_time__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.7/lichenggong/Program_Files/System/__user__.py` & `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__user__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.7/lichenggong.egg-info/PKG-INFO` & `lichenggong-0.3.0.8/lichenggong.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.7
+Version: 0.3.0.8
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.7/lichenggong.egg-info/SOURCES.txt` & `lichenggong-0.3.0.8/lichenggong.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.7/setup.py` & `lichenggong-0.3.0.8/setup.py`

 * *Files identical despite different names*

