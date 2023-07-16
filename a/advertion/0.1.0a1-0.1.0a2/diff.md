# Comparing `tmp/advertion-0.1.0a1.tar.gz` & `tmp/advertion-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advertion-0.1.0a1.tar", max compression
+gzip compressed data, was "advertion-0.1.0a2.tar", max compression
```

## Comparing `advertion-0.1.0a1.tar` & `advertion-0.1.0a2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1321 2023-07-16 08:51:42.125751 advertion-0.1.0a1/README.md
--rw-r--r--   0        0        0       98 2023-07-16 08:51:42.125751 advertion-0.1.0a1/advertion/__init__.py
--rw-r--r--   0        0        0     5480 2023-07-16 08:51:42.125751 advertion-0.1.0a1/advertion/core.py
--rw-r--r--   0        0        0     1555 2023-07-16 08:51:42.125751 advertion-0.1.0a1/advertion/public.py
--rw-r--r--   0        0        0     1312 2023-07-16 08:51:42.125751 advertion-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 advertion-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-07-16 11:09:45.586284 advertion-0.1.0a2/README.md
+-rw-r--r--   0        0        0       98 2023-07-16 11:09:45.586284 advertion-0.1.0a2/advertion/__init__.py
+-rw-r--r--   0        0        0     6287 2023-07-16 11:09:45.586284 advertion-0.1.0a2/advertion/core.py
+-rw-r--r--   0        0        0     1857 2023-07-16 11:09:45.586284 advertion-0.1.0a2/advertion/public.py
+-rw-r--r--   0        0        0     1445 2023-07-16 11:09:45.590284 advertion-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2959 1970-01-01 00:00:00.000000 advertion-0.1.0a2/PKG-INFO
```

### Comparing `advertion-0.1.0a1/README.md` & `advertion-0.1.0a2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # adversarial-validation
 
 [![PyPI](https://img.shields.io/pypi/v/advertion?color=blue&label=PyPI&logo=PyPI&logoColor=white)](https://pypi.org/project/advertion/) 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/advertion?logo=python&logoColor=white)](https://www.python.org/) 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ilias-ant/advertion/ci.yml?branch=main)](https://github.com/ilias-ant/advertion/actions/workflows/ci.yml) 
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ilias-ant/adversarial-validation/ci.yml?branch=main)](https://github.com/ilias-ant/adversarial-validation/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/advertion/badge/?version=latest)](https://advertion.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/advertion?color=orange)](https://www.python.org/dev/peps/pep-0427/)
 
 A tiny framework to perform adversarial validation of your training and test data.
 
 ## Install
 
 The recommended installation is via `pip`:
```

### Comparing `advertion-0.1.0a1/advertion/core.py` & `advertion-0.1.0a2/advertion/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,35 +6,19 @@
 import pandas as pd
 import xgboost as xgb
 from pydantic import validate_call
 from sklearn import metrics, model_selection
 
 
 class AdversarialValidation(object):
-    """`AdversarialValidation` is an internal interface performing adversarial validation on your training and testing datasets.
+    """`AdversarialValidation` is an internal interface performing adversarial validation
+    on your training and test datasets.
 
     **Note**: Any attributes or methods prefixed with _underscores are forming a so-called "private" API, and is
     for internal use only. They may be changed or removed at anytime.
-
-    Example:
-
-        >>> train = pd.read_csv("...")
-        >>> test = pd.read_csv("...")
-        >>>
-        >>> adv = AdversarialValidation(
-        >>>     train=train,
-        >>>     test=test,
-        >>>     target="label",
-        >>>     smart=True,
-        >>>     n_splits=5,
-        >>>     verbose=True,
-        >>>     random_state=42,
-        >>> )
-        >>>
-        >>> adv.perform()
     """
 
     @validate_call(config=dict(arbitrary_types_allowed=True))
     def __init__(
         self,
         train: pd.DataFrame,
         test: pd.DataFrame,
@@ -61,15 +45,15 @@
         - Creates a new feature in both the training and test datasets.
         - Sets the value of the new feature to 0.0 for the training dataset, and 1.0 for the test dataset.
         - Drops original target variable from training dataset.
         - Combines the training and test datasets into a single dataset - let's call it `meta-dataset`.
         - Performs cross-validation on the meta-dataset, using the new feature as the target variable.
 
         Returns:
-            bool: Whether the training and test datasets are similar or not.
+            bool: Whether the train & test datasets follow the same underlying distribution.
         """
         train = self.__keep_numeric_types(self._train)
         test = self.__keep_numeric_types(self._test)
 
         train[self._av_target] = 0.0
         test[self._av_target] = 1.0
 
@@ -91,35 +75,59 @@
         return (
             self.datasets_are_similar(mean_roc_auc)
             if no_better_than_random
             else self.datasets_are_different(mean_roc_auc)
         )
 
     def datasets_are_similar(self, metric: float) -> bool:
+        """Handles the response when the training and test datasets follow the same underlying distribution.
+
+        Args:
+            metric (float): The mean ROC AUC score.
+
+        Returns:
+            bool: Always returns True.
+        """
         if self._verbose:
             print(
                 f"INFO: The training and test datasets are similar [mean ROC AUC: {round(metric, 3)}]."
             )
         return True
 
     def datasets_are_different(self, metric: float) -> bool:
+        """Handles the response when the training and test datasets follow different underlying distributions.
+
+        Args:
+            metric (float): The mean ROC AUC score.
+
+        Returns:
+            bool: Always returns False.
+        """
         if self._verbose:
             print(
                 f"INFO: The training and test datasets are similar [mean ROC AUC: {round(metric, 3)}]."
             )
 
             if metric < 0.4:
                 print(
                     f"INFO: The reported ROC AUC value is very low, which may indicate a class confusion problem."
                 )
         return False
 
     def _cross_validate(self, X: pd.DataFrame, y: pd.Series) -> Iterable[float]:
-        """Performs cross-validation, calculating the Area Under the Receiver Operating Characteristic Curve
-        (ROC AUC) from prediction scores.
+        """Performs cross-validation, calculating the
+        Area Under the Receiver Operating Characteristic Curve (ROC AUC)
+        from prediction scores.
+
+        Args:
+            X (pd.DataFrame): The design matrix.
+            y (pd.Series): The target variable.
+
+        Returns:
+            Iterable[float]: An iterable of ROC AUC scores.
         """
         cv = model_selection.StratifiedKFold(
             n_splits=self._n_splits, shuffle=True, random_state=self._random_state
         )
 
         for train, test in cv.split(X, y):
             X_train, X_test = X.iloc[train], X.iloc[test]
@@ -130,15 +138,23 @@
             clf.fit(X_train, y_train)
 
             y_pred = clf.predict_proba(X_test)[:, 1]
 
             yield metrics.roc_auc_score(y_test, y_pred)
 
     def _prune_features(self, X: pd.DataFrame, y: pd.Series) -> pd.DataFrame:
-        """Prunes features from the design matrix, based on a feature importance scheme."""
+        """Prunes features from the design matrix, based on a feature importance scheme.
+
+        Args:
+            X (pd.DataFrame): The design matrix.
+            y (pd.Series): The target variable.
+
+        Returns:
+            pd.DataFrame: The pruned design matrix.
+        """
         clf = self._classifier()
 
         model = clf.fit(X, y)
 
         prunable_features = [
             feature
             for feature, importance in zip(X.columns, model.feature_importances_)
@@ -150,14 +166,28 @@
                 f"INFO: The following features were pruned, based on feature importance: {prunable_features}"
             )
 
         return X.drop(prunable_features, axis=1)
 
     @staticmethod
     def __keep_numeric_types(df: pd.DataFrame) -> pd.DataFrame:
-        """Keeps only numeric columns in the `df`."""
+        """Keeps only numeric columns in the `df`.
+
+        Args:
+            df (pd.DataFrame): A DataFrame.
+
+        Returns:
+            pd.DataFrame: A DataFrame with only numeric-type columns.
+        """
         return df.select_dtypes(include=np.number).copy()
 
     @staticmethod
     def _classifier(**params):
-        """Returns a classifier instance."""
+        """Returns a classifier instance.
+
+        Args:
+            **params: Arbitrary keyword arguments.
+
+        Returns:
+            xgb.XGBClassifier: An XGBoost classifier instance.
+        """
         return xgb.XGBClassifier(**params)
```

### Comparing `advertion-0.1.0a1/pyproject.toml` & `advertion-0.1.0a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 [tool.poetry]
 name = "advertion"
-version = "0.1.0-alpha1"
+version = "0.1.0-alpha2"
 description = "A tiny framework to perform adversarial validation of your training and test data."
 authors = ["Ilias Antonopoulos <ilias.antonopoulos@yahoo.gr>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://pypi.org/project/advertion"
-repository = "https://github.com/ilias-ant/advertion"
+repository = "https://github.com/ilias-ant/adversarial-validation"
 keywords = ["adversarial-validation", "data-drift", "machine-learning"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/ilias-ant/advertion/issues"
+"Bug Tracker" = "https://github.com/ilias-ant/adversarial-validation/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.8.6,<3.12"
 
 scikit-learn = "~1.3.0"
 pandas = "~2.0.3"
 pydantic = "~2.0.3"
 xgboost = "~1.7.6"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.18"
+mkdocstrings = {version = "^0.20.0", extras = ["python"]}
 notebook = "^6.5.4"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `advertion-0.1.0a1/PKG-INFO` & `advertion-0.1.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: advertion
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A tiny framework to perform adversarial validation of your training and test data.
 Home-page: https://pypi.org/project/advertion
 License: Apache-2.0
 Keywords: adversarial-validation,data-drift,machine-learning
 Author: Ilias Antonopoulos
 Author-email: ilias.antonopoulos@yahoo.gr
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.8.6,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -22,24 +22,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pandas (>=2.0.3,<2.1.0)
 Requires-Dist: pydantic (>=2.0.3,<2.1.0)
 Requires-Dist: scikit-learn (>=1.3.0,<1.4.0)
 Requires-Dist: xgboost (>=1.7.6,<1.8.0)
-Project-URL: Bug Tracker, https://github.com/ilias-ant/advertion/issues
-Project-URL: Repository, https://github.com/ilias-ant/advertion
+Project-URL: Bug Tracker, https://github.com/ilias-ant/adversarial-validation/issues
+Project-URL: Repository, https://github.com/ilias-ant/adversarial-validation
 Description-Content-Type: text/markdown
 
 # adversarial-validation
 
 [![PyPI](https://img.shields.io/pypi/v/advertion?color=blue&label=PyPI&logo=PyPI&logoColor=white)](https://pypi.org/project/advertion/) 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/advertion?logo=python&logoColor=white)](https://www.python.org/) 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ilias-ant/advertion/ci.yml?branch=main)](https://github.com/ilias-ant/advertion/actions/workflows/ci.yml) 
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ilias-ant/adversarial-validation/ci.yml?branch=main)](https://github.com/ilias-ant/adversarial-validation/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/advertion/badge/?version=latest)](https://advertion.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/advertion?color=orange)](https://www.python.org/dev/peps/pep-0427/)
 
 A tiny framework to perform adversarial validation of your training and test data.
 
 ## Install
 
 The recommended installation is via `pip`:
```

