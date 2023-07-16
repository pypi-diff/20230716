# Comparing `tmp/socscikit-0.0.5.4.tar.gz` & `tmp/socscikit-0.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.5.4.tar", last modified: Sun Jul 16 06:48:36 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.5.tar", last modified: Sun Jul 16 06:59:17 2023, max compression
```

## Comparing `socscikit-0.0.5.4.tar` & `socscikit-0.0.5.5.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.646345 socscikit-0.0.5.4/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.4/LICENSE.txt
--rw-rw-rw-   0        0        0      308 2023-07-16 06:43:38.000000 socscikit-0.0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-16 06:48:36.646345 socscikit-0.0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.4/README.md
--rw-rw-rw-   0        0        0       86 2023-07-16 06:48:36.651428 socscikit-0.0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-07-16 06:48:20.000000 socscikit-0.0.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.567201 socscikit-0.0.5.4/socscikit/
--rw-rw-rw-   0        0        0     1548 2023-07-16 06:45:34.000000 socscikit-0.0.5.4/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.4/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.551195 socscikit-0.0.5.4/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.615460 socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.644383 socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.4/socscikit/socialmedia.py
--rw-rw-rw-   0        0        0      136 2023-07-15 23:01:18.000000 socscikit-0.0.5.4/socscikit/test.py
--rw-rw-rw-   0        0        0     7570 2023-07-16 00:45:30.000000 socscikit-0.0.5.4/socscikit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.584206 socscikit-0.0.5.4/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:17.005854 socscikit-0.0.5.5/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      308 2023-07-16 06:56:47.000000 socscikit-0.0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-16 06:59:17.005854 socscikit-0.0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-16 06:59:17.006854 socscikit-0.0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-07-16 06:59:06.000000 socscikit-0.0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:16.975854 socscikit-0.0.5.5/socscikit/
+-rw-rw-rw-   0        0        0     1548 2023-07-16 06:45:34.000000 socscikit-0.0.5.5/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.5/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:16.964855 socscikit-0.0.5.5/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:16.990855 socscikit-0.0.5.5/socscikit/lexicon_dictionary/AFINN/
+-rw-rw-rw-   0        0        0    50662 2023-07-16 06:40:36.000000 socscikit-0.0.5.5/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:16.991853 socscikit-0.0.5.5/socscikit/lexicon_dictionary/Aigents/
+-rw-rw-rw-   0        0        0   247057 2023-07-16 06:38:52.000000 socscikit-0.0.5.5/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:17.001854 socscikit-0.0.5.5/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:17.004855 socscikit-0.0.5.5/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.5/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.5/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.5/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0      136 2023-07-15 23:01:18.000000 socscikit-0.0.5.5/socscikit/test.py
+-rw-rw-rw-   0        0        0     7570 2023-07-16 00:45:30.000000 socscikit-0.0.5.5/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:16.989855 socscikit-0.0.5.5/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-16 06:59:16.000000 socscikit-0.0.5.5/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      649 2023-07-16 06:59:16.000000 socscikit-0.0.5.5/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:59:16.000000 socscikit-0.0.5.5/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-16 06:59:16.000000 socscikit-0.0.5.5/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 06:59:16.000000 socscikit-0.0.5.5/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.5.4/LICENSE.txt` & `socscikit-0.0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.4/setup.py` & `socscikit-0.0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.5.4',      
+  version = '0.0.5.5',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.4.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.5.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp',
           'spacy'
       ],
```

### Comparing `socscikit-0.0.5.4/socscikit/CompliSent.py` & `socscikit-0.0.5.5/socscikit/CompliSent.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5.5/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5.5/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.4/socscikit/socialmedia.py` & `socscikit-0.0.5.5/socscikit/socialmedia.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.4/socscikit/utils.py` & `socscikit-0.0.5.5/socscikit/utils.py`

 * *Files identical despite different names*

