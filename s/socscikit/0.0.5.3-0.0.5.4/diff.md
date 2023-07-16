# Comparing `tmp/socscikit-0.0.5.3.tar.gz` & `tmp/socscikit-0.0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.5.3.tar", last modified: Sat Jul 15 23:03:23 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.4.tar", last modified: Sun Jul 16 06:48:36 2023, max compression
```

## Comparing `socscikit-0.0.5.3.tar` & `socscikit-0.0.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:23.750324 socscikit-0.0.5.3/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-15 23:03:23.750324 socscikit-0.0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.3/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 23:03:23.751320 socscikit-0.0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-07-15 23:03:20.000000 socscikit-0.0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:23.721283 socscikit-0.0.5.3/socscikit/
--rw-rw-rw-   0        0        0     1012 2023-07-15 22:53:25.000000 socscikit-0.0.5.3/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.3/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:23.710325 socscikit-0.0.5.3/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:23.747330 socscikit-0.0.5.3/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:23.749326 socscikit-0.0.5.3/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.3/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.3/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.3/socscikit/socialmedia.py
--rw-rw-rw-   0        0        0      136 2023-07-15 23:01:18.000000 socscikit-0.0.5.3/socscikit/test.py
--rw-rw-rw-   0        0        0     7458 2023-07-15 23:02:17.000000 socscikit-0.0.5.3/socscikit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:23.736282 socscikit-0.0.5.3/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-15 23:03:23.000000 socscikit-0.0.5.3/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-15 23:03:23.000000 socscikit-0.0.5.3/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 23:03:23.000000 socscikit-0.0.5.3/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-15 23:03:23.000000 socscikit-0.0.5.3/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 23:03:23.000000 socscikit-0.0.5.3/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.646345 socscikit-0.0.5.4/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      308 2023-07-16 06:43:38.000000 socscikit-0.0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-16 06:48:36.646345 socscikit-0.0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-16 06:48:36.651428 socscikit-0.0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-07-16 06:48:20.000000 socscikit-0.0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.567201 socscikit-0.0.5.4/socscikit/
+-rw-rw-rw-   0        0        0     1548 2023-07-16 06:45:34.000000 socscikit-0.0.5.4/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.4/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.551195 socscikit-0.0.5.4/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.615460 socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.644383 socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.4/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0      136 2023-07-15 23:01:18.000000 socscikit-0.0.5.4/socscikit/test.py
+-rw-rw-rw-   0        0        0     7570 2023-07-16 00:45:30.000000 socscikit-0.0.5.4/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:48:36.584206 socscikit-0.0.5.4/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 06:48:36.000000 socscikit-0.0.5.4/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.5.3/LICENSE.txt` & `socscikit-0.0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.3/setup.py` & `socscikit-0.0.5.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.5.3',      
+  version = '0.0.5.4',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.3.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.4.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
-          'conlp'
+          'conlp',
+          'spacy'
       ],
   include_package_data=True
 )
```

### Comparing `socscikit-0.0.5.3/socscikit/CompliSent.py` & `socscikit-0.0.5.4/socscikit/CompliSent.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,12 +15,22 @@
                 self.lex_dict = pickle.load(handle)
         
         elif idx == "VADER_v2014_mod": 
             file_path = os.path.join(self.script_dir, 'lexicon_dictionary', 'VADER', 'VADER_v2014_mod.pickle')
             with open(file_path, 'rb') as handle: 
                 self.lex_dict = pickle.load(handle)
                 
+        elif idx == "AFINN_v2015": 
+            file_path = os.path.join(self.script_dir, 'lexicon_dictionary', 'AFINN', 'AFINN_v2015.pickle')
+            with open(file_path, 'rb') as handle: 
+                self.lex_dict = pickle.load(handle)
+        
+        elif idx == "Aigents+_v2022": 
+            file_path = os.path.join(self.script_dir, 'lexicon_dictionary', 'Aigents', 'Aigents+_v2022.pickle')
+            with open(file_path, 'rb') as handle: 
+                self.lex_dict = pickle.load(handle)
+                
         return self.lex_dict
     
     def overview(self, dictionary:dict): 
         #dict:str = Consider if users simply come up with the lex_dict_idx
         return CS().summarise_lex_dict(dictionary)
```

### Comparing `socscikit-0.0.5.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.3/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.3/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.3/socscikit/socialmedia.py` & `socscikit-0.0.5.4/socscikit/socialmedia.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.3/socscikit/utils.py` & `socscikit-0.0.5.4/socscikit/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     def count_categorical_labels(self, dictionary):
         label_counts = Counter()
         multi_label_counts = Counter()
 
         for sublist in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
+            transient=True
         ):
             if isinstance(sublist, list):
                 if all(isinstance(item, str) for item in sublist):
                     labels = sublist
                     label_counts.update(labels)
 
                     combinations_set = set(
@@ -47,14 +48,15 @@
     def count_discrete_labels(self, dictionary):
         label_counts = {}
         multi_label_counts = {}
 
         for value_list in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
+            transient=True
         ):
             unique_labels = set(value_list)
 
             for label in unique_labels:
                 if label in label_counts:
                     label_counts[label] += 1
                 else:
@@ -82,14 +84,15 @@
     def count_cont_variables(self, dictionary):
         value_range = [min(dictionary.values()), max(dictionary.values())]
         neg, pos, neu = [], [], []
 
         for value in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
+            transient=True
         ):
             if value < 0:
                 neg.append(value)
             elif value > 0:
                 pos.append(value)
             else:
                 neu.append(value)
@@ -169,14 +172,15 @@
         }
         granular_dict = {}
         misc = []
 
         for key in track(
             lexicon_dictionary.keys(),
             description="Extracting Summary Insights from Sentiment Lexicons",
+            transient=True
         ):
             doc = self.spacy_nlp(key)
             for token in doc:
                 pos_tags.append(token.tag_)
 
         for element in pos_tags:
             if element in granular_dict:
```

### Comparing `socscikit-0.0.5.3/socscikit.egg-info/SOURCES.txt` & `socscikit-0.0.5.4/socscikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

