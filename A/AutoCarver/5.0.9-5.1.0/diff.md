# Comparing `tmp/AutoCarver-5.0.9.tar.gz` & `tmp/AutoCarver-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.9.tar", last modified: Sun Jul 16 01:25:36 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.0.tar", last modified: Sun Jul 16 14:10:56 2023, max compression
```

## Comparing `AutoCarver-5.0.9.tar` & `AutoCarver-5.1.0.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.425522 AutoCarver-5.0.9/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34051 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.429523 AutoCarver-5.0.9/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23378 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34717 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28766 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.429523 AutoCarver-5.0.9/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 01:25:36.000000 AutoCarver-5.0.9/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18904 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 01:25:36.437523 AutoCarver-5.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:25:36.433523 AutoCarver-5.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-16 01:25:17.000000 AutoCarver-5.0.9/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.049478 AutoCarver-5.1.0/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34099 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35075 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29285 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.049478 AutoCarver-5.1.0/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 14:10:56.000000 AutoCarver-5.1.0/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-16 14:10:56.000000 AutoCarver-5.1.0/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 14:10:56.000000 AutoCarver-5.1.0/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 14:10:56.000000 AutoCarver-5.1.0/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 14:10:56.000000 AutoCarver-5.1.0/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:10:56.053478 AutoCarver-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-16 14:10:40.000000 AutoCarver-5.1.0/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.0.9/AutoCarver/auto_carver.py` & `AutoCarver-5.1.0/AutoCarver/auto_carver.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .discretizers.utils.serialization import json_deserialize_values_orders
 
 
 class AutoCarver(BaseDiscretizer):
     """Automatic carving of continuous, discrete, categorical and ordinal
     features that maximizes association with a binary target.
 
-    Applies ``Discretizer``, data should not be given raw.
+    Fits a ``Discretizer``. Raw data should be provided as input (not a result of ``Discretizer.transform()``).
     """
 
     def __init__(
         self,
         quantitative_features: list[str],
         qualitative_features: list[str],
         min_freq: float,
@@ -261,15 +261,15 @@
         self.input_dtypes.update(discretizer.input_dtypes)  # saving data types
 
         # updating values_orders according to base bucketization
         self.values_orders.update(discretizer.values_orders)
 
         # removing dropped features
         for feature in self.features:
-            if feature not in discretizer.values_orders:
+            if feature not in discretizer.features:
                 self._remove_feature(feature)
 
         # converting potential quantiles into there respective labels
         labels_orders = convert_to_labels(
             features=self.features,
             quantitative_features=self.quantitative_features,
             values_orders=self.values_orders,
```

### Comparing `AutoCarver-5.0.9/AutoCarver/converters.py` & `AutoCarver-5.1.0/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.9/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.0/AutoCarver/discretizers/discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,22 @@
             output_dtype="str",
             str_nan=str_nan,
             str_default=str_default,
             copy=copy,
             verbose=verbose,
         )
 
+        # checking for missing orders
+        no_order_provided = [
+            feature for feature in self.ordinal_features if feature not in self.values_orders
+        ]
+        assert (
+            len(no_order_provided) == 0
+        ), f"No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
+
         # class specific attributes
         self.min_freq = min_freq
 
     def _remove_feature(self, feature: str) -> None:
         """Removes a feature from all `feature` attributes
 
         Parameters
@@ -153,15 +161,15 @@
             qualitative_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
             self.values_orders.update(qualitative_discretizer.values_orders)
 
             # removing dropped features
             for feature in self.qualitative_features:
-                if feature not in qualitative_discretizer.values_orders:
+                if feature not in qualitative_discretizer.features:
                     self._remove_feature(feature)
             if self.verbose:  # verbose if requested
                 print("------\n")
 
         # [Quantitative features] Grouping quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
@@ -179,15 +187,15 @@
             quantitative_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
             self.values_orders.update(quantitative_discretizer.values_orders)
 
             # removing dropped features
             for feature in self.quantitative_features:
-                if feature not in quantitative_discretizer.values_orders:
+                if feature not in quantitative_discretizer.features:
                     self._remove_feature(feature)
             if self.verbose:  # verbose if requested
                 print("------\n")
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
@@ -280,14 +288,22 @@
             output_dtype="str",
             str_nan=str_nan,
             str_default=str_default,
             copy=copy,
             verbose=verbose,
         )
 
+        # checking for missing orders
+        no_order_provided = [
+            feature for feature in self.ordinal_features if feature not in self.values_orders
+        ]
+        assert (
+            len(no_order_provided) == 0
+        ), f"No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
+
         # non-ordinal qualitative features
         self.non_ordinal_features = [
             feature for feature in self.qualitative_features if feature not in self.ordinal_features
         ]
 
     def _prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Validates format and content of X and y. Converts non-string columns into strings.
@@ -310,17 +326,15 @@
 
         # checking for ids (unique value per row)
         frequencies = x_copy[self.features].apply(
             lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
             axis=0,
         )
         # for each feature, checking that at least one value is more frequent than min_freq
-        all_features = self.features[
-            :
-        ]  # necessary as features are being removed from self.features
+        all_features = self.features[:]  # features are being removed from self.features
         for feature in all_features:
             if frequencies[feature] < self.min_freq:
                 print(
                     f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than min_freq={self.min_freq:2.1%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
                 )
                 self._remove_feature(feature)
```

### Comparing `AutoCarver-5.0.9/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.0/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,18 +233,20 @@
 
         # for each feature, getting label associated to each value
         self.labels_per_values = self._get_labels_per_values(self.output_dtype)
 
         return self
 
     def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """Applies discretization using a dict of GroupedList to transform a DataFrame's columns whatever there ``input_dtypes``.
+        """Applies discretization to a DataFrame's columns.
 
-        Groups values of features (keys of ``values_orders``) according to there ``GroupedList`` (defined in ``values_orders``) by
-        reading the historized merges inside the ``GroupedList.content`` dict.
+        * For each feature's modality, the associated group label is attributed as definid by ``values_orders``.
+        * If ``output_dtype="float"``, converts labels into floats.
+        * Data types are matched as ``input_dtypes=="str"`` for qualitative features and ``input_dtypes=="float"`` for quantitative ones.
+        * If ``copye=True``, the input DataFrame will be copied.
 
         Parameters
         ----------
         X : DataFrame
             Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
@@ -261,35 +263,38 @@
 
         # transforming quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print(
                     f" - [BaseDiscretizer] Transform Quantitative {str(self.quantitative_features)}"
                 )
-            x_copy = self.transform_quantitative(x_copy, y)
+            x_copy = self._transform_quantitative(x_copy, y)
 
         # transforming qualitative features
         if len(self.qualitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print(
                     f" - [BaseDiscretizer] Transform Qualitative {str(self.qualitative_features)}"
                 )
-            x_copy = self.transform_qualitative(x_copy, y)
+            x_copy = self._transform_qualitative(x_copy, y)
 
         # reinstating nans
         if not self.dropna:
             for feature in self.features:
                 label_per_value = self.labels_per_values[feature]
                 if self.str_nan in label_per_value:  # checking for nans in the feature
                     x_copy[feature] = x_copy[feature].replace(label_per_value[self.str_nan], nan)
 
         return x_copy
 
-    def transform_quantitative(self, X: DataFrame, y: Series) -> DataFrame:
-        """Applies discretization using a dict of GroupedList to transform a DataFrame's Quantitative columns (as defined by ``input_dtypes=="float"``).
+    def _transform_quantitative(self, X: DataFrame, y: Series) -> DataFrame:
+        """Applies discretization to a DataFrame's Quantitative columns.
+
+        * Data types are matched as ``input_dtypes=="str"`` for qualitative features and ``input_dtypes=="float"`` for quantitative ones.
+        * If ``copye=True``, the input DataFrame will be copied.
 
         Parameters
         ----------
         X : DataFrame
             Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
@@ -338,16 +343,19 @@
 
             # converting nans to there value
             if any(nans):
                 X.loc[nans, feature] = self.labels_per_values[feature].get(nan_value, self.str_nan)
 
         return X
 
-    def transform_qualitative(self, X: DataFrame, y: Series = None) -> DataFrame:
-        """Applies discretization using a dict of GroupedList to transform a DataFrame's Qualitative columns (as defined by ``input_dtypes=="str"``).
+    def _transform_qualitative(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """Applies discretization to a DataFrame's Qualitative columns.
+
+        * Data types are matched as ``input_dtypes=="str"`` for qualitative features and ``input_dtypes=="float"`` for quantitative ones.
+        * If ``copye=True``, the input DataFrame will be copied.
 
         Parameters
         ----------
         X : DataFrame
             Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
```

### Comparing `AutoCarver-5.0.9/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.0/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.9/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.0/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,22 @@
             input_dtypes=input_dtypes,
             output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
+        # checking for missong orders
+        no_order_provided = [
+            feature for feature in self.features if feature not in self.values_orders
+        ]
+        assert (
+            len(no_order_provided) == 0
+        ), f"No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
+
         # class specific attributes
         self.min_freq = min_freq
 
     def _prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Validates format and content of X and y.
 
         Parameters
```

### Comparing `AutoCarver-5.0.9/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.0/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.9/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.0/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.9/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.0/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.9/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.0/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.9
+Version: 5.1.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 \n</p>
 <p align="left">
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
-    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
-    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
+    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
+    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
+    <img src="https://github.com/mdefrance/AutoCarver/actions/workflows/pytest.yml/badge.svg">
     <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
 This is a work in progress.
 
 # AutoCarver
```

### Comparing `AutoCarver-5.0.9/LICENSE` & `AutoCarver-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.9/PKG-INFO` & `AutoCarver-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.9
+Version: 5.1.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 \n</p>
 <p align="left">
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
-    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
-    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
+    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
+    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
+    <img src="https://github.com/mdefrance/AutoCarver/actions/workflows/pytest.yml/badge.svg">
     <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
 This is a work in progress.
 
 # AutoCarver
```

### Comparing `AutoCarver-5.0.9/README.md` & `AutoCarver-5.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 </p>
 <p align="left">
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
-    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
-    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
+    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
+    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
+    <img src="https://github.com/mdefrance/AutoCarver/actions/workflows/pytest.yml/badge.svg">
     <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
 This is a work in progress.
 
 # AutoCarver
```

### Comparing `AutoCarver-5.0.9/setup.py` & `AutoCarver-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.9",
+    version="5.1.0",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
@@ -36,12 +36,12 @@
         # ou 4 - Beta ou 5 - Production/Stable
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
-        # "Operating System :: MacOS :: MacOS X",
+        "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     python_requires=">=3.9",
 )
```

### Comparing `AutoCarver-5.0.9/tests/test_auto_carver.py` & `AutoCarver-5.1.0/tests/test_auto_carver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Set of tests for auto_carver module.
-
-# TODO: test avec chained_discretizer
 """
 
 from json import dumps, loads
 
 from pandas import DataFrame
 from pytest import fixture, raises
 
-from AutoCarver.auto_carver import AutoCarver, load_carver
+from AutoCarver import AutoCarver, load_carver
+from AutoCarver.discretizers import ChainedDiscretizer
 
 
 @fixture(scope="module", params=["float", "str"])
 def output_dtype(request) -> str:
     return request.param
 
 
@@ -58,14 +57,18 @@
     dropna : bool
         Whether or note to drop nans
     sort_by : str
         Sorting measure 'tschuprowt' or 'cramerv'
     copy : bool
         Whether or not to copy the input dataset
     """
+    # copying x_train for comparison purposes
+    raw_x_train = x_train.copy()
+
+    # list of feaures
     quantitative_features = [
         "Quantitative",
         "Discrete_Quantitative_highnan",
         "Discrete_Quantitative_lownan",
         "Discrete_Quantitative",
         "Discrete_Quantitative_rarevalue",
         "one",
@@ -109,22 +112,42 @@
             "Medium+",
             "High-",
             "High",
             "High+",
         ],
         "Discrete_Qualitative_highnan": ["1", "2", "3", "4", "5", "6", "7"],
     }
+    chained_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan"]
+
+    level0_to_level1 = {
+        "Lows": ["Low-", "Low", "Low+", "Lows"],
+        "Mediums": ["Medium-", "Medium", "Medium+", "Mediums"],
+        "Highs": ["High-", "High", "High+", "Highs"],
+    }
+    level1_to_level2 = {
+        "Worst": ["Lows", "Mediums", "Worst"],
+        "Best": ["Highs", "Best"],
+    }
+
+    min_freq = 0.15
+
+    chained_discretizer = ChainedDiscretizer(
+        qualitative_features=chained_features,
+        chained_orders=[level0_to_level1, level1_to_level2],
+        min_freq=min_freq,
+        values_orders=values_orders,
+        copy=copy,
+    )
+    x_discretized = chained_discretizer.fit_transform(x_train)
+    values_orders.update(chained_discretizer.values_orders)
 
     # minimum frequency per modality
     min_freq = 0.06
     max_n_mod = 4
 
-    # copying x_train for comparison purposes
-    raw_x_train = x_train.copy()
-
     # tests with 'tschuprowt' measure
     auto_carver = AutoCarver(
         quantitative_features=quantitative_features,
         qualitative_features=qualitative_features,
         ordinal_features=ordinal_features,
         values_orders=values_orders,
         min_freq=min_freq,
```

