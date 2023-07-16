# Comparing `tmp/langful-0.33-py3-none-any.whl.zip` & `tmp/langful-0.34-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5446 bytes, number of entries: 7
+Zip file size: 5480 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
--rw-rw-rw-  2.0 fat    10230 b- defN 23-Jul-06 06:51 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/RECORD
-7 files, 15479 bytes uncompressed, 4516 bytes compressed:  70.8%
+-rw-rw-rw-  2.0 fat    10190 b- defN 23-Jul-13 13:38 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/RECORD
+7 files, 15439 bytes uncompressed, 4550 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.33.dist-info/LICENSE
+Filename: langful-0.34.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.33.dist-info/METADATA
+Filename: langful-0.34.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.33.dist-info/WHEEL
+Filename: langful-0.34.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.33.dist-info/top_level.txt
+Filename: langful-0.34.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.33.dist-info/RECORD
+Filename: langful-0.34.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -1,29 +1,30 @@
 """
 # lang
 """
 from locale import getdefaultlocale
 import json
 import os
+import re
 
 def to_json( lang_file : str ) -> dict :
     """
     .lang -> .json
     """
     ret = {}
-    for i in lang_file.split( "\n" ) :
-        text = i.split( "#" )[ 0 ]
-        line = "".join( text.split( maxsplit = 2 ) )
-        if line :
-            key_value = line.split( "=" , 1 )
-            if len( key_value ) == 2 :
-                key , value = key_value
-            else :
-                raise SyntaxError( "can't to read .lang file" )
-            ret[ key ] = value
+    for line in lang_file.split( "\n" ) :
+        text = re.split( "([^#^=^\\s]+|)(\\s+=\\s+|\\s+=|=\\s+|=|)([^#^\\n]+|)" , line )
+        n = 0
+        for s in text :
+            if "=" in s :
+                break
+            n += 1
+        else :
+            continue
+        ret[ "".join( text[:n] ) ] = "".join( text[n + 1:] )
     return ret
 
 def to_lang( dict_file : dict ) -> str :
     """
     .json -> .lang
     """
     ret = ""
```

## Comparing `langful-0.33.dist-info/LICENSE` & `langful-0.34.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.33.dist-info/METADATA` & `langful-0.34.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.33
+Version: 0.34
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

