# Comparing `tmp/omnixai-1.3.0.tar.gz` & `tmp/omnixai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnixai-1.3.0.tar", last modified: Sat May 27 06:16:07 2023, max compression
+gzip compressed data, was "omnixai-1.3.1.tar", last modified: Sun Jul 16 04:58:01 2023, max compression
```

## Comparing `omnixai-1.3.0.tar` & `omnixai-1.3.1.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.515314 omnixai-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-27 06:15:55.000000 omnixai-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    25485 2023-05-27 06:16:07.515314 omnixai-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24993 2023-05-27 06:15:55.000000 omnixai-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.443313 omnixai-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-05-27 06:15:55.000000 omnixai-1.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.443313 omnixai-1.3.0/omnixai/
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/data/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7594 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/multi_inputs.py
--rw-r--r--   0 runner    (1001) docker     (122)     9288 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/text.py
--rw-r--r--   0 runner    (1001) docker     (122)     7308 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/deployment/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/deployment/bentoml/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/deployment/bentoml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8423 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/deployment/bentoml/omnixai.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/explainers/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15333 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/data/
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/auto.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/chi_square.py
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/correlation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5470 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2937 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/mutual_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13999 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/l2x.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/polyjuice.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/specific/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12781 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/specific/ig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/prediction/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12257 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/prediction/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/ranking/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6199 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/permutation.py
--rw-r--r--   0 runner    (1001) docker     (122)     8572 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13597 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/mace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/tabular/
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14425 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/l2x.py
--rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11890 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/ale.py
--rw-r--r--   0 runner    (1001) docker     (122)    15687 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/bias.py
--rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/gpt.py
--rw-r--r--   0 runner    (1001) docker     (122)     7493 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     6632 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/pdp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/permutation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap_global.py
--rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/auto.py
--rw-r--r--   0 runner    (1001) docker     (122)    10220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18191 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/ce.py
--rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/knn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/
--rw-r--r--   0 runner    (1001) docker     (122)     6913 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/diversify.py
--rw-r--r--   0 runner    (1001) docker     (122)    10231 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/gld.py
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/greedy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6616 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/mace.py
--rw-r--r--   0 runner    (1001) docker     (122)     3461 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/refine.py
--rw-r--r--   0 runner    (1001) docker     (122)    10768 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (122)    12648 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/rl.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/tabular/specific/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8023 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    12323 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/ig.py
--rw-r--r--   0 runner    (1001) docker     (122)     8461 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/shap_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/ce.py
--rw-r--r--   0 runner    (1001) docker     (122)    14166 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/mace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/vision/
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/vision/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12137 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/l2x.py
--rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     6200 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/pdp.py
--rw-r--r--   0 runner    (1001) docker     (122)     6946 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/vision/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/counterfactual/ce.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20052 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/cem.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py
--rw-r--r--   0 runner    (1001) docker     (122)     8979 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/feature_maps.py
--rw-r--r--   0 runner    (1001) docker     (122)    10233 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     3525 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11892 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7815 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/gradcam.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/pytorch/
--rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/tf/
--rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py
--rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/guided_bp.py
--rw-r--r--   0 runner    (1001) docker     (122)     7351 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/ig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/pytorch/
--rw-r--r--   0 runner    (1001) docker     (122)     4944 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py
--rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/scorecam.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/tf/
--rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py
--rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)    12357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/specific/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/gradcam.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7249 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py
--rw-r--r--   0 runner    (1001) docker     (122)     7890 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/ig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explanations/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12095 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explanations/image/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8304 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/contrast.py
--rw-r--r--   0 runner    (1001) docker     (122)     7679 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (122)     6849 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/mask.py
--rw-r--r--   0 runner    (1001) docker     (122)    16919 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/pixel_importance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5431 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/plain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/prediction/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4120 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/confusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     5909 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/cumulative.py
--rw-r--r--   0 runner    (1001) docker     (122)     4739 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/lift.py
--rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/pr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4060 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/residual.py
--rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/roc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/tabular/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7331 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/ale.py
--rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/bias.py
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/correlation.py
--rw-r--r--   0 runner    (1001) docker     (122)    13514 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (122)    14586 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     7804 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/pdp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (122)     9267 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/tree.py
--rw-r--r--   0 runner    (1001) docker     (122)     7965 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/text/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11622 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/text/word_importance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7839 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/timeseries/counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (122)    10436 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/timeseries/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/encode.py
--rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/fill.py
--rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/sampler/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.443313 omnixai-1.3.0/omnixai/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_image.py
--rw-r--r--   0 runner    (1001) docker     (122)      976 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_text.py
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.439313 omnixai-1.3.0/omnixai/tests/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/
--rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/api_server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/
--rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/
--rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2634 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/save.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/L2X/
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x.py
--rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/ale/
--rw-r--r--   0 runner    (1001) docker     (122)     1925 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/bias/
--rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/ce/
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (122)     8048 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     6241 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/cem/
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5627 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_chi2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_imbalance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_mutual.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/decision_tree/
--rw-r--r--   0 runner    (1001) docker     (122)     4369 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_explainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6033 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fft.py
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/gpt/
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gpt/gpt_explainer_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/gradcam/
--rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/guided_bp/
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/ig/
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6529 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     8873 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/vlm_ig_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/knn/
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/knn/test_ce_knn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/lime/
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     5527 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/linear/
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/mace/
--rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_mace.py
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_mace_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_rl_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/pdp/
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/pdp/pdp_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/permutation/
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/permutation/test_permutation_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/permutation/test_permutation_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/polyjuice/
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/polyjuice/polyjuice_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/polyjuice/polyjuice_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/prediction/
--rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_confusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_lift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_pr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_regression_metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_residual.py
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_roc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/ranking/
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ranking/test_perm_ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ranking/test_validity_ranking.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/scorecam/
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/scorecam/scorecam_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/scorecam/test_scorecam_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/sensitivity/test_sa_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/explainers/shap/
--rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6134 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_merlion.py
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_text.py
--rw-r--r--   0 runner    (1001) docker     (122)     3940 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_global.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/explainers/shap_tree/
--rw-r--r--   0 runner    (1001) docker     (122)     4693 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/
--rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10940 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_fill.py
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)     2059 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_tabular_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_text_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/sampler/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/utils/json/
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/json/test_counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/json/test_feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/json/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/test_explanation_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/test_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_da.py
--rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_image_compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     5016 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_text.py
--rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_text_imdb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/utils/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.511314 omnixai-1.3.0/omnixai/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.511314 omnixai-1.3.0/omnixai/visualization/assets/
--rwxr-xr-x   0 runner    (1001) docker     (122)    83784 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/Acumin-BdPro.otf
--rw-r--r--   0 runner    (1001) docker     (122)    12235 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/base.css
--rw-r--r--   0 runner    (1001) docker     (122)    28366 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/logo_small.png
--rw-r--r--   0 runner    (1001) docker     (122)     6085 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/modal.css
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/resizing.js
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/xai.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.511314 omnixai-1.3.0/omnixai/visualization/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/data_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/global_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/local_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/prediction_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/whatif_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     8589 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.515314 omnixai-1.3.0/omnixai/visualization/pages/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/data_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/global_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/local_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/prediction_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6981 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/whatif_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     7663 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/state.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    25485 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    15849 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-27 06:16:07.515314 omnixai-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-27 06:15:55.000000 omnixai-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.185985 omnixai-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-07-16 04:57:47.000000 omnixai-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    25620 2023-07-16 04:58:01.181985 omnixai-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    25128 2023-07-16 04:57:47.000000 omnixai-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.117981 omnixai-1.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-16 04:57:47.000000 omnixai-1.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.117981 omnixai-1.3.1/omnixai/
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7594 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/data/multi_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9288 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/data/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/data/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7308 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/data/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/deployment/bentoml/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/deployment/bentoml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8423 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/deployment/bentoml/omnixai.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15333 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/data/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/data/chi_square.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/data/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5470 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/data/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2937 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/data/mutual_info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/nlp/
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/nlp/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13999 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/agnostic/l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/agnostic/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/nlp/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/counterfactual/polyjuice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/nlp/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12781 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/nlp/specific/ig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/prediction/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12257 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/prediction/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.121981 omnixai-1.3.1/omnixai/explainers/ranking/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/ranking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.125981 omnixai-1.3.1/omnixai/explainers/ranking/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/ranking/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6199 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/ranking/agnostic/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8572 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/ranking/agnostic/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.125981 omnixai-1.3.1/omnixai/explainers/ranking/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/ranking/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13597 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/ranking/counterfactual/mace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.125981 omnixai-1.3.1/omnixai/explainers/tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.125981 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.125981 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/L2X/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/L2X/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14425 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/L2X/l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/L2X/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11890 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/ale.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15687 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/bias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7493 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6632 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/agnostic/shap_global.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.125981 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18191 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/ce.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/knn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.129982 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/
+-rw-r--r--   0 runner    (1001) docker     (122)     6913 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/diversify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10231 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/gld.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6616 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/mace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3461 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/refine.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10768 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12648 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/rl.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.129982 omnixai-1.3.1/omnixai/explainers/tabular/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8023 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/specific/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12323 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/specific/ig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8461 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/specific/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/tabular/specific/shap_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.129982 omnixai-1.3.1/omnixai/explainers/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.129982 omnixai-1.3.1/omnixai/explainers/timeseries/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/timeseries/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/timeseries/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/timeseries/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.133982 omnixai-1.3.1/omnixai/explainers/timeseries/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/timeseries/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/timeseries/counterfactual/ce.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14166 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/timeseries/counterfactual/mace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.133982 omnixai-1.3.1/omnixai/explainers/vision/
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.133982 omnixai-1.3.1/omnixai/explainers/vision/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12137 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/agnostic/l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/agnostic/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6200 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/agnostic/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6946 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.133982 omnixai-1.3.1/omnixai/explainers/vision/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/counterfactual/ce.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.137982 omnixai-1.3.1/omnixai/explainers/vision/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20052 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/cem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.137982 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.137982 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8979 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.137982 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/feature_maps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10233 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3525 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11892 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.137982 omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7815 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/gradcam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.137982 omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.137982 omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/tf/
+-rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/guided_bp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7351 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/ig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)     4944 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/scorecam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/tf/
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12357 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision/specific/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explainers/vision_language/
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision_language/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explainers/vision_language/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision_language/specific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/gradcam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7249 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7890 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explainers/vision_language/specific/ig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.141982 omnixai-1.3.1/omnixai/explanations/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12095 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.145983 omnixai-1.3.1/omnixai/explanations/image/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8304 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/image/contrast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7679 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/image/counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6849 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/image/mask.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16919 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/image/pixel_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5431 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/image/plain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.145983 omnixai-1.3.1/omnixai/explanations/prediction/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4120 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/confusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5909 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4739 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/lift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/pr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4060 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/prediction/roc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.149983 omnixai-1.3.1/omnixai/explanations/tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7331 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/ale.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/bias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13514 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14586 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7804 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9267 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7965 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/tabular/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.149983 omnixai-1.3.1/omnixai/explanations/text/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11622 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/text/word_importance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.149983 omnixai-1.3.1/omnixai/explanations/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7839 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/timeseries/counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10436 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/timeseries/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/explanations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.149983 omnixai-1.3.1/omnixai/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/encode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/fill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8298 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.149983 omnixai-1.3.1/omnixai/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/sampler/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.117981 omnixai-1.3.1/omnixai/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.153983 omnixai-1.3.1/omnixai/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/data/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/data/test_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/data/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/data/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.113981 omnixai-1.3.1/omnixai/tests/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.153983 omnixai-1.3.1/omnixai/tests/deployment/bentoml/
+-rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/api_server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.153983 omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.153983 omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2634 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.157983 omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.157983 omnixai-1.3.1/omnixai/tests/explainers/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.157983 omnixai-1.3.1/omnixai/tests/explainers/L2X/
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.157983 omnixai-1.3.1/omnixai/tests/explainers/ale/
+-rw-r--r--   0 runner    (1001) docker     (122)     1925 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ale/test_ale_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ale/test_ale_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.157983 omnixai-1.3.1/omnixai/tests/explainers/bias/
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/bias/test_bias_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/bias/test_bias_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.157983 omnixai-1.3.1/omnixai/tests/explainers/ce/
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8048 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6241 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.161983 omnixai-1.3.1/omnixai/tests/explainers/cem/
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/cem/cem_optimizer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5627 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/cem/cem_optimizer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/cem/test_cem_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/cem/test_cem_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.161983 omnixai-1.3.1/omnixai/tests/explainers/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/data/test_chi2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/data/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/data/test_imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/data/test_mutual.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.161983 omnixai-1.3.1/omnixai/tests/explainers/decision_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)     4369 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/decision_tree/test_tree_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/decision_tree/test_tree_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/explainer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/explainer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/feature_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6033 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_fft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/gpt/
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/gpt/gpt_explainer_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/gradcam/
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_gradcam_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_gradcam_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_layercam_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_layercam_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/guided_bp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/ig/
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ig/nlp_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6529 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ig/nlp_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ig/test_ig_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8873 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ig/test_ig_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ig/vlm_ig_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/knn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/knn/test_ce_knn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/lime/
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5527 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.165984 omnixai-1.3.1/omnixai/tests/explainers/linear/
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/linear/test_linear_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/linear/test_linear_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.169984 omnixai-1.3.1/omnixai/tests/explainers/mace/
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/mace/test_mace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/mace/test_mace_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/mace/test_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/mace/test_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/mace/test_rl_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.169984 omnixai-1.3.1/omnixai/tests/explainers/pdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/pdp/pdp_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/pdp/test_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/pdp/test_tabular_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.169984 omnixai-1.3.1/omnixai/tests/explainers/permutation/
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/permutation/test_permutation_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/permutation/test_permutation_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.169984 omnixai-1.3.1/omnixai/tests/explainers/polyjuice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/polyjuice/polyjuice_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/polyjuice/polyjuice_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.169984 omnixai-1.3.1/omnixai/tests/explainers/prediction/
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_confusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_lift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_pr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_regression_metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/prediction/test_roc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.173984 omnixai-1.3.1/omnixai/tests/explainers/ranking/
+-rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ranking/test_perm_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/ranking/test_validity_ranking.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.173984 omnixai-1.3.1/omnixai/tests/explainers/scorecam/
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/scorecam/scorecam_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/scorecam/test_scorecam_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.173984 omnixai-1.3.1/omnixai/tests/explainers/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/sensitivity/test_sa_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.173984 omnixai-1.3.1/omnixai/tests/explainers/shap/
+-rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/shap_image_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6134 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/shap_image_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/shap_merlion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/shap_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3940 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_tabular_global.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.173984 omnixai-1.3.1/omnixai/tests/explainers/shap_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)     4693 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap_tree/shaptree_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/shap_tree/shaptree_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.173984 omnixai-1.3.1/omnixai/tests/explainers/smoothgrad/
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10940 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/explainers/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.177984 omnixai-1.3.1/omnixai/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/preprocessing/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/preprocessing/test_fill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/preprocessing/test_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/preprocessing/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/preprocessing/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2059 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/preprocessing/test_tabular_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/preprocessing/test_text_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.177984 omnixai-1.3.1/omnixai/tests/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/sampler/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.177984 omnixai-1.3.1/omnixai/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.177984 omnixai-1.3.1/omnixai/tests/utils/json/
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/utils/json/test_counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/utils/json/test_feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/utils/json/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/utils/test_explanation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/utils/test_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.177984 omnixai-1.3.1/omnixai/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_da.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_image_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5016 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_text_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/tests/visualization/dashboard_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.177984 omnixai-1.3.1/omnixai/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/utils/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.181985 omnixai-1.3.1/omnixai/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.181985 omnixai-1.3.1/omnixai/visualization/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    83784 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/assets/Acumin-BdPro.otf
+-rw-r--r--   0 runner    (1001) docker     (122)    12235 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/assets/base.css
+-rw-r--r--   0 runner    (1001) docker     (122)    28366 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/assets/logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6085 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/assets/modal.css
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/assets/resizing.js
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/assets/xai.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.181985 omnixai-1.3.1/omnixai/visualization/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/callbacks/data_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/callbacks/global_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/callbacks/local_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/callbacks/prediction_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/callbacks/whatif_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8589 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.181985 omnixai-1.3.1/omnixai/visualization/pages/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/pages/data_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/pages/global_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/pages/local_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/pages/prediction_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/pages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6981 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/pages/whatif_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7663 2023-07-16 04:57:47.000000 omnixai-1.3.1/omnixai/visualization/state.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 04:58:01.117981 omnixai-1.3.1/omnixai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25620 2023-07-16 04:58:01.000000 omnixai-1.3.1/omnixai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    15849 2023-07-16 04:58:01.000000 omnixai-1.3.1/omnixai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-16 04:58:01.000000 omnixai-1.3.1/omnixai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-16 04:58:00.000000 omnixai-1.3.1/omnixai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-16 04:58:01.000000 omnixai-1.3.1/omnixai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-16 04:58:01.000000 omnixai-1.3.1/omnixai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-16 04:58:01.185985 omnixai-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-07-16 04:57:47.000000 omnixai-1.3.1/setup.py
```

### Comparing `omnixai-1.3.0/LICENSE` & `omnixai-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/PKG-INFO` & `omnixai-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnixai
-Version: 1.3.0
+Version: 1.3.1
 Summary: OmniXAI: An Explainable AI Toolbox
 Home-page: https://github.com/salesforce/omnixai
 Author: Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
 License: 3-Clause BSD
 Keywords: XAI Explainable AI Explanation
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
@@ -43,15 +43,15 @@
 ## Table of Contents
 1. [Introduction](#introduction)
 2. [Installation](#installation)
 3. [Getting Started](#getting-started)
 4. [Documentation](https://opensource.salesforce.com/OmniXAI/latest/index.html)
 5. [Tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html)
 6. [Deployment](#deployment)
-7. [Dashboard Demo](https://sfr-omnixai-demo.herokuapp.com/)
+7. [Dashboard Demo](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/)
 8. [How to Contribute](https://opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute)
 9. [Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai)
 
 ## What's New
 
 The latest version includes an experimental GPT explainer. This explainer leverages the outcomes 
 produced by SHAP and MACE to formulate the input prompt for ChatGPT. Subsequently, ChatGPT 
@@ -133,26 +133,27 @@
 - **Install all the dependencies**: Calling ``pip install omnixai[all]``, or ``pip install .[all]`` from the
   root directory of the repo.
 
 ## Getting Started
 
 For example code and an introduction to the library, see the Jupyter notebooks in
 [tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html), and the guided walkthrough
-[here](https://opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be found [here](https://sfr-omnixai-demo.herokuapp.com/).
+[here](https://opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be found [here](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/).
 
 Some examples:
 1. [Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_classification.ipynb)
 2. [Tabular regression](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb)
 3. [Image classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision.ipynb)
 4. [Text classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/nlp_imdb.ipynb)
 5. [Time-series anomaly detection](https://github.com/salesforce/OmniXAI/blob/main/tutorials/timeseries.ipynb)
 6. [Vision-language tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/gradcam_vlm.ipynb)
 7. [Ranking tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/ranking.ipynb)
 8. [Feature visualization](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/feature_visualization_torch.ipynb)
 9. [Check feature maps](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/feature_map_torch.ipynb)
+10. [GPT explainer for tabular](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/gpt.ipynb)
 
 To get started, we recommend the linked tutorials in [tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html).
 In general, we recommend using `TabularExplainer`, `VisionExplainer`,
 `NLPExplainer` and `TimeseriesExplainer` for tabular, vision, NLP and time-series tasks, respectively, and using
 `DataAnalyzer` and `PredictionAnalyzer` for feature analysis and prediction result analysis.
 These classes act as the factories of the individual explainers supported in OmniXAI, providing a simpler
 interface to generate multiple explanations. To generate explanations, you only need to specify
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: omnixai Version: 1.3.0 Summary: OmniXAI: An
+Metadata-Version: 2.1 Name: omnixai Version: 1.3.1 Summary: OmniXAI: An
 Explainable AI Toolbox Home-page: https://github.com/salesforce/omnixai Author:
 Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
 License: 3-Clause BSD Keywords: XAI Explainable AI Explanation Requires-Python:
 >=3.7,<4 Description-Content-Type: text/markdown Provides-Extra: plot Provides-
 Extra: vision Provides-Extra: nlp Provides-Extra: bentoml Provides-Extra: all
 License-File: LICENSE
 
@@ -10,40 +10,40 @@
 # OmniXAI: A Library for Explainable AI
     [https://img.shields.io/badge/Python-3.7,_3.8,_3.9,_3.10-blue] [PyPI]
                        [Documentation] [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://opensource.salesforce.com/OmniXAI/latest/index.html) 5. [Tutorials]
 (https://opensource.salesforce.com/OmniXAI/latest/tutorials.html) 6.
-[Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-
-demo.herokuapp.com/) 8. [How to Contribute](https://opensource.salesforce.com/
-OmniXAI/latest/omnixai.html#how-to-contribute) 9. [Technical Report and Citing
-OmniXAI](#technical-report-and-citing-omnixai) ## What's New The latest version
-includes an experimental GPT explainer. This explainer leverages the outcomes
-produced by SHAP and MACE to formulate the input prompt for ChatGPT.
-Subsequently, ChatGPT analyzes these results and generates the corresponding
-explanations that provide developers with a clearer understanding of the
-rationale behind the model's predictions. ## Introduction OmniXAI (short for
-Omni eXplainable AI) is a Python machine-learning library for explainable AI
-(XAI), offering omni-way explainable AI and interpretable machine learning
-capabilities to address many pain points in explaining decisions made by
-machine learning models in practice. OmniXAI aims to be a one-stop
-comprehensive library that makes explainable AI easy for data scientists, ML
-researchers and practitioners who need explanation for various types of data,
-models and explanation methods at different stages of ML process: ![alt text]
-(https://github.com/salesforce/OmniXAI/raw/main/docs/_static/ml_pipeline.png)
-OmniXAI includes a rich family of explanation methods integrated in a unified
-interface, which supports multiple data types (tabular data, images, texts,
-time-series), multiple types of ML models (traditional ML in Scikit-learn and
-deep learning models in PyTorch/TensorFlow), and a range of diverse
-explaination methods including "model-specific" and "model-agnostic" methods
-(such as feature-attribution explanation, counterfactual explanation, gradient-
-based explanation, feature visualization, etc). For practitioners, OmniXAI
-provides an easy-to-use unified interface to generate the explanations for
-their applications by only writing a few lines of codes, and also a GUI
+[Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-demo-
+cc9e4edb6447.herokuapp.com/) 8. [How to Contribute](https://
+opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute) 9.
+[Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai) ##
+What's New The latest version includes an experimental GPT explainer. This
+explainer leverages the outcomes produced by SHAP and MACE to formulate the
+input prompt for ChatGPT. Subsequently, ChatGPT analyzes these results and
+generates the corresponding explanations that provide developers with a clearer
+understanding of the rationale behind the model's predictions. ## Introduction
+OmniXAI (short for Omni eXplainable AI) is a Python machine-learning library
+for explainable AI (XAI), offering omni-way explainable AI and interpretable
+machine learning capabilities to address many pain points in explaining
+decisions made by machine learning models in practice. OmniXAI aims to be a
+one-stop comprehensive library that makes explainable AI easy for data
+scientists, ML researchers and practitioners who need explanation for various
+types of data, models and explanation methods at different stages of ML
+process: ![alt text](https://github.com/salesforce/OmniXAI/raw/main/docs/
+_static/ml_pipeline.png) OmniXAI includes a rich family of explanation methods
+integrated in a unified interface, which supports multiple data types (tabular
+data, images, texts, time-series), multiple types of ML models (traditional ML
+in Scikit-learn and deep learning models in PyTorch/TensorFlow), and a range of
+diverse explaination methods including "model-specific" and "model-agnostic"
+methods (such as feature-attribution explanation, counterfactual explanation,
+gradient-based explanation, feature visualization, etc). For practitioners,
+OmniXAI provides an easy-to-use unified interface to generate the explanations
+for their applications by only writing a few lines of codes, and also a GUI
 dashboard for visualization for obtaining more insights about decisions. The
 following table shows the supported explanation methods and features in our
 library. We will continue improving this library to make it more comprehensive
 in the future. | Method | Model Type | Explanation Type | EDA | Tabular | Image
 | Text | Timeseries | :-------------------------:|:-------------:|:------------
 ----:|:---:|:-------:|:-----:| :---: | :---: | Feature analysis | NA | Global |
 â | | | | | | Feature selection | NA | Global | â | | | | | | Prediction
@@ -85,80 +85,81 @@
 ``pip install omnixai[nlp]``, or ``pip install .[nlp]`` from the root directory
 of the repo. - **Install all the dependencies**: Calling ``pip install omnixai
 [all]``, or ``pip install .[all]`` from the root directory of the repo. ##
 Getting Started For example code and an introduction to the library, see the
 Jupyter notebooks in [tutorials](https://opensource.salesforce.com/OmniXAI/
 latest/tutorials.html), and the guided walkthrough [here](https://
 opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be
-found [here](https://sfr-omnixai-demo.herokuapp.com/). Some examples: 1.
-[Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/tabular_classification.ipynb) 2. [Tabular regression](https://
-github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb) 3.
-[Image classification](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/vision.ipynb) 4. [Text classification](https://github.com/salesforce/
-OmniXAI/blob/main/tutorials/nlp_imdb.ipynb) 5. [Time-series anomaly detection]
-(https://github.com/salesforce/OmniXAI/blob/main/tutorials/timeseries.ipynb) 6.
-[Vision-language tasks](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/vision/gradcam_vlm.ipynb) 7. [Ranking tasks](https://github.com/
-salesforce/OmniXAI/blob/main/tutorials/tabular/ranking.ipynb) 8. [Feature
-visualization](https://github.com/salesforce/OmniXAI/blob/main/tutorials/
-vision/feature_visualization_torch.ipynb) 9. [Check feature maps](https://
-github.com/salesforce/OmniXAI/blob/main/tutorials/vision/
-feature_map_torch.ipynb) To get started, we recommend the linked tutorials in
-[tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html).
-In general, we recommend using `TabularExplainer`, `VisionExplainer`,
-`NLPExplainer` and `TimeseriesExplainer` for tabular, vision, NLP and time-
-series tasks, respectively, and using `DataAnalyzer` and `PredictionAnalyzer`
-for feature analysis and prediction result analysis. These classes act as the
-factories of the individual explainers supported in OmniXAI, providing a
-simpler interface to generate multiple explanations. To generate explanations,
-you only need to specify - **The ML model to explain**: e.g., a scikit-learn
-model, a tensorflow model, a pytorch model or a black-box prediction function.
-- **The pre-processing function**: i.e., converting raw input features into the
-model inputs. - **The post-processing function (optional)**: e.g., converting
-the model outputs into class probabilities. - **The explainers to apply**:
-e.g., SHAP, MACE, Grad-CAM. Besides using these classes, you can also create a
-single explainer defined in the `omnixai.explainers` package, e.g.,
-`ShapTabular`, `GradCAM`, `IntegratedGradient` or `FeatureVisualizer`. Let's
-take the income prediction task as an example. The [dataset](https://
-archive.ics.uci.edu/ml/datasets/adult) used in this example is for income
-prediction. We recommend using data class `Tabular` to represent a tabular
-dataset. To create a `Tabular` instance given a pandas dataframe, you need to
-specify the dataframe, the categorical feature names (if exists) and the
-target/label column name (if exists). ```python from omnixai.data.tabular
-import Tabular # Load the dataset feature_names = [ "Age", "Workclass",
-"fnlwgt", "Education", "Education-Num", "Marital Status", "Occupation",
-"Relationship", "Race", "Sex", "Capital Gain", "Capital Loss", "Hours per
-week", "Country", "label" ] df = pd.DataFrame( np.genfromtxt('adult.data',
-delimiter=', ', dtype=str), columns=feature_names ) tabular_data = Tabular( df,
-categorical_columns=[feature_names[i] for i in [1, 3, 5, 6, 7, 8, 9, 13]],
-target_column='label' ) ``` The package `omnixai.preprocessing` provides
-several useful preprocessing functions for a `Tabular` instance.
-`TabularTransform` is a special transform designed for processing tabular data.
-By default, it converts categorical features into one-hot encoding, and keeps
-continuous-valued features. The method ``transform`` of `TabularTransform`
-transforms a `Tabular` instance to a numpy array. If the `Tabular` instance has
-a target/label column, the last column of the numpy array will be the target/
-label. You can apply any customized preprocessing functions instead of using
-`TabularTransform`. After data preprocessing, let's train a XGBoost classifier
-for this task. ```python from omnixai.preprocessing.tabular import
-TabularTransform # Data preprocessing transformer = TabularTransform().fit
-(tabular_data) class_names = transformer.class_names x = transformer.transform
-(tabular_data) # Split into training and test datasets train, test,
-train_labels, test_labels = \ sklearn.model_selection.train_test_split(x[:, :-
-1], x[:, -1], train_size=0.80) # Train an XGBoost model (the last column of `x`
-is the label column after transformation) model = xgboost.XGBClassifier
-(n_estimators=300, max_depth=5) model.fit(train, train_labels) # Convert the
-transformed data back to Tabular instances train_data = transformer.invert
-(train) test_data = transformer.invert(test) ``` To initialize
-`TabularExplainer`, the following parameters need to be set: - ``explainers``:
-The names of the explainers to apply, e.g., ["lime", "shap", "mace", "pdp"]. -
-``data``: The data used to initialize explainers. ``data`` is the training
-dataset for training the machine learning model. If the training dataset is too
-large, ``data`` can be a subset of it by applying
+found [here](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/). Some
+examples: 1. [Tabular classification](https://github.com/salesforce/OmniXAI/
+blob/main/tutorials/tabular_classification.ipynb) 2. [Tabular regression]
+(https://github.com/salesforce/OmniXAI/blob/main/tutorials/
+tabular_regression.ipynb) 3. [Image classification](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/vision.ipynb) 4. [Text classification]
+(https://github.com/salesforce/OmniXAI/blob/main/tutorials/nlp_imdb.ipynb) 5.
+[Time-series anomaly detection](https://github.com/salesforce/OmniXAI/blob/
+main/tutorials/timeseries.ipynb) 6. [Vision-language tasks](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/vision/gradcam_vlm.ipynb) 7. [Ranking
+tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/
+ranking.ipynb) 8. [Feature visualization](https://github.com/salesforce/
+OmniXAI/blob/main/tutorials/vision/feature_visualization_torch.ipynb) 9. [Check
+feature maps](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/
+feature_map_torch.ipynb) 10. [GPT explainer for tabular](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/tabular/gpt.ipynb) To get started, we
+recommend the linked tutorials in [tutorials](https://
+opensource.salesforce.com/OmniXAI/latest/tutorials.html). In general, we
+recommend using `TabularExplainer`, `VisionExplainer`, `NLPExplainer` and
+`TimeseriesExplainer` for tabular, vision, NLP and time-series tasks,
+respectively, and using `DataAnalyzer` and `PredictionAnalyzer` for feature
+analysis and prediction result analysis. These classes act as the factories of
+the individual explainers supported in OmniXAI, providing a simpler interface
+to generate multiple explanations. To generate explanations, you only need to
+specify - **The ML model to explain**: e.g., a scikit-learn model, a tensorflow
+model, a pytorch model or a black-box prediction function. - **The pre-
+processing function**: i.e., converting raw input features into the model
+inputs. - **The post-processing function (optional)**: e.g., converting the
+model outputs into class probabilities. - **The explainers to apply**: e.g.,
+SHAP, MACE, Grad-CAM. Besides using these classes, you can also create a single
+explainer defined in the `omnixai.explainers` package, e.g., `ShapTabular`,
+`GradCAM`, `IntegratedGradient` or `FeatureVisualizer`. Let's take the income
+prediction task as an example. The [dataset](https://archive.ics.uci.edu/ml/
+datasets/adult) used in this example is for income prediction. We recommend
+using data class `Tabular` to represent a tabular dataset. To create a
+`Tabular` instance given a pandas dataframe, you need to specify the dataframe,
+the categorical feature names (if exists) and the target/label column name (if
+exists). ```python from omnixai.data.tabular import Tabular # Load the dataset
+feature_names = [ "Age", "Workclass", "fnlwgt", "Education", "Education-Num",
+"Marital Status", "Occupation", "Relationship", "Race", "Sex", "Capital Gain",
+"Capital Loss", "Hours per week", "Country", "label" ] df = pd.DataFrame
+( np.genfromtxt('adult.data', delimiter=', ', dtype=str), columns=feature_names
+) tabular_data = Tabular( df, categorical_columns=[feature_names[i] for i in
+[1, 3, 5, 6, 7, 8, 9, 13]], target_column='label' ) ``` The package
+`omnixai.preprocessing` provides several useful preprocessing functions for a
+`Tabular` instance. `TabularTransform` is a special transform designed for
+processing tabular data. By default, it converts categorical features into one-
+hot encoding, and keeps continuous-valued features. The method ``transform`` of
+`TabularTransform` transforms a `Tabular` instance to a numpy array. If the
+`Tabular` instance has a target/label column, the last column of the numpy
+array will be the target/label. You can apply any customized preprocessing
+functions instead of using `TabularTransform`. After data preprocessing, let's
+train a XGBoost classifier for this task. ```python from
+omnixai.preprocessing.tabular import TabularTransform # Data preprocessing
+transformer = TabularTransform().fit(tabular_data) class_names =
+transformer.class_names x = transformer.transform(tabular_data) # Split into
+training and test datasets train, test, train_labels, test_labels = \
+sklearn.model_selection.train_test_split(x[:, :-1], x[:, -1], train_size=0.80)
+# Train an XGBoost model (the last column of `x` is the label column after
+transformation) model = xgboost.XGBClassifier(n_estimators=300, max_depth=5)
+model.fit(train, train_labels) # Convert the transformed data back to Tabular
+instances train_data = transformer.invert(train) test_data = transformer.invert
+(test) ``` To initialize `TabularExplainer`, the following parameters need to
+be set: - ``explainers``: The names of the explainers to apply, e.g., ["lime",
+"shap", "mace", "pdp"]. - ``data``: The data used to initialize explainers.
+``data`` is the training dataset for training the machine learning model. If
+the training dataset is too large, ``data`` can be a subset of it by applying
 `omnixai.sampler.tabular.Sampler.subsample`. - ``model``: The ML model to
 explain, e.g., a scikit-learn model, a tensorflow model or a pytorch model. -
 ``preprocess``: The preprocessing function converting the raw inputs (A
 `Tabular` instance) into the inputs of ``model``. - ``postprocess`` (optional):
 The postprocessing function transforming the outputs of ``model`` to a user-
 specific form, e.g., the predicted probability for each class. The output of
 `postprocess` should be a numpy array. - ``mode``: The task type, e.g.,
```

### Comparing `omnixai-1.3.0/README.md` & `omnixai-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ## Table of Contents
 1. [Introduction](#introduction)
 2. [Installation](#installation)
 3. [Getting Started](#getting-started)
 4. [Documentation](https://opensource.salesforce.com/OmniXAI/latest/index.html)
 5. [Tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html)
 6. [Deployment](#deployment)
-7. [Dashboard Demo](https://sfr-omnixai-demo.herokuapp.com/)
+7. [Dashboard Demo](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/)
 8. [How to Contribute](https://opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute)
 9. [Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai)
 
 ## What's New
 
 The latest version includes an experimental GPT explainer. This explainer leverages the outcomes 
 produced by SHAP and MACE to formulate the input prompt for ChatGPT. Subsequently, ChatGPT 
@@ -116,26 +116,27 @@
 - **Install all the dependencies**: Calling ``pip install omnixai[all]``, or ``pip install .[all]`` from the
   root directory of the repo.
 
 ## Getting Started
 
 For example code and an introduction to the library, see the Jupyter notebooks in
 [tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html), and the guided walkthrough
-[here](https://opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be found [here](https://sfr-omnixai-demo.herokuapp.com/).
+[here](https://opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be found [here](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/).
 
 Some examples:
 1. [Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_classification.ipynb)
 2. [Tabular regression](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb)
 3. [Image classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision.ipynb)
 4. [Text classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/nlp_imdb.ipynb)
 5. [Time-series anomaly detection](https://github.com/salesforce/OmniXAI/blob/main/tutorials/timeseries.ipynb)
 6. [Vision-language tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/gradcam_vlm.ipynb)
 7. [Ranking tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/ranking.ipynb)
 8. [Feature visualization](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/feature_visualization_torch.ipynb)
 9. [Check feature maps](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/feature_map_torch.ipynb)
+10. [GPT explainer for tabular](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/gpt.ipynb)
 
 To get started, we recommend the linked tutorials in [tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html).
 In general, we recommend using `TabularExplainer`, `VisionExplainer`,
 `NLPExplainer` and `TimeseriesExplainer` for tabular, vision, NLP and time-series tasks, respectively, and using
 `DataAnalyzer` and `PredictionAnalyzer` for feature analysis and prediction result analysis.
 These classes act as the factories of the individual explainers supported in OmniXAI, providing a simpler
 interface to generate multiple explanations. To generate explanations, you only need to specify
```

#### html2text {}

```diff
@@ -3,40 +3,40 @@
 # OmniXAI: A Library for Explainable AI
     [https://img.shields.io/badge/Python-3.7,_3.8,_3.9,_3.10-blue] [PyPI]
                        [Documentation] [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://opensource.salesforce.com/OmniXAI/latest/index.html) 5. [Tutorials]
 (https://opensource.salesforce.com/OmniXAI/latest/tutorials.html) 6.
-[Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-
-demo.herokuapp.com/) 8. [How to Contribute](https://opensource.salesforce.com/
-OmniXAI/latest/omnixai.html#how-to-contribute) 9. [Technical Report and Citing
-OmniXAI](#technical-report-and-citing-omnixai) ## What's New The latest version
-includes an experimental GPT explainer. This explainer leverages the outcomes
-produced by SHAP and MACE to formulate the input prompt for ChatGPT.
-Subsequently, ChatGPT analyzes these results and generates the corresponding
-explanations that provide developers with a clearer understanding of the
-rationale behind the model's predictions. ## Introduction OmniXAI (short for
-Omni eXplainable AI) is a Python machine-learning library for explainable AI
-(XAI), offering omni-way explainable AI and interpretable machine learning
-capabilities to address many pain points in explaining decisions made by
-machine learning models in practice. OmniXAI aims to be a one-stop
-comprehensive library that makes explainable AI easy for data scientists, ML
-researchers and practitioners who need explanation for various types of data,
-models and explanation methods at different stages of ML process: ![alt text]
-(https://github.com/salesforce/OmniXAI/raw/main/docs/_static/ml_pipeline.png)
-OmniXAI includes a rich family of explanation methods integrated in a unified
-interface, which supports multiple data types (tabular data, images, texts,
-time-series), multiple types of ML models (traditional ML in Scikit-learn and
-deep learning models in PyTorch/TensorFlow), and a range of diverse
-explaination methods including "model-specific" and "model-agnostic" methods
-(such as feature-attribution explanation, counterfactual explanation, gradient-
-based explanation, feature visualization, etc). For practitioners, OmniXAI
-provides an easy-to-use unified interface to generate the explanations for
-their applications by only writing a few lines of codes, and also a GUI
+[Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-demo-
+cc9e4edb6447.herokuapp.com/) 8. [How to Contribute](https://
+opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute) 9.
+[Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai) ##
+What's New The latest version includes an experimental GPT explainer. This
+explainer leverages the outcomes produced by SHAP and MACE to formulate the
+input prompt for ChatGPT. Subsequently, ChatGPT analyzes these results and
+generates the corresponding explanations that provide developers with a clearer
+understanding of the rationale behind the model's predictions. ## Introduction
+OmniXAI (short for Omni eXplainable AI) is a Python machine-learning library
+for explainable AI (XAI), offering omni-way explainable AI and interpretable
+machine learning capabilities to address many pain points in explaining
+decisions made by machine learning models in practice. OmniXAI aims to be a
+one-stop comprehensive library that makes explainable AI easy for data
+scientists, ML researchers and practitioners who need explanation for various
+types of data, models and explanation methods at different stages of ML
+process: ![alt text](https://github.com/salesforce/OmniXAI/raw/main/docs/
+_static/ml_pipeline.png) OmniXAI includes a rich family of explanation methods
+integrated in a unified interface, which supports multiple data types (tabular
+data, images, texts, time-series), multiple types of ML models (traditional ML
+in Scikit-learn and deep learning models in PyTorch/TensorFlow), and a range of
+diverse explaination methods including "model-specific" and "model-agnostic"
+methods (such as feature-attribution explanation, counterfactual explanation,
+gradient-based explanation, feature visualization, etc). For practitioners,
+OmniXAI provides an easy-to-use unified interface to generate the explanations
+for their applications by only writing a few lines of codes, and also a GUI
 dashboard for visualization for obtaining more insights about decisions. The
 following table shows the supported explanation methods and features in our
 library. We will continue improving this library to make it more comprehensive
 in the future. | Method | Model Type | Explanation Type | EDA | Tabular | Image
 | Text | Timeseries | :-------------------------:|:-------------:|:------------
 ----:|:---:|:-------:|:-----:| :---: | :---: | Feature analysis | NA | Global |
 â | | | | | | Feature selection | NA | Global | â | | | | | | Prediction
@@ -78,80 +78,81 @@
 ``pip install omnixai[nlp]``, or ``pip install .[nlp]`` from the root directory
 of the repo. - **Install all the dependencies**: Calling ``pip install omnixai
 [all]``, or ``pip install .[all]`` from the root directory of the repo. ##
 Getting Started For example code and an introduction to the library, see the
 Jupyter notebooks in [tutorials](https://opensource.salesforce.com/OmniXAI/
 latest/tutorials.html), and the guided walkthrough [here](https://
 opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be
-found [here](https://sfr-omnixai-demo.herokuapp.com/). Some examples: 1.
-[Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/tabular_classification.ipynb) 2. [Tabular regression](https://
-github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb) 3.
-[Image classification](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/vision.ipynb) 4. [Text classification](https://github.com/salesforce/
-OmniXAI/blob/main/tutorials/nlp_imdb.ipynb) 5. [Time-series anomaly detection]
-(https://github.com/salesforce/OmniXAI/blob/main/tutorials/timeseries.ipynb) 6.
-[Vision-language tasks](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/vision/gradcam_vlm.ipynb) 7. [Ranking tasks](https://github.com/
-salesforce/OmniXAI/blob/main/tutorials/tabular/ranking.ipynb) 8. [Feature
-visualization](https://github.com/salesforce/OmniXAI/blob/main/tutorials/
-vision/feature_visualization_torch.ipynb) 9. [Check feature maps](https://
-github.com/salesforce/OmniXAI/blob/main/tutorials/vision/
-feature_map_torch.ipynb) To get started, we recommend the linked tutorials in
-[tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html).
-In general, we recommend using `TabularExplainer`, `VisionExplainer`,
-`NLPExplainer` and `TimeseriesExplainer` for tabular, vision, NLP and time-
-series tasks, respectively, and using `DataAnalyzer` and `PredictionAnalyzer`
-for feature analysis and prediction result analysis. These classes act as the
-factories of the individual explainers supported in OmniXAI, providing a
-simpler interface to generate multiple explanations. To generate explanations,
-you only need to specify - **The ML model to explain**: e.g., a scikit-learn
-model, a tensorflow model, a pytorch model or a black-box prediction function.
-- **The pre-processing function**: i.e., converting raw input features into the
-model inputs. - **The post-processing function (optional)**: e.g., converting
-the model outputs into class probabilities. - **The explainers to apply**:
-e.g., SHAP, MACE, Grad-CAM. Besides using these classes, you can also create a
-single explainer defined in the `omnixai.explainers` package, e.g.,
-`ShapTabular`, `GradCAM`, `IntegratedGradient` or `FeatureVisualizer`. Let's
-take the income prediction task as an example. The [dataset](https://
-archive.ics.uci.edu/ml/datasets/adult) used in this example is for income
-prediction. We recommend using data class `Tabular` to represent a tabular
-dataset. To create a `Tabular` instance given a pandas dataframe, you need to
-specify the dataframe, the categorical feature names (if exists) and the
-target/label column name (if exists). ```python from omnixai.data.tabular
-import Tabular # Load the dataset feature_names = [ "Age", "Workclass",
-"fnlwgt", "Education", "Education-Num", "Marital Status", "Occupation",
-"Relationship", "Race", "Sex", "Capital Gain", "Capital Loss", "Hours per
-week", "Country", "label" ] df = pd.DataFrame( np.genfromtxt('adult.data',
-delimiter=', ', dtype=str), columns=feature_names ) tabular_data = Tabular( df,
-categorical_columns=[feature_names[i] for i in [1, 3, 5, 6, 7, 8, 9, 13]],
-target_column='label' ) ``` The package `omnixai.preprocessing` provides
-several useful preprocessing functions for a `Tabular` instance.
-`TabularTransform` is a special transform designed for processing tabular data.
-By default, it converts categorical features into one-hot encoding, and keeps
-continuous-valued features. The method ``transform`` of `TabularTransform`
-transforms a `Tabular` instance to a numpy array. If the `Tabular` instance has
-a target/label column, the last column of the numpy array will be the target/
-label. You can apply any customized preprocessing functions instead of using
-`TabularTransform`. After data preprocessing, let's train a XGBoost classifier
-for this task. ```python from omnixai.preprocessing.tabular import
-TabularTransform # Data preprocessing transformer = TabularTransform().fit
-(tabular_data) class_names = transformer.class_names x = transformer.transform
-(tabular_data) # Split into training and test datasets train, test,
-train_labels, test_labels = \ sklearn.model_selection.train_test_split(x[:, :-
-1], x[:, -1], train_size=0.80) # Train an XGBoost model (the last column of `x`
-is the label column after transformation) model = xgboost.XGBClassifier
-(n_estimators=300, max_depth=5) model.fit(train, train_labels) # Convert the
-transformed data back to Tabular instances train_data = transformer.invert
-(train) test_data = transformer.invert(test) ``` To initialize
-`TabularExplainer`, the following parameters need to be set: - ``explainers``:
-The names of the explainers to apply, e.g., ["lime", "shap", "mace", "pdp"]. -
-``data``: The data used to initialize explainers. ``data`` is the training
-dataset for training the machine learning model. If the training dataset is too
-large, ``data`` can be a subset of it by applying
+found [here](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/). Some
+examples: 1. [Tabular classification](https://github.com/salesforce/OmniXAI/
+blob/main/tutorials/tabular_classification.ipynb) 2. [Tabular regression]
+(https://github.com/salesforce/OmniXAI/blob/main/tutorials/
+tabular_regression.ipynb) 3. [Image classification](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/vision.ipynb) 4. [Text classification]
+(https://github.com/salesforce/OmniXAI/blob/main/tutorials/nlp_imdb.ipynb) 5.
+[Time-series anomaly detection](https://github.com/salesforce/OmniXAI/blob/
+main/tutorials/timeseries.ipynb) 6. [Vision-language tasks](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/vision/gradcam_vlm.ipynb) 7. [Ranking
+tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/
+ranking.ipynb) 8. [Feature visualization](https://github.com/salesforce/
+OmniXAI/blob/main/tutorials/vision/feature_visualization_torch.ipynb) 9. [Check
+feature maps](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/
+feature_map_torch.ipynb) 10. [GPT explainer for tabular](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/tabular/gpt.ipynb) To get started, we
+recommend the linked tutorials in [tutorials](https://
+opensource.salesforce.com/OmniXAI/latest/tutorials.html). In general, we
+recommend using `TabularExplainer`, `VisionExplainer`, `NLPExplainer` and
+`TimeseriesExplainer` for tabular, vision, NLP and time-series tasks,
+respectively, and using `DataAnalyzer` and `PredictionAnalyzer` for feature
+analysis and prediction result analysis. These classes act as the factories of
+the individual explainers supported in OmniXAI, providing a simpler interface
+to generate multiple explanations. To generate explanations, you only need to
+specify - **The ML model to explain**: e.g., a scikit-learn model, a tensorflow
+model, a pytorch model or a black-box prediction function. - **The pre-
+processing function**: i.e., converting raw input features into the model
+inputs. - **The post-processing function (optional)**: e.g., converting the
+model outputs into class probabilities. - **The explainers to apply**: e.g.,
+SHAP, MACE, Grad-CAM. Besides using these classes, you can also create a single
+explainer defined in the `omnixai.explainers` package, e.g., `ShapTabular`,
+`GradCAM`, `IntegratedGradient` or `FeatureVisualizer`. Let's take the income
+prediction task as an example. The [dataset](https://archive.ics.uci.edu/ml/
+datasets/adult) used in this example is for income prediction. We recommend
+using data class `Tabular` to represent a tabular dataset. To create a
+`Tabular` instance given a pandas dataframe, you need to specify the dataframe,
+the categorical feature names (if exists) and the target/label column name (if
+exists). ```python from omnixai.data.tabular import Tabular # Load the dataset
+feature_names = [ "Age", "Workclass", "fnlwgt", "Education", "Education-Num",
+"Marital Status", "Occupation", "Relationship", "Race", "Sex", "Capital Gain",
+"Capital Loss", "Hours per week", "Country", "label" ] df = pd.DataFrame
+( np.genfromtxt('adult.data', delimiter=', ', dtype=str), columns=feature_names
+) tabular_data = Tabular( df, categorical_columns=[feature_names[i] for i in
+[1, 3, 5, 6, 7, 8, 9, 13]], target_column='label' ) ``` The package
+`omnixai.preprocessing` provides several useful preprocessing functions for a
+`Tabular` instance. `TabularTransform` is a special transform designed for
+processing tabular data. By default, it converts categorical features into one-
+hot encoding, and keeps continuous-valued features. The method ``transform`` of
+`TabularTransform` transforms a `Tabular` instance to a numpy array. If the
+`Tabular` instance has a target/label column, the last column of the numpy
+array will be the target/label. You can apply any customized preprocessing
+functions instead of using `TabularTransform`. After data preprocessing, let's
+train a XGBoost classifier for this task. ```python from
+omnixai.preprocessing.tabular import TabularTransform # Data preprocessing
+transformer = TabularTransform().fit(tabular_data) class_names =
+transformer.class_names x = transformer.transform(tabular_data) # Split into
+training and test datasets train, test, train_labels, test_labels = \
+sklearn.model_selection.train_test_split(x[:, :-1], x[:, -1], train_size=0.80)
+# Train an XGBoost model (the last column of `x` is the label column after
+transformation) model = xgboost.XGBClassifier(n_estimators=300, max_depth=5)
+model.fit(train, train_labels) # Convert the transformed data back to Tabular
+instances train_data = transformer.invert(train) test_data = transformer.invert
+(test) ``` To initialize `TabularExplainer`, the following parameters need to
+be set: - ``explainers``: The names of the explainers to apply, e.g., ["lime",
+"shap", "mace", "pdp"]. - ``data``: The data used to initialize explainers.
+``data`` is the training dataset for training the machine learning model. If
+the training dataset is too large, ``data`` can be a subset of it by applying
 `omnixai.sampler.tabular.Sampler.subsample`. - ``model``: The ML model to
 explain, e.g., a scikit-learn model, a tensorflow model or a pytorch model. -
 ``preprocess``: The preprocessing function converting the raw inputs (A
 `Tabular` instance) into the inputs of ``model``. - ``postprocess`` (optional):
 The postprocessing function transforming the outputs of ``model`` to a user-
 specific form, e.g., the predicted probability for each class. The output of
 `postprocess` should be a numpy array. - ``mode``: The task type, e.g.,
```

### Comparing `omnixai-1.3.0/docs/conf.py` & `omnixai-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/data/base.py` & `omnixai-1.3.1/omnixai/data/base.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/data/image.py` & `omnixai-1.3.1/omnixai/data/image.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/data/multi_inputs.py` & `omnixai-1.3.1/omnixai/data/multi_inputs.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/data/tabular.py` & `omnixai-1.3.1/omnixai/data/tabular.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/data/text.py` & `omnixai-1.3.1/omnixai/data/text.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/data/timeseries.py` & `omnixai-1.3.1/omnixai/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/deployment/bentoml/omnixai.py` & `omnixai-1.3.1/omnixai/deployment/bentoml/omnixai.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/base.py` & `omnixai-1.3.1/omnixai/explainers/base.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/data/__init__.py` & `omnixai-1.3.1/omnixai/explainers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/data/auto.py` & `omnixai-1.3.1/omnixai/explainers/data/auto.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/data/chi_square.py` & `omnixai-1.3.1/omnixai/explainers/data/chi_square.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/data/correlation.py` & `omnixai-1.3.1/omnixai/explainers/data/correlation.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/data/imbalance.py` & `omnixai-1.3.1/omnixai/explainers/data/imbalance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/data/mutual_info.py` & `omnixai-1.3.1/omnixai/explainers/data/mutual_info.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/nlp/__init__.py` & `omnixai-1.3.1/omnixai/explainers/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/nlp/agnostic/l2x.py` & `omnixai-1.3.1/omnixai/explainers/nlp/agnostic/l2x.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/nlp/agnostic/lime.py` & `omnixai-1.3.1/omnixai/explainers/nlp/agnostic/lime.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/nlp/agnostic/shap.py` & `omnixai-1.3.1/omnixai/explainers/nlp/agnostic/shap.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/nlp/auto.py` & `omnixai-1.3.1/omnixai/explainers/nlp/auto.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/polyjuice.py` & `omnixai-1.3.1/omnixai/explainers/nlp/counterfactual/polyjuice.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/nlp/specific/ig.py` & `omnixai-1.3.1/omnixai/explainers/nlp/specific/ig.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/prediction/auto.py` & `omnixai-1.3.1/omnixai/explainers/prediction/auto.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/ranking/agnostic/permutation.py` & `omnixai-1.3.1/omnixai/explainers/ranking/agnostic/permutation.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/ranking/agnostic/validity.py` & `omnixai-1.3.1/omnixai/explainers/ranking/agnostic/validity.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/mace.py` & `omnixai-1.3.1/omnixai/explainers/ranking/counterfactual/mace.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/__init__.py` & `omnixai-1.3.1/omnixai/explainers/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/l2x.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/L2X/l2x.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/utils.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/L2X/utils.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/ale.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/ale.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/bias.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/bias.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/gpt.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/gpt.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/lime.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/lime.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/pdp.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/pdp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/permutation.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/permutation.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/sensitivity.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/sensitivity.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/shap.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap_global.py` & `omnixai-1.3.1/omnixai/explainers/tabular/agnostic/shap_global.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/auto.py` & `omnixai-1.3.1/omnixai/explainers/tabular/auto.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/base.py` & `omnixai-1.3.1/omnixai/explainers/tabular/base.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/ce.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/ce.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/knn.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/knn.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/diversify.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/diversify.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/gld.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/gld.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/greedy.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/greedy.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/mace.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/mace.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/refine.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/refine.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/retrieval.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/retrieval.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/rl.py` & `omnixai-1.3.1/omnixai/explainers/tabular/counterfactual/mace/rl.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/specific/decision_tree.py` & `omnixai-1.3.1/omnixai/explainers/tabular/specific/decision_tree.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/specific/ig.py` & `omnixai-1.3.1/omnixai/explainers/tabular/specific/ig.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/specific/linear.py` & `omnixai-1.3.1/omnixai/explainers/tabular/specific/linear.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/tabular/specific/shap_tree.py` & `omnixai-1.3.1/omnixai/explainers/tabular/specific/shap_tree.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/timeseries/__init__.py` & `omnixai-1.3.1/omnixai/explainers/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/shap.py` & `omnixai-1.3.1/omnixai/explainers/timeseries/agnostic/shap.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/timeseries/auto.py` & `omnixai-1.3.1/omnixai/explainers/timeseries/auto.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/ce.py` & `omnixai-1.3.1/omnixai/explainers/timeseries/counterfactual/ce.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/mace.py` & `omnixai-1.3.1/omnixai/explainers/timeseries/counterfactual/mace.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/__init__.py` & `omnixai-1.3.1/omnixai/explainers/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/agnostic/l2x.py` & `omnixai-1.3.1/omnixai/explainers/vision/agnostic/l2x.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/agnostic/lime.py` & `omnixai-1.3.1/omnixai/explainers/vision/agnostic/lime.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/agnostic/pdp.py` & `omnixai-1.3.1/omnixai/explainers/vision/agnostic/pdp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/agnostic/shap.py` & `omnixai-1.3.1/omnixai/explainers/vision/agnostic/shap.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/auto.py` & `omnixai-1.3.1/omnixai/explainers/vision/auto.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/counterfactual/ce.py` & `omnixai-1.3.1/omnixai/explainers/vision/counterfactual/ce.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/cem.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/cem.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/feature_maps.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/feature_maps.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/utils.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/utils.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/visualizer.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/feature_visualization/visualizer.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/gradcam.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/gradcam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/guided_bp.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/guided_bp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/ig.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/ig.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/scorecam.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/scorecam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/utils.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/scorecam/utils.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/smoothgrad.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/smoothgrad.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision/specific/utils.py` & `omnixai-1.3.1/omnixai/explainers/vision/specific/utils.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/gradcam.py` & `omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/gradcam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py` & `omnixai-1.3.1/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explainers/vision_language/specific/ig.py` & `omnixai-1.3.1/omnixai/explainers/vision_language/specific/ig.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/base.py` & `omnixai-1.3.1/omnixai/explanations/base.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/image/contrast.py` & `omnixai-1.3.1/omnixai/explanations/image/contrast.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/image/counterfactual.py` & `omnixai-1.3.1/omnixai/explanations/image/counterfactual.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/image/mask.py` & `omnixai-1.3.1/omnixai/explanations/image/mask.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/image/pixel_importance.py` & `omnixai-1.3.1/omnixai/explanations/image/pixel_importance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/image/plain.py` & `omnixai-1.3.1/omnixai/explanations/image/plain.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/prediction/confusion.py` & `omnixai-1.3.1/omnixai/explanations/prediction/confusion.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/prediction/cumulative.py` & `omnixai-1.3.1/omnixai/explanations/prediction/cumulative.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/prediction/lift.py` & `omnixai-1.3.1/omnixai/explanations/prediction/lift.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/prediction/metrics.py` & `omnixai-1.3.1/omnixai/explanations/prediction/metrics.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/prediction/pr.py` & `omnixai-1.3.1/omnixai/explanations/prediction/pr.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/prediction/residual.py` & `omnixai-1.3.1/omnixai/explanations/prediction/residual.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/prediction/roc.py` & `omnixai-1.3.1/omnixai/explanations/prediction/roc.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/ale.py` & `omnixai-1.3.1/omnixai/explanations/tabular/ale.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/bias.py` & `omnixai-1.3.1/omnixai/explanations/tabular/bias.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/correlation.py` & `omnixai-1.3.1/omnixai/explanations/tabular/correlation.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/counterfactual.py` & `omnixai-1.3.1/omnixai/explanations/tabular/counterfactual.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/feature_importance.py` & `omnixai-1.3.1/omnixai/explanations/tabular/feature_importance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/imbalance.py` & `omnixai-1.3.1/omnixai/explanations/tabular/imbalance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/linear.py` & `omnixai-1.3.1/omnixai/explanations/tabular/linear.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/pdp.py` & `omnixai-1.3.1/omnixai/explanations/tabular/pdp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/sensitivity.py` & `omnixai-1.3.1/omnixai/explanations/tabular/sensitivity.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/tree.py` & `omnixai-1.3.1/omnixai/explanations/tabular/tree.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/tabular/validity.py` & `omnixai-1.3.1/omnixai/explanations/tabular/validity.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/text/word_importance.py` & `omnixai-1.3.1/omnixai/explanations/text/word_importance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/timeseries/counterfactual.py` & `omnixai-1.3.1/omnixai/explanations/timeseries/counterfactual.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/timeseries/feature_importance.py` & `omnixai-1.3.1/omnixai/explanations/timeseries/feature_importance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/explanations/utils.py` & `omnixai-1.3.1/omnixai/explanations/utils.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/preprocessing/base.py` & `omnixai-1.3.1/omnixai/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/preprocessing/encode.py` & `omnixai-1.3.1/omnixai/preprocessing/encode.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/preprocessing/fill.py` & `omnixai-1.3.1/omnixai/preprocessing/fill.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/preprocessing/image.py` & `omnixai-1.3.1/omnixai/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/preprocessing/normalize.py` & `omnixai-1.3.1/omnixai/preprocessing/normalize.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/preprocessing/pipeline.py` & `omnixai-1.3.1/omnixai/preprocessing/pipeline.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/preprocessing/tabular.py` & `omnixai-1.3.1/omnixai/preprocessing/tabular.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,41 +5,46 @@
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The pre-processing function for tabular data.
 """
 import numpy as np
 import pandas as pd
+from typing import Optional
 from .base import TransformBase, Identity
 from .encode import OneHot, Ordinal, LabelEncoder
 from ..data.tabular import Tabular
 
 
 class TabularTransform(TransformBase):
     """
     Transforms for a ``data.tabular.Tabular`` instance.
     """
 
     def __init__(
         self,
-        cate_transform: TransformBase = OneHot(),
-        cont_transform: TransformBase = Identity(),
-        target_transform: TransformBase = LabelEncoder(),
+        cate_transform: Optional[TransformBase] = None,
+        cont_transform: Optional[TransformBase] = None,
+        target_transform: Optional[TransformBase] = None,
     ):
         """
         :param cate_transform: The transform for the categorical features, e.g.,
-            `OneHot`, `Ordinal`.
+            `OneHot`, `Ordinal`. Default is `OneHot`.
         :param cont_transform: The transform for the continuous-valued features,
-            e.g., `Identity`, `Standard`, `MinMax`, `Scale`.
+            e.g., `Identity`, `Standard`, `MinMax`, `Scale`. Default is `Identity`.
         :param target_transform: The transform for the target column, e.g.,
-            `Identity` for regression, `LabelEncoder` for classification.
+            `Identity` for regression, `LabelEncoder` for classification. Default is `LabelEncoder`.
         """
         super().__init__()
-        assert cate_transform is not None, "Transform for categorical features cannot be None."
-        assert cont_transform is not None, "Transform for continuous-valued features cannot be None."
+        if cate_transform is None:
+            cate_transform = OneHot()
+        if cont_transform is None:
+            cont_transform = Identity()
+        if target_transform is None:
+            target_transform = LabelEncoder()
 
         # Feature column
         self.cate_transform = cate_transform
         self.cont_transform = cont_transform
         self.cate_shape = None
         self.cont_shape = None
         self.cate_columns = None
```

### Comparing `omnixai-1.3.0/omnixai/preprocessing/text.py` & `omnixai-1.3.1/omnixai/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/sampler/tabular.py` & `omnixai-1.3.1/omnixai/sampler/tabular.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/data/test_image.py` & `omnixai-1.3.1/omnixai/tests/data/test_image.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/data/test_multi.py` & `omnixai-1.3.1/omnixai/tests/data/test_multi.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/data/test_tabular.py` & `omnixai-1.3.1/omnixai/tests/data/test_tabular.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/data/test_text.py` & `omnixai-1.3.1/omnixai/tests/data/test_text.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/data/test_timeseries.py` & `omnixai-1.3.1/omnixai/tests/data/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/api_server.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/api_server.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/model.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/model.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/request.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/request.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/test.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/test.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/train.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/nlp/train.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/request.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/request.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/test.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/test.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/train.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/tabular/train.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/request.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/request.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/save.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/save.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/test.py` & `omnixai-1.3.1/omnixai/tests/deployment/bentoml/vision/test.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x.py` & `omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_image_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_image_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_text_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/L2X/test_l2x_text_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/ale/test_ale_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/ale/test_ale_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/bias/test_bias_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/bias/test_bias_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_imagenet.py` & `omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_imagenet.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tabular.py` & `omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_tabular.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_timeseries.py` & `omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_timeseries.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/ce/test_ce_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/cem/cem_optimizer_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/cem/cem_optimizer_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/cem/test_cem_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/cem/test_cem_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/data/test_chi2.py` & `omnixai-1.3.1/omnixai/tests/explainers/data/test_chi2.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/data/test_correlation.py` & `omnixai-1.3.1/omnixai/tests/explainers/data/test_correlation.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/data/test_imbalance.py` & `omnixai-1.3.1/omnixai/tests/explainers/data/test_imbalance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/data/test_mutual.py` & `omnixai-1.3.1/omnixai/tests/explainers/data/test_mutual.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/decision_tree/test_tree_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/decision_tree/test_tree_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/example.py` & `omnixai-1.3.1/omnixai/tests/explainers/example.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/explainer_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/explainer_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_explainer.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/feature_explainer.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fft.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_fft.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/gpt/gpt_explainer_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/gpt/gpt_explainer_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_gradcam_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_gradcam_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_layercam_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/gradcam/test_layercam_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/ig/nlp_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/ig/nlp_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py` & `omnixai-1.3.1/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_image.py` & `omnixai-1.3.1/omnixai/tests/explainers/ig/test_ig_image.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_tabular.py` & `omnixai-1.3.1/omnixai/tests/explainers/ig/test_ig_tabular.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ig/vlm_ig_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/ig/vlm_ig_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/knn/test_ce_knn.py` & `omnixai-1.3.1/omnixai/tests/explainers/knn/test_ce_knn.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_image_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_image_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_tabular_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_tabular_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_text_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/lime/test_lime_text_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/linear/test_linear_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/linear/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/mace/test_mace.py` & `omnixai-1.3.1/omnixai/tests/explainers/mace/test_mace.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/mace/test_mace_timeseries.py` & `omnixai-1.3.1/omnixai/tests/explainers/mace/test_mace_timeseries.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/mace/test_ranking.py` & `omnixai-1.3.1/omnixai/tests/explainers/mace/test_ranking.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/mace/test_retrieval.py` & `omnixai-1.3.1/omnixai/tests/explainers/mace/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/mace/test_rl_optimizer.py` & `omnixai-1.3.1/omnixai/tests/explainers/mace/test_rl_optimizer.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/pdp/pdp_image.py` & `omnixai-1.3.1/omnixai/tests/explainers/pdp/pdp_image.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/pdp/test_tabular_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/pdp/test_tabular_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/permutation/test_permutation_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/permutation/test_permutation_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/permutation/test_permutation_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/permutation/test_permutation_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/polyjuice/polyjuice_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/polyjuice/polyjuice_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/polyjuice/polyjuice_qa.py` & `omnixai-1.3.1/omnixai/tests/explainers/polyjuice/polyjuice_qa.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_classification_metrics.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_confusion.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_confusion.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_cumulative.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_lift.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_lift.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_pr.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_pr.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_regression_metric.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_regression_metric.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_residual.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_residual.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_roc.py` & `omnixai-1.3.1/omnixai/tests/explainers/prediction/test_roc.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ranking/test_perm_ranking.py` & `omnixai-1.3.1/omnixai/tests/explainers/ranking/test_perm_ranking.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/ranking/test_validity_ranking.py` & `omnixai-1.3.1/omnixai/tests/explainers/ranking/test_validity_ranking.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/scorecam/scorecam_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/scorecam/scorecam_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/scorecam/test_scorecam_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/scorecam/test_scorecam_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/sensitivity/test_sa_tabular.py` & `omnixai-1.3.1/omnixai/tests/explainers/sensitivity/test_sa_tabular.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/shap_image_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/shap_image_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_merlion.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/shap_merlion.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_text.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/shap_text.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_tabular_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_global.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_tabular_global.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_tabular_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_timeseries.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap/test_shap_timeseries.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_classification.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap_tree/shaptree_classification.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_regression.py` & `omnixai-1.3.1/omnixai/tests/explainers/shap_tree/shaptree_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py` & `omnixai-1.3.1/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py` & `omnixai-1.3.1/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/explainers/tasks.py` & `omnixai-1.3.1/omnixai/tests/explainers/tasks.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/preprocessing/test_encode.py` & `omnixai-1.3.1/omnixai/tests/preprocessing/test_encode.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/preprocessing/test_fill.py` & `omnixai-1.3.1/omnixai/tests/preprocessing/test_fill.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/preprocessing/test_image_transform.py` & `omnixai-1.3.1/omnixai/tests/preprocessing/test_image_transform.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/preprocessing/test_normalize.py` & `omnixai-1.3.1/omnixai/tests/preprocessing/test_normalize.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/preprocessing/test_pipeline.py` & `omnixai-1.3.1/omnixai/tests/preprocessing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/preprocessing/test_tabular_transform.py` & `omnixai-1.3.1/omnixai/tests/preprocessing/test_tabular_transform.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/preprocessing/test_text_transform.py` & `omnixai-1.3.1/omnixai/tests/preprocessing/test_text_transform.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/sampler/test_sampler.py` & `omnixai-1.3.1/omnixai/tests/sampler/test_sampler.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/utils/json/test_counterfactual.py` & `omnixai-1.3.1/omnixai/tests/utils/json/test_counterfactual.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/utils/json/test_feature_importance.py` & `omnixai-1.3.1/omnixai/tests/utils/json/test_feature_importance.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/utils/json/test_prediction.py` & `omnixai-1.3.1/omnixai/tests/utils/json/test_prediction.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/utils/test_explanation_utils.py` & `omnixai-1.3.1/omnixai/tests/utils/test_explanation_utils.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/utils/test_segmentation.py` & `omnixai-1.3.1/omnixai/tests/utils/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_da.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_da.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_image.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_image.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_image_compare.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_image_compare.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_tabular.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular_regression.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_tabular_regression.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_text.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_text.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_text_imdb.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_text_imdb.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/tests/visualization/dashboard_timeseries.py` & `omnixai-1.3.1/omnixai/tests/visualization/dashboard_timeseries.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/utils/misc.py` & `omnixai-1.3.1/omnixai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/utils/segmentation.py` & `omnixai-1.3.1/omnixai/utils/segmentation.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/assets/Acumin-BdPro.otf` & `omnixai-1.3.1/omnixai/visualization/assets/Acumin-BdPro.otf`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/assets/base.css` & `omnixai-1.3.1/omnixai/visualization/assets/base.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/assets/logo_small.png` & `omnixai-1.3.1/omnixai/visualization/assets/logo_small.png`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/assets/modal.css` & `omnixai-1.3.1/omnixai/visualization/assets/modal.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/assets/styles.css` & `omnixai-1.3.1/omnixai/visualization/assets/styles.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/assets/xai.css` & `omnixai-1.3.1/omnixai/visualization/assets/xai.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/callbacks/data_exp.py` & `omnixai-1.3.1/omnixai/visualization/callbacks/data_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/callbacks/global_exp.py` & `omnixai-1.3.1/omnixai/visualization/callbacks/global_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/callbacks/local_exp.py` & `omnixai-1.3.1/omnixai/visualization/callbacks/local_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/callbacks/prediction_exp.py` & `omnixai-1.3.1/omnixai/visualization/callbacks/prediction_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/callbacks/whatif_exp.py` & `omnixai-1.3.1/omnixai/visualization/callbacks/whatif_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/dashboard.py` & `omnixai-1.3.1/omnixai/visualization/dashboard.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/layout.py` & `omnixai-1.3.1/omnixai/visualization/layout.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/pages/data_exp.py` & `omnixai-1.3.1/omnixai/visualization/pages/data_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/pages/global_exp.py` & `omnixai-1.3.1/omnixai/visualization/pages/global_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/pages/local_exp.py` & `omnixai-1.3.1/omnixai/visualization/pages/local_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/pages/prediction_exp.py` & `omnixai-1.3.1/omnixai/visualization/pages/prediction_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/pages/utils.py` & `omnixai-1.3.1/omnixai/visualization/pages/utils.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/pages/whatif_exp.py` & `omnixai-1.3.1/omnixai/visualization/pages/whatif_exp.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/plot.py` & `omnixai-1.3.1/omnixai/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai/visualization/state.py` & `omnixai-1.3.1/omnixai/visualization/state.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai.egg-info/PKG-INFO` & `omnixai-1.3.1/omnixai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnixai
-Version: 1.3.0
+Version: 1.3.1
 Summary: OmniXAI: An Explainable AI Toolbox
 Home-page: https://github.com/salesforce/omnixai
 Author: Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
 License: 3-Clause BSD
 Keywords: XAI Explainable AI Explanation
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
@@ -43,15 +43,15 @@
 ## Table of Contents
 1. [Introduction](#introduction)
 2. [Installation](#installation)
 3. [Getting Started](#getting-started)
 4. [Documentation](https://opensource.salesforce.com/OmniXAI/latest/index.html)
 5. [Tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html)
 6. [Deployment](#deployment)
-7. [Dashboard Demo](https://sfr-omnixai-demo.herokuapp.com/)
+7. [Dashboard Demo](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/)
 8. [How to Contribute](https://opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute)
 9. [Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai)
 
 ## What's New
 
 The latest version includes an experimental GPT explainer. This explainer leverages the outcomes 
 produced by SHAP and MACE to formulate the input prompt for ChatGPT. Subsequently, ChatGPT 
@@ -133,26 +133,27 @@
 - **Install all the dependencies**: Calling ``pip install omnixai[all]``, or ``pip install .[all]`` from the
   root directory of the repo.
 
 ## Getting Started
 
 For example code and an introduction to the library, see the Jupyter notebooks in
 [tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html), and the guided walkthrough
-[here](https://opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be found [here](https://sfr-omnixai-demo.herokuapp.com/).
+[here](https://opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be found [here](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/).
 
 Some examples:
 1. [Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_classification.ipynb)
 2. [Tabular regression](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb)
 3. [Image classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision.ipynb)
 4. [Text classification](https://github.com/salesforce/OmniXAI/blob/main/tutorials/nlp_imdb.ipynb)
 5. [Time-series anomaly detection](https://github.com/salesforce/OmniXAI/blob/main/tutorials/timeseries.ipynb)
 6. [Vision-language tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/gradcam_vlm.ipynb)
 7. [Ranking tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/ranking.ipynb)
 8. [Feature visualization](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/feature_visualization_torch.ipynb)
 9. [Check feature maps](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/feature_map_torch.ipynb)
+10. [GPT explainer for tabular](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/gpt.ipynb)
 
 To get started, we recommend the linked tutorials in [tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html).
 In general, we recommend using `TabularExplainer`, `VisionExplainer`,
 `NLPExplainer` and `TimeseriesExplainer` for tabular, vision, NLP and time-series tasks, respectively, and using
 `DataAnalyzer` and `PredictionAnalyzer` for feature analysis and prediction result analysis.
 These classes act as the factories of the individual explainers supported in OmniXAI, providing a simpler
 interface to generate multiple explanations. To generate explanations, you only need to specify
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: omnixai Version: 1.3.0 Summary: OmniXAI: An
+Metadata-Version: 2.1 Name: omnixai Version: 1.3.1 Summary: OmniXAI: An
 Explainable AI Toolbox Home-page: https://github.com/salesforce/omnixai Author:
 Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
 License: 3-Clause BSD Keywords: XAI Explainable AI Explanation Requires-Python:
 >=3.7,<4 Description-Content-Type: text/markdown Provides-Extra: plot Provides-
 Extra: vision Provides-Extra: nlp Provides-Extra: bentoml Provides-Extra: all
 License-File: LICENSE
 
@@ -10,40 +10,40 @@
 # OmniXAI: A Library for Explainable AI
     [https://img.shields.io/badge/Python-3.7,_3.8,_3.9,_3.10-blue] [PyPI]
                        [Documentation] [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://opensource.salesforce.com/OmniXAI/latest/index.html) 5. [Tutorials]
 (https://opensource.salesforce.com/OmniXAI/latest/tutorials.html) 6.
-[Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-
-demo.herokuapp.com/) 8. [How to Contribute](https://opensource.salesforce.com/
-OmniXAI/latest/omnixai.html#how-to-contribute) 9. [Technical Report and Citing
-OmniXAI](#technical-report-and-citing-omnixai) ## What's New The latest version
-includes an experimental GPT explainer. This explainer leverages the outcomes
-produced by SHAP and MACE to formulate the input prompt for ChatGPT.
-Subsequently, ChatGPT analyzes these results and generates the corresponding
-explanations that provide developers with a clearer understanding of the
-rationale behind the model's predictions. ## Introduction OmniXAI (short for
-Omni eXplainable AI) is a Python machine-learning library for explainable AI
-(XAI), offering omni-way explainable AI and interpretable machine learning
-capabilities to address many pain points in explaining decisions made by
-machine learning models in practice. OmniXAI aims to be a one-stop
-comprehensive library that makes explainable AI easy for data scientists, ML
-researchers and practitioners who need explanation for various types of data,
-models and explanation methods at different stages of ML process: ![alt text]
-(https://github.com/salesforce/OmniXAI/raw/main/docs/_static/ml_pipeline.png)
-OmniXAI includes a rich family of explanation methods integrated in a unified
-interface, which supports multiple data types (tabular data, images, texts,
-time-series), multiple types of ML models (traditional ML in Scikit-learn and
-deep learning models in PyTorch/TensorFlow), and a range of diverse
-explaination methods including "model-specific" and "model-agnostic" methods
-(such as feature-attribution explanation, counterfactual explanation, gradient-
-based explanation, feature visualization, etc). For practitioners, OmniXAI
-provides an easy-to-use unified interface to generate the explanations for
-their applications by only writing a few lines of codes, and also a GUI
+[Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-demo-
+cc9e4edb6447.herokuapp.com/) 8. [How to Contribute](https://
+opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute) 9.
+[Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai) ##
+What's New The latest version includes an experimental GPT explainer. This
+explainer leverages the outcomes produced by SHAP and MACE to formulate the
+input prompt for ChatGPT. Subsequently, ChatGPT analyzes these results and
+generates the corresponding explanations that provide developers with a clearer
+understanding of the rationale behind the model's predictions. ## Introduction
+OmniXAI (short for Omni eXplainable AI) is a Python machine-learning library
+for explainable AI (XAI), offering omni-way explainable AI and interpretable
+machine learning capabilities to address many pain points in explaining
+decisions made by machine learning models in practice. OmniXAI aims to be a
+one-stop comprehensive library that makes explainable AI easy for data
+scientists, ML researchers and practitioners who need explanation for various
+types of data, models and explanation methods at different stages of ML
+process: ![alt text](https://github.com/salesforce/OmniXAI/raw/main/docs/
+_static/ml_pipeline.png) OmniXAI includes a rich family of explanation methods
+integrated in a unified interface, which supports multiple data types (tabular
+data, images, texts, time-series), multiple types of ML models (traditional ML
+in Scikit-learn and deep learning models in PyTorch/TensorFlow), and a range of
+diverse explaination methods including "model-specific" and "model-agnostic"
+methods (such as feature-attribution explanation, counterfactual explanation,
+gradient-based explanation, feature visualization, etc). For practitioners,
+OmniXAI provides an easy-to-use unified interface to generate the explanations
+for their applications by only writing a few lines of codes, and also a GUI
 dashboard for visualization for obtaining more insights about decisions. The
 following table shows the supported explanation methods and features in our
 library. We will continue improving this library to make it more comprehensive
 in the future. | Method | Model Type | Explanation Type | EDA | Tabular | Image
 | Text | Timeseries | :-------------------------:|:-------------:|:------------
 ----:|:---:|:-------:|:-----:| :---: | :---: | Feature analysis | NA | Global |
 â | | | | | | Feature selection | NA | Global | â | | | | | | Prediction
@@ -85,80 +85,81 @@
 ``pip install omnixai[nlp]``, or ``pip install .[nlp]`` from the root directory
 of the repo. - **Install all the dependencies**: Calling ``pip install omnixai
 [all]``, or ``pip install .[all]`` from the root directory of the repo. ##
 Getting Started For example code and an introduction to the library, see the
 Jupyter notebooks in [tutorials](https://opensource.salesforce.com/OmniXAI/
 latest/tutorials.html), and the guided walkthrough [here](https://
 opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be
-found [here](https://sfr-omnixai-demo.herokuapp.com/). Some examples: 1.
-[Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/tabular_classification.ipynb) 2. [Tabular regression](https://
-github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb) 3.
-[Image classification](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/vision.ipynb) 4. [Text classification](https://github.com/salesforce/
-OmniXAI/blob/main/tutorials/nlp_imdb.ipynb) 5. [Time-series anomaly detection]
-(https://github.com/salesforce/OmniXAI/blob/main/tutorials/timeseries.ipynb) 6.
-[Vision-language tasks](https://github.com/salesforce/OmniXAI/blob/main/
-tutorials/vision/gradcam_vlm.ipynb) 7. [Ranking tasks](https://github.com/
-salesforce/OmniXAI/blob/main/tutorials/tabular/ranking.ipynb) 8. [Feature
-visualization](https://github.com/salesforce/OmniXAI/blob/main/tutorials/
-vision/feature_visualization_torch.ipynb) 9. [Check feature maps](https://
-github.com/salesforce/OmniXAI/blob/main/tutorials/vision/
-feature_map_torch.ipynb) To get started, we recommend the linked tutorials in
-[tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html).
-In general, we recommend using `TabularExplainer`, `VisionExplainer`,
-`NLPExplainer` and `TimeseriesExplainer` for tabular, vision, NLP and time-
-series tasks, respectively, and using `DataAnalyzer` and `PredictionAnalyzer`
-for feature analysis and prediction result analysis. These classes act as the
-factories of the individual explainers supported in OmniXAI, providing a
-simpler interface to generate multiple explanations. To generate explanations,
-you only need to specify - **The ML model to explain**: e.g., a scikit-learn
-model, a tensorflow model, a pytorch model or a black-box prediction function.
-- **The pre-processing function**: i.e., converting raw input features into the
-model inputs. - **The post-processing function (optional)**: e.g., converting
-the model outputs into class probabilities. - **The explainers to apply**:
-e.g., SHAP, MACE, Grad-CAM. Besides using these classes, you can also create a
-single explainer defined in the `omnixai.explainers` package, e.g.,
-`ShapTabular`, `GradCAM`, `IntegratedGradient` or `FeatureVisualizer`. Let's
-take the income prediction task as an example. The [dataset](https://
-archive.ics.uci.edu/ml/datasets/adult) used in this example is for income
-prediction. We recommend using data class `Tabular` to represent a tabular
-dataset. To create a `Tabular` instance given a pandas dataframe, you need to
-specify the dataframe, the categorical feature names (if exists) and the
-target/label column name (if exists). ```python from omnixai.data.tabular
-import Tabular # Load the dataset feature_names = [ "Age", "Workclass",
-"fnlwgt", "Education", "Education-Num", "Marital Status", "Occupation",
-"Relationship", "Race", "Sex", "Capital Gain", "Capital Loss", "Hours per
-week", "Country", "label" ] df = pd.DataFrame( np.genfromtxt('adult.data',
-delimiter=', ', dtype=str), columns=feature_names ) tabular_data = Tabular( df,
-categorical_columns=[feature_names[i] for i in [1, 3, 5, 6, 7, 8, 9, 13]],
-target_column='label' ) ``` The package `omnixai.preprocessing` provides
-several useful preprocessing functions for a `Tabular` instance.
-`TabularTransform` is a special transform designed for processing tabular data.
-By default, it converts categorical features into one-hot encoding, and keeps
-continuous-valued features. The method ``transform`` of `TabularTransform`
-transforms a `Tabular` instance to a numpy array. If the `Tabular` instance has
-a target/label column, the last column of the numpy array will be the target/
-label. You can apply any customized preprocessing functions instead of using
-`TabularTransform`. After data preprocessing, let's train a XGBoost classifier
-for this task. ```python from omnixai.preprocessing.tabular import
-TabularTransform # Data preprocessing transformer = TabularTransform().fit
-(tabular_data) class_names = transformer.class_names x = transformer.transform
-(tabular_data) # Split into training and test datasets train, test,
-train_labels, test_labels = \ sklearn.model_selection.train_test_split(x[:, :-
-1], x[:, -1], train_size=0.80) # Train an XGBoost model (the last column of `x`
-is the label column after transformation) model = xgboost.XGBClassifier
-(n_estimators=300, max_depth=5) model.fit(train, train_labels) # Convert the
-transformed data back to Tabular instances train_data = transformer.invert
-(train) test_data = transformer.invert(test) ``` To initialize
-`TabularExplainer`, the following parameters need to be set: - ``explainers``:
-The names of the explainers to apply, e.g., ["lime", "shap", "mace", "pdp"]. -
-``data``: The data used to initialize explainers. ``data`` is the training
-dataset for training the machine learning model. If the training dataset is too
-large, ``data`` can be a subset of it by applying
+found [here](https://sfr-omnixai-demo-cc9e4edb6447.herokuapp.com/). Some
+examples: 1. [Tabular classification](https://github.com/salesforce/OmniXAI/
+blob/main/tutorials/tabular_classification.ipynb) 2. [Tabular regression]
+(https://github.com/salesforce/OmniXAI/blob/main/tutorials/
+tabular_regression.ipynb) 3. [Image classification](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/vision.ipynb) 4. [Text classification]
+(https://github.com/salesforce/OmniXAI/blob/main/tutorials/nlp_imdb.ipynb) 5.
+[Time-series anomaly detection](https://github.com/salesforce/OmniXAI/blob/
+main/tutorials/timeseries.ipynb) 6. [Vision-language tasks](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/vision/gradcam_vlm.ipynb) 7. [Ranking
+tasks](https://github.com/salesforce/OmniXAI/blob/main/tutorials/tabular/
+ranking.ipynb) 8. [Feature visualization](https://github.com/salesforce/
+OmniXAI/blob/main/tutorials/vision/feature_visualization_torch.ipynb) 9. [Check
+feature maps](https://github.com/salesforce/OmniXAI/blob/main/tutorials/vision/
+feature_map_torch.ipynb) 10. [GPT explainer for tabular](https://github.com/
+salesforce/OmniXAI/blob/main/tutorials/tabular/gpt.ipynb) To get started, we
+recommend the linked tutorials in [tutorials](https://
+opensource.salesforce.com/OmniXAI/latest/tutorials.html). In general, we
+recommend using `TabularExplainer`, `VisionExplainer`, `NLPExplainer` and
+`TimeseriesExplainer` for tabular, vision, NLP and time-series tasks,
+respectively, and using `DataAnalyzer` and `PredictionAnalyzer` for feature
+analysis and prediction result analysis. These classes act as the factories of
+the individual explainers supported in OmniXAI, providing a simpler interface
+to generate multiple explanations. To generate explanations, you only need to
+specify - **The ML model to explain**: e.g., a scikit-learn model, a tensorflow
+model, a pytorch model or a black-box prediction function. - **The pre-
+processing function**: i.e., converting raw input features into the model
+inputs. - **The post-processing function (optional)**: e.g., converting the
+model outputs into class probabilities. - **The explainers to apply**: e.g.,
+SHAP, MACE, Grad-CAM. Besides using these classes, you can also create a single
+explainer defined in the `omnixai.explainers` package, e.g., `ShapTabular`,
+`GradCAM`, `IntegratedGradient` or `FeatureVisualizer`. Let's take the income
+prediction task as an example. The [dataset](https://archive.ics.uci.edu/ml/
+datasets/adult) used in this example is for income prediction. We recommend
+using data class `Tabular` to represent a tabular dataset. To create a
+`Tabular` instance given a pandas dataframe, you need to specify the dataframe,
+the categorical feature names (if exists) and the target/label column name (if
+exists). ```python from omnixai.data.tabular import Tabular # Load the dataset
+feature_names = [ "Age", "Workclass", "fnlwgt", "Education", "Education-Num",
+"Marital Status", "Occupation", "Relationship", "Race", "Sex", "Capital Gain",
+"Capital Loss", "Hours per week", "Country", "label" ] df = pd.DataFrame
+( np.genfromtxt('adult.data', delimiter=', ', dtype=str), columns=feature_names
+) tabular_data = Tabular( df, categorical_columns=[feature_names[i] for i in
+[1, 3, 5, 6, 7, 8, 9, 13]], target_column='label' ) ``` The package
+`omnixai.preprocessing` provides several useful preprocessing functions for a
+`Tabular` instance. `TabularTransform` is a special transform designed for
+processing tabular data. By default, it converts categorical features into one-
+hot encoding, and keeps continuous-valued features. The method ``transform`` of
+`TabularTransform` transforms a `Tabular` instance to a numpy array. If the
+`Tabular` instance has a target/label column, the last column of the numpy
+array will be the target/label. You can apply any customized preprocessing
+functions instead of using `TabularTransform`. After data preprocessing, let's
+train a XGBoost classifier for this task. ```python from
+omnixai.preprocessing.tabular import TabularTransform # Data preprocessing
+transformer = TabularTransform().fit(tabular_data) class_names =
+transformer.class_names x = transformer.transform(tabular_data) # Split into
+training and test datasets train, test, train_labels, test_labels = \
+sklearn.model_selection.train_test_split(x[:, :-1], x[:, -1], train_size=0.80)
+# Train an XGBoost model (the last column of `x` is the label column after
+transformation) model = xgboost.XGBClassifier(n_estimators=300, max_depth=5)
+model.fit(train, train_labels) # Convert the transformed data back to Tabular
+instances train_data = transformer.invert(train) test_data = transformer.invert
+(test) ``` To initialize `TabularExplainer`, the following parameters need to
+be set: - ``explainers``: The names of the explainers to apply, e.g., ["lime",
+"shap", "mace", "pdp"]. - ``data``: The data used to initialize explainers.
+``data`` is the training dataset for training the machine learning model. If
+the training dataset is too large, ``data`` can be a subset of it by applying
 `omnixai.sampler.tabular.Sampler.subsample`. - ``model``: The ML model to
 explain, e.g., a scikit-learn model, a tensorflow model or a pytorch model. -
 ``preprocess``: The preprocessing function converting the raw inputs (A
 `Tabular` instance) into the inputs of ``model``. - ``postprocess`` (optional):
 The postprocessing function transforming the outputs of ``model`` to a user-
 specific form, e.g., the predicted probability for each class. The output of
 `postprocess` should be a numpy array. - ``mode``: The task type, e.g.,
```

### Comparing `omnixai-1.3.0/omnixai.egg-info/SOURCES.txt` & `omnixai-1.3.1/omnixai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/omnixai.egg-info/requires.txt` & `omnixai-1.3.1/omnixai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `omnixai-1.3.0/setup.py` & `omnixai-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "nlp": ["nltk>=3.4.5", "polyjuice_nlp"],
     "bentoml": ["bentoml>=1.0.0"],
 }
 extras_require["all"] = sum(extras_require.values(), [])
 
 setup(
     name="omnixai",
-    version="1.3.0",
+    version="1.3.1",
     author="Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi",
     description="OmniXAI: An Explainable AI Toolbox",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="XAI Explainable AI Explanation",
     url="https://github.com/salesforce/omnixai",
     license="3-Clause BSD",
```

