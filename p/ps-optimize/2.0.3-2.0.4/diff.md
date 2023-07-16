# Comparing `tmp/ps-optimize-2.0.3.tar.gz` & `tmp/ps-optimize-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ps-optimize-2.0.3.tar", last modified: Sun Jul 16 06:53:11 2023, max compression
+gzip compressed data, was "ps-optimize-2.0.4.tar", last modified: Sun Jul 16 09:49:04 2023, max compression
```

## Comparing `ps-optimize-2.0.3.tar` & `ps-optimize-2.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.549479 ps-optimize-2.0.3/
--rw-rw-rw-   0        0        0     4341 2023-07-16 06:53:11.548479 ps-optimize-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3827 2023-07-16 06:50:41.000000 ps-optimize-2.0.3/README.md
--rw-rw-rw-   0        0        0      639 2023-07-16 06:52:58.000000 ps-optimize-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 06:53:11.549479 ps-optimize-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.523480 ps-optimize-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.533479 ps-optimize-2.0.3/src/ps_opt/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:29:29.000000 ps-optimize-2.0.3/src/ps_opt/__init__.py
--rw-rw-rw-   0        0        0      574 2023-07-15 13:55:46.000000 ps-optimize-2.0.3/src/ps_opt/_base.py
--rw-rw-rw-   0        0        0      159 2023-07-15 13:55:46.000000 ps-optimize-2.0.3/src/ps_opt/_error.py
--rw-rw-rw-   0        0        0    13575 2023-07-15 14:58:48.000000 ps-optimize-2.0.3/src/ps_opt/_feature_selection_process.py
--rw-rw-rw-   0        0        0    19807 2023-07-15 14:56:30.000000 ps-optimize-2.0.3/src/ps_opt/_hyperparameters_tuning_process.py
--rw-rw-rw-   0        0        0     6337 2023-07-15 14:58:55.000000 ps-optimize-2.0.3/src/ps_opt/feature_selection.py
--rw-rw-rw-   0        0        0    17852 2023-07-15 14:56:36.000000 ps-optimize-2.0.3/src/ps_opt/hyperparameters_tuning.py
--rw-rw-rw-   0        0        0     3716 2023-06-20 14:43:23.000000 ps-optimize-2.0.3/src/ps_opt/search_space_characteristics.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.547479 ps-optimize-2.0.3/src/ps_optimize.egg-info/
--rw-rw-rw-   0        0        0     4341 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 09:49:04.865257 ps-optimize-2.0.4/
+-rw-rw-rw-   0        0        0     4063 2023-07-16 09:49:04.864257 ps-optimize-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2023-07-16 09:48:30.000000 ps-optimize-2.0.4/README.md
+-rw-rw-rw-   0        0        0      639 2023-07-16 09:48:30.000000 ps-optimize-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 09:49:04.865257 ps-optimize-2.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 09:49:04.799258 ps-optimize-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 09:49:04.850260 ps-optimize-2.0.4/src/ps_opt/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:29:29.000000 ps-optimize-2.0.4/src/ps_opt/__init__.py
+-rw-rw-rw-   0        0        0      574 2023-07-15 13:55:46.000000 ps-optimize-2.0.4/src/ps_opt/_base.py
+-rw-rw-rw-   0        0        0      159 2023-07-15 13:55:46.000000 ps-optimize-2.0.4/src/ps_opt/_error.py
+-rw-rw-rw-   0        0        0    13575 2023-07-15 14:58:48.000000 ps-optimize-2.0.4/src/ps_opt/_feature_selection_process.py
+-rw-rw-rw-   0        0        0    19807 2023-07-15 14:56:30.000000 ps-optimize-2.0.4/src/ps_opt/_hyperparameters_tuning_process.py
+-rw-rw-rw-   0        0        0     6337 2023-07-15 14:58:55.000000 ps-optimize-2.0.4/src/ps_opt/feature_selection.py
+-rw-rw-rw-   0        0        0    17852 2023-07-15 14:56:36.000000 ps-optimize-2.0.4/src/ps_opt/hyperparameters_tuning.py
+-rw-rw-rw-   0        0        0     3716 2023-06-20 14:43:23.000000 ps-optimize-2.0.4/src/ps_opt/search_space_characteristics.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:49:04.863257 ps-optimize-2.0.4/src/ps_optimize.egg-info/
+-rw-rw-rw-   0        0        0     4063 2023-07-16 09:49:04.000000 ps-optimize-2.0.4/src/ps_optimize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-16 09:49:04.000000 ps-optimize-2.0.4/src/ps_optimize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 09:49:04.000000 ps-optimize-2.0.4/src/ps_optimize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 09:49:04.000000 ps-optimize-2.0.4/src/ps_optimize.egg-info/top_level.txt
```

### Comparing `ps-optimize-2.0.3/PKG-INFO` & `ps-optimize-2.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ps-optimize
-Version: 2.0.3
+Version: 2.0.4
 Summary: PSO meet hyperparameter tuning.
 Author-email: Yuen Shing Yan Hindy <yuenshingyan@gmail.com>
 Project-URL: Homepage, https://github.com/yuenshingyan/ps-opt
 Project-URL: Bug Tracker, https://github.com/yuenshingyan/ps-opt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -84,21 +84,14 @@
     from sklearn.linear_model import LogisticRegression
     
     
     X, y = make_classification()
     X = pd.DataFrame(X)
     y = pd.Series(y)
     
-    search_space = {
-        "penalty": Categorical("l1", "l2", "elasticnet", None),
-        "max_iter": Integer(10, 20, "exponential"),
-        "tol": Real(.0001, .1, "uniform"),
-        "solver": Categorical('lbfgs', 'liblinear', 'newton-cg', 'sag', 'saga')
-    }
-    
     psocv = ParticleSwarmFeatureSelectionCV(
         n_particles=30,
         estimator=LogisticRegression,
         cv=5,
         scoring="accuracy",
         max_iter=10,
         n_jobs=-1,
```

### Comparing `ps-optimize-2.0.3/README.md` & `ps-optimize-2.0.4/src/ps_optimize.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: ps-optimize
+Version: 2.0.4
+Summary: PSO meet hyperparameter tuning.
+Author-email: Yuen Shing Yan Hindy <yuenshingyan@gmail.com>
+Project-URL: Homepage, https://github.com/yuenshingyan/ps-opt
+Project-URL: Bug Tracker, https://github.com/yuenshingyan/ps-opt/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # ps-opt
 This Python package provides a tool for hyperparameter tuning and feature selection in machine learning models using Particle Swarm Optimization (PSO) techniques. The package includes a vanilla PSO for feature selection, a vanilla PSO for hyperparameter tuning, and two different PSO variants for machine learning hyperparameter tuning.
 
 ## Features
 
 Vanilla PSO for Feature Selection: This feature uses the standard PSO algorithm to select the most optimal features for a given machine learning model. The algorithm works by searching the feature space and identifying a subset of features that maximizes the performance of the model.
 
@@ -71,21 +84,14 @@
     from sklearn.linear_model import LogisticRegression
     
     
     X, y = make_classification()
     X = pd.DataFrame(X)
     y = pd.Series(y)
     
-    search_space = {
-        "penalty": Categorical("l1", "l2", "elasticnet", None),
-        "max_iter": Integer(10, 20, "exponential"),
-        "tol": Real(.0001, .1, "uniform"),
-        "solver": Categorical('lbfgs', 'liblinear', 'newton-cg', 'sag', 'saga')
-    }
-    
     psocv = ParticleSwarmFeatureSelectionCV(
         n_particles=30,
         estimator=LogisticRegression,
         cv=5,
         scoring="accuracy",
         max_iter=10,
         n_jobs=-1,
```

### Comparing `ps-optimize-2.0.3/pyproject.toml` & `ps-optimize-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ps-optimize"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
   { name="Yuen Shing Yan Hindy", email="yuenshingyan@gmail.com" },
 ]
 description = "PSO meet hyperparameter tuning."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ps-optimize-2.0.3/src/ps_opt/_base.py` & `ps-optimize-2.0.4/src/ps_opt/_base.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.3/src/ps_opt/_feature_selection_process.py` & `ps-optimize-2.0.4/src/ps_opt/_feature_selection_process.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.3/src/ps_opt/_hyperparameters_tuning_process.py` & `ps-optimize-2.0.4/src/ps_opt/_hyperparameters_tuning_process.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.3/src/ps_opt/feature_selection.py` & `ps-optimize-2.0.4/src/ps_opt/feature_selection.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.3/src/ps_opt/hyperparameters_tuning.py` & `ps-optimize-2.0.4/src/ps_opt/hyperparameters_tuning.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.3/src/ps_opt/search_space_characteristics.py` & `ps-optimize-2.0.4/src/ps_opt/search_space_characteristics.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.3/src/ps_optimize.egg-info/PKG-INFO` & `ps-optimize-2.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: ps-optimize
-Version: 2.0.3
-Summary: PSO meet hyperparameter tuning.
-Author-email: Yuen Shing Yan Hindy <yuenshingyan@gmail.com>
-Project-URL: Homepage, https://github.com/yuenshingyan/ps-opt
-Project-URL: Bug Tracker, https://github.com/yuenshingyan/ps-opt/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # ps-opt
 This Python package provides a tool for hyperparameter tuning and feature selection in machine learning models using Particle Swarm Optimization (PSO) techniques. The package includes a vanilla PSO for feature selection, a vanilla PSO for hyperparameter tuning, and two different PSO variants for machine learning hyperparameter tuning.
 
 ## Features
 
 Vanilla PSO for Feature Selection: This feature uses the standard PSO algorithm to select the most optimal features for a given machine learning model. The algorithm works by searching the feature space and identifying a subset of features that maximizes the performance of the model.
 
@@ -84,21 +71,14 @@
     from sklearn.linear_model import LogisticRegression
     
     
     X, y = make_classification()
     X = pd.DataFrame(X)
     y = pd.Series(y)
     
-    search_space = {
-        "penalty": Categorical("l1", "l2", "elasticnet", None),
-        "max_iter": Integer(10, 20, "exponential"),
-        "tol": Real(.0001, .1, "uniform"),
-        "solver": Categorical('lbfgs', 'liblinear', 'newton-cg', 'sag', 'saga')
-    }
-    
     psocv = ParticleSwarmFeatureSelectionCV(
         n_particles=30,
         estimator=LogisticRegression,
         cv=5,
         scoring="accuracy",
         max_iter=10,
         n_jobs=-1,
```

