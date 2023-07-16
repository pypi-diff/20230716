# Comparing `tmp/zint-1.2.tar.gz` & `tmp/zint-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zint-1.2.tar", last modified: Sat Sep  7 11:35:43 2019, max compression
+gzip compressed data, was "zint-1.4.tar", last modified: Sun Jul 16 16:13:05 2023, max compression
```

## Comparing `zint-1.2.tar` & `zint-1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 aragon     (501) staff       (20)        0 2019-09-07 11:35:43.000000 zint-1.2/
--rw-r--r--   0 aragon     (501) staff       (20)     1484 2017-07-05 21:45:58.000000 zint-1.2/LICENSE.rst
--rw-r--r--   0 aragon     (501) staff       (20)       41 2016-05-18 21:33:38.000000 zint-1.2/MANIFEST.in
--rw-r--r--   0 aragon     (501) staff       (20)      523 2019-09-07 11:35:43.000000 zint-1.2/PKG-INFO
--rw-r--r--   0 aragon     (501) staff       (20)     3289 2019-05-31 15:05:59.000000 zint-1.2/README.rst
--rw-r--r--   0 aragon     (501) staff       (20)       67 2019-09-07 11:35:43.000000 zint-1.2/setup.cfg
--rw-r--r--   0 aragon     (501) staff       (20)      981 2019-05-31 15:06:49.000000 zint-1.2/setup.py
-drwxr-xr-x   0 aragon     (501) staff       (20)        0 2019-09-07 11:35:43.000000 zint-1.2/zint/
--rw-r--r--   0 aragon     (501) staff       (20)       20 2016-05-18 20:17:05.000000 zint-1.2/zint/__init__.py
--rw-r--r--   0 aragon     (501) staff       (20)    12728 2019-06-09 14:43:51.000000 zint-1.2/zint/zint.py
-drwxr-xr-x   0 aragon     (501) staff       (20)        0 2019-09-07 11:35:43.000000 zint-1.2/zint.egg-info/
--rw-r--r--   0 aragon     (501) staff       (20)      523 2019-09-07 11:35:43.000000 zint-1.2/zint.egg-info/PKG-INFO
--rw-r--r--   0 aragon     (501) staff       (20)      222 2019-09-07 11:35:43.000000 zint-1.2/zint.egg-info/SOURCES.txt
--rw-r--r--   0 aragon     (501) staff       (20)        1 2019-09-07 11:35:43.000000 zint-1.2/zint.egg-info/dependency_links.txt
--rw-r--r--   0 aragon     (501) staff       (20)        1 2016-05-18 19:57:38.000000 zint-1.2/zint.egg-info/not-zip-safe
--rw-r--r--   0 aragon     (501) staff       (20)        5 2019-09-07 11:35:43.000000 zint-1.2/zint.egg-info/top_level.txt
+drwxr-xr-x   0 aragon    (1000) wheel      (998)        0 2023-07-16 16:13:05.138566 zint-1.4/
+-rw-r--r--   0 aragon    (1000) wheel      (998)     1489 2023-07-16 16:04:37.000000 zint-1.4/LICENSE.rst
+-rw-r--r--   0 aragon    (1000) wheel      (998)       41 2023-05-30 14:10:26.000000 zint-1.4/MANIFEST.in
+-rw-r--r--   0 aragon    (1000) wheel      (998)      471 2023-07-16 16:13:05.138566 zint-1.4/PKG-INFO
+-rw-r--r--   0 aragon    (1000) wheel      (998)     3292 2023-07-16 14:59:57.000000 zint-1.4/README.rst
+-rw-r--r--   0 aragon    (1000) wheel      (998)      132 2023-07-16 16:13:05.138566 zint-1.4/setup.cfg
+-rw-r--r--   0 aragon    (1000) wheel      (998)      941 2023-07-16 14:59:57.000000 zint-1.4/setup.py
+drwxr-xr-x   0 aragon    (1000) wheel      (998)        0 2023-07-16 16:13:05.138566 zint-1.4/zint/
+-rw-r--r--   0 aragon    (1000) wheel      (998)       20 2023-07-11 18:24:30.000000 zint-1.4/zint/__init__.py
+-rw-r--r--   0 aragon    (1000) wheel      (998)       20 2023-07-16 14:59:57.000000 zint-1.4/zint/_version.py
+-rw-r--r--   0 aragon    (1000) wheel      (998)    23876 2023-07-16 14:59:57.000000 zint-1.4/zint/zint.py
+drwxr-xr-x   0 aragon    (1000) wheel      (998)        0 2023-07-16 16:13:05.138566 zint-1.4/zint.egg-info/
+-rw-r--r--   0 aragon    (1000) wheel      (998)      471 2023-07-16 16:13:05.000000 zint-1.4/zint.egg-info/PKG-INFO
+-rw-r--r--   0 aragon    (1000) wheel      (998)      239 2023-07-16 16:13:05.000000 zint-1.4/zint.egg-info/SOURCES.txt
+-rw-r--r--   0 aragon    (1000) wheel      (998)        1 2023-07-16 16:13:05.000000 zint-1.4/zint.egg-info/dependency_links.txt
+-rw-r--r--   0 aragon    (1000) wheel      (998)        1 2023-07-16 16:13:05.000000 zint-1.4/zint.egg-info/not-zip-safe
+-rw-r--r--   0 aragon    (1000) wheel      (998)        5 2023-07-16 16:13:05.000000 zint-1.4/zint.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zint-1.2/LICENSE.rst` & `zint-1.4/LICENSE.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017, Aragon Gouveia
+Copyright (c) 2019-2023, Aragon Gouveia
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `zint-1.2/README.rst` & `zint-1.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 Generate a QRCode in memory only::
 
     import zint
     import sys
     
     symbol = zint.ZBarcode_Create()
     symbol.contents.symbology = zint.BARCODE_QRCODE
-    symbol.contents.scale = 0
+    symbol.contents.scale = 0.01
     symbol.contents.option_1 = 4
     symbol.contents.border_width = 0
     input = zint.instr(b'https://github.com/jmptbl/python-zint')
     if zint.ZBarcode_Encode_and_Buffer(symbol, input, 0, 0) != 0:
         print('error: %s' % symbol.contents.errtxt)
         sys.exit(1)
     bitmap = zint.bitmapbuf(symbol)
```

### Comparing `zint-1.2/setup.py` & `zint-1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
 Usage closely follows the C API:
 
 <http://www.zint.org.uk/Manual.aspx?type=p&page=5>
     """
     pass
 
-setup(name='zint',
-      version='1.2',
-      description='Python ctypes interface to libzint',
+setup(description='Python ctypes interface to libzint',
       long_description=description.__doc__.strip(),
       url='http://github.com/jmptbl/python-zint',
       author='Aragon Gouveia',
       author_email='aragon@phat.za.net',
       packages=['zint'],
       keywords='zint ctypes',
       license='BSD',
```

