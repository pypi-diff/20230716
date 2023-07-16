# Comparing `tmp/PlistParser-2023.7.18.tar.gz` & `tmp/PlistParser-2023.7.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlistParser-2023.7.18.tar", last modified: Sun Jul 16 08:57:03 2023, max compression
+gzip compressed data, was "PlistParser-2023.7.19.tar", last modified: Sun Jul 16 15:28:22 2023, max compression
```

## Comparing `PlistParser-2023.7.18.tar` & `PlistParser-2023.7.19.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.957795 PlistParser-2023.7.18/
--rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.18/LICENSE.txt
--rw-rw-rw-   0        0        0     7881 2023-07-16 08:57:03.956794 PlistParser-2023.7.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.943217 PlistParser-2023.7.18/PlistParser/
--rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.18/PlistParser/Base64.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.956794 PlistParser-2023.7.18/PlistParser/DisplaceTemplate/
--rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.18/PlistParser/DisplaceTemplate/__init__.py
--rw-rw-rw-   0        0        0     3215 2023-07-14 12:40:42.000000 PlistParser-2023.7.18/PlistParser/Extend.py
--rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.18/PlistParser/Info.py
--rw-rw-rw-   0        0        0    12291 2023-07-16 05:59:01.000000 PlistParser-2023.7.18/PlistParser/Plist.py
--rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.18/PlistParser/PlistParser.py
--rw-rw-rw-   0        0        0      174 2023-07-16 08:56:15.000000 PlistParser-2023.7.18/PlistParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.955795 PlistParser-2023.7.18/PlistParser.egg-info/
--rw-rw-rw-   0        0        0     7881 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7179 2023-07-16 08:48:08.000000 PlistParser-2023.7.18/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 08:57:03.957795 PlistParser-2023.7.18/setup.cfg
--rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:28:22.370548 PlistParser-2023.7.19/
+-rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.19/LICENSE.txt
+-rw-rw-rw-   0        0        0     7881 2023-07-16 15:28:22.370548 PlistParser-2023.7.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 15:28:22.366549 PlistParser-2023.7.19/PlistParser/
+-rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.19/PlistParser/Base64.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:28:22.370548 PlistParser-2023.7.19/PlistParser/DisplaceTemplate/
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.19/PlistParser/DisplaceTemplate/__init__.py
+-rw-rw-rw-   0        0        0     3215 2023-07-14 12:40:42.000000 PlistParser-2023.7.19/PlistParser/Extend.py
+-rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.19/PlistParser/Info.py
+-rw-rw-rw-   0        0        0    12291 2023-07-16 05:59:01.000000 PlistParser-2023.7.19/PlistParser/Plist.py
+-rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.19/PlistParser/PlistParser.py
+-rw-rw-rw-   0        0        0      174 2023-07-16 15:28:17.000000 PlistParser-2023.7.19/PlistParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:28:22.369548 PlistParser-2023.7.19/PlistParser.egg-info/
+-rw-rw-rw-   0        0        0     7881 2023-07-16 15:28:22.000000 PlistParser-2023.7.19/PlistParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-16 15:28:22.000000 PlistParser-2023.7.19/PlistParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 15:28:22.000000 PlistParser-2023.7.19/PlistParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 15:28:22.000000 PlistParser-2023.7.19/PlistParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7179 2023-07-16 08:48:08.000000 PlistParser-2023.7.19/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 15:28:22.371661 PlistParser-2023.7.19/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.19/setup.py
```

### Comparing `PlistParser-2023.7.18/LICENSE.txt` & `PlistParser-2023.7.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.18/PKG-INFO` & `PlistParser-2023.7.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.18
+Version: 2023.7.19
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
```

### Comparing `PlistParser-2023.7.18/PlistParser/Extend.py` & `PlistParser-2023.7.19/PlistParser/Extend.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.18/PlistParser/Info.py` & `PlistParser-2023.7.19/PlistParser/Info.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.18/PlistParser/Plist.py` & `PlistParser-2023.7.19/PlistParser/Plist.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.18/PlistParser/PlistParser.py` & `PlistParser-2023.7.19/PlistParser/PlistParser.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.18/PlistParser.egg-info/PKG-INFO` & `PlistParser-2023.7.19/PlistParser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.18
+Version: 2023.7.19
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
```

### Comparing `PlistParser-2023.7.18/README.md` & `PlistParser-2023.7.19/README.md`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.18/setup.py` & `PlistParser-2023.7.19/setup.py`

 * *Files identical despite different names*

