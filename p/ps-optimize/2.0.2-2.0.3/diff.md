# Comparing `tmp/ps-optimize-2.0.2.tar.gz` & `tmp/ps-optimize-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ps-optimize-2.0.2.tar", last modified: Sun Jul 16 06:42:39 2023, max compression
+gzip compressed data, was "ps-optimize-2.0.3.tar", last modified: Sun Jul 16 06:53:11 2023, max compression
```

## Comparing `ps-optimize-2.0.2.tar` & `ps-optimize-2.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:42:39.915151 ps-optimize-2.0.2/
--rw-rw-rw-   0        0        0      925 2023-07-16 06:42:39.914152 ps-optimize-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-07-15 14:14:14.000000 ps-optimize-2.0.2/README.md
--rw-rw-rw-   0        0        0      639 2023-07-16 06:42:16.000000 ps-optimize-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 06:42:39.915151 ps-optimize-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 06:42:39.849150 ps-optimize-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 06:42:39.900149 ps-optimize-2.0.2/src/ps_opt/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:29:29.000000 ps-optimize-2.0.2/src/ps_opt/__init__.py
--rw-rw-rw-   0        0        0      574 2023-07-15 13:55:46.000000 ps-optimize-2.0.2/src/ps_opt/_base.py
--rw-rw-rw-   0        0        0      159 2023-07-15 13:55:46.000000 ps-optimize-2.0.2/src/ps_opt/_error.py
--rw-rw-rw-   0        0        0    13575 2023-07-15 14:58:48.000000 ps-optimize-2.0.2/src/ps_opt/_feature_selection_process.py
--rw-rw-rw-   0        0        0    19807 2023-07-15 14:56:30.000000 ps-optimize-2.0.2/src/ps_opt/_hyperparameters_tuning_process.py
--rw-rw-rw-   0        0        0     6337 2023-07-15 14:58:55.000000 ps-optimize-2.0.2/src/ps_opt/feature_selection.py
--rw-rw-rw-   0        0        0    17852 2023-07-15 14:56:36.000000 ps-optimize-2.0.2/src/ps_opt/hyperparameters_tuning.py
--rw-rw-rw-   0        0        0     3716 2023-06-20 14:43:23.000000 ps-optimize-2.0.2/src/ps_opt/search_space_characteristics.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:42:39.913150 ps-optimize-2.0.2/src/ps_optimize.egg-info/
--rw-rw-rw-   0        0        0      925 2023-07-16 06:42:39.000000 ps-optimize-2.0.2/src/ps_optimize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-16 06:42:39.000000 ps-optimize-2.0.2/src/ps_optimize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 06:42:39.000000 ps-optimize-2.0.2/src/ps_optimize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 06:42:39.000000 ps-optimize-2.0.2/src/ps_optimize.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.549479 ps-optimize-2.0.3/
+-rw-rw-rw-   0        0        0     4341 2023-07-16 06:53:11.548479 ps-optimize-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3827 2023-07-16 06:50:41.000000 ps-optimize-2.0.3/README.md
+-rw-rw-rw-   0        0        0      639 2023-07-16 06:52:58.000000 ps-optimize-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 06:53:11.549479 ps-optimize-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.523480 ps-optimize-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.533479 ps-optimize-2.0.3/src/ps_opt/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:29:29.000000 ps-optimize-2.0.3/src/ps_opt/__init__.py
+-rw-rw-rw-   0        0        0      574 2023-07-15 13:55:46.000000 ps-optimize-2.0.3/src/ps_opt/_base.py
+-rw-rw-rw-   0        0        0      159 2023-07-15 13:55:46.000000 ps-optimize-2.0.3/src/ps_opt/_error.py
+-rw-rw-rw-   0        0        0    13575 2023-07-15 14:58:48.000000 ps-optimize-2.0.3/src/ps_opt/_feature_selection_process.py
+-rw-rw-rw-   0        0        0    19807 2023-07-15 14:56:30.000000 ps-optimize-2.0.3/src/ps_opt/_hyperparameters_tuning_process.py
+-rw-rw-rw-   0        0        0     6337 2023-07-15 14:58:55.000000 ps-optimize-2.0.3/src/ps_opt/feature_selection.py
+-rw-rw-rw-   0        0        0    17852 2023-07-15 14:56:36.000000 ps-optimize-2.0.3/src/ps_opt/hyperparameters_tuning.py
+-rw-rw-rw-   0        0        0     3716 2023-06-20 14:43:23.000000 ps-optimize-2.0.3/src/ps_opt/search_space_characteristics.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:53:11.547479 ps-optimize-2.0.3/src/ps_optimize.egg-info/
+-rw-rw-rw-   0        0        0     4341 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 06:53:11.000000 ps-optimize-2.0.3/src/ps_optimize.egg-info/top_level.txt
```

### Comparing `ps-optimize-2.0.2/pyproject.toml` & `ps-optimize-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ps-optimize"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Yuen Shing Yan Hindy", email="yuenshingyan@gmail.com" },
 ]
 description = "PSO meet hyperparameter tuning."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ps-optimize-2.0.2/src/ps_opt/_base.py` & `ps-optimize-2.0.3/src/ps_opt/_base.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.2/src/ps_opt/_feature_selection_process.py` & `ps-optimize-2.0.3/src/ps_opt/_feature_selection_process.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.2/src/ps_opt/_hyperparameters_tuning_process.py` & `ps-optimize-2.0.3/src/ps_opt/_hyperparameters_tuning_process.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.2/src/ps_opt/feature_selection.py` & `ps-optimize-2.0.3/src/ps_opt/feature_selection.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.2/src/ps_opt/hyperparameters_tuning.py` & `ps-optimize-2.0.3/src/ps_opt/hyperparameters_tuning.py`

 * *Files identical despite different names*

### Comparing `ps-optimize-2.0.2/src/ps_opt/search_space_characteristics.py` & `ps-optimize-2.0.3/src/ps_opt/search_space_characteristics.py`

 * *Files identical despite different names*

