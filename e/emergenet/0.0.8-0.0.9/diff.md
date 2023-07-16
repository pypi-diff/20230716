# Comparing `tmp/emergenet-0.0.8.tar.gz` & `tmp/emergenet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emergenet-0.0.8.tar", last modified: Fri Sep  2 03:36:22 2022, max compression
+gzip compressed data, was "emergenet-0.0.9.tar", last modified: Fri Sep  2 03:39:13 2022, max compression
```

## Comparing `emergenet-0.0.8.tar` & `emergenet-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-09-02 03:36:22.886460 emergenet-0.0.8/
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     2031 2022-09-01 22:28:22.000000 emergenet-0.0.8/LICENSE
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     2025 2022-08-20 15:58:07.000000 emergenet-0.0.8/LICENSE.md
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      171 2022-09-01 22:35:18.000000 emergenet-0.0.8/MANIFEST.in
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1530 2022-09-02 03:36:22.886460 emergenet-0.0.8/PKG-INFO
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      673 2022-09-02 03:25:43.000000 emergenet-0.0.8/README.rst
-drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-09-02 03:36:22.885460 emergenet-0.0.8/emergenet/
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        0 2022-09-01 22:00:10.000000 emergenet-0.0.8/emergenet/__init__.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     7183 2022-09-01 22:00:10.000000 emergenet-0.0.8/emergenet/emergenet.py
-drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-09-02 03:36:22.886460 emergenet-0.0.8/emergenet.egg-info/
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1530 2022-09-02 03:36:22.000000 emergenet-0.0.8/emergenet.egg-info/PKG-INFO
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      270 2022-09-02 03:36:22.000000 emergenet-0.0.8/emergenet.egg-info/SOURCES.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        1 2022-09-02 03:36:22.000000 emergenet-0.0.8/emergenet.egg-info/dependency_links.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       54 2022-09-02 03:36:22.000000 emergenet-0.0.8/emergenet.egg-info/requires.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       10 2022-09-02 03:36:22.000000 emergenet-0.0.8/emergenet.egg-info/top_level.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       38 2022-09-02 03:36:22.886460 emergenet-0.0.8/setup.cfg
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1737 2022-09-01 22:33:51.000000 emergenet-0.0.8/setup.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       22 2022-09-02 03:27:43.000000 emergenet-0.0.8/version.py
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-09-02 03:39:13.959955 emergenet-0.0.9/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     2031 2022-09-01 22:28:22.000000 emergenet-0.0.9/LICENSE
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     2025 2022-08-20 15:58:07.000000 emergenet-0.0.9/LICENSE.md
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      171 2022-09-01 22:35:18.000000 emergenet-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1530 2022-09-02 03:39:13.959955 emergenet-0.0.9/PKG-INFO
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      673 2022-09-02 03:25:43.000000 emergenet-0.0.9/README.rst
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-09-02 03:39:13.958955 emergenet-0.0.9/emergenet/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        0 2022-09-01 22:00:10.000000 emergenet-0.0.9/emergenet/__init__.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     7183 2022-09-01 22:00:10.000000 emergenet-0.0.9/emergenet/emergenet.py
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-09-02 03:39:13.959955 emergenet-0.0.9/emergenet.egg-info/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1530 2022-09-02 03:39:13.000000 emergenet-0.0.9/emergenet.egg-info/PKG-INFO
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      270 2022-09-02 03:39:13.000000 emergenet-0.0.9/emergenet.egg-info/SOURCES.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        1 2022-09-02 03:39:13.000000 emergenet-0.0.9/emergenet.egg-info/dependency_links.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       54 2022-09-02 03:39:13.000000 emergenet-0.0.9/emergenet.egg-info/requires.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       10 2022-09-02 03:39:13.000000 emergenet-0.0.9/emergenet.egg-info/top_level.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       38 2022-09-02 03:39:13.959955 emergenet-0.0.9/setup.cfg
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1737 2022-09-01 22:33:51.000000 emergenet-0.0.9/setup.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       22 2022-09-02 03:36:30.000000 emergenet-0.0.9/version.py
```

### Comparing `emergenet-0.0.8/LICENSE` & `emergenet-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `emergenet-0.0.8/LICENSE.md` & `emergenet-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `emergenet-0.0.8/PKG-INFO` & `emergenet-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: emergenet
-Version: 0.0.8
+Version: 0.0.9
 Summary: Superfast Risk Estimation of Emerging Pathogens
 Home-page: https://github.com/zeroknowledgediscovery/emergenet
 Author: zed.uchicago.edu
 Author-email: ishanu@uchicago.edu
 License: LICENSE
-Download-URL: https://github.com/zeroknowledgediscovery/emergenet/archive/0.0.8.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/emergenet/archive/0.0.9.tar.gz
 Keywords: computational biology,decision trees,machine learning,emerging pathogens
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `emergenet-0.0.8/README.rst` & `emergenet-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `emergenet-0.0.8/emergenet/emergenet.py` & `emergenet-0.0.9/emergenet/emergenet.py`

 * *Files identical despite different names*

### Comparing `emergenet-0.0.8/emergenet.egg-info/PKG-INFO` & `emergenet-0.0.9/emergenet.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: emergenet
-Version: 0.0.8
+Version: 0.0.9
 Summary: Superfast Risk Estimation of Emerging Pathogens
 Home-page: https://github.com/zeroknowledgediscovery/emergenet
 Author: zed.uchicago.edu
 Author-email: ishanu@uchicago.edu
 License: LICENSE
-Download-URL: https://github.com/zeroknowledgediscovery/emergenet/archive/0.0.8.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/emergenet/archive/0.0.9.tar.gz
 Keywords: computational biology,decision trees,machine learning,emerging pathogens
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `emergenet-0.0.8/setup.py` & `emergenet-0.0.9/setup.py`

 * *Files identical despite different names*

