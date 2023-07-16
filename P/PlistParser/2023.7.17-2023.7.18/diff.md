# Comparing `tmp/PlistParser-2023.7.17.tar.gz` & `tmp/PlistParser-2023.7.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlistParser-2023.7.17.tar", last modified: Thu Jul 13 14:51:38 2023, max compression
+gzip compressed data, was "PlistParser-2023.7.18.tar", last modified: Sun Jul 16 08:57:03 2023, max compression
```

## Comparing `PlistParser-2023.7.17.tar` & `PlistParser-2023.7.18.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.293854 PlistParser-2023.7.17/
--rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.17/LICENSE.txt
--rw-rw-rw-   0        0        0    15688 2023-07-13 14:51:38.293854 PlistParser-2023.7.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.282791 PlistParser-2023.7.17/PlistParser/
--rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.17/PlistParser/Base64.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.292871 PlistParser-2023.7.17/PlistParser/DisplaceTemplate/
--rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.17/PlistParser/DisplaceTemplate/__init__.py
--rw-rw-rw-   0        0        0       47 2023-07-11 15:47:49.000000 PlistParser-2023.7.17/PlistParser/Extend.py
--rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.17/PlistParser/Info.py
--rw-rw-rw-   0        0        0     6001 2023-07-13 14:41:47.000000 PlistParser-2023.7.17/PlistParser/Plist.py
--rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.17/PlistParser/PlistParser.py
--rw-rw-rw-   0        0        0      174 2023-07-13 14:46:51.000000 PlistParser-2023.7.17/PlistParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.292871 PlistParser-2023.7.17/PlistParser.egg-info/
--rw-rw-rw-   0        0        0    15688 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14986 2023-07-13 14:51:28.000000 PlistParser-2023.7.17/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 14:51:38.293854 PlistParser-2023.7.17/setup.cfg
--rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.957795 PlistParser-2023.7.18/
+-rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.18/LICENSE.txt
+-rw-rw-rw-   0        0        0     7881 2023-07-16 08:57:03.956794 PlistParser-2023.7.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.943217 PlistParser-2023.7.18/PlistParser/
+-rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.18/PlistParser/Base64.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.956794 PlistParser-2023.7.18/PlistParser/DisplaceTemplate/
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.18/PlistParser/DisplaceTemplate/__init__.py
+-rw-rw-rw-   0        0        0     3215 2023-07-14 12:40:42.000000 PlistParser-2023.7.18/PlistParser/Extend.py
+-rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.18/PlistParser/Info.py
+-rw-rw-rw-   0        0        0    12291 2023-07-16 05:59:01.000000 PlistParser-2023.7.18/PlistParser/Plist.py
+-rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.18/PlistParser/PlistParser.py
+-rw-rw-rw-   0        0        0      174 2023-07-16 08:56:15.000000 PlistParser-2023.7.18/PlistParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:57:03.955795 PlistParser-2023.7.18/PlistParser.egg-info/
+-rw-rw-rw-   0        0        0     7881 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 08:57:03.000000 PlistParser-2023.7.18/PlistParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7179 2023-07-16 08:48:08.000000 PlistParser-2023.7.18/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 08:57:03.957795 PlistParser-2023.7.18/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.18/setup.py
```

### Comparing `PlistParser-2023.7.17/LICENSE.txt` & `PlistParser-2023.7.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.17/PlistParser/Info.py` & `PlistParser-2023.7.18/PlistParser/Info.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.17/PlistParser/PlistParser.py` & `PlistParser-2023.7.18/PlistParser/PlistParser.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.17/setup.py` & `PlistParser-2023.7.18/setup.py`

 * *Files identical despite different names*

