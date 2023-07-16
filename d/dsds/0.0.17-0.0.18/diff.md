# Comparing `tmp/dsds-0.0.17.tar.gz` & `tmp/dsds-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.17.tar", last modified: Sun Jul  9 00:37:04 2023, max compression
+gzip compressed data, was "dsds-0.0.18.tar", last modified: Sun Jul 16 03:54:37 2023, max compression
```

## Comparing `dsds-0.0.17.tar` & `dsds-0.0.18.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.934278 dsds-0.0.17/
--rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.17/LICENSE
--rw-rw-rw-   0        0        0     5850 2023-07-09 00:37:04.934278 dsds-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     3478 2023-07-09 00:29:00.000000 dsds-0.0.17/README.md
--rw-rw-rw-   0        0        0     1398 2023-07-09 00:36:45.000000 dsds-0.0.17/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 00:37:04.934278 dsds-0.0.17/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.896269 dsds-0.0.17/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.914273 dsds-0.0.17/src/dsds/
--rw-rw-rw-   0        0        0       87 2023-07-09 00:36:50.000000 dsds-0.0.17/src/dsds/__init__.py
--rw-rw-rw-   0        0        0     4937 2023-07-09 00:31:32.000000 dsds-0.0.17/src/dsds/blueprint.py
--rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.17/src/dsds/eda_text.py
--rw-rw-rw-   0        0        0    31557 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/fs.py
--rw-rw-rw-   0        0        0     7916 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/metrics.py
--rw-rw-rw-   0        0        0    27272 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/prescreen.py
--rw-rw-rw-   0        0        0     9095 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/sample.py
--rw-rw-rw-   0        0        0    28827 2023-07-09 00:31:23.000000 dsds-0.0.17/src/dsds/transform.py
--rw-rw-rw-   0        0        0     1771 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/type_alias.py
--rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.932278 dsds-0.0.17/src/dsds.egg-info/
--rw-rw-rw-   0        0        0     5850 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.198434 dsds-0.0.18/
+-rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.18/LICENSE
+-rw-rw-rw-   0        0        0     6759 2023-07-16 03:54:37.198434 dsds-0.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0     4387 2023-07-11 16:38:19.000000 dsds-0.0.18/README.md
+-rw-rw-rw-   0        0        0     1398 2023-07-16 03:51:44.000000 dsds-0.0.18/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 03:54:37.199434 dsds-0.0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.161425 dsds-0.0.18/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.176429 dsds-0.0.18/src/dsds/
+-rw-rw-rw-   0        0        0       87 2023-07-16 03:36:00.000000 dsds-0.0.18/src/dsds/__init__.py
+-rw-rw-rw-   0        0        0     6875 2023-07-13 01:01:02.000000 dsds-0.0.18/src/dsds/blueprint.py
+-rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.18/src/dsds/eda_text.py
+-rw-rw-rw-   0        0        0    32902 2023-07-16 03:51:24.000000 dsds-0.0.18/src/dsds/fs.py
+-rw-rw-rw-   0        0        0     9077 2023-07-13 03:33:56.000000 dsds-0.0.18/src/dsds/metrics.py
+-rw-rw-rw-   0        0        0    29200 2023-07-14 19:43:13.000000 dsds-0.0.18/src/dsds/prescreen.py
+-rw-rw-rw-   0        0        0    15707 2023-07-14 17:19:08.000000 dsds-0.0.18/src/dsds/sample.py
+-rw-rw-rw-   0        0        0    43353 2023-07-15 03:30:38.000000 dsds-0.0.18/src/dsds/transform.py
+-rw-rw-rw-   0        0        0     2686 2023-07-14 19:40:24.000000 dsds-0.0.18/src/dsds/type_alias.py
+-rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.18/src/dsds/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.197433 dsds-0.0.18/src/dsds.egg-info/
+-rw-rw-rw-   0        0        0     6759 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/top_level.txt
```

### Comparing `dsds-0.0.17/LICENSE` & `dsds-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `dsds-0.0.17/PKG-INFO` & `dsds-0.0.18/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.17
+Version: 0.0.18
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,16 +74,15 @@
     , constant_removal
     , date_removal
     , non_numeric_removal
     , get_unique_count
     , get_string_cols
     , suggest_normal
     , discrete_inferral
-)
-
+) # and a lot more!
 
 ```
 
 Functional Pipeline Interface which supports both Eager and LazyFrames! And it can be pickled and load back and reapplied! See more in the examples on github.
 
 ```python
 from dsds.prescreen import *
@@ -113,12 +112,30 @@
 
 pip install dsds[all]
 
 Note: scikit-learn, lightgbm, xgboost are needed for full functionalities. 
 
 # Why DSDS?
 
-I choose DarkSide because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
+(1) Fast and furious
+
+(2) Simple, single-purpose, clean, optimized and fully typed functions
+
+(3) Easy to extend
+
+(4) Supports Polars LazyFrame, and therefore query optimizations in pipeline.
+
+(5) No boilerplate
+
+# Why the name DSDS?
+
+I choose the name Dark Side of Data Science because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
 
 # Why is this package dependent on Sklearn?
 
-You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives. 
+You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
+
+# Why not write more functionalities in Rust?
+
+Yes. I will. I am not confident enough with my Rust skill at the moment. I am slowly learning more Rust and hopefully we can delegate more heavy work to Rust. The immediate benefit of using more Rust will be (1) slightly more memory efficient, and (2) slightly faster. I do not expect huge speed boost because most code are written in Polars already. There are some cases when a lot of Python stuff is added (lists and for loops, etc.). But we definitely need to evaluate the gain by using Rust more carefully in the future.
+
+See CONTRIBUTING.md for my contact info.
```

### Comparing `dsds-0.0.17/README.md` & `dsds-0.0.18/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     , constant_removal
     , date_removal
     , non_numeric_removal
     , get_unique_count
     , get_string_cols
     , suggest_normal
     , discrete_inferral
-)
-
+) # and a lot more!
 
 ```
 
 Functional Pipeline Interface which supports both Eager and LazyFrames! And it can be pickled and load back and reapplied! See more in the examples on github.
 
 ```python
 from dsds.prescreen import *
@@ -65,12 +64,30 @@
 
 pip install dsds[all]
 
 Note: scikit-learn, lightgbm, xgboost are needed for full functionalities. 
 
 # Why DSDS?
 
-I choose DarkSide because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
+(1) Fast and furious
+
+(2) Simple, single-purpose, clean, optimized and fully typed functions
+
+(3) Easy to extend
+
+(4) Supports Polars LazyFrame, and therefore query optimizations in pipeline.
+
+(5) No boilerplate
+
+# Why the name DSDS?
+
+I choose the name Dark Side of Data Science because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
 
 # Why is this package dependent on Sklearn?
 
-You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives. 
+You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
+
+# Why not write more functionalities in Rust?
+
+Yes. I will. I am not confident enough with my Rust skill at the moment. I am slowly learning more Rust and hopefully we can delegate more heavy work to Rust. The immediate benefit of using more Rust will be (1) slightly more memory efficient, and (2) slightly faster. I do not expect huge speed boost because most code are written in Polars already. There are some cases when a lot of Python stuff is added (lists and for loops, etc.). But we definitely need to evaluate the gain by using Rust more carefully in the future.
+
+See CONTRIBUTING.md for my contact info.
```

### Comparing `dsds-0.0.17/pyproject.toml` & `dsds-0.0.18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "dsds"
-version = "0.0.17"
+version = "0.0.18"
 requires-python = ">=3.9"
 readme = "README.md"
 description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
 authors = [
     {name = "Tianren Qin", email = "tq9695@gmail.com"}
 ]
 license = {file = "LICENSE"}
```

### Comparing `dsds-0.0.17/src/dsds/eda_text.py` & `dsds-0.0.18/src/dsds/eda_text.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.17/src/dsds/fs.py` & `dsds-0.0.18/src/dsds/fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .prescreen import (
     discrete_inferral
     , check_binary_target
     , get_numeric_cols
     , get_unique_count
     , get_string_cols
+    , type_checker
 )
 
 from .type_alias import (
     PolarsFrame
     , MRMRStrategy
     , BinaryModels
     , CPU_COUNT
     , clean_strategy_str
+    , ClassifModel
 )
 from .blueprint import( # Need this for Polars extension to work
     Blueprint
 )
 from .sample import (
     train_test_split
 )
@@ -25,65 +27,27 @@
 )
 import polars as pl
 import numpy as np
 from typing import Any, Optional, Tuple
 from scipy.spatial import KDTree
 from scipy.special import fdtrc, psi
 from concurrent.futures import ThreadPoolExecutor, as_completed
+import logging
 from tqdm import tqdm
 import math
 from itertools import combinations
 
-def _conditional_entropy(
-    df:pl.DataFrame
-    , target:str
-    , predictive:str
-) -> Tuple[str, float]:
-
-    cond_entropy = df.groupby((target, predictive)).agg(
-        pl.count()
-    ).with_columns(
-        (pl.col("count").sum().over(predictive) / len(df)).alias("prob(predictive)"),
-        (pl.col("count") / pl.col("count").sum()).alias("prob(target,predictive)")
-    ).select(
-        (-((pl.col("prob(target,predictive)")/pl.col("prob(predictive)")).log() 
-           * pl.col("prob(target,predictive)")).sum()) # This is the conditional entropy.
-    ).row(0)[0]
-
-    return (predictive, cond_entropy)
+logger = logging.getLogger(__name__)
 
-# !!!NEED REVIEW FOR CORRECTNESS
 def discrete_ig(
     df:pl.DataFrame
     , target:str
     , cols:Optional[list[str]] = None
-    , n_threads:int = CPU_COUNT
 ) -> pl.DataFrame:
-    '''The entropy here is "discrete entropy".
-
-        Computes the information gain: Entropy(target) - Conditional_Entropy(target|c), where c is a column in 
-        discrete_cols. For more information, please take a look at https://en.wikipedia.org/wiki/Entropy_(information_theory)
-
-        Information gain defined in this way suffers from high cardinality (high uniqueness), and therefore a weighted 
-        information gain is provided, weighted by (1 - unique_pct), where unique_pct represents the percentage of unique
-         values in feature.
 
-        Currently this only works for discrete columns. For continuous features vs discrete target, use mutual_info.
-
-        Arguments:
-            df: Eager frame only.
-            target:
-            cols: list of discrete columns. If not provided, they will be inferred.
-            top_k: must be >= 0. If <= 0, the entire DataFrame will be returned.
-            n_threads: 4, 8 ,16 will not make any real difference. But there is a difference between 0 and 4 threads. 
-            
-        Returns:
-            a poalrs dataframe with information gain computed for each categorical column. 
-    '''
-    output = []
     if isinstance(cols, list):
         discretes = cols
     else: # If discrete_cols is not passed, infer it
         discretes = discrete_inferral(df, exclude=[target])
 
     # Compute target entropy. This only needs to be done once.
     target_entropy = df.groupby(target).agg(
@@ -91,30 +55,37 @@
                     ).get_column("prob(target)").entropy()
 
     # Get unique count for selected columns. This is because higher unique percentage may skew information gain
     unique_count = get_unique_count(df.select(discretes)).with_columns(
         (pl.col("n_unique") / len(df)).alias("unique_pct")
     ).rename({"column":"feature"})
 
-    with ThreadPoolExecutor(max_workers=n_threads) as ex: # 10% speed gain ? Need to retest this..
-        pbar = tqdm(total=len(discretes), desc = "discrete_ig")
-        for f in as_completed(ex.submit(_conditional_entropy, df, target, pred) for pred in discretes):
-            output.append(f.result())
-            pbar.update(1)
-        pbar.close()
+    conditional_entropy = (
+        df.lazy().groupby(target, pred).agg(
+            pl.count()
+        ).with_columns(
+            (pl.col("count").sum().over(pred) / len(df)).alias("prob(predictive)"),
+            (pl.col("count") / pl.col("count").sum()).alias("prob(target,predictive)")
+        ).select(
+            pl.lit(pred, dtype=pl.Utf8).alias("feature"),
+            (-((pl.col("prob(target,predictive)")/pl.col("prob(predictive)")).log() 
+            * pl.col("prob(target,predictive)")).sum()).alias("conditional_entropy") 
+        )
+        for pred in discretes
+    )
 
-    return pl.from_records(output, schema=["feature", "conditional_entropy"])\
+    return pl.concat(conditional_entropy)\
         .with_columns(
             target_entropy = pl.lit(target_entropy),
-            information_gain = pl.lit(target_entropy) - pl.col("conditional_entropy")
+            information_gain = pl.max(pl.lit(target_entropy) - pl.col("conditional_entropy"), 0)
         ).join(unique_count, on="feature")\
         .select("feature", "target_entropy", "conditional_entropy", "unique_pct", "information_gain")\
         .with_columns(
             weighted_information_gain = (1 - pl.col("unique_pct")) * pl.col("information_gain")
-        )
+        ).collect()
 
 discrete_mi = discrete_ig
 
 def discrete_ig_selector(
     df:PolarsFrame
     , target:str
     , top_k:int
@@ -144,55 +115,65 @@
     df:pl.DataFrame
     , target:str
     , conti_cols:list[str]
     , n_neighbors:int=3
     , seed:int=42
     , n_threads:int=CPU_COUNT
 ) -> pl.DataFrame:
-    '''Approximates mutual information (information gain) between the continuous variables and the target.
-
-        This is essentially a "copy-and-paste" of the mutual_info_classif call in sklearn library. 
-        There are a few important distinctions:
+    '''
+    Approximates mutual information (information gain) between the continuous variables and the target. This
+    is essentially the same as sklearn's implementation, except that
 
-        1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors. 
-        2. The use of Scipy enables us to use more cores. 
-        3. There are less "checks" and "safeguards", meaning input data quality is expected to be "good".
-        4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense 
-            matrix X, it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
-        5. This method is based on method described the sources.
+    1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors
+    2. This uses all cores by default
+    3. There are less "checks" and "safeguards", meaning input data quality is expected to be "good".
+    4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense 
+        matrix X, it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
 
-        Arguments:
-            df:
-            conti_cols: 
-            target: list of discrete columns.
-            n_neighbors:
-            random_state: a random seed to generate small noise.
-            n_threads: 
-            
-        Returns:
+    Parameters
+    ----------
+    df
+        An eager dataframe
+    target
+        The target column
+    conti_cols
+        A list of columns with continuous values
+    n_neighbors
+        Number of neighbors. Used in the approximation method provided by the paper
+    seed
+        The random seed used to generate noise, which prevents points to collide and cause difficulty for the
+        nearest neighbor method used in the approximation
+    n_threads
+        The number of threads used in scipy's Kdtree
 
-        Sources:
-            (1). B. C. Ross “Mutual Information between Discrete and Continuous Data Sets”. PLoS ONE 9(2), 2014.\n
-            (2). A. Kraskov, H. Stogbauer and P. Grassberger, “Estimating mutual information”. Phys. Rev. E 69, 2004.
-            
+    Sources
+    -------
+        (1). B. C. Ross “Mutual Information between Discrete and Continuous Data Sets”. PLoS ONE 9(2), 2014.\n
+        (2). A. Kraskov, H. Stogbauer and P. Grassberger, “Estimating mutual information”. Phys. Rev. E 69, 2004. 
     '''
     n = len(df)
     rng = np.random.default_rng(seed)
     target_col = df.get_column(target).to_numpy().ravel()
     unique_targets = np.unique(target_col)
     all_masks = {}
     for t in unique_targets:
         all_masks[t] = target_col == t
         if np.sum(all_masks[t]) <= n_neighbors:
             raise ValueError(f"The target class {t} must have more than {n_neighbors} values in the dataset.")        
 
     estimates = []
     psi_n_and_k = psi(n) + psi(n_neighbors)
-    for col in tqdm(conti_cols, desc = "Mutual Info"):
-        c = df.get_column(col).cast(pl.Float64).to_numpy().reshape(-1,1)
+    pbar = tqdm(total = len(conti_cols), desc = "Mutual Info")
+    for col in df.select(conti_cols).get_columns():
+        if col.null_count() > 0:
+            logger.warn(f"Found column {col.name} has null values. It is filled with the mean of the column. "
+                        "It is highly recommended that you impute the column beforehand.")
+            c = col.fill_null(col.mean()).cast(pl.Float64).to_numpy().reshape(-1,1)
+        else:
+            c = col.cast(pl.Float64).to_numpy().reshape(-1,1)
         # Add random noise here because if inpute data is too big, then adding
         # a random matrix of the same size will require a lot of memory upfront.
         c = c + (1e-10 * np.mean(c) * rng.standard_normal(size=c.shape)) 
         radius = np.empty(n)
         label_counts = np.empty(n)
         for t in unique_targets:
             mask = all_masks[t]
@@ -205,26 +186,34 @@
             label_counts[mask] = np.sum(mask)
 
         kd2 = KDTree(data=c, leafsize=40) 
         m_all = kd2.query_ball_point(c, r = radius, return_length=True, workers=n_threads)
         estimates.append(
             max(0, psi_n_and_k - np.mean(psi(label_counts) + psi(m_all)))
         ) # smallest is 0
+        pbar.update(1)
 
+    pbar.close()
     return pl.from_records((conti_cols, estimates), schema=["feature", "estimated_mi"])
 
 # Selectors should always return target
 def mutual_info_selector(
     df:PolarsFrame
     , target:str
     , n_neighbors:int=3
     , seed:int=42
     , n_threads:int=CPU_COUNT
     , top_k:int = 50
 ) -> PolarsFrame:
+    '''
+    A selector based on the mutual_info feature selection method.
+
+    This 
+    
+    '''
     
     is_lazy = isinstance(df, pl.LazyFrame)
     if is_lazy:
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
@@ -511,14 +500,16 @@
     df:PolarsFrame
     , target:str
     , top_k:int
     , strategy:MRMRStrategy = "fscore"
     , params:Optional[dict[str,Any]] = None
     , low_memory:bool=False
 ) -> PolarsFrame:
+    '''
+    '''
 
     is_lazy = isinstance(df, pl.LazyFrame)
     if is_lazy:
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
@@ -599,14 +590,17 @@
     df:PolarsFrame
     , target:str
     , top_k:int 
     , strategy:MRMRStrategy = "fscore"
     , corr_threshold:float = 0.7
     , params:Optional[dict[str,Any]] = None
 ) -> PolarsFrame:
+    '''
+    Performs knock out MRMR
+    '''
 
     is_lazy = isinstance(df, pl.LazyFrame)
     if isinstance(df, pl.LazyFrame):
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
@@ -630,33 +624,41 @@
     df:PolarsFrame
     , target:str
     , cols:Optional[list[str]]=None
     , min_count:float = 1.
     , check_binary:bool = True
 ) -> pl.DataFrame:
     '''
-        Arguments:
-            df: ..
-            target: ..
-            cols: a list of string or highly discrete numeric columns. Currently woe_iv for continuous values
-            is not implemenented. If not provided, it will use only string columns.
-            min_count: a regularization term that prevents ln(0). This is the same as 
-            category_encoders package's regularization parameter.
-            check_binary: whether to check if target is binary or not
+    Computes information values for categorical variables. Notice that by using binning methods provided, you can turn
+    numerical values into categorical bins.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars Dataframe
+    target
+        The target column
+    cols
+        If not provided, will use all string columns
+    min_count
+        A regularization term that prevents ln(0). This is the same as category_encoders package's 
+        regularization parameter.
+    check_binary
+        Whether to check if target is binary or not
     '''
     if isinstance(cols, list):
+        _ = type_checker(df, cols, "string", "woe_iv_cat")
         input_cols = cols
     else:
         input_cols = get_string_cols(df)
 
     if check_binary:
         if not check_binary_target(df, target):
             raise ValueError("Target is not binary or not properly encoded.")
 
-    # No tqdm then..
     results = (
         df.lazy().groupby(s).agg(
             ev = pl.col(target).sum()
             , nonev = (pl.lit(1) - pl.col(target)).sum()
         ).with_columns(
             ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
             , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
@@ -669,144 +671,215 @@
             , information_value = ((pl.col("ev_rate")-pl.col("nonev_rate")) * pl.col("woe")).sum()
         )
         for s in input_cols
     )
     return pl.concat(results).collect()
 
 def _binary_model_init(
-    model:BinaryModels
+    model_str:BinaryModels
     , params: dict[str, Any]
-):
+) -> ClassifModel:
+    '''
+    Creates the binary classification model given by the model_str and the params dict
+    '''
     if "n_jobs" not in params:
         params["n_jobs"] = -1
 
-    if model in ("logistic", "lr"):
+    if model_str in ("logistic", "lr"):
         from sklearn.linear_model import LogisticRegression
         model = LogisticRegression(**params)
-    elif model in ("rf", "random_forest"):
+    elif model_str in ("rf", "random_forest"):
         from sklearn.ensemble import RandomForestClassifier
         model = RandomForestClassifier(**params)
-    elif model in ("xgb", "xgboost"):
+    elif model_str in ("xgb", "xgboost"):
         from xgboost import XGBClassifier
         model = XGBClassifier(**params)
-    elif model in ("lgbm", "lightgbm"):
+    elif model_str in ("lgbm", "lightgbm"):
         from lightgbm import LGBMClassifier
         model = LGBMClassifier(**params)
     else:
-        raise ValueError(f"The model {model} is not available.")
+        raise ValueError(f"The model {model_str} is not available.")
     
     return model
 
-def _ebfs(
-    model:str
+def _fc_fi(
+    model_str:str
     , params:dict[str, Any]
     , target:str
-    , comb: Tuple
+    , features: Tuple | list
     , train: pl.DataFrame
-    , test:pl.DataFrame
-)-> Tuple[Tuple[Tuple, float, float, float], np.ndarray]:
-    estimator = _binary_model_init(model, params)
-    _ = estimator.fit(train.select(comb), train[target])
-    y_pred = estimator.predict_proba(test.select(comb))[:,1]
+    , test: pl.DataFrame
+)-> Tuple[Tuple[Tuple, float, float], np.ndarray]:
+    
+    estimator = _binary_model_init(model_str, params)
+    _ = estimator.fit(train.select(features), train[target])
+    y_pred = estimator.predict_proba(test.select(features))[:,1]
     y_test = test[target].to_numpy()
-    rec = (
-        comb,
+    fc_rec = (
+        features,
         logloss(y_test, y_pred, check_binary=False),
         roc_auc(y_test, y_pred, check_binary=False)
     )
-    if model in ("lr", "logistic"):
-        importances = np.abs(estimator.coef_).ravel()
+    if model_str in ("lr", "logistic"):
+        fi_rec = np.abs(estimator.coef_).ravel()
     else:
-        importances = estimator.feature_importances_
-
-    return rec, importances
+        fi_rec = estimator.feature_importances_
+    # fc_rec feature comb record, fi_rec feature importance record
+    return fc_rec, fi_rec
 
 # ebfs: stands for Exhaustive Binary Feature Selection
 def ebfs(
     df:pl.DataFrame
     , target:str
-    , model:BinaryModels
+    , model_str:BinaryModels
     , params:dict[str, Any]
     , n_comb: int = 3
     , train_frac:float = 0.75
 ) -> Tuple[pl.DataFrame, pl.DataFrame]:
-    '''Suppose we have n features and n_comb = 2. This method will select all (n choose 2) 
-    combinations of features, split dataset into a train and a test, train a model on train, 
-    and compute feature importance and roc_auc and logloss, and then finally put 
-    everything into two separate dataframes, the first of which will contain the feature
-    combinations and model performances, and the second will contain the min, avg, max and var of 
-    feature importance of each feature in all its occurences in the training rounds.
+    '''
+    Suppose we have n features and n_comb = 2. This method will select all (n choose 2) 
+    combinations of features, split dataset into a train and a test for each combination, 
+    train a model on train, and compute feature importance and roc_auc and logloss, and 
+    then finally put everything into two separate dataframes, the first of which will contain 
+    the feature combinations and model performances, and the second will contain the min, avg, 
+    max and var of feature importance of each feature in all its occurences in the training rounds.
+
+    Notice since we split data into train and test every time for a different feature combination, the 
+    average feature importance we derive naturally are `cross-validated` to a certain degree.
 
     This method will be extremely slow if (n choose n_comb) is a big number. All numerical columns 
     will be taken as potential features. Please encode the string columns if you want to use them
     as features here.
 
-    Future Improvement? Record progress and skip through results.
-
     If n_jobs is not provided in params, it will be defaulted to -1.
 
-        Arguments:
-            df: an eager Polars DataFrame
-            target: target column
-            model: one of 'logistic', 'lr', 'lightgbm', 'lgbm', 'xgboost', 'xgb', 'random_forest', 'rf'
-            params: parameters for the model.
-            n_comb: n choose n_comb
-
-        Returns:
-            a feature combination summary, a feature importance summary
+    Parameters
+    ----------
+    df
+        An eager Polars DataFrame
+    target
+        The target column
+    model_str
+        one of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        Parameters for the model
+    n_comb
+        We will run this for all n choose n_comb combinations of features
     '''
-    
     features = get_numeric_cols(df, exclude=[target])
-    train, test = train_test_split(df.select(features + [target]), train_frac)
     fi = {f:[] for f in features}
     records = []
-    pbar = tqdm(total=math.comb(len(features), n_comb), desc="Total Combinations")
-    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
-        futures = (
-            ex.submit(
-                _ebfs
-                , model
-                , params
-                , target
-                , comb
-                , train
-                , test
-            )
-            for comb in combinations(features, r=n_comb)
-        )
-        for f in as_completed(futures):
-            fc_rec, fi_rec = f.result()
-            records.append(fc_rec)
-            for f, i in zip(fc_rec[0], fi_rec):
-                fi[f].append(i)
-            pbar.update(1)
+    pbar = tqdm(total=math.comb(len(features), n_comb), desc="Tested Combinations")
+    df_keep = df.select(features + [target])
+    for comb in combinations(features, r=n_comb):
+        train, test = train_test_split(df_keep, train_frac)
+        fc_rec, fi_rec = _fc_fi(model_str, params, target, comb, train, test) 
+        records.append(fc_rec)
+        for f, i in zip(fc_rec[0], fi_rec):
+            fi[f].append(i)
+        pbar.update(1)
 
     fc_summary = pl.from_records(records, schema=["combination", "logloss", "roc_auc"])
     stats = [
         (f, len(fi[f]), np.min(fi[f]), np.mean(fi[f]), np.max(fi[f]), np.std(fi[f])) for f in fi
     ]
-    fi_summary = pl.from_records(stats, schema=["feature", "occurrences", "min", "mean", "max", "std"])
+    fi_summary = pl.from_records(stats, schema=["feature", "occurrences", "fi_min", "fi_mean", "fi_max", "fi_std"])
     pbar.close()
     return fc_summary, fi_summary
 
 def ebfs_fc_filter(
     fc: pl.DataFrame
     , logloss_threshold:float
     , roc_auc_threshold:float
 ) -> list[str]:
-    '''A filter method based on the feature combination result of ebfs. First, 
-
-        Arguments:
-            fc: the feature combination result from ebfs
-            logloss_threshold: the maximum logloss for the combination to be kept
-            roc_auc_threshold: the minumum roc_auc for the combination to be kept
+    '''
+    A filter method based on the feature combination result of ebfs.
 
-        Returns:
-            a list of string representing all features in the combinations after filtering
+    Parameters
+    ----------
+    fc
+        The feature combination result from ebfs
+    logloss_threshold
+        The maximum logloss for the combination to be kept
+    roc_auc_threshold
+        The minimum roc_auc for the combination to be kept
     '''
     return fc.filter(
-        pl.col("logloss") <= logloss_threshold
-        & pl.col("roc_auc") >= roc_auc_threshold
+        (pl.col("logloss") <= logloss_threshold)
+        & (pl.col("roc_auc") >= roc_auc_threshold)
     ).get_column("combination").explode().unique().to_list()
 
+def _permute_importance(
+    model:ClassifModel
+    , df:pl.DataFrame
+    , y: np.ndarray
+    , features: Tuple | list
+    , index: int
+    , k: int
+) -> Tuple[float, int]:
+    test_score = 0.
+    for _ in range(k):
+        shuffled_df = df.with_columns(
+            pl.col(features[index]).shuffle(seed=42)
+        )
+        pred = model.predict_proba(shuffled_df[features])[:, -1]
+        test_score += roc_auc(y, pred)
+
+    return test_score, index
+
+# Can extend this for n_comb as well, as 
+
+def permutation_importance(
+    df:pl.DataFrame
+    , target:str
+    , model_str:BinaryModels
+    , params:dict[str, Any]
+    , k:int = 5
+) -> pl.DataFrame:
+    '''
+    Computes permutation importance for every non-target column in df. Please make sure all columns are properly encoded
+    or transformed before calling this.
+    
+    Only works for binary classification and score = roc_auc for now.
+
+    Parameters
+    ----------
+    df
+        An eager Polars DataFrame
+    target
+        The target column
+    model_str
+        One of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        Parameters for the model
+    k
+        Permute the same feature k times
+    '''
+    features = df.columns
+    features.remove(target)
+    
+    estimator = _binary_model_init(model_str, params)
+    estimator.fit(df[features], df[target])
+    y = df[target].to_numpy()
+    pred = estimator.predict_proba(df[features])[:, -1]
+    score = roc_auc(y, pred)
+    pbar = tqdm(total=len(features), desc="Analyzing Features")
+    imp = np.zeros(shape=len(features))
+    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
+        futures = (
+            ex.submit(
+                _permute_importance,
+                estimator,
+                df,
+                y,
+                features, 
+                j,
+                k
+            )
+            for j in range(len(features))
+        )
+        for f in as_completed(futures):
+            test_score, i = f.result()
+            imp[i] = score - (1/k)*test_score
+            pbar.update(1)
 
-    
+    return pl.from_records((features, imp), schema=["feature", "permutation_importance"])
```

### Comparing `dsds-0.0.17/src/dsds/metrics.py` & `dsds-0.0.18/src/dsds/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 
 def get_tp_fp(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , ratio:bool = True
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     '''
-        Get true positive and false positive counts at various thresholds.
+    Get true positive and false positive counts at various thresholds.
 
-        Arguments:
-            y_actual: actual binary labels
-            y_predicted: predicted labels
-            ratio: if true, return true positive rate and false positive rate at the threholds; 
-            if false return the count.
-
-        Returns:
-            True positive count/rate, False positive count/rate, the thresholds
+    Parameters
+    ----------
+    y_actual
+        Actual binary labels
+    y_predicted
+        Predicted probabilities
+    ratio
+        If true, return true positive rate and false positive rate at the threholds; if false return the count
     '''
    
     df = pl.from_records((y_predicted, y_actual), schema=["predicted", "actual"])
     all_positives = pl.lit(np.sum(y_actual))
     n = len(df)
     temp = df.lazy().groupby("predicted").agg(
         pl.count().alias("cnt")
@@ -61,22 +61,25 @@
     tp = temp["tp"].to_numpy()
     fp = temp["fp"].to_numpy()
     if ratio:
         return tp/tp[0], fp/fp[0], temp["predicted"].to_numpy()
     return tp, fp, temp["predicted"].to_numpy()
 
 def roc_auc(y_actual:np.ndarray, y_predicted:np.ndarray, check_binary:bool=True) -> float:
-    '''Return the Area Under the Curve metric for the model's predictions.
-
-        Arguments:
-            y_actual: actual target
-            y_predicted: predicted probability
+    '''
+    Return the Area Under the Curve metric for the model's predictions.
 
-        Returns:
-            the auc value
+    Parameters
+    ----------
+    y_actual
+        Actual binary labels
+    y_predicted
+        Predicted probabilities
+    check_binary
+        If true, checks if y_actual is binary
     ''' 
     
     # This currently has difference of magnitude 1e-10 from the sklearn implementation, 
     # which is likely caused by sklearn adding zeros to the front? Not 100% sure
     # This is about 50% faster than sklearn's implementation. I know, not that this matters
     # that much...
     
@@ -95,29 +98,31 @@
 def logloss(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , sample_weights:Optional[np.ndarray]=None
     , min_prob:float = 1e-12
     , check_binary:bool = True
 ) -> float:
-    '''Return the logloss of the prediction.
-
-        Arguments:
-            y_actual: actual target
-            y_predicted: predicted probability
-            sample_weights: an array of size (n_sample, ) which provides weights to each sample
-            min_prob: minimum probability to clip so that we can prevent illegal computations like 
-            log(0). If p < min_prob, log(min_prob) will be computed instead.
-
-        Returns:
-            the average logloss
+    '''
+    Return the logloss of the binary classification.
 
+    Parameters
+    ----------
+    y_actual
+        Actual binary labels
+    y_predicted
+        Predicted probabilities
+    sample_weights
+        An array of size (n_sample, ) which provides weights to each sample
+    min_prob
+        Minimum probability to clip so that we can prevent illegal computations like 
+        log(0). If p < min_prob, log(min_prob) will be computed instead.
     '''
-    # Takes about 1/3 time of sklearn's log_loss because we parallelized some computations
 
+    # Takes about 1/3 time of sklearn's log_loss because we parallelized some computations
     y_a, y_p = _flatten_input(y_actual, y_predicted)
     if check_binary:
         uniques = np.unique(y_a)
         if uniques.size != 2:
             raise ValueError("Currently this only supports binary classification.")
         if not (0 in uniques and 1 in uniques):
             raise ValueError("Currently this only supports binary classification with 0 and 1 target.")
@@ -138,69 +143,125 @@
             ny = 1 - pl.col("y")
         ).select(
             pl.lit(-1, dtype=pl.Float64)
             * pl.col("s") 
             * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o")).mean()
         ).row(0)[0]
 
-
 def l2_loss(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , sample_weights:Optional[np.ndarray]=None
 ) -> float:
+    '''
+    Computes average L2 loss of some regression model
+
+    Parameters
+    ----------
+    y_actual
+        Actual target
+    y_predicted
+        Predicted target
+    sample_weights
+        An array of size (n_sample, ) which provides weights to each sample
+    '''
     diff = y_actual - y_predicted
     if sample_weights is None:
         return np.mean(diff.dot(diff))
     else:
         return (sample_weights/(len(diff))).dot(diff.dot(diff))
     
 mse = l2_loss
 
 def l1_loss(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , sample_weights:Optional[np.ndarray]=None
 ) -> float:
+    '''
+    Computes average L1 loss of some regression model
+
+    Parameters
+    ----------
+    y_actual
+        Actual target
+    y_predicted
+        Predicted target
+    sample_weights
+        An array of size (n_sample, ) which provides weights to each sample
+    '''
     diff = np.abs(y_actual - y_predicted)
     if sample_weights is None:
         return np.mean(diff)
     else:
         return (sample_weights/(len(diff))).dot(diff)
 
 mae = l1_loss 
 
 def r2(y_actual:np.ndarray, y_predicted:np.ndarray) -> float:
-    '''Returns the r2 of the prediction.'''
+    '''
+    Computes R square metric for some regression model
+
+    Parameters
+    ----------
+    y_actual
+        Actual target
+    y_predicted
+        Predicted target
+    '''
 
     # This is trivial, and we won't really have any performance gain by using Polars' or other stuff.
     # This is here just for completeness
     d1 = y_actual - y_predicted
     d2 = y_actual - np.mean(y_actual)
     # ss_res = d1.dot(d1), ss_tot = d2.dot(d2) 
     return 1 - d1.dot(d1)/d2.dot(d2)
 
 def adjusted_r2(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , p:int
 ) -> float:
-    '''Computes the adjusted r2 of the prediction.
+    '''
+    Computes adjusted R square metric for some regression model
 
-        p: number of predictive variables
+    Parameters
+    ----------
+    y_actual
+        Actual target
+    y_predicted
+        Predicted target
+    p
+        Number of predictive variables used
     '''
     df_tot = len(y_actual) - 1
     return 1 - (1 - r2(y_actual, y_predicted)) * df_tot / (df_tot - p)
 
 def huber_loss(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , delta:float
     , sample_weights:Optional[np.ndarray]=None  
 ) -> float:
+    '''
+    Computes huber loss of some regression model
+
+    See: https://en.wikipedia.org/wiki/Huber_loss
+
+    Parameters
+    ----------
+    y_actual
+        Actual target
+    y_predicted
+        Predicted target
+    delta
+        The delta parameter in huber loss
+    sample_weights
+        An array of size (n_sample, ) which provides weights to each sample
+    '''
     
     y_a = y_actual.ravel()
     y_p = y_predicted.ravel()
     
     if delta <= 0:
         raise ValueError("Delta in Huber loss must be positive.")
```

### Comparing `dsds-0.0.17/src/dsds/prescreen.py` & `dsds-0.0.18/src/dsds/prescreen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .type_alias import (
     PolarsFrame
     , KSAlternatives
     , CommonContinuousDist
+    , SimpleDtypes
     , CPU_COUNT
     , POLARS_DATETIME_TYPES
     , POLARS_NUMERICAL_TYPES
 )
 from .sample import (
     lazy_sample
 )
@@ -30,66 +31,127 @@
 logger = logging.getLogger(__name__)
 
 #----------------------------------------------------------------------------------------------#
 # Generic columns checks | Only works with Polars because Pandas's data types suck!            #
 #----------------------------------------------------------------------------------------------#
 
 def get_numeric_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
+    '''Returns numerical columns except those in exclude.'''
     if exclude is None:
         selector = cs.numeric()
     else:
         selector = cs.numeric() & ~cs.by_name(exclude)
     return df.select(selector).columns
 
 def get_string_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
+    '''Returns string columns except those in exclude.'''
     if exclude is None:
         selector = cs.string()
     else:
         selector = cs.string() & ~cs.by_name(exclude)
     return df.select(selector).columns
 
 def get_datetime_cols(df:PolarsFrame) -> list[str]:
-    '''Only gets datetime columns, will not infer from strings.'''
+    '''Returns only datetime columns. This will not try to infer date from strings.'''
     return df.select(cs.datetime()).columns
 
 def get_bool_cols(df:PolarsFrame) -> list[str]:
+    '''Returns boolean columns.'''
     return df.select(cs.by_dtype(pl.Boolean)).columns
 
 def get_cols_regex(df:PolarsFrame, pattern:str) -> list[str]:
+    '''Returns columns that have names matching the regex pattern.'''
     return df.select(cs.matches(pattern=pattern)).columns
 
-def lowercase_columns(df:PolarsFrame) -> PolarsFrame:
-    return df.rename({c: c.lower() for c in df.columns})
+def lowercase_columns(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+    '''
+    Lowercases all column names.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    output = df.rename({c: c.lower() for c in df.columns})
+    if isinstance(df, pl.LazyFrame) and persist:
+        return output.blueprint.apply_func(df, lowercase_columns, kwargs = {})
+    return output
+
+def drop_nulls(
+    df:PolarsFrame
+    , subset:Optional[list[str]] = None
+    , persist:bool=False
+) -> PolarsFrame:
+    '''
+    A wrapper function for Polars' drop_nulls so that it can be used in pipeline.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    if subset is None:
+        by = df.columns
+    else:
+        by = subset
+
+    if isinstance(df, pl.LazyFrame):
+        cond = pl.lit(True)
+        for c in by:
+            cond = cond & pl.col(c).is_not_null()
+        
+        if persist:
+            return df.blueprint.filter(cond)
+        return df.filter(cond)
+    else:
+        return df.drop_nulls(subset=by)
+
+def filter(
+    df:PolarsFrame
+    , condition: pl.Expr
+    , persist: bool = False
+) -> PolarsFrame:
+    ''' 
+    A wrapper function for Polars' filter so that it can be used in pipeline.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    if isinstance(df, pl.LazyFrame):
+        if persist:
+            return df.blueprint.filter(condition)
+    return df.filter(condition)
 
 def check_binary_target(df:PolarsFrame, target:str) -> bool:
+    '''Checks if target is binary or not. Only binary targets with 0s and 1s will pass.'''
     target_uniques = df.lazy().select(pl.col(target).unique()).collect().get_column(target)
     if len(target_uniques) != 2:
         logger.error("Target is not binary.")
         return False
     elif not (0 in target_uniques and 1 in target_uniques):
         logger.error("The binary target is not encoded as 0s and 1s.")
         return False
     return True
     
 def check_target_cardinality(df:PolarsFrame, target:str) -> pl.DataFrame:
+    '''Returns a dataframe showing the cardinality of different target values.'''
     return df.lazy().groupby(target).count().sort(target).collect()
 
 def check_columns_types(df:PolarsFrame, cols:Optional[list[str]]=None) -> str:
     '''Returns the unique types of given columns in a single string. If multiple types are present
-    they are joined by a |. If cols is not given, automatically uses all df's columns.'''
+    they are joined by a |. If cols is not given, automatically uses all columns.'''
     if cols is None:
         check_cols:list[str] = df.columns
     else:
         check_cols:list[str] = cols 
 
     types = set(dtype_mapping(t) for t in df.select(check_cols).dtypes)
     return "|".join(types) if len(types) > 0 else "unknown"
-    
+
+def type_checker(df:PolarsFrame, cols:list[str], expected_type:SimpleDtypes, caller_name:str) -> bool:
+    types = check_columns_types(df, cols)
+    if types != expected_type:
+        raise ValueError(f"The call `{caller_name}` can only be used on {expected_type} columns, not {types} types.")    
+    return True
+
 # dtype can be a "pl.datatype" or just some random data for which we want to infer a generic type.
-def dtype_mapping(d: Any) -> str:
+def dtype_mapping(d: Any) -> SimpleDtypes:
     if isinstance(d, str) or d == pl.Utf8:
         return "string"
     elif isinstance(d, bool) or d == pl.Boolean:
         return "bool"
     elif isinstance(d, (int,float)) or d in POLARS_NUMERICAL_TYPES:
         return "numeric"
     elif isinstance(d, datetime) or d in POLARS_DATETIME_TYPES:
@@ -103,23 +165,17 @@
 
 # Add a slim option that returns fewer stats? This is generic describe.
 # Separate str and numeric?
 def describe(
     df:PolarsFrame
     , sample_frac:float = 0.75
 ) -> pl.DataFrame:
-    '''Profile the data.
-
-        Arguments:
-            df: Either an eager dataframe or a lazy dataframe
-            sample_frac: If input is a LazyFrame, a sample of sample_frac will be used. If input is eager,
-            no sampling will be done.
+    '''
+    Profile the data.
 
-        Returns:
-            a dataframe containing the necessary information.
     '''
 
     if isinstance(df, pl.LazyFrame):
         df_local = lazy_sample(df, sample_frac=sample_frac)
     else:
         df_local = df
     
@@ -143,19 +199,20 @@
     dtypes_dict = dict(zip(df_local.columns, map(dtype_mapping, df_local.dtypes)))
     # Combine all
     nums = ("count", "null_count", "mean", "std", "median", "25%", "75%")
     final = temp.transpose(include_header=True, column_names=desc).with_columns(
         pl.col(c).cast(pl.Float64) for c in nums
     ).with_columns(
         null_pct = pl.col("null_count")/pl.col("count")
+        , CoV = pl.col("std") / pl.col("mean")
         , dtype = pl.col("column").map_dict(dtypes_dict)
     ).join(unique_counts, on="column").join(skew_and_kt, on="column")
     
     return final.select('column','count','null_count','null_pct','n_unique'
-                        , 'unique_pct','mean','std','min','max','25%'
+                        , 'unique_pct','mean','std', 'CoV','min','max','25%'
                         , 'median','75%', "skew", "kurtosis",'dtype')
 
 # Numeric only describe. Be more detailed.
 
 # String only describe. Be more detailed about interesting string stats.
 
 def describe_str(df:PolarsFrame
@@ -243,15 +300,16 @@
     , pattern:str
     , sample_frac:float = 0.75
     , sample_count:int = 100_000
     , sample_rounds:int = 3
     , threshold:float = 0.9
     , count_null:bool = True
 ) -> list[str]:
-    '''Find all string columns whose elements reasonably match the given pattern. The match logic can 
+    '''
+    Find all string columns whose elements reasonably match the given pattern. The match logic can 
     be tuned using the all the parameters.
 
     Arguments:
         sample_frac: the pct of the total dataframe to use as basis
         sample_count: from the basis, how many rows to sample for each round 
         sample_rounds: how many rounds of sampling we are doing
         threhold: For each round, what is the match% that is needed to be a counted as a success. For instance, 
@@ -640,12 +698,12 @@
 
 def suggest_dist(
     df:PolarsFrame
     , target: Optional[str] = None
     , threshold:float = 0.05
     , dist: CommonContinuousDist = "norm"
 ) -> list[str]:
-    '''Suggests which columns follow the given distribution. This takes the columns which the null hypothesis
+    '''Suggests which columns follow the given distribution. This returns the columns which the null hypothesis
     cannot be rejected in the dist_test (KS test).
     '''
     return dist_test(df, dist, target=target).filter(pl.col("p-value") > threshold)\
         .get_column("feature").to_list()
```

### Comparing `dsds-0.0.17/src/dsds/utils.py` & `dsds-0.0.18/src/dsds/utils.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.17/src/dsds.egg-info/PKG-INFO` & `dsds-0.0.18/src/dsds.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.17
+Version: 0.0.18
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,16 +74,15 @@
     , constant_removal
     , date_removal
     , non_numeric_removal
     , get_unique_count
     , get_string_cols
     , suggest_normal
     , discrete_inferral
-)
-
+) # and a lot more!
 
 ```
 
 Functional Pipeline Interface which supports both Eager and LazyFrames! And it can be pickled and load back and reapplied! See more in the examples on github.
 
 ```python
 from dsds.prescreen import *
@@ -113,12 +112,30 @@
 
 pip install dsds[all]
 
 Note: scikit-learn, lightgbm, xgboost are needed for full functionalities. 
 
 # Why DSDS?
 
-I choose DarkSide because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
+(1) Fast and furious
+
+(2) Simple, single-purpose, clean, optimized and fully typed functions
+
+(3) Easy to extend
+
+(4) Supports Polars LazyFrame, and therefore query optimizations in pipeline.
+
+(5) No boilerplate
+
+# Why the name DSDS?
+
+I choose the name Dark Side of Data Science because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
 
 # Why is this package dependent on Sklearn?
 
-You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives. 
+You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
+
+# Why not write more functionalities in Rust?
+
+Yes. I will. I am not confident enough with my Rust skill at the moment. I am slowly learning more Rust and hopefully we can delegate more heavy work to Rust. The immediate benefit of using more Rust will be (1) slightly more memory efficient, and (2) slightly faster. I do not expect huge speed boost because most code are written in Polars already. There are some cases when a lot of Python stuff is added (lists and for loops, etc.). But we definitely need to evaluate the gain by using Rust more carefully in the future.
+
+See CONTRIBUTING.md for my contact info.
```

