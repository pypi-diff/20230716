# Comparing `tmp/colorthon-2.3.6.tar.gz` & `tmp/colorthon-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorthon-2.3.6.tar", last modified: Tue Jul 11 19:44:55 2023, max compression
+gzip compressed data, was "colorthon-2.3.9.tar", last modified: Sun Jul 16 15:29:58 2023, max compression
```

## Comparing `colorthon-2.3.6.tar` & `colorthon-2.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 19:44:55.234666 colorthon-2.3.6/
--rw-rw-rw-   0        0        0     3025 2023-07-11 19:44:55.234666 colorthon-2.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2330 2023-07-11 19:38:35.000000 colorthon-2.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 19:44:55.234666 colorthon-2.3.6/colorthon.egg-info/
--rw-rw-rw-   0        0        0     3025 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 19:44:55.000000 colorthon-2.3.6/colorthon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 19:44:55.234666 colorthon-2.3.6/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-07-11 19:43:58.000000 colorthon-2.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:29:58.814257 colorthon-2.3.9/
+-rw-rw-rw-   0        0        0     3690 2023-07-16 15:29:58.813257 colorthon-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2330 2023-07-11 19:38:35.000000 colorthon-2.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 15:29:58.813257 colorthon-2.3.9/colorthon.egg-info/
+-rw-rw-rw-   0        0        0     3690 2023-07-16 15:29:58.000000 colorthon-2.3.9/colorthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-07-16 15:29:58.000000 colorthon-2.3.9/colorthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 15:29:58.000000 colorthon-2.3.9/colorthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 15:29:58.000000 colorthon-2.3.9/colorthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 15:29:58.814257 colorthon-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-07-16 15:06:58.000000 colorthon-2.3.9/setup.py
```

### Comparing `colorthon-2.3.6/PKG-INFO` & `colorthon-2.3.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: colorthon
-Version: 2.3.6
-Summary: Python package for coloring text and background text
-Home-page: https://github.com/colorthon/colorthon
-Author: Mohammadreza Fekri
-Author-email: Pymmdrza@Gmail.Com
-License: UNKNOWN
-Project-URL: Documentation, https://colorthon.github.io/colorthon/
-Project-URL: Personal Website, https://mmdrza.com
-Keywords: colorthon,text color,console,python color,color print,text color,back color
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Colorthon
 
 Colorthon is a powerful Python package that provides a simple and intuitive way to work with colors in the terminal.
 
 ## Features
 
 - Easy-to-use syntax for applying colors and background colors to text in the terminal.
@@ -94,9 +76,7 @@
 
 other package :
 
 **_Blockthon_** - _Generate Easy and Fast Private Key & Mnemonic and Decimal , Binary & seed (Bytes)_ , Compress and UnCompress address Bitcoin , Ethereum , TRON, Dogecoin, Litecoin, zcash, Digibyte, Dash, Qtum, Ravencoin, BitcoinGold
 
 programmer and Owner Website : [Mmdrza.Com](https://mmdrza.com)
 
-
-
```

### Comparing `colorthon-2.3.6/setup.py` & `colorthon-2.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='colorthon',
-    version='2.3.6',
+    version='2.3.9',
     author='Mohammadreza Fekri',
     author_email='Pymmdrza@Gmail.Com',
     description='Python package for coloring text and background text',
     keywords=['colorthon', 'text color', 'console', 'python color', 'color print', 'text color', 'back color'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/colorthon/colorthon",
```

