# Comparing `tmp/suod-0.0.8.tar.gz` & `tmp/suod-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\suod-0.0.8.tar", last modified: Fri Oct  1 18:05:13 2021, max compression
+gzip compressed data, was "suod-0.0.9.tar", last modified: Sun Jul 16 11:31:55 2023, max compression
```

## Comparing `suod-0.0.8.tar` & `suod-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0        0        0        0 2021-10-01 18:05:13.000000 suod-0.0.8/
--rw-rw-rw-   0        0        0      215 2021-10-01 18:03:29.000000 suod-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    14515 2021-10-01 18:05:13.000000 suod-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    10927 2021-10-01 18:03:29.000000 suod-0.0.8/README.rst
--rw-rw-rw-   0        0        0       97 2021-10-01 18:03:29.000000 suod-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       87 2021-10-01 18:05:13.000000 suod-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1876 2021-10-01 18:03:29.000000 suod-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-01 18:05:13.000000 suod-0.0.8/suod/
--rw-rw-rw-   0        0        0        0 2021-10-01 18:03:29.000000 suod-0.0.8/suod/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-01 18:05:13.000000 suod-0.0.8/suod/models/
--rw-rw-rw-   0        0        0        0 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/__init__.py
--rw-rw-rw-   0        0        0    28017 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/base.py
--rw-rw-rw-   0        0        0     3445 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/cost_predictor.py
--rw-rw-rw-   0        0        0     3522 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/jl_projection.py
--rw-rw-rw-   0        0        0    10728 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/parallel_processes.py
-drwxrwxrwx   0        0        0        0 2021-10-01 18:05:13.000000 suod-0.0.8/suod/models/saved_models/
--rw-rw-rw-   0        0        0        0 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/saved_models/__init__.py
--rw-rw-rw-   0        0        0  3622995 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/saved_models/bps_prediction.joblib
--rw-rw-rw-   0        0        0  3720787 2021-10-01 18:03:29.000000 suod-0.0.8/suod/models/saved_models/bps_train.joblib
-drwxrwxrwx   0        0        0        0 2021-10-01 18:05:13.000000 suod-0.0.8/suod/utils/
--rw-rw-rw-   0        0        0        1 2021-10-01 18:03:29.000000 suod-0.0.8/suod/utils/__init__.py
--rw-rw-rw-   0        0        0    41772 2021-10-01 18:03:29.000000 suod-0.0.8/suod/utils/utility.py
--rw-rw-rw-   0        0        0      578 2021-10-01 18:03:29.000000 suod-0.0.8/suod/version.py
-drwxrwxrwx   0        0        0        0 2021-10-01 18:05:13.000000 suod-0.0.8/suod.egg-info/
--rw-rw-rw-   0        0        0    14515 2021-10-01 18:05:13.000000 suod-0.0.8/suod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2021-10-01 18:05:13.000000 suod-0.0.8/suod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-01 18:05:13.000000 suod-0.0.8/suod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2021-10-01 18:05:13.000000 suod-0.0.8/suod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-10-01 18:05:13.000000 suod-0.0.8/suod.egg-info/top_level.txt
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:31:55.017836 suod-0.0.9/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     1312 2023-07-16 11:29:26.000000 suod-0.0.9/LICENSE
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      328 2023-07-16 11:29:26.000000 suod-0.0.9/MANIFEST.in
+-rw-r--r--   0 yuezhao    (501) staff       (20)    11593 2023-07-16 11:31:55.017926 suod-0.0.9/PKG-INFO
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10636 2023-07-16 11:29:26.000000 suod-0.0.9/README.rst
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      104 2023-07-16 11:29:26.000000 suod-0.0.9/requirements.txt
+-rw-rw-r--   0 yuezhao    (501) staff       (20)       80 2023-07-16 11:31:55.018217 suod-0.0.9/setup.cfg
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     1876 2023-07-16 11:29:26.000000 suod-0.0.9/setup.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:31:54.990902 suod-0.0.9/suod/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:29:26.000000 suod-0.0.9/suod/__init__.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:31:54.992413 suod-0.0.9/suod/models/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/__init__.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    28423 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/base.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     3445 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/cost_predictor.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     3522 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/jl_projection.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10725 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/parallel_processes.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:31:55.010717 suod-0.0.9/suod/models/saved_models/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/saved_models/__init__.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)  4262065 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/saved_models/bps_prediction.joblib
+-rw-rw-r--   0 yuezhao    (501) staff       (20)  3622995 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/saved_models/bps_prediction_old.joblib
+-rw-rw-r--   0 yuezhao    (501) staff       (20)  4254577 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/saved_models/bps_train.joblib
+-rw-rw-r--   0 yuezhao    (501) staff       (20)  3720787 2023-07-16 11:29:26.000000 suod-0.0.9/suod/models/saved_models/bps_train_old.joblib
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:31:55.017313 suod-0.0.9/suod/utils/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)        1 2023-07-16 11:29:26.000000 suod-0.0.9/suod/utils/__init__.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    42325 2023-07-16 11:29:26.000000 suod-0.0.9/suod/utils/utility.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      578 2023-07-16 11:29:26.000000 suod-0.0.9/suod/version.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-07-16 11:31:54.991510 suod-0.0.9/suod.egg-info/
+-rw-r--r--   0 yuezhao    (501) staff       (20)    11593 2023-07-16 11:31:54.000000 suod-0.0.9/suod.egg-info/PKG-INFO
+-rw-r--r--   0 yuezhao    (501) staff       (20)      643 2023-07-16 11:31:54.000000 suod-0.0.9/suod.egg-info/SOURCES.txt
+-rw-r--r--   0 yuezhao    (501) staff       (20)        1 2023-07-16 11:31:54.000000 suod-0.0.9/suod.egg-info/dependency_links.txt
+-rw-r--r--   0 yuezhao    (501) staff       (20)      105 2023-07-16 11:31:54.000000 suod-0.0.9/suod.egg-info/requires.txt
+-rw-r--r--   0 yuezhao    (501) staff       (20)       14 2023-07-16 11:31:54.000000 suod-0.0.9/suod.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `suod-0.0.8/README.rst` & `suod-0.0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -35,28 +35,17 @@
 
 ----
 
 
 **Build Status & Coverage & Maintainability & License**
 
 
-.. image::  https://app.travis-ci.com/yzhao062/SUOD.svg?branch=master
-   :target: https://app.travis-ci.com/yzhao062/SUOD
-   :alt: Build Status
-
-
-.. image:: https://circleci.com/gh/yzhao062/SUOD.svg?style=svg
-   :target: https://circleci.com/gh/yzhao062/SUOD
-   :alt: Circle CI
-
-
-.. image:: https://ci.appveyor.com/api/projects/status/5kp8psvntp5m1d6m/branch/master?svg=true
-   :target: https://ci.appveyor.com/project/yzhao062/combo/branch/master
-   :alt: Appveyor
-
+.. image:: https://github.com/yzhao062/suod/actions/workflows/testing.yml/badge.svg
+   :target: https://github.com/yzhao062/suod/actions/workflows/testing.yml
+   :alt: testing
 
 .. image:: https://coveralls.io/repos/github/yzhao062/SUOD/badge.svg
    :target: https://coveralls.io/github/yzhao062/SUOD
    :alt: Coverage Status
 
 .. image:: https://img.shields.io/github/license/yzhao062/suod.svg
    :target: https://github.com/yzhao062/suod/blob/master/LICENSE
```

### Comparing `suod-0.0.8/setup.py` & `suod-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `suod-0.0.8/suod/models/base.py` & `suod-0.0.9/suod/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from suod.models.parallel_processes import balanced_scheduling
 from suod.models.parallel_processes import _parallel_fit
 from suod.models.parallel_processes import _parallel_predict
 from suod.models.parallel_processes import _parallel_predict_proba
 from suod.models.parallel_processes import _parallel_decision_function
 from suod.models.parallel_processes import _partition_estimators
 from suod.models.parallel_processes import _parallel_approx_estimators
-from ..utils.utility import _unfold_parallel, build_codes
+from ..utils.utility import _unfold_parallel, build_codes, _get_sklearn_version
 
 import warnings
 from collections import defaultdict
 
 # temporary solution for relative imports
 sys.path.append(
     os.path.abspath(os.path.join(os.path.dirname("__file__"), '..')))
@@ -212,16 +212,22 @@
         else:
             self.approx_ng_clf_list = approx_ng_clf_list
 
         this_directory = os.path.abspath(os.path.dirname(__file__))
 
         # validate the trained model
         if cost_forecast_loc_fit is None:
-            self.cost_forecast_loc_fit_ = os.path.join(
-                this_directory, 'saved_models', 'bps_train.joblib')
+
+            sklearn_version = _get_sklearn_version()
+            if sklearn_version[:3] >= '1.3':
+                self.cost_forecast_loc_fit_ = os.path.join(
+                    this_directory, 'saved_models', 'bps_train.joblib')
+            else:
+                self.cost_forecast_loc_fit_ = os.path.join(
+                    this_directory, 'saved_models', 'bps_train_old.joblib')
         else:
             self.cost_forecast_loc_fit_ = cost_forecast_loc_fit
 
         if cost_forecast_loc_pred is None:
             self.cost_forecast_loc_pred_ = os.path.join(
                 this_directory, 'saved_models', 'bps_prediction.joblib')
         else:
@@ -247,14 +253,18 @@
 
         # Validate target_dim_frac for random projection
         if isinstance(self.target_dim_frac, (numbers.Integral, np.integer)):
             self.target_dim_frac_ = self.target_dim_frac
         else:  # float
             self.target_dim_frac_ = int(self.target_dim_frac * n_features)
 
+        # it should have at least 1 dimension
+        if self.target_dim_frac_ < 1:
+            self.target_dim_frac_ = 1
+
         # build flags for random projection
         self.rp_flags_, _ = build_codes(self.base_estimators, self.rp_clf_list,
                                         self.rp_ng_clf_list,
                                         self.rp_flag_global)
 
         # decide whether bps is needed
         # it is turned off
```

### Comparing `suod-0.0.8/suod/models/cost_predictor.py` & `suod-0.0.9/suod/models/cost_predictor.py`

 * *Files identical despite different names*

### Comparing `suod-0.0.8/suod/models/jl_projection.py` & `suod-0.0.9/suod/models/jl_projection.py`

 * *Files identical despite different names*

### Comparing `suod-0.0.8/suod/models/parallel_processes.py` & `suod-0.0.9/suod/models/parallel_processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     """Private function used to partition estimators between jobs.
     """
     # Compute the number of jobs
     n_jobs = min(effective_n_jobs(n_jobs), n_estimators)
 
     # Partition estimators between jobs
     n_estimators_per_job = np.full(n_jobs, n_estimators // n_jobs,
-                                   dtype=np.int)
+                                   dtype=int)
     n_estimators_per_job[:n_estimators % n_jobs] += 1
     starts = np.cumsum(n_estimators_per_job)
 
     xdiff = [starts[n] - starts[n - 1] for n in range(1, len(starts))]
 
     if verbose:
         print("Split among workers default:", starts, xdiff)
```

### Comparing `suod-0.0.8/suod/models/saved_models/bps_prediction.joblib` & `suod-0.0.9/suod/models/saved_models/bps_prediction_old.joblib`

 * *Files identical despite different names*

### Comparing `suod-0.0.8/suod/models/saved_models/bps_train.joblib` & `suod-0.0.9/suod/models/saved_models/bps_train_old.joblib`

 * *Files identical despite different names*

### Comparing `suod-0.0.8/suod/utils/utility.py` & `suod-0.0.9/suod/utils/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Author: Yue Zhao <zhaoy@cmu.edu>
 # License: MIT
-import numpy as np
-from scipy.special import erf
-from sklearn.preprocessing import MinMaxScaler
+# suppress warnings
+import warnings
 
+import numpy as np
+import sklearn
+from pyod.models.abod import ABOD
+from pyod.models.hbos import HBOS
 from pyod.models.iforest import IForest
+from pyod.models.knn import KNN
 from pyod.models.lof import LOF
+from pyod.models.lscp import LSCP
+from pyod.models.mcd import MCD
 from pyod.models.ocsvm import OCSVM
 from pyod.models.pca import PCA
-from pyod.models.knn import KNN
-from pyod.models.hbos import HBOS
-from pyod.models.abod import ABOD
-from pyod.models.mcd import MCD
-from pyod.models.lscp import LSCP
-
-# suppress warnings
-import warnings
+from scipy.special import erf
+from sklearn.preprocessing import MinMaxScaler
 
 clf_idx_mapping = {
     'ABOD': 1,
     'CBLOF': 2,
     'FeatureBagging': 3,
     'HBOS': 4,
     'IForest': 5,
@@ -164,14 +164,34 @@
         probs[:, 0] = 1 - probs[:, 1]
         return probs
     else:
         raise ValueError(
             method, 'is not a valid probability conversion method')
 
 
+def _get_sklearn_version():  # pragma: no cover
+    """ Utility function to decide the version of sklearn.
+    PyOD will result in different behaviors with different sklearn version
+
+    Returns
+    -------
+    sk_learn version : int
+
+    """
+
+    sklearn_version = str(sklearn.__version__)
+    # print(sklearn_version)
+    # if int(sklearn_version.split(".")[1]) < 19 or int(
+    #         sklearn_version.split(".")[1]) > 24:
+    #     raise ValueError("Sklearn version error")
+    # print(sklearn_version)
+
+    return sklearn_version
+
+
 def get_estimators_small(contamination=0.1):
     """Internal method to create a list of 600 base outlier detectors.
 
     Parameters
     ----------
     contamination : float in (0., 0.5), optional (default=0.1)
         The amount of contamination of the data set,
```

### Comparing `suod-0.0.8/suod/version.py` & `suod-0.0.9/suod/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '0.0.8'  # pragma: no cover
+__version__ = '0.0.9'  # pragma: no cover
```

### Comparing `suod-0.0.8/suod.egg-info/SOURCES.txt` & `suod-0.0.9/suod.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 suod/__init__.py
 suod/version.py
@@ -13,10 +14,12 @@
 suod/models/__init__.py
 suod/models/base.py
 suod/models/cost_predictor.py
 suod/models/jl_projection.py
 suod/models/parallel_processes.py
 suod/models/saved_models/__init__.py
 suod/models/saved_models/bps_prediction.joblib
+suod/models/saved_models/bps_prediction_old.joblib
 suod/models/saved_models/bps_train.joblib
+suod/models/saved_models/bps_train_old.joblib
 suod/utils/__init__.py
 suod/utils/utility.py
```

