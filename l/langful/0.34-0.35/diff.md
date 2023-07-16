# Comparing `tmp/langful-0.34-py3-none-any.whl.zip` & `tmp/langful-0.35-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5480 bytes, number of entries: 7
+Zip file size: 5610 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
--rw-rw-rw-  2.0 fat    10190 b- defN 23-Jul-13 13:38 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jul-14 00:11 langful-0.34.dist-info/RECORD
-7 files, 15439 bytes uncompressed, 4550 bytes compressed:  70.5%
+-rw-rw-rw-  2.0 fat    10563 b- defN 23-Jul-16 01:14 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/RECORD
+7 files, 15812 bytes uncompressed, 4680 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.34.dist-info/LICENSE
+Filename: langful-0.35.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.34.dist-info/METADATA
+Filename: langful-0.35.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.34.dist-info/WHEEL
+Filename: langful-0.35.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.34.dist-info/top_level.txt
+Filename: langful-0.35.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.34.dist-info/RECORD
+Filename: langful-0.35.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -1,19 +1,19 @@
 """
 # lang
 """
-from locale import getdefaultlocale
+
 import json
 import os
-import re
 
 def to_json( lang_file : str ) -> dict :
     """
     .lang -> .json
     """
+    import re
     ret = {}
     for line in lang_file.split( "\n" ) :
         text = re.split( "([^#^=^\\s]+|)(\\s+=\\s+|\\s+=|=\\s+|=|)([^#^\\n]+|)" , line )
         n = 0
         for s in text :
             if "=" in s :
                 break
@@ -28,14 +28,28 @@
     .json -> .lang
     """
     ret = ""
     for key , value in dict_file.items() :
         ret += f"{ key } = { value }\n"
     return ret
 
+def getdefaultlocale() -> str :
+    """
+    getdefaultlocale will deprecated so use this
+    """
+    import locale
+    import sys
+    if sys.platform == "win32" :
+        code = __import__( "_locale" )._getdefaultlocale()[ 0 ]
+        if code[ :2 ] == "0x" :
+            code = locale.windows_locale[ code ]
+    else :
+        code = locale.getlocale()[ 0 ]
+    return code.replace( "-" , "_" ).lower()
+
 class lang :
     """
     # lang
     """
 
     def __setitem__( self , key , value ) -> None :
         """
@@ -66,19 +80,20 @@
 
     def __init__( self , lang_dir : str | dict = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
         """
         lang_dir: lang files dir, if use dict to set that to a dictionary or False
         default_locale: default locale
         json_first: is load json file first
         """
-        self.system_locale = self.system_locale_get()
+        self.system_locale = getdefaultlocale()
         self.default_locale = default_locale
         self.json_first = json_first
         self.replace_letter = "%"
         self.lang_dir = lang_dir
+        self.use_locale = None
         self.is_file = False
         self.languages = {}
         self.types = {}
         self.init()
 
     def init( self ) :
         """
@@ -138,33 +153,29 @@
         set type to file
         """
         if not os.path.exists( path ) :
             os.makedirs( path )
         self.lang_dir = path
         self.is_file = True
 
-    def system_locale_get( self ) -> str :
-        """
-        get system locale
-        """
-        return getdefaultlocale()[ 0 ].lower()
-
     @property
     def locales( self ) -> list :
         """
         locales
         """
         return list( self.types.keys() )
 
     @property
     def locale( self ) -> str :
         """
         choose locale
         """
-        if self.system_locale in self.locales :
+        if self.use_locale and self.use_locale in self.locales :
+            return self.use_locale
+        elif self.system_locale in self.locales :
             return self.system_locale
         elif self.default_locale in self.locales :
             return self.default_locale
         else :
             raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
 
     @property
@@ -213,18 +224,17 @@
         else :
             return self.replace_letter
 
     def locale_set( self , locale : str = None  ) -> None :
         """
         if give a locale then set that, else reset it
         """
-        if locale != None :
-            self.system_locale = locale
-        else :
-            self.system_locale = self.system_locale_get()
+        if locale and locale not in self.locales :
+            raise KeyError( f"no such locale '{ locale }'" )
+        self.use_locale = locale
 
     def lang_get( self , locale : str ) -> dict :
         """
         get a lang
         """
         return self.languages[ locale ]
```

## Comparing `langful-0.34.dist-info/LICENSE` & `langful-0.35.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.34.dist-info/METADATA` & `langful-0.35.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.34
+Version: 0.35
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `langful-0.34.dist-info/RECORD` & `langful-0.35.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 langful/__init__.py,sha256=BSJ-BT1Yr3Xz-SFnmZu7QvgV5pgg2WEqUO42oM3Py2w,166
-langful/lang.py,sha256=TGLWdsGws9B9f0MtjEgryklhIWHBTK_LVdGjTJIAMP0,10190
-langful-0.34.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
-langful-0.34.dist-info/METADATA,sha256=LSXCS6bbeMA0UvAzm9CAssxHohPSBhcrWRk3zw0gzs8,3389
-langful-0.34.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-langful-0.34.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.34.dist-info/RECORD,,
+langful/lang.py,sha256=N0qHGK7XUqawFQz69mHuj9HkC5iDy4ONaKgNYspzniE,10563
+langful-0.35.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
+langful-0.35.dist-info/METADATA,sha256=DH0FqGgMp-_frBE0h0SkWOAIq-a1EKpaMmUIZTsxyT8,3389
+langful-0.35.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+langful-0.35.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.35.dist-info/RECORD,,
```

