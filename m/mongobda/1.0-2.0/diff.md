# Comparing `tmp/mongobda-1.0-py3-none-any.whl.zip` & `tmp/mongobda-2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7524 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    23054 b- defN 23-Jul-16 18:26 mongobda/__init__.py
--rw-rw-rw-  2.0 fat     1048 b- defN 23-Jul-16 18:29 mongobda-1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      364 b- defN 23-Jul-16 18:29 mongobda-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 18:29 mongobda-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 18:29 mongobda-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      461 b- defN 23-Jul-16 18:29 mongobda-1.0.dist-info/RECORD
-6 files, 25028 bytes uncompressed, 6690 bytes compressed:  73.3%
+Zip file size: 7520 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    23035 b- defN 23-Jul-16 18:32 mongobda/__init__.py
+-rw-rw-rw-  2.0 fat     1048 b- defN 23-Jul-16 18:32 mongobda-2.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      364 b- defN 23-Jul-16 18:32 mongobda-2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 18:32 mongobda-2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 18:32 mongobda-2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      461 b- defN 23-Jul-16 18:32 mongobda-2.0.dist-info/RECORD
+6 files, 25009 bytes uncompressed, 6686 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: mongobda/__init__.py
 Comment: 
 
-Filename: mongobda-1.0.dist-info/LICENSE.txt
+Filename: mongobda-2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mongobda-1.0.dist-info/METADATA
+Filename: mongobda-2.0.dist-info/METADATA
 Comment: 
 
-Filename: mongobda-1.0.dist-info/WHEEL
+Filename: mongobda-2.0.dist-info/WHEEL
 Comment: 
 
-Filename: mongobda-1.0.dist-info/top_level.txt
+Filename: mongobda-2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mongobda-1.0.dist-info/RECORD
+Filename: mongobda-2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mongobda/__init__.py

```diff
@@ -776,18 +776,15 @@
   Output:
   Check database and data inserted in collection
   >> show dbs
   >> use mybigdata
   >> show collections
   >> db.student.findOne()
   >> db.student.count()
-  
-
-         
-                """)
+              """)
 
     
 
 
 
     else:
         print("invalid input")
```

## Comparing `mongobda-1.0.dist-info/LICENSE.txt` & `mongobda-2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

