# Comparing `tmp/mongobda-3.0-py3-none-any.whl.zip` & `tmp/mongobda-4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7525 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    23052 b- defN 23-Jul-16 18:34 mongobda/__init__.py
--rw-rw-rw-  2.0 fat     1048 b- defN 23-Jul-16 18:34 mongobda-3.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      364 b- defN 23-Jul-16 18:34 mongobda-3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 18:34 mongobda-3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 18:34 mongobda-3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      461 b- defN 23-Jul-16 18:34 mongobda-3.0.dist-info/RECORD
-6 files, 25026 bytes uncompressed, 6691 bytes compressed:  73.3%
+Zip file size: 7529 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    23115 b- defN 23-Jul-16 18:46 mongobda/__init__.py
+-rw-rw-rw-  2.0 fat     1048 b- defN 23-Jul-16 18:56 mongobda-4.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      364 b- defN 23-Jul-16 18:56 mongobda-4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 18:56 mongobda-4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 18:56 mongobda-4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      461 b- defN 23-Jul-16 18:56 mongobda-4.0.dist-info/RECORD
+6 files, 25089 bytes uncompressed, 6695 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: mongobda/__init__.py
 Comment: 
 
-Filename: mongobda-3.0.dist-info/LICENSE.txt
+Filename: mongobda-4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mongobda-3.0.dist-info/METADATA
+Filename: mongobda-4.0.dist-info/METADATA
 Comment: 
 
-Filename: mongobda-3.0.dist-info/WHEEL
+Filename: mongobda-4.0.dist-info/WHEEL
 Comment: 
 
-Filename: mongobda-3.0.dist-info/top_level.txt
+Filename: mongobda-4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mongobda-3.0.dist-info/RECORD
+Filename: mongobda-4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mongobda/__init__.py

```diff
@@ -733,28 +733,29 @@
         print("""
 
   
 
   Install mongoDB
 
   Open new command prompt
-  >> C:\users\admin> cd\ 
-  >> C:\>md data\db
-  >> C:\> cd C:\Program Files\MongoDB\Server\4.0\bin
-  >> C:\Program Files\MongoDB\Server\4.0\bin> mongod
+  >> C:\\users\\admin> cd ..
+  >> C:\\users\\admin> cd ..
+  >> C:\\>md data\\db
+  >> C:\\> cd C:\\Program Files\\MongoDB\\Server\\4.0\\bin
+  >> C:\\Program Files\\MongoDB\\Server\\4.0\\bin> mongod
   (in case error then)
-  >> C:\Program Files\MongoDB\Server\4.0\bin> mongod –repair
+  >> C:\\Program Files\\MongoDB\\Server\\4.0\\bin> mongod -repair
 
   Open new command prompt
-  >> C:\users\admin> cd C:\Program Files\MongoDB\Server\4.0\bin
-  >> C:\Program Files\MongoDB\Server\4.0\bin>mongo
+  >> C:\\users\\admin> cd C:\\Program Files\\MongoDB\\Server\\4.0\\bin
+  >> C:\\Program Files\\MongoDB\\Server\\4.0\\bin>mongo
   >> show dbs
 
   Open new command prompt and Install PyMongo
-  >> C:\users\admin> pip install pymongo
+  >> C:\\users\\admin> pip install pymongo
 
   Code:
   import pymongo
   myclient = pymongo.MongoClient('mongodb://localhost:27017/')
   mydb = myclient['mybigdata']
   print(myclient.list_database_names())
```

## Comparing `mongobda-3.0.dist-info/LICENSE.txt` & `mongobda-4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

