# Comparing `tmp/tf2-sku-to-name-1.0.4.tar.gz` & `tmp/tf2-sku-to-name-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2-sku-to-name-1.0.4.tar", last modified: Fri Jul 14 15:25:33 2023, max compression
+gzip compressed data, was "tf2-sku-to-name-1.0.5.tar", last modified: Sun Jul 16 06:43:08 2023, max compression
```

## Comparing `tf2-sku-to-name-1.0.4.tar` & `tf2-sku-to-name-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:33.001724 tf2-sku-to-name-1.0.4/
--rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.4/LICENSE
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:25:33.001602 tf2-sku-to-name-1.0.4/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)     1508 2023-07-14 14:53:36.000000 tf2-sku-to-name-1.0.4/README.md
--rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-14 15:25:33.001764 tf2-sku-to-name-1.0.4/setup.cfg
--rw-r--r--   0 ketan1     (502) staff       (20)      621 2023-07-14 15:25:28.000000 tf2-sku-to-name-1.0.4/setup.py
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:32.998936 tf2-sku-to-name-1.0.4/sku/
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:32.999045 tf2-sku-to-name-1.0.4/sku/data/
--rw-r--r--   0 ketan1     (502) staff       (20)  3849421 2023-07-14 15:22:12.000000 tf2-sku-to-name-1.0.4/sku/data/data.json
--rw-r--r--   0 ketan1     (502) staff       (20)      668 2023-07-14 07:35:40.000000 tf2-sku-to-name-1.0.4/sku/models.py
--rw-r--r--   0 ketan1     (502) staff       (20)     5204 2023-07-14 15:20:38.000000 tf2-sku-to-name-1.0.4/sku/parser.py
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:33.001410 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)      267 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/SOURCES.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/dependency_links.txt
--rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/requires.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        4 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/top_level.txt
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-16 06:43:08.139368 tf2-sku-to-name-1.0.5/
+-rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.5/LICENSE
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-16 06:43:08.139232 tf2-sku-to-name-1.0.5/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)     1508 2023-07-14 14:53:36.000000 tf2-sku-to-name-1.0.5/README.md
+-rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-16 06:43:08.139412 tf2-sku-to-name-1.0.5/setup.cfg
+-rw-r--r--   0 ketan1     (502) staff       (20)      621 2023-07-16 06:42:59.000000 tf2-sku-to-name-1.0.5/setup.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-16 06:43:08.133875 tf2-sku-to-name-1.0.5/sku/
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-16 06:43:08.134135 tf2-sku-to-name-1.0.5/sku/data/
+-rw-r--r--   0 ketan1     (502) staff       (20)  3849421 2023-07-14 15:22:12.000000 tf2-sku-to-name-1.0.5/sku/data/data.json
+-rw-r--r--   0 ketan1     (502) staff       (20)      804 2023-07-16 06:42:54.000000 tf2-sku-to-name-1.0.5/sku/models.py
+-rw-r--r--   0 ketan1     (502) staff       (20)     5204 2023-07-14 15:20:38.000000 tf2-sku-to-name-1.0.5/sku/parser.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-16 06:43:08.139027 tf2-sku-to-name-1.0.5/tf2_sku_to_name.egg-info/
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-16 06:43:08.000000 tf2-sku-to-name-1.0.5/tf2_sku_to_name.egg-info/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)      267 2023-07-16 06:43:08.000000 tf2-sku-to-name-1.0.5/tf2_sku_to_name.egg-info/SOURCES.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-16 06:43:08.000000 tf2-sku-to-name-1.0.5/tf2_sku_to_name.egg-info/dependency_links.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-16 06:43:08.000000 tf2-sku-to-name-1.0.5/tf2_sku_to_name.egg-info/requires.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        4 2023-07-16 06:43:08.000000 tf2-sku-to-name-1.0.5/tf2_sku_to_name.egg-info/top_level.txt
```

### Comparing `tf2-sku-to-name-1.0.4/LICENSE` & `tf2-sku-to-name-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.4/README.md` & `tf2-sku-to-name-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.4/setup.py` & `tf2-sku-to-name-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tf2-sku-to-name',
-    version='1.0.4',
+    version='1.0.5',
     author='Purple Barber',
     description="A python library that parses TF2 item SKU to the item's name and vice versa.",
     url='https://github.com/purplebarber/tf2-sku',
     license='MIT',
     packages=["sku"],
     package_data={
         'sku': ['data/data.json'],
```

### Comparing `tf2-sku-to-name-1.0.4/sku/data/data.json` & `tf2-sku-to-name-1.0.5/sku/data/data.json`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.4/sku/models.py` & `tf2-sku-to-name-1.0.5/sku/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from json import dumps
 
 
 class itemClass:
-    def __init__(self):
+    def __init__(self, data=None):
         # Initialize the properties with their default values
         self.Defindex = 0
         self.Quality = 6
         self.Craftable = True
         self.Killstreak = 0
         self.Australium = False
         self.Festive = False
@@ -16,10 +16,15 @@
         self.ElevatedQuality = None
         self.Target = None
         self.CraftNum = None
         self.CrateSn = None
         self.Output = None
         self.OutputQuality = None
 
+        # Update the properties with the provided data
+        if data is not None:
+            self.__dict__.update(data)
+
+
     def __str__(self):
         # Serialize the object to a JSON string
         return dumps(self.__dict__)
```

### Comparing `tf2-sku-to-name-1.0.4/sku/parser.py` & `tf2-sku-to-name-1.0.5/sku/parser.py`

 * *Files identical despite different names*

