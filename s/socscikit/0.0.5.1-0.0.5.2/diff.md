# Comparing `tmp/socscikit-0.0.5.1.tar.gz` & `tmp/socscikit-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.5.1.tar", last modified: Sat Jul 15 22:54:15 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.2.tar", last modified: Sat Jul 15 22:59:49 2023, max compression
```

## Comparing `socscikit-0.0.5.1.tar` & `socscikit-0.0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.795493 socscikit-0.0.5.1/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-15 22:54:15.795493 socscikit-0.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.1/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 22:54:15.799492 socscikit-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-07-15 22:53:59.000000 socscikit-0.0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.763492 socscikit-0.0.5.1/socscikit/
--rw-rw-rw-   0        0        0     1012 2023-07-15 22:53:25.000000 socscikit-0.0.5.1/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.1/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.751493 socscikit-0.0.5.1/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.791492 socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.794493 socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.1/socscikit/socialmedia.py
--rw-rw-rw-   0        0        0      136 2023-07-15 22:49:33.000000 socscikit-0.0.5.1/socscikit/test.py
--rw-rw-rw-   0        0        0     7454 2023-07-15 22:41:43.000000 socscikit-0.0.5.1/socscikit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.781491 socscikit-0.0.5.1/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 22:59:49.263678 socscikit-0.0.5.2/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-15 22:59:49.264689 socscikit-0.0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 22:59:49.265679 socscikit-0.0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-07-15 22:59:31.000000 socscikit-0.0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:59:49.229163 socscikit-0.0.5.2/socscikit/
+-rw-rw-rw-   0        0        0     1012 2023-07-15 22:53:25.000000 socscikit-0.0.5.2/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.2/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:59:49.218110 socscikit-0.0.5.2/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-15 22:59:49.259679 socscikit-0.0.5.2/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.2/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.2/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-15 22:59:49.262678 socscikit-0.0.5.2/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.2/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.2/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.2/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0      136 2023-07-15 22:56:09.000000 socscikit-0.0.5.2/socscikit/test.py
+-rw-rw-rw-   0        0        0     7448 2023-07-15 22:58:00.000000 socscikit-0.0.5.2/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:59:49.250680 socscikit-0.0.5.2/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-15 22:59:48.000000 socscikit-0.0.5.2/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-15 22:59:49.000000 socscikit-0.0.5.2/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 22:59:48.000000 socscikit-0.0.5.2/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-15 22:59:48.000000 socscikit-0.0.5.2/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 22:59:48.000000 socscikit-0.0.5.2/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.5.1/LICENSE.txt` & `socscikit-0.0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.1/setup.py` & `socscikit-0.0.5.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.5.1',      
+  version = '0.0.5.2',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.1.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.2.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp'
       ],
   include_package_data=True
```

### Comparing `socscikit-0.0.5.1/socscikit/CompliSent.py` & `socscikit-0.0.5.2/socscikit/CompliSent.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5.2/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5.2/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5.2/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5.2/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.1/socscikit/socialmedia.py` & `socscikit-0.0.5.2/socscikit/socialmedia.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.1/socscikit/utils.py` & `socscikit-0.0.5.2/socscikit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rich.progress import track
 from rich import print as pprint
 import itertools
-from itertools import combinations
+from itertools import combinations, chain
 import statistics
-from collections import defaultdict, Counter
+from collections import Counter
 import spacy
 
 
 class CS:
     def __init__(self):
         self.spacy_nlp = spacy.load(
             "en_core_web_sm"
```

### Comparing `socscikit-0.0.5.1/socscikit.egg-info/SOURCES.txt` & `socscikit-0.0.5.2/socscikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

