# Comparing `tmp/clustutils4r-0.0.7.tar.gz` & `tmp/clustutils4r-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-0.0.7.tar", last modified: Sun Jul 16 08:26:00 2023, max compression
+gzip compressed data, was "clustutils4r-0.0.8.tar", last modified: Sun Jul 16 08:29:46 2023, max compression
```

## Comparing `clustutils4r-0.0.7.tar` & `clustutils4r-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.7/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5299 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4667 2023-07-16 08:23:55.000000 clustutils4r-0.0.7/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-16 08:25:16.000000 clustutils4r-0.0.7/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-16 08:25:24.000000 clustutils4r-0.0.7/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.7/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    28396 2023-07-16 08:18:23.000000 clustutils4r-0.0.7/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/src/clustutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5299 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.8/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5423 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4791 2023-07-16 08:28:10.000000 clustutils4r-0.0.8/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-16 08:29:32.000000 clustutils4r-0.0.8/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-16 08:29:24.000000 clustutils4r-0.0.8/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.8/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    28396 2023-07-16 08:18:23.000000 clustutils4r-0.0.8/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/src/clustutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5423 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-0.0.7/LICENSE` & `clustutils4r-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.7/PKG-INFO` & `clustutils4r-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.7
+Version: 0.0.8
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -68,14 +68,18 @@
                            random_state=0)
 
 ## Setup model
 model = KMeans()
 model_params = {'init':'k-means++', 'n_init':1}
 n_clusters_param_name='n_clusters'
 
+# model = GaussianMixture()
+# model_params = {'covariance_type':'full', 'n_init':1}
+# n_clusters_param_name='n_components'
+
 ## Run the evaluation
 range_clusters = list(range(3,10+1))
 labelled_datapoints, \
    nongt_metrics, \
       gt_metrics = eval_clustering(X=X, gt_labels=y,
                                     model=model, model_params=model_params, n_clusters_param_name=n_clusters_param_name,
                                     num_clusters=range_clusters, num_runs=10,
```

### Comparing `clustutils4r-0.0.7/README.md` & `clustutils4r-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,18 @@
                            random_state=0)
 
 ## Setup model
 model = KMeans()
 model_params = {'init':'k-means++', 'n_init':1}
 n_clusters_param_name='n_clusters'
 
+# model = GaussianMixture()
+# model_params = {'covariance_type':'full', 'n_init':1}
+# n_clusters_param_name='n_components'
+
 ## Run the evaluation
 range_clusters = list(range(3,10+1))
 labelled_datapoints, \
    nongt_metrics, \
       gt_metrics = eval_clustering(X=X, gt_labels=y,
                                     model=model, model_params=model_params, n_clusters_param_name=n_clusters_param_name,
                                     num_clusters=range_clusters, num_runs=10,
```

### Comparing `clustutils4r-0.0.7/pyproject.toml` & `clustutils4r-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-0.0.7/setup.py` & `clustutils4r-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clustutils4r", # Replace with your own username
-    version="0.0.7",
+    version="0.0.8",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn utilities for clustering.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clustutils4r",
     project_urls={
```

### Comparing `clustutils4r-0.0.7/src/clustutils4r/eval_clustering.py` & `clustutils4r-0.0.8/src/clustutils4r/eval_clustering.py`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.7/src/clustutils4r.egg-info/PKG-INFO` & `clustutils4r-0.0.8/src/clustutils4r.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.7
+Version: 0.0.8
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -68,14 +68,18 @@
                            random_state=0)
 
 ## Setup model
 model = KMeans()
 model_params = {'init':'k-means++', 'n_init':1}
 n_clusters_param_name='n_clusters'
 
+# model = GaussianMixture()
+# model_params = {'covariance_type':'full', 'n_init':1}
+# n_clusters_param_name='n_components'
+
 ## Run the evaluation
 range_clusters = list(range(3,10+1))
 labelled_datapoints, \
    nongt_metrics, \
       gt_metrics = eval_clustering(X=X, gt_labels=y,
                                     model=model, model_params=model_params, n_clusters_param_name=n_clusters_param_name,
                                     num_clusters=range_clusters, num_runs=10,
```

