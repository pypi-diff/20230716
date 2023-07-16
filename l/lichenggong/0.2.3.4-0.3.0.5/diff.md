# Comparing `tmp/lichenggong-0.2.3.4.tar.gz` & `tmp/lichenggong-0.3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.2.3.4.tar", last modified: Fri Sep 23 13:49:30 2022, max compression
+gzip compressed data, was "lichenggong-0.3.0.5.tar", last modified: Sun Jul 16 09:34:52 2023, max compression
```

## Comparing `lichenggong-0.2.3.4.tar` & `lichenggong-0.3.0.5.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.233404 lichenggong-0.2.3.4/
--rw-rw-rw-   0        0        0     1091 2022-09-02 00:32:24.000000 lichenggong-0.2.3.4/LICENSE
--rw-rw-rw-   0        0        0     1242 2022-09-23 13:49:30.200403 lichenggong-0.2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      833 2022-09-23 13:49:21.000000 lichenggong-0.2.3.4/README.md
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.168404 lichenggong-0.2.3.4/lichenggong/
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.198407 lichenggong-0.2.3.4/lichenggong/System/
--rw-rw-rw-   0        0        0        6 2022-09-18 09:10:01.000000 lichenggong-0.2.3.4/lichenggong/System/Password_for_Boss.txt
--rw-rw-rw-   0        0        0        1 2022-09-18 02:20:17.000000 lichenggong-0.2.3.4/lichenggong/System/lauguage.txt
--rw-rw-rw-   0        0        0        0 2022-09-10 11:16:06.000000 lichenggong-0.2.3.4/lichenggong/System/pi.txt
--rw-rw-rw-   0        0        0        5 2022-09-18 01:49:37.000000 lichenggong-0.2.3.4/lichenggong/System/upgrade.txt
--rw-rw-rw-   0        0        0        7 2022-09-23 13:43:34.000000 lichenggong-0.2.3.4/lichenggong/System/version.txt
--rw-rw-rw-   0        0        0     3473 2022-09-14 11:15:35.000000 lichenggong-0.2.3.4/lichenggong/System/windows蓝瓶钙圣经.txt
--rw-rw-rw-   0        0        0      198 2022-09-13 00:48:06.000000 lichenggong-0.2.3.4/lichenggong/__init__.py
--rw-rw-rw-   0        0        0    65334 2022-09-23 13:45:58.000000 lichenggong-0.2.3.4/lichenggong/__lidao__.py
--rw-rw-rw-   0        0        0       33 2022-09-23 13:22:16.000000 lichenggong-0.2.3.4/lichenggong/__test__.py
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.179405 lichenggong-0.2.3.4/lichenggong.egg-info/
--rw-rw-rw-   0        0        0     1242 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-23 13:49:30.234404 lichenggong-0.2.3.4/setup.cfg
--rw-rw-rw-   0        0        0      858 2022-09-23 13:46:42.000000 lichenggong-0.2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/
+-rw-rw-rw-   0        0        0      619 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.404236 lichenggong-0.3.0.5/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-16 09:34:52.000000 lichenggong-0.3.0.5/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      795 2023-07-16 09:34:08.000000 lichenggong-0.3.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.388613 lichenggong-0.3.0.5/ver/
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.404236 lichenggong-0.3.0.5/ver/Noodows/
+-rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.0.5/ver/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0     8603 2023-07-16 07:28:02.000000 lichenggong-0.3.0.5/ver/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.0.5/ver/Noodows/first.txt
+-rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.0.5/ver/Noodows/practice.py
+-rw-rw-rw-   0        0        0     2287 2023-07-16 07:40:01.000000 lichenggong-0.3.0.5/ver/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.435485 lichenggong-0.3.0.5/ver/Noodows/version/
+-rw-rw-rw-   0        0        0       13 2023-01-17 00:54:54.000000 lichenggong-0.3.0.5/ver/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 09:34:47.000000 lichenggong-0.3.0.5/ver/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.388613 lichenggong-0.3.0.5/ver/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/ver/Program_Files/System/
+-rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__n_time__.py
+-rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__start_menu__.py
+-rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    15967 2023-07-16 07:36:38.000000 lichenggong-0.3.0.5/ver/Program_Files/System/__user__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:34:52.451110 lichenggong-0.3.0.5/ver/Program_Files/User/
+-rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.0.5/ver/Program_Files/User/_.py
```

### Comparing `lichenggong-0.2.3.4/setup.py` & `lichenggong-0.3.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-import setuptools
-with open('.\lichenggong\\System\\version.txt','r') as f1:
-    version=f1.readline()
-with open("README.md","r",encoding="utf-8") as f:
-    long_description=f.read()
-setuptools.setup(
+# coding=utf-8
+from setuptools import setup
+with open(".\\ver\\Noodows\\version\\version.txt", 'r') as f1:
+    version = f1.readline()
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+setup(
+    packages=['ver','ver.Noodows','ver.Noodows.version','ver.Program_Files.System','ver.Program_Files.User'],
     name="lichenggong",
     version=version,
-    author="2368916680",
-    author_email="2368916680@qq.com",
-    description="编程语言：python 3 操作系统：windows",
+    description="python 3   windows 10 (best)",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url=None,
-    include_package_data=True,
-    package_data={
-        'lichenggong':[
-            'System/*.*']
-        },
-    packages=setuptools.find_packages(),
+    url='',
+    package_data={'':['*.py','*.txt','*.log']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        ],
-    python_requires=">=3"
-)
+    ],
+    python_requires=">=3")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

