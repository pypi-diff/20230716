# Comparing `tmp/bitmap2-0.2.3.tar.gz` & `tmp/bitmap2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmap2-0.2.3.tar", last modified: Wed Jun 21 17:33:37 2023, max compression
+gzip compressed data, was "bitmap2-0.2.4.tar", last modified: Sat Jul 15 22:05:30 2023, max compression
```

## Comparing `bitmap2-0.2.3.tar` & `bitmap2-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.443524 bitmap2-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 17:33:32.000000 bitmap2-0.2.3/.github/workflows/pypi-upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-21 17:33:32.000000 bitmap2-0.2.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-21 17:33:32.000000 bitmap2-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 17:33:32.000000 bitmap2-0.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 17:33:32.000000 bitmap2-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-21 17:33:37.443524 bitmap2-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-21 17:33:32.000000 bitmap2-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/bitmap2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:33:37.443524 bitmap2-0.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-06-21 17:33:32.000000 bitmap2-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 17:33:32.000000 bitmap2-0.2.3/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6595 2023-06-21 17:33:32.000000 bitmap2-0.2.3/src/bitmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-06-21 17:33:32.000000 bitmap2-0.2.3/test/test_bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.027397 bitmap2-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.027397 bitmap2-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-15 22:05:20.000000 bitmap2-0.2.4/.github/workflows/pypi-upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-15 22:05:20.000000 bitmap2-0.2.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-15 22:05:20.000000 bitmap2-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-15 22:05:20.000000 bitmap2-0.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 22:05:20.000000 bitmap2-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-15 22:05:30.031397 bitmap2-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-15 22:05:20.000000 bitmap2-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/bitmap2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-15 22:05:29.000000 bitmap2-0.2.4/bitmap2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 22:05:30.000000 bitmap2-0.2.4/bitmap2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:05:29.000000 bitmap2-0.2.4/bitmap2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 22:05:29.000000 bitmap2-0.2.4/bitmap2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:05:30.031397 bitmap2-0.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-07-15 22:05:20.000000 bitmap2-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 22:05:20.000000 bitmap2-0.2.4/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6619 2023-07-15 22:05:20.000000 bitmap2-0.2.4/src/bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-07-15 22:05:20.000000 bitmap2-0.2.4/test/test_bitmap.py
```

### Comparing `bitmap2-0.2.3/.github/workflows/pypi-upload.yml` & `bitmap2-0.2.4/.github/workflows/pypi-upload.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.3/.github/workflows/test.yml` & `bitmap2-0.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.3/.gitignore` & `bitmap2-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.3/LICENSE.md` & `bitmap2-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.3/PKG-INFO` & `bitmap2-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.3
+Version: 0.2.4
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.3/README.md` & `bitmap2-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.3/bitmap2.egg-info/PKG-INFO` & `bitmap2-0.2.4/bitmap2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.3
+Version: 0.2.4
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.3/setup.py` & `bitmap2-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.3/src/bitmap.py` & `bitmap2-0.2.4/src/bitmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
       E-mail: wanji@live.com
   Created on: Thu May  1 15:26:18 2014 CST
 
   Description: BitMap Class
 """
 
 import array
+import itertools
 try:
     from past.builtins import range
 except ImportError:
     pass
 
 class BitMap(object):
     """
@@ -30,15 +31,15 @@
         """
         self.bits = maxnum
         nbytes = (maxnum + 7) // 8
         bit_value = 0xFF if preset else 0x00
         if bitmap:
             self.bitmap = bytearray(bitmap)
         else:
-            self.bitmap = array.array('B', [bit_value for i in range(nbytes)])
+            self.bitmap = array.array('B', itertools.repeat(bit_value, times=nbytes))
 
     def __del__(self):
         """
         Destroy the BitMap
         """
         pass
```

### Comparing `bitmap2-0.2.3/test/test_bitmap.py` & `bitmap2-0.2.4/test/test_bitmap.py`

 * *Files identical despite different names*

