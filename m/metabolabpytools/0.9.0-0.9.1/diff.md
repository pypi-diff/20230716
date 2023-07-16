# Comparing `tmp/metabolabpytools-0.9.0.tar.gz` & `tmp/metabolabpytools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolabpytools-0.9.0.tar", last modified: Sun Jul 16 14:37:51 2023, max compression
+gzip compressed data, was "metabolabpytools-0.9.1.tar", last modified: Sun Jul 16 20:10:32 2023, max compression
```

## Comparing `metabolabpytools-0.9.0.tar` & `metabolabpytools-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:37:51.193739 metabolabpytools-0.9.0/
--rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-07-11 16:28:03.000000 metabolabpytools-0.9.0/LICENSE
--rw-r--r--   0 ludwigc    (501) staff       (20)       78 2023-07-11 16:28:03.000000 metabolabpytools-0.9.0/MANIFEST.in
--rw-r--r--   0 ludwigc    (501) staff       (20)     3709 2023-07-16 14:37:51.193607 metabolabpytools-0.9.0/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)       67 2023-07-11 16:28:03.000000 metabolabpytools-0.9.0/README.md
--rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-07-11 16:28:03.000000 metabolabpytools-0.9.0/README.rst
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:37:51.192399 metabolabpytools-0.9.0/metabolabpytools/
--rw-r--r--   0 ludwigc    (501) staff       (20)      153 2023-07-16 14:35:19.000000 metabolabpytools-0.9.0/metabolabpytools/__init__.py
--rw-r--r--   0 ludwigc    (501) staff       (20)     1893 2023-07-11 16:28:03.000000 metabolabpytools-0.9.0/metabolabpytools/analysis.py
--rw-r--r--   0 ludwigc    (501) staff       (20)    25753 2023-07-16 14:32:50.000000 metabolabpytools-0.9.0/metabolabpytools/isotopomerAnalysis.py
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:37:51.193406 metabolabpytools-0.9.0/metabolabpytools.egg-info/
--rw-r--r--   0 ludwigc    (501) staff       (20)     3709 2023-07-16 14:37:51.000000 metabolabpytools-0.9.0/metabolabpytools.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)      362 2023-07-16 14:37:51.000000 metabolabpytools-0.9.0/metabolabpytools.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-07-16 14:37:51.000000 metabolabpytools-0.9.0/metabolabpytools.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-07-16 14:37:51.000000 metabolabpytools-0.9.0/metabolabpytools.egg-info/requires.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       17 2023-07-16 14:37:51.000000 metabolabpytools-0.9.0/metabolabpytools.egg-info/top_level.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-07-11 16:28:03.000000 metabolabpytools-0.9.0/requirements.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-07-16 14:37:51.193779 metabolabpytools-0.9.0/setup.cfg
--rw-r--r--   0 ludwigc    (501) staff       (20)     1507 2023-07-11 16:28:03.000000 metabolabpytools-0.9.0/setup.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:10:32.725096 metabolabpytools-0.9.1/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:10.000000 metabolabpytools-0.9.1/LICENSE
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       78 2023-06-29 16:08:10.000000 metabolabpytools-0.9.1/MANIFEST.in
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3709 2023-07-16 20:10:32.724915 metabolabpytools-0.9.1/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       67 2023-06-29 16:08:10.000000 metabolabpytools-0.9.1/README.md
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:10.000000 metabolabpytools-0.9.1/README.rst
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:10:32.723792 metabolabpytools-0.9.1/metabolabpytools/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      153 2023-07-16 20:10:25.000000 metabolabpytools-0.9.1/metabolabpytools/__init__.py
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     1893 2023-06-29 16:08:10.000000 metabolabpytools-0.9.1/metabolabpytools/analysis.py
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079    25753 2023-07-16 14:50:21.000000 metabolabpytools-0.9.1/metabolabpytools/isotopomerAnalysis.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:10:32.724742 metabolabpytools-0.9.1/metabolabpytools.egg-info/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3709 2023-07-16 20:10:32.000000 metabolabpytools-0.9.1/metabolabpytools.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      362 2023-07-16 20:10:32.000000 metabolabpytools-0.9.1/metabolabpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-16 20:10:32.000000 metabolabpytools-0.9.1/metabolabpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-07-16 20:10:32.000000 metabolabpytools-0.9.1/metabolabpytools.egg-info/requires.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       17 2023-07-16 20:10:32.000000 metabolabpytools-0.9.1/metabolabpytools.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-06-29 16:08:10.000000 metabolabpytools-0.9.1/requirements.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-16 20:10:32.725132 metabolabpytools-0.9.1/setup.cfg
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     1507 2023-06-29 16:08:10.000000 metabolabpytools-0.9.1/setup.py
```

### Comparing `metabolabpytools-0.9.0/LICENSE` & `metabolabpytools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.0/PKG-INFO` & `metabolabpytools-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.9.0/README.rst` & `metabolabpytools-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.0/metabolabpytools/analysis.py` & `metabolabpytools-0.9.1/metabolabpytools/analysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.0/metabolabpytools/isotopomerAnalysis.py` & `metabolabpytools-0.9.1/metabolabpytools/isotopomerAnalysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.0/metabolabpytools.egg-info/PKG-INFO` & `metabolabpytools-0.9.1/metabolabpytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.9.0/setup.py` & `metabolabpytools-0.9.1/setup.py`

 * *Files identical despite different names*

