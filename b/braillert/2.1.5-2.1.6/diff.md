# Comparing `tmp/braillert-2.1.5-py3-none-any.whl.zip` & `tmp/braillert-2.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9003 bytes, number of entries: 13
+Zip file size: 9047 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      519 b- defN 22-Jun-24 20:11 braillert/__init__.py
--rw-r--r--  2.0 unx     2346 b- defN 22-Nov-05 20:45 braillert/colors.py
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jul-16 11:59 braillert/colors.py
 -rw-r--r--  2.0 unx      335 b- defN 22-Jun-25 15:03 braillert/exceptions.py
--rw-r--r--  2.0 unx     3887 b- defN 22-Nov-05 12:28 braillert/generator.py
+-rw-r--r--  2.0 unx     3887 b- defN 23-Feb-19 10:27 braillert/generator.py
 -rw-r--r--  2.0 unx     1434 b- defN 22-Nov-04 21:47 braillert/logger.py
 -rw-r--r--  2.0 unx     9689 b- defN 22-Nov-04 21:37 braillert/logo.ansi
--rw-r--r--  2.0 unx     5823 b- defN 22-Nov-25 19:27 braillert/main.py
--rw-r--r--  2.0 unx     1066 b- defN 22-Nov-25 19:29 braillert-2.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      227 b- defN 22-Nov-25 19:29 braillert-2.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-25 19:29 braillert-2.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 22-Nov-25 19:29 braillert-2.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 22-Nov-25 19:29 braillert-2.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1029 b- defN 22-Nov-25 19:29 braillert-2.1.5.dist-info/RECORD
-13 files, 26507 bytes uncompressed, 7291 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx     5889 b- defN 22-Nov-29 19:25 braillert/main.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-16 12:04 braillert-2.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-16 12:04 braillert-2.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 12:04 braillert-2.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-16 12:04 braillert-2.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-16 12:04 braillert-2.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1029 b- defN 23-Jul-16 12:04 braillert-2.1.6.dist-info/RECORD
+13 files, 26665 bytes uncompressed, 7335 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: braillert/logo.ansi
 Comment: 
 
 Filename: braillert/main.py
 Comment: 
 
-Filename: braillert-2.1.5.dist-info/LICENSE
+Filename: braillert-2.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: braillert-2.1.5.dist-info/METADATA
+Filename: braillert-2.1.6.dist-info/METADATA
 Comment: 
 
-Filename: braillert-2.1.5.dist-info/WHEEL
+Filename: braillert-2.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: braillert-2.1.5.dist-info/entry_points.txt
+Filename: braillert-2.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: braillert-2.1.5.dist-info/top_level.txt
+Filename: braillert-2.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: braillert-2.1.5.dist-info/RECORD
+Filename: braillert-2.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## braillert/colors.py

```diff
@@ -7,16 +7,18 @@
 ANSI_RESETTER: str = ESC + "[0m"
 
 LOW_8_COLORS: tuple = ((0, 0, 0), (128, 0, 0), (0, 128, 0), (128, 128, 0),
                         (0, 0, 128), (128, 0, 128), (0, 128, 128), (192, 192, 192))
 
 HIGH_8_COLORS: tuple = ((128, 128, 128), (255, 0, 0), (0, 255, 0), (255, 255, 0),
                         (0, 0, 255), (255, 0, 255), (0, 255, 255), (255, 255, 255))
-LOW_8_COLORS_DICT: dict = {str(i): LOW_8_COLORS[i] for i in range(8)}
-HIGH_8_COLORS_DICT: dict = {str(i + 8): HIGH_8_COLORS[i] for i in range(8)}
+LOW_8_COLORS_PREFIX = 30
+LOW_8_COLORS_DICT: dict = {str(LOW_8_COLORS_PREFIX + i): LOW_8_COLORS[i] for i in range(8)}
+HIGH_8_COLORS_PREFIX = 40
+HIGH_8_COLORS_DICT: dict = {str(HIGH_8_COLORS_PREFIX + i): HIGH_8_COLORS[i] for i in range(8)}
 
 EXTENDED_GRAYSCALE_COLORS: tuple = tuple((int(i*(256 / 24)),)*3 for i in range(1,24+1))
 
 COLOR_MATRIX_INCREMENTS = range(95, 256, 40)
 
 ANSI_BASIC_16_DICT: dict = {**LOW_8_COLORS_DICT, **HIGH_8_COLORS_DICT}
```

## braillert/main.py

```diff
@@ -1,11 +1,12 @@
 import argparse
 import logging
 import os
 import sys
+import traceback
 from functools import wraps
 from time import sleep
 from typing import Callable
 
 from PIL import Image
 
 from braillert.__init__ import __author__, __author_email__, __version__
@@ -112,14 +113,15 @@
         except GifUnsupportedSaveError:
             logger.error("Error! Gif arts saving is not supported.")
         except KeyboardInterrupt:
             pass
         except Exception as error: #pylint: disable = broad-except
             logger.error("Error! Unexpected exception caught:")
             logger.error(str(error))
+            logger.debug(traceback.format_exc())
 
     return wrapper
 
 @_exception_handler
 def main() -> None:
     """Main function."""
     argument_parser = argparse.ArgumentParser()
```

## Comparing `braillert-2.1.5.dist-info/LICENSE` & `braillert-2.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `braillert-2.1.5.dist-info/RECORD` & `braillert-2.1.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 braillert/__init__.py,sha256=zzG_15Gt-W0eFF3q7o4CYNFsmNK69EGWGnDk6l37jvc,519
-braillert/colors.py,sha256=vPOu5eNcbHGRqHEY9DGSMjStdgRDXYWYlxiRMXgiUcg,2346
+braillert/colors.py,sha256=zk7ludspz5Pj9iKA8-vz6VThmjtZeN32XUwxXIEViNw,2438
 braillert/exceptions.py,sha256=67LZOEEP9iM0oZ0f1Dx2l8TfovLuUZRMYlwtrN0IvUI,335
 braillert/generator.py,sha256=u-MaJWm8Nx0C8NbmFTinstusKh2v9jNkFU7m6Kb3PY8,3887
 braillert/logger.py,sha256=kii-XRTtCQ-c8s---DtJS4syvTsq20Tr_P95CfZ-mRk,1434
 braillert/logo.ansi,sha256=nkRGRqoZ5x5L_USn7rneVfjY93YV8H_xWKT__zkvgII,9689
-braillert/main.py,sha256=6LQLGHBPYt-K-WERO2SKqqkAYLn6-5whxNM1U80zg9A,5823
-braillert-2.1.5.dist-info/LICENSE,sha256=_mRuCWEeZ5U_QsODVjteoOTXjZ_jvyt1uRan7locHsI,1066
-braillert-2.1.5.dist-info/METADATA,sha256=RetJKLs88vF1X4cgbsTiMr0eDYN9z984K59SvjjXe8o,227
-braillert-2.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-braillert-2.1.5.dist-info/entry_points.txt,sha256=huN2xByRZztWPR34ldTDdDeaGFxKYjqYxTlp7i7vNkU,50
-braillert-2.1.5.dist-info/top_level.txt,sha256=1ACDvCxW7IzuT_XvGuhPVel2GOkfBeoyikP0SQT89bA,10
-braillert-2.1.5.dist-info/RECORD,,
+braillert/main.py,sha256=ys2YprKEhvPtvYWS8_VRthwdnYZtIL55M1iVgzcgwo8,5889
+braillert-2.1.6.dist-info/LICENSE,sha256=_mRuCWEeZ5U_QsODVjteoOTXjZ_jvyt1uRan7locHsI,1066
+braillert-2.1.6.dist-info/METADATA,sha256=RkTMx_lIk0npfGtgvQ-euOwDh1f4nyaVhgOxZfLE8Zc,227
+braillert-2.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+braillert-2.1.6.dist-info/entry_points.txt,sha256=huN2xByRZztWPR34ldTDdDeaGFxKYjqYxTlp7i7vNkU,50
+braillert-2.1.6.dist-info/top_level.txt,sha256=1ACDvCxW7IzuT_XvGuhPVel2GOkfBeoyikP0SQT89bA,10
+braillert-2.1.6.dist-info/RECORD,,
```

