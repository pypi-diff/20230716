# Comparing `tmp/liqa-1.2.1.tar.gz` & `tmp/liqa-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liqa-1.2.1.tar", last modified: Fri Jun  2 15:47:15 2023, max compression
+gzip compressed data, was "liqa-1.3.0.tar", last modified: Sun Jul 16 05:36:21 2023, max compression
```

## Comparing `liqa-1.2.1.tar` & `liqa-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-06-02 15:47:15.669809 liqa-1.2.1/
--rw-r--r--   0 wenli      (501) staff       (20)      693 2023-06-02 14:46:22.000000 liqa-1.2.1/LICENSE
--rw-r--r--   0 wenli      (501) staff       (20)       25 2023-06-02 14:46:22.000000 liqa-1.2.1/MANIFEST.in
--rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-06-02 15:47:15.669674 liqa-1.2.1/PKG-INFO
--rw-r--r--   0 wenli      (501) staff       (20)     1743 2023-06-02 14:46:22.000000 liqa-1.2.1/README.md
-drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-06-02 15:47:15.663758 liqa-1.2.1/liqa.egg-info/
--rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-06-02 15:47:15.000000 liqa-1.2.1/liqa.egg-info/PKG-INFO
--rw-r--r--   0 wenli      (501) staff       (20)      385 2023-06-02 15:47:15.000000 liqa-1.2.1/liqa.egg-info/SOURCES.txt
--rw-r--r--   0 wenli      (501) staff       (20)        1 2023-06-02 15:47:15.000000 liqa-1.2.1/liqa.egg-info/dependency_links.txt
--rw-r--r--   0 wenli      (501) staff       (20)       44 2023-06-02 15:47:15.000000 liqa-1.2.1/liqa.egg-info/entry_points.txt
--rw-r--r--   0 wenli      (501) staff       (20)       16 2023-06-02 15:47:15.000000 liqa-1.2.1/liqa.egg-info/requires.txt
--rw-r--r--   0 wenli      (501) staff       (20)        9 2023-06-02 15:47:15.000000 liqa-1.2.1/liqa.egg-info/top_level.txt
-drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-06-02 15:47:15.669048 liqa-1.2.1/liqa_src/
--rw-r--r--   0 wenli      (501) staff       (20)     5381 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/PreProcess.pl
--rw-r--r--   0 wenli      (501) staff       (20)     6619 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/PreProcess_gtf.pl
--rw-r--r--   0 wenli      (501) staff       (20)     6823 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/detect.pl
--rw-r--r--   0 wenli      (501) staff       (20)     2302 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/group_process.pl
--rw-r--r--   0 wenli      (501) staff       (20)     4087 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/liqa.py
--rw-r--r--   0 wenli      (501) staff       (20)     2949 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/my_functions.py
--rw-r--r--   0 wenli      (501) staff       (20)    26418 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/quantify.py
--rw-r--r--   0 wenli      (501) staff       (20)     5750 2023-06-02 14:46:22.000000 liqa-1.2.1/liqa_src/testDAS.R
--rw-r--r--   0 wenli      (501) staff       (20)       38 2023-06-02 15:47:15.669849 liqa-1.2.1/setup.cfg
--rw-r--r--   0 wenli      (501) staff       (20)     1177 2023-06-02 15:47:03.000000 liqa-1.2.1/setup.py
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 05:36:21.147078 liqa-1.3.0/
+-rw-r--r--   0 wenli      (501) staff       (20)      693 2023-07-16 05:30:58.000000 liqa-1.3.0/LICENSE
+-rw-r--r--   0 wenli      (501) staff       (20)       25 2023-07-16 05:30:58.000000 liqa-1.3.0/MANIFEST.in
+-rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-07-16 05:36:21.146953 liqa-1.3.0/PKG-INFO
+-rw-r--r--   0 wenli      (501) staff       (20)     1743 2023-07-16 05:30:58.000000 liqa-1.3.0/README.md
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 05:36:21.145409 liqa-1.3.0/liqa.egg-info/
+-rw-r--r--   0 wenli      (501) staff       (20)     2195 2023-07-16 05:36:21.000000 liqa-1.3.0/liqa.egg-info/PKG-INFO
+-rw-r--r--   0 wenli      (501) staff       (20)      387 2023-07-16 05:36:21.000000 liqa-1.3.0/liqa.egg-info/SOURCES.txt
+-rw-r--r--   0 wenli      (501) staff       (20)        1 2023-07-16 05:36:21.000000 liqa-1.3.0/liqa.egg-info/dependency_links.txt
+-rw-r--r--   0 wenli      (501) staff       (20)       44 2023-07-16 05:36:21.000000 liqa-1.3.0/liqa.egg-info/entry_points.txt
+-rw-r--r--   0 wenli      (501) staff       (20)       16 2023-07-16 05:36:21.000000 liqa-1.3.0/liqa.egg-info/requires.txt
+-rw-r--r--   0 wenli      (501) staff       (20)        9 2023-07-16 05:36:21.000000 liqa-1.3.0/liqa.egg-info/top_level.txt
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-07-16 05:36:21.146770 liqa-1.3.0/liqa_src/
+-rw-r--r--   0 wenli      (501) staff       (20)     5381 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/PreProcess.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     6619 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/PreProcess_gtf.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     2302 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/group_process.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     4321 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/liqa.py
+-rw-r--r--   0 wenli      (501) staff       (20)     2949 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/my_functions.py
+-rw-r--r--   0 wenli      (501) staff       (20)    19896 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/noveliso.py
+-rw-r--r--   0 wenli      (501) staff       (20)    26418 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/quantify.py
+-rw-r--r--   0 wenli      (501) staff       (20)     5750 2023-07-16 05:30:58.000000 liqa-1.3.0/liqa_src/testDAS.R
+-rw-r--r--   0 wenli      (501) staff       (20)       38 2023-07-16 05:36:21.147112 liqa-1.3.0/setup.cfg
+-rw-r--r--   0 wenli      (501) staff       (20)     1179 2023-07-16 05:36:17.000000 liqa-1.3.0/setup.py
```

### Comparing `liqa-1.2.1/LICENSE` & `liqa-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/PKG-INFO` & `liqa-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liqa
-Version: 1.2.1
+Version: 1.3.0
 Summary: A statistical tool to quantify isoform-specific expression using long-read RNA-seq
 Home-page: https://github.com/WGLab/LIQA
 Author: Yu Hu
 Author-email: huyu999999@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `liqa-1.2.1/README.md` & `liqa-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/liqa.egg-info/PKG-INFO` & `liqa-1.3.0/liqa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liqa
-Version: 1.2.1
+Version: 1.3.0
 Summary: A statistical tool to quantify isoform-specific expression using long-read RNA-seq
 Home-page: https://github.com/WGLab/LIQA
 Author: Yu Hu
 Author-email: huyu999999@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `liqa-1.2.1/liqa_src/PreProcess.pl` & `liqa-1.3.0/liqa_src/PreProcess.pl`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/liqa_src/PreProcess_gtf.pl` & `liqa-1.3.0/liqa_src/PreProcess_gtf.pl`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/liqa_src/group_process.pl` & `liqa-1.3.0/liqa_src/group_process.pl`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/liqa_src/liqa.py` & `liqa-1.3.0/liqa_src/liqa.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,23 +36,27 @@
         elif (formatFile == "gtf"):
             myCommand = "perl " + fileAbsPath + "/PreProcess_gtf.pl -r " + refFile + " -o " + outFile
             os.system(myCommand)
         else:
             print("Please specify reference file format: gtf/ucsc")
 
     if task == "novel":
-        validArgList = ["-task", "-ref", "-bamlist", "-out"]
-        addAbsPath = [0, 1, 1, 3]
-        message = "liqa -task novel -ref <reference_file> -bamlist <list of bam file> -out <output_file>"
+        validArgList = ["-task", "-refgene", "-bam", "-out", "-num_cover", "-num_support_read"]
+        addAbsPath = [0, 1, 1, 3, 0, 0]
+        message = "liqa -task novel -refgene <refgene_file> -bam <bam_file> -out <output_file> -num_cover <# bp coverage> -num_support_read <# support reads>"
         inputs = my.parse_argument(validArgList, addAbsPath, message)
         refFile = inputs[1]
-        bamList = inputs[2]
+        bamFile = inputs[2]
         outFile = inputs[3]
+        misMatch = inputs[4]
+        weightF = inputs[5]
+
+        myCommand = "python " + fileAbsPath + "/noveliso.py -ref " + refFile + " -bam " +  bamFile + " -out " + outFile + " -num_cover " + misMatch + " -num_support_read " + weightF
 
-        myCommand = "perl " + fileAbsPath + "/detect.pl -r " + refFile + " -o " + outFile + " -b " + bamList
+        
         os.system(myCommand)
             
     if task == "quantify":
         validArgList = ["-task", "-refgene", "-bam", "-out", "-max_distance", "-f_weight"]
         addAbsPath = [0, 1, 1, 3, 0, 0]
         message = "liqa -task quantify -refgene <refgene_file> -bam <bam_file> -out <output_file> -max_distance <max distance> -f_weight <weight of F function>"
         inputs = my.parse_argument(validArgList, addAbsPath, message)
```

### Comparing `liqa-1.2.1/liqa_src/my_functions.py` & `liqa-1.3.0/liqa_src/my_functions.py`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/liqa_src/quantify.py` & `liqa-1.3.0/liqa_src/quantify.py`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/liqa_src/testDAS.R` & `liqa-1.3.0/liqa_src/testDAS.R`

 * *Files identical despite different names*

### Comparing `liqa-1.2.1/setup.py` & `liqa-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="liqa",
-    version="1.2.1",
+    version="1.3.0",
     author="Yu Hu",
     author_email="huyu999999@gmail.com",
     description="A statistical tool to quantify isoform-specific expression using long-read RNA-seq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WGLab/LIQA",
     license="MIT",
@@ -20,15 +20,15 @@
     ],
     install_requires=["pysam", "lifelines"],
     #python_requires='>=3.6',
     #packages=["liqa_src","liqa_bin"],
     #package_dir={"liqa_src":"liqa_src","liqa_bin":"liqa_src/liqa_bin"},
     packages=["liqa_src"],
     package_dir={"liqa_src":"liqa_src"},
-    scripts=["liqa_src/group_process.pl","liqa_src/testDAS.R", "liqa_src/PreProcess.pl", "liqa_src/PreProcess_gtf.pl", "liqa_src/detect.pl"],
+    scripts=["liqa_src/group_process.pl","liqa_src/testDAS.R", "liqa_src/PreProcess.pl", "liqa_src/PreProcess_gtf.pl", "liqa_src/noveliso.py"],
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "liqa=liqa_src.liqa:main",
         ]
     },
 )
```

