# Comparing `tmp/golfy-2.2.0.tar.gz` & `tmp/golfy-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-2.2.0.tar", last modified: Thu Jul 13 21:46:01 2023, max compression
+gzip compressed data, was "golfy-2.3.0.tar", last modified: Sun Jul 16 21:55:25 2023, max compression
```

## Comparing `golfy-2.2.0.tar` & `golfy-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.758552 golfy-2.2.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.2.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 21:46:01.758401 golfy-2.2.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     4495 2023-07-13 19:03:02.000000 golfy-2.2.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.755200 golfy-2.2.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-13 21:43:52.000000 golfy-2.2.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.2.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.2.0/golfy/design.py
--rw-r--r--   0 iskander   (501) staff       (20)     2455 2023-07-13 19:55:22.000000 golfy-2.2.0/golfy/evaluation.py
--rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.2.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8071 2023-07-13 21:43:37.000000 golfy-2.2.0/golfy/main.py
--rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.2.0/golfy/merging.py
--rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.2.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.2.0/golfy/simulation.py
--rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.2.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.2.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.2.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.755943 golfy-2.2.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      582 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.2.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.2.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-13 21:46:01.758591 golfy-2.2.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.757978 golfy-2.2.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.2.0/tests/test_best_design_for_pool_budget.py
--rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.2.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.2.0/tests/test_find_best_design.py
--rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.2.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.2.0/tests/test_optimize.py
--rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.2.0/tests/test_simulation.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.321959 golfy-2.3.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.3.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-16 21:55:25.321832 golfy-2.3.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     4495 2023-07-13 19:03:02.000000 golfy-2.3.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.319290 golfy-2.3.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-16 21:53:56.000000 golfy-2.3.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.3.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.3.0/golfy/design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2455 2023-07-13 19:55:22.000000 golfy-2.3.0/golfy/evaluation.py
+-rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.3.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9826 2023-07-16 21:53:51.000000 golfy-2.3.0/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.3.0/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.3.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.3.0/golfy/simulation.py
+-rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.3.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.3.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.3.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.319876 golfy-2.3.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      582 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.3.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.3.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-16 21:55:25.321994 golfy-2.3.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.321555 golfy-2.3.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.3.0/tests/test_best_design_for_pool_budget.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.3.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.3.0/tests/test_find_best_design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.3.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.3.0/tests/test_optimize.py
+-rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.3.0/tests/test_simulation.py
```

### Comparing `golfy-2.2.0/LICENSE` & `golfy-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/PKG-INFO` & `golfy-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.2.0
+Version: 2.3.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-2.2.0/README.md` & `golfy-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/__init__.py` & `golfy-2.3.0/golfy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     simulate_elispot_counts,
     simulate_any_hits_per_pool,
     simulate_number_hits_per_pool,
 )
 from .types import SpotCounts
 from .validity import is_valid, count_violations, violations_per_replicate
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 __all__ = [
     "__version__",
     "find_best_design",
     "best_design_for_pool_budget",
     "Design",
     "init",
```

### Comparing `golfy-2.2.0/golfy/deconvolution.py` & `golfy-2.3.0/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/design.py` & `golfy-2.3.0/golfy/design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/evaluation.py` & `golfy-2.3.0/golfy/evaluation.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/initialization.py` & `golfy-2.3.0/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/main.py` & `golfy-2.3.0/golfy/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -118,62 +118,92 @@
                 print("^^ new best solution")
     return best_design
 
 
 def generate_candidate_specs_for_pool_budget(
     num_peptides: int = 100,
     max_pools: int = 96,
+    min_num_replicates: int = 2,
+    max_num_replicates: int = 5,
+    min_max_peptides_per_pool: int = 2,
+    max_max_peptides_per_pool: Optional[int] = None,
+    allow_extra_pools: Optional[bool] = None,
 ) -> list[Spec]:
     """
     Generator of candidate configurations from which we might want to try
     to make Designs that fit into the given pool budget.
     """
-    for max_peptides_per_pool in range(2, max(3, num_peptides // 5)):
+    if allow_extra_pools is None:
+        allow_extra_pools = [True, False]
+    elif type(allow_extra_pools) is bool:
+        allow_extra_pools = [allow_extra_pools]
+
+    if max_max_peptides_per_pool is None:
+        max_max_peptides_per_pool = max(3, num_peptides // 5)
+
+    if min_num_replicates > max_num_replicates:
+        max_num_replicates = min_num_replicates
+
+    if min_max_peptides_per_pool > max_max_peptides_per_pool:
+        max_max_peptides_per_pool = min_max_peptides_per_pool
+
+    for max_peptides_per_pool in range(
+        min_max_peptides_per_pool, max_max_peptides_per_pool
+    ):
         if max_peptides_per_pool * max_pools < num_peptides:
             # not enough pools to fit all peptides without replicates
             continue
 
-        for num_replicates in range(2, 6):
+        for num_replicates in range(min_num_replicates, max_num_replicates + 1):
             min_pools_for_spec = math.ceil(
                 num_peptides * num_replicates / max_peptides_per_pool
             )
             if min_pools_for_spec > max_pools:
                 # not enough pools to fit all peptides with given number of replicates
                 continue
 
-            for allow_extra_pools in [True, False]:
-                if min_pools_for_spec == max_pools and allow_extra_pools:
-                    # no need to allow extra pools if we're already at the maximum
-                    continue
+            for curr_allow_extra_pools in allow_extra_pools:
                 yield Spec(
                     num_peptides=num_peptides,
                     max_peptides_per_pool=max_peptides_per_pool,
                     num_replicates=num_replicates,
-                    allow_extra_pools=allow_extra_pools,
+                    allow_extra_pools=curr_allow_extra_pools,
                     invalid_neighbors=[],
                     preferred_neighbors=[],
                 )
 
 
 def score_designs_for_pool_budget(
     num_peptides: int = 100,
     max_pools: int = 96,
-    num_simulation_iters: int = 2,
+    num_simulation_iters: int = 3,
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
+    min_pools: Optional[int] = None,
+    min_num_replicates: int = 2,
+    max_num_replicates: int = 5,
+    min_max_peptides_per_pool: int = 2,
+    max_max_peptides_per_pool: Optional[int] = None,
+    allow_extra_pools: Optional[bool] = None,
     verbose: bool = False,
 ) -> list[tuple[Design, EvaluationResult]]:
     assert num_peptides > 1, "No need to pool if there's only one peptide"
     assert max_pools > 1, "Must have more than one pool"
     assert max_pools <= num_peptides, "Can't have more pools than peptides"
 
     designs = []
     specs = list(
         generate_candidate_specs_for_pool_budget(
-            num_peptides=num_peptides, max_pools=max_pools
+            num_peptides=num_peptides,
+            max_pools=max_pools,
+            min_num_replicates=min_num_replicates,
+            max_num_replicates=max_num_replicates,
+            min_max_peptides_per_pool=min_max_peptides_per_pool,
+            max_max_peptides_per_pool=max_max_peptides_per_pool,
+            allow_extra_pools=allow_extra_pools,
         )
     )
     print("Generated %d candidate specs" % (len(specs),))
 
     shared_kwargs = dict(
         num_peptides=num_peptides,
         invalid_neighbors=invalid_neighbors,
@@ -185,35 +215,50 @@
         s = find_best_design(
             max_peptides_per_pool=spec.max_peptides_per_pool,
             num_replicates=spec.num_replicates,
             allow_extra_pools=spec.allow_extra_pools,
             **shared_kwargs,
         )
         num_pools = s.num_pools()
-        if num_pools <= max_pools:
+        if min_pools is not None and num_pools < min_pools:
+            continue
+
+        if num_pools > max_pools:
+            print("%s: %d pools > %d max pools" % (spec, num_pools, max_pools))
+        else:
             scores = evaluate_design(s, num_simulation_iters)
             print("%s: %s" % (spec, scores))
             designs.append((s, scores))
     return designs
 
 
 def best_design_for_pool_budget(
     num_peptides: int = 100,
     max_pools: int = 96,
-    num_simulation_iters: int = 2,
+    num_simulation_iters: int = 3,
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
+    min_pools: Optional[int] = None,
+    min_num_replicates: int = 2,
+    max_num_replicates: int = 5,
+    min_max_peptides_per_pool: int = 2,
+    max_max_peptides_per_pool: Optional[int] = None,
     verbose: bool = False,
 ):
     assert num_peptides > 1, "No need to pool if there's only one peptide"
     assert max_pools > 1, "Must have more than one pool"
     assert max_pools <= num_peptides, "Can't have more pools than peptides"
     designs_with_scores = score_designs_for_pool_budget(
         num_peptides=num_peptides,
         max_pools=max_pools,
         num_simulation_iters=num_simulation_iters,
         invalid_neighbors=invalid_neighbors,
         preferred_neighbors=preferred_neighbors,
+        min_pools=min_pools,
+        min_num_replicates=min_num_replicates,
+        max_num_replicates=max_num_replicates,
+        min_max_peptides_per_pool=min_max_peptides_per_pool,
+        max_max_peptides_per_pool=max_max_peptides_per_pool,
         verbose=verbose,
     )
     best_pair = sorted(designs_with_scores, key=lambda x: x[1].sort_key())[0]
     return best_pair[0]
```

### Comparing `golfy-2.2.0/golfy/merging.py` & `golfy-2.3.0/golfy/merging.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/optimization.py` & `golfy-2.3.0/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/simulation.py` & `golfy-2.3.0/golfy/simulation.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/util.py` & `golfy-2.3.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy/validity.py` & `golfy-2.3.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/golfy.egg-info/PKG-INFO` & `golfy-2.3.0/golfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.2.0
+Version: 2.3.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-2.2.0/golfy.egg-info/SOURCES.txt` & `golfy-2.3.0/golfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/pyproject.toml` & `golfy-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/tests/test_deconvolution.py` & `golfy-2.3.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/tests/test_find_best_design.py` & `golfy-2.3.0/tests/test_find_best_design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/tests/test_init.py` & `golfy-2.3.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `golfy-2.2.0/tests/test_simulation.py` & `golfy-2.3.0/tests/test_simulation.py`

 * *Files identical despite different names*

