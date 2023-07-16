# Comparing `tmp/clustutils4r-0.0.6.tar.gz` & `tmp/clustutils4r-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-0.0.6.tar", last modified: Fri Jul 14 02:13:39 2023, max compression
+gzip compressed data, was "clustutils4r-0.0.7.tar", last modified: Sun Jul 16 08:26:00 2023, max compression
```

## Comparing `clustutils4r-0.0.6.tar` & `clustutils4r-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.6/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4905 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4273 2023-07-14 02:12:15.000000 clustutils4r-0.0.6/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-14 02:13:08.000000 clustutils4r-0.0.6/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-14 02:13:12.000000 clustutils4r-0.0.6/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.6/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    26853 2023-07-14 02:01:24.000000 clustutils4r-0.0.6/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/src/clustutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4905 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.7/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5299 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4667 2023-07-16 08:23:55.000000 clustutils4r-0.0.7/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-16 08:25:16.000000 clustutils4r-0.0.7/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-16 08:25:24.000000 clustutils4r-0.0.7/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.7/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    28396 2023-07-16 08:18:23.000000 clustutils4r-0.0.7/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:26:00.479929 clustutils4r-0.0.7/src/clustutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5299 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-16 08:26:00.000000 clustutils4r-0.0.7/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-0.0.6/LICENSE` & `clustutils4r-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.6/PKG-INFO` & `clustutils4r-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: clustutils4r
-Version: 0.0.6
-Summary: Wrapper around some basic sklearn utilities for clustering.
-Home-page: https://github.com/rutujagurav/clustutils4r
-Author: Rutuja Gurav
-Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
-Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
-Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
 ## Installation
 `pip install clustutils4r`
 
@@ -29,15 +13,15 @@
 
 `gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
 
 `num_clusters`: Range of no. of clusters to grid search over.
 
 `num_runs`: No. of runs per no. of cluster (defaults = 10).
 
-`make_metrics_plots`: Plot various clustering evaluation metrics. Depending on whether `gt_labels` are provided, you will get one or more plots - one for non-ground truth-based metrics and another for ground truth-based metrics. (default = `True`).
+`make_metrics_plots`: Plot various clustering evaluation metrics. Depending on whether `gt_labels` are provided, you will get one or two sets of plots - one for non-ground truth-based metrics and another for ground truth-based metrics. (default = `True`).
 
 `annotate_topN_best_scores`: Whether to annotate top N score in metrics plots (defined by `annotN`) (defaults = `True`).
 
 `annotN`: No. of top scores to annotated in metrics plots (defaults = 3).
 
 `make_silhoutte_plots`: Whether to make silhouette plots for each `num_clusters` value (default = `False`).
 
@@ -47,41 +31,48 @@
 
 `save`: set True if you want to save all results in RESULTS_DIR; defaults to False
 
 `show`: display all results; useful in notebooks; defaults to False
 
 ## Example Usage
 ```python
-import os
-from sklearn import datasets
-
-# Load the iris dataset
-data = datasets.load_digits()
+import matplotlib.pyplot as plt
+%matplotlib inline
 
-# Split the data into features and labels
-X = data.data
-y = data.target
-
-# Define clustering model
+import os, collections
+from sklearn import datasets
 from sklearn.cluster import KMeans
-kmeans_model = KMeans()
+from sklearn.mixture import GaussianMixture
 
-# Run the evaluation
 from clustutils4r.eval_clustering import eval_clustering
-range_clusters = list(range(3,15+1))
-labelled_datapoints, nongt_metrics, gt_metrics \
-    = eval_clustering(X=X, gt_labels=y,
-                        model=KMeans(),
-                        num_clusters=range_clusters, num_runs=10,
-                        annotate_topN_best_scores=True, annotN=3,
-                        make_metrics_plots=True,
-                        make_silhoutte_plots=True, embed_data_in_2d=True,
-                        show=True, 
-                        save=True, RESULTS_DIR=os.getcwd()+'/results',
-                    )
+
+## Load the dataset
+X, y = datasets.make_blobs(n_samples=5*100, 
+                           centers=5, 
+                           n_features=2, 
+                           random_state=0)
+
+## Setup model
+model = KMeans()
+model_params = {'init':'k-means++', 'n_init':1}
+n_clusters_param_name='n_clusters'
+
+## Run the evaluation
+range_clusters = list(range(3,10+1))
+labelled_datapoints, \
+   nongt_metrics, \
+      gt_metrics = eval_clustering(X=X, gt_labels=y,
+                                    model=model, model_params=model_params, n_clusters_param_name=n_clusters_param_name,
+                                    num_clusters=range_clusters, num_runs=10,
+                                    annotate_topN_best_scores=True, annotN=3,
+                                    make_metrics_plots=True,
+                                    make_silhoutte_plots=False,
+                                    show=True, 
+                                    save=True, RESULTS_DIR=os.getcwd()+'/results',
+                                )
 
 ```
 
 ![ch](tests/example_clustering/results/nongt_metrics_plots/cal_har.png)
 ![sil](tests/example_clustering/results/nongt_metrics_plots/dav_bou.png)
 ![sil](tests/example_clustering/results/nongt_metrics_plots/hopkn.png)
 ![sil](tests/example_clustering/results/nongt_metrics_plots/sil.png)
@@ -97,10 +88,10 @@
 ![ri](tests/example_clustering/results/gt_metrics_plots/rand_index.png)
 
 <!-- ![fmi](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/fmi.png)
 ![mi](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/mutual_info.png)
 ![hcv](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/hcv.png)
 ![ri](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/rand_index.png) -->
 
-![silplt](tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png)
+![silplt](tests/example_clustering/results/silhouette_plots/5_silhouette_plot.png)
 
-<!-- ![silplt](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
+<!-- ![silplt](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
```

### Comparing `clustutils4r-0.0.6/pyproject.toml` & `clustutils4r-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-0.0.6/setup.py` & `clustutils4r-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clustutils4r", # Replace with your own username
-    version="0.0.6",
+    version="0.0.7",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn utilities for clustering.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clustutils4r",
     project_urls={
```

### Comparing `clustutils4r-0.0.6/src/clustutils4r/eval_clustering.py` & `clustutils4r-0.0.7/src/clustutils4r/eval_clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,22 +47,29 @@
     homogeneity, completeness, v_measure = homogeneity_completeness_v_measure(gt_labels, cluster_labels)
 
     fmi = fowlkes_mallows_score(gt_labels, cluster_labels).round(3)
 
     return dict(zip(metric_names, [ri, ari, mi, ami, nmi, homogeneity, completeness, v_measure, fmi]))
 
 def calc_nongt_metrics(X=None, cluster_labels=None):
-    metric_names = ['Silhouette', 'Calinski-Harabasz', 'Davies-Bouldin', 'Hopkins']
+    metric_names = ['Silhouette', 
+                                'Calinski-Harabasz', 'Davies-Bouldin', 
+                                # 'Hopkins'
+                            ]
     silhouette_avg = silhouette_score(X, cluster_labels).round(3)
     calinski_harabasz_score_avg = calinski_harabasz_score(X, cluster_labels).round(3)
     davies_bouldin_score_avg = davies_bouldin_score(X, cluster_labels).round(3)
-    hopkins_score = hopkins_statistic(X).round(3)
+    # hopkins_score = hopkins_statistic(X).round(3)
     
     # return silhouette_avg,calinski_harabasz_score_avg, davies_bouldin_score_avg, hopkins_score
-    return dict(zip(metric_names, [silhouette_avg, calinski_harabasz_score_avg, davies_bouldin_score_avg, hopkins_score]))
+    return dict(zip(metric_names, [silhouette_avg, 
+                                                    calinski_harabasz_score_avg, 
+                                                    davies_bouldin_score_avg, 
+                                                    # hopkins_score
+                                                ]))
 
 def plot_gt_metrics(gt_metrics=None, num_clusters=None,
                     annotate_topN_best_scores=True, annotN=3,
                     show=False, save=False, save_dir=None):
 
     if isinstance(gt_metrics, dict):
         ri_scores_mean = gt_metrics['mean']['RI'].values
@@ -119,15 +126,15 @@
 
     ## ARI
     ax.plot(num_clusters, ari_scores_mean, label='ARI')
     ax.fill_between(num_clusters,
                         ari_scores_mean - ari_scores_std,
                         ari_scores_mean + ari_scores_std,
                         alpha=0.2)
-    ax.set_title("Rand Index")
+    ax.set_title("Rand Index\n(RI: [0, 1], ARI: [-1, 1]; closer to 1 = better)")
     ax.set_xlabel("No. of Clusters")
     # axs[0,0].set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(ari_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = ari_scores_mean[i]
             ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
@@ -160,14 +167,15 @@
     ## NMI
     ax.plot(num_clusters, nmi_scores_mean, label='NMI')
     ax.fill_between(num_clusters,
                         nmi_scores_mean - nmi_scores_std,
                         nmi_scores_mean + nmi_scores_std,
                         alpha=0.2)
     
+    ax.set_title("Mutual Information\n([0,1]; closer to 1 = better)")
     ax.set_xlabel("No. of Clusters")
     # axs[0,1].set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(nmi_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = nmi_scores_mean[i]
             ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
@@ -198,14 +206,15 @@
     ## V-Measure
     ax.plot(num_clusters, v_measure_scores_mean, label='V-Measure')
     ax.fill_between(num_clusters,
                         v_measure_scores_mean - v_measure_scores_std,
                         v_measure_scores_mean + v_measure_scores_std,
                         alpha=0.2)
     
+    ax.set_title("Conditional Entropy Analysis\n([0,1]; closer to 1 = better)")
     ax.set_xlabel("No. of Clusters")
     # ax.set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(v_measure_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = v_measure_scores_mean[i]
             ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
@@ -221,15 +230,15 @@
     fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## FMI
     ax.plot(num_clusters, fmi_scores_mean, label='FMI')
     ax.fill_between(num_clusters,
                         fmi_scores_mean - fmi_scores_std,
                         fmi_scores_mean + fmi_scores_std,
                         alpha=0.2)
-    ax.set_title("Fowlkes-Mallows Index")
+    ax.set_title("Fowlkes-Mallows Index\n([0,1]; closer to 1 = better)")
     ax.set_xlabel("No. of Clusters")
     # ax.set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(fmi_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = fmi_scores_mean[i]
             ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
@@ -246,52 +255,58 @@
     # if save:
     #     print("Saving ground truth-based clustering metrics plot at {}".format(os.path.join(save_dir, 'feats_clustering_metrics.png')))
     #     plt.savefig(os.path.join(save_dir, 'feats_clustering_gt_metrics.png'), dpi=300)
     # if show:
     #     plt.show()
     # plt.close()    
 
-
 def plot_nongt_metrics(nongt_metrics=None, 
                        num_clusters=None, annotate_topN_best_scores=False, annotN=3,
                        show=False, save=False, save_dir=None):
     if isinstance(nongt_metrics, dict):
         sil_scores_mean = nongt_metrics['mean']['Silhouette'].values
         ch_scores_mean = nongt_metrics['mean']['Calinski-Harabasz'].values
         db_scores_mean = nongt_metrics['mean']['Davies-Bouldin'].values
-        hpkn_scores_mean = nongt_metrics['mean']['Hopkins'].values
+        # hpkn_scores_mean = nongt_metrics['mean']['Hopkins'].values
 
         sil_scores_std = nongt_metrics['std']['Silhouette'].values
         ch_scores_std = nongt_metrics['std']['Calinski-Harabasz'].values
         db_scores_std = nongt_metrics['std']['Davies-Bouldin'].values
-        hpkn_scores_std = nongt_metrics['std']['Hopkins'].values
+        # hpkn_scores_std = nongt_metrics['std']['Hopkins'].values
 
     elif isinstance(nongt_metrics, pd.DataFrame):
         sil_scores_mean = nongt_metrics['Silhouette'].values
         ch_scores_mean = nongt_metrics['Calinski-Harabasz'].values
         db_scores_mean = nongt_metrics['Davies-Bouldin'].values
-        hpkn_scores_mean = nongt_metrics['Hopkins'].values
+        # hpkn_scores_mean = nongt_metrics['Hopkins'].values
 
         sil_scores_std = [0.0]*len(sil_scores_mean)
         ch_scores_std = [0.0]*len(ch_scores_mean)
         db_scores_std = [0.0]*len(db_scores_mean)
-        hpkn_scores_std = [0.0]*len(hpkn_scores_mean)
+        # hpkn_scores_std = [0.0]*len(hpkn_scores_mean)
     
     # fig, axs = plt.subplots(2,2, figsize=(10,10))
 
     fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Silhouette
     ax.plot(num_clusters, sil_scores_mean)
     ax.fill_between(num_clusters, 
                         sil_scores_mean - sil_scores_std, 
                         sil_scores_mean + sil_scores_std, 
-                        color='b', alpha=0.2)
+                        alpha=0.2)
     ax.set_title("Avg. Silhoutte Score\n(-1=incorrect, 0=overlap, 1=dense)")
     ax.set_xlabel("No. of Clusters")
-    ax.set_ylim(-1.1,1.1)
+    # ax.set_ylim(-1.1,1.1)
+
+    if annotate_topN_best_scores:
+        # # top_k_indices = sorted(range(len(ch_scores)), key=lambda i: ch_scores[i], reverse=True)[:k]
+        top_k_indices = np.array(sil_scores_mean).argsort()[-annotN:][::-1]
+        for i in top_k_indices:
+            value = sil_scores_mean[i]
+            ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
 
     plt.tight_layout()    
     if save:
         plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/sil.png'), dpi=300)
     if show:
         plt.show()
     plt.close()
@@ -299,15 +314,15 @@
     
     fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Calinski-Harabasz
     ax.plot(num_clusters, ch_scores_mean)
     ax.fill_between(num_clusters, 
                         ch_scores_mean - ch_scores_std, 
                         ch_scores_mean + ch_scores_std, 
-                        color='b', alpha=0.2)
+                        alpha=0.2)
     ax.set_title("Calinski Harabasz Score\n(higher=dense,well-separated)")
     ax.set_xlabel("No. of Clusters")
     
     if annotate_topN_best_scores:
         # # top_k_indices = sorted(range(len(ch_scores)), key=lambda i: ch_scores[i], reverse=True)[:k]
         top_k_indices = np.array(ch_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
@@ -324,15 +339,15 @@
 
     fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Davies-Bouldin
     ax.plot(num_clusters, db_scores_mean)
     ax.fill_between(num_clusters, 
                         db_scores_mean - db_scores_std, 
                         db_scores_mean + db_scores_std, 
-                        color='b', alpha=0.2)
+                        alpha=0.2)
     ax.set_title("Davies Bouldin Score\n(lower=better)")
     ax.set_xlabel("No. of Clusters") 
     
     if annotate_topN_best_scores:
         # # top_k_indices = sorted(range(len(db_scores)), key=lambda i: db_scores[i], reverse=False)[:k]
         top_k_indices = np.array(db_scores_mean).argsort()[:annotN]
         for i in top_k_indices:
@@ -342,70 +357,73 @@
     plt.tight_layout()    
     if save:
         plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/dav_bou.png'), dpi=300)
     if show:
         plt.show()
     plt.close()
     
-    fig, ax = plt.subplots(1, 1, figsize=(5,5))
-    ## Hopkins
-    ax.plot(num_clusters, hpkn_scores_mean)
-    ax.fill_between(num_clusters, 
-                        hpkn_scores_mean - hpkn_scores_std, 
-                        hpkn_scores_mean + hpkn_scores_std, 
-                        color='b', alpha=0.2)
-    ax.set_title("Hopkins Statistic\n(1=clustered, 0.5=random, 0=uniforrm)")
-    ax.set_xlabel("No. of Clusters")
-    ax.set_ylim(-0.1,1.1) 
+    # fig, ax = plt.subplots(1, 1, figsize=(5,5))
+    # ## Hopkins
+    # ax.plot(num_clusters, hpkn_scores_mean)
+    # ax.fill_between(num_clusters, 
+    #                     hpkn_scores_mean - hpkn_scores_std, 
+    #                     hpkn_scores_mean + hpkn_scores_std, 
+    #                     alpha=0.2)
+    # ax.set_title("Hopkins Statistic\n(1=clustered, 0.5=random, 0=uniforrm)")
+    # ax.set_xlabel("No. of Clusters")
+    # ax.set_ylim(-0.1,1.1) 
 
-    plt.tight_layout()    
-    if save:
-        plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/hopkn.png'), dpi=300)
-    if show:
-        plt.show()
-    plt.close()
+    # plt.tight_layout()    
+    # if save:
+    #     plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/hopkn.png'), dpi=300)
+    # if show:
+    #     plt.show()
+    # plt.close()
 
     # plt.tight_layout()    
     # if save:
     #     print("Saving non-ground truth-based clustering metrics plot at {}".format(os.path.join(save_dir, 'feats_clustering_metrics.png')))
     #     plt.savefig(os.path.join(save_dir, 'feats_clustering_nongt_metrics.png'), dpi=300)
     # if show:
     #     plt.show()
     # plt.close()
 
 def cluster_feats(X=None, gt_labels=[],
                 #   algorithm='k-Means',
-                  model=None,
+                  model=None, model_params={}, n_clusters_param_name='n_clusters',
                   num_clusters = [2,3,5,10], num_runs=10, 
                   make_metrics_plots=True, annotate_topN_best_scores=False, annotN=3,
                   make_silhoutte_plots=True, embed_data_in_2d = False,
                   show=False, save=False, save_dir=None):
     
     if len(gt_labels)!=0:
         print("Ground truth labels provided. Computing ground truth-based clustering metrics along with non-ground truth based metrics.") 
     
     labels = []
     gt_metrics = {}
     nongt_metrics = {}
 
     gt_metrics_mean, gt_metrics_std = {}, {}
     nongt_metrics_mean, nongt_metrics_std = {}, {}
+
+    print("Hopkins Statistic (1=clustered, 0.5=random, 0=uniforrm) : {}".format(hopkins_statistic(X).round(3)))
     
     for n_clusters in num_clusters:
         ## Do 100 runs of kmeans for a given value of k? EXPENSIVE!
         # runIDs = np.random.randint(0, num_runs, size=num_runs)
         run_nongt_scores, run_gt_scores = {},{}
         
         best_run_id_, best_run_lbls_ = None, None
-        best_run_sil_score_, best_score_ = 0,0
+        best_run_sil_score_, best_score_ = 0, 0
         best_run_metric_ = 'Calinski-Harabasz'  #'Silhouette'
         for run in range(num_runs):
-            # if algorithm == 'k-Means':
-            #     clusterer = KMeans(n_clusters=n_clusters, random_state=run)
-            clusterer = model.set_params(n_clusters=n_clusters, random_state=run)
+            model_params[n_clusters_param_name] = n_clusters
+            model_params['random_state'] = run
+            # print(model_params)
+            clusterer = model.set_params(**model_params) #n_clusters=n_clusters, random_state=run
             run_lbls_=clusterer.fit_predict(X)
 
             if len(gt_labels)!=0:
                 gt_metrics_ = calc_gt_metrics(gt_labels=gt_labels, cluster_labels=run_lbls_)
                 run_gt_scores['run={}'.format(run)] = gt_metrics_
             nongt_metrics_ = calc_nongt_metrics(X=X, cluster_labels=run_lbls_)
             run_nongt_scores['run={}'.format(run)] = nongt_metrics_
@@ -440,27 +458,27 @@
         nongt_metrics_mean['k={}'.format(n_clusters)] = run_nongt_scores.T['mean']
         nongt_metrics_std['k={}'.format(n_clusters)] = run_nongt_scores.T['std']
         
         # print(nongt_metrics_mean)
         # print(nongt_metrics_std)
         # print(sys.exit())
             
-        ## -------------- Single Run -----------------
+        ## -------------- Single Run -------------------------------------------
         # Initialize the clusterer with n_clusters value and a random generator
         # seed of 10 for reproducibility.
         # clusterer = KMeans(n_clusters=n_clusters, random_state=10)
         # cluster_labels = clusterer.fit_predict(X)
         # labels.append(cluster_labels)
         # print(labels)
         # if gt_labels:
         #     gt_metrics['k={}'.format(n_clusters)] = calc_gt_metrics(gt_labels=gt_labels, cluster_labels=cluster_labels)
         # nongt_metrics_ = calc_nongt_metrics(X=X, cluster_labels=cluster_labels)
         # nongt_metrics['k={}'.format(n_clusters)] = nongt_metrics_
         # silhouette_avg = nongt_metrics_['Silhouette']
-        ## -------------------------------------------
+        ## -----------------------------------------------------------------------
         
         if make_silhoutte_plots:
             # Create a subplot with 1 row and 2 columns
             fig1, (ax1, ax2) = plt.subplots(1, 2, figsize=(20,10))
             # fig.set_size_inches(18, 7)
             # The 1st subplot is the silhouette plot
             # The silhouette coefficient can range from -1, 1 but in this example all
@@ -490,25 +508,26 @@
                     ith_cluster_silhouette_values,
                     facecolor=color,
                     edgecolor=color,
                     alpha=0.7,
                 )
 
                 # Label the silhouette plots with their cluster numbers at the middle
-                ax1.text(-0.05, y_lower + 0.5 * size_cluster_i, str(i))
+                ax1.text(-0.05, y_lower + 0.5 * size_cluster_i, str(i), fontsize=20)
 
                 # Compute the new y_lower for next plot
                 y_lower = y_upper + 10  # 10 for the 0 samples
 
-            ax1.set_title("The silhouette plot for the various clusters.")
-            ax1.set_xlabel("The silhouette coefficient values")
-            ax1.set_ylabel("Cluster label")
+            ax1.set_title("The silhouette plot for the various clusters", fontsize=20)
+            ax1.set_xlabel("The silhouette coefficient values", fontsize=20)
+            ax1.set_ylabel("Cluster label", fontsize=20)
 
             # The vertical line for average silhouette score of all the values
-            ax1.axvline(x=silhouette_avg, color="red", linestyle="--")
+            ax1.axvline(x=silhouette_avg, color="red", linestyle="--", label="Avg. Silhouette Score")
+            # ax1.text(silhouette_avg+0.05, 100.0, "avg. silhouette score = {}".format(silhouette_avg), color="red", fontsize=20, rotation=90)
 
             ax1.set_yticks([])  # Clear the yaxis labels / ticks
             ax1.set_xticks([-1, 0, 0.2, 0.4, 0.6, 0.8, 1])
 
             # 2nd Plot showing the actual clusters formed
             colors = cm.nipy_spectral(cluster_labels.astype(float) / n_clusters)
             if embed_data_in_2d:
@@ -516,14 +535,15 @@
                 X_embedded = TSNE(n_components=2).fit(X)
                 # X_embedded = Isomap(n_components=2).fit_transform(X)
                 # X_embedded = SpectralEmbedding(n_components=2).fit_transform(X)
                 # X_embedded = PCA(n_components=2).fit_transform(X)
                 ax2.scatter(
                     X_embedded[:, 0], X_embedded[:, 1], marker=".", s=100, lw=0, alpha=1, c=colors, edgecolor="k"
                 )
+                
             else:
                 print("Plotting first 2 features of the data...")
                 ax2.scatter(
                     X[:, 0], X[:, 1], marker=".", s=100, lw=0, alpha=1, c=colors, edgecolor="k"
                 )
 
             # # Labeling the clusters
@@ -538,24 +558,24 @@
             #     s=200,
             #     edgecolor="k",
             # )
 
             # for i, c in enumerate(centers):
             #     ax2.scatter(c[0], c[1], marker="$%d$" % i, alpha=1, s=50, edgecolor="k")
 
-            ax2.set_title("The visualization of the clustered data.")
+            ax2.set_title("The visualization of the clustered data", fontsize=20)
             # ax2.set_xlabel("TSNE axis-1")
             # ax2.set_ylabel("TSNE axis-2")
             # ax2.set_xlabel("Feature space for the 1st feature")
             # ax2.set_ylabel("Feature space for the 2nd feature")
 
             plt.suptitle(
                 "Silhouette analysis for KMeans clustering on sample data with n_clusters = %d"
                 % n_clusters,
-                fontsize=14,
+                fontsize=20,
                 fontweight="bold",
             )
             
             plt.tight_layout()
             if save:
                 print("Saving silhouette plot for k={} at {}"\
                       .format(n_clusters, os.path.join(save_dir,'silhouette_plots/{}_silhouette_plot.png'.format(n_clusters))))
@@ -590,28 +610,28 @@
                             annotate_topN_best_scores=annotate_topN_best_scores, annotN=annotN,
                             save_dir=save_dir, show=show, save=save)
 
     return labels, nongt_metrics, gt_metrics
 
 def eval_clustering(X=None, gt_labels=[], 
                     num_clusters = [2,3,5,10], num_runs=10, 
-                    model=None,
+                    model=None, n_clusters_param_name='n_clusters', model_params={},
                     # algorithm='k-Means',
                     dataset_type='features',
                     distance_metric='euclidean',
                     show=False, save=False, RESULTS_DIR=None, 
                     make_metrics_plots=True, annotate_topN_best_scores=True, annotN=3,
                     make_silhoutte_plots=False, embed_data_in_2d=False):
     
     if not os.path.exists(RESULTS_DIR):
         os.makedirs(RESULTS_DIR+'/silhouette_plots')
         os.makedirs(RESULTS_DIR+'/gt_metrics_plots')
         os.makedirs(RESULTS_DIR+'/nongt_metrics_plots')
     
     # if dataset_type == 'features':
     return cluster_feats(X=X, gt_labels=gt_labels, 
-                        model=model,
+                        model=model, n_clusters_param_name=n_clusters_param_name, model_params=model_params,
                         # algorithm=algorithm,
                         num_clusters=num_clusters, num_runs=num_runs,
                         show=show, save=save, save_dir=RESULTS_DIR,
                         make_metrics_plots=make_metrics_plots, annotate_topN_best_scores=annotate_topN_best_scores, annotN=annotN,
                         make_silhoutte_plots=make_silhoutte_plots, embed_data_in_2d=embed_data_in_2d)
```

### Comparing `clustutils4r-0.0.6/src/clustutils4r.egg-info/PKG-INFO` & `clustutils4r-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 
 `gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
 
 `num_clusters`: Range of no. of clusters to grid search over.
 
 `num_runs`: No. of runs per no. of cluster (defaults = 10).
 
-`make_metrics_plots`: Plot various clustering evaluation metrics. Depending on whether `gt_labels` are provided, you will get one or more plots - one for non-ground truth-based metrics and another for ground truth-based metrics. (default = `True`).
+`make_metrics_plots`: Plot various clustering evaluation metrics. Depending on whether `gt_labels` are provided, you will get one or two sets of plots - one for non-ground truth-based metrics and another for ground truth-based metrics. (default = `True`).
 
 `annotate_topN_best_scores`: Whether to annotate top N score in metrics plots (defined by `annotN`) (defaults = `True`).
 
 `annotN`: No. of top scores to annotated in metrics plots (defaults = 3).
 
 `make_silhoutte_plots`: Whether to make silhouette plots for each `num_clusters` value (default = `False`).
 
@@ -47,41 +47,48 @@
 
 `save`: set True if you want to save all results in RESULTS_DIR; defaults to False
 
 `show`: display all results; useful in notebooks; defaults to False
 
 ## Example Usage
 ```python
-import os
-from sklearn import datasets
-
-# Load the iris dataset
-data = datasets.load_digits()
-
-# Split the data into features and labels
-X = data.data
-y = data.target
+import matplotlib.pyplot as plt
+%matplotlib inline
 
-# Define clustering model
+import os, collections
+from sklearn import datasets
 from sklearn.cluster import KMeans
-kmeans_model = KMeans()
+from sklearn.mixture import GaussianMixture
 
-# Run the evaluation
 from clustutils4r.eval_clustering import eval_clustering
-range_clusters = list(range(3,15+1))
-labelled_datapoints, nongt_metrics, gt_metrics \
-    = eval_clustering(X=X, gt_labels=y,
-                        model=KMeans(),
-                        num_clusters=range_clusters, num_runs=10,
-                        annotate_topN_best_scores=True, annotN=3,
-                        make_metrics_plots=True,
-                        make_silhoutte_plots=True, embed_data_in_2d=True,
-                        show=True, 
-                        save=True, RESULTS_DIR=os.getcwd()+'/results',
-                    )
+
+## Load the dataset
+X, y = datasets.make_blobs(n_samples=5*100, 
+                           centers=5, 
+                           n_features=2, 
+                           random_state=0)
+
+## Setup model
+model = KMeans()
+model_params = {'init':'k-means++', 'n_init':1}
+n_clusters_param_name='n_clusters'
+
+## Run the evaluation
+range_clusters = list(range(3,10+1))
+labelled_datapoints, \
+   nongt_metrics, \
+      gt_metrics = eval_clustering(X=X, gt_labels=y,
+                                    model=model, model_params=model_params, n_clusters_param_name=n_clusters_param_name,
+                                    num_clusters=range_clusters, num_runs=10,
+                                    annotate_topN_best_scores=True, annotN=3,
+                                    make_metrics_plots=True,
+                                    make_silhoutte_plots=False,
+                                    show=True, 
+                                    save=True, RESULTS_DIR=os.getcwd()+'/results',
+                                )
 
 ```
 
 ![ch](tests/example_clustering/results/nongt_metrics_plots/cal_har.png)
 ![sil](tests/example_clustering/results/nongt_metrics_plots/dav_bou.png)
 ![sil](tests/example_clustering/results/nongt_metrics_plots/hopkn.png)
 ![sil](tests/example_clustering/results/nongt_metrics_plots/sil.png)
@@ -97,10 +104,10 @@
 ![ri](tests/example_clustering/results/gt_metrics_plots/rand_index.png)
 
 <!-- ![fmi](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/fmi.png)
 ![mi](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/mutual_info.png)
 ![hcv](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/hcv.png)
 ![ri](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/rand_index.png) -->
 
-![silplt](tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png)
+![silplt](tests/example_clustering/results/silhouette_plots/5_silhouette_plot.png)
 
 <!-- ![silplt](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
```

