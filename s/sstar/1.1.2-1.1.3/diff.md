# Comparing `tmp/sstar-1.1.2.tar.gz` & `tmp/sstar-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sstar-1.1.2.tar", last modified: Wed Aug  3 20:37:27 2022, max compression
+gzip compressed data, was "sstar-1.1.3.tar", last modified: Sun Jul 16 21:06:28 2023, max compression
```

## Comparing `sstar-1.1.2.tar` & `sstar-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxr-x   0 cuda      (1000) cuda      (1000)        0 2022-08-03 20:37:27.637353 sstar-1.1.2/
--rw-rw-r--   0 cuda      (1000) cuda      (1000)    11357 2022-08-03 18:45:25.000000 sstar-1.1.2/LICENSE
--rw-rw-r--   0 cuda      (1000) cuda      (1000)     1321 2022-08-03 20:37:27.637353 sstar-1.1.2/PKG-INFO
--rw-rw-r--   0 cuda      (1000) cuda      (1000)      835 2022-08-03 18:45:25.000000 sstar-1.1.2/README.md
--rw-rw-r--   0 cuda      (1000) cuda      (1000)       38 2022-08-03 20:37:27.637353 sstar-1.1.2/setup.cfg
--rw-rw-r--   0 cuda      (1000) cuda      (1000)     1095 2022-08-03 19:07:01.000000 sstar-1.1.2/setup.py
-drwxrwxr-x   0 cuda      (1000) cuda      (1000)        0 2022-08-03 20:37:27.637353 sstar-1.1.2/sstar/
--rw-rw-r--   0 cuda      (1000) cuda      (1000)        0 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/__init__.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)    11117 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/__main__.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)     8955 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/cal_match_rate.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)    10744 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/cal_s_star.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)     8054 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/cal_threshold.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)        0 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/conftest.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)    12716 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/get_quantile.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)     2921 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/get_tract.py
--rw-rw-r--   0 cuda      (1000) cuda      (1000)    17002 2022-08-03 18:45:25.000000 sstar-1.1.2/sstar/utils.py
-drwxrwxr-x   0 cuda      (1000) cuda      (1000)        0 2022-08-03 20:37:27.637353 sstar-1.1.2/sstar.egg-info/
--rw-rw-r--   0 cuda      (1000) cuda      (1000)     1321 2022-08-03 20:37:27.000000 sstar-1.1.2/sstar.egg-info/PKG-INFO
--rw-rw-r--   0 cuda      (1000) cuda      (1000)      379 2022-08-03 20:37:27.000000 sstar-1.1.2/sstar.egg-info/SOURCES.txt
--rw-rw-r--   0 cuda      (1000) cuda      (1000)        1 2022-08-03 20:37:27.000000 sstar-1.1.2/sstar.egg-info/dependency_links.txt
--rw-rw-r--   0 cuda      (1000) cuda      (1000)       46 2022-08-03 20:37:27.000000 sstar-1.1.2/sstar.egg-info/entry_points.txt
--rw-rw-r--   0 cuda      (1000) cuda      (1000)       43 2022-08-03 20:37:27.000000 sstar-1.1.2/sstar.egg-info/requires.txt
--rw-rw-r--   0 cuda      (1000) cuda      (1000)        6 2022-08-03 20:37:27.000000 sstar-1.1.2/sstar.egg-info/top_level.txt
+drwxr-sr-x   0 huangxin (11326) admixlab (10011)        0 2023-07-16 21:06:28.501165 sstar-1.1.3/
+-rw-r--r--   0 huangxin (11326) admixlab (10011)    11357 2023-07-16 20:41:35.000000 sstar-1.1.3/LICENSE
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     1321 2023-07-16 21:06:28.000000 sstar-1.1.3/PKG-INFO
+-rw-r--r--   0 huangxin (11326) admixlab (10011)      835 2023-07-16 20:41:35.000000 sstar-1.1.3/README.md
+-rw-r--r--   0 huangxin (11326) admixlab (10011)       38 2023-07-16 21:06:28.000000 sstar-1.1.3/setup.cfg
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     1095 2023-07-16 20:51:40.000000 sstar-1.1.3/setup.py
+drwxr-sr-x   0 huangxin (11326) admixlab (10011)        0 2023-07-16 21:06:28.400164 sstar-1.1.3/sstar/
+-rw-r--r--   0 huangxin (11326) admixlab (10011)        0 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/__init__.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)    11117 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/__main__.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     8955 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/cal_match_rate.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)    10744 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/cal_s_star.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     8030 2023-07-16 20:58:51.000000 sstar-1.1.3/sstar/cal_threshold.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)        0 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/conftest.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)    12716 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/get_quantile.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     2921 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/get_tract.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)    17002 2023-07-16 20:41:36.000000 sstar-1.1.3/sstar/utils.py
+drwxr-sr-x   0 huangxin (11326) admixlab (10011)        0 2023-07-16 21:06:28.429164 sstar-1.1.3/sstar.egg-info/
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     1321 2023-07-16 21:06:28.000000 sstar-1.1.3/sstar.egg-info/PKG-INFO
+-rw-r--r--   0 huangxin (11326) admixlab (10011)      532 2023-07-16 21:06:28.000000 sstar-1.1.3/sstar.egg-info/SOURCES.txt
+-rw-r--r--   0 huangxin (11326) admixlab (10011)        1 2023-07-16 21:06:28.000000 sstar-1.1.3/sstar.egg-info/dependency_links.txt
+-rw-r--r--   0 huangxin (11326) admixlab (10011)       46 2023-07-16 21:06:28.000000 sstar-1.1.3/sstar.egg-info/entry_points.txt
+-rw-r--r--   0 huangxin (11326) admixlab (10011)       43 2023-07-16 21:06:28.000000 sstar-1.1.3/sstar.egg-info/requires.txt
+-rw-r--r--   0 huangxin (11326) admixlab (10011)        6 2023-07-16 21:06:28.000000 sstar-1.1.3/sstar.egg-info/top_level.txt
+drwxr-sr-x   0 huangxin (11326) admixlab (10011)        0 2023-07-16 21:06:28.494165 sstar-1.1.3/tests/
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     1536 2023-07-16 20:41:36.000000 sstar-1.1.3/tests/test_cal_match_rate.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     1508 2023-07-16 20:41:36.000000 sstar-1.1.3/tests/test_cal_s_star.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     1444 2023-07-16 20:41:36.000000 sstar-1.1.3/tests/test_cal_threshold.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     1361 2023-07-16 20:41:36.000000 sstar-1.1.3/tests/test_get_quantile.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     2449 2023-07-16 20:41:36.000000 sstar-1.1.3/tests/test_get_tract.py
+-rw-r--r--   0 huangxin (11326) admixlab (10011)     7001 2023-07-16 20:41:36.000000 sstar-1.1.3/tests/test_utils.py
```

### Comparing `sstar-1.1.2/LICENSE` & `sstar-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/PKG-INFO` & `sstar-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sstar
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python package for detecting archaic introgression from population genetic data with S*
 Home-page: https://github.com/xin-huang/sstar
 Author: Xin Huang
 Author-email: xinhuang.res@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `sstar-1.1.2/README.md` & `sstar-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/setup.py` & `sstar-1.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="sstar",
-    version="1.1.2",
+    version="1.1.3",
     description="A Python package for detecting archaic introgression from population genetic data with S*",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/xin-huang/sstar",
     author="Xin Huang",
     author_email="xinhuang.res@gmail.com",
     license="Apache-2.0",
```

### Comparing `sstar-1.1.2/sstar/__main__.py` & `sstar-1.1.3/sstar/__main__.py`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/sstar/cal_match_rate.py` & `sstar-1.1.3/sstar/cal_match_rate.py`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/sstar/cal_s_star.py` & `sstar-1.1.3/sstar/cal_s_star.py`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/sstar/cal_threshold.py` & `sstar-1.1.3/sstar/cal_threshold.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             score = float(meta_data[s][i][4])
             null_score = round(thresholds[s][i], 6)
             if score > null_score: sig = 'True'
             else: sig = 'False'
 
             line = "\t".join(meta_data[s][i])
             line += "\t" + str(null_score)
-            line += "\t" + str(10**data[s]['lr'][i])
+            line += "\t" + str(data[s]['lr'][i])
             line += "\t" + str(data[s]['q'][i])
             line += "\t" + sig
 
             res.append(line)
 
     return res
 
@@ -164,18 +164,18 @@
                 win_end = element[2]
                 sample = element[3]
                 score = element[4]
                 total_snp_num = element[5]
                 if fit_lr:
                     if recomb_map != None: 
                         key = chr_name+":"+win_start+"-"+win_end
-                        if key in recomb_map.keys(): local_recomb_rate = np.log10(recomb_map[key])
+                        if key in recomb_map.keys(): local_recomb_rate = recomb_map[key]
                         else: continue
                     else:
-                        local_recomb_rate = np.log10(recomb_rate)
+                        local_recomb_rate = recomb_rate
                 else: local_recomb_rate = np.nan
 
                 if sample not in data.keys(): 
                     data[sample] = dict()
                     data[sample]['snps'] = list()
                     data[sample]['lr'] = list()
                     data[sample]['q'] = list()
```

### Comparing `sstar-1.1.2/sstar/get_quantile.py` & `sstar-1.1.3/sstar/get_quantile.py`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/sstar/get_tract.py` & `sstar-1.1.3/sstar/get_tract.py`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/sstar/utils.py` & `sstar-1.1.3/sstar/utils.py`

 * *Files identical despite different names*

### Comparing `sstar-1.1.2/sstar.egg-info/PKG-INFO` & `sstar-1.1.3/sstar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sstar
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python package for detecting archaic introgression from population genetic data with S*
 Home-page: https://github.com/xin-huang/sstar
 Author: Xin Huang
 Author-email: xinhuang.res@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

