# Comparing `tmp/ArucoScanner-0.0.1.tar.gz` & `tmp/ArucoScanner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArucoScanner-0.0.1.tar", last modified: Sat Jul 15 22:09:07 2023, max compression
+gzip compressed data, was "ArucoScanner-0.0.2.tar", last modified: Sat Jul 15 22:14:17 2023, max compression
```

## Comparing `ArucoScanner-0.0.1.tar` & `ArucoScanner-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 22:09:07.349112 ArucoScanner-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-15 22:09:07.309438 ArucoScanner-0.0.1/ArucoScanner/
--rw-rw-rw-   0        0        0     1435 2023-07-15 21:39:10.000000 ArucoScanner-0.0.1/ArucoScanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:09:07.342122 ArucoScanner-0.0.1/ArucoScanner.egg-info/
--rw-rw-rw-   0        0        0      698 2023-07-15 22:09:06.000000 ArucoScanner-0.0.1/ArucoScanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-15 22:09:07.000000 ArucoScanner-0.0.1/ArucoScanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 22:09:06.000000 ArucoScanner-0.0.1/ArucoScanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-15 22:09:06.000000 ArucoScanner-0.0.1/ArucoScanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-15 22:09:06.000000 ArucoScanner-0.0.1/ArucoScanner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1078 2023-07-15 21:51:46.000000 ArucoScanner-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0      698 2023-07-15 22:09:07.347118 ArucoScanner-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-15 21:48:51.000000 ArucoScanner-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 22:09:07.349112 ArucoScanner-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-07-15 22:09:00.000000 ArucoScanner-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:14:17.729632 ArucoScanner-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-15 22:14:17.693657 ArucoScanner-0.0.2/ArucoScanner/
+-rw-rw-rw-   0        0        0     1435 2023-07-15 21:39:10.000000 ArucoScanner-0.0.2/ArucoScanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:14:17.724633 ArucoScanner-0.0.2/ArucoScanner.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-07-15 22:14:17.000000 ArucoScanner-0.0.2/ArucoScanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-15 22:14:17.000000 ArucoScanner-0.0.2/ArucoScanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 22:14:17.000000 ArucoScanner-0.0.2/ArucoScanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-15 22:14:17.000000 ArucoScanner-0.0.2/ArucoScanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-15 22:14:17.000000 ArucoScanner-0.0.2/ArucoScanner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1078 2023-07-15 21:51:46.000000 ArucoScanner-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0      616 2023-07-15 22:14:17.726625 ArucoScanner-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-15 21:48:51.000000 ArucoScanner-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 22:14:17.729632 ArucoScanner-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      728 2023-07-15 22:14:12.000000 ArucoScanner-0.0.2/setup.py
```

### Comparing `ArucoScanner-0.0.1/ArucoScanner/__init__.py` & `ArucoScanner-0.0.2/ArucoScanner/__init__.py`

 * *Files identical despite different names*

### Comparing `ArucoScanner-0.0.1/LICENCE.txt` & `ArucoScanner-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ArucoScanner-0.0.1/setup.py` & `ArucoScanner-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,17 +6,17 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ArucoScanner',
-  version='0.0.1',
+  version='0.0.2',
   description='Simplicity for Aruco code',
-  long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
+  long_description=open('README.txt').read(),
   url='https://pypi.org/project/ArduinoScanner/',  
   author='Julien Serbanescu',
   author_email='julien.serbanescu@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='aruco', 
   packages=find_packages(),
```

