# Comparing `tmp/AutoCarver-5.0.8.tar.gz` & `tmp/AutoCarver-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.8.tar", last modified: Sat Jul 15 18:06:52 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.9.tar", last modified: Sun Jul 16 01:25:36 2023, max compression
```

## Comparing `AutoCarver-5.0.8.tar` & `AutoCarver-5.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32200 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18904 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.425522 AutoCarver-5.0.9/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34051 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.429523 AutoCarver-5.0.9/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23378 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34717 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28766 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.429523 AutoCarver-5.0.9/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18904 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 01:25:36.437523 AutoCarver-5.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.8/AutoCarver/auto_carver.py` & `AutoCarver-5.0.9/AutoCarver/auto_carver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,153 @@
 """Tool to build optimized buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
 from typing import Any
 
-from numpy import array, sqrt, searchsorted, add, unique, zeros
 from IPython.display import display_html
+from numpy import add, array, searchsorted, sqrt, unique, zeros
 from pandas import DataFrame, Series, crosstab
 from scipy.stats import chi2_contingency
 from tqdm import tqdm
 
+from .discretizers import GroupedList
 from .discretizers.discretizers import Discretizer
 from .discretizers.utils.base_discretizers import (
-    GroupedListDiscretizer,
+    BaseDiscretizer,
     convert_to_labels,
     convert_to_values,
 )
-from .discretizers.utils.grouped_list import GroupedList
 from .discretizers.utils.serialization import json_deserialize_values_orders
 
 
-class AutoCarver(GroupedListDiscretizer):
-    """Automatic carving of continuous, categorical and categorical ordinal
+class AutoCarver(BaseDiscretizer):
+    """Automatic carving of continuous, discrete, categorical and ordinal
     features that maximizes association with a binary target.
 
-    Modalities/values of features are carved/regrouped according to a computed
-    specific order defined based on their types:
-     - [Qualitative features] grouped based on modality target rate.
-     - [Qualitative ordinal features] grouped based on specified modality order
-     - [Quantitative features] grouped based on the order of their values.
-    Uses Tschurpow's T to find the optimal carving (regrouping) of modalities/
-    values of features.
-
-    Parameters
-    ----------
-    values_orders: dict, default {}
-        Dictionnary of features and list of their respective values' order.
-        Exemple: for an `age` feature, `values_orders` could be
-        `{'age': ['0-18', '18-30', '30-50', '50+']}`.
-
-    sort_by: str, default 'tschuprowt'
-        Association measure used to find the optimal group modality combination
-        Implemented: ['cramerv', 'tschuprowt']
-
-    max_n_mod: int, default 5
-        Maximum number of modalities for the carved features (excluding `nan`).
-         - All possible combinations of less than `max_n_mod` groups of
-           modalities will be tested.
-        Recommandation: `max_n_mod` should be set from 4 (faster) to 6
-        (preciser).
-
-    keep_nans: bool, default False
-        Whether or not to group `numpy.nan` to other modalities/values.
-
-    Examples
-    ----------
-
-    from AutoCarver import AutoCarver
-    from Discretizers import Discretizer
-    from sklearn.pipeline import Pipeline
-
-    # defining training and testing sets
-    X_train, y_train = train_set, train_set[target]
-    X_dev, y_dev = test_set, test_set[target]
-
-    # specifying features to be carved
-    selected_quanti = ['amount', 'distance', 'length', 'height']
-    selected_quali = ['age', 'type', 'grade', 'city']
-
-    # specifying orders of categorical ordinal features
-    values_orders = {
-        'age': ['0-18', '18-30', '30-50', '50+'],
-        'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
-    }
-
-    # pre-processing of features into categorical ordinal features
-    discretizer = Discretizer(
-        selected_quanti, selected_quali, min_freq=0.02, q=20,
-        values_orders=values_orders
-    )
-    X_train = discretizer.fit_transform(X_train, y_train)
-    X_dev = discretizer.transform(X_dev)
-
-    # storing Discretizer
-    pipe = [('Discretizer', discretizer)]
-
-    # updating features' values orders (every features are qualitative ordinal)
-    values_orders = discretizer.values_orders
-
-    # intiating AutoCarver
-    auto_carver = AutoCarver(
-        values_orders, sort_by='cramerv', max_n_mod=5, sample_size=0.01)
-
-    # fitting on training sample
-    # a test sample can be specified to evaluate carving robustness
-    X_train = auto_carver.fit_transform(X_train, y_train, X_dev, y_dev)
-
-    # applying transformation on test sample
-    X_dev = auto_carver.transform(X_dev)
-
-    # identifying non stable/robust features
-    print(auto_carver.non_viable_features)
-
-    # storing fitted GroupedListDiscretizer in a sklearn.pipeline.Pipeline
-    pipe += [('AutoCarver', auto_carver)]
-    pipe = Pipeline(pipe)
-
-    # applying pipe to a validation set or in production
-    X_val = pipe.transform(X_val)
-
+    Applies ``Discretizer``, data should not be given raw.
     """
 
     def __init__(
         self,
         quantitative_features: list[str],
         qualitative_features: list[str],
         min_freq: float,
         *,
         ordinal_features: list[str] = None,
         values_orders: dict[str, GroupedList] = None,
         max_n_mod: int = 5,
-        min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
+        # min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
         sort_by: str = "tschuprowt",
-        str_nan: str = "__NAN__",
-        str_default: str = "__OTHER__",
         output_dtype: str = "float",
         dropna: bool = True,
         copy: bool = False,
         verbose: bool = False,
         pretty_print: bool = False,
+        str_nan: str = "__NAN__",
+        str_default: str = "__OTHER__",
     ) -> None:
-        """_summary_
+        """Initiates an AutoCarver.
 
         Parameters
         ----------
         quantitative_features : list[str]
-            _description_
+            List of column names of quantitative features (continuous and discrete) to be carved
+
         qualitative_features : list[str]
-            _description_
+            List of column names of qualitative features (non-ordinal) to be carved
+
         min_freq : float
-            _description_
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be carved.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
         ordinal_features : list[str], optional
-            _description_, by default None
+            List of column names of ordinal features to be carved. For those features a list of
+            values has to be provided in the `values_orders` dict, by default None
+
         values_orders : dict[str, GroupedList], optional
-            _description_, by default None
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         max_n_mod : int, optional
-            _description_, by default 5
-        min_carved_freq : float, optional
-            _description_, by default 0
-        str_nan : str, optional
-            _description_, by default "__NAN__"
-        str_default : str, optional
-            _description_, by default "__OTHER__"
+            Maximum number of modality per feature, by default 5
+
+            All combinations of modalities for groups of modalities of sizes from 1 to `max_n_mod` will be tested.
+            The combination with the greatest association (as defined by `sort_by`) will be the selected one.
+
+            **Tip**: should be set between 4 (faster, more robust) and 7 (slower, preciser, less robust)
+
+        sort_by : str, optional
+            To be choosen amongst `["tschuprowt", "cramerv"]`, by default "tschuprowt"
+            Metric to be used to perform association measure between features and target.
+
+            * If `sort_by="tschuprowt"`, Tschuprow's T will be used as the association measure (more robust).
+            * If `sort_by="cramerv"`, Cramer's V will be used as the association measure (less robust).
+
+            **Tip**: use `sort_by="tschuprowt"` for more robust, or less output modalities,
+            use `sort_by="cramerv"` for more output modalities.
+
         output_dtype : str, optional
-            _description_, by default 'float'
+            To be choosen amongst `["float", "str"]`, by default "float"
+
+            * If `output_dtype="float"`, grouped modalities will be converted to there corresponding floating rank.
+            * If `output_dtype="str"`, a per-group modality will be set for all the modalities of a group.
+
         dropna : bool, optional
-            _description_, by default True
+            * If `dropna=True`, `AutoCarver` will try to group `numpy.nan` with other modalities.
+            * If `dropna=False`, `AutoCarver` all non-`numpy.nan` will be grouped, by default True
+
         copy : bool, optional
-            _description_, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            _description_, by default True
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, as long as
+            information on AutoCarver's processing and tables of target rates and frequencies for
+            X, by default False
+
         pretty_print : bool, optional
-            _description_, by default True
+            If `pretty_print=True`, adds to the verbose some HTML tables of target rates and frequencies for X and, if provided, X_dev.
+            Overrides the value of `verbose`, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
+
+        str_default : str, optional
+            String representation for default qualitative values, i.e. values less frequent than `min_freq`, by default "__OTHER__"
+
+        Examples
+        --------
+        See `AutoCarver examples <https://autocarver.readthedocs.io/en/latest/index.html>`_
         """
         # Lists of features
         self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
         self.ordinal_features = list(set(ordinal_features))
 
         # checking that qualitatitve and quantitative featues are distinct
-        assert all(quali_feature not in quantitative_features for quali_feature in qualitative_features + ordinal_features), f"A feature of `quantitative_features` also is in `qualitative_features` or `ordinal_features`. Be carreful with your inputs!"
-        assert all(quanti_feature not in qualitative_features + ordinal_features for quanti_feature in quantitative_features), f"A feature of `qualitative_features` or `ordinal_features` also is in `quantitative_features`. Be carreful with your inputs!"
+        assert all(
+            quali_feature not in quantitative_features
+            for quali_feature in qualitative_features + ordinal_features
+        ), "A feature of `quantitative_features` also is in `qualitative_features` or `ordinal_features`. Be carreful with your inputs!"
+        assert all(
+            quanti_feature not in qualitative_features + ordinal_features
+            for quanti_feature in quantitative_features
+        ), "A feature of `qualitative_features` or `ordinal_features` also is in `quantitative_features`. Be carreful with your inputs!"
 
         # initializing input_dtypes
         self.input_dtypes = {feature: "str" for feature in qualitative_features + ordinal_features}
         self.input_dtypes.update({feature: "float" for feature in quantitative_features})
 
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=self.input_dtypes,
             output_dtype=output_dtype,
             str_nan=str_nan,
             str_default=str_default,
@@ -189,89 +155,97 @@
             copy=copy,
             verbose=bool(max(verbose, pretty_print)),
         )
 
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
-        self.min_carved_freq = min_carved_freq
+        # self.min_carved_freq = min_carved_freq
         self.min_group_size = 1
         self.pretty_print = pretty_print
         measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
         assert (
             sort_by in measures
         ), f"""Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
         self.sort_by = sort_by
 
-    def prepare_data(
+    def _prepare_data(
         self,
         X: DataFrame,
         y: Series,
         X_dev: DataFrame = None,
         y_dev: Series = None,
     ) -> tuple[DataFrame, DataFrame]:
-        """Checks validity of provided data
+        """Validates format and content of X and y.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            _description_
+            Binary target feature with wich the association is maximized.
+
         X_dev : DataFrame, optional
-            _description_, by default None
+            Dataset to evalute the robustness of discretization, by default None
+            It should have the same distribution as X.
+
         y_dev : Series, optional
-            _description_, by default None
+            Binary target feature with wich the robustness of discretization is evaluated, by default None
 
         Returns
         -------
         tuple[DataFrame, DataFrame]
             Copies of (X, X_dev)
         """
         # Checking for binary target and copying X
-        x_copy = super().prepare_data(X, y)
-        x_dev_copy = super().prepare_data(X_dev, y_dev)
+        x_copy = super()._prepare_data(X, y)
+        x_dev_copy = super()._prepare_data(X_dev, y_dev)
 
         return x_copy, x_dev_copy
 
-    def remove_feature(self, feature: str) -> None:
-        """Removes a feature from all instances
+    def _remove_feature(self, feature: str) -> None:
+        """Removes a feature from all `feature` attributes
 
         Parameters
         ----------
         feature : str
-            Column name
+            Column name of the feature to remove
         """
         if feature in self.features:
-            super().remove_feature(feature)
+            super()._remove_feature(feature)
             if feature in self.ordinal_features:
                 self.ordinal_features.remove(feature)
 
     def fit(
         self,
         X: DataFrame,
         y: Series,
         X_dev: DataFrame = None,
         y_dev: Series = None,
     ) -> None:
-        """_summary_
+        """Finds the combination of modalities of X that provides the best association with y.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            _description_
+            Binary target feature with wich the association is maximized.
+
         X_dev : DataFrame, optional
-            _description_, by default None
+            Dataset to evalute the robustness of discretization, by default None
+            It should have the same distribution as X.
+
         y_dev : Series, optional
-            _description_, by default None
+            Binary target feature with wich the robustness of discretization is evaluated, by default None
         """
         # preparing datasets and checking for wrong values
-        x_copy, x_dev_copy = self.prepare_data(X, y, X_dev, y_dev)
+        x_copy, x_dev_copy = self._prepare_data(X, y, X_dev, y_dev)
 
         # discretizing all features
         discretizer = Discretizer(
             quantitative_features=self.quantitative_features,
             qualitative_features=self.qualitative_features,
             min_freq=self.min_freq,
             ordinal_features=self.ordinal_features,
@@ -288,15 +262,15 @@
 
         # updating values_orders according to base bucketization
         self.values_orders.update(discretizer.values_orders)
 
         # removing dropped features
         for feature in self.features:
             if feature not in discretizer.values_orders:
-                self.remove_feature(feature)
+                self._remove_feature(feature)
 
         # converting potential quantiles into there respective labels
         labels_orders = convert_to_labels(
             features=self.features,
             quantitative_features=self.quantitative_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
@@ -304,48 +278,52 @@
         )
 
         # computing crosstabs for each feature on train/test
         xtabs = get_xtabs(self.features, x_copy, y, labels_orders)
         xtabs_dev = get_xtabs(self.features, x_dev_copy, y_dev, labels_orders)
 
         # optimal butcketization/carving of each feature
-        all_features = self.features[:]  # necessary as features are being removed from self.features
+        all_features = self.features[
+            :
+        ]  # necessary as features are being removed from self.features
         for n, feature in enumerate(all_features):
             if self.verbose:  # verbose if requested
                 print(f"\n------\n[AutoCarver] Fit {feature} ({n+1}/{len(all_features)})\n---")
 
             # getting xtabs on train/test
             xtab = xtabs[feature]
             xtab_dev = xtabs_dev[feature]
             if self.verbose:  # verbose if requested
-                print(f"\n - Raw, feature distribution")
+                print("\n - Raw feature distribution")
                 print_xtabs(xtab, xtab_dev, pretty_print=self.pretty_print)
 
             # ordering
             order = labels_orders[feature]
 
             # getting best combination
-            best_combination = self.get_best_combination(order, xtab, xtab_dev=xtab_dev)
+            best_combination = self._get_best_combination(order, xtab, xtab_dev=xtab_dev)
 
             # checking that a suitable combination has been found
             if best_combination is not None:
                 order, xtab, xtab_dev = best_combination
                 if self.verbose:  # verbose if requested
-                    print(f"\n - Carved crosstab")
-                    print_xtabs(xtab, xtab_dev, pretty_print=self.pretty_print)  # TODO get the good labels
+                    print("\n - Carved feature distribution")
+                    print_xtabs(
+                        xtab, xtab_dev, pretty_print=self.pretty_print
+                    )  # TODO get the good labels
 
                 # updating label_orders
                 labels_orders.update({feature: order})
 
             # no suitable combination has been found -> removing feature
             else:
                 print(
                     f"No robust combination for feature '{feature}' could be found. It will be ignored. You might have to increase the size of your test sample (test sample not representative of test sample for this feature) or you should consider dropping this features."
                 )
-                self.remove_feature(feature)
+                self._remove_feature(feature)
                 if feature in labels_orders:
                     labels_orders.pop(feature)
 
             if self.verbose:  # verbose if requested
                 print("------\n")
 
         # converting potential labels into there respective values (quantiles)
@@ -355,28 +333,42 @@
                 quantitative_features=self.quantitative_features,
                 values_orders=self.values_orders,
                 label_orders=labels_orders,
                 str_nan=self.str_nan,
             )
         )
 
-        # TODO pretty displaying
-
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
 
-    def get_best_combination(
+    def _get_best_combination(
         self,
         order: GroupedList,
         xtab: DataFrame,
         *,
         xtab_dev: DataFrame = None,
     ) -> tuple[GroupedList, DataFrame, DataFrame]:
+        """_summary_
+
+        Parameters
+        ----------
+        order : GroupedList
+            _description_
+        xtab : DataFrame
+            _description_
+        xtab_dev : DataFrame, optional
+            _description_, by default None
+
+        Returns
+        -------
+        tuple[GroupedList, DataFrame, DataFrame]
+            _description_
+        """
         # raw ordering
         raw_order = GroupedList(order)
         if self.str_nan in raw_order:
             raw_order.remove(self.str_nan)
 
         # filtering out nans if requested from train/test crosstabs
         raw_xtab = filter_nan_xtab(xtab, self.str_nan)
@@ -437,40 +429,77 @@
                     xtab_dev = xtab_apply_order(xtab_dev, order)
 
         # checking that a suitable combination has been found
         if best_association is not None:
             return order, xtab, xtab_dev
 
 
-    
 def xtab_target_rate(xtab: DataFrame) -> DataFrame:
-    """Computes target rate per row for a binary target (column) in a crosstab"""
+    """Computes target rate per row for a binary target (column) in a crosstab
+
+    Parameters
+    ----------
+    xtab : DataFrame
+        _description_
 
+    Returns
+    -------
+    DataFrame
+        _description_
+    """
     return xtab[1].divide(xtab[0]).sort_values()
 
 
 def filter_nan_xtab(xtab: DataFrame, str_nan: str) -> DataFrame:
-    """Filters out nans from the crosstab"""
+    """Filters out nans from the crosstab
 
+    Parameters
+    ----------
+    xtab : DataFrame
+        _description_
+    str_nan : str
+        _description_
+
+    Returns
+    -------
+    DataFrame
+        _description_
+    """
     # cehcking for values in crosstab
     filtered_xtab = None
     if xtab is not None:
         # filtering out nans if requested from train crosstab
         filtered_xtab = xtab.copy()
         if str_nan in xtab.index:
             filtered_xtab = xtab.drop(str_nan, axis=0)
 
     return filtered_xtab
 
 
 def get_xtabs(
     features: list[str], X: DataFrame, y: Series, labels_orders: dict[str, GroupedList]
 ) -> dict[str, DataFrame]:
-    """Computes crosstabs for specified features and ensures that the crosstab is ordered according to the known labels"""
+    """Computes crosstabs for specified features and ensures that the crosstab is ordered according to the known labels
+
+    Parameters
+    ----------
+    features : list[str]
+        _description_
+    X : DataFrame
+        _description_
+    y : Series
+        _description_
+    labels_orders : dict[str, GroupedList]
+        _description_
 
+    Returns
+    -------
+    dict[str, DataFrame]
+        _description_
+    """
     # checking for empty datasets
     xtabs = {feature: None for feature in features}
     if X is not None:
         # crosstab for each feature
         for feature in features:
             # computing crosstab with str_nan
             xtab = crosstab(X[feature], y)
@@ -480,17 +509,33 @@
 
             # storing results
             xtabs.update({feature: xtab})
 
     return xtabs
 
 
-def association_xtab(xtab: DataFrame, n_obs, n_mod_y) -> dict[str, float]:
-    """Computes measures of association between feature x and feature2."""
+def association_xtab(xtab: DataFrame, n_obs: int, n_mod_y: int) -> dict[str, float]:
+    """Computes measures of association between feature and target by crosstab.
 
+    Parameters
+    ----------
+    xtab : DataFrame
+        Crosstab between feature and target.
+
+    n_obs : int
+        Sample total size.
+
+    n_mod_y : int
+        Number of modality of the target (and minimum number of modality).
+
+    Returns
+    -------
+    dict[str, float]
+        Cramer's V and Tschuprow's as a dict.
+    """
     # number of values taken by the features
     n_mod_x = xtab.shape[0]
 
     # Chi2 statistic
     chi2 = chi2_contingency(xtab)[0]
 
     # Cramer's V
@@ -498,17 +543,29 @@
 
     # Tschuprow's T
     tschuprowt = sqrt(chi2 / n_obs / sqrt((n_mod_x - 1) * (n_mod_y - 1)))
 
     return {"cramerv": cramerv, "tschuprowt": tschuprowt}
 
 
-def vectorized_groupby_sum(xtab: DataFrame, groupby: list[str]):
-    """Groups a crosstab by groupby and sums column values by groups"""
+def vectorized_groupby_sum(xtab: DataFrame, groupby: list[str]) -> DataFrame:
+    """Groups a crosstab by groupby and sums column values by groups
+
+    Parameters
+    ----------
+    xtab : DataFrame
+        _description_
+    groupby : list[str]
+        _description_
 
+    Returns
+    -------
+    DataFrame
+        _description_
+    """
     # all indices that may be duplicated
     index_values = array(groupby)
 
     # all unique indices deduplicated
     unique_indices = unique(index_values)
 
     # initiating summed up array with zeros
@@ -519,40 +576,85 @@
 
     # converting back to dataframe
     grouped_xtab = DataFrame(summed_values, index=unique_indices, columns=xtab.columns)
 
     return grouped_xtab
 
 
-def combinations_at_index(start_idx, order, nb_remaining_groups, min_group_size=1):
-    """Gets all possible combinations of sizes up to the last element of a list"""
+def combinations_at_index(
+    start_idx: int, order: list[Any], nb_remaining_groups: int, min_group_size: int = 1
+) -> tuple[list[Any], int, int]:
+    """Gets all possible combinations of sizes up to the last element of a list
+
+    Parameters
+    ----------
+    start_idx : int
+        _description_
+    order : list[Any]
+        _description_
+    nb_remaining_groups : int
+        _description_
+    min_group_size : int, optional
+        _description_, by default 1
+
+    Returns
+    -------
+    tuple[list[Any], int, int]
+        _description_
 
+    Yields
+    ------
+    Iterator[tuple[list[Any], int, int]]
+        _description_
+    """
     # iterating over each possible length of groups
     for size in range(min_group_size, len(order) + 1):
         next_idx = start_idx + size  # index from which to start the next group
 
         # checking that next index is not off the order list
         if next_idx < len(order) + 1:
             # checking that there are remaining groups or that it is the last group
             if (nb_remaining_groups > 1) | (next_idx == len(order)):
                 combination = list(order[start_idx:next_idx])
                 yield (combination, next_idx, nb_remaining_groups - 1)
 
 
 def consecutive_combinations(
-    raw_order,
-    max_group_size,
-    min_group_size=1,
-    nb_remaining_group=None,
-    current_combination=None,
-    next_index=None,
-    all_combinations=None,
-):
-    """Computes all possible combinations of values of order up to max_group_size."""
+    raw_order: list[Any],
+    max_group_size: int,
+    min_group_size: int = 1,
+    nb_remaining_group: int = None,
+    current_combination: list[Any] = None,
+    next_index: int = None,
+    all_combinations: list[list[Any]] = None,
+) -> list[list[Any]]:
+    """Computes all possible combinations of values of order up to max_group_size.
+
+    Parameters
+    ----------
+    raw_order : list[Any]
+        _description_
+    max_group_size : int
+        _description_
+    min_group_size : int, optional
+        _description_, by default 1
+    nb_remaining_group : int, optional
+        _description_, by default None
+    current_combination : list[Any], optional
+        _description_, by default None
+    next_index : int, optional
+        _description_, by default None
+    all_combinations : list[list[Any]], optional
+        _description_, by default None
 
+    Returns
+    -------
+    list[list[Any]]
+        _description_
+    """
     # initiating recursive attributes
     if current_combination is None:
         current_combination = []
     if next_index is None:
         next_index = 0
     if nb_remaining_group is None:
         nb_remaining_group = max_group_size
@@ -585,28 +687,41 @@
             next_index=next_index,
             all_combinations=all_combinations,
         )
 
     return all_combinations
 
 
-def xtab_target_rate(xtab: DataFrame) -> DataFrame:
-    """Computes target rate per row for a binary target (column) in a crosstab"""
-
-    return xtab[1].divide(xtab[0]).sort_values()
-
-
 def get_best_association(
     xtab: DataFrame,
     combinations: list[list[str]],
     sort_by: str,
     xtab_dev: DataFrame = None,
     verbose: bool = False,
 ) -> dict[str, Any]:
-    """Computes associations of the xtab for each combination"""
+    """Computes associations of the xtab for each combination
+
+    Parameters
+    ----------
+    xtab : DataFrame
+        _description_
+    combinations : list[list[str]]
+        _description_
+    sort_by : str
+        _description_
+    xtab_dev : DataFrame, optional
+        _description_, by default None
+    verbose : bool, optional
+        _description_, by default False
+
+    Returns
+    -------
+    dict[str, Any]
+        _description_
+    """
 
     # values to groupby indices with
     indices_to_groupby = [
         [value for values in ([group[0]] * len(group) for group in combination) for value in values]
         for combination in combinations
     ]
 
@@ -662,16 +777,30 @@
         if all(train_ranks == test_ranks):
             return association
 
 
 def add_nan_in_combinations(
     combinations: list[list[str]], str_nan: str, max_n_mod: int
 ) -> list[list[str]]:
-    """Adds nan to each possible group and a last group only with nan if the max_n_mod is not reached by the combination"""
+    """Adds nan to each possible group and a last group only with nan if the max_n_mod is not reached by the combination
 
+    Parameters
+    ----------
+    combinations : list[list[str]]
+        _description_
+    str_nan : str
+        _description_
+    max_n_mod : int
+        _description_
+
+    Returns
+    -------
+    list[list[str]]
+        _description_
+    """
     # iterating over each combination
     nan_combinations = []
     for combination in combinations:
         # adding nan to each group of the combination
         nan_combination = []
         for n in range(len(combination)):
             # copying input combination
@@ -690,16 +819,28 @@
 
         nan_combinations += nan_combination
 
     return nan_combinations
 
 
 def order_apply_combination(order: GroupedList, combination: list[list[Any]]) -> GroupedList:
-    """Converts a list of combination to a GroupedList"""
+    """Converts a list of combination to a GroupedList
+
+    Parameters
+    ----------
+    order : GroupedList
+        _description_
+    combination : list[list[Any]]
+        _description_
 
+    Returns
+    -------
+    GroupedList
+        _description_
+    """
     order_copy = GroupedList(order)
     for combi in combination:
         order_copy.group_list(combi, combi[0])
 
     return order_copy
 
 
@@ -712,46 +853,50 @@
         Crosstab
     order : GroupedList
         Combination of index to apply to the crosstab
 
     Returns
     -------
     dict[str, Any]
-        _description_
+        Orderd crosstab.
     """
     # checking for input values
     combi_xtab = None
     if xtab is not None:
         # grouping modalities in the crosstab
         groups = list(map(order.get_group, xtab.index))
         combi_xtab = xtab.groupby(groups, dropna=False, sort=False).sum()
 
     return combi_xtab
 
-def load_carver(json_serialized_auto_carver: dict) -> GroupedListDiscretizer:
-    """_summary_
+
+def load_carver(auto_carver_json: dict) -> BaseDiscretizer:
+    """Allows one to load an AutoCarver saved as a .json file.
+
+    The AutoCarver has to be saved with `json.dump(f, AutoCarver.to_json())`, otherwise there
+    can be no guarantee for it to be restored.
 
     Parameters
     ----------
-    json_serialized_auto_carver : str
-        _description_
+    auto_carver_json : str
+        Loaded .json file using `json.load(f)`.
 
     Returns
     -------
-    GroupedListDiscretizer
-        _description_
+    BaseDiscretizer
+        A fitted AutoCarver.
     """
     # deserializing values_orders
-    values_orders = json_deserialize_values_orders(json_serialized_auto_carver["values_orders"])
+    values_orders = json_deserialize_values_orders(auto_carver_json["values_orders"])
 
     # updating auto_carver attributes
-    json_serialized_auto_carver.update({"values_orders": values_orders})
+    auto_carver_json.update({"values_orders": values_orders})
 
-    # initiating GroupedListDiscretizer
-    auto_carver = GroupedListDiscretizer(**json_serialized_auto_carver)
+    # initiating BaseDiscretizer
+    auto_carver = BaseDiscretizer(**auto_carver_json)
     auto_carver.fit()
 
     return auto_carver
 
 
 def pretty_xtab(xtab: DataFrame = None) -> DataFrame:
     """Prints a binary xtab's statistics
@@ -780,14 +925,15 @@
         )
 
         # rounding up stats
         stats = stats.round(3)
 
     return stats
 
+
 def prettier_xtab(
     nice_xtab: DataFrame = None,
     caption: str = None,
 ) -> str:
     """Converts a crosstab to the HTML format, adding nice colors
 
     Parameters
@@ -800,15 +946,15 @@
     Returns
     -------
     str
         HTML format of the crosstab
     """
     """Pretty display of frequency and target rate per modality on the same line."""
     # checking for a provided xtab
-    nicer_xtab = ''
+    nicer_xtab = ""
     if nice_xtab is not None:
         # adding coolwarn color gradient
         nicer_xtab = nice_xtab.style.background_gradient(cmap="coolwarm")
 
         # printing inline notebook
         nicer_xtab = nicer_xtab.set_table_attributes("style='display:inline'")
 
@@ -817,14 +963,15 @@
             nicer_xtab = nicer_xtab.set_caption(caption)
 
         # converting to html
         nicer_xtab = nicer_xtab._repr_html_()
 
     return nicer_xtab
 
+
 def print_xtabs(xtab: DataFrame, xtab_dev: DataFrame = None, pretty_print: bool = False) -> None:
     """Prints crosstabs' target rates and frequencies per modality, in raw or html format
 
     Parameters
     ----------
     xtab : DataFrame
         Train crosstab
@@ -835,20 +982,20 @@
     """
     # getting pretty xtabs
     nice_xtab = pretty_xtab(xtab)
     nice_xtab_dev = pretty_xtab(xtab_dev)
 
     # case 0: no pretty hmtl printing
     if not pretty_print:
-        print(nice_xtab, '\n')
-    
+        print(nice_xtab, "\n")
+
     # case 1: pretty html printing
     else:
         # getting prettier xtabs
-        nicer_xtab = prettier_xtab(nice_xtab, caption='X distribution')
-        nicer_xtab_dev = prettier_xtab(nice_xtab_dev, caption='X_dev distribution')
+        nicer_xtab = prettier_xtab(nice_xtab, caption="X distribution")
+        nicer_xtab_dev = prettier_xtab(nice_xtab_dev, caption="X_dev distribution")
 
         # merging outputs
-        nicer_xtabs = nicer_xtab + '    ' + nicer_xtab_dev
-        
+        nicer_xtabs = nicer_xtab + "    " + nicer_xtab_dev
+
         # displaying html of colored DataFrame
-        display_html(nicer_xtabs, raw=True)
+        display_html(nicer_xtabs, raw=True)
```

### Comparing `AutoCarver-5.0.8/AutoCarver/converters.py` & `AutoCarver-5.0.9/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.8/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.9/AutoCarver/discretizers/discretizers.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,61 +3,31 @@
 """
 
 from typing import Union
 
 from numpy import nan
 from pandas import DataFrame, Series, unique
 
-from .utils.base_discretizers import GroupedListDiscretizer, check_new_values, min_value_counts
+from .utils.base_discretizers import BaseDiscretizer, check_new_values, min_value_counts
 from .utils.grouped_list import GroupedList
 from .utils.qualitative_discretizers import DefaultDiscretizer, OrdinalDiscretizer
 from .utils.quantitative_discretizers import QuantileDiscretizer
 from .utils.type_discretizers import StringDiscretizer
 
 
-class Discretizer(GroupedListDiscretizer):
-    """Automatic discretizing of continuous, categorical and categorical ordinal features.
+class Discretizer(BaseDiscretizer):
+    """Automatic discretization pipeline of continuous, discrete, categorical and ordinal features.
+
+    Pipeline steps: QuantitativeDiscretizer, QualitativeDiscretizer
 
     Modalities/values of features are grouped according to there respective orders:
-     - [Qualitative features] order based on modality target rate.
-     - [Qualitative ordinal features] user-specified order.
-     - [Quantitative features] real order of the values.
-
-    Parameters
-    ----------
-    quantitative_features: list
-        Contains quantitative (continuous) features to be discretized.
-
-    qualitative_features: list
-        Contains qualitative (categorical and categorical ordinal) features to be discretized.
-
-    min_freq: int, default None
-        [Qualitative features] Minimal frequency of a modality.
-         - NaNs are considered a specific modality but will not be grouped.
-         - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality
-        (smallest frequency or closest target rate), between the superior and inferior values (specified
-        in the `values_orders` dictionnary).
-        Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
-
-    q: int, default None
-        [Quantitative features] Number of quantiles to initialy cut the feature.
-         - NaNs are considered a specific value but will not be grouped.
-         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
-        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`).
-        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be
-        cut in q=5 quantiles.
-        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
-
-    values_orders: dict, default {}
-        [Qualitative ordinal features] dict of features values and list of orders of their values.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality
-        (smallest frequency or closest target rate), between the superior and inferior values (described
-        by the `values_orders`).
-        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
+
+    * [Qualitative features] order based on modality target rate.
+    * [Ordinal features] user-specified order.
+    * [Quantitative features] real order of the values.
     """
 
     def __init__(
         self,
         quantitative_features: list[str],
         qualitative_features: list[str],
         min_freq: float,
@@ -65,93 +35,107 @@
         ordinal_features: list[str] = None,
         values_orders: dict[str, GroupedList] = None,
         copy: bool = False,
         verbose: bool = False,
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
     ) -> None:
-        """_summary_
+        """Initiates a Discretizer (pipeline).
 
         Parameters
         ----------
         quantitative_features : list[str]
-            _description_
+            List of column names of quantitative features (continuous and discrete) to be dicretized
+
         qualitative_features : list[str]
-            _description_
+            List of column names of qualitative features (non-ordinal) to be discretized
+
         min_freq : float
-            _description_
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be discretized.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
         ordinal_features : list[str], optional
-            _description_, by default None
+            List of column names of ordinal features to be discretized. For those features a list of values has to be provided in the `values_orders` dict, by default None
+
         values_orders : dict[str, GroupedList], optional
-            _description_, by default None
-        input_dtypes : Union[str, dict[str, str]], optional
-            String of type to be considered for all features or
-            Dict of column names and associated types:
-            - if 'float' uses transform_quantitative
-            - if 'str' uses transform_qualitative,
-            default 'str'
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         copy : bool, optional
-            _description_, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            _description_, by default False
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, by default False
+
         str_nan : str, optional
-            _description_, by default '__NAN__'
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
+
         str_default : str, optional
-            _description_, by default '__OTHER__'
+            String representation for default qualitative values, i.e. values less frequent than `min_freq`, by default "__OTHER__"
+
+        Examples
+        --------
+        See `AutoCarver examples <https://autocarver.readthedocs.io/en/latest/index.html>`_
         """
         # Lists of features per type
         self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
         self.ordinal_features = list(set(ordinal_features))
 
         # initializing input_dtypes
         self.input_dtypes = {feature: "str" for feature in qualitative_features + ordinal_features}
         self.input_dtypes.update({feature: "float" for feature in quantitative_features})
 
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=self.input_dtypes,
             output_dtype="str",
             str_nan=str_nan,
             str_default=str_default,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
 
-    def remove_feature(self, feature: str) -> None:
-        """Removes a feature from the Discretizer
+    def _remove_feature(self, feature: str) -> None:
+        """Removes a feature from all `feature` attributes
 
         Parameters
         ----------
         feature : str
-            Column name of the feature
+            Column name of the feature to remove
         """
         if feature in self.features:
-            super().remove_feature(feature)
+            super()._remove_feature(feature)
             if feature in self.ordinal_features:
                 self.ordinal_features.remove(feature)
 
     def fit(self, X: DataFrame, y: Series) -> None:
-        """_summary_
+        """Finds relevant buckets of modalities of X to provide the best association with y.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            _description_
+            Binary target feature.
         """
         # Checking for binary target and copying X
-        x_copy = self.prepare_data(X, y)
+        x_copy = self._prepare_data(X, y)
 
         # [Qualitative features] Grouping qualitative features
         if len(self.qualitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print("------\n[Discretizer] Fit Qualitative Features\n---")
 
             # grouping qualitative features
@@ -170,15 +154,15 @@
 
             # storing orders of grouped features
             self.values_orders.update(qualitative_discretizer.values_orders)
 
             # removing dropped features
             for feature in self.qualitative_features:
                 if feature not in qualitative_discretizer.values_orders:
-                    self.remove_feature(feature)
+                    self._remove_feature(feature)
             if self.verbose:  # verbose if requested
                 print("------\n")
 
         # [Quantitative features] Grouping quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print("------\n[Discretizer] Fit Quantitative Features\n---")
@@ -196,101 +180,103 @@
 
             # storing orders of grouped features
             self.values_orders.update(quantitative_discretizer.values_orders)
 
             # removing dropped features
             for feature in self.quantitative_features:
                 if feature not in quantitative_discretizer.values_orders:
-                    self.remove_feature(feature)
+                    self._remove_feature(feature)
             if self.verbose:  # verbose if requested
                 print("------\n")
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
 
 
-class QualitativeDiscretizer(GroupedListDiscretizer):
-    """Automatic discretizing of categorical and categorical ordinal features.
+class QualitativeDiscretizer(BaseDiscretizer):
+    """Automatic discretiziation pipeline of categorical and ordinal features.
+
+    Pipeline steps: DefaultDiscretizer, OrdinalDiscretizer
 
     Modalities/values of features are grouped according to there respective orders:
-     - [Qualitative features] order based on modality target rate.
-     - [Qualitative ordinal features] user-specified order.
 
-    Parameters
-    ----------
-    features: list
-        Contains qualitative (categorical and categorical ordinal) features to be discretized.
-
-    min_freq: int
-        [Qualitative features] Minimal frequency of a modality.
-         - NaNs are considered a specific modality but will not be grouped.
-         - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality
-        (smallest frequency or closest target rate), between the superior and inferior values (specified
-        in the `values_orders` dictionnary).
-        Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
-
-    values_orders: dict, default {}
-        [Qualitative ordinal features] dict of features values and list of orders of their values.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality
-        (smallest frequency or closest target rate), between the superior and inferior values (described
-        by the `values_orders`).
-        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
+    * [Qualitative features] order based on modality target rate.
+    * [Ordinal features] user-specified order.
     """
 
     def __init__(
         self,
         qualitative_features: list[str],
         min_freq: float,
         *,
         ordinal_features: list[str] = None,
         values_orders: dict[str, GroupedList] = None,
         input_dtypes: Union[str, dict[str, str]] = "str",
-        str_nan: str = "__NAN__",
-        str_default: str = "__OTHER__",
         copy: bool = False,
         verbose: bool = False,
+        str_nan: str = "__NAN__",
+        str_default: str = "__OTHER__",
     ) -> None:
-        """_summary_
+        """Initiates a QualitativeDiscretizer (pipeline).
 
         Parameters
         ----------
         qualitative_features : list[str]
-            _description_
+            List of column names of qualitative features (non-ordinal) to be discretized
+
         min_freq : float
-            _description_
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be discretized.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
         ordinal_features : list[str], optional
-            _description_, by default None
+            List of column names of ordinal features to be discretized. For those features a list of values has to be provided in the `values_orders` dict, by default None
+
         values_orders : dict[str, GroupedList], optional
-            _description_, by default None
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         input_dtypes : Union[str, dict[str, str]], optional
-            String of type to be considered for all features or
-            Dict of column names and associated types:
-            - if 'float' uses transform_quantitative
-            - if 'str' uses transform_qualitative,
-            default 'str'
-        str_nan : str, optional
-            _description_, by default '__NAN__'
+            Input data type, converted to a dict of the provided type for each feature, by default "str"
+
+            * If `input_dtypes="str"`, features are considered as qualitative.
+            * If `input_dtypes="float"`, features are considered as quantitative.
+
         copy : bool, optional
-            _description_, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            _description_, by default False
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
+
+        str_default : str, optional
+            String representation for default qualitative values, i.e. values less frequent than `min_freq`, by default "__OTHER__"
+
+        Examples
+        --------
+        See `AutoCarver examples <https://autocarver.readthedocs.io/en/latest/index.html>`_
         """
         # Lists of features
         self.features = list(set(qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
         self.ordinal_features = list(set(ordinal_features))
 
         # class specific attributes
         self.min_freq = min_freq
 
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
             output_dtype="str",
             str_nan=str_nan,
             str_default=str_default,
@@ -299,46 +285,48 @@
         )
 
         # non-ordinal qualitative features
         self.non_ordinal_features = [
             feature for feature in self.qualitative_features if feature not in self.ordinal_features
         ]
 
-    def prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """Prepares the data for bucketization, checks column types.
-        Converts non-string columns into strings.
+    def _prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """Validates format and content of X and y. Converts non-string columns into strings.
 
         Parameters
         ----------
         X : DataFrame
-            Dataset to be bucketized
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            Model target, by default None
+            Binary target feature with wich the association is maximized.
 
         Returns
         -------
         DataFrame
-            Formatted X for bucketization
+            A formatted copy of X
         """
         # checking for binary target, copying X
-        x_copy = super().prepare_data(X, y)
+        x_copy = super()._prepare_data(X, y)
 
         # checking for ids (unique value per row)
         frequencies = x_copy[self.features].apply(
             lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
             axis=0,
         )
         # for each feature, checking that at least one value is more frequent than min_freq
-        all_features = self.features[:]  # necessary as features are being removed from self.features
+        all_features = self.features[
+            :
+        ]  # necessary as features are being removed from self.features
         for feature in all_features:
             if frequencies[feature] < self.min_freq:
                 print(
                     f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than min_freq={self.min_freq:2.1%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
                 )
-                self.remove_feature(feature)
+                self._remove_feature(feature)
 
         # checking for columns containing floats or integers even with filled nans
         dtypes = x_copy[self.features].fillna(self.str_nan).applymap(type).apply(unique)
         not_object = dtypes.apply(lambda u: any(typ != str for typ in u))
 
         # non qualitative features detected
         if any(not_object):
@@ -349,15 +337,17 @@
                 ]
                 print(
                     f"""Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
                 )
 
             # converting specified features into qualitative features
             string_discretizer = StringDiscretizer(
-                features=features_to_convert, values_orders=self.values_orders, verbose=self.verbose
+                qualitative_features=features_to_convert,
+                values_orders=self.values_orders,
+                verbose=self.verbose,
             )
             x_copy = string_discretizer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(string_discretizer.values_orders)
 
         # all known values for features
@@ -366,67 +356,62 @@
         # checking that all unique values in X are in values_orders
         check_new_values(
             x_copy, self.ordinal_features, known_values, self.str_nan, self.str_default
         )
 
         return x_copy
 
-    def remove_feature(self, feature: str) -> None:
-        """Removes a feature from the Discretizer
+    def _remove_feature(self, feature: str) -> None:
+        """Removes a feature from all `feature` attributes
 
         Parameters
         ----------
         feature : str
-            Column name of the feature
+            Column name of the feature to remove
         """
         if feature in self.features:
-            super().remove_feature(feature)
+            super()._remove_feature(feature)
             if feature in self.ordinal_features:
                 self.ordinal_features.remove(feature)
             if feature in self.non_ordinal_features:
                 self.non_ordinal_features.remove(feature)
 
     def fit(self, X: DataFrame, y: Series) -> None:
-        """Learning TRAIN distribution
+        """Finds relevant buckets of modalities of X to provide the best association with y.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
-        y : Series
-            _description_
+            Dataset used to discretize. Needs to have columns has specified in `features`.
 
-        Returns
-        -------
-        _type_
-            _description_
+        y : Series
+            Binary target feature.
         """
-
         # checking data before bucketization
-        x_copy = self.prepare_data(X, y)
+        x_copy = self._prepare_data(X, y)
 
         # [Qualitative ordinal features] Grouping rare values into closest common one
         if len(self.ordinal_features) > 0:
             ordinal_discretizer = OrdinalDiscretizer(
-                features=self.ordinal_features,
+                ordinal_features=self.ordinal_features,
                 values_orders=self.values_orders,
                 min_freq=self.min_freq,
                 verbose=self.verbose,
                 str_nan=self.str_nan,
                 copy=False,
             )
             ordinal_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
             self.values_orders.update(ordinal_discretizer.values_orders)
 
         # [Qualitative non-ordinal features] Grouping rare values into str_default '__OTHER__'
         if len(self.non_ordinal_features) > 0:
             default_discretizer = DefaultDiscretizer(
-                features=self.non_ordinal_features,
+                qualitative_features=self.non_ordinal_features,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
                 str_nan=self.str_nan,
                 str_default=self.str_default,
                 verbose=self.verbose,
                 copy=False,
             )
@@ -437,107 +422,133 @@
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
 
 
-class QuantitativeDiscretizer(GroupedListDiscretizer):
-    """Automatic discretizing of continuous features.
+class QuantitativeDiscretizer(BaseDiscretizer):
+    """Automatic discretization pipeline of continuous and discrete features.
 
-    Modalities/values of features are grouped according to there respective orders:
-     - [Quantitative features] real order of the values.
+    Pipeline steps: QuantileDiscretizer, OrdinalDiscretizer
 
-    Parameters
-    ----------
-    features: list
-        Contains quantitative (continuous) features to be discretized.
-
-    min_freq: float, default None
-        [Quantitative features] Inverse of the number of quantiles `q` to initialy cut the feature.
-         - NaNs are considered a specific value but will not be grouped.
-         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
-        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`).
-        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be
-        cut in q=5 quantiles.
-        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
+    Modalities/values of features are grouped according to there respective orders:
 
+     * [Quantitative features] real order of the values.
     """
 
     def __init__(
         self,
         quantitative_features: list[str],
         min_freq: float,
         *,
         values_orders: dict[str, GroupedList] = None,
         input_dtypes: Union[str, dict[str, str]] = "float",
-        str_nan: str = "__NAN__",
         verbose: bool = False,
         copy: bool = False,
+        str_nan: str = "__NAN__",
     ) -> None:
-        """_summary_
+        """Initiates a Discretizer (pipeline).
 
         Parameters
         ----------
-        features : list[str]
-            _description_
+        quantitative_features : list[str]
+            List of column names of quantitative features (continuous and discrete) to be dicretized
+
         min_freq : float
-            _description_
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be discretized.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
         values_orders : dict[str, GroupedList], optional
-            _description_, by default None
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         input_dtypes : Union[str, dict[str, str]], optional
-            String of type to be considered for all features or
-            Dict of column names and associated types:
-            - if 'float' uses transform_quantitative
-            - if 'str' uses transform_qualitative,
-            default 'str'
-        str_nan : str, optional
-            _description_, by default '__NAN__'
+            Input data type, converted to a dict of the provided type for each feature, by default "str"
+
+            * If `input_dtypes="str"`, features are considered as qualitative.
+            * If `input_dtypes="float"`, features are considered as quantitative.
+
         copy : bool, optional
-            _description_, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            _description_, by default False
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
+
+        Examples
+        --------
+        See `AutoCarver examples <https://autocarver.readthedocs.io/en/latest/index.html>`_
         """
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
             features=quantitative_features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
             output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
 
-    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
-        """Checking data for bucketization"""
+    def _prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """Validates format and content of X and y.
+
+        Parameters
+        ----------
+        X : DataFrame
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
+        y : Series
+            Binary target feature with wich the association is maximized.
+
+        Returns
+        -------
+        DataFrame
+            A formatted copy of X
+        """
         # checking for binary target and copying X
-        x_copy = super().prepare_data(X, y)
+        x_copy = super()._prepare_data(X, y)
 
         # checking for quantitative columns
         dtypes = x_copy[self.features].applymap(type).apply(unique)
         not_numeric = dtypes.apply(lambda u: str in u)
         assert all(
             ~not_numeric
         ), f"Non-numeric features: {str(list(not_numeric[not_numeric].index))}"
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
-        """Learning TRAIN distribution"""
+        """Finds relevant buckets of modalities of X to provide the best association with y.
 
+        Parameters
+        ----------
+        X : DataFrame
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
+        y : Series
+            Binary target feature.
+        """
         # checking data before bucketization
-        x_copy = self.prepare_data(X, y)
+        x_copy = self._prepare_data(X, y)
 
         # [Quantitative features] Grouping values into quantiles
         quantile_discretizer = QuantileDiscretizer(
-            self.features,
+            quantitative_features=self.features,
             min_freq=self.min_freq,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
             copy=True,  # needs to be True so that it does not transform x_copy
             verbose=self.verbose,
         )
         x_copy = quantile_discretizer.fit_transform(x_copy, y)
@@ -557,15 +568,15 @@
 
         # identifying features that have rare modalities
         has_rare = list(frequencies[frequencies <= q_min_freq].index)
 
         # Grouping rare modalities
         if len(has_rare) > 0:
             ordinal_discretizer = OrdinalDiscretizer(
-                has_rare,
+                ordinal_features=has_rare,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
                 str_nan=self.str_nan,
                 copy=False,
                 verbose=self.verbose,
                 input_dtypes=self.input_dtypes,
             )
```

### Comparing `AutoCarver-5.0.8/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.9/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,51 +8,70 @@
 from pandas import DataFrame, Series, isna, notna, unique
 from sklearn.base import BaseEstimator, TransformerMixin
 
 from .grouped_list import GroupedList
 from .serialization import json_serialize_values_orders
 
 
-# TODO: output a json
-class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
-    """Discretizer that uses a dict of grouped values."""
+class BaseDiscretizer(BaseEstimator, TransformerMixin):
+    """Applies discretization using a dict of GroupedList to transform a DataFrame's columns."""
 
     def __init__(
         self,
         features: list[str],
         *,
         values_orders: dict[str, GroupedList] = None,
         input_dtypes: Union[str, dict[str, str]] = "str",
         output_dtype: str = "str",
-        str_nan: str = None,
-        str_default: str = None,
         dropna: bool = True,
         copy: bool = True,
         verbose: bool = True,
+        str_nan: str = None,
+        str_default: str = None,
     ) -> None:
-        """Initiates a Discretizer by dict of GroupedList
+        """Initiates a BaseDiscretizer.
 
         Parameters
         ----------
         features : list[str]
-            List of column names to be discretized
+            List of column names of features (continuous, discrete, categorical or ordinal) to be dicretized
+
         values_orders : dict[str, GroupedList], optional
-            Per feature ordering, by default None
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         input_dtypes : Union[str, dict[str, str]], optional
-            String of type to be considered for all features or
-            Dict of column names and associated types:
-            - if 'float' uses transform_quantitative
-            - if 'str' uses transform_qualitative,
-            by default 'str'
+            Input data type, converted to a dict of the provided type for each feature, by default "str"
+
+            * If `input_dtypes="str"`, features are considered as qualitative.
+            * If `input_dtypes="float"`, features are considered as quantitative.
+
         output_dtype : str, optional
-            _description_, by default 'str'
-        str_nan : str, optional
-            Default string value attributed to nan, by default None
+            To be choosen amongst `["float", "str"]`, by default "str"
+
+            * If `output_dtype="float"`, grouped modalities will be converted to there corresponding floating rank.
+            * If `output_dtype="str"`, a per-group modality will be set for all the modalities of a group.
+
+        dropna : bool, optional
+            * If `dropna=True`, ``numpy.nan`` will be attributed there label.
+            * If `dropna=False`, ``numpy.nan`` will be restored after discretization, by default True
+
         copy : bool, optional
-            Whether or not to copy the input DataFrame, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
+        verbose : bool, optional
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, as long as
+            information on AutoCarver's processing and tables of target rates and frequencies for
+            X, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
+
+        str_default : str, optional
+            String representation for default qualitative values, i.e. values less frequent than `min_freq`, by default "__OTHER__"
         """
         self.features = list(set(features))
         if values_orders is None:
             values_orders: dict[str, GroupedList] = {}
         self.values_orders = {
             feature: GroupedList(values) for feature, values in values_orders.items()
         }
@@ -87,15 +106,15 @@
         self.quantitative_features = [
             feature for feature in features if self.input_dtypes[feature] == "float"
         ]
 
         # for each feature, getting label associated to each value
         self.labels_per_values: dict[str, dict[Any, Any]] = {}  # will be initiated during fit
 
-    def get_labels_per_values(self, output_dtype: str) -> dict[str, dict[Any, Any]]:
+    def _get_labels_per_values(self, output_dtype: str) -> dict[str, dict[Any, Any]]:
         """Creates a dict that contains, for each feature, for each value, the associated label
 
         Parameters
         ----------
         output_dtype : str
             Whether or not to convert the output to float.
 
@@ -134,49 +153,50 @@
                     label_per_value.update({value: label})
 
             # storing in full dict
             labels_per_values.update({feature: label_per_value})
 
         return labels_per_values
 
-    def remove_feature(self, feature: str) -> None:
-        """Removes a feature from the Discretizer
+    def _remove_feature(self, feature: str) -> None:
+        """Removes a feature from all `feature` attributes
 
         Parameters
         ----------
         feature : str
-            Column name of the feature
+            Column name of the feature to remove
         """
         if feature in self.features:
             self.features.remove(feature)
             if feature in self.qualitative_features:
                 self.qualitative_features.remove(feature)
             if feature in self.quantitative_features:
                 self.quantitative_features.remove(feature)
             if feature in self.values_orders:
                 self.values_orders.pop(feature)
             if feature in self.input_dtypes:
                 self.input_dtypes.pop(feature)
             if feature in self.labels_per_values:
                 self.labels_per_values.pop(feature)
 
-    def prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """_summary_
+    def _prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """Validates format and content of X and y.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
-        y : Series, optional
-            _description_, by default None
+            Dataset used to discretize. Needs to have columns has specified in `features`, by default None.
+
+        y : Series
+            Binary target feature, by default None.
 
         Returns
         -------
         DataFrame
-            _description_
+            A formatted copy of X
         """
         # copying X
         x_copy = X
         if self.copy and X is not None:
             missing_columns = [feature for feature in self.features if feature not in X]
             assert (
                 len(missing_columns) == 0
@@ -208,82 +228,80 @@
             feature for feature in self.features if feature not in self.values_orders
         ]
         assert (
             len(missing_features) == 0
         ), f"Missing values_orders for following features {str(missing_features)}."
 
         # for each feature, getting label associated to each value
-        self.labels_per_values = self.get_labels_per_values(self.output_dtype)
+        self.labels_per_values = self._get_labels_per_values(self.output_dtype)
 
         return self
 
     def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """Groups values of features (values_orders keys) according to
-        there corresponding GroupedList (values_orders values) based on
-        the `GroupedList.content` dict.
+        """Applies discretization using a dict of GroupedList to transform a DataFrame's columns whatever there ``input_dtypes``.
+
+        Groups values of features (keys of ``values_orders``) according to there ``GroupedList`` (defined in ``values_orders``) by
+        reading the historized merges inside the ``GroupedList.content`` dict.
 
         Parameters
         ----------
         X : DataFrame
-            Contains columns named after `features` attribute
+            Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
 
         Returns
         -------
         DataFrame
-            _description_
+            Discretized X.
         """
-
         # copying dataframes
         x_copy = X
         if self.copy:
             x_copy = X.copy()
 
         # transforming quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print(
-                    f" - [GroupedListDiscretizer] Transform Quantitative {str(self.quantitative_features)}"
+                    f" - [BaseDiscretizer] Transform Quantitative {str(self.quantitative_features)}"
                 )
             x_copy = self.transform_quantitative(x_copy, y)
 
         # transforming qualitative features
         if len(self.qualitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print(
-                    f" - [GroupedListDiscretizer] Transform Qualitative {str(self.qualitative_features)}"
+                    f" - [BaseDiscretizer] Transform Qualitative {str(self.qualitative_features)}"
                 )
             x_copy = self.transform_qualitative(x_copy, y)
 
         # reinstating nans
         if not self.dropna:
             for feature in self.features:
                 label_per_value = self.labels_per_values[feature]
                 if self.str_nan in label_per_value:  # checking for nans in the feature
                     x_copy[feature] = x_copy[feature].replace(label_per_value[self.str_nan], nan)
 
         return x_copy
 
     def transform_quantitative(self, X: DataFrame, y: Series) -> DataFrame:
-        """Groups values of features (values_orders keys) according to
-        there corresponding GroupedList (values_orders values) based on
-        the `GroupedList.content` dict.
+        """Applies discretization using a dict of GroupedList to transform a DataFrame's Quantitative columns (as defined by ``input_dtypes=="float"``).
 
         Parameters
         ----------
         X : DataFrame
-            Contains columns named after `values_orders` keys
+            Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
 
         Returns
         -------
         DataFrame
-            _description_
+            Discretized X.
         """
         # dataset length
         x_len = X.shape[0]
 
         # grouping each quantitative feature
         for feature in self.quantitative_features:
             # feature's labels associated to each quantile
@@ -321,29 +339,27 @@
             # converting nans to there value
             if any(nans):
                 X.loc[nans, feature] = self.labels_per_values[feature].get(nan_value, self.str_nan)
 
         return X
 
     def transform_qualitative(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """Groups values of features (values_orders keys) according to
-        there corresponding GroupedList (values_orders values) based on
-        the `GroupedList.content` dict.
+        """Applies discretization using a dict of GroupedList to transform a DataFrame's Qualitative columns (as defined by ``input_dtypes=="str"``).
 
         Parameters
         ----------
         X : DataFrame
-            Contains columns named after `values_orders` keys
+            Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
 
         Returns
         -------
         DataFrame
-            _description_
+            Discretized X.
         """
         # filling up nans with specified value
         if self.str_nan:
             X[self.qualitative_features] = X[self.qualitative_features].fillna(self.str_nan)
 
         # checking that all unique values in X are in values_orders
         check_new_values(
@@ -362,20 +378,22 @@
                 if feature in self.qualitative_features
             }
         )
 
         return X
 
     def to_json(self) -> str:
-        """Converts the GroupedListDiscretizer's values_orders to .json
+        """Converts the BaseDiscretizer's values_orders to .json format.
+
+        To be used with ``json.dump``.
 
         Returns
         -------
         str
-            JSON serialized GroupedListDiscretizer
+            JSON serialized BaseDiscretizer
         """
         # extracting content dictionnaries
         json_serialized_groupedlistdiscretizer = {
             "features": self.features,
             "values_orders": json_serialize_values_orders(self.values_orders),
             "input_dtypes": self.input_dtypes,
             "output_dtype": self.output_dtype,
@@ -384,26 +402,25 @@
             "dropna": self.dropna,
             "copy": self.copy,
         }
 
         # dumping as json
         return json_serialized_groupedlistdiscretizer
 
+    # TODO: add crosstabs per feature for a provided X?
     def summary(self) -> DataFrame:
-        """Summarizes the data bucketization
-
-        TODO: add crosstabs per feature for a provided X?
+        """Summarizes the data discretization process.
 
         Returns
         -------
         DataFrame
-            A summary of feature's values
+            A summary of features' values per modalities.
         """
         # raw label per value with output_dtype 'str'
-        raw_labels_per_values = self.get_labels_per_values(output_dtype="str")
+        raw_labels_per_values = self._get_labels_per_values(output_dtype="str")
 
         # initiating summaries
         summaries: list[dict[str, Any]] = []
         for feature in self.features:
             # adding each value/label
             for value, label in self.labels_per_values[feature].items():
                 # initiating feature summary (default value/label)
@@ -464,16 +481,34 @@
 def convert_to_labels(
     features: list[str],
     quantitative_features: list[str],
     values_orders: dict[str, GroupedList],
     str_nan: str,
     dropna: bool = True,
 ) -> dict[str, GroupedList]:
-    """Converts a values_orders values to labels (quantiles)"""
+    """Converts a values_orders values (quantiles) to labels
 
+    Parameters
+    ----------
+    features : list[str]
+        _description_
+    quantitative_features : list[str]
+        _description_
+    values_orders : dict[str, GroupedList]
+        _description_
+    str_nan : str
+        _description_
+    dropna : bool, optional
+        _description_, by default True
+
+    Returns
+    -------
+    dict[str, GroupedList]
+        _description_
+    """
     # copying values_orders without nans
     labels_orders = {
         feature: GroupedList([value for value in values_orders[feature] if value != str_nan])
         for feature in features
     }
 
     # for quantitative features getting labels per quantile
@@ -505,14 +540,34 @@
 def convert_to_values(
     features: list[str],
     quantitative_features: list[str],
     values_orders: dict[str, GroupedList],
     label_orders: dict[str, GroupedList],
     str_nan: str,
 ):
+    """Converts a values_orders labels to values (quantiles)
+
+    Parameters
+    ----------
+    features : list[str]
+        _description_
+    quantitative_features : list[str]
+        _description_
+    values_orders : dict[str, GroupedList]
+        _description_
+    label_orders : dict[str, GroupedList]
+        _description_
+    str_nan : str
+        _description_
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
     # for quantitative features getting labels per quantile
     if any(quantitative_features):
         # getting quantile per group "name"
         labels_to_quantiles = get_labels_quantiles(quantitative_features, values_orders, str_nan)
 
     # updating feature orders (that keeps NaNs and quantiles)
     for feature in features:
@@ -561,16 +616,20 @@
 ) -> float:
     """Minimum of modalities' frequencies.
 
     Parameters
     ----------
     x : Series
         _description_
-    values_orders : dict[str, GroupedList]
-        _description_
+    values_orders : dict[str, GroupedList], optional
+        _description_, by default None
+    dropna : bool, optional
+        _description_, by default False
+    normalize : bool, optional
+        _description_, by default True
 
     Returns
     -------
     float
         _description_
     """
     # modality frequency
```

### Comparing `AutoCarver-5.0.8/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.0.9/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Union
 
 from numpy import ndarray, sort
 from pandas import isna
 
 
 class GroupedList(list):
-    """An ordered list that's extended with a dict."""
+    """An ordered list that's extended with a per-value content dict."""
 
     def __init__(self, iterable: Union[ndarray, dict, list, tuple] = ()) -> None:
         """An ordered list that historizes its elements' content.
 
         Parameters
         ----------
         iterable : Union[ndarray, dict, list, tuple], optional
```

### Comparing `AutoCarver-5.0.8/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.9/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,141 +1,160 @@
 """Tools to build simple buckets out of Qualitative features
 for a binary classification model.
 """
 
-from typing import Any, Dict, List, Union
+from typing import Any, Union
 
 from numpy import argmin, nan, select
 from pandas import DataFrame, Series, isna, notna, unique
 
 from .base_discretizers import (
-    GroupedListDiscretizer,
+    BaseDiscretizer,
     check_missing_values,
     check_new_values,
     convert_to_labels,
     convert_to_values,
     nan_unique,
     target_rate,
     value_counts,
 )
 from .grouped_list import GroupedList
 from .type_discretizers import StringDiscretizer
 
 
-class DefaultDiscretizer(GroupedListDiscretizer):
-    """Groups a qualitative features' values less frequent than min_freq into a str_default string
+class DefaultDiscretizer(BaseDiscretizer):
+    """Automatic discretization of categorical features, building simple groups frequent enough.
 
-    Only use for qualitative non-ordinal features
+    Groups a qualitative features' values less frequent than ``min_freq`` into a ``str_default`` string.
+
+    NaNs are left untouched.
+
+    Only use for qualitative non-ordinal features.
     """
 
     def __init__(
         self,
-        features: list[str],
+        qualitative_features: list[str],
         min_freq: float,
         *,
         values_orders: dict[str, GroupedList] = None,
-        str_default: str = "__OTHER__",
-        str_nan: str = "__NAN__",
         copy: bool = False,
         verbose: bool = False,
+        str_default: str = "__OTHER__",
+        str_nan: str = "__NAN__",
     ) -> None:
-        """_summary_
+        """Initiates a DefaultDiscretizer.
 
         Parameters
         ----------
-        features : list[str]
-            List of column names to be discretized
+        qualitative_features : list[str]
+            List of column names of qualitative features (non-ordinal) to be discretized
+
         min_freq : float
-            Minimum frequency per modality. Less frequent modalities are grouped in the closest value of the order.
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be discretized.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
         values_orders : dict[str, GroupedList], optional
-            Dict of column names (keys) and modalities' associated order (values), by default None
-        str_default : str, optional
-            _description_, by default "__OTHER__"
-        str_nan : str, optional
-            _description_, by default "__NAN__"
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         copy : bool, optional
-            _description_, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            _description_, by default False
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
+
+        str_default : str, optional
+            String representation for default qualitative values, i.e. values less frequent than `min_freq`, by default "__OTHER__"
         """
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
-            features=features,
+            features=qualitative_features,
             values_orders=values_orders,
             input_dtypes="str",
             output_dtype="str",
             str_nan=str_nan,
             str_default=str_default,
             copy=copy,
             verbose=verbose,
         )
 
         self.min_freq = min_freq
 
-    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
-        """Called during fit step
+    def _prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """Validates format and content of X and y.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            _description_
+            Binary target feature with wich the association is maximized.
 
         Returns
         -------
         DataFrame
-            _description_
+            A formatted copy of X
         """
         # checking for binary target
-        x_copy = super().prepare_data(X, y)
+        x_copy = super()._prepare_data(X, y)
 
         # checks and initilizes values_orders
-        for feature in self.features:
+        for feature in self.qualitative_features:
             # initiating features missing from values_orders
             if feature not in self.values_orders:
                 self.values_orders.update({feature: GroupedList(nan_unique(x_copy[feature]))})
 
         # checking that all unique values in X are in values_orders
         check_new_values(
-            x_copy, self.features, self.values_orders, self.str_nan, self.str_default
-        )  # TODO problem here
+            x_copy, self.qualitative_features, self.values_orders, self.str_nan, self.str_default
+        )
         # checking that all unique values in values_orders are in X
-        check_missing_values(x_copy, self.features, self.values_orders)
+        check_missing_values(x_copy, self.qualitative_features, self.values_orders)
 
         # adding NANS
-        for feature in self.features:
+        for feature in self.qualitative_features:
             if any(x_copy[feature].isna()):
                 self.values_orders[feature].append(self.str_nan)
 
         # filling up NaNs
-        x_copy = x_copy[self.features].fillna(self.str_nan)
+        x_copy = x_copy[self.qualitative_features].fillna(self.str_nan)
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
-        """Learns modalities that are common enough (greater than min_freq)
+        """Finds simple buckets of modalities of X.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            _description_
+            Binary target feature.
         """
         # copying dataframe and checking data before bucketization
-        x_copy = self.prepare_data(X, y)
+        x_copy = self._prepare_data(X, y)
 
         if self.verbose:  # verbose if requested
-            print(f" - [DefaultDiscretizer] Fit {str(self.features)}")
+            print(f" - [DefaultDiscretizer] Fit {str(self.qualitative_features)}")
 
         # computing frequencies of each modality
         frequencies = x_copy.apply(value_counts, normalize=True, axis=0)
 
-        for feature in self.features:
+        for feature in self.qualitative_features:
             # sorting orders based on target rates
             order = self.values_orders[feature]
 
             # checking for rare values
             values_to_group = [
                 val
                 for val, freq in frequencies[feature].items()
@@ -152,15 +171,15 @@
                 # updating values_orders
                 self.values_orders.update({feature: order})
 
         # computing target rate per modality for ordering
         target_rates = x_copy.apply(target_rate, y=y, ascending=True, axis=0)
 
         # sorting orders based on target rates
-        for feature in self.features:
+        for feature in self.qualitative_features:
             order = self.values_orders[feature]
 
             # new ordering according to target rate
             new_order = list(target_rates[feature])
 
             # leaving NaNs at the end of the list
             if self.str_nan in new_order:
@@ -172,89 +191,101 @@
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
 
 
-class OrdinalDiscretizer(GroupedListDiscretizer):
-    """Discretizes ordered qualitative features into groups more frequent than min_freq.
+class OrdinalDiscretizer(BaseDiscretizer):
+    """Automatic discretization of ordinal features, grouping less frequent modalities with the
+    closest modlity in target rate or by frequency.
+
     NaNs are left untouched.
 
-    Modality is choosen amongst the preceding and following values in the provided order.
-    The choosen modality is:
-    - the closest in target rate
-    - or the one with the lowest frequency
+    Only use for qualitative ordinal features.
     """
 
     def __init__(
         self,
-        features: list[str],
-        values_orders: dict[str, GroupedList],
+        ordinal_features: list[str],
         min_freq: float,
+        values_orders: dict[str, GroupedList],
         *,
-        str_nan: str = "__NAN__",
         input_dtypes: Union[str, dict[str, str]] = "str",
         copy: bool = False,
         verbose: bool = False,
+        str_nan: str = "__NAN__",
     ):
-        """Initializes a OrdinalDiscretizer
+        """Initiates a DefaultDiscretizer.
 
         Parameters
         ----------
-        features : list[str]
-            List of column names to be discretized
-        values_orders : dict[str, Any]
-            Dict of column names (keys) and modalities' associated order (values)
+        ordinal_features : list[str]
+            List of column names of ordinal features to be discretized. For those features a list of values has to be provided in the `values_orders` dict.
+
         min_freq : float
-            Minimum frequency per modality. Less frequent modalities are grouped in the closest value of the order.
-        str_nan : str, optional
-            _description_, by default None
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be discretized.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
+        values_orders : dict[str, GroupedList], optional
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         input_dtypes : Union[str, dict[str, str]], optional
-            String of type to be considered for all features or
-            Dict of column names and associated types:
-            - if 'float' uses transform_quantitative
-            - if 'str' uses transform_qualitative,
-            default 'str'
+            Input data type, converted to a dict of the provided type for each feature, by default "str"
+
+            * If `input_dtypes="str"`, features are considered as qualitative.
+            * If `input_dtypes="float"`, features are considered as quantitative.
+
         copy : bool, optional
-            _description_, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            _description_, by default False
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
         """
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
-            features=features,
+            features=ordinal_features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
             output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
 
-    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
-        """Called during fit step
+    def _prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """Validates format and content of X and y.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            _description_
+            Binary target feature.
 
         Returns
         -------
         DataFrame
-            _description_
+            A formatted copy of X
         """
         # checking for binary target and copying X
-        x_copy = super().prepare_data(X, y)
+        x_copy = super()._prepare_data(X, y)
         # adding NANS
         for feature in self.features:
             if any(x_copy[feature].isna()):
                 values = self.values_orders[feature]
                 if not values.contains(self.str_nan):
                     values.append(self.str_nan)
                     self.values_orders.update({feature: values})
@@ -262,28 +293,29 @@
         # removing NaNs if any already imputed -> grouping only non-nan values
         if self.str_nan:
             x_copy = x_copy.replace(self.str_nan, nan)
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
-        """Learns common modalities on the training set
+        """Finds simple buckets of modalities of X.
 
         Parameters
         ----------
         X : DataFrame
-            Training set that contains columns named after `values_orders` keys.
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            Model target.
+            Binary target feature.
         """
         if self.verbose:  # verbose if requested
             print(f" - [OrdinalDiscretizer] Fit {str(self.features)}")
 
         # checking values orders
-        x_copy = self.prepare_data(X, y)
+        x_copy = self._prepare_data(X, y)
 
         # converting potential quantiles into there labels
         known_orders = convert_to_labels(
             features=self.features,
             quantitative_features=self.quantitative_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
@@ -313,54 +345,77 @@
 
         # discretizing features based on each feature's values_order
         super().fit(x_copy, y)
 
         return self
 
 
-class ChainedDiscretizer(GroupedListDiscretizer):
-    """Chained Discretization based on a list of GroupedList."""
+class ChainedDiscretizer(BaseDiscretizer):
+    """Automatic discretization of categorical features, joining rare modalities into higher
+    level groups.
+
+    For each provided ``GroupedList`` from ``chained_orders``, values less frequent than
+    ``min_freq`` are grouped in there respective group, as defined by ``GroupedList``.
+    """
 
     def __init__(
         self,
-        features: list[str],
+        qualitative_features: list[str],
         min_freq: float,
         chained_orders: list[GroupedList],
         *,
         values_orders: dict[str, GroupedList] = None,
         remove_unknown: bool = True,
-        str_nan: str = "__NAN__",
         copy: bool = False,
         verbose: bool = False,
+        str_nan: str = "__NAN__",
     ) -> None:
-        """Initializes a ChainedDiscretizer
+        """Initiates a ChainedDiscretizer.
 
         Parameters
         ----------
-        features : list[str]
-            Columns to be bucketized
-        min_freq : float
-            Minimum frequency per modality
+        qualitative_features : list[str]
+            List of column names of qualitative features (non-ordinal) to be discretized
+
         chained_orders : list[GroupedList]
-            List of modality orders
+            A list of interlocked higher level groups for each modalities of each ordianl feature.
+            Values of ``chained_orders[0]`` have to be grouped in ``chained_order[1]`` etc.
+
+        min_freq : float
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be discretized.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
+        values_orders : dict[str, GroupedList], optional
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         remove_unknown : bool, optional
-            Whether or not to remove unknown values. If true, they are grouped
-            into the value of`str_nan` otherwise it throws an error,
-            by default True
-        str_nan : str, optional
-            Value used to replace nan. If set, same value should be used across
-            all Discretizers, by default "__NAN__"
+            Whether or not to remove unknown values, by default True.
+            If ``remove_unknown=True``, unknown values are grouped into the value ``str_nan``
+
         copy : bool, optional
-            Whether or not to copy the dataset, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            Whether or not to print information during fit, by default False
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
+
+        str_default : str, optional
+            String representation for default qualitative values, i.e. values less frequent than `min_freq`, by default "__OTHER__"
         """
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
-            features=features,
+            features=qualitative_features,
             values_orders=values_orders,
             input_dtypes="str",
             output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
@@ -409,29 +464,29 @@
                 if value not in order.values():
                     order.append(value)
             order = order.sort_by(self.known_values)
             self.values_orders.update({feature: order})
 
         self.verbose = verbose
 
-    def prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """Prepares the data for bucketization, checks column types.
-        Converts non-string columns into strings.
+    def _prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """Validates format and content of X and y. Converts non-string columns into strings.
 
         Parameters
         ----------
         X : DataFrame
-            Dataset to be bucketized
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
         y : Series
-            Model target, by default None
+            Binary target feature, not used, by default None.
 
         Returns
         -------
         DataFrame
-            Formatted X for bucketization
+            A formatted copy of X
         """
         # copying dataframe
         x_copy = X.copy()
 
         # checking for ids (unique value per row)
         frequencies = x_copy[self.features].apply(
             lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
@@ -439,15 +494,15 @@
         )
         # for each feature, checking that at least one value is more frequent than min_freq
         for feature in self.features:
             if frequencies[feature] < self.min_freq:
                 print(
                     f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than {self.min_freq:2.2%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
                 )
-                self.remove_feature(feature)
+                self._remove_feature(feature)
 
         # checking for columns containing floats or integers even with filled nans
         dtypes = x_copy[self.features].fillna(self.str_nan).applymap(type).apply(unique)
         not_object = dtypes.apply(lambda u: any(typ != str for typ in u))
 
         # non qualitative features detected
         if any(not_object):
@@ -458,15 +513,15 @@
                 ]
                 print(
                     f"""Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
                 )
 
             # converting specified features into qualitative features
             stringer = StringDiscretizer(
-                features=features_to_convert, values_orders=self.values_orders
+                qualitative_features=features_to_convert, values_orders=self.values_orders
             )
             x_copy = stringer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(stringer.values_orders)
 
         # all known values for features
@@ -477,30 +532,26 @@
 
         # filling nans
         x_copy = x_copy.fillna(self.str_nan)
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
-        """_summary_
+        """Finds simple buckets of modalities of X.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
-        y : Series, optional
-            _description_, by default None
+            Dataset used to discretize. Needs to have columns has specified in `features`.
 
-        Returns
-        -------
-        _type_
-            _description_
+        y : Series
+            Binary target feature, not used, by default None.
         """
         # filling nans
-        x_copy = self.prepare_data(X, y)
+        x_copy = self._prepare_data(X, y)
 
         # iterating over each feature
         if self.verbose:  # verbose if requested
             print(f" - [ChainedDiscretizer] Fit {str(self.features)}")
         for feature in self.features:
             # computing frequencies of each modality
             frequencies = x_copy[feature].value_counts(normalize=True)
@@ -569,30 +620,25 @@
 def find_common_modalities(
     df_feature: Series,
     y: Series,
     min_freq: float,
     values_orders: dict[str, GroupedList],
     len_df: int = None,
 ) -> dict[str, Any]:
-    """Découpage en modalités de fréquence minimal (Cas des variables ordonnées).
-
-    Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
-    Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
-    Une fois il n'y a plus de valeurs qui soient sur-représentées,
-    on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
+    """Recursively finds the closest modality by target rate or by frequency.
 
     Parameters
     ----------
     df_feature : Series
         _description_
     y : Series
         _description_
     min_freq : float
         _description_
-    order : GroupedList
+    values_orders : dict[str, GroupedList]
         _description_
     len_df : int, optional
         _description_, by default None
 
     Returns
     -------
     dict[str, Any]
@@ -672,28 +718,32 @@
 
     return grouped_series
 
 
 def find_closest_modality(
     idx: int, order: GroupedList, frequencies: list[float], target_rates: Series, min_freq: float
 ) -> Any:
-    """HELPER Finds the closest modality in terms of frequency and target rate
+    """Finds the closest modality in terms of frequency and target rate
 
     Parameters
     ----------
     idx : int
         _description_
-    freq_target : Series
+    order : GroupedList
+        _description_
+    frequencies : list[float]
+        _description_
+    target_rates : Series
         _description_
     min_freq : float
         _description_
 
     Returns
     -------
-    int
+    Any
         _description_
     """
     # case 1: lowest ranked modality
     if idx == 0:
         idx_closest_modality = 1
 
     # case 2: highest ranked modality
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `AutoCarver-5.0.8/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.9/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,108 @@
 """Tools to build simple buckets out of Quantitative features
 for a binary classification model.
 """
 
-from typing import Any, Dict, List
+from typing import Any
 
 from numpy import array, inf, linspace, nan, quantile
 from pandas import DataFrame, Series, isna, notna
 
-from .base_discretizers import GroupedListDiscretizer, applied_to_dict_list
+from .base_discretizers import BaseDiscretizer, applied_to_dict_list
 from .grouped_list import GroupedList
 
 
-class QuantileDiscretizer(GroupedListDiscretizer):
-    """Builds per-feature buckets of quantiles"""
+class QuantileDiscretizer(BaseDiscretizer):
+    """Automatic discretizing of continuous and discrete features, building simple groups of quantiles of values.
+
+    Quantile discretization creates a lot of modalities (for example: 100 modalities for ``min_freq=0.01``).
+    Set ``min_freq`` with caution.
+
+    The number of quantiles depends on overrepresented modalities and nans:
+
+    * Values more frequent than ``min_freq`` are set as there own modalities.
+    * Other values are cut in quantiles using ``numpy.quantile``.
+    * The number of quantiles is set as ``(1-freq_of_frequent_modalities)/(min_freq)``.
+    * Nans are considered as a modality (and are taken into account in ``freq_of_frequent_modalities``).
+    """
 
     def __init__(
         self,
-        features: list[str],
+        quantitative_features: list[str],
         min_freq: float,
         *,
         values_orders: dict[str, Any] = None,
-        str_nan: str = "__NAN__",
         copy: bool = False,
         verbose: bool = False,
+        str_nan: str = "__NAN__",
     ) -> None:
-        """Discretizes quantitative features into groups of q quantiles
+        """Initiates a QuantileDiscretizer.
 
         Parameters
         ----------
-        features : List[str]
-            _description_
+        quantitative_features : list[str]
+            List of column names of quantitative features (continuous and discrete) to be dicretized
+
         min_freq : float
-            _description_
-        values_orders : Dict[str, Any], optional
-            _description_, by default None
-        str_nan : str, optional
-            _description_, by default '__NAN__'
+            Minimum frequency per grouped modalities.
+
+            * Features whose most frequent modality is less frequent than `min_freq` will not be discretized.
+            * Sets the number of quantiles in which to discretize the continuous features.
+            * Sets the minimum frequency of a quantitative feature's modality.
+
+            **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
+
+        values_orders : dict[str, GroupedList], optional
+            Dict of feature's column names and there associated ordering.
+            If lists are passed, a GroupedList will automatically be initiated, by default None
+
         copy : bool, optional
-            _description_, by default False
+            If `copy=True`, feature processing at transform is applied to a copy of the provided DataFrame, by default False
+
         verbose : bool, optional
-            _description_, by default False
+            If `verbose=True`, prints raw Discretizers Fit and Transform steps, by default False
+
+        str_nan : str, optional
+            String representation to input `numpy.nan`. If `dropna=False`, `numpy.nan` will be left unchanged, by default "__NAN__"
         """
-        # Initiating GroupedListDiscretizer
+        # Initiating BaseDiscretizer
         super().__init__(
-            features=features,
+            features=quantitative_features,
             values_orders=values_orders,
             input_dtypes="float",
             output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
         self.min_freq = min_freq
         self.q = round(1 / min_freq)  # number of quantiles
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
-        """_summary_
+        """Finds simple buckets of modalities of X.
 
         Parameters
         ----------
         X : DataFrame
-            _description_
-        y : Series, optional
-            _description_, by default None
+            Dataset used to discretize. Needs to have columns has specified in `features`.
+
+        y : Series
+            Binary target feature, not used, by default None
         """
         if self.verbose:  # verbose if requested
-            print(f" - [QuantileDiscretizer] Fit {str(self.features)}")
+            print(f" - [QuantileDiscretizer] Fit {str(self.quantitative_features)}")
 
         # computing quantiles for the feature
-        quantiles = applied_to_dict_list(X[self.features].apply(find_quantiles, q=self.q, axis=0))
+        quantiles = applied_to_dict_list(
+            X[self.quantitative_features].apply(find_quantiles, q=self.q, axis=0)
+        )
 
         # storing ordering
-        for feature in self.features:
+        for feature in self.quantitative_features:
             # Converting to a groupedlist
             order = GroupedList(quantiles[feature] + [inf])
 
             # adding NANs if ther are any
             if any(isna(X[feature])):
                 order.append(self.str_nan)
 
@@ -89,25 +115,39 @@
         return self
 
 
 def find_quantiles(
     df_feature: Series,
     q: int,
     len_df: int = None,
-    quantiles: List[float] = None,
-) -> List[float]:
-    """[Quantitative] Découpage en quantile de la feature.
-
-    Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
-    Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
-    Une fois il n'y a plus de valeurs qui soient sur-représentées,
-    on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
-
+    quantiles: list[float] = None,
+) -> list[float]:
+    """Finds quantiles of a Series recursively.
+
+    * Values more frequent than ``min_freq`` are set as there own modalities.
+    * Other values are cut in quantiles using ``numpy.quantile``.
+    * The number of quantiles is set as ``(1-freq_of_frequent_modalities)/(min_freq)``.
+    * Nans are considered as a modality (and are taken into account in ``freq_of_frequent_modalities``).
+
+    Parameters
+    ----------
+    df_feature : Series
+        _description_
+    q : int
+        _description_
+    len_df : int, optional
+        _description_, by default None
+    quantiles : list[float], optional
+        _description_, by default None
+
+    Returns
+    -------
+    list[float]
+        _description_
     """
-
     # initialisation de la taille total du dataframe
     if len_df is None:
         len_df = len(df_feature)
 
     # initialisation de la liste des quantiles
     if quantiles is None:
         quantiles = []
```

### Comparing `AutoCarver-5.0.8/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.0.9/AutoCarver/discretizers/utils/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Sets of helper functions for GroupedListDiscretizer JSON serialization"""
+"""Sets of helper functions for BaseDiscretizer JSON serialization"""
 
 from json import dumps, loads
 from typing import Any, Union
 
 from numpy import floating, inf, integer, isfinite
 
 from .grouped_list import GroupedList
```

### Comparing `AutoCarver-5.0.8/AutoCarver/feature_selector.py` & `AutoCarver-5.0.9/AutoCarver/feature_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Tools to select the best Quantitative and Qualitative features."""
 
 from math import sqrt
 from random import shuffle
-from typing import Any, Callable, Dict, Tuple
+from typing import Any, Callable, Tuple
 
 from IPython.display import display_html
 from numpy import inf, nan, ones, triu
 from pandas import DataFrame, Series, crosstab, notna
 from scipy.stats import chi2_contingency, kruskal
 from sklearn.base import BaseEstimator, TransformerMixin
 from statsmodels.formula.api import ols
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 
-from .discretizers.utils.base_discretizers import GroupedListDiscretizer
+from .discretizers.utils.base_discretizers import BaseDiscretizer
 from .discretizers.utils.grouped_list import GroupedList
 
 
 # TODO: convert to groupedlistdiscretizer
 # TODO: add parameter to shut down displayed info
 class FeatureSelector(BaseEstimator, TransformerMixin):
     """A pipeline of measures to perform EDA and feature pre-selection
@@ -141,15 +141,15 @@
         self.copy = copy
         self.verbose = verbose
         self.params = params
 
         self.associations = None
         self.filtered_associations = None
 
-    def measure(self, x: Series, y: Series) -> Dict[str, Any]:
+    def measure(self, x: Series, y: Series) -> dict[str, Any]:
         """Measures association between x and y"""
 
         passed = True  # measures keep going only if previous basic tests are passed
         association = {}
 
         # iterating over each measure
         for measure in self.measures:
@@ -305,19 +305,19 @@
 
         return X
 
 
 # MEASURES
 def nans_measure(
     active: bool,
-    association: Dict[str, Any],
+    association: dict[str, Any],
     x: Series,
     y: Series = None,
     **params,
-) -> Tuple[bool, Dict[str, Any]]:
+) -> tuple[bool, dict[str, Any]]:
     """Measure of the percentage of NaNs
 
     Parameters
     ----------
     thresh_nan, float: default 1.
       Maximum percentage of NaNs in a feature
     """
@@ -334,34 +334,34 @@
         active = pct_nan < params.get("thresh_nan", 1.0)
 
     return active, association
 
 
 def dtype_measure(
     active: bool,
-    association: Dict[str, Any],
+    association: dict[str, Any],
     x: Series,
     y: Series = None,
     **params,
-) -> Tuple[bool, Dict[str, Any]]:
+) -> tuple[bool, dict[str, Any]]:
     """Gets dtype"""
 
     # updating association
     association.update({"dtype": x.dtype})
 
     return active, association
 
 
 def mode_measure(
     active: bool,
-    association: Dict[str, Any],
+    association: dict[str, Any],
     x: Series,
     y: Series = None,
     **params,
-) -> Tuple[bool, Dict[str, Any]]:
+) -> tuple[bool, dict[str, Any]]:
     """Measure of the percentage of the Mode
 
     Parameters
     ----------
     thresh_mode, float: default 1.
       Maximum percentage of the mode of a feature
     """
@@ -377,16 +377,16 @@
         # Excluding feature with too frequent modes
         active = pct_mode < params.get("thresh_mode", 1.0)
 
     return active, association
 
 
 def kruskal_measure(
-    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
-) -> Tuple[bool, Dict[str, Any]]:
+    active: bool, association: dict[str, Any], x: Series, y: Series, **params
+) -> tuple[bool, dict[str, Any]]:
     """Kruskal-Wallis statistic between x (quantitative) and y (binary)"""
 
     # check that previous steps where passed
     if active:
         nans = x.isnull()  # ckecking for nans
 
         # computation of Kruskal-Wallis statistic
@@ -396,16 +396,16 @@
         if kw:
             association.update({"kruskal_measure": kw[0]})
 
     return active, association
 
 
 def R_measure(
-    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
-) -> Tuple[bool, Dict[str, Any]]:
+    active: bool, association: dict[str, Any], x: Series, y: Series, **params
+) -> tuple[bool, dict[str, Any]]:
     """R of the linear regression of x (quantitative) by y (binary)"""
 
     # check that previous steps where passed
     if active:
         nans = x.isnull()  # ckecking for nans
 
         # grouping feature and target
@@ -422,19 +422,19 @@
                 association.update({"R_measure": nan})
 
     return active, association
 
 
 def zscore_measure(
     active: bool,
-    association: Dict[str, Any],
+    association: dict[str, Any],
     x: Series,
     y: Series = None,
     **params,
-) -> Tuple[bool, Dict[str, Any]]:
+) -> tuple[bool, dict[str, Any]]:
     """Computes outliers based on the z-score
 
     Parameters
     ----------
     thresh_outlier, float: default 1.
       Maximum percentage of Outliers in a feature
     """
@@ -464,19 +464,19 @@
         active = pct_zscore < params.get("thresh_outlier", 1.0)
 
     return active, association
 
 
 def iqr_measure(
     active: bool,
-    association: Dict[str, Any],
+    association: dict[str, Any],
     x: Series,
     y: Series = None,
     **params,
-) -> Tuple[bool, Dict[str, Any]]:
+) -> tuple[bool, dict[str, Any]]:
     """Computes outliers based on the inter-quartile range
 
     Parameters
     ----------
     thresh_outlier, float: default 1.
       Maximum percentage of Outliers in a feature
     """
@@ -498,16 +498,16 @@
         # Excluding feature with too frequent modes
         active = pct_iqr < params.get("thresh_outlier", 1.0)
 
     return active, association
 
 
 def chi2_measure(
-    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
-) -> Tuple[bool, Dict[str, Any]]:
+    active: bool, association: dict[str, Any], x: Series, y: Series, **params
+) -> tuple[bool, dict[str, Any]]:
     """Chi2 Measure between two Series of qualitative features"""
 
     # check that previous steps where passed
     if active:
         # computing crosstab between x and y
         xtab = crosstab(x, y)
 
@@ -517,16 +517,16 @@
         # updating association
         association.update({"chi2_measure": chi2})
 
     return active, association
 
 
 def cramerv_measure(
-    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
-) -> Tuple[bool, Dict[str, Any]]:
+    active: bool, association: dict[str, Any], x: Series, y: Series, **params
+) -> tuple[bool, dict[str, Any]]:
     """Carmer's V between two Series of qualitative features"""
 
     # check that previous steps where passed
     if active:
         # computing chi2
         if "chi2_measure" not in association:
             active, association = chi2_measure(active, association, x, y, **params)
@@ -547,16 +547,16 @@
         # updating association
         association.update({"cramerv_measure": cramerv})
 
     return active, association
 
 
 def tschuprowt_measure(
-    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
-) -> Tuple[bool, Dict[str, Any]]:
+    active: bool, association: dict[str, Any], x: Series, y: Series, **params
+) -> tuple[bool, dict[str, Any]]:
     """Tschuprow's T between two Series of qualitative features"""
 
     # check that previous steps where passed
     if active:
         # computing chi2
         if "chi2_measure" not in association:
             active, association = chi2_measure(active, association, x, y, **params)
@@ -579,24 +579,24 @@
         # updating association
         association.update({"tschuprowt_measure": tschuprowt})
 
     return active, association
 
 
 # FILTERS
-def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Filters out missing association measure (did not pass a threshold)"""
 
     # drops rows with nans
     associations = ranks.dropna(axis=0)
 
     return associations
 
 
-def measure_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+def measure_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Filters out specified measure's lower ranks than threshold
 
     Parameters
     ----------
     thresh_measure, float: default 0.
         Minimum association between target and features
         To be used with: `association_filter`
@@ -612,15 +612,15 @@
         associations = ranks[ranks[params.get("name_measure")] > params.get("thresh_measure", 0.0)]
 
     return associations
 
 
 def quantitative_filter(
     X: DataFrame, ranks: DataFrame, corr_measure: str, **params
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """Computes max association between X and X (quantitative) excluding features
     that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
@@ -664,45 +664,45 @@
 
     # applying filter on association
     associations = ranks.join(associations, how="right")
 
     return associations
 
 
-def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Computes max Spearman between X and X (quantitative) excluding features
     that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
       Maximum association between features
     """
 
     # applying quantitative filter with spearman correlation
     return quantitative_filter(X, ranks, "spearman", **params)
 
 
-def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Computes max Pearson between X and X (quantitative) excluding features
     that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
       Maximum association between features
     """
 
     # applying quantitative filter with spearman correlation
     return quantitative_filter(X, ranks, "pearson", **params)
 
 
-def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Computes Variance Inflation Factor (multicolinearity)
 
     Parameters
     ----------
     thresh_vif, float: default inf
       Maximum VIF between features
     """
@@ -796,15 +796,15 @@
             return ranks, None
 
     return ranks, worst_corr
 
 
 def qualitative_filter(
     X: DataFrame, ranks: DataFrame, corr_measure: Callable, **params
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """Computes max association between X and X (qualitative) excluding features
     that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
@@ -831,30 +831,30 @@
 
     # applying filter on association
     associations = ranks.join(associations, how="right")
 
     return associations
 
 
-def cramerv_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+def cramerv_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Computes max Cramer's V between X and X (qualitative) excluding features
     that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
         Maximum association between features
     """
 
     # applying quantitative filter with Cramer's V correlation
     return qualitative_filter(X, ranks, cramerv_measure, **params)
 
 
-def tschuprowt_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+def tschuprowt_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Computes max Tschuprow's T between X and X (qualitative) excluding
      features that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
```

### Comparing `AutoCarver-5.0.8/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.9/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.8
+Version: 5.0.9
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
+Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
```

### Comparing `AutoCarver-5.0.8/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.9/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.8/LICENSE` & `AutoCarver-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.8/PKG-INFO` & `AutoCarver-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.8
+Version: 5.0.9
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
+Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
```

### Comparing `AutoCarver-5.0.8/README.md` & `AutoCarver-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.8/setup.py` & `AutoCarver-5.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from codecs import open
 from os import path
 
-from setuptools import setup,find_packages
+from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.8",
+    version="5.0.9",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
-        "Bug Tracker": "https://github.com/mdefrance/AutoCarver/issues"
+        "Documentation": "https://autocarver.readthedocs.io/en/latest/index.html",
+        "Bug Tracker": "https://github.com/mdefrance/AutoCarver/issues",
     },
     license="MIT",
     install_requires=[
-        'pandas',
-        'numpy',
-        'scipy',
-        'scikit-learn',
-        'statsmodels',
-        'tqdm',
-        'ipython',
+        "pandas",
+        "numpy",
+        "scipy",
+        "scikit-learn",
+        "statsmodels",
+        "tqdm",
+        "ipython",
     ],
     packages=find_packages(),
     classifiers=[
         # ou 4 - Beta ou 5 - Production/Stable
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
```

### Comparing `AutoCarver-5.0.8/tests/test_auto_carver.py` & `AutoCarver-5.0.9/tests/test_auto_carver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Set of tests for auto_carver module.
 
 # TODO: test avec chained_discretizer
 """
 
 from json import dumps, loads
+
 from pandas import DataFrame
 from pytest import fixture, raises
 
 from AutoCarver.auto_carver import AutoCarver, load_carver
 
 
 @fixture(scope="module", params=["float", "str"])
@@ -20,20 +21,29 @@
     return request.param
 
 
 @fixture(scope="module", params=["tschuprowt", "cramerv"])
 def sort_by(request) -> str:
     return request.param
 
+
 @fixture(scope="module", params=[True, False])
 def copy(request) -> bool:
     return request.param
 
+
 def test_auto_carver(
-    x_train: DataFrame, x_dev_1: DataFrame, x_dev_wrong_1: DataFrame, x_dev_wrong_2: DataFrame, output_dtype: str, dropna: bool, sort_by: str, copy: bool
+    x_train: DataFrame,
+    x_dev_1: DataFrame,
+    x_dev_wrong_1: DataFrame,
+    x_dev_wrong_2: DataFrame,
+    output_dtype: str,
+    dropna: bool,
+    sort_by: str,
+    copy: bool,
 ) -> None:
     """Tests AutoCarver
 
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
@@ -161,24 +171,27 @@
     else:
         assert all(
             x_discretized[auto_carver.features].isna().mean() == 0
         ), "Some Nans are not dropped (grouped)"
 
     # testing copy functionnality
     if copy:
-        assert all(x_discretized[auto_carver.features].fillna('__NAN__') == x_train[auto_carver.features].fillna('__NAN__')), "Not copied correctly"
+        assert all(
+            x_discretized[auto_carver.features].fillna("__NAN__")
+            == x_train[auto_carver.features].fillna("__NAN__")
+        ), "Not copied correctly"
 
     # testing json serialization
     json_serialized_auto_carver = dumps(auto_carver.to_json())
     loaded_carver = load_carver(loads(json_serialized_auto_carver))
 
     assert all(
         loaded_carver.summary() == auto_carver.summary()
     ), "Non-identical AutoCarver when loading JSON"
 
     # testing to transform dev set with unexpected modality
     with raises(AssertionError):
         auto_carver.transform(x_dev_wrong_1)
-        
+
     # testing to transform dev set with unexpected nans
     with raises(AssertionError):
         auto_carver.transform(x_dev_wrong_2)
```

### Comparing `AutoCarver-5.0.8/tests/test_base_discretizers.py` & `AutoCarver-5.0.9/tests/test_base_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Set of tests for base_discretizers module."""
 
 from numpy import nan
 from pandas import DataFrame
 
-from AutoCarver.discretizers.utils.base_discretizers import GroupedListDiscretizer
+from AutoCarver.discretizers.utils.base_discretizers import BaseDiscretizer
 from AutoCarver.discretizers.utils.grouped_list import GroupedList
 
+
 # TODO: test quantitative discretization
 def test_grouped_list_discretizer(x_train: DataFrame, x_dev_1: DataFrame, x_dev_2: DataFrame):
-    """Tests GroupedListDiscretizer
+    """Tests BaseDiscretizer
 
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
     x_dev_1 : DataFrame
         Simulated Test DataFrame
@@ -40,15 +41,15 @@
     values_orders = {
         "Qualitative_Ordinal": groupedlist,
         "Qualitative_Ordinal_lownan": groupedlist_lownan,
     }
     features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan"]
 
     # initiating discretizer
-    discretizer = GroupedListDiscretizer(
+    discretizer = BaseDiscretizer(
         features=features,
         values_orders=values_orders,
         str_nan=str_nan,
         input_dtypes="str",
         copy=True,
     )
     x_discretized = discretizer.fit_transform(x_train)
```

### Comparing `AutoCarver-5.0.8/tests/test_discretizers.py` & `AutoCarver-5.0.9/tests/test_discretizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Set of tests for discretizers module."""
 
 from numpy import inf
 from pandas import DataFrame
 
-from AutoCarver.discretizers import discretizers
+from AutoCarver.discretizers import Discretizer, QualitativeDiscretizer, QuantitativeDiscretizer
 
 
 def test_quantitative_discretizer(x_train: DataFrame):
     """Tests QuantitativeDiscretizer
 
     Parameters
     ----------
@@ -20,15 +20,15 @@
         "Discrete_Quantitative",
         "Discrete_Quantitative_highnan",
         "Discrete_Quantitative_lownan",
         "Discrete_Quantitative_rarevalue",
     ]
     min_freq = 0.1
 
-    discretizer = discretizers.QuantitativeDiscretizer(features, min_freq=min_freq)
+    discretizer = QuantitativeDiscretizer(quantitative_features=features, min_freq=min_freq)
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     assert (
         "__NAN__" in discretizer.values_orders["Discrete_Quantitative_lownan"]
     ), "Missing order should not be grouped with ordinal_discretizer"
     assert all(
         x_discretized.Quantitative.value_counts(normalize=True) >= min_freq
@@ -82,17 +82,17 @@
             "High",
             "High+",
         ],
     }
 
     min_freq = 0.1
 
-    discretizer = discretizers.QualitativeDiscretizer(
-        features,
-        min_freq,
+    discretizer = QualitativeDiscretizer(
+        qualitative_features=features,
+        min_freq=min_freq,
         ordinal_features=ordinal_features,
         values_orders=values_orders,
         copy=True,
         verbose=True,
     )
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
@@ -195,15 +195,15 @@
         "Discrete_Qualitative_highnan": ["1", "2", "3", "4", "5", "6", "7"],
     }
 
     # minimum frequency per modality + apply(find_common_modalities) outputs a Series
     min_freq = 0.1
 
     # discretizing features
-    discretizer = discretizers.Discretizer(
+    discretizer = Discretizer(
         quantitative_features=quantitative_features,
         qualitative_features=qualitative_features,
         ordinal_features=ordinal_features,
         values_orders=values_orders,
         min_freq=min_freq,
         copy=True,
     )
```

### Comparing `AutoCarver-5.0.8/tests/test_grouped_list.py` & `AutoCarver-5.0.9/tests/test_grouped_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Set of tests for base_discretizers module."""
 
-from numpy import nan
-from pandas import DataFrame
 from pytest import raises
 
 from AutoCarver.discretizers.utils.grouped_list import GroupedList
 
 
 def test_grouped_list_init():
     """Tests the initialization of a GroupedList"""
```

### Comparing `AutoCarver-5.0.8/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.9/tests/test_qualitative_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Set of tests for qualitative_discretizers module."""
 
 from pandas import DataFrame
 from pytest import raises
 
-from AutoCarver.discretizers.utils.qualitative_discretizers import ChainedDiscretizer, DefaultDiscretizer, OrdinalDiscretizer
 from AutoCarver.discretizers.utils.grouped_list import GroupedList
+from AutoCarver.discretizers.utils.qualitative_discretizers import (
+    ChainedDiscretizer,
+    DefaultDiscretizer,
+    OrdinalDiscretizer,
+)
 
 
 def test_chained_discretizer(x_train: DataFrame) -> None:
     """Tests DefaultDiscretizer
 
     Parameters
     ----------
@@ -48,15 +52,15 @@
         "Worst": ["Lows", "Mediums", "Worst"],
         "Best": ["Highs", "Best"],
     }
 
     min_freq = 0.15
 
     discretizer = ChainedDiscretizer(
-        features=ordinal_features,
+        qualitative_features=ordinal_features,
         chained_orders=[level0_to_level1, level1_to_level2],
         min_freq=min_freq,
         values_orders=values_orders,
         copy=True,
     )
     x_discretized = discretizer.fit_transform(x_train)
 
@@ -148,15 +152,15 @@
             "Worst": ["Lows", "Mediums", "Worst"],
             "Best": ["Highs", "Best"],
         }
 
         min_freq = 0.15
 
         discretizer = ChainedDiscretizer(
-            features=ordinal_features,
+            qualitative_features=ordinal_features,
             chained_orders=[level0_to_level1, level1_to_level2],
             min_freq=min_freq,
             values_orders=values_orders,
             copy=True,
         )
         x_discretized = discretizer.fit_transform(x_train)
 
@@ -196,27 +200,31 @@
     }
 
     features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan"]
 
     min_freq = 0.02
     # unwanted value in values_orders
     with raises(AssertionError):
-        discretizer = DefaultDiscretizer(features, min_freq, values_orders=values_orders, copy=True)
+        discretizer = DefaultDiscretizer(
+            qualitative_features=features, min_freq=min_freq, values_orders=values_orders, copy=True
+        )
         x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     # correct feature ordering
     groupedlist_grouped.group("Category B", "Category D")
     values_orders = {
         "Qualitative_grouped": groupedlist_grouped,
         "Qualitative_highnan": groupedlist_highnan,
         "Qualitative_lownan": groupedlist_lownan,
         "Qualitative_Ordinal": groupedlist_ordinal,
     }
 
-    discretizer = DefaultDiscretizer(features, min_freq, values_orders=values_orders, copy=True)
+    discretizer = DefaultDiscretizer(
+        qualitative_features=features, min_freq=min_freq, values_orders=values_orders, copy=True
+    )
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     assert (
         discretizer.values_orders["Qualitative_Ordinal"].content == groupedlist_ordinal.content
     ), "Column names of values_orders not provided if features should not be discretized."
     quali_expected = {
         "__OTHER__": ["Category A", "__OTHER__"],
@@ -304,15 +312,17 @@
         "Qualitative_Ordinal_lownan": groupedlist_lownan,
     }
 
     # minimum frequency per modality + apply(find_common_modalities) outputs a Series
     min_freq = 0.01
 
     # discretizing features
-    discretizer = OrdinalDiscretizer(features, values_orders, min_freq, copy=True)
+    discretizer = OrdinalDiscretizer(
+        ordinal_features=features, min_freq=min_freq, values_orders=values_orders, copy=True
+    )
     discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     expected_ordinal_01 = {
         "Low-": ["Low", "Low-"],
         "Low+": ["Low+"],
         "Medium-": ["Medium-"],
         "Medium": ["Medium"],
@@ -337,15 +347,17 @@
         == expected_ordinal_lownan_01
     ), "Missing value in order not correctly grouped or introduced nans."
 
     # minimum frequency per modality + apply(find_common_modalities) outputs a DataFrame
     min_freq = 0.08
 
     # discretizing features
-    discretizer = OrdinalDiscretizer(features, values_orders, min_freq, copy=True)
+    discretizer = OrdinalDiscretizer(
+        ordinal_features=features, min_freq=min_freq, values_orders=values_orders, copy=True
+    )
     discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     expected_ordinal_08 = {
         "Low+": ["Low-", "Low", "Low+"],
         "Medium-": ["Medium-"],
         "Medium": ["Medium"],
         "High": ["Medium+", "High-", "High"],
```

### Comparing `AutoCarver-5.0.8/tests/test_quantitative_discretizers.py` & `AutoCarver-5.0.9/tests/test_quantitative_discretizers.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Set of tests for quantitative_discretizers module."""
 
-from pandas import DataFrame
 from numpy import inf
+from pandas import DataFrame
 
 from AutoCarver.discretizers.utils.quantitative_discretizers import QuantileDiscretizer
 
 
 def test_quantile_discretizer(x_train: DataFrame):
     """Tests QuantileDiscretizer
```

### Comparing `AutoCarver-5.0.8/tests/test_type_discretizers.py` & `AutoCarver-5.0.9/tests/test_type_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             "High",
             "High+",
         ],
         "Discrete_Qualitative_highnan": ["1", "2", "3", "4", "5", "6", "7"],
     }
 
     discretizer = StringDiscretizer(
-        features=list(set(ordinal_features + qualitative_features)), values_orders=values_orders
+        qualitative_features=list(set(ordinal_features + qualitative_features)),
+        values_orders=values_orders,
     )
     x_discretized = discretizer.fit_transform(x_train)
 
     expected = {
         "2": [2, "2"],
         "4": [4, "4"],
         "3": [3, "3"],
```

