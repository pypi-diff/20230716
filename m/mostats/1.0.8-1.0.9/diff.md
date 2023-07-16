# Comparing `tmp/mostats-1.0.8-py3-none-any.whl.zip` & `tmp/mostats-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 18791 bytes, number of entries: 8
+Zip file size: 18788 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 08:19 mostats/__init__.py
--rw-r--r--  2.0 unx    13354 b- defN 23-Jul-15 18:15 mostats/getCluster.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     5555 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      633 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/RECORD
-8 files, 54843 bytes uncompressed, 17683 bytes compressed:  67.8%
+-rw-r--r--  2.0 unx    13351 b- defN 23-Jul-16 02:44 mostats/getCluster.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-16 02:44 mostats-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5555 b- defN 23-Jul-16 02:44 mostats-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 02:44 mostats-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-16 02:44 mostats-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-16 02:44 mostats-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jul-16 02:44 mostats-1.0.9.dist-info/RECORD
+8 files, 54840 bytes uncompressed, 17680 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: mostats/__init__.py
 Comment: 
 
 Filename: mostats/getCluster.py
 Comment: 
 
-Filename: mostats-1.0.8.dist-info/LICENSE
+Filename: mostats-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: mostats-1.0.8.dist-info/METADATA
+Filename: mostats-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: mostats-1.0.8.dist-info/WHEEL
+Filename: mostats-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: mostats-1.0.8.dist-info/entry_points.txt
+Filename: mostats-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: mostats-1.0.8.dist-info/top_level.txt
+Filename: mostats-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mostats-1.0.8.dist-info/RECORD
+Filename: mostats-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mostats/getCluster.py

```diff
@@ -30,29 +30,29 @@
     argparser.add_argument('-fa', '--fa', default="",
                             help='Frequently access ratio in percent (input number only)\n')
     argparser.add_argument('-iops', '--iops', default="",
                             help='Expected IOPS\n')
     args = argparser.parse_args()
     
     print('\nMostats - Get the MongoDB database statistic to an excel file\nPlease follow the instruction by run mostats -h\n')
+    
+    if args.urlfile != "":
+        conn_pool = read_file(args.urlfile)          
+    else: 
+        conn_pool = args.url
 
     if args.namefile != "":
         cname = read_file(args.namefile)
         if(len(conn_pool) != len(cname)) and (len(cname) >0 ):
             raise Exception(f'The number of MongoDB URL "{len(conn_pool)}" doesnt match with the number of cluster name "{len(cname)}"')
     elif args.name != "": 
         cname = args.name
         if(len(conn_pool) != len(cname)) and (len(cname) >0 ):
             raise Exception(f'The number of MongoDB URL "{len(conn_pool)}" doesnt match with the number of cluster name "{len(cname)}"')
 
-    if args.urlfile != "":
-        conn_pool = read_file(args.urlfile)          
-    else: 
-        conn_pool = args.url       
-
     if args.name == "":
         print(f'Get the database information from : "{conn_pool}" and save to "{args.excelfile}"')
     else:
         print(f'Get the database information from : "{conn_pool}" with cluster name "{args.name}" and save to "{args.excelfile}"')
     #print('\n')
     print('\nPlease wait as it might take a while...')
```

## Comparing `mostats-1.0.8.dist-info/LICENSE` & `mostats-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mostats-1.0.8.dist-info/METADATA` & `mostats-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostats
-Version: 1.0.8
+Version: 1.0.9
 Summary: Get the MongoDB database statistic to a local CSV file
 Home-page: https://github.com/pix3lize/mostats
 Author: Hendri Tjipto
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `mostats-1.0.8.dist-info/RECORD` & `mostats-1.0.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 mostats/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mostats/getCluster.py,sha256=yvXbs0Su68z-KP9Is3mH_UzCzs1NpTZMljYEahAlhe0,13354
-mostats-1.0.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-mostats-1.0.8.dist-info/METADATA,sha256=WOrrzQomu4Q57wgESCilm4Awa4ux5_rbgARRCkG4QWo,5555
-mostats-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mostats-1.0.8.dist-info/entry_points.txt,sha256=MFCYVlscfpdhPtCwqqleHqxY9mGkYu6bMfHisM19ICk,52
-mostats-1.0.8.dist-info/top_level.txt,sha256=BIn_J562X-h3Crx1bzpv_IHDpL981YY0z2Aqb0z6O4I,8
-mostats-1.0.8.dist-info/RECORD,,
+mostats/getCluster.py,sha256=mCKEfE_7Na_jKe-W4nJwS4eQZJZTYVMBZKPCDwOu89k,13351
+mostats-1.0.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+mostats-1.0.9.dist-info/METADATA,sha256=UirJyPZnSr3l2HkSiTVlDZ196cwXNmPhh1iyUMHB4AA,5555
+mostats-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mostats-1.0.9.dist-info/entry_points.txt,sha256=MFCYVlscfpdhPtCwqqleHqxY9mGkYu6bMfHisM19ICk,52
+mostats-1.0.9.dist-info/top_level.txt,sha256=BIn_J562X-h3Crx1bzpv_IHDpL981YY0z2Aqb0z6O4I,8
+mostats-1.0.9.dist-info/RECORD,,
```

