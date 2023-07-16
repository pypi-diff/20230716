# Comparing `tmp/neuropop-1.0.tar.gz` & `tmp/neuropop-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuropop-1.0.tar", last modified: Fri Jul 14 13:07:44 2023, max compression
+gzip compressed data, was "neuropop-1.0.1.tar", last modified: Sun Jul 16 02:07:19 2023, max compression
```

## Comparing `neuropop-1.0.tar` & `neuropop-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.874613 neuropop-1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.874613 neuropop-1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-14 13:07:28.000000 neuropop-1.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 13:07:28.000000 neuropop-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-14 13:07:44.878613 neuropop-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-14 13:07:28.000000 neuropop-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-14 13:07:28.000000 neuropop-1.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    87394 2023-07-14 13:07:28.000000 neuropop-1.0/figures/SVCA.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    70690 2023-07-14 13:07:28.000000 neuropop-1.0/figures/cvPCA.PNG
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 13:07:28.000000 neuropop-1.0/figures/figsfromrefs
--rw-r--r--   0 runner    (1001) docker     (123)   380397 2023-07-14 13:07:28.000000 neuropop-1.0/figures/nn_prediction.PNG
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/neuropop/
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/future_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/linear_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/nn_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/peer_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/split_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/neuropop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:07:44.878613 neuropop-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 13:07:28.000000 neuropop-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-14 13:07:28.000000 neuropop-1.0/tests/make_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-14 13:07:28.000000 neuropop-1.0/tests/test_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-14 13:07:28.000000 neuropop-1.0/tests/test_linpred.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-14 13:07:28.000000 neuropop-1.0/tests/test_nnpred.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-14 13:07:28.000000 neuropop-1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:19.749177 neuropop-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:19.745177 neuropop-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:19.745177 neuropop-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-16 02:07:02.000000 neuropop-1.0.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 02:07:02.000000 neuropop-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-16 02:07:19.749177 neuropop-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-16 02:07:02.000000 neuropop-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-16 02:07:02.000000 neuropop-1.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:19.745177 neuropop-1.0.1/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    87394 2023-07-16 02:07:02.000000 neuropop-1.0.1/figures/SVCA.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    70690 2023-07-16 02:07:02.000000 neuropop-1.0.1/figures/cvPCA.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 02:07:02.000000 neuropop-1.0.1/figures/figsfromrefs
+-rw-r--r--   0 runner    (1001) docker     (123)   380397 2023-07-16 02:07:02.000000 neuropop-1.0.1/figures/nn_prediction.PNG
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:19.749177 neuropop-1.0.1/neuropop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/future_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/linear_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/nn_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/peer_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/split_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-16 02:07:02.000000 neuropop-1.0.1/neuropop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:19.749177 neuropop-1.0.1/neuropop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-16 02:07:19.000000 neuropop-1.0.1/neuropop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-16 02:07:19.000000 neuropop-1.0.1/neuropop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:07:19.000000 neuropop-1.0.1/neuropop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-16 02:07:19.000000 neuropop-1.0.1/neuropop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 02:07:19.000000 neuropop-1.0.1/neuropop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 02:07:19.749177 neuropop-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-16 02:07:02.000000 neuropop-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:07:19.749177 neuropop-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-16 02:07:02.000000 neuropop-1.0.1/tests/make_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-16 02:07:02.000000 neuropop-1.0.1/tests/test_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-16 02:07:02.000000 neuropop-1.0.1/tests/test_linpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-16 02:07:02.000000 neuropop-1.0.1/tests/test_nnpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-16 02:07:02.000000 neuropop-1.0.1/tox.ini
```

### Comparing `neuropop-1.0/.github/workflows/test_and_deploy.yml` & `neuropop-1.0.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/LICENSE` & `neuropop-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/PKG-INFO` & `neuropop-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropop
-Version: 1.0
+Version: 1.0.1
 Summary: analysis tools for neural population recordings
 Home-page: https://github.com/MouseLand/neuropop
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: stringerc@janelia.hhmi.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `neuropop-1.0/README.md` & `neuropop-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/conftest.py` & `neuropop-1.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/figures/SVCA.PNG` & `neuropop-1.0.1/figures/SVCA.PNG`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/figures/cvPCA.PNG` & `neuropop-1.0.1/figures/cvPCA.PNG`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/figures/nn_prediction.PNG` & `neuropop-1.0.1/figures/nn_prediction.PNG`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/dimensionality.py` & `neuropop-1.0.1/neuropop/dimensionality.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/filtering.py` & `neuropop-1.0.1/neuropop/filtering.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/future_prediction.py` & `neuropop-1.0.1/neuropop/future_prediction.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/linear_prediction.py` & `neuropop-1.0.1/neuropop/linear_prediction.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/nn_prediction.py` & `neuropop-1.0.1/neuropop/nn_prediction.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/peer_prediction.py` & `neuropop-1.0.1/neuropop/peer_prediction.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/split_data.py` & `neuropop-1.0.1/neuropop/split_data.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop/utils.py` & `neuropop-1.0.1/neuropop/utils.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/neuropop.egg-info/PKG-INFO` & `neuropop-1.0.1/neuropop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropop
-Version: 1.0
+Version: 1.0.1
 Summary: analysis tools for neural population recordings
 Home-page: https://github.com/MouseLand/neuropop
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: stringerc@janelia.hhmi.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `neuropop-1.0/neuropop.egg-info/SOURCES.txt` & `neuropop-1.0.1/neuropop.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
 figures/SVCA.PNG
 figures/cvPCA.PNG
 figures/figsfromrefs
 figures/nn_prediction.PNG
+neuropop/__init__.py
 neuropop/dimensionality.py
 neuropop/filtering.py
 neuropop/future_prediction.py
 neuropop/linear_prediction.py
 neuropop/nn_prediction.py
 neuropop/peer_prediction.py
 neuropop/split_data.py
```

### Comparing `neuropop-1.0/setup.py` & `neuropop-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/tests/make_test.ipynb` & `neuropop-1.0.1/tests/make_test.ipynb`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/tests/test_linpred.py` & `neuropop-1.0.1/tests/test_linpred.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/tests/test_nnpred.py` & `neuropop-1.0.1/tests/test_nnpred.py`

 * *Files identical despite different names*

### Comparing `neuropop-1.0/tox.ini` & `neuropop-1.0.1/tox.ini`

 * *Files identical despite different names*

