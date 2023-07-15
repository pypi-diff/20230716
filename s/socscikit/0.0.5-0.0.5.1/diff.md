# Comparing `tmp/socscikit-0.0.5.tar.gz` & `tmp/socscikit-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.5.tar", last modified: Sat Jul 15 22:44:19 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.1.tar", last modified: Sat Jul 15 22:54:15 2023, max compression
```

## Comparing `socscikit-0.0.5.tar` & `socscikit-0.0.5.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 22:44:19.029989 socscikit-0.0.5/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      404 2023-07-15 22:44:19.029989 socscikit-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 22:44:19.033989 socscikit-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-07-15 22:12:46.000000 socscikit-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:44:18.960427 socscikit-0.0.5/socscikit/
--rw-rw-rw-   0        0        0     1010 2023-07-15 22:43:56.000000 socscikit-0.0.5/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:44:18.946426 socscikit-0.0.5/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-15 22:44:19.014989 socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-15 22:44:19.028989 socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5/socscikit/socialmedia.py
--rw-rw-rw-   0        0        0     7454 2023-07-15 22:41:43.000000 socscikit-0.0.5/socscikit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:44:18.987522 socscikit-0.0.5/socscikit.egg-info/
--rw-rw-rw-   0        0        0      404 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 22:44:18.000000 socscikit-0.0.5/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.795493 socscikit-0.0.5.1/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-15 22:54:15.795493 socscikit-0.0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 22:54:15.799492 socscikit-0.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-07-15 22:53:59.000000 socscikit-0.0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.763492 socscikit-0.0.5.1/socscikit/
+-rw-rw-rw-   0        0        0     1012 2023-07-15 22:53:25.000000 socscikit-0.0.5.1/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.1/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.751493 socscikit-0.0.5.1/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.791492 socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.794493 socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.1/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0      136 2023-07-15 22:49:33.000000 socscikit-0.0.5.1/socscikit/test.py
+-rw-rw-rw-   0        0        0     7454 2023-07-15 22:41:43.000000 socscikit-0.0.5.1/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:54:15.781491 socscikit-0.0.5.1/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 22:54:15.000000 socscikit-0.0.5.1/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.5/LICENSE.txt` & `socscikit-0.0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5/setup.py` & `socscikit-0.0.5.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.5',      
+  version = '0.0.5.1',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.1.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp'
       ],
   include_package_data=True
```

### Comparing `socscikit-0.0.5/socscikit/CompliSent.py` & `socscikit-0.0.5.1/socscikit/CompliSent.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
             with open(file_path, 'rb') as handle: 
                 self.lex_dict = pickle.load(handle)
                 
         return self.lex_dict
     
     def overview(self, dictionary:dict): 
         #dict:str = Consider if users simply come up with the lex_dict_idx
-        return CS.summarise_lex_dict(dictionary)
+        return CS().summarise_lex_dict(dictionary)
```

### Comparing `socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5.1/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5.1/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5/socscikit/socialmedia.py` & `socscikit-0.0.5.1/socscikit/socialmedia.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5/socscikit/utils.py` & `socscikit-0.0.5.1/socscikit/utils.py`

 * *Files identical despite different names*

