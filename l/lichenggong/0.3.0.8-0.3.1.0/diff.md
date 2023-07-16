# Comparing `tmp/lichenggong-0.3.0.8.tar.gz` & `tmp/lichenggong-0.3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.3.0.8.tar", last modified: Sun Jul 16 10:49:00 2023, max compression
+gzip compressed data, was "lichenggong-0.3.1.0.tar", last modified: Sun Jul 16 12:51:25 2023, max compression
```

## Comparing `lichenggong-0.3.0.8.tar` & `lichenggong-0.3.1.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.507216 lichenggong-0.3.0.8/
--rw-rw-rw-   0        0        0      619 2023-07-16 10:49:00.506216 lichenggong-0.3.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.458215 lichenggong-0.3.0.8/lichenggong/
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.479211 lichenggong-0.3.0.8/lichenggong/Noodows/
--rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.8/lichenggong/Noodows/__bios__.py
--rw-rw-rw-   0        0        0     8609 2023-07-16 10:48:26.000000 lichenggong-0.3.0.8/lichenggong/Noodows/__noodows__.py
--rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.8/lichenggong/Noodows/first.txt
--rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.8/lichenggong/Noodows/practice.py
--rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.8/lichenggong/Noodows/update.log
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.484211 lichenggong-0.3.0.8/lichenggong/Noodows/version/
--rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.8/lichenggong/Noodows/version/build_version.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 10:48:54.000000 lichenggong-0.3.0.8/lichenggong/Noodows/version/version.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.452210 lichenggong-0.3.0.8/lichenggong/Program_Files/
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.501212 lichenggong-0.3.0.8/lichenggong/Program_Files/System/
--rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__calc__.py
--rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__logo__.py
--rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__n_time__.py
--rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__start_menu__.py
--rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__thanks__.py
--rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/System/__user__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.503213 lichenggong-0.3.0.8/lichenggong/Program_Files/User/
--rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.8/lichenggong/Program_Files/User/_.py
--rw-rw-rw-   0        0        0      144 2023-07-16 10:48:26.000000 lichenggong-0.3.0.8/lichenggong/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:49:00.467215 lichenggong-0.3.0.8/lichenggong.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 10:49:00.000000 lichenggong-0.3.0.8/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:49:00.508214 lichenggong-0.3.0.8/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-16 10:40:05.000000 lichenggong-0.3.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/
+-rw-rw-rw-   0        0        0      619 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.409278 lichenggong-0.3.1.0/lichenggong/
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.425223 lichenggong-0.3.1.0/lichenggong/Noodows/
+-rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.1.0/lichenggong/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0      130 2023-07-16 10:50:48.000000 lichenggong-0.3.1.0/lichenggong/Noodows/__init__.py
+-rw-rw-rw-   0        0        0     8595 2023-07-16 11:51:15.000000 lichenggong-0.3.1.0/lichenggong/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.1.0/lichenggong/Noodows/first.txt
+-rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.1.0/lichenggong/Noodows/practice.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 12:12:38.000000 lichenggong-0.3.1.0/lichenggong/Noodows/python.txt
+-rw-rw-rw-   0        0        0     2270 2023-07-16 12:50:31.000000 lichenggong-0.3.1.0/lichenggong/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.440852 lichenggong-0.3.1.0/lichenggong/Noodows/version/
+-rw-rw-rw-   0        0        0        9 2023-07-16 12:50:10.000000 lichenggong-0.3.1.0/lichenggong/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 12:49:08.000000 lichenggong-0.3.1.0/lichenggong/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.393657 lichenggong-0.3.1.0/lichenggong/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/lichenggong/Program_Files/System/
+-rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__n_time__.py
+-rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__start_menu__.py
+-rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    15973 2023-07-16 11:51:15.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__user__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/lichenggong/Program_Files/User/
+-rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/User/_.py
+-rw-rw-rw-   0        0        0      870 2023-07-16 12:47:21.000000 lichenggong-0.3.1.0/lichenggong/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.409278 lichenggong-0.3.1.0/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-07-16 10:40:05.000000 lichenggong-0.3.1.0/setup.py
```

### Comparing `lichenggong-0.3.0.8/PKG-INFO` & `lichenggong-0.3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.8
+Version: 0.3.1.0
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.8/lichenggong/Noodows/__bios__.py` & `lichenggong-0.3.1.0/lichenggong/Noodows/__bios__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.8/lichenggong/Noodows/__noodows__.py` & `lichenggong-0.3.1.0/lichenggong/Noodows/__noodows__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,33 @@
 import __bios__
 import __calc__
 import __logo__
 import __user__
 import __thanks__
 import __n_time__
 
-# 自建包
-
-sys.path.append('../Program_Files/User')
 
+# 自建包
 
 # import some modules
 
 # 优雅
 
 def __n_start__():
     def __first_choose__():
-        with open('first.txt', 'r') as Fir:
-                firs = Fir.readline()
-        if firs == 'True':
-            __user__.First(0)
-            firs = 'False'
-            with open('first.txt', "w", encoding="utf-8") as Fir:
-                Fir.write(firs)
-            del firs
+        with open('first.txt', 'r') as First:
+            first = First.readline()
+        if first == 'True':
+            __user__.__u_first__(0)
+            first = 'False'
+            with open('first.txt', "w", encoding="utf-8") as First:
+                First.write(first)
+            del first
             gc.collect()
+
     def __language__(model, us_en, zn_cn, zn_tw):
         if users_language == 'US_en':
             if model == 'print':
                 print(us_en)
             elif model == 'input':
                 print(us_en, end='')
                 variable = input("")
@@ -188,7 +187,8 @@
                 print("Good bye!")
             elif choose == '2':
                 __thanks__.thanks()
         elif choose == '99':
             exit(0)
         else:
             print('error: input an undefined thing')
+__n_start__()
```

### Comparing `lichenggong-0.3.0.8/lichenggong/Noodows/update.log` & `lichenggong-0.3.1.0/lichenggong/Noodows/update.log`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 >>at version 0.2.3.4
 '''
 
 streamline content update
 
 delete the Cutscenes at the time of the change password
 
-because it is too long(my dear......)
+because it is too long
 
 practicability update
 
 fix calc is error
 
 file control update
 
@@ -141,14 +141,14 @@
 >>at version 0.2.4.0 build_version 10.7.1.19920
 '''
 version change
 
 there is the latest 0.2 version
 
 '''
->>at version 0.3.0.5 build_version 23.1.17.84800
+>>at version 0.3.1.0 build_version 33.17.81919
 '''
 big change
 
 I can't wait fighting with my computer and dividing it into two piece
 
 '''
```

### Comparing `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__calc__.py` & `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__calc__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__logo__.py` & `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__logo__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__n_time__.py` & `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__n_time__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.0.8/lichenggong/Program_Files/System/__user__.py` & `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__user__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 祖宗之法不可变 切记
 
 import gc
 import os
 import shutil
 
 
-def first(__first):
+def __u_first__(__first):
     with open('../Noodows//version//version.txt', 'r') as Version_version:
         version = Version_version.readline()  # read the version
     with open('../Noodows//version//build_version.txt', 'r') as Build_version:
         build_version = Build_version.readline()  # read the version
     print()
     print('您正在使用巨硬产品 noodows yee{0}(测试{1}) 无图像版 (用户创建区)'.format(version, build_version))
     print("You're use noodows yee{0}(build{1}) no Image by Big-hard (setup user)".format(version, build_version))
```

### Comparing `lichenggong-0.3.0.8/lichenggong.egg-info/PKG-INFO` & `lichenggong-0.3.1.0/lichenggong.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.3.0.8
+Version: 0.3.1.0
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.3.0.8/lichenggong.egg-info/SOURCES.txt` & `lichenggong-0.3.1.0/lichenggong.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 setup.py
 lichenggong/__init__.py
 lichenggong.egg-info/PKG-INFO
 lichenggong.egg-info/SOURCES.txt
 lichenggong.egg-info/dependency_links.txt
 lichenggong.egg-info/top_level.txt
 lichenggong/Noodows/__bios__.py
+lichenggong/Noodows/__init__.py
 lichenggong/Noodows/__noodows__.py
 lichenggong/Noodows/first.txt
 lichenggong/Noodows/practice.py
+lichenggong/Noodows/python.txt
 lichenggong/Noodows/update.log
 lichenggong/Noodows/version/build_version.txt
 lichenggong/Noodows/version/version.txt
 lichenggong/Program_Files/System/__calc__.py
 lichenggong/Program_Files/System/__logo__.py
 lichenggong/Program_Files/System/__n_time__.py
 lichenggong/Program_Files/System/__start_menu__.py
```

### Comparing `lichenggong-0.3.0.8/setup.py` & `lichenggong-0.3.1.0/setup.py`

 * *Files identical despite different names*

