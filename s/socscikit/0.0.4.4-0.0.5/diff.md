# Comparing `tmp/socscikit-0.0.4.4.tar.gz` & `tmp/socscikit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.4.4.tar", last modified: Fri Jul 14 23:11:17 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.tar", last modified: Sat Jul 15 22:44:19 2023, max compression
```

## Comparing `socscikit-0.0.4.4.tar` & `socscikit-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.294418 socscikit-0.0.4.4/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-14 23:11:17.294418 socscikit-0.0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.4.4/README.md
--rw-rw-rw-   0        0        0       86 2023-07-14 23:11:17.297412 socscikit-0.0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-07-14 23:10:59.000000 socscikit-0.0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.220833 socscikit-0.0.4.4/socscikit/
--rw-rw-rw-   0        0        0      803 2023-07-14 23:07:08.000000 socscikit-0.0.4.4/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.4.4/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.200467 socscikit-0.0.4.4/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.288413 socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.293418 socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.4.4/socscikit/socialmedia.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.272414 socscikit-0.0.4.4/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-07-14 23:11:17.000000 socscikit-0.0.4.4/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 22:44:19.029989 socscikit-0.0.5/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      404 2023-07-15 22:44:19.029989 socscikit-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 22:44:19.033989 socscikit-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-07-15 22:12:46.000000 socscikit-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:44:18.960427 socscikit-0.0.5/socscikit/
+-rw-rw-rw-   0        0        0     1010 2023-07-15 22:43:56.000000 socscikit-0.0.5/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:44:18.946426 socscikit-0.0.5/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-15 22:44:19.014989 socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-15 22:44:19.028989 socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0     7454 2023-07-15 22:41:43.000000 socscikit-0.0.5/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:44:18.987522 socscikit-0.0.5/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.4.4/LICENSE.txt` & `socscikit-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.4/setup.py` & `socscikit-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.4.4',      
+  version = '0.0.5',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.4.4.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp'
       ],
   include_package_data=True
```

### Comparing `socscikit-0.0.4.4/socscikit/CompliSent.py` & `socscikit-0.0.5/socscikit/CompliSent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import os 
 import pickle 
+from socscikit.utils import CS 
 
 class lexicon:
     def __init__(self): 
         self.script_dir = os.path.dirname(os.path.abspath(__file__))
         self.lex_dict = None 
     
-    def dictionary(self, idx:str):
+    def load_dict(self, idx:str):
         
         if idx == 'MASTER_v2022':   
             file_path = os.path.join(self.script_dir, 'lexicon_dictionary', 'MASTER', 'MASTER_v2022.pickle')           
             with open(file_path, 'rb') as handle: 
                 self.lex_dict = pickle.load(handle)
         
         elif idx == "VADER_v2014_mod": 
             file_path = os.path.join(self.script_dir, 'lexicon_dictionary', 'VADER', 'VADER_v2014_mod.pickle')
             with open(file_path, 'rb') as handle: 
                 self.lex_dict = pickle.load(handle)
                 
-        return self.lex_dict
+        return self.lex_dict
+    
+    def overview(self, dictionary:dict): 
+        #dict:str = Consider if users simply come up with the lex_dict_idx
+        return CS.summarise_lex_dict(dictionary)
```

### Comparing `socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.4/socscikit/socialmedia.py` & `socscikit-0.0.5/socscikit/socialmedia.py`

 * *Files identical despite different names*

