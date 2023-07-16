# Comparing `tmp/psychoanalyze-0.6.1.tar.gz` & `tmp/psychoanalyze-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.6.1.tar", max compression
+gzip compressed data, was "psychoanalyze-0.6.2.tar", max compression
```

## Comparing `psychoanalyze-0.6.1.tar` & `psychoanalyze-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-15 10:19:00.005840 psychoanalyze-0.6.1/LICENSE
--rw-r--r--   0        0        0     1105 2023-07-15 10:19:00.005840 psychoanalyze-0.6.1/README.md
--rw-r--r--   0        0        0     1357 2023-07-15 10:21:13.073870 psychoanalyze-0.6.1/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1153 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     8080 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     7763 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5206 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     2938 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1589 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1881 2023-07-15 10:21:13.073870 psychoanalyze-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 psychoanalyze-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-16 03:40:00.954832 psychoanalyze-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1105 2023-07-16 03:40:00.954832 psychoanalyze-0.6.2/README.md
+-rw-r--r--   0        0        0     1357 2023-07-16 03:43:03.128028 psychoanalyze-0.6.2/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1153 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     7140 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     7225 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5206 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3002 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1589 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1919 2023-07-16 03:43:03.128028 psychoanalyze-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 psychoanalyze-0.6.2/PKG-INFO
```

### Comparing `psychoanalyze-0.6.1/LICENSE` & `psychoanalyze-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/README.md` & `psychoanalyze-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/__init__.py` & `psychoanalyze-0.6.2/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.6.2/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.6.2/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.6.2/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.6.2/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.6.2/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/__init__.py` & `psychoanalyze-0.6.2/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/blocks.py` & `psychoanalyze-0.6.2/psychoanalyze/data/blocks.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 from psychoanalyze.data import (
     points,
     sessions,
     stimulus,
     subjects,
     trials,
-    types,
 )
 from psychoanalyze.plot import template
 
 dims = ["Amp2", "Width2", "Freq2", "Dur2", "Active Channels", "Return Channels"]
 index_levels = dims
 
 
@@ -54,51 +53,21 @@
     p = scipy_logistic.cdf(index)
     return pd.DataFrame(
         {"n": n, "Hits": np.random.default_rng().binomial(n, p)},
         index=index,
     )
 
 
-def prep_psych_curve(curves_data: pd.DataFrame, x: pd.Index, y: str) -> pd.DataFrame:
-    """Transform & fit curve data."""
-    curves_data.index = x
-    fits = points.fit(curves_data)
-    return reshape_fit_results(fits, x, y)
-
-
 def dimensions(_points: pd.DataFrame, dims: list[str]) -> pd.Series:
     """Calculate dimensions for multiple blocks."""
     return _points.groupby(
         [dim for dim in list(_points.index.names) if dim not in dims],
     ).apply(points.dimension)
 
 
-def fits(_points: pd.DataFrame) -> pd.DataFrame:
-    """Apply fits to multiple blocks."""
-    if len(_points):
-        return _points.groupby(types.block_index_levels).apply(points.fit)
-    return pd.DataFrame(
-        {"Threshold": [], "Fixed Magnitude": [], "Dimension": []},
-        index=pd.MultiIndex.from_frame(
-            pd.DataFrame(
-                {
-                    "Subject": [],
-                    "Date": [],
-                    "Amp2": [],
-                    "Width2": [],
-                    "Freq2": [],
-                    "Dur2": [],
-                    "Active Channels": [],
-                    "Return Channels": [],
-                },
-            ),
-        ),
-    )
-
-
 def plot_fits(blocks: pd.DataFrame) -> go.Figure:
     """Plot fits."""
     x = np.linspace(-3, 3, 100)
     y = expit(x)
     return px.line(blocks.reset_index(), x=x, y=y)
```

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/points.py` & `psychoanalyze-0.6.2/psychoanalyze/data/points.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,20 +35,19 @@
 
 index_levels = ["Amp1", "Width1", "Freq1", "Dur1"]
 
 
 @check_io(trials=types.trials, out=types.points)
 def from_trials(trials: pd.DataFrame) -> pd.DataFrame:
     """Aggregate point-level measures from trial data."""
-    points = trials.groupby("Intensity").agg(["count", "sum"])
-    points.columns = points.columns.droplevel()
-    points = points.rename(columns={"count": "n", "sum": "Hits"})
-    points["Hit Rate"] = points["Hits"] / points["n"]
+    points = trials.groupby(["Block", "Intensity"])["Result"].agg(["count", "sum"])
+    points = points.rename(columns={"count": "n trials", "sum": "Hits"})
+    points["Hit Rate"] = points["Hits"] / points["n trials"]
     points["logit(Hit Rate)"] = logit(points["Hit Rate"])
-    return points
+    return points.reset_index()
 
 
 @check_output(types.points)
 def load(data_path: Path) -> pd.DataFrame:
     """Load points data from csv."""
     trials = pa_trials.load(data_path)
     return from_trials(trials)
@@ -80,38 +79,14 @@
 
 
 def model() -> stan.CmdStanModel:
     """Instantiate Stan binomial regression model."""
     return stan.CmdStanModel(stan_file="models/binomial_regression.stan")
 
 
-def fit(
-    points: pd.DataFrame,
-) -> pd.DataFrame:
-    """Fit psychometric curve to points."""
-    if len(points):
-        fit = pa_trials.fit(points[["x", "Hits", "n"]])
-        return pd.DataFrame(
-            {
-                "Threshold": [fit["Threshold"]],
-                "Slope": [fit["Slope"]],
-            },
-        )
-    return pd.DataFrame(
-        {
-            "Threshold": [],
-            "width": [],
-            "lambda": [],
-            "gamma": [],
-            "err+": [],
-            "err-": [],
-        },
-    )
-
-
 def hits(
     n: pd.Series,
     params: dict[str, float],
 ) -> pd.Series:
     """Sample list of n hits from a list of intensity values."""
     p = logistic.cdf(n.index.to_numpy(), params["Threshold"], params["Slope"])
     psi = params["Guess Rate"] + (1.0 - params["Guess Rate"] - params["Lapse Rate"]) * p
```

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/sessions.py` & `psychoanalyze-0.6.2/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.6.2/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/subjects.py` & `psychoanalyze-0.6.2/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/trials.py` & `psychoanalyze-0.6.2/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/data/types.py` & `psychoanalyze-0.6.2/psychoanalyze/data/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,26 +33,28 @@
 
 block_index_levels = session_dims + block_dims
 points_index_levels = block_index_levels + point_dims
 
 
 points = DataFrameSchema(
     {
-        "n": Column(int),
+        "n trials": Column(int),
         "Hits": Column(int),
         "Hit Rate": Column(float),
         "logit(Hit Rate)": Column(float),
+        "Block": Column(int, required=False),
+        "Intensity": Column(float),
     },
-    index=Index(float, name="Intensity", unique=True),
 )
 
 trials = DataFrameSchema(
     columns={
         "Intensity": Column(float),
         "Result": Column(int),
+        "Block": Column(int),
     },
 )
 
 
 blocks = DataFrameSchema(
     columns={"Threshold": Column(dtype=float), "width": Column(dtype=float)},
     index=MultiIndex(
```

### Comparing `psychoanalyze-0.6.1/psychoanalyze/plot.py` & `psychoanalyze-0.6.2/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/psychoanalyze/sigmoids.py` & `psychoanalyze-0.6.2/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.1/pyproject.toml` & `psychoanalyze-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.6.1"
+version = "0.6.2"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
@@ -32,14 +32,15 @@
 tuna = "^0.5.11"
 ruff = "^0.0.276"
 black = "^23.3.0"
 ipykernel = "^6.24.0"
 ipywidgets = "^8.0.7"
 kaleido = "0.2.1"
 pyarrow = "^12.0.1"
+types-pytz = "^2023.3.0.0"
 
 [tool.poetry.scripts]
 psychoanalyze = "psychoanalyze.__main__:main"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
@@ -71,14 +72,15 @@
     'scipy.special',
     'sklearn.linear_model',
     'dash_daq',
     'datatest',
     'bambi',
     'hypothesis',
     'statsmodels.*',
+    'pytz'
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 fix = true
 select = ["ALL", "CPY001"]
 ignore = ["S101", "S311", "D211", "D213"]
```

### Comparing `psychoanalyze-0.6.1/PKG-INFO` & `psychoanalyze-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,15 @@
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
 Requires-Dist: ruff (>=0.0.276,<0.0.277)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: tuna (>=0.5.11,<0.6.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: types-pytz (>=2023.3.0.0,<2024.0.0.0)
 Description-Content-Type: text/markdown
 
 # PsychoAnalyze
 
 Psychophysics analysis in Python.
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
```

