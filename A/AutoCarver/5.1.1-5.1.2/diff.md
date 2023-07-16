# Comparing `tmp/AutoCarver-5.1.1.tar.gz` & `tmp/AutoCarver-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.1.tar", last modified: Sun Jul 16 15:41:14 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.2.tar", last modified: Sun Jul 16 21:50:57 2023, max compression
```

## Comparing `AutoCarver-5.1.1.tar` & `AutoCarver-5.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.700730 AutoCarver-5.1.1/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34144 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    29468 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 15:41:14.000000 AutoCarver-5.1.1/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-16 15:41:14.000000 AutoCarver-5.1.1/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:41:14.000000 AutoCarver-5.1.1/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 15:41:14.000000 AutoCarver-5.1.1/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 15:41:14.000000 AutoCarver-5.1.1/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 15:41:14.708730 AutoCarver-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:41:14.704730 AutoCarver-5.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-16 15:41:01.000000 AutoCarver-5.1.1/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34702 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.1/AutoCarver/auto_carver.py` & `AutoCarver-5.1.2/AutoCarver/auto_carver.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     features that maximizes association with a binary target.
 
     First fits a :ref:`Discretizer`. Raw data should be provided as input (not a result of ``Discretizer.transform()``).
     """
 
     def __init__(
         self,
-        quantitative_features: list[str],
-        qualitative_features: list[str],
         min_freq: float,
         *,
+        quantitative_features: list[str] = None,
+        qualitative_features: list[str] = None,
         ordinal_features: list[str] = None,
         values_orders: dict[str, GroupedList] = None,
         max_n_mod: int = 5,
         # min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
         sort_by: str = "tschuprowt",
         output_dtype: str = "float",
         dropna: bool = True,
@@ -46,29 +46,29 @@
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
     ) -> None:
         """Initiates an ``AutoCarver``.
 
         Parameters
         ----------
-        quantitative_features : list[str]
-            List of column names of quantitative features (continuous and discrete) to be carved
-
-        qualitative_features : list[str]
-            List of column names of qualitative features (non-ordinal) to be carved
-
         min_freq : float
             Minimum frequency per grouped modalities.
 
             * Features whose most frequent modality is less frequent than ``min_freq`` will not be carved.
             * Sets the number of quantiles in which to discretize the continuous features.
             * Sets the minimum frequency of a quantitative feature's modality.
 
             **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
 
+        quantitative_features : list[str]
+            List of column names of quantitative features (continuous and discrete) to be carved, by default ``None``
+
+        qualitative_features : list[str]
+            List of column names of qualitative features (non-ordinal) to be carved, by default ``None``
+
         ordinal_features : list[str], optional
             List of column names of ordinal features to be carved. For those features a list of
             values has to be provided in the ``values_orders`` dict, by default ``None``
 
         values_orders : dict[str, GroupedList], optional
             Dict of feature's column names and there associated ordering.
             If lists are passed, a GroupedList will automatically be initiated, by default ``None``
@@ -120,29 +120,28 @@
             String representation for default qualitative values, i.e. values less frequent than ``min_freq``, by default ``"__OTHER__"``
 
         Examples
         --------
         See `AutoCarver examples <https://autocarver.readthedocs.io/en/latest/index.html>`_
         """
         # Lists of features
+        if quantitative_features is None:
+            quantitative_features = []
+        if qualitative_features is None:
+            qualitative_features = []
         if ordinal_features is None:
             ordinal_features = []
+        assert (
+            len(quantitative_features) > 0
+            or len(qualitative_features) > 0
+            or len(ordinal_features) > 0
+        ), "No feature passed as input. Pleased provided column names to Carver by setting quantitative_features, quantitative_features or ordinal_features."
         self.ordinal_features = list(set(ordinal_features))
         self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
 
-        # checking that qualitatitve and quantitative featues are distinct
-        assert all(
-            quali_feature not in quantitative_features
-            for quali_feature in qualitative_features + ordinal_features
-        ), "A feature of `quantitative_features` also is in `qualitative_features` or `ordinal_features`. Be carreful with your inputs!"
-        assert all(
-            quanti_feature not in qualitative_features + ordinal_features
-            for quanti_feature in quantitative_features
-        ), "A feature of `qualitative_features` or `ordinal_features` also is in `quantitative_features`. Be carreful with your inputs!"
-
         # initializing input_dtypes
         self.input_dtypes = {feature: "str" for feature in qualitative_features + ordinal_features}
         self.input_dtypes.update({feature: "float" for feature in quantitative_features})
 
         # Initiating BaseDiscretizer
         super().__init__(
             features=self.features,
@@ -152,14 +151,24 @@
             str_nan=str_nan,
             str_default=str_default,
             dropna=dropna,
             copy=copy,
             verbose=bool(max(verbose, pretty_print)),
         )
 
+        # checking that qualitatitve and qualitative featues are distinct
+        assert all(
+            quali_feature not in self.quantitative_features
+            for quali_feature in self.qualitative_features
+        ), "A feature of quantitative_features also is in qualitative_features or ordinal_features. Please, be carreful with your inputs!"
+        assert all(
+            quanti_feature not in self.qualitative_features
+            for quanti_feature in self.quantitative_features
+        ), "A feature of qualitative_features or ordinal_features also is in quantitative_features. Please, be carreful with your inputs!"
+
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
         # self.min_carved_freq = min_carved_freq
         self.min_group_size = 1
         self.pretty_print = pretty_print
         measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
@@ -260,17 +269,19 @@
             x_dev_copy = discretizer.transform(x_dev_copy, y_dev)
         self.input_dtypes.update(discretizer.input_dtypes)  # saving data types
 
         # updating values_orders according to base bucketization
         self.values_orders.update(discretizer.values_orders)
 
         # removing dropped features
-        for feature in self.features:
-            if feature not in discretizer.features:
-                self._remove_feature(feature)
+        removed_features = [
+            feature for feature in self.features if feature not in discretizer.features
+        ]
+        for feature in removed_features:
+            self._remove_feature(feature)
 
         # converting potential quantiles into there respective labels
         labels_orders = convert_to_labels(
             features=self.features,
             quantitative_features=self.quantitative_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
@@ -278,50 +289,48 @@
         )
 
         # computing crosstabs for each feature on train/test
         xtabs = get_xtabs(self.features, x_copy, y, labels_orders)
         xtabs_dev = get_xtabs(self.features, x_dev_copy, y_dev, labels_orders)
 
         # optimal butcketization/carving of each feature
-        all_features = self.features[
-            :
-        ]  # necessary as features are being removed from self.features
+        all_features = self.features[:]  # (features are being removed from self.features)
         for n, feature in enumerate(all_features):
             if self.verbose:  # verbose if requested
                 print(f"\n------\n[AutoCarver] Fit {feature} ({n+1}/{len(all_features)})\n---")
 
             # getting xtabs on train/test
             xtab = xtabs[feature]
             xtab_dev = xtabs_dev[feature]
             if self.verbose:  # verbose if requested
-                print("\n - Raw feature distribution")
+                print("\n - [AutoCarver] Raw feature distribution")
                 print_xtabs(xtab, xtab_dev, pretty_print=self.pretty_print)
 
             # ordering
             order = labels_orders[feature]
 
             # getting best combination
             best_combination = self._get_best_combination(order, xtab, xtab_dev=xtab_dev)
 
             # checking that a suitable combination has been found
             if best_combination is not None:
                 order, xtab, xtab_dev = best_combination
                 if self.verbose:  # verbose if requested
-                    print("\n - Carved feature distribution")
+                    print("\n - [AutoCarver] Carved feature distribution")
                     print_xtabs(
                         xtab, xtab_dev, pretty_print=self.pretty_print
                     )  # TODO get the good labels
 
                 # updating label_orders
                 labels_orders.update({feature: order})
 
             # no suitable combination has been found -> removing feature
             else:
                 print(
-                    f"No robust combination for feature '{feature}' could be found. It will be ignored. You might have to increase the size of your test sample (test sample not representative of test sample for this feature) or you should consider dropping this features."
+                    f" - [AutoCarver] No robust combination for feature '{feature}' could be found. It will be ignored. You might have to increase the size of your test sample (test sample not representative of test sample for this feature) or you should consider dropping this features."
                 )
                 self._remove_feature(feature)
                 if feature in labels_orders:
                     labels_orders.pop(feature)
 
             if self.verbose:  # verbose if requested
                 print("------\n")
@@ -501,15 +510,15 @@
     if X is not None:
         # crosstab for each feature
         for feature in features:
             # computing crosstab with str_nan
             xtab = crosstab(X[feature], y)
 
             # reordering according to known_order
-            xtab = xtab.reindex(labels_orders[feature])  # TODO: fill nans for x_dev?
+            xtab = xtab.reindex(labels_orders[feature])
 
             # storing results
             xtabs.update({feature: xtab})
 
     return xtabs
```

### Comparing `AutoCarver-5.1.1/AutoCarver/converters/converters.py` & `AutoCarver-5.1.2/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.2/AutoCarver/discretizers/discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,17 +160,22 @@
             )
             qualitative_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
             self.values_orders.update(qualitative_discretizer.values_orders)
 
             # removing dropped features
-            for feature in self.qualitative_features:
-                if feature not in qualitative_discretizer.features:
-                    self._remove_feature(feature)
+            removed_features = [
+                feature
+                for feature in self.qualitative_features
+                if feature not in qualitative_discretizer.features
+            ]
+            for feature in removed_features:
+                self._remove_feature(feature)
+
             if self.verbose:  # verbose if requested
                 print("------\n")
 
         # [Quantitative features] Grouping quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print("------\n[Discretizer] Fit Quantitative Features\n---")
@@ -186,17 +191,22 @@
             )
             quantitative_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
             self.values_orders.update(quantitative_discretizer.values_orders)
 
             # removing dropped features
-            for feature in self.quantitative_features:
-                if feature not in quantitative_discretizer.features:
-                    self._remove_feature(feature)
+            removed_features = [
+                feature
+                for feature in self.quantitative_features
+                if feature not in quantitative_discretizer.features
+            ]
+            for feature in removed_features:
+                self._remove_feature(feature)
+
             if self.verbose:  # verbose if requested
                 print("------\n")
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
@@ -321,24 +331,24 @@
         DataFrame
             A formatted copy of X
         """
         # checking for binary target, copying X
         x_copy = super()._prepare_data(X, y)
 
         # checking for ids (unique value per row)
-        frequencies = x_copy[self.features].apply(
+        max_frequencies = x_copy[self.features].apply(
             lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
             axis=0,
         )
         # for each feature, checking that at least one value is more frequent than min_freq
         all_features = self.features[:]  # features are being removed from self.features
         for feature in all_features:
-            if frequencies[feature] < self.min_freq:
+            if max_frequencies[feature] < self.min_freq:
                 print(
-                    f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than min_freq={self.min_freq:2.1%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
+                    f" - [QualitatitveDiscretizer] For feature '{feature}', the largest modality has {max_frequencies[feature]:2.2%} observations which is lower than min_freq={self.min_freq:2.1%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
                 )
                 self._remove_feature(feature)
 
         # checking for columns containing floats or integers even with filled nans
         dtypes = x_copy[self.features].fillna(self.str_nan).applymap(type).apply(unique)
         not_object = dtypes.apply(lambda u: any(typ != str for typ in u))
 
@@ -346,15 +356,15 @@
         if any(not_object):
             features_to_convert = list(not_object.index[not_object])
             if self.verbose:
                 unexpected_dtypes = [
                     typ for dtyp in dtypes[not_object] for typ in dtyp if typ != str
                 ]
                 print(
-                    f"""Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
+                    f""" - [QualitatitveDiscretizer] Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
                 )
 
             # converting specified features into qualitative features
             string_discretizer = StringDiscretizer(
                 qualitative_features=features_to_convert,
                 values_orders=self.values_orders,
                 verbose=self.verbose,
```

### Comparing `AutoCarver-5.1.1/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.2/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.2/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.2/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,39 +492,40 @@
         DataFrame
             A formatted copy of X
         """
         # copying dataframe
         x_copy = X.copy()
 
         # checking for ids (unique value per row)
-        frequencies = x_copy[self.features].apply(
+        max_frequencies = x_copy[self.features].apply(
             lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
             axis=0,
         )
         # for each feature, checking that at least one value is more frequent than min_freq
-        for feature in self.features:
-            if frequencies[feature] < self.min_freq:
+        all_features = self.features[:]
+        for feature in all_features:
+            if max_frequencies[feature] < self.min_freq:
                 print(
-                    f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than {self.min_freq:2.2%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
+                    f" - [ChainedDiscretizer] For feature '{feature}', the largest modality has {max_frequencies[feature]:2.2%} observations which is lower than {self.min_freq:2.2%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
                 )
-                self._remove_feature(feature)
+                super()._remove_feature(feature)
 
         # checking for columns containing floats or integers even with filled nans
         dtypes = x_copy[self.features].fillna(self.str_nan).applymap(type).apply(unique)
         not_object = dtypes.apply(lambda u: any(typ != str for typ in u))
 
         # non qualitative features detected
         if any(not_object):
             features_to_convert = list(not_object.index[not_object])
             if self.verbose:
                 unexpected_dtypes = [
                     typ for dtyp in dtypes[not_object] for typ in dtyp if typ != str
                 ]
                 print(
-                    f"""Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
+                    f""" - [ChainedDiscretizer] Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
                 )
 
             # converting specified features into qualitative features
             stringer = StringDiscretizer(
                 qualitative_features=features_to_convert, values_orders=self.values_orders
             )
             x_copy = stringer.fit_transform(x_copy)
@@ -577,15 +578,15 @@
                 if value not in self.known_values and value != self.str_nan
             ]
 
             # converting unknown values to NaN
             if self.remove_unknown & (len(missing) > 0):
                 # alerting user
                 print(
-                    f"Order for feature '{feature}' was not provided for values:  {str(missing)}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)"
+                    f" - [ChainedDiscretizer] Order for feature '{feature}' was not provided for values:  {str(missing)}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)"
                 )
 
                 # adding missing values to the order
                 order.update({self.str_nan: missing + order.get(self.str_nan)})
 
             # alerting user
             else:
```

### Comparing `AutoCarver-5.1.1/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.2/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.2/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.2/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.2/AutoCarver/feature_selection/feature_selector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Tools to select the best Quantitative and Qualitative features."""
 
 from random import shuffle
 from typing import Any, Callable
 
 from IPython.display import display_html
 from pandas import DataFrame, Series
-from sklearn.base import BaseEstimator, TransformerMixin
 
-from ..discretizers import GroupedList
-from .filters import thresh_filter
-from .measures import dtype_measure, mode_measure, nans_measure
+from .filters import cramerv_filter, spearman_filter, thresh_filter
+from .measures import cramerv_measure, dtype_measure, kruskal_measure, mode_measure, nans_measure
 
 
-# TODO: convert to groupedlistdiscretizer
+# TODO: add thresh_mode, thresh_nan to the class parameters
 # TODO: add parameter to shut down displayed info
-class FeatureSelector(BaseEstimator, TransformerMixin):
+class FeatureSelector:
     """A pipeline of measures to perform EDA and feature pre-selection
 
      - best features are the n_best of each measure
      - selected features are stored in FeatureSelector.best_features
 
     Parameters
     ----------
@@ -77,26 +75,26 @@
         According to this measure:
          - True: Lower values of the measure are to be considered as more associated to the target
          - False: Higher values of the measure are to be considered as more associated to the target
     """
 
     def __init__(
         self,
-        features: list[str],
         n_best: int,
-        measures: list[Callable],
         *,
+        quantitative_features: list[str] = None,
+        qualitative_features: list[str] = None,
+        measures: list[Callable] = None,
         filters: list[Callable] = None,
         sample_size: float = 1.0,
-        copy: bool = True,
-        drop: bool = False,  # TODO
-        verbose: bool = True,
+        verbose: bool = False,
+        pretty_print: bool = False,  # TODO
         **params,
     ) -> None:
-        """_summary_
+        """Initiates a ``FeatureSelector``.
 
         Parameters
         ----------
         features : list[str]
             _description_
         n_best : int
             _description_
@@ -107,142 +105,163 @@
         sample_size : float, optional
             _description_, by default 1.0
         copy : bool, optional
             _description_, by default True
         verbose : bool, optional
             _description_, by default True
         """
-        print("Warning: not fully optimized for package versions greater than 4.")
+        # settinp up list of features
+        if quantitative_features is None:
+            quantitative_features = []
+        if qualitative_features is None:
+            qualitative_features = []
+        assert (
+            len(quantitative_features) > 0 or len(qualitative_features) > 0
+        ), "No feature passed as input. Pleased provided column names to Carver by setting qualitative_features or quantitative_features."
+        assert (len(quantitative_features) > 0 and len(qualitative_features) == 0) or (
+            len(qualitative_features) > 0 and len(quantitative_features) == 0
+        ), "Mixed quantitative and qualitative features. One only of quantitative_features and qualitative_features should be set."
+        self.features = list(set(qualitative_features + quantitative_features))
 
-        self.features = list(set(features))
+        # number of features selected
         self.n_best = n_best
-        assert n_best <= len(features), "Must set n_best <= len(features)"
-        self.best_features = features[:]
+        assert n_best <= len(self.features) + 1, "Must set n_best <= len(features)"
+
+        # feature sample size per iteration
         self.sample_size = sample_size
 
+        # initiating measures
+        if measures is None:
+            if any(quantitative_features):  # quantitative feature association measure
+                measures = [kruskal_measure]
+            else:  # qualitative feature association measure
+                measures = [cramerv_measure]
         self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
+
+        # initiating filters
         if filters is None:
-            filters = []
+            if any(quantitative_features):  # quantitative feature association measure
+                filters = [spearman_filter]
+            else:  # qualitative feature association measure
+                filters = [cramerv_filter]
         self.filters = [thresh_filter] + filters[:]
-        self.sort_measures = [measure.__name__ for measure in measures[::-1]]
 
-        # Values_orders from GroupedListDiscretizer
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {
-            feature: GroupedList(value) for feature, value in values_orders.items()
-        }
-
-        self.drop = drop
-        self.copy = copy
-        self.verbose = verbose
+        # names of measures to sort by
+        self.measure_names = [measure.__name__ for measure in measures[::-1]]
+
+        # wether or not to print tables
+        self.verbose = bool(max(verbose, pretty_print))
+        self.pretty_print = pretty_print
+
+        # keyword arguments
         self.params = params
 
         self.associations = None
         self.filtered_associations = None
 
-    def measure(self, x: Series, y: Series) -> dict[str, Any]:
-        """Measures association between x and y"""
-
-        passed = True  # measures keep going only if previous basic tests are passed
-        association = {}
-
-        # iterating over each measure
-        for measure in self.measures:
-            passed, association = measure(passed, association, x, y, **self.params)
-
-        return association
-
-    def measure_apply(self, X: DataFrame, y: Series, features: list[str]) -> None:
-        """Measures association between columns of X and y
+    def _select_features(
+        self, X: DataFrame, y: Series, features: list[str], n_best: int
+    ) -> list[str]:
+        """Selects the n_best features amongst the specified ones
 
         Parameters
         ----------
-        ascending, bool default False
-            According to this measure:
-             - True: Lower values of the measure are to be considered as more associated to the target
-             - False: Higher values of the measure are to be considered as more associated to the target
-        """
+        X : DataFrame
+            _description_
+        y : Series
+            _description_
+        features : list[str]
+            _description_
+        n_best : int
+            _description_
 
-        # applying association measure to each column
-        self.associations = X[features].apply(self.measure, y=y, result_type="expand", axis=0).T
+        Returns
+        -------
+        list[str]
+            _description_
+        """
+        if self.verbose:  # verbose if requested
+            print(f"------\n[FeatureSelector] Selecting from Features: {str(features)}\n---")
 
-        # filtering non association measure (pct_zscore, pct_iqr...)
-        asso_measures = [c for c in self.associations if "_measure" in c]
-        self.sort_measures = [c for c in self.sort_measures if c in asso_measures]
-
-        # sorting statistics if an association measure was provided
-        self.associations = self.associations.sort_values(
-            self.sort_measures, ascending=self.params.get("ascending", False)
+        # Computes association between X and y
+        initial_associations = apply_measures(
+            X, y, measures=self.measures, features=features, **self.params
         )
 
-    def filter_apply(self, X: DataFrame, sort_measure: str) -> DataFrame:
-        """Filters out too correlated features (least relevant first)
+        # sorting statistics
+        measure_names = evaluated_measure_names(initial_associations, self.measure_names)
+        initial_associations = initial_associations.sort_values(
+            measure_names, ascending=self.params.get("ascending", False)
+        )
 
-        Parameters
-        ----------
-        ascending, bool default False
-            According to this measure:
-             - True: Lower values of the measure are to be considered as more associated to the target
-             - False: Higher values of the measure are to be considered as more associated to the target
-        """
+        if self.verbose:  # displaying association measure
+            print("\n - Association between X and y")
+            print_associations(initial_associations, self.pretty_print)
+
+        # applying filtering for each measure
+        all_best_features: dict[str, Any] = {}
+        for measure_name in measure_names:
+            # sorting association for each measure
+            associations = initial_associations.sort_values(
+                measure_name, ascending=self.params.get("ascending", False)
+            )
+
+            # filtering for each measure, as each measure ranks the features differently
+            filtered_association = apply_filters(
+                X, associations, filters=self.filters, **self.params
+            )
+
+            # selected features for the measure
+            selected_features = [
+                feature
+                for feature in initial_associations.index
+                if feature in filtered_association.index[:n_best]
+            ]
 
-        # ordering features by sort_by
-        self.filtered_associations = self.associations.sort_values(
-            sort_measure, ascending=self.params.get("ascending", False)
-        )
+            # saving results
+            all_best_features.update(
+                {
+                    measure_name: {
+                        "selected": selected_features,
+                        "association": filtered_association,
+                    }
+                }
+            )
+
+        # list of unique best_featues per measure_name
+        best_features = [
+            # ordering according target association
+            feature
+            for feature in initial_associations.index
+            # checking that feature has been selected by a measure
+            if any(feature in all_best_features[measure]["selected"] for measure in measure_names)
+        ]
 
-        # applying successive filters
-        for filtering in self.filters:
-            # ordered filtering
-            self.filtered_associations = filtering(X, self.filtered_associations, **self.params)
-
-    def display_stats(self, association: DataFrame, caption: str) -> None:
-        """EDA of fitted associations"""
-
-        # appllying style
-        subset = [c for c in association if "pct_" in c or "_measure" in c or "_filter" in c]
-        style = association.style.background_gradient(cmap="coolwarm", subset=subset)
-        style = style.set_table_attributes("style='display:inline'")
-        style = style.set_caption(caption)
-        display_html(style._repr_html_(), raw=True)
-
-    def fit_features(self, X: DataFrame, y: Series, features: list[str], n_best: int) -> list[str]:
-        """Selects the n_best features amongst the specified ones"""
-
-        # initial computation of all association measures
-        self.measure_apply(X, y, features)
-
-        # displaying association measure
-        if self.verbose:
-            self.display_stats(self.associations, "Raw association")
-
-        # iterating over each sort_measures
-        # useful when measures hints to specific associations
-        ranks = []
-        for n, sort_measure in enumerate(self.sort_measures):
-            # filtering by sort_measure
-            self.filter_apply(X, sort_measure)
-            ranks += [list(self.filtered_associations.index)]
-
-            # displaying filtered out association measure
-            if n == 0 and self.verbose and len(self.filters) > 1:
-                self.display_stats(self.filtered_associations, "Filtered association")
-
-        # retrieving the n_best features per each ranking
-        best_features = []
-        if len(self.sort_measures) > 0:
-            best_features = [feature for rank in ranks for feature in rank[:n_best]]
-            best_features = list(set(best_features))  # deduplicating
+        if self.verbose:  # displaying association measure
+            print("\n - Association between X and y, filtered for inter-feature assocation")
+            print_associations(initial_associations.reindex(best_features), self.pretty_print)
+            print("------\n")
 
         return best_features
 
-    def fit(self, X: DataFrame, y: Series) -> None:
-        """Selects the n_best features"""
+    def select(self, X: DataFrame, y: Series) -> list[str]:
+        """Selects the ``n_best`` features of the DataFrame, by association with the binary target
 
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series
+            Binary target feature with wich the association is maximized.
+
+        Returns
+        -------
+        list[str]
+            List of selected features
+        """
         # splitting features in chunks
         if self.sample_size < 1:
             # shuffling features to get random samples of features
             shuffle(self.features)
 
             # number of features per sample
             chunks = int(len(self.features) // (1 / self.sample_size))
@@ -256,46 +275,167 @@
             # adding last sample with all remaining features
             feature_samples += [self.features[chunks * (int(1 / self.sample_size) - 1) :]]
 
             # iterating over each feature samples
             best_features = []
             for features in feature_samples:
                 # fitting association on features
-                best_features += self.fit_features(X, y, features, int(self.n_best // 2))
+                best_features += self._select_features(X, y, features, int(self.n_best // 2))
 
         # splitting in chunks not requested
         else:
             best_features = self.features[:]
 
         # final selection with all best_features selected
-        self.best_features = self.fit_features(X, y, best_features, self.n_best)
+        best_features = self._select_features(X, y, best_features, self.n_best)
+
+        return best_features
+
+
+def print_associations(association: DataFrame, pretty_print: bool = False) -> None:
+    """EDA of fitted associations
 
-        # ordering best_features according to their rank
-        self.best_features = [
-            f for f in self.filtered_associations.index if f in self.best_features
+    Parameters
+    ----------
+    association : DataFrame
+        _description_
+    pretty_print : bool, optional
+        _description_, by default False
+    """
+    # printing raw DataFrame
+    if not pretty_print:
+        print(association)
+
+    # adding colors and displaying DataFrame as html
+    else:
+        # finding columns with indicators to colorize
+        subset = [
+            column
+            for column in association
+            # checking for an association indicator
+            if any(indic in column for indic in ["pct_", "_measure", "_filter"])
         ]
+        # getting prettier association table
+        nicer_association = association.style.background_gradient(cmap="coolwarm", subset=subset)
+        nicer_association = nicer_association.set_table_attributes("style='display:inline'")
 
-        # removing feature from values_orders
-        dropped_features = [f for f in self.associations.index if f not in self.best_features]
-        for feature in dropped_features:
-            if feature in self.values_orders:
-                self.values_orders.pop(feature)
+        # displaying html of colored DataFrame
+        display_html(nicer_association._repr_html_(), raw=True)
 
-        return self
 
-    def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """Drops the non-selected columns from `features`.
+def feature_association(x: Series, y: Series, measures: list[Callable], **params) -> dict[str, Any]:
+    """Measures association between x and y
 
-        Parameters
-        ----------
-        X : DataFrame
-            Contains columns named in `features`
-        y : Series, optional
-            Model target, by default None
+    Parameters
+    ----------
+    x : Series
+        Sample of a feature.
+    y : Series
+        Binary target feature with wich the association is evaluated.
+
+    Returns
+    -------
+    dict[str, Any]
+        Association metrics' values
+    """
+    # measures keep going only if previous basic tests are passed
+    passed = True
+    association = {}
 
-        Returns
-        -------
-        DataFrame
-            `X` without non-selected columns from `features`.
-        """
+    # iterating over each measure
+    for measure in measures:
+        passed, association = measure(passed, association, x, y, **params)
+
+    return association
+
+
+def apply_measures(
+    X: DataFrame, y: Series, measures: list[Callable], features: list[str], **params
+) -> DataFrame:
+    """Measures association between columns of X and y
+
+    Parameters
+    ----------
+    X : DataFrame
+        _description_
+    y : Series
+        _description_
+    features : list[str]
+        _description_
+    measure_names : list[str]
+        _description_
+    ascending, bool default False
+        According to this measure:
+            - True: Lower values of the measure are to be considered as more associated to the target
+            - False: Higher values of the measure are to be considered as more associated to the target
+
+    Returns
+    -------
+    DataFrame
+        _description_
+    """
+    # applying association measure to each column
+    associations = (
+        X[features]
+        .apply(feature_association, y=y, measures=measures, **params, result_type="expand", axis=0)
+        .T
+    )
+
+    return associations
+
+
+def evaluated_measure_names(associations: DataFrame, measure_names: list[str]) -> list[str]:
+    """_summary_
+
+    Parameters
+    ----------
+    associations : DataFrame
+        _description_
+    measure_names : list[str]
+        _description_
+
+    Returns
+    -------
+    list[str]
+        _description_
+    """
+    # Getting evaluated measures (filtering out non-measures: pct_zscore, pct_iqr...)
+    sort_by = [
+        measure_name
+        for measure_name in measure_names
+        if measure_name in associations and "_measure" in measure_name
+    ]
+
+    return sort_by
+
+
+def apply_filters(
+    X: DataFrame, associations: DataFrame, filters: list[Callable], **params
+) -> DataFrame:
+    """Filters out too correlated features (least relevant first)
+
+    Parameters
+    ----------
+    X : DataFrame
+        _description_
+    associations : DataFrame
+        _description_
+    filters : list[Callable]
+        _description_
+    measure_name : str
+        _description_
+    ascending, bool default False
+        According to this measure:
+            - True: Lower values of the measure are to be considered as more associated to the target
+            - False: Higher values of the measure are to be considered as more associated to the target
+
+    Returns
+    -------
+    DataFrame
+        _description_
+    """
+    # applying successive filters
+    filtered_associations = associations.copy()
+    for filtering in filters:
+        filtered_associations = filtering(X, filtered_associations, **params)
 
-        return X
+    return filtered_associations
```

### Comparing `AutoCarver-5.1.1/AutoCarver/feature_selection/filters/base_filters.py` & `AutoCarver-5.1.2/AutoCarver/feature_selection/filters/base_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.1.2/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.2/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.2/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,15 +25,20 @@
         nans = x.isnull()  # ckecking for nans
         pct_nan = nans.mean()  # Computing percentage of nans
 
         # updating association
         association.update({"pct_nan": pct_nan})
 
         # Excluding feature that have to many NaNs
-        active = pct_nan < params.get("thresh_nan", 1.0)
+        thresh_nan = params.get("thresh_nan", 0.999)
+        active = pct_nan < thresh_nan
+        if not active:
+            print(
+                f"Feature {x.name} will be discarded (more than {thresh_nan:2.2%} of nans). Otherwise, set a greater value for thresh_nan."
+            )
 
     return active, association
 
 
 def dtype_measure(
     active: bool,
     association: dict[str, Any],
@@ -69,10 +74,15 @@
         mode = x.mode(dropna=True).values[0]  # computing mode
         pct_mode = (x == mode).mean()  # Computing percentage of the mode
 
         # updating association
         association.update({"pct_mode": pct_mode, "mode": mode})
 
         # Excluding feature with too frequent modes
-        active = pct_mode < params.get("thresh_mode", 1.0)
+        thresh_mode = params.get("thresh_mode", 0.999)
+        active = pct_mode < thresh_mode
+        if not active:
+            print(
+                f"Feature {x.name} will be discarded (more than {thresh_mode:2.2%} of its mode). Otherwise, set a greater value for thresh_mode."
+            )
 
     return active, association
```

### Comparing `AutoCarver-5.1.1/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.1.2/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.1.2/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.2/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.1
+Version: 5.1.2
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
```

### Comparing `AutoCarver-5.1.1/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.2/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/LICENSE` & `AutoCarver-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/PKG-INFO` & `AutoCarver-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.1
+Version: 5.1.2
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
```

### Comparing `AutoCarver-5.1.1/README.md` & `AutoCarver-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.1/setup.py` & `AutoCarver-5.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.1",
+    version="5.1.2",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.1.1/tests/test_auto_carver.py` & `AutoCarver-5.1.2/tests/test_auto_carver.py`

 * *Files identical despite different names*

