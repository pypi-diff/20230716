# Comparing `tmp/liqa-1.3.2.tar.gz` & `tmp/liqa-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liqa-1.3.2.tar", last modified: Sun Jul 16 06:24:19 2023, max compression
+gzip compressed data, was "liqa-1.3.3.tar", last modified: Sun Jul 16 06:30:07 2023, max compression
```

## Comparing `liqa-1.3.2.tar` & `liqa-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 06:24:19.853088 liqa-1.3.2/
--rw-r--r--   0 wenli      (501) staff       (20)      693 2023-07-16 05:30:58.000000 liqa-1.3.2/LICENSE
--rw-r--r--   0 wenli      (501) staff       (20)       25 2023-07-16 05:30:58.000000 liqa-1.3.2/MANIFEST.in
--rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-07-16 06:24:19.852924 liqa-1.3.2/PKG-INFO
--rw-r--r--   0 wenli      (501) staff       (20)     1743 2023-07-16 05:30:58.000000 liqa-1.3.2/README.md
-drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 06:24:19.851229 liqa-1.3.2/liqa.egg-info/
--rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-07-16 06:24:19.000000 liqa-1.3.2/liqa.egg-info/PKG-INFO
--rw-r--r--   0 wenli      (501) staff       (20)      387 2023-07-16 06:24:19.000000 liqa-1.3.2/liqa.egg-info/SOURCES.txt
--rw-r--r--   0 wenli      (501) staff       (20)        1 2023-07-16 06:24:19.000000 liqa-1.3.2/liqa.egg-info/dependency_links.txt
--rw-r--r--   0 wenli      (501) staff       (20)       44 2023-07-16 06:24:19.000000 liqa-1.3.2/liqa.egg-info/entry_points.txt
--rw-r--r--   0 wenli      (501) staff       (20)       16 2023-07-16 06:24:19.000000 liqa-1.3.2/liqa.egg-info/requires.txt
--rw-r--r--   0 wenli      (501) staff       (20)        9 2023-07-16 06:24:19.000000 liqa-1.3.2/liqa.egg-info/top_level.txt
-drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 06:24:19.852724 liqa-1.3.2/liqa_src/
--rw-r--r--   0 wenli      (501) staff       (20)     5381 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/PreProcess.pl
--rw-r--r--   0 wenli      (501) staff       (20)     6619 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/PreProcess_gtf.pl
--rw-r--r--   0 wenli      (501) staff       (20)     2302 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/group_process.pl
--rw-r--r--   0 wenli      (501) staff       (20)     4321 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/liqa.py
--rw-r--r--   0 wenli      (501) staff       (20)     2949 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/my_functions.py
--rw-r--r--   0 wenli      (501) staff       (20)    19896 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/noveliso.py
--rw-r--r--   0 wenli      (501) staff       (20)    26418 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/quantify.py
--rw-r--r--   0 wenli      (501) staff       (20)     5750 2023-07-16 05:30:58.000000 liqa-1.3.2/liqa_src/testDAS.R
--rw-r--r--   0 wenli      (501) staff       (20)       38 2023-07-16 06:24:19.853142 liqa-1.3.2/setup.cfg
--rw-r--r--   0 wenli      (501) staff       (20)     1199 2023-07-16 06:23:39.000000 liqa-1.3.2/setup.py
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 06:30:07.299283 liqa-1.3.3/
+-rw-r--r--   0 wenli      (501) staff       (20)      693 2023-07-16 05:30:58.000000 liqa-1.3.3/LICENSE
+-rw-r--r--   0 wenli      (501) staff       (20)       25 2023-07-16 05:30:58.000000 liqa-1.3.3/MANIFEST.in
+-rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-07-16 06:30:07.299116 liqa-1.3.3/PKG-INFO
+-rw-r--r--   0 wenli      (501) staff       (20)     1743 2023-07-16 05:30:58.000000 liqa-1.3.3/README.md
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 06:30:07.297449 liqa-1.3.3/liqa.egg-info/
+-rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-07-16 06:30:07.000000 liqa-1.3.3/liqa.egg-info/PKG-INFO
+-rw-r--r--   0 wenli      (501) staff       (20)      387 2023-07-16 06:30:07.000000 liqa-1.3.3/liqa.egg-info/SOURCES.txt
+-rw-r--r--   0 wenli      (501) staff       (20)        1 2023-07-16 06:30:07.000000 liqa-1.3.3/liqa.egg-info/dependency_links.txt
+-rw-r--r--   0 wenli      (501) staff       (20)       44 2023-07-16 06:30:07.000000 liqa-1.3.3/liqa.egg-info/entry_points.txt
+-rw-r--r--   0 wenli      (501) staff       (20)       16 2023-07-16 06:30:07.000000 liqa-1.3.3/liqa.egg-info/requires.txt
+-rw-r--r--   0 wenli      (501) staff       (20)        9 2023-07-16 06:30:07.000000 liqa-1.3.3/liqa.egg-info/top_level.txt
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 06:30:07.298912 liqa-1.3.3/liqa_src/
+-rw-r--r--   0 wenli      (501) staff       (20)     5381 2023-07-16 05:30:58.000000 liqa-1.3.3/liqa_src/PreProcess.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     6619 2023-07-16 05:30:58.000000 liqa-1.3.3/liqa_src/PreProcess_gtf.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     2302 2023-07-16 05:30:58.000000 liqa-1.3.3/liqa_src/group_process.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     4321 2023-07-16 05:30:58.000000 liqa-1.3.3/liqa_src/liqa.py
+-rw-r--r--   0 wenli      (501) staff       (20)     2949 2023-07-16 05:30:58.000000 liqa-1.3.3/liqa_src/my_functions.py
+-rw-r--r--   0 wenli      (501) staff       (20)    19880 2023-07-16 06:28:53.000000 liqa-1.3.3/liqa_src/noveliso.py
+-rw-r--r--   0 wenli      (501) staff       (20)    26418 2023-07-16 05:30:58.000000 liqa-1.3.3/liqa_src/quantify.py
+-rw-r--r--   0 wenli      (501) staff       (20)     5750 2023-07-16 05:30:58.000000 liqa-1.3.3/liqa_src/testDAS.R
+-rw-r--r--   0 wenli      (501) staff       (20)       38 2023-07-16 06:30:07.299323 liqa-1.3.3/setup.cfg
+-rw-r--r--   0 wenli      (501) staff       (20)     1199 2023-07-16 06:29:42.000000 liqa-1.3.3/setup.py
```

### Comparing `liqa-1.3.2/LICENSE` & `liqa-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/PKG-INFO` & `liqa-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liqa
-Version: 1.3.2
+Version: 1.3.3
 Summary: A statistical tool to quantify isoform-specific expression using long-read RNA-seq
 Home-page: https://github.com/WGLab/LIQA
 Author: Yu Hu
 Author-email: huyu999999@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `liqa-1.3.2/README.md` & `liqa-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/liqa.egg-info/PKG-INFO` & `liqa-1.3.3/liqa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liqa
-Version: 1.3.2
+Version: 1.3.3
 Summary: A statistical tool to quantify isoform-specific expression using long-read RNA-seq
 Home-page: https://github.com/WGLab/LIQA
 Author: Yu Hu
 Author-email: huyu999999@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `liqa-1.3.2/liqa_src/PreProcess.pl` & `liqa-1.3.3/liqa_src/PreProcess.pl`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/liqa_src/PreProcess_gtf.pl` & `liqa-1.3.3/liqa_src/PreProcess_gtf.pl`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/liqa_src/group_process.pl` & `liqa-1.3.3/liqa_src/group_process.pl`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/liqa_src/liqa.py` & `liqa-1.3.3/liqa_src/liqa.py`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/liqa_src/my_functions.py` & `liqa-1.3.3/liqa_src/my_functions.py`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/liqa_src/noveliso.py` & `liqa-1.3.3/liqa_src/noveliso.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,15 +407,15 @@
                     if qualitycheck[readName] == 1:
                         readCount1iso += 1
                     readCount += 1
 
     ### COMPATIBLE MATRIX OBTAINED !!!
     ###############################################################################################################
 
-    #print(",".join(tmpisoinf))
+    print(gene)
     noveliso_wt = []
     for weight in noveliso_ct:
         if noveliso_ct[weight] >= weightF:
             noveliso_wt.append(weight)
 
     refoutput = geneStructureInformation[gene][0]
```

### Comparing `liqa-1.3.2/liqa_src/quantify.py` & `liqa-1.3.3/liqa_src/quantify.py`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/liqa_src/testDAS.R` & `liqa-1.3.3/liqa_src/testDAS.R`

 * *Files identical despite different names*

### Comparing `liqa-1.3.2/setup.py` & `liqa-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="liqa",
-    version="1.3.2",
+    version="1.3.3",
     author="Yu Hu",
     author_email="huyu999999@gmail.com",
     description="A statistical tool to quantify isoform-specific expression using long-read RNA-seq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WGLab/LIQA",
     license="MIT",
```

