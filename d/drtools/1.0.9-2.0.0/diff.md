# Comparing `tmp/drtools-1.0.9.tar.gz` & `tmp/drtools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtools-1.0.9.tar", last modified: Sat Feb 11 04:32:48 2023, max compression
+gzip compressed data, was "drtools-2.0.0.tar", last modified: Sun Jul 16 21:13:47 2023, max compression
```

## Comparing `drtools-1.0.9.tar` & `drtools-2.0.0.tar`

### file list

```diff
@@ -1,63 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-11 04:32:34.000000 drtools-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-11 04:32:48.870935 drtools-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-11 04:32:34.000000 drtools-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-11 04:32:34.000000 drtools-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-11 04:32:48.870935 drtools-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.850936 drtools-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.858935 drtools-1.0.9/src/drtools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.862935 drtools-1.0.9/src/drtools/data_science/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/beyond_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/data_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/data_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.862935 drtools-1.0.9/src/drtools/data_science/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/shrinkage.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/subset_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/multiple_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    28368 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.862935 drtools-1.0.9/src/drtools/data_science/resampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resampling/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resampling/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/data_science/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54879 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resources/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/statistical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/survival_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/test_error_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/tree_based.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/unsupervised_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/database/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/connection/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/geo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/geo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/scrapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/thread_pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.858935 drtools-1.0.9/src/drtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-11 04:32:34.000000 drtools-1.0.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.355742 drtools-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 21:13:38.000000 drtools-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-16 21:13:47.355742 drtools-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-16 21:13:38.000000 drtools-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-16 21:13:38.000000 drtools-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-16 21:13:47.355742 drtools-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.347742 drtools-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.351742 drtools-2.0.0/src/drtools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.351742 drtools-2.0.0/src/drtools/data_science/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/data_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/data_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/features_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/model_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28368 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.351742 drtools-2.0.0/src/drtools/data_science/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54259 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/resources/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/statistical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/data_science/time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.351742 drtools-2.0.0/src/drtools/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.355742 drtools-2.0.0/src/drtools/database/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/database/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/database/connection/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/database/connection/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/database/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.355742 drtools-2.0.0/src/drtools/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/geo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.355742 drtools-2.0.0/src/drtools/scrapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/scrapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/scrapping/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/scrapping/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/scrapping/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/thread_pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37340 2023-07-16 21:13:38.000000 drtools-2.0.0/src/drtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.351742 drtools-2.0.0/src/drtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-16 21:13:47.000000 drtools-2.0.0/src/drtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-16 21:13:47.000000 drtools-2.0.0/src/drtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:13:47.000000 drtools-2.0.0/src/drtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 21:13:47.000000 drtools-2.0.0/src/drtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:13:47.355742 drtools-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-16 21:13:38.000000 drtools-2.0.0/tests/test_utils.py
```

### Comparing `drtools-1.0.9/LICENSE` & `drtools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/PKG-INFO` & `drtools-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drtools
-Version: 1.0.9
+Version: 2.0.0
 Summary: Kit of MY useful tools.
 Home-page: https://github.com/andreylcj/drtools
 Author: Andrey Malheiros
 Author-email: example@email.com
 Project-URL: repository, https://github.com/andreylcj/dr_tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drtools-1.0.9/setup.cfg` & `drtools-2.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drtools
-version = 1.0.9
+version = 2.0.0
 author = Andrey Malheiros
 author_email = example@email.com
 description = Kit of MY useful tools.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/andreylcj/drtools
 project_urls =
```

### Comparing `drtools-1.0.9/src/drtools/data_science/data_handle.py` & `drtools-2.0.0/src/drtools/data_science/data_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """ 
 This module was created to handle DataFrames and returns 
 pandas DataFrame or pandas Series.
 
 """
 
 
-import drtools.utils as Utils
+from drtools.utils import list_ops
 from typing import List, Union, Tuple
 from pandas import DataFrame, Series, cut
 from scipy import stats
 import numpy as np
 import math
 from copy import deepcopy
+import pandas as pd
 
 
 ByPercentage = 'by-percentage'
 ByCount = 'by-count'
 Lower = 'lower'
 Upper = 'upper'
 
@@ -183,15 +184,15 @@
     categories: List[str]=[], 
     to_category: str='others'
 ) -> DataFrame:
     """Join categories and fill these values with desired value.
 
     Parameters
     ----------
-    df : DataFrame
+    dataframe : DataFrame
         The DataFrame
     col_name : str
         The column name where categories will be joined.
     categories : List[str], optional
         List of categories will be joined, by default []
     to_category : str, optional
         New value for selected categories, by default 'others'
@@ -205,14 +206,52 @@
     if len(categories) == 0:
         return df
     condition = df[col_name].isin(categories)
     df.loc[condition, col_name] = to_category
     return df
 
 
+def keep_categories_and_join_remaining(
+    dataframe: DataFrame,
+    column: str,
+    categories: List[str]=[], 
+    to_category: str='others'
+) -> DataFrame:
+    """Join categories and fill these values with desired value.
+
+    Parameters
+    ----------
+    dataframe : DataFrame
+        The DataFrame
+    column : str
+        The column name where categories will be joined.
+    categories : List[str], optional
+        List of categories will be joined, by default []
+    to_category : str, optional
+        New value for selected categories, by default 'others'
+
+    Returns
+    -------
+    DataFrame
+        The DataFrame after join the categories
+    """
+    df = dataframe.copy()
+    if len(categories) == 0:
+        return df
+    df[column] = np.where(
+        pd.isnull(df[column]), 
+        df[column], 
+        df[column].astype(str)
+    ) 
+    join_cat = list(df[column].dropna().unique())
+    join_cat = list_ops(join_cat, categories)
+    df = join_categories(df, column, join_cat, to_category)
+    return df
+
+
 def drop_categories(
     dataframe: DataFrame,
     col_name: str,
     categories: List[str],
 ) -> DataFrame:
     """Drop categories of column
 
@@ -446,15 +485,15 @@
     keep_categories = get_categories_ge(
         df, 
         col_name, 
         by=by,
         value=value,
     )
     all_categories = list(df[col_name].value_counts().index)
-    join_categories_list = Utils.list_difference(
+    join_categories_list = list_ops(
         all_categories, 
         keep_categories
     )
     df = join_categories(
         df, 
         col_name, 
         categories=join_categories_list,
@@ -498,15 +537,15 @@
     
     keep_categories = get_categories_ge(
         df, 
         col_name, 
         by=by,
         value=value,
     )
-    keep_categories = Utils.list_difference(
+    keep_categories = list_ops(
         keep_categories, 
         force_remove
     )
     df_copy = keep_categories(
         df, 
         col_name, 
         keep_categories=keep_categories
```

### Comparing `drtools-1.0.9/src/drtools/data_science/data_load.py` & `drtools-2.0.0/src/drtools/data_science/data_load.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,97 @@
 from typing import Union
 from types import FunctionType
 from pandas.core.frame import DataFrame
 import pandas as pd
 import os
 import joblib
 import pyarrow.parquet as pq
+from enum import Enum
+from drtools.logging import FormatterOptions, Logger
+from drtools.utils import ExpectedRemainingTimeHandle
+
+
+class FileType(Enum):
+    CSV = "csv", ".csv"
+    JSON = "json", ".json"
+    
+    @property
+    def pname(self):
+        return self.value[0]
+    
+    @property
+    def extension(self):
+        return self.value[1]
+
+
+def concat_dir(
+    dir: str, 
+    out_path: str, 
+    verbose: int=100, 
+    file_type: FileType=FileType.CSV,
+    LOGGER: Logger=Logger(
+        formatter_options=FormatterOptions(
+            include_thread_name=True,
+            include_datetime=True,
+            include_level_name=True,
+        ),
+        default_start=False
+    ),
+    ignore_error_logs: bool=True,
+):
+    """Concat all files from directory to single file
+
+    Parameters
+    ----------
+    dir : str
+        The directory path containing files.
+    out_path : str
+        Path so write output file.
+    verbose : int, optional
+        Verbose num, by default 100
+    file_type : FileType, optional
+        Type of files on directory, by default FileType.CSV
+    LOGGER : Log, optional
+        Logger instance, by default Log( formatter_options=FormatterOptions( IncludeThreadName=True, IncludeDate=True, IncludeLevelName=True, ), default_start=False )
+    ignore_error_logs : bool, optional
+        If True, all error logs when writting and skipping header 
+        from files will be ignored, by default True
+
+    Raises
+    ------
+    Exception
+        If the file_type is not supported.
+    """
+    all_paths = list_path_of_all_files_inside_directory(dir)
+    expected_remaining_time = ExpectedRemainingTimeHandle(total=len(all_paths))
+    insert_header = True
+    count = 0
+    total_paths_len = len(all_paths)
+    LOGGER.info('Start concatenating...')
+    if file_type is FileType.CSV:
+        with open(out_path, 'w') as f:
+            for path in all_paths:
+                count += 1            
+                if count % verbose == 0:
+                    LOGGER.debug(f'({(count+1):,}/{total_paths_len:,}) Expected remaining time: {expected_remaining_time.display_time(count-1)}')
+                with open(path, 'r') as f1:
+                    try:
+                        if not insert_header:
+                            next(f1)
+                        insert_header = False
+                        for line in f1:
+                            f.write(line)
+                    except Exception as exc:
+                        if not ignore_error_logs:
+                            LOGGER.error(f'Error {exc} on {path}')
+    elif file_type is FileType.JSON:
+        raise Exception(f"Not implemented.")
+    else:
+        raise Exception(f"File type {file_type} not supported.")
+    LOGGER.info('Start concatenating... Done!')
 
 
 def save_df(
     dataframe: DataFrame,
     path: str,
     overwrite_if_exists: bool=False,
     **kwargs
```

### Comparing `drtools-1.0.9/src/drtools/data_science/plot.py` & `drtools-2.0.0/src/drtools/data_science/plot.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/src/drtools/data_science/resources/main.py` & `drtools-2.0.0/src/drtools/data_science/resources/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 
 from pandas import DataFrame
 import pandas as pd
 import os
 import numpy as np
 from datetime import datetime
 import logging
-from drtools.utils import ValueRestrictions, ValueRestrictionsAsJson
+from drtools.utils import (
+    ValueRestrictions, ValueRestrictionsAsJson
+)
+from drtools.decorators import start_end_log
 from drtools.file_manager import (
     create_directories_of_path, rm_file, 
     list_path_of_all_files_inside_directory
 )
 import drtools.data_science.data_handle as DataHandle
 import drtools.utils as Utils
 from typing import List, Union, Optional, Dict, TypedDict, Any
 from types import FunctionType
-from drtools.logs import Log
+from drtools.logging import Logger
 from drtools.utils import list_ops
 from pathlib import Path
 from pydbml import PyDBML
 from abc import ABC
 import ast
 from drtools.data_science.data_load import read_dir_as_df, read_as_df
 import joblib
@@ -67,40 +70,14 @@
 
 class Config(TypedDict):
     insert_oneFile: bool
     insert_fileExtension: bool
     typeraze_customTreatment: List[TypeColumm]
 
 
-def start_end_log(method):
-    """Decorator to print name of execution method before and 
-    after method execution.
-
-    Parameters
-    ----------
-    method : str
-        The method name that will be executed.
-    """
-    def decorator(f):
-        def wrapper(self, *args, **kwargs):
-            if self.LOGGER is not None:
-                self.LOGGER.debug(f'Executing {method}()...')
-                
-            # execution
-            response = f(self, *args, **kwargs)
-            
-            if self.LOGGER is not None:
-                self.LOGGER.debug(f'Executing {method}()... Done!')
-                
-            return response
-        wrapper.__doc__ = f.__doc__
-        return wrapper
-    return decorator
-
-
 def filter_categorical(
     df: DataFrame,
     col: str,
     conditions: dict
 ) -> DataFrame:
     """Filter categorical data based on conditions.
 
@@ -204,15 +181,15 @@
     dataframe: DataFrame,
     features: List[SimpleFeature],
     dtypes: List[str]=None,
     ignore_dtypes: List[str]=[],
     custom_treatment: List[TypeColumm]=[],
     utc: Union[bool, None]=None,
     to_numeric: bool=False,
-    LOGGER: Log=None,
+    LOGGER: Logger=None,
     **kwargs
 ) -> DataFrame:
     """Type database columns.
 
     Parameters
     ----------
     dataframe : DataFrame
@@ -229,16 +206,16 @@
         can be specified here, by default []
     utc : Union[bool, None], optional
         If True, apply pd.to_datetime with utc=True, 
         if False, apply with False, by default None.
     to_numeric : bool, optional
         If True, apply pd.to_numeric before type, 
         if False, do not apply, by default False
-    LOGGER : Log, optional
-        The Log to verbose, by default None
+    LOGGER : Logger, optional
+        The Logger to verbose, by default None
 
     Returns
     -------
     DataFrame
         The typed DataFrame
 
     Raises
@@ -430,24 +407,24 @@
     - filter()
     - typeraze()
     """
     
     def __init__(
         self,
         model_catalogue_single: ModelCatalogueSingle,
-  		LOGGER: Log=None,
+  		LOGGER: Logger=None,
         chained_assignment_log: bool=False
     ) -> None:
         """Init Model instance.
 
         Parameters
         ----------
         model_catalogue_single : ModelCatalogueSingle
             The model definitions.
-        LOGGER : Log, optional
+        LOGGER : Logger, optional
             The LOGGER instance to handle logs 
             , by default None
         chained_assignment_log : bool, optional
             If False, put pandas chained assignment equals None, 
             If True, do not change anything, by default False.
         """
         for k in model_catalogue_single:
@@ -495,16 +472,15 @@
 
         Returns
         -------
         str
             Model name combining id, algorithm nickname, model name 
             and model version.
         """
-        # return f'{self.id}-{self.algorithm}_{self.name}_{self.version}'
-        return f'{self.id}-{self.algorithm}'
+        return f'{self.name}-{self.version}'
     
     # @start_end_log('cols_correct_order')        
     def cols_correct_order(
         self
     ) -> List[str]:
         """Returns list of all cols of model, including 
         extra columns, in correct order.
@@ -549,43 +525,43 @@
 
         Raises
         ------
         Exception
             If model algorithm is invalid
         """
         
-        self.LOGGER.info(f'Loading model {self.get_model_name()}...')        
+        self.LOGGER.debug(f'Loading model {self.get_model_name()}...')        
         model = None        
-        if self.algorithm == 'lgbm':
+        if self.model_algorithm == 'LightGBM':
             import lightgbm as lgb
             model = lgb.Booster(model_file=model_file_path, *args, **kwargs)
-        elif self.algorithm == 'NN':
+        elif self.model_algorithm == 'NeuralNetworks':
             from tensorflow import keras
             model = keras.models.load_model(model_file_path, *args, **kwargs)
         else:
-            raise Exception(f'Algorithm {self.algorithm} is invalid.')        
-        self.LOGGER.info(f'Loading model {self.get_model_name()}... Done!')        
+            raise Exception(f'Algorithm {self.model_algorithm} is invalid.')        
+        self.LOGGER.debug(f'Loading model {self.get_model_name()}... Done!')        
         return model
     
     @start_end_log('save_model')
     def save_model(
         self,
         model_instance: Any,
-        project_root_path: str,
+        path: str,
         *args,
         **kwargs
     ) -> None:
         """Save model with path.
 
         Parameters
         ----------
         model_instance : Any
             Instance of desired model to save. 
-        project_root_path : str
-            The root path of project.
+        path : str
+            The path to save model.
         args : Tuple, optional
             All args inputs will be passed to save model 
             function, by default ().
         kwargs : Dict, optional
             All args inputs will be passed to save model 
             function, by default {}.
 
@@ -595,25 +571,25 @@
             None is returned.
 
         Raises
         ------
         Exception
             If model algorithm is invalid
         """
-        self.LOGGER.info(f'Saving model {self.get_model_name()}...')        
-        save_path = f'{project_root_path}/models/{self.get_model_name()}/model/{self.get_model_name()}'        
-        if self.algorithm == 'lgbm':
-            create_directories_of_path(save_path)
-            model_instance.save_model(filename=save_path, *args, **kwargs)
-        elif self.algorithm == 'NN':
-            create_directories_of_path(save_path)
-            model_instance.save(save_path, *args, **kwargs)
+        self.LOGGER.debug(f'Saving model {self.get_model_name()}...')        
+        # save_path = f'{project_root_path}/models/{self.get_model_name()}/model/{self.get_model_name()}'        
+        if self.model_algorithm == 'LightGBM':
+            create_directories_of_path(path)
+            model_instance.save_model(filename=path, *args, **kwargs)
+        elif self.model_algorithm == 'NeuralNetworks':
+            create_directories_of_path(path)
+            model_instance.save(path, *args, **kwargs)
         else:
-            raise Exception(f'Algorithm {self.algorithm} is invalid.')        
-        self.LOGGER.info(f'Saving model {self.get_model_name()}... Done!')
+            raise Exception(f'Algorithm {self.model_algorithm} is invalid.')        
+        self.LOGGER.debug(f'Saving model {self.get_model_name()}... Done!')
     
     @start_end_log('train')
     def train(
         self,
         model_instance: Any,
         *args,
         **kwargs
@@ -637,26 +613,26 @@
             Returns different data for each algorithm. 
 
         Raises
         ------
         Exception
             If model algorithm is invalid
         """
-        self.LOGGER.info(f'Training model {self.get_model_name()}...')                
-        if self.algorithm == 'lgbm':
+        self.LOGGER.debug(f'Training model {self.get_model_name()}...')                
+        if self.model_algorithm == 'LightGBM':
             import lightgbm as lgb
             model_instance = lgb.train(*args, **kwargs)
-            self.LOGGER.info(f'Training model {self.get_model_name()}... Done!')            
+            self.LOGGER.debug(f'Training model {self.get_model_name()}... Done!')            
             return model_instance
-        elif self.algorithm == 'NN':
+        elif self.model_algorithm == 'NeuralNetworks':
             history = model_instance.fit(*args, **kwargs)
-            self.LOGGER.info(f'Training model {self.get_model_name()}... Done!')            
+            self.LOGGER.debug(f'Training model {self.get_model_name()}... Done!')            
             return model_instance, history
         else:
-            raise Exception(f'Algorithm {self.algorithm} is invalid.')
+            raise Exception(f'Algorithm {self.model_algorithm} is invalid.')
     
     @start_end_log('predict')
     def predict(
         self,
         model_file_path: str,
         X: Any,
         *args,
@@ -683,24 +659,24 @@
             Returns different data for each algorithm. 
 
         Raises
         ------
         Exception
             If model algorithm is invalid
         """    
-        self.LOGGER.info(f'Predicting data for model {self.get_model_name()}...')  
+        self.LOGGER.debug(f'Predicting data for model {self.get_model_name()}...')  
         model_instance = self.load_model(model_file_path)
-        if self.algorithm == 'lgbm':
+        if self.model_algorithm == 'LightGBM':
             y_pred = model_instance.predict(X, *args, **kwargs)
-        elif self.algorithm == 'NN':
+        elif self.model_algorithm == 'NeuralNetworks':
             y_pred = model_instance.predict(X, *args, **kwargs)
             y_pred = y_pred.reshape(1, -1)[0]
         else:
-            raise Exception(f'Algorithm {self.algorithm} is invalid.')        
-        self.LOGGER.info(f'Predicting data for model {self.get_model_name()}... Done!')        
+            raise Exception(f'Algorithm {self.model_algorithm} is invalid.')        
+        self.LOGGER.debug(f'Predicting data for model {self.get_model_name()}... Done!')        
         return y_pred
     
     @start_end_log('one_hot_encoding')
     def one_hot_encoding(
         self,
         dataframe: DataFrame,
         encode_cols: List[str]
@@ -1066,15 +1042,15 @@
         
         if custom is not None:
             features = [
                 {'name': feature['name'], 'type': feature['type']}
                 for feature in custom
             ]
         df = dataframe.copy()
-        df = typeraze(dataframe=df, features=features, LOGGER=self.LOGGER, **kwargs)        
+        df = typeraze(dataframe=df, features=features, LOGGER=self.LOGGER, **kwargs)
         return df
 
 
 class Database(ABC):
     """Abstract class to handle database loading based on default 
     infrastructure.
     
@@ -1095,25 +1071,25 @@
         'typeraze_customTreatment': []
     })
     
     def __init__(
         self,
         database_dbml_path: str,
         database_root_path: str,
-  		LOGGER: Log=None,
+  		LOGGER: Logger=None,
     ) -> None:
         """Init Database instance.
 
         Parameters
         ----------
         database_dbml_path : str
             Path to .dbml database documentation.
         database_root_path : str
             Path to root of database.
-        LOGGER : Log, optional
+        LOGGER : Logger, optional
             The LOGGER instance to handle logs 
             , by default None
         """
         assert hasattr(self, 'SCHEMA')
         assert hasattr(self, 'TABLE')  
         self.database_dbml_path = database_dbml_path
         self.database_root_path = database_root_path
@@ -1265,15 +1241,15 @@
             , by default {}.
 
         Returns
         -------
         DataFrame
             The local database data as DataFrame
         """
-        self.LOGGER.info(f'Loading {self.db_name()}...')
+        self.LOGGER.debug(f'Loading {self.db_name()}...')
         
         df = read_dir_as_df(
             Utils.join_path(
                 self.database_root_path, self.SCHEMA, self.TABLE
             ),
             **kwargs
         )
@@ -1290,15 +1266,15 @@
                 verbosity=verbosity,
                 **kwargs
             )
         
         cols_correct_order = list_ops(self.get_col_names(), df.columns, ops='intersection')            
         df = df.loc[:, cols_correct_order]
             
-        self.LOGGER.info(f'Loading {self.db_name()}... Done!')
+        self.LOGGER.debug(f'Loading {self.db_name()}... Done!')
             
         return df
     
     @start_end_log('_save_data')
     def _save_data(
         self,
         dataframe: DataFrame,
@@ -1384,15 +1360,15 @@
 
         Returns
         -------
         List[int]
             The inserted ids.
         """
         
-        self.LOGGER.info(f'Inserting data on {self.db_name()}...')
+        self.LOGGER.debug(f'Inserting data on {self.db_name()}...')
         
         df = dataframe.copy()
         
         if df.shape[0] == 0:
             return []
         
         already_on_db = self.load_db_as_df(
@@ -1435,15 +1411,15 @@
                 rm_file(
                     path,
                     ignore_if_path_not_exists=True
                 )
         else:
             self._save_data(df, filename)
         
-        self.LOGGER.info(f'Inserting data on {self.db_name()}... Done!')
+        self.LOGGER.debug(f'Inserting data on {self.db_name()}... Done!')
         
         return sorted(inserted_ids)
     
     def insert_if_not_exists(
         self,
         dataframe: DataFrame
     ) -> List[int]:
@@ -1463,15 +1439,15 @@
         
         
         df = dataframe.copy()
         
         if df.shape[0] == 0:
             return []        
         
-        self.LOGGER.info(f'Filtering already inserted...')
+        self.LOGGER.debug(f'Filtering already inserted...')
         original_shape = df.shape
         necessary_cols = list_ops(
             self.get_col_names(),
             ['id', 'created_at', 'updated_at']
         )
         df = df.loc[:, necessary_cols]
         df['md5_of_row'] = df.apply(lambda x: joblib.hash(x.values), axis=1)
@@ -1486,17 +1462,17 @@
         intersection_data['md5_of_row'] = intersection_data.apply(
             lambda x: joblib.hash(x.values), axis=1
         )
         df = df[~df.md5_of_row.isin(intersection_data.md5_of_row.values)]
         df = df.drop('md5_of_row', axis=1)
         del intersection_data
         final_shape = df.shape
-        self.LOGGER.info(f'{(original_shape[0] - final_shape[0]):,} rows was already inserted.')
-        self.LOGGER.info(f'{final_shape[0]:,} rows to insert.')
-        self.LOGGER.info(f'Filtering already inserted... Done!')
+        self.LOGGER.debug(f'{(original_shape[0] - final_shape[0]):,} rows was already inserted.')
+        self.LOGGER.debug(f'{final_shape[0]:,} rows to insert.')
+        self.LOGGER.debug(f'Filtering already inserted... Done!')
         
         # return df
         
         inserted_ids = self.insert(
             dataframe=df
         )
         
@@ -1576,15 +1552,15 @@
         if 'id' not in intersect_cols:
             raise Exception('Column id must be on DataFrame.')
         
         if df.id.values.shape[0] != df.id.unique().shape[0]:
             seen = set()
             dupes = [x for x in df.id.values if x in seen or seen.add(x)]
             dupes_df = df[df.id.isin(dupes)]
-            self.LOGGER.info(dupes_df)
+            self.LOGGER.debug(dupes_df)
             raise Exception(f'There are duplicated ids on received data. Duplicate ids: {dupes}')
         
         data_path = Utils.join_path(
             self.database_root_path, self.SCHEMA, self.TABLE
         )
         paths = list_path_of_all_files_inside_directory(data_path)
```

### Comparing `drtools-1.0.9/src/drtools/data_science/statistical_test.py` & `drtools-2.0.0/src/drtools/data_science/statistical_test.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/src/drtools/data_science/time_series.py` & `drtools-2.0.0/src/drtools/data_science/time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from typing import List, Union
 import drtools.utils as Utils
 from pandas.core.frame import DataFrame
 import pandas as pd
 import math
 import numpy as np
-from drtools.logs import Log
+from drtools.logging import Logger
 
 
 OneDimension = int
 TwoDimension = int
 Axis0 = int
 Axis1 = int
 
@@ -112,15 +112,15 @@
     ignore_cols: List[str]=[],
     data_leak_cols: List[str]=[],
     immutable_cols: List[str]=[],
     light: bool=False,
     dtype: bool=True,
     chunksize: int=1,
     return_numpy: bool=False,
-    LOGGER: Log=None
+    LOGGER: Logger=None
 ) -> DataFrame:
     """Generate data for time series prediction.py
 
     Parameters
     ----------
     dataframe : DataFrame
         DataFrame containing data that will be transformed 
@@ -151,15 +151,15 @@
         as DataFrame, this can safe memo usage, by default False.
     dtype : bool, optional
         If True, type cols after transformations.
         If False, will not type cols after transformations 
         , by default True.
     chunksize : int, optional
         Process by chunks, by default 1.
-    LOGGER : Log, optional
+    LOGGER : Logger, optional
         Logging object to debug execution, 
         by default None.
     
     Returns
     -------
     DataFrame
         The DataFrame after transform the data into Time Series.
```

### Comparing `drtools-1.0.9/src/drtools/database/utils.py` & `drtools-2.0.0/src/drtools/database/utils.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/src/drtools/file_manager.py` & `drtools-2.0.0/src/drtools/file_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 This module was created to manage files and directories
 of system.
 
 """
 
 import os
 from typing import List
-import drtools.utils as Utils
+from drtools.utils import (
+    get_os_name,
+    join_path
+)
 import json
 import gzip
 
 
 def path_exist(
     path: str
 ) -> bool: 
@@ -41,17 +44,17 @@
         Path to be splited
 
     Returns
     -------
     List[str]
         List with pieces of path.
     """
-    if Utils.get_os_name() == "Windows": return path.split("\\")
-    elif Utils.get_os_name() == "Linux": return path.split("/")
-    elif Utils.get_os_name() == "Darwin": return path.split("\\")
+    if get_os_name() == "Windows": return path.split("\\")
+    elif get_os_name() == "Linux": return path.split("/")
+    elif get_os_name() == "Darwin": return path.split("\\")
 
 
 def move_file(
     current_path: str,
     destination_path: str,
 ) -> None:
     """Move file handling when file already exists.
@@ -104,43 +107,48 @@
         the names presented on this list, by default []
 
     Returns
     -------
     List
         List of files path inside parent path directory.
     """
-    filesPathArr = []
+    files_path_arr = []
     ignore_cuz_content_name_have_some_of_the_words = False
-    for contentName in content_arr:
+    for content_name in content_arr:
+        
+        content_path = f'{parent_path}/{content_name}'
+        
         ignore_words_len = len(ignore_if_contain_some_of_the_words)
         for index1, word in enumerate(ignore_if_contain_some_of_the_words):
-            if word in contentName:
+            if word in content_name:
                 ignore_cuz_content_name_have_some_of_the_words = True
                 break
             elif index1 == ignore_words_len - 1:
                 ignore_cuz_content_name_have_some_of_the_words = False
-        if len(contentName.split(".")) > 1:
-            if contentName not in ignore_files \
+                
+        if os.path.isfile(content_path):
+            if content_name not in ignore_files \
             and not ignore_cuz_content_name_have_some_of_the_words:
-                filesPathArr.append(
-                    Utils.join_path(parent_path, contentName)
+                files_path_arr.append(
+                    join_path(parent_path, content_name)
                 )
-        elif contentName not in ignore_folders \
+                
+        elif content_name not in ignore_folders \
         and not ignore_cuz_content_name_have_some_of_the_words:
-            nextParentPath = Utils.join_path(parent_path, contentName)
-            nextContentArr = os.listdir(nextParentPath)
-            filesPathArr = filesPathArr \
+            next_parent_path = join_path(parent_path, content_name)
+            next_content_arr = os.listdir(next_parent_path)
+            files_path_arr = files_path_arr \
                 + get_files_path(
-                    nextParentPath, 
-                    nextContentArr, 
+                    next_parent_path, 
+                    next_content_arr, 
                     ignore_files, 
                     ignore_folders, 
                     ignore_if_contain_some_of_the_words
                 )
-    return filesPathArr
+    return files_path_arr
 
 
 def list_path_of_all_files_inside_directory(
     root_directory_path: str,
     ignore_files: List[str]=[],
     ignore_folders: List[str]=[],
     ignore_if_contain_some_of_the_words: List[str]=[]
@@ -167,19 +175,19 @@
     try:
       dataDirectoryContent = os.listdir(root_directory_path)
     except:
       dataDirectoryContent = []
     itemsPath = []
     if len(dataDirectoryContent) > 0:
       itemsPath = get_files_path(
-            root_directory_path, 
-            dataDirectoryContent, 
-            ignore_files, 
-            ignore_folders, 
-            ignore_if_contain_some_of_the_words
+            parent_path=root_directory_path, 
+            content_arr=dataDirectoryContent, 
+            ignore_files=ignore_files, 
+            ignore_folders=ignore_folders, 
+            ignore_if_contain_some_of_the_words=ignore_if_contain_some_of_the_words
         )
     return itemsPath
 
 
 def search_by_name_on_directory(
     name: str, 
     directory: str,
@@ -217,35 +225,35 @@
     -----
     None
         None is returned
     """
     
     split_path = None
     
-    if Utils.get_os_name() == "Windows": 
+    if get_os_name() == "Windows": 
         split_path = path.split("\\")
-    elif Utils.get_os_name() == "Linux": 
+    elif get_os_name() == "Linux": 
         split_path = path.split("/")
-    elif Utils.get_os_name() == "Darwin": 
+    elif get_os_name() == "Darwin": 
         split_path = path.split("\\")
         
     temp_path = None
     
     for index, env_path in enumerate(split_path):
         if not env_path: 
             continue
         if len(env_path.split(".")) > 1 and index == len(split_path) - 1: 
             break
         if temp_path == None: 
-            if Utils.get_os_name() == "Windows": 
+            if get_os_name() == "Windows": 
                 temp_path = env_path + '\\'
                 continue
-            elif Utils.get_os_name() == "Linux": 
+            elif get_os_name() == "Linux": 
                 temp_path = "/"
-        temp_path = Utils.join_path(temp_path, env_path)
+        temp_path = join_path(temp_path, env_path)
         if not os.path.exists(temp_path): 
             try:
                 os.makedirs(temp_path, exist_ok=True)
             except Exception as e:
                 template = "An exception of type {0} occurred. Arguments:\n{1!r}"
                 message = template.format(type(e).__name__, e.args)
                 print("Error: " + str(e))
```

### Comparing `drtools-1.0.9/src/drtools/geo/common.py` & `drtools-2.0.0/src/drtools/geo/common.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/src/drtools/scrapping/authentication.py` & `drtools-2.0.0/src/drtools/scrapping/authentication.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/src/drtools/scrapping/config.py` & `drtools-2.0.0/src/drtools/scrapping/config.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/src/drtools/scrapping/interaction.py` & `drtools-2.0.0/src/drtools/scrapping/interaction.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.9/src/drtools.egg-info/PKG-INFO` & `drtools-2.0.0/src/drtools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drtools
-Version: 1.0.9
+Version: 2.0.0
 Summary: Kit of MY useful tools.
 Home-page: https://github.com/andreylcj/drtools
 Author: Andrey Malheiros
 Author-email: example@email.com
 Project-URL: repository, https://github.com/andreylcj/dr_tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drtools-1.0.9/src/drtools.egg-info/SOURCES.txt` & `drtools-2.0.0/src/drtools.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,48 +2,38 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/drtools/__init__.py
 src/drtools/decorators.py
 src/drtools/file_manager.py
-src/drtools/logs.py
+src/drtools/logging.py
+src/drtools/retry.py
 src/drtools/thread_pool_executor.py
 src/drtools/utils.py
 src/drtools.egg-info/PKG-INFO
 src/drtools.egg-info/SOURCES.txt
 src/drtools.egg-info/dependency_links.txt
 src/drtools.egg-info/top_level.txt
 src/drtools/data_science/__init__.py
-src/drtools/data_science/beyond_linearity.py
-src/drtools/data_science/classification.py
 src/drtools/data_science/data_handle.py
 src/drtools/data_science/data_load.py
-src/drtools/data_science/multiple_testing.py
+src/drtools/data_science/features_handle.py
+src/drtools/data_science/general.py
+src/drtools/data_science/model_handling.py
 src/drtools/data_science/plot.py
 src/drtools/data_science/statistical_test.py
-src/drtools/data_science/survival_analysis.py
-src/drtools/data_science/test_error_estimation.py
 src/drtools/data_science/time_series.py
-src/drtools/data_science/transformation.py
-src/drtools/data_science/tree_based.py
-src/drtools/data_science/unsupervised_learning.py
-src/drtools/data_science/model_selection/__init__.py
-src/drtools/data_science/model_selection/dimension_reduction.py
-src/drtools/data_science/model_selection/shrinkage.py
-src/drtools/data_science/model_selection/subset_selection.py
-src/drtools/data_science/resampling/__init__.py
-src/drtools/data_science/resampling/bootstrap.py
-src/drtools/data_science/resampling/cross_validation.py
 src/drtools/data_science/resources/__init__.py
 src/drtools/data_science/resources/main.py
 src/drtools/database/__init__.py
 src/drtools/database/utils.py
 src/drtools/database/connection/__init__.py
 src/drtools/database/connection/postgresql.py
+src/drtools/database/connection/resources.py
 src/drtools/geo/__init__.py
 src/drtools/geo/common.py
 src/drtools/scrapping/__init__.py
 src/drtools/scrapping/authentication.py
 src/drtools/scrapping/config.py
 src/drtools/scrapping/interaction.py
 tests/test_utils.py
```

### Comparing `drtools-1.0.9/tests/test_utils.py` & `drtools-2.0.0/tests/test_utils.py`

 * *Files identical despite different names*

