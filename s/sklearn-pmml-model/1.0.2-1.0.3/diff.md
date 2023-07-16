# Comparing `tmp/sklearn-pmml-model-1.0.2.tar.gz` & `tmp/sklearn-pmml-model-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn-pmml-model-1.0.2.tar", last modified: Tue Apr 25 21:06:37 2023, max compression
+gzip compressed data, was "sklearn-pmml-model-1.0.3.tar", last modified: Sun Jul 16 09:52:16 2023, max compression
```

## Comparing `sklearn-pmml-model-1.0.2.tar` & `sklearn-pmml-model-1.0.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.712983 sklearn-pmml-model-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-04-25 21:06:37.712983 sklearn-pmml-model-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:06:37.712983 sklearn-pmml-model-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.696981 sklearn-pmml-model-1.0.2/sklearn_pmml_model/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.700981 sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1126680 2023-04-25 21:06:32.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/_gradient_boosting.c
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/_gradient_boosting.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/gb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.700981 sklearn-pmml-model-1.0.2/sklearn_pmml_model/linear_model/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/linear_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/linear_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/linear_model/implementations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.700981 sklearn-pmml-model-1.0.2/sklearn_pmml_model/naive_bayes/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/naive_bayes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/naive_bayes/implementations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.700981 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neighbors/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neighbors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neighbors/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neighbors/_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.700981 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neural_network/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/neural_network/_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.704982 sklearn-pmml-model-1.0.2/sklearn_pmml_model/svm/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/svm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/svm/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/svm/_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.708982 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   685970 2023-04-25 21:06:33.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_criterion.c
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_criterion.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    46203 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_criterion.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   970487 2023-04-25 21:06:33.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_splitter.c
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_splitter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    73174 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_splitter.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1222081 2023-04-25 21:06:34.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_tree.c
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    48921 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_tree.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   683994 2023-04-25 21:06:35.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   659064 2023-04-25 21:06:36.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/quad_tree.c
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/quad_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    25744 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/quad_tree.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.696981 sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-04-25 21:06:37.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 21:06:37.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:06:37.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:06:37.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 21:06:37.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 21:06:37.000000 sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:37.708982 sklearn-pmml-model-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-25 21:06:23.000000 sklearn-pmml-model-1.0.2/tests/test_datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.918948 sklearn-pmml-model-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-16 09:52:16.918948 sklearn-pmml-model-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 09:52:16.918948 sklearn-pmml-model-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.894947 sklearn-pmml-model-1.0.3/sklearn_pmml_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.902947 sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1129090 2023-07-16 09:52:11.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/_gradient_boosting.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/_gradient_boosting.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/gb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.902947 sklearn-pmml-model-1.0.3/sklearn_pmml_model/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/linear_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/linear_model/implementations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.902947 sklearn-pmml-model-1.0.3/sklearn_pmml_model/naive_bayes/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/naive_bayes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/naive_bayes/implementations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.906947 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neighbors/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neighbors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neighbors/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neighbors/_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.906947 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neural_network/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/neural_network/_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.906947 sklearn-pmml-model-1.0.3/sklearn_pmml_model/svm/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/svm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/svm/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/svm/_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.918948 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   687362 2023-07-16 09:52:12.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_criterion.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_criterion.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    46203 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_criterion.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   972006 2023-07-16 09:52:13.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_splitter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_splitter.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    73174 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_splitter.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1223582 2023-07-16 09:52:14.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_tree.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    48922 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_tree.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   686062 2023-07-16 09:52:14.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   661240 2023-07-16 09:52:15.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/quad_tree.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/quad_tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    25744 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/quad_tree.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.898947 sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-16 09:52:16.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-16 09:52:16.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:52:16.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:52:16.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-16 09:52:16.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 09:52:16.000000 sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:16.918948 sklearn-pmml-model-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-16 09:52:03.000000 sklearn-pmml-model-1.0.3/tests/test_datatypes.py
```

### Comparing `sklearn-pmml-model-1.0.2/LICENSE` & `sklearn-pmml-model-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/PKG-INFO` & `sklearn-pmml-model-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: sklearn-pmml-model
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library to parse PMML models into Scikit-learn estimators.
 Home-page: https://github.com/iamDecode/sklearn-pmml-model
 Author: Dennis Collaris
 Author-email: d.collaris@me.com
 License: BSD-2-Clause
 Description: <img src="https://user-images.githubusercontent.com/1223300/41346080-c2c910a0-6f05-11e8-89e9-71a72bb9543f.png" width="300">
         
         # sklearn-pmml-model
         
         [![PyPI version](https://badge.fury.io/py/sklearn-pmml-model.svg)](https://badge.fury.io/py/sklearn-pmml-model)
         [![codecov](https://codecov.io/gh/iamDecode/sklearn-pmml-model/branch/master/graph/badge.svg?token=CGbbgziGwn)](https://codecov.io/gh/iamDecode/sklearn-pmml-model)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/iamDecode/sklearn-pmml-model.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/iamDecode/sklearn-pmml-model/context:python)
         [![CircleCI](https://circleci.com/gh/iamDecode/sklearn-pmml-model.svg?style=shield)](https://circleci.com/gh/iamDecode/sklearn-pmml-model)
         [![ReadTheDocs](https://readthedocs.org/projects/sklearn-pmml-model/badge/?version=latest&style=flat)](https://sklearn-pmml-model.readthedocs.io/en/latest/)
         
         A library to effortlessly import models trained on different platforms and with programming languages into scikit-learn in Python. First export your model to [PMML](http://dmg.org/pmml/v4-3/GeneralStructure.html) (widely supported). Next, load the exported PMML file with this library, and use the class as any other scikit-learn estimator.
         
         
         ## Installation
```

### Comparing `sklearn-pmml-model-1.0.2/README.md` & `sklearn-pmml-model-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 <img src="https://user-images.githubusercontent.com/1223300/41346080-c2c910a0-6f05-11e8-89e9-71a72bb9543f.png" width="300">
 
 # sklearn-pmml-model
 
 [![PyPI version](https://badge.fury.io/py/sklearn-pmml-model.svg)](https://badge.fury.io/py/sklearn-pmml-model)
 [![codecov](https://codecov.io/gh/iamDecode/sklearn-pmml-model/branch/master/graph/badge.svg?token=CGbbgziGwn)](https://codecov.io/gh/iamDecode/sklearn-pmml-model)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/iamDecode/sklearn-pmml-model.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/iamDecode/sklearn-pmml-model/context:python)
 [![CircleCI](https://circleci.com/gh/iamDecode/sklearn-pmml-model.svg?style=shield)](https://circleci.com/gh/iamDecode/sklearn-pmml-model)
 [![ReadTheDocs](https://readthedocs.org/projects/sklearn-pmml-model/badge/?version=latest&style=flat)](https://sklearn-pmml-model.readthedocs.io/en/latest/)
 
 A library to effortlessly import models trained on different platforms and with programming languages into scikit-learn in Python. First export your model to [PMML](http://dmg.org/pmml/v4-3/GeneralStructure.html) (widely supported). Next, load the exported PMML file with this library, and use the class as any other scikit-learn estimator.
 
 
 ## Installation
```

### Comparing `sklearn-pmml-model-1.0.2/setup.py` & `sklearn-pmml-model-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/base.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/base.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/datatypes.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/datatypes.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/_gradient_boosting.c` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/_gradient_boosting.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O2"
         ],
         "include_dirs": [
             ".",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sklearn_pmml_model.ensemble._gradient_boosting",
         "sources": [
             "sklearn_pmml_model/ensemble/_gradient_boosting.pyx"
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,18 +103,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +394,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +471,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1125,195 +1131,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1617,42 +1623,42 @@
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree;
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3002,14 +3008,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
@@ -3038,30 +3061,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -3286,18 +3309,18 @@
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
 static PyObject *__pyx_memoryview_is_slice(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_obj); /* proto*/
@@ -6899,15 +6922,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_rand);
   __Pyx_XDECREF((PyObject *)__pyx_v_sample_mask);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6916,29 +6939,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6949,15 +6972,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6966,29 +6989,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6999,15 +7022,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7016,29 +7039,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7049,15 +7072,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7066,29 +7089,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7099,15 +7122,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7116,29 +7139,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7149,212 +7172,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7370,15 +7393,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7386,53 +7409,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -7440,30 +7463,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7478,15 +7501,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7502,15 +7525,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7518,53 +7541,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -7572,30 +7595,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7610,15 +7633,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7634,15 +7657,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7650,53 +7673,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -7704,30 +7727,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7742,176 +7765,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -15254,15 +15277,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -20981,15 +21004,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -21144,15 +21167,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -21166,15 +21189,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -21266,15 +21289,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -21297,15 +21320,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -21530,15 +21553,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -21550,15 +21573,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -21679,15 +21702,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"_partial_dependence_tree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_18sklearn_pmml_model_8ensemble_18_gradient_boosting_7_partial_dependence_tree, METH_VARARGS|METH_KEYWORDS, __pyx_doc_18sklearn_pmml_model_8ensemble_18_gradient_boosting_6_partial_dependence_tree},
   {0, 0, 0, 0}
@@ -21911,26 +21934,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -22248,14 +22271,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -22372,132 +22400,77 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(4, 54, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(4, 54, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree)) __PYX_ERR(4, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(5, 141, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(5, 141, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_Stack*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack)) __PYX_ERR(5, 141, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(5, 170, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(5, 170, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_PriorityHeap*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap)) __PYX_ERR(5, 170, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(5, 193, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(5, 193, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue)) __PYX_ERR(5, 193, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(5, 213, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(5, 213, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator)) __PYX_ERR(5, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._criterion"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "Criterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion) __PYX_ERR(6, 23, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "Criterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion) __PYX_ERR(6, 23, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_Criterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_Criterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_Criterion)) __PYX_ERR(6, 23, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "ClassificationCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion) __PYX_ERR(6, 71, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "ClassificationCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion) __PYX_ERR(6, 71, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion)) __PYX_ERR(6, 71, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "RegressionCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion) __PYX_ERR(6, 77, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "RegressionCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion) __PYX_ERR(6, 77, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion)) __PYX_ERR(6, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._splitter"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._splitter", "Splitter", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter) __PYX_ERR(7, 28, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._splitter", "Splitter", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter) __PYX_ERR(7, 28, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_9_splitter_Splitter = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_Splitter*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_9_splitter_Splitter)) __PYX_ERR(7, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._tree", "CategoryCacheMgr", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr) __PYX_ERR(8, 30, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._tree", "CategoryCacheMgr", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr) __PYX_ERR(8, 30, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr)) __PYX_ERR(8, 30, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_5_tree_Tree = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._tree", "Tree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_Tree) __PYX_ERR(8, 39, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_5_tree_Tree = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._tree", "Tree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_Tree) __PYX_ERR(8, 39, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_5_tree_Tree = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_5_tree_Tree*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_Tree->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_5_tree_Tree)) __PYX_ERR(8, 39, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_5_tree_TreeBuilder = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._tree", "TreeBuilder", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_TreeBuilder) __PYX_ERR(8, 89, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_5_tree_TreeBuilder = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._tree", "TreeBuilder", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_TreeBuilder) __PYX_ERR(8, 89, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_5_tree_TreeBuilder = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_5_tree_TreeBuilder*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_5_tree_TreeBuilder->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_5_tree_TreeBuilder)) __PYX_ERR(8, 89, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -22510,15 +22483,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_36(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -22530,28 +22503,28 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "goes_left", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_goes_left, "int (__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SplitValue, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "goes_left", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_goes_left, "int (__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SplitValue, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -25634,18 +25607,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -25691,22 +25664,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -26825,15 +26798,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27021,15 +26994,15 @@
                         } else if (8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT) {
                             return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27369,15 +27342,15 @@
                         } else if (8 * sizeof(npy_int32) >= 4 * PyLong_SHIFT) {
                             return (npy_int32) (((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27565,15 +27538,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27761,15 +27734,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27936,17 +27909,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrImport */
-  #ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
@@ -27985,17 +27958,17 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/_gradient_boosting.pyx` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/_gradient_boosting.pyx`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/forest.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/ensemble/gb.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/ensemble/gb.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/linear_model/base.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/linear_model/base.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/linear_model/implementations.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/linear_model/implementations.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/naive_bayes/implementations.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/naive_bayes/implementations.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/neighbors/_base.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/neighbors/_base.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/neighbors/_classes.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/neighbors/_classes.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/neural_network/_base.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/neural_network/_base.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/neural_network/_classes.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/neural_network/_classes.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/svm/_base.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/svm/_base.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/svm/_classes.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/svm/_classes.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_criterion.c` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_criterion.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O2"
         ],
         "include_dirs": [
             ".",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sklearn_pmml_model.tree._criterion",
         "sources": [
             "sklearn_pmml_model/tree/_criterion.pyx"
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,18 +103,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +394,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +471,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1065,195 +1071,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1428,42 +1434,42 @@
 struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion;
 struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Entropy;
 struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Gini;
 struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MSE;
 struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MAE;
 struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_FriedmanMSE;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2441,30 +2447,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -2649,18 +2655,18 @@
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static int __pyx_f_18sklearn_pmml_model_4tree_10_criterion_9Criterion_init(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion *__pyx_v_self, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_10_criterion_DOUBLE_t *__pyx_v_y, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_10_criterion_SIZE_t __pyx_v_y_stride, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_10_criterion_DOUBLE_t *__pyx_v_sample_weight, CYTHON_UNUSED double __pyx_v_weighted_n_samples, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_10_criterion_SIZE_t *__pyx_v_samples, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_10_criterion_SIZE_t __pyx_v_start, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_10_criterion_SIZE_t __pyx_v_end); /* proto*/
 static int __pyx_f_18sklearn_pmml_model_4tree_10_criterion_9Criterion_reset(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion *__pyx_v_self); /* proto*/
 static int __pyx_f_18sklearn_pmml_model_4tree_10_criterion_9Criterion_reverse_reset(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion *__pyx_v_self); /* proto*/
@@ -10211,15 +10217,15 @@
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10228,29 +10234,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10261,15 +10267,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10278,29 +10284,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10311,15 +10317,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10328,29 +10334,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10361,15 +10367,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10378,29 +10384,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10411,15 +10417,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10428,29 +10434,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10461,212 +10467,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10682,15 +10688,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -10698,53 +10704,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -10752,30 +10758,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10790,15 +10796,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10814,15 +10820,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10830,53 +10836,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -10884,30 +10890,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10922,15 +10928,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10946,15 +10952,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10962,53 +10968,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -11016,30 +11022,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11054,176 +11060,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -11245,15 +11251,15 @@
   p = ((struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion *)o);
   p->__pyx_vtab = __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_Criterion;
   return o;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_10_criterion_Criterion(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -11335,15 +11341,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion __pyx_vtable_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion *p;
@@ -11356,15 +11362,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -11443,15 +11449,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion __pyx_vtable_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion *p;
@@ -11534,15 +11540,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_Entropy __pyx_vtable_18sklearn_pmml_model_4tree_10_criterion_Entropy;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_10_criterion_Entropy(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Entropy *p;
@@ -11616,15 +11622,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_Gini __pyx_vtable_18sklearn_pmml_model_4tree_10_criterion_Gini;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_10_criterion_Gini(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Gini *p;
@@ -11698,15 +11704,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_MSE __pyx_vtable_18sklearn_pmml_model_4tree_10_criterion_MSE;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_10_criterion_MSE(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MSE *p;
@@ -11780,15 +11786,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_MAE __pyx_vtable_18sklearn_pmml_model_4tree_10_criterion_MAE;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_10_criterion_MAE(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MAE *p;
@@ -11804,33 +11810,30 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_10_criterion_MAE(PyObject *o) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MAE *p = (struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MAE *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
     __pyx_pw_18sklearn_pmml_model_4tree_10_criterion_3MAE_1__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->left_child);
   Py_CLEAR(p->right_child);
-  #if CYTHON_USE_TYPE_SLOTS
-  if (PyType_IS_GC(Py_TYPE(o)->tp_base))
-  #endif
-  PyObject_GC_Track(o);
+  if (PyType_IS_GC(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_18sklearn_pmml_model_4tree_10_criterion_Criterion(o);
 }
 
 static int __pyx_tp_traverse_18sklearn_pmml_model_4tree_10_criterion_MAE(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MAE *p = (struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_MAE *)o;
   e = ((likely(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion)) ? ((__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion->tp_traverse) ? __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_18sklearn_pmml_model_4tree_10_criterion_MAE)); if (e) return e;
@@ -11923,15 +11926,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_FriedmanMSE __pyx_vtable_18sklearn_pmml_model_4tree_10_criterion_FriedmanMSE;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_10_criterion_FriedmanMSE(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_FriedmanMSE *p;
@@ -12005,15 +12008,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -12126,26 +12129,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.sample_weight,self.samples,self.sum_left,self.sum_right,self.sum_total,self.y cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_self_sample_weight_self_samples); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -12359,95 +12362,54 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(4, 54, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(4, 54, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree)) __PYX_ERR(4, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(5, 141, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(5, 141, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_Stack*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack)) __PYX_ERR(5, 141, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(5, 170, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(5, 170, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_PriorityHeap*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap)) __PYX_ERR(5, 170, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(5, 193, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(5, 193, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue)) __PYX_ERR(5, 193, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(5, 213, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(5, 213, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator)) __PYX_ERR(5, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -12460,15 +12422,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_36(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -12480,29 +12442,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "sizet_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_sizet_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "log", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_log, "double (double)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "sizet_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_sizet_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "log", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_log, "double (double)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -12736,15 +12698,15 @@
  * # cython: boundscheck=False
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -14460,18 +14422,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -14517,22 +14479,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -15262,15 +15224,15 @@
                         } else if (8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT) {
                             return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15534,15 +15496,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15730,15 +15692,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16005,17 +15967,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrImport */
-  #ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
@@ -16054,17 +16016,17 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_criterion.pxd` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_criterion.pxd`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_criterion.pyx` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_criterion.pyx`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_splitter.c` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_splitter.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O2"
         ],
         "include_dirs": [
             ".",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sklearn_pmml_model.tree._splitter",
         "sources": [
             "sklearn_pmml_model/tree/_splitter.pyx"
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,18 +103,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +394,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +471,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1066,195 +1072,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1485,42 +1491,42 @@
 struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter;
 struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BestSplitter;
 struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_RandomSplitter;
 struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BaseSparseSplitter;
 struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BestSparseSplitter;
 struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_RandomSparseSplitter;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2654,30 +2660,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -2883,18 +2889,18 @@
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static int __pyx_f_18sklearn_pmml_model_4tree_9_splitter_8Splitter_init(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter *__pyx_v_self, PyObject *__pyx_v_X, PyArrayObject *__pyx_v_y, __pyx_t_18sklearn_pmml_model_4tree_9_splitter_DOUBLE_t *__pyx_v_sample_weight, __pyx_t_18sklearn_pmml_model_4tree_9_splitter_INT32_t *__pyx_v_n_categories, struct __pyx_opt_args_18sklearn_pmml_model_4tree_9_splitter_8Splitter_init *__pyx_optional_args); /* proto*/
 static int __pyx_f_18sklearn_pmml_model_4tree_9_splitter_8Splitter_node_reset(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter *__pyx_v_self, __pyx_t_18sklearn_pmml_model_4tree_9_splitter_SIZE_t __pyx_v_start, __pyx_t_18sklearn_pmml_model_4tree_9_splitter_SIZE_t __pyx_v_end, double *__pyx_v_weighted_n_node_samples); /* proto*/
 static int __pyx_f_18sklearn_pmml_model_4tree_9_splitter_8Splitter_node_split(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter *__pyx_v_self, CYTHON_UNUSED double __pyx_v_impurity, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_6_utils_SplitRecord *__pyx_v_split, CYTHON_UNUSED __pyx_t_18sklearn_pmml_model_4tree_9_splitter_SIZE_t *__pyx_v_n_constant_features); /* proto*/
@@ -14987,15 +14993,15 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -15004,29 +15010,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -15037,15 +15043,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15054,29 +15060,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15087,15 +15093,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15104,29 +15110,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15137,15 +15143,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15154,29 +15160,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15187,15 +15193,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15204,29 +15210,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15237,212 +15243,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15458,15 +15464,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -15474,53 +15480,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -15528,30 +15534,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15566,15 +15572,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15590,15 +15596,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -15606,53 +15612,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -15660,30 +15666,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15698,15 +15704,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15722,15 +15728,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -15738,53 +15744,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -15792,30 +15798,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15830,176 +15836,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -16028,15 +16034,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_9_splitter_Splitter(PyObject *o) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter *p = (struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16208,15 +16214,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter __pyx_vtable_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter *p;
@@ -16231,15 +16237,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter(PyObject *o) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter *p = (struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BaseDenseSplitter *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16342,15 +16348,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_BestSplitter __pyx_vtable_18sklearn_pmml_model_4tree_9_splitter_BestSplitter;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_9_splitter_BestSplitter(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BestSplitter *p;
@@ -16429,15 +16435,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_RandomSplitter __pyx_vtable_18sklearn_pmml_model_4tree_9_splitter_RandomSplitter;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_9_splitter_RandomSplitter(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_RandomSplitter *p;
@@ -16516,15 +16522,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_BaseSparseSplitter __pyx_vtable_18sklearn_pmml_model_4tree_9_splitter_BaseSparseSplitter;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_9_splitter_BaseSparseSplitter(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BaseSparseSplitter *p;
@@ -16537,15 +16543,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_9_splitter_BaseSparseSplitter(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16627,15 +16633,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_BestSparseSplitter __pyx_vtable_18sklearn_pmml_model_4tree_9_splitter_BestSparseSplitter;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_9_splitter_BestSparseSplitter(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_BestSparseSplitter *p;
@@ -16714,15 +16720,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_RandomSparseSplitter __pyx_vtable_18sklearn_pmml_model_4tree_9_splitter_RandomSparseSplitter;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_9_splitter_RandomSparseSplitter(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_RandomSparseSplitter *p;
@@ -16801,15 +16807,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -16984,26 +16990,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -17182,110 +17188,63 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(5, 54, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(5, 54, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree)) __PYX_ERR(5, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(6, 141, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(6, 141, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_Stack*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack)) __PYX_ERR(6, 141, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(6, 170, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(6, 170, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_PriorityHeap*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap)) __PYX_ERR(6, 170, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(6, 193, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(6, 193, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue)) __PYX_ERR(6, 193, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(6, 213, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(6, 213, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator)) __PYX_ERR(6, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._criterion"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "Criterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion) __PYX_ERR(7, 23, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "Criterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion) __PYX_ERR(7, 23, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_Criterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_Criterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_Criterion)) __PYX_ERR(7, 23, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "ClassificationCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion) __PYX_ERR(7, 71, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "ClassificationCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion) __PYX_ERR(7, 71, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion)) __PYX_ERR(7, 71, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "RegressionCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion) __PYX_ERR(7, 77, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "RegressionCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion) __PYX_ERR(7, 77, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion)) __PYX_ERR(7, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -17298,15 +17257,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_36(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -17318,32 +17277,32 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "rand_int", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_rand_int, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t (__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "rand_uniform", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_rand_uniform, "double (double, double, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "log", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_log, "double (double)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "setup_cat_cache", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_setup_cat_cache, "void (__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT64_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "goes_left", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_goes_left, "int (__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SplitValue, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "rand_int", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_rand_int, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t (__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "rand_uniform", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_rand_uniform, "double (double, double, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "log", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_log, "double (double)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "setup_cat_cache", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_setup_cat_cache, "void (__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT64_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "goes_left", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_goes_left, "int (__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SplitValue, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -17634,15 +17593,15 @@
  * # cython: boundscheck=False
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19374,18 +19333,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -19431,22 +19390,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -20190,15 +20149,15 @@
                         } else if (8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT) {
                             return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20424,15 +20383,15 @@
                         } else if (8 * sizeof(npy_uint32) >= 4 * PyLong_SHIFT) {
                             return (npy_uint32) (((((((((npy_uint32)digits[3]) << PyLong_SHIFT) | (npy_uint32)digits[2]) << PyLong_SHIFT) | (npy_uint32)digits[1]) << PyLong_SHIFT) | (npy_uint32)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20696,15 +20655,15 @@
                         } else if (8 * sizeof(npy_int32) >= 4 * PyLong_SHIFT) {
                             return (npy_int32) (((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20968,15 +20927,15 @@
                         } else if (8 * sizeof(npy_uint64) >= 4 * PyLong_SHIFT) {
                             return (npy_uint64) (((((((((npy_uint64)digits[3]) << PyLong_SHIFT) | (npy_uint64)digits[2]) << PyLong_SHIFT) | (npy_uint64)digits[1]) << PyLong_SHIFT) | (npy_uint64)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21164,15 +21123,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21360,15 +21319,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21635,17 +21594,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrImport */
-  #ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
@@ -21684,17 +21643,17 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_splitter.pxd` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_splitter.pxd`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_splitter.pyx` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_splitter.pyx`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_tree.c` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_tree.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O2"
         ],
         "include_dirs": [
             ".",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sklearn_pmml_model.tree._tree",
         "sources": [
             "sklearn_pmml_model/tree/_tree.pyx"
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,18 +103,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +394,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +471,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1071,195 +1077,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1535,42 +1541,42 @@
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr;
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree;
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder;
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder;
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder;
 struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree___pyx_scope_struct____get__;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2917,30 +2923,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -3146,18 +3152,18 @@
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_f_18sklearn_pmml_model_4tree_5_tree_11TreeBuilder_build(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder *__pyx_v_self, CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_tree, CYTHON_UNUSED PyObject *__pyx_v_X, CYTHON_UNUSED PyArrayObject *__pyx_v_y, int __pyx_skip_dispatch, struct __pyx_opt_args_18sklearn_pmml_model_4tree_5_tree_11TreeBuilder_build *__pyx_optional_args); /* proto*/
 static PyObject *__pyx_f_18sklearn_pmml_model_4tree_5_tree_11TreeBuilder__check_input(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder *__pyx_v_self, PyObject *__pyx_v_X, PyArrayObject *__pyx_v_y, PyArrayObject *__pyx_v_sample_weight); /* proto*/
 static PyObject *__pyx_f_18sklearn_pmml_model_4tree_5_tree_21DepthFirstTreeBuilder_build(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder *__pyx_v_self, struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_tree, PyObject *__pyx_v_X, PyArrayObject *__pyx_v_y, int __pyx_skip_dispatch, struct __pyx_opt_args_18sklearn_pmml_model_4tree_5_tree_21DepthFirstTreeBuilder_build *__pyx_optional_args); /* proto*/
@@ -3660,15 +3666,15 @@
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_21DepthFirstTreeBuilder_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_21DepthFirstTreeBuilder_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_18sklearn_pmml_model_4tree_5_tree_20BestFirstTreeBuilder___cinit__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder *__pyx_v_self, struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter *__pyx_v_splitter, __pyx_t_18sklearn_pmml_model_4tree_5_tree_SIZE_t __pyx_v_min_samples_split, __pyx_t_18sklearn_pmml_model_4tree_5_tree_SIZE_t __pyx_v_min_samples_leaf, PyObject *__pyx_v_min_weight_leaf, __pyx_t_18sklearn_pmml_model_4tree_5_tree_SIZE_t __pyx_v_max_depth, __pyx_t_18sklearn_pmml_model_4tree_5_tree_SIZE_t __pyx_v_max_leaf_nodes, double __pyx_v_min_impurity_decrease, double __pyx_v_min_impurity_split); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_20BestFirstTreeBuilder_2build(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder *__pyx_v_self, struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_tree, PyObject *__pyx_v_X, PyArrayObject *__pyx_v_y, PyArrayObject *__pyx_v_sample_weight, PyArrayObject *__pyx_v_n_categories, PyArrayObject *__pyx_v_X_idx_sorted); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_20BestFirstTreeBuilder_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_20BestFirstTreeBuilder_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr___cinit__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_2_dealloc__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *__pyx_v_self); /* proto */
+static void __pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_2__dealloc__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_4Tree_9n_classes___get__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_4Tree_13children_left___get__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_4Tree_14children_right___get__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_4Tree_8n_leaves___get__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_4Tree_7feature___get__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *__pyx_v_self); /* proto */
@@ -9005,15 +9011,15 @@
   __pyx_v_self->n_nodes = 0;
 
   /* "sklearn_pmml_model/tree/_tree.pyx":535
  *     def __cinit__(self):
  *         self.n_nodes = 0
  *         self.bits = NULL             # <<<<<<<<<<<<<<
  * 
- *     def _dealloc__(self):
+ *     def __dealloc__(self):
  */
   __pyx_v_self->bits = NULL;
 
   /* "sklearn_pmml_model/tree/_tree.pyx":533
  *     """
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
@@ -9026,41 +9032,38 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "sklearn_pmml_model/tree/_tree.pyx":537
  *         self.bits = NULL
  * 
- *     def _dealloc__(self):             # <<<<<<<<<<<<<<
+ *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cdef int i
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_3_dealloc__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_3_dealloc__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
+static void __pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_dealloc__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_2_dealloc__(((struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *)__pyx_v_self));
+  __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
+  __pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_2__dealloc__(((struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
-  return __pyx_r;
 }
 
-static PyObject *__pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_2_dealloc__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *__pyx_v_self) {
+static void __pyx_pf_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_2__dealloc__(struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr *__pyx_v_self) {
   int __pyx_v_i;
-  PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __pyx_t_18sklearn_pmml_model_4tree_5_tree_SIZE_t __pyx_t_2;
   __pyx_t_18sklearn_pmml_model_4tree_5_tree_SIZE_t __pyx_t_3;
   int __pyx_t_4;
-  __Pyx_RefNannySetupContext("_dealloc__", 0);
+  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "sklearn_pmml_model/tree/_tree.pyx":540
  *         cdef int i
  * 
  *         if self.bits != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(self.n_nodes):
  *                 free(self.bits[i])
@@ -9107,24 +9110,21 @@
  *     cdef void populate(self, Node *nodes, SIZE_t n_nodes, INT32_t *n_categories):
  */
   free(__pyx_v_self->bits);
 
   /* "sklearn_pmml_model/tree/_tree.pyx":537
  *         self.bits = NULL
  * 
- *     def _dealloc__(self):             # <<<<<<<<<<<<<<
+ *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cdef int i
  * 
  */
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
-  return __pyx_r;
 }
 
 /* "sklearn_pmml_model/tree/_tree.pyx":545
  *         free(self.bits)
  * 
  *     cdef void populate(self, Node *nodes, SIZE_t n_nodes, INT32_t *n_categories):             # <<<<<<<<<<<<<<
  *         cdef SIZE_t i
@@ -18582,15 +18582,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18599,29 +18599,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18632,15 +18632,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18649,29 +18649,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18682,15 +18682,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18699,29 +18699,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18732,15 +18732,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18749,29 +18749,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18782,15 +18782,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18799,29 +18799,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18832,212 +18832,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19053,15 +19053,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19069,53 +19069,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -19123,30 +19123,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19161,15 +19161,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19185,15 +19185,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19201,53 +19201,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -19255,30 +19255,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19293,15 +19293,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19317,15 +19317,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19333,53 +19333,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -19387,30 +19387,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19425,176 +19425,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19620,23 +19620,30 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
+  {
+    PyObject *etype, *eval, *etb;
+    PyErr_Fetch(&etype, &eval, &etb);
+    __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
+    __pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_3__dealloc__(o);
+    __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
+    PyErr_Restore(etype, eval, etb);
+  }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr[] = {
-  {"_dealloc__", (PyCFunction)__pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_3_dealloc__, METH_NOARGS, 0},
   {"__reduce_cython__", (PyCFunction)__pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_5__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw_18sklearn_pmml_model_4tree_5_tree_16CategoryCacheMgr_7__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_18sklearn_pmml_model_4tree_5_tree_CategoryCacheMgr = {
   PyVarObject_HEAD_INIT(0, 0)
@@ -19701,15 +19708,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_5_tree_Tree __pyx_vtable_18sklearn_pmml_model_4tree_5_tree_Tree;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_5_tree_Tree(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_Tree *p;
@@ -19727,15 +19734,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_5_tree_Tree(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -19970,15 +19977,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_5_tree_TreeBuilder __pyx_vtable_18sklearn_pmml_model_4tree_5_tree_TreeBuilder;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_5_tree_TreeBuilder(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder *p;
@@ -19994,15 +20001,15 @@
   p->splitter = ((struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_5_tree_TreeBuilder(PyObject *o) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder *p = (struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_TreeBuilder *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->splitter);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -20095,15 +20102,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder __pyx_vtable_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_DepthFirstTreeBuilder *p;
@@ -20188,15 +20195,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder __pyx_vtable_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree_BestFirstTreeBuilder *p;
@@ -20281,15 +20288,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_18sklearn_pmml_model_4tree_5_tree___pyx_scope_struct____get__ *__pyx_freelist_18sklearn_pmml_model_4tree_5_tree___pyx_scope_struct____get__[8];
 static int __pyx_freecount_18sklearn_pmml_model_4tree_5_tree___pyx_scope_struct____get__ = 0;
 
@@ -20399,15 +20406,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -20735,26 +20742,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5739659, 0x7c1ad9d, 0x3dc6771) = (max_depth, min_impurity_decrease, min_impurity_split, min_samples_leaf, min_samples_split, min_weight_leaf, splitter))" % __pyx_checksum)
  */
   __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_91461209, __pyx_int_130133405, __pyx_int_64776049); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -20945,129 +20952,76 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(7, 54, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(7, 54, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree)) __PYX_ERR(7, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(8, 141, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(8, 141, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_Stack*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack)) __PYX_ERR(8, 141, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(8, 170, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(8, 170, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_PriorityHeap*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap)) __PYX_ERR(8, 170, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(8, 193, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(8, 193, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue)) __PYX_ERR(8, 193, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(8, 213, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(8, 213, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator)) __PYX_ERR(8, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._criterion"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "Criterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion) __PYX_ERR(9, 23, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "Criterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_Criterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion) __PYX_ERR(9, 23, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_Criterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_Criterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_Criterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_Criterion)) __PYX_ERR(9, 23, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "ClassificationCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion) __PYX_ERR(9, 71, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "ClassificationCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion) __PYX_ERR(9, 71, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_ClassificationCriterion)) __PYX_ERR(9, 71, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "RegressionCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion) __PYX_ERR(9, 77, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._criterion", "RegressionCriterion", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion) __PYX_ERR(9, 77, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_10_criterion_RegressionCriterion)) __PYX_ERR(9, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._splitter"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._splitter", "Splitter", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter) __PYX_ERR(10, 28, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._splitter", "Splitter", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_9_splitter_Splitter),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter) __PYX_ERR(10, 28, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_9_splitter_Splitter = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9_splitter_Splitter*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_9_splitter_Splitter->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_9_splitter_Splitter)) __PYX_ERR(10, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -21080,15 +21034,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_36(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -21100,31 +21054,31 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "sizet_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_sizet_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "int32_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_int32_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "setup_cat_cache", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_setup_cat_cache, "void (__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT64_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "goes_left", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_goes_left, "int (__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SplitValue, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "sizet_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_sizet_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "int32_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_int32_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "setup_cat_cache", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_setup_cat_cache, "void (__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT64_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "goes_left", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_goes_left, "int (__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SplitValue, __pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t, __pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -21877,15 +21831,15 @@
  * # cython: boundscheck=False
  */
   __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_6) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23764,15 +23718,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -24893,18 +24850,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -24950,22 +24907,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -25755,15 +25712,15 @@
                         } else if (8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT) {
                             return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25951,15 +25908,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26147,15 +26104,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26457,15 +26414,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26691,15 +26648,15 @@
                         } else if (8 * sizeof(npy_int32) >= 4 * PyLong_SHIFT) {
                             return (npy_int32) (((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26966,17 +26923,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrImport */
-  #ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
@@ -27015,17 +26972,17 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_tree.pxd` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_tree.pxd`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_tree.pyx` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_tree.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -530,15 +530,15 @@
     """Class to manage the category cache memory during Tree.apply()
     """
 
     def __cinit__(self):
         self.n_nodes = 0
         self.bits = NULL
 
-    def _dealloc__(self):
+    def __dealloc__(self):
         cdef int i
 
         if self.bits != NULL:
             for i in range(self.n_nodes):
                 free(self.bits[i])
         free(self.bits)
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_utils.c` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_utils.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O2"
         ],
         "include_dirs": [
             ".",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sklearn_pmml_model.tree._utils",
         "sources": [
             "sklearn_pmml_model/tree/_utils.pyx"
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,18 +103,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +394,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +471,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1028,195 +1034,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1338,42 +1344,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree;
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack;
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap;
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue;
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1961,14 +1967,31 @@
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
@@ -2039,30 +2062,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -2257,15 +2280,15 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static int __pyx_f_18sklearn_pmml_model_4tree_6_utils_5Stack_is_empty(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack *__pyx_v_self); /* proto*/
 static int __pyx_f_18sklearn_pmml_model_4tree_6_utils_5Stack_push(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack *__pyx_v_self, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t __pyx_v_start, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t __pyx_v_end, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t __pyx_v_depth, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t __pyx_v_parent, int __pyx_v_is_left, double __pyx_v_impurity, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t __pyx_v_n_constant_features); /* proto*/
 static int __pyx_f_18sklearn_pmml_model_4tree_6_utils_5Stack_pop(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack *__pyx_v_self, struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *__pyx_v_res); /* proto*/
@@ -6223,15 +6246,15 @@
  *     if p != NULL:
  *         free(p)
  *         assert False             # <<<<<<<<<<<<<<
  * 
  * 
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!0)) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(0, 53, __pyx_L1_error)
       }
     }
     #endif
 
@@ -10828,15 +10851,15 @@
   __Pyx_AddTraceback("sklearn_pmml_model.tree._utils.WeightedMedianCalculator.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10845,29 +10868,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10878,15 +10901,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10895,29 +10918,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10928,15 +10951,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10945,29 +10968,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10978,15 +11001,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10995,29 +11018,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11028,15 +11051,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11045,29 +11068,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11078,212 +11101,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11299,15 +11322,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -11315,53 +11338,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -11369,30 +11392,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11407,15 +11430,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11431,15 +11454,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11447,53 +11470,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -11501,30 +11524,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11539,15 +11562,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11563,15 +11586,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11579,53 +11602,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -11633,30 +11656,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11671,176 +11694,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -11866,15 +11889,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_6_utils_Stack(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -11954,15 +11977,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_PriorityHeap __pyx_vtable_18sklearn_pmml_model_4tree_6_utils_PriorityHeap;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_6_utils_PriorityHeap(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap *p;
@@ -11980,15 +12003,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_6_utils_PriorityHeap(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -12068,15 +12091,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue __pyx_vtable_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue *p;
@@ -12094,15 +12117,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -12182,15 +12205,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator __pyx_vtable_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator;
 
 static PyObject *__pyx_tp_new_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator *p;
@@ -12210,15 +12233,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator(PyObject *o) {
   struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator *p = (struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->samples);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -12310,15 +12333,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -12490,26 +12513,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -12531,14 +12554,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -12692,76 +12720,43 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(4, 54, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree.quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree) __PYX_ERR(4, 54, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_9quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_9quad_tree__QuadTree->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_9quad_tree__QuadTree)) __PYX_ERR(4, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -12774,15 +12769,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree.quad_tree"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_36(__pyx_t_1, "EPSILON", (void **)&__pyx_vp_18sklearn_pmml_model_4tree_9quad_tree_EPSILON, "float") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -13036,15 +13031,15 @@
  * # cython: boundscheck=False
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -14285,18 +14280,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -14342,22 +14337,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -15106,15 +15101,15 @@
                         } else if (8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT) {
                             return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15340,15 +15335,15 @@
                         } else if (8 * sizeof(npy_int32) >= 4 * PyLong_SHIFT) {
                             return (npy_int32) (((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15536,15 +15531,15 @@
                         } else if (8 * sizeof(npy_uint64) >= 4 * PyLong_SHIFT) {
                             return (npy_uint64) (((((((((npy_uint64)digits[3]) << PyLong_SHIFT) | (npy_uint64)digits[2]) << PyLong_SHIFT) | (npy_uint64)digits[1]) << PyLong_SHIFT) | (npy_uint64)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15770,15 +15765,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15966,15 +15961,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16278,17 +16273,17 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* VoidPtrImport */
-#ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_36
+static int __Pyx_ImportVoidPtr_0_29_36(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_utils.pxd` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_utils.pxd`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/_utils.pyx` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/_utils.pyx`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/quad_tree.c` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/quad_tree.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O2"
         ],
         "include_dirs": [
             ".",
-            "/opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sklearn_pmml_model.tree.quad_tree",
         "sources": [
             "sklearn_pmml_model/tree/quad_tree.pyx"
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,18 +103,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +394,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +471,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1032,195 +1038,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1342,42 +1348,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack;
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap;
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue;
 struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator;
 struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2064,14 +2070,31 @@
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
@@ -2158,30 +2181,30 @@
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -2374,15 +2397,15 @@
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
 #endif
 
 /* VoidPtrExport.proto */
 static int __Pyx_ExportVoidPtr(PyObject *name, void *p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static int __pyx_f_18sklearn_pmml_model_4tree_9quad_tree_9_QuadTree_insert_point(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree *__pyx_v_self, __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_DTYPE_t *__pyx_v_point, __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_SIZE_t __pyx_v_point_index, struct __pyx_opt_args_18sklearn_pmml_model_4tree_9quad_tree_9_QuadTree_insert_point *__pyx_optional_args); /* proto*/
 static __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_SIZE_t __pyx_f_18sklearn_pmml_model_4tree_9quad_tree_9_QuadTree__insert_point_in_new_child(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree *__pyx_v_self, __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_DTYPE_t *__pyx_v_point, struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *__pyx_v_cell, __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_SIZE_t __pyx_v_point_index, struct __pyx_opt_args_18sklearn_pmml_model_4tree_9quad_tree_9_QuadTree__insert_point_in_new_child *__pyx_optional_args); /* proto*/
 static int __pyx_f_18sklearn_pmml_model_4tree_9quad_tree_9_QuadTree__is_duplicate(struct __pyx_obj_18sklearn_pmml_model_4tree_9quad_tree__QuadTree *__pyx_v_self, __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_DTYPE_t *__pyx_v_point1, __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_DTYPE_t *__pyx_v_point2); /* proto*/
@@ -5286,15 +5309,15 @@
  *                         child = self.cells[child_id]
  *                         n_points += child.cumulative_size
  *                         assert child.cell_id == child_id, (             # <<<<<<<<<<<<<<
  *                             "Cell id not correctly initiliazed.")
  *                 if n_points != cell.cumulative_size:
  */
           #ifndef CYTHON_WITHOUT_ASSERTIONS
-          if (unlikely(!Py_OptimizeFlag)) {
+          if (unlikely(__pyx_assertions_enabled())) {
             if (unlikely(!((__pyx_v_child.cell_id == __pyx_v_child_id) != 0))) {
               PyErr_SetObject(PyExc_AssertionError, __pyx_kp_u_Cell_id_not_correctly_initiliaze);
               __PYX_ERR(0, 379, __pyx_L1_error)
             }
           }
           #endif
 
@@ -5905,15 +5928,15 @@
  *         cdef int i
  * 
  *         assert len(point) == self.n_dimensions, (             # <<<<<<<<<<<<<<
  *             "Query point should be a point in dimension {}."
  *             .format(self.n_dimensions))
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = PyObject_Length(__pyx_v_point); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 479, __pyx_L1_error)
     if (unlikely(!((__pyx_t_1 == __pyx_v_self->n_dimensions) != 0))) {
 
       /* "sklearn_pmml_model/tree/quad_tree.pyx":481
  *         assert len(point) == self.n_dimensions, (
  *             "Query point should be a point in dimension {}."
  *             .format(self.n_dimensions))             # <<<<<<<<<<<<<<
@@ -7787,15 +7810,15 @@
  *         ds2c = ((X[0] - barycenter) ** 2).sum()
  * 
  *         assert idx == offset             # <<<<<<<<<<<<<<
  *         assert node_size == 3, "summary size = {}".format(node_size)
  *         assert np.isclose(node_dist, ds2c)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_v_offset, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 651, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(0, 651, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_14)) {
@@ -7809,15 +7832,15 @@
  * 
  *         assert idx == offset
  *         assert node_size == 3, "summary size = {}".format(node_size)             # <<<<<<<<<<<<<<
  *         assert np.isclose(node_dist, ds2c)
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_v_node_size, __pyx_int_3, 3, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_14)) {
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_summary_size, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
@@ -7850,15 +7873,15 @@
  *         assert idx == offset
  *         assert node_size == 3, "summary size = {}".format(node_size)
  *         assert np.isclose(node_dist, ds2c)             # <<<<<<<<<<<<<<
  * 
  *         # Summary should contain all 3 node with size 1 and distance to
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 653, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_isclose); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 653, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
@@ -8012,15 +8035,15 @@
  *         ds2c = ((X[0] - barycenter) ** 2).sum()
  * 
  *         assert idx == 3 * (offset)             # <<<<<<<<<<<<<<
  *         for i in range(3):
  *             node_dist = summary[i * offset + n_dimensions]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_6 = __Pyx_PyInt_From_long(__pyx_v_idx); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = PyNumber_Multiply(__pyx_int_3, __pyx_v_offset); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_1 = PyObject_RichCompare(__pyx_t_6, __pyx_t_7, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
@@ -8139,15 +8162,15 @@
     /* "sklearn_pmml_model/tree/quad_tree.pyx":672
  *             ds2c = ((X[0] - X[i + 1]) ** 2).sum()
  * 
  *             assert node_size == 1, "summary size = {}".format(node_size)             # <<<<<<<<<<<<<<
  *             assert np.isclose(node_dist, ds2c)
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_v_node_size, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 672, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(0, 672, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(!__pyx_t_14)) {
         __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_summary_size, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 672, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
@@ -8178,15 +8201,15 @@
 
     /* "sklearn_pmml_model/tree/quad_tree.pyx":673
  * 
  *             assert node_size == 1, "summary size = {}".format(node_size)
  *             assert np.isclose(node_dist, ds2c)             # <<<<<<<<<<<<<<
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 673, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isclose); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 673, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       __pyx_t_9 = 0;
@@ -8765,15 +8788,15 @@
   __Pyx_AddTraceback("sklearn_pmml_model.tree.quad_tree._QuadTree.n_points.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8782,29 +8805,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8815,15 +8838,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8832,29 +8855,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8865,15 +8888,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8882,29 +8905,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8915,15 +8938,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8932,29 +8955,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8965,15 +8988,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8982,29 +9005,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9015,212 +9038,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9236,15 +9259,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -9252,53 +9275,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -9306,30 +9329,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9344,15 +9367,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9368,15 +9391,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9384,53 +9407,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -9438,30 +9461,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9476,15 +9499,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9500,15 +9523,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9516,53 +9539,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -9570,30 +9593,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9608,176 +9631,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -10022,15 +10045,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_18sklearn_pmml_model_4tree_9quad_tree__QuadTree(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -10219,15 +10242,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -10422,26 +10445,26 @@
  *         ds2c = ((X[0] - barycenter) ** 2).sum()
  * 
  */
   __pyx_slice__5 = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.8.16/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.8.17/x64/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -10463,14 +10486,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1_ = PyFloat_FromDouble(1.); if (unlikely(!__pyx_float_1_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_9_ = PyFloat_FromDouble(9.); if (unlikely(!__pyx_float_9_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_10_ = PyFloat_FromDouble(10.); if (unlikely(!__pyx_float_10_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1eneg_3 = PyFloat_FromDouble(1e-3); if (unlikely(!__pyx_float_1eneg_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_neg_10_ = PyFloat_FromDouble(-10.); if (unlikely(!__pyx_float_neg_10_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -10565,100 +10593,57 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(7, 141, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "Stack", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_Stack),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack) __PYX_ERR(7, 141, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_Stack*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_Stack->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_Stack)) __PYX_ERR(7, 141, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(7, 170, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "PriorityHeap", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_PriorityHeap),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap) __PYX_ERR(7, 170, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_PriorityHeap*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_PriorityHeap->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_PriorityHeap)) __PYX_ERR(7, 170, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(7, 193, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue) __PYX_ERR(7, 193, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedPQueue)) __PYX_ERR(7, 193, __pyx_L1_error)
-  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(7, 213, __pyx_L1_error)
+  __pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = __Pyx_ImportType_0_29_36(__pyx_t_1, "sklearn_pmml_model.tree._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator) __PYX_ERR(7, 213, __pyx_L1_error)
   __pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator = (struct __pyx_vtabstruct_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator*)__Pyx_GetVtable(__pyx_ptype_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator->tp_dict); if (unlikely(!__pyx_vtabptr_18sklearn_pmml_model_4tree_6_utils_WeightedMedianCalculator)) __PYX_ERR(7, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -10679,28 +10664,28 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("sklearn_pmml_model.tree._utils"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "sizet_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_sizet_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "sizet_ptr_to_ndarray", (void (**)(void))&__pyx_f_18sklearn_pmml_model_4tree_6_utils_sizet_ptr_to_ndarray, "PyArrayObject *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *, __pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_0safe_realloc", (void (**)(void))&__pyx_fuse_0__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DTYPE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_1safe_realloc", (void (**)(void))&__pyx_fuse_1__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_SIZE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_2safe_realloc", (void (**)(void))&__pyx_fuse_2__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "unsigned char *(unsigned char **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_3safe_realloc", (void (**)(void))&__pyx_fuse_3__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_WeightedPQueueRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_4safe_realloc", (void (**)(void))&__pyx_fuse_4__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_DOUBLE_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_5safe_realloc", (void (**)(void))&__pyx_fuse_5__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_6safe_realloc", (void (**)(void))&__pyx_fuse_6__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell *(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_7safe_realloc", (void (**)(void))&__pyx_fuse_7__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node **(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_Node ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_8safe_realloc", (void (**)(void))&__pyx_fuse_8__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_StackRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_9safe_realloc", (void (**)(void))&__pyx_fuse_9__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord *(struct __pyx_t_18sklearn_pmml_model_4tree_6_utils_PriorityHeapRecord **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_10safe_realloc", (void (**)(void))&__pyx_fuse_10__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "void **(void ***, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_11safe_realloc", (void (**)(void))&__pyx_fuse_11__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_INT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "__pyx_fuse_12safe_realloc", (void (**)(void))&__pyx_fuse_12__pyx_f_18sklearn_pmml_model_4tree_6_utils_safe_realloc, "__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t *(__pyx_t_18sklearn_pmml_model_4tree_6_utils_UINT32_t **, size_t, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11379,15 +11364,15 @@
  * })
  * 
  * assert CELL_DTYPE.itemsize == sizeof(Cell)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_CELL_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyInt_FromSize_t((sizeof(struct __pyx_t_18sklearn_pmml_model_4tree_9quad_tree_Cell))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
@@ -13163,18 +13148,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-    #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+    #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -13220,22 +13205,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -14019,15 +14004,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14329,15 +14314,15 @@
                         } else if (8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT) {
                             return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14525,15 +14510,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14721,15 +14706,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15041,17 +15026,17 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* FunctionImport */
-    #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+    #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/quad_tree.pxd` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/quad_tree.pxd`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/quad_tree.pyx` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/quad_tree.pyx`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model/tree/tree.py` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model/tree/tree.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/PKG-INFO` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: sklearn-pmml-model
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library to parse PMML models into Scikit-learn estimators.
 Home-page: https://github.com/iamDecode/sklearn-pmml-model
 Author: Dennis Collaris
 Author-email: d.collaris@me.com
 License: BSD-2-Clause
 Description: <img src="https://user-images.githubusercontent.com/1223300/41346080-c2c910a0-6f05-11e8-89e9-71a72bb9543f.png" width="300">
         
         # sklearn-pmml-model
         
         [![PyPI version](https://badge.fury.io/py/sklearn-pmml-model.svg)](https://badge.fury.io/py/sklearn-pmml-model)
         [![codecov](https://codecov.io/gh/iamDecode/sklearn-pmml-model/branch/master/graph/badge.svg?token=CGbbgziGwn)](https://codecov.io/gh/iamDecode/sklearn-pmml-model)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/iamDecode/sklearn-pmml-model.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/iamDecode/sklearn-pmml-model/context:python)
         [![CircleCI](https://circleci.com/gh/iamDecode/sklearn-pmml-model.svg?style=shield)](https://circleci.com/gh/iamDecode/sklearn-pmml-model)
         [![ReadTheDocs](https://readthedocs.org/projects/sklearn-pmml-model/badge/?version=latest&style=flat)](https://sklearn-pmml-model.readthedocs.io/en/latest/)
         
         A library to effortlessly import models trained on different platforms and with programming languages into scikit-learn in Python. First export your model to [PMML](http://dmg.org/pmml/v4-3/GeneralStructure.html) (widely supported). Next, load the exported PMML file with this library, and use the class as any other scikit-learn estimator.
         
         
         ## Installation
```

### Comparing `sklearn-pmml-model-1.0.2/sklearn_pmml_model.egg-info/SOURCES.txt` & `sklearn-pmml-model-1.0.3/sklearn_pmml_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/tests/test_base.py` & `sklearn-pmml-model-1.0.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sklearn-pmml-model-1.0.2/tests/test_datatypes.py` & `sklearn-pmml-model-1.0.3/tests/test_datatypes.py`

 * *Files identical despite different names*

