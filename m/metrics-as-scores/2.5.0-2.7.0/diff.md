# Comparing `tmp/metrics_as_scores-2.5.0.tar.gz` & `tmp/metrics_as_scores-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrics_as_scores-2.5.0.tar", max compression
+gzip compressed data, was "metrics_as_scores-2.7.0.tar", max compression
```

## Comparing `metrics_as_scores-2.5.0.tar` & `metrics_as_scores-2.7.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      287 2023-02-20 16:35:52.783754 metrics_as_scores-2.5.0/build.py
--rw-r--r--   0        0        0    36442 2022-09-30 12:51:35.511324 metrics_as_scores-2.5.0/LICENSE
--rw-r--r--   0        0        0     2709 2023-03-11 21:37:49.322147 metrics_as_scores-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    22901 2023-03-11 22:48:53.707042 metrics_as_scores-2.5.0/README.md
--rw-r--r--   0        0        0     1063 2023-02-21 15:04:45.717411 metrics_as_scores-2.5.0/src/metrics_as_scores/__init__.py
--rw-r--r--   0        0        0     1157 2023-02-20 16:35:52.798739 metrics_as_scores-2.5.0/src/metrics_as_scores/__version__.py
--rw-r--r--   0        0        0      284 2023-02-21 14:36:01.334095 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/__init__.py
--rw-r--r--   0        0        0     4247 2023-02-21 14:41:08.627396 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/BundleOwn.py
--rw-r--r--   0        0        0      895 2023-02-20 16:35:52.800735 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/Cli.py
--rw-r--r--   0        0        0    19298 2023-02-22 18:45:00.153334 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/CreateDataset.py
--rw-r--r--   0        0        0     2716 2023-03-11 08:16:06.622840 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/Download.py
--rw-r--r--   0        0        0    11279 2023-02-22 17:34:05.272925 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/FitParametric.py
--rw-r--r--   0        0        0     5096 2023-02-22 17:50:36.341028 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/GenerateDensities.py
--rw-r--r--   0        0        0     8278 2023-02-23 10:31:27.664091 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/helpers.py
--rw-r--r--   0        0        0     2203 2023-02-21 14:45:48.693604 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/KnownDatasets.py
--rw-r--r--   0        0        0     1805 2023-02-21 14:46:19.522152 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/LocalDatasets.py
--rw-r--r--   0        0        0     9257 2023-03-11 09:03:13.115378 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/LocalWebserver.py
--rw-r--r--   0        0        0     3199 2023-02-27 21:53:48.302230 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/MainWorkflow.py
--rw-r--r--   0        0        0     3800 2023-02-21 19:55:10.903287 metrics_as_scores-2.5.0/src/metrics_as_scores/cli/Workflow.py
--rw-r--r--   0        0        0      265 2023-02-21 14:50:32.143284 metrics_as_scores-2.5.0/src/metrics_as_scores/data/__init__.py
--rw-r--r--   0        0        0    13093 2023-02-22 21:39:05.757609 metrics_as_scores-2.5.0/src/metrics_as_scores/data/pregenerate.py
--rw-r--r--   0        0        0     5576 2023-02-21 14:51:15.534575 metrics_as_scores-2.5.0/src/metrics_as_scores/data/pregenerate_distns.py
--rw-r--r--   0        0        0     7468 2023-02-21 14:52:04.110566 metrics_as_scores-2.5.0/src/metrics_as_scores/data/pregenerate_fit.py
--rw-r--r--   0        0        0      342 2023-02-22 23:23:44.232871 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/_quarto.yml
--rw-r--r--   0        0        0    14513 2023-02-20 16:35:52.810722 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/About.qmd
--rw-r--r--   0        0        0      507 2023-02-20 16:35:52.811720 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/readme.md
--rw-r--r--   0        0        0     1876 2023-02-20 16:35:52.812720 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/refs.bib
--rw-r--r--   0        0        0      435 2023-02-20 16:35:52.813718 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/web/about.html
--rw-r--r--   0        0        0      467 2023-02-20 16:35:52.813718 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/web/references.html
--rw-r--r--   0        0        0     1488 2023-02-23 10:26:41.636541 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/known-datasets.bib
--rw-r--r--   0        0        0     1277 2023-02-23 10:25:57.611021 metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/known-datasets.json
--rw-r--r--   0        0        0      226 2023-02-21 14:55:03.869208 metrics_as_scores-2.5.0/src/metrics_as_scores/distribution/__init__.py
--rw-r--r--   0        0        0    46370 2023-02-22 22:30:40.743996 metrics_as_scores-2.5.0/src/metrics_as_scores/distribution/distribution.py
--rw-r--r--   0        0        0    22219 2023-02-21 11:51:27.268549 metrics_as_scores-2.5.0/src/metrics_as_scores/distribution/fitting.py
--rw-r--r--   0        0        0    22308 2023-02-20 16:35:52.817713 metrics_as_scores-2.5.0/src/metrics_as_scores/distribution/fitting_problems.py
--rw-r--r--   0        0        0     2709 2023-03-11 22:49:03.230446 metrics_as_scores-2.5.0/src/metrics_as_scores/pyproject.toml
--rw-r--r--   0        0        0       82 2023-02-21 14:57:18.585561 metrics_as_scores-2.5.0/src/metrics_as_scores/tools/__init__.py
--rw-r--r--   0        0        0     5377 2023-02-22 15:47:07.550809 metrics_as_scores-2.5.0/src/metrics_as_scores/tools/funcs.py
--rw-r--r--   0        0        0     5440 2023-02-21 15:01:17.203704 metrics_as_scores-2.5.0/src/metrics_as_scores/tools/lazy.py
--rw-r--r--   0        0        0      229 2023-02-21 15:02:54.043069 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/__init__.py
--rw-r--r--   0        0        0     3414 2023-02-27 22:33:35.208735 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/app_hooks.py
--rw-r--r--   0        0        0      931 2023-02-20 16:35:52.820709 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/data.py
--rw-r--r--   0        0        0      408 2023-02-20 16:35:52.821708 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/exception.py
--rw-r--r--   0        0        0    10579 2023-02-20 16:35:52.822709 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/footer.html
--rw-r--r--   0        0        0      719 2023-02-20 16:35:52.822709 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/header.html
--rw-r--r--   0        0        0    22496 2023-03-11 21:23:38.641502 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/main.py
--rw-r--r--   0        0        0     1774 2023-02-23 13:00:06.071638 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf
--rw-r--r--   0        0        0      556 2023-02-23 12:55:19.966184 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/metrics-as-scores.service
--rw-r--r--   0        0        0      180 2022-09-05 06:40:38.188152 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/readme.md
--rw-r--r--   0        0        0   113561 2022-09-05 06:40:56.466003 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/curve.ico
--rw-r--r--   0        0        0    29350 2022-09-05 06:40:22.832754 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/curve.png
--rw-r--r--   0        0        0    11170 2022-09-20 15:00:30.424180 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/loading.png
--rw-r--r--   0        0        0      121 2023-02-20 16:35:52.824708 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/main.js
--rw-r--r--   0        0        0      981 2023-02-20 16:35:52.825704 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/styles.css
--rw-r--r--   0        0        0     1643 2023-02-20 16:35:52.827702 metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/templates/index.html
--rw-r--r--   0        0        0    24574 1970-01-01 00:00:00.000000 metrics_as_scores-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      287 2023-02-20 16:35:52.783754 metrics_as_scores-2.7.0/build.py
+-rw-r--r--   0        0        0    36442 2022-09-30 12:51:35.511324 metrics_as_scores-2.7.0/LICENSE
+-rw-r--r--   0        0        0     2709 2023-07-16 11:42:51.235669 metrics_as_scores-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    23183 2023-07-16 11:43:08.741420 metrics_as_scores-2.7.0/README.md
+-rw-r--r--   0        0        0     1063 2023-04-13 06:55:30.716391 metrics_as_scores-2.7.0/src/metrics_as_scores/__init__.py
+-rw-r--r--   0        0        0     1157 2023-02-20 16:35:52.798739 metrics_as_scores-2.7.0/src/metrics_as_scores/__version__.py
+-rw-r--r--   0        0        0      284 2023-04-13 06:55:30.745365 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/__init__.py
+-rw-r--r--   0        0        0     4247 2023-04-13 06:55:30.717395 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/BundleOwn.py
+-rw-r--r--   0        0        0      895 2023-02-20 16:35:52.800735 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/Cli.py
+-rw-r--r--   0        0        0    20437 2023-07-16 08:13:42.684832 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/CreateDataset.py
+-rw-r--r--   0        0        0     2716 2023-04-13 06:55:30.722386 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/Download.py
+-rw-r--r--   0        0        0    11653 2023-04-21 13:19:41.659645 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/FitParametric.py
+-rw-r--r--   0        0        0     5096 2023-04-13 06:55:30.728381 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/GenerateDensities.py
+-rw-r--r--   0        0        0     8397 2023-07-16 08:13:42.685838 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/helpers.py
+-rw-r--r--   0        0        0     2203 2023-04-13 06:55:30.735370 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/KnownDatasets.py
+-rw-r--r--   0        0        0     1805 2023-04-13 06:55:30.736372 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/LocalDatasets.py
+-rw-r--r--   0        0        0     9257 2023-04-13 06:55:30.738364 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/LocalWebserver.py
+-rw-r--r--   0        0        0     3199 2023-04-13 06:55:30.742360 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/MainWorkflow.py
+-rw-r--r--   0        0        0     3800 2023-04-13 06:55:30.743360 metrics_as_scores-2.7.0/src/metrics_as_scores/cli/Workflow.py
+-rw-r--r--   0        0        0      265 2023-04-13 06:55:30.747364 metrics_as_scores-2.7.0/src/metrics_as_scores/data/__init__.py
+-rw-r--r--   0        0        0    13093 2023-04-21 13:19:41.661631 metrics_as_scores-2.7.0/src/metrics_as_scores/data/pregenerate.py
+-rw-r--r--   0        0        0     5576 2023-04-13 06:55:30.749364 metrics_as_scores-2.7.0/src/metrics_as_scores/data/pregenerate_distns.py
+-rw-r--r--   0        0        0     7256 2023-04-21 13:19:41.661631 metrics_as_scores-2.7.0/src/metrics_as_scores/data/pregenerate_fit.py
+-rw-r--r--   0        0        0      342 2023-04-13 06:55:30.752350 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/_quarto.yml
+-rw-r--r--   0        0        0    14513 2023-02-20 16:35:52.810722 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/About.qmd
+-rw-r--r--   0        0        0      507 2023-02-20 16:35:52.811720 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/readme.md
+-rw-r--r--   0        0        0     1876 2023-02-20 16:35:52.812720 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/refs.bib
+-rw-r--r--   0        0        0      435 2023-02-20 16:35:52.813718 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/web/about.html
+-rw-r--r--   0        0        0      467 2023-02-20 16:35:52.813718 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/web/references.html
+-rw-r--r--   0        0        0     1488 2023-04-13 06:55:30.752350 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/known-datasets.bib
+-rw-r--r--   0        0        0     1277 2023-04-13 06:55:30.753348 metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/known-datasets.json
+-rw-r--r--   0        0        0      226 2023-04-13 06:55:30.754353 metrics_as_scores-2.7.0/src/metrics_as_scores/distribution/__init__.py
+-rw-r--r--   0        0        0    48503 2023-07-16 08:13:42.686830 metrics_as_scores-2.7.0/src/metrics_as_scores/distribution/distribution.py
+-rw-r--r--   0        0        0    22219 2023-04-13 06:55:30.757346 metrics_as_scores-2.7.0/src/metrics_as_scores/distribution/fitting.py
+-rw-r--r--   0        0        0    22308 2023-02-20 16:35:52.817713 metrics_as_scores-2.7.0/src/metrics_as_scores/distribution/fitting_problems.py
+-rw-r--r--   0        0        0     2709 2023-07-16 11:43:18.080115 metrics_as_scores-2.7.0/src/metrics_as_scores/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-04-13 06:55:30.758350 metrics_as_scores-2.7.0/src/metrics_as_scores/tools/__init__.py
+-rw-r--r--   0        0        0     5389 2023-04-13 06:55:30.760341 metrics_as_scores-2.7.0/src/metrics_as_scores/tools/funcs.py
+-rw-r--r--   0        0        0     5440 2023-04-13 06:55:30.761351 metrics_as_scores-2.7.0/src/metrics_as_scores/tools/lazy.py
+-rw-r--r--   0        0        0      229 2023-04-13 06:55:30.762348 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-13 06:55:30.764342 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/app_hooks.py
+-rw-r--r--   0        0        0      931 2023-02-20 16:35:52.820709 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/data.py
+-rw-r--r--   0        0        0      408 2023-02-20 16:35:52.821708 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/exception.py
+-rw-r--r--   0        0        0    10664 2023-07-16 08:13:42.689826 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/footer.html
+-rw-r--r--   0        0        0      746 2023-07-16 08:13:42.690824 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/header.html
+-rw-r--r--   0        0        0    22752 2023-07-16 11:40:55.495096 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/main.py
+-rw-r--r--   0        0        0     1774 2023-04-13 06:55:30.766341 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf
+-rw-r--r--   0        0        0      556 2023-04-13 06:55:30.788315 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/metrics-as-scores.service
+-rw-r--r--   0        0        0      180 2022-09-05 06:40:38.188152 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/readme.md
+-rw-r--r--   0        0        0   113561 2022-09-05 06:40:56.466003 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/curve.ico
+-rw-r--r--   0        0        0    29350 2022-09-05 06:40:22.832754 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/curve.png
+-rw-r--r--   0        0        0    11170 2022-09-20 15:00:30.424180 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/loading.png
+-rw-r--r--   0        0        0      121 2023-02-20 16:35:52.824708 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/main.js
+-rw-r--r--   0        0        0      981 2023-02-20 16:35:52.825704 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/styles.css
+-rw-r--r--   0        0        0     1643 2023-02-20 16:35:52.827702 metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/templates/index.html
+-rw-r--r--   0        0        0    24845 1970-01-01 00:00:00.000000 metrics_as_scores-2.7.0/PKG-INFO
```

### Comparing `metrics_as_scores-2.5.0/LICENSE` & `metrics_as_scores-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/pyproject.toml` & `metrics_as_scores-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metrics-as-scores"
-version = "2.5.0"
+version = "2.7.0"
 description = "Interactive web application, tool- and analysis suite for approximating, exploring, understanding, and sampling from conditional distributions."
 authors = ["Sebastian Hönel <development@hoenel.net>"]
 license = "Dual-licensed under GNU General Public License v3 (GPLv3) and closed-source"
 readme = "README.md"
 homepage = "https://github.com/mrshoenel/metrics-as-scores"
 repository = "https://github.com/mrshoenel/metrics-as-scores/issues"
 packages = [{include = "metrics_as_scores", from = "src"}]
@@ -33,15 +33,15 @@
 python = ">=3.10, <3.12"
 bokeh = "^2.4.3"
 joblib = "^1.2.0"
 jupyterlab = "^3.4.7"
 matplotlib = "^3.6.0"
 ptvsd = "^4.3.2"
 pymoo = "^0.6.0"
-scipy = "^1.9.1"
+scipy = "1.10.1"
 statsmodels = "^0.13.2"
 StrEnum = "^0.4.8"
 tqdm = "^4.64.1"
 Sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 toml = "^0.10.2"
 rich = "^13.3.1"
@@ -54,15 +54,15 @@
 wget = "^3.2"
 myst-parser = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.1"
 build = "^0.8.0"
-poetry = "^1.2.1"
+poetry = "^1.3.2"
 pytest = "^7.1.3"
 coverage = "^6.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `metrics_as_scores-2.5.0/README.md` & `metrics_as_scores-2.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ------------------------------------------------------------------------
 
 **Please Note**: ***Metrics As Scores*** (`MAS`) changed considerably
 between versions
 [**`v1.0.8`**](https://github.com/MrShoenel/metrics-as-scores/tree/v1.0.8)
 and **`v2.x.x`**.
 
-The current version is `v2.5.0`.
+The current version is `v2.7.0`.
 
 From version **`v2.x.x`** it has the following new features:
 
 - [Textual User Interface (TUI)](#text-based-user-interface-tui)
 - Proper documentation and testing
 - New version on PyPI. Install the package and run the command line
   interface by typing **`mas`**!
@@ -132,28 +132,30 @@
 
 ## Web Application
 
 Metrics As Scores’ main feature is perhaps the Web Application. It can
 be run directly and locally from the TUI using a selected dataset (you
 may download a known dataset or use your own). The Web Application
 allows to visually inspect each *feature* across all the defined
-*groups*. It feates the PDF/PMF, CDF and CCDF, as well as the PPF for
+*groups*. It features the PDF/PMF, CDF and CCDF, as well as the PPF for
 each feature in each group. It offers five different principal types of
 densities: Parametric, Parametric (discrete), Empirical, Empirical
 (discrete), and (approximate) Kernel Density Estimation. The Web
 Application includes a detailed [Help
 section](https://metrics-as-scores.ml/#help) that should answer most of
 your questions.
 
 ![Metrics As Scores Interactive Web
 .](./WebApp.png "Metrics As Scores Interactive Web Appliction.")
 
 ## Development Setup
 
-This project was developed using and requires Python `>=3.10`. Steps:
+This project was developed using and requires Python `>=3.10`. The
+development documentation can be found at
+<https://mrshoenel.github.io/metrics-as-scores/>. Steps:
 
 1.  Clone the Repository,
 2.  Set up a virtual environment,
 3.  Install packages.
 
 ### Setting Up a Virtual Environment
 
@@ -178,25 +180,28 @@
 ### Installing Packages
 
 The project is managed with `Poetry`. To install the required packages,
 simply run the following.
 
 ``` shell
 venv/Scripts/activate
-# First install Poetry using pip:
-(venv) C:\metrics-as-scores>pip install poetry
+# First, update pip:
+(venv) C:\metrics-as-scores>python -m pip install --upgrade pip
+# First install Poetry v1.3.2 using pip:
+(venv) C:\metrics-as-scores>pip install poetry==1.3.2
 # Install the projects and its dependencies
 (venv) C:\metrics-as-scores> poetry install
 ```
 
 The same in Linux:
 
 ``` shell
 source venv/bin/activate # Linux
-(venv) ubuntu@vm:/tmp/metrics-as-scores$ pip install poetry
+(venv) ubuntu@vm:/tmp/metrics-as-scores$ python -m pip install --upgrade pip
+(venv) ubuntu@vm:/tmp/metrics-as-scores$ pip install poetry==1.3.2
 (venv) ubuntu@vm:/tmp/metrics-as-scores$ poetry install
 ```
 
 ### Running Tests
 
 Tests are run using `poethepoet`:
 
@@ -517,15 +522,15 @@
 
 </div>
 
 <div id="ref-tukey1949anova" class="csl-entry">
 
 Tukey, John W. 1949. “Comparing Individual Means in the Analysis of
 Variance.” *Biometrics* 5 (2): 99–114.
-<http://www.jstor.org/stable/3001913>.
+<https://doi.org/10.2307/3001913>.
 
 </div>
 
 <div id="ref-ggplot2" class="csl-entry">
 
 Wickham, Hadley. 2016. *<span class="nocase">ggplot2</span>: Elegant
 Graphics for Data Analysis*. Springer-Verlag New York.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 Packages - 1.3.3_Running_Tests - 2_Example_Usage - 2.1_Concrete_Example_Using
 the_Qualitas.class_Corpus_Dataset - 2.2_Concrete_Example_Using_the_Iris_Dataset
 - 2.3_Diamonds_Example - 3_Datasets - 3.1_Use_Your_Own - 3.2_Known_Datasets - 4
 Personalizing_the_Web_Application - References --------------------------------
 ---------------------------------------- **Please Note**: ***Metrics As
 Scores*** (`MAS`) changed considerably between versions [**`v1.0.8`**](https://
 github.com/MrShoenel/metrics-as-scores/tree/v1.0.8) and **`v2.x.x`**. The
-current version is `v2.5.0`. From version **`v2.x.x`** it has the following new
+current version is `v2.7.0`. From version **`v2.x.x`** it has the following new
 features: - [Textual User Interface (TUI)](#text-based-user-interface-tui) -
 Proper documentation and testing - New version on PyPI. Install the package and
 run the command line interface by typing **`mas`**! [Metrics As Scores Demo.]
 (https://user-images.githubusercontent.com/5049151/219892077-58854478-b761-
 4a3d-9faf-2fe46c122cf5.webm) --------------------------------------------------
 ---------------------- Contains the data and scripts needed for the application
 **`Metrics as Scores`**, check out
@@ -55,37 +55,41 @@
 in the [**Web-Application**](#web-application) - Bundle Own dataset so it can
 be published - Run local, interactive Web-Application using a selected dataset
 ![Metrics As Scores Text-based User Interface (TUI).](./TUI.png "Metrics As
 Scores Text-based User Interface (TUI).") ## Web Application Metrics As
 Scoresâ main feature is perhaps the Web Application. It can be run directly
 and locally from the TUI using a selected dataset (you may download a known
 dataset or use your own). The Web Application allows to visually inspect each
-*feature* across all the defined *groups*. It feates the PDF/PMF, CDF and CCDF,
-as well as the PPF for each feature in each group. It offers five different
-principal types of densities: Parametric, Parametric (discrete), Empirical,
-Empirical (discrete), and (approximate) Kernel Density Estimation. The Web
-Application includes a detailed [Help section](https://metrics-as-scores.ml/
-#help) that should answer most of your questions. ![Metrics As Scores
+*feature* across all the defined *groups*. It features the PDF/PMF, CDF and
+CCDF, as well as the PPF for each feature in each group. It offers five
+different principal types of densities: Parametric, Parametric (discrete),
+Empirical, Empirical (discrete), and (approximate) Kernel Density Estimation.
+The Web Application includes a detailed [Help section](https://metrics-as-
+scores.ml/#help) that should answer most of your questions. ![Metrics As Scores
 Interactive Web .](./WebApp.png "Metrics As Scores Interactive Web
 Appliction.") ## Development Setup This project was developed using and
-requires Python `>=3.10`. Steps: 1. Clone the Repository, 2. Set up a virtual
-environment, 3. Install packages. ### Setting Up a Virtual Environment It is
-recommended to use a virtual environment. To use a virtual environment, follow
-these steps (Windows specific; activation of the environment might differ). ```
-shell virtualenv --python=C:/Python310/python.exe venv # Use specific Python
-version for virtual environment venv/Scripts/activate ``` Here is a Linux
-example that assumes you have Python `3.10` installed (this may also require
-installing `python3.10-venv` and/or `python3.10-dev`): ``` shell python3.10 -
-m venv venv source venv/bin/activate # Linux ``` ### Installing Packages The
-project is managed with `Poetry`. To install the required packages, simply run
-the following. ``` shell venv/Scripts/activate # First install Poetry using
-pip: (venv) C:\metrics-as-scores>pip install poetry # Install the projects and
-its dependencies (venv) C:\metrics-as-scores> poetry install ``` The same in
-Linux: ``` shell source venv/bin/activate # Linux (venv) ubuntu@vm:/tmp/
-metrics-as-scores$ pip install poetry (venv) ubuntu@vm:/tmp/metrics-as-scores$
+requires Python `>=3.10`. The development documentation can be found at
+mrshoenel.github.io/metrics-as-scores/>. Steps: 1. Clone the Repository, 2. Set
+up a virtual environment, 3. Install packages. ### Setting Up a Virtual
+Environment It is recommended to use a virtual environment. To use a virtual
+environment, follow these steps (Windows specific; activation of the
+environment might differ). ``` shell virtualenv --python=C:/Python310/
+python.exe venv # Use specific Python version for virtual environment venv/
+Scripts/activate ``` Here is a Linux example that assumes you have Python
+`3.10` installed (this may also require installing `python3.10-venv` and/or
+`python3.10-dev`): ``` shell python3.10 -m venv venv source venv/bin/activate #
+Linux ``` ### Installing Packages The project is managed with `Poetry`. To
+install the required packages, simply run the following. ``` shell venv/
+Scripts/activate # First, update pip: (venv) C:\metrics-as-scores>python -m pip
+install --upgrade pip # First install Poetry v1.3.2 using pip: (venv) C:
+\metrics-as-scores>pip install poetry==1.3.2 # Install the projects and its
+dependencies (venv) C:\metrics-as-scores> poetry install ``` The same in Linux:
+``` shell source venv/bin/activate # Linux (venv) ubuntu@vm:/tmp/metrics-as-
+scores$ python -m pip install --upgrade pip (venv) ubuntu@vm:/tmp/metrics-as-
+scores$ pip install poetry==1.3.2 (venv) ubuntu@vm:/tmp/metrics-as-scores$
 poetry install ``` ### Running Tests Tests are run using `poethepoet`: ```
 shell # Runs the tests and prints coverage (venv) C:\metrics-as-scores>poe test
 ``` You can also generate coverage reports: ``` shell # Writes reports to the
 local directory htmlcov (venv) C:\metrics-as-scores>poe cov ``` ---------------
 --------------------------------------------------------- # Example Usage
 *Metrics As Scores* can be thought of an *interactive*, *multiple-ANOVA*
 analysis and explorer. The analysis of variance (ANOVA; John M. Chambers
@@ -261,11 +265,11 @@
 doi.org/10.1109/APSEC.2010.46>.
 Terra, Ricardo, Luis Fernando Miranda, Marco TÃºlio Valente, and Roberto da
 Silva Bigonha. 2013. âQualitas.class Corpus: A Compiled Version of the
 Qualitas Corpus.â *ACM SIGSOFT Softw. Eng. Notes* 38 (5): 1â4.
 doi.org/10.1145/2507288.2507314>.
 Tukey, John W. 1949. âComparing Individual Means in the Analysis of
 Variance.â *Biometrics* 5 (2): 99â114.
-www.jstor.org/stable/3001913>.
+doi.org/10.2307/3001913>.
 Wickham, Hadley. 2016. *ggplot2: Elegant Graphics for Data Analysis*. Springer-
 Verlag New York.
 ggplot2.tidyverse.org>.
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/__init__.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/__init__.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/__version__.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/__version__.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/BundleOwn.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/BundleOwn.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/Cli.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/Cli.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/CreateDataset.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/CreateDataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,18 @@
         return self.dataset_dir.joinpath('./org-data.csv')
 
 
     @property
     def path_test_ANOVA(self) -> Path:
         return self.tests_dir.joinpath('./anova.csv')
     
+    @property
+    def path_test_KruskalWallis(self) -> Path:
+        return self.tests_dir.joinpath('./kruskal.csv')
+    
 
     @property
     def path_test_TukeyHSD(self) -> Path:
         return self.tests_dir.joinpath('./tukeyhsd.csv')
     
 
     @property
@@ -128,15 +132,15 @@
 
     def _transform_dataset(self) -> pd.DataFrame:
         self.q.print('\n' + 10*'-')
         file_type = self.ask(options=[
             'CSV', 'Excel'
         ], prompt='What kind of file do you want to read?', rtype=str)
 
-        path = self.q.text(message='Absolute file path or URL to original file:', validate=lambda s: len(s) > 0).ask().strip()
+        path = self.q.text(message='Absolute file path or URL to original file:', validate=lambda s: len(s) > 0).ask().strip().strip('"\'')
         df: pd.DataFrame = None
         if file_type == 'CSV':
             df = self._read_csv(path_like=path)
         elif file_type == 'Excel':
             df = self._read_excel(path_like=path)
         
         available_cols = OrderedDict({ k: k for k in df.columns.values.tolist() })
@@ -284,19 +288,25 @@
         return (jsd, df)
 
 
     def _run_statistical_tests(self) -> None:
         self.q.print('We will now perform some statistical tests and summarize the results.')
         
         self.print_info(text_normal='Performing tests: ', text_vital='Analysis of Variance (ANOVA) ...', arrow='\n')
-        anova = self.dataset.analyze_ANOVA(qtypes=self.dataset.quantity_types, contexts=list(self.dataset.contexts(include_all_contexts=True)), unique_vals=True)
+        anova = self.dataset.analyze_groups(use='anova', qtypes=self.dataset.quantity_types, contexts=list(self.dataset.contexts(include_all_contexts=True)), unique_vals=True)
         file_anova = str(self.path_test_ANOVA)
         anova.to_csv(file_anova, index=False)
         self.print_info(text_normal='Wrote result to: ', text_vital=file_anova)
 
+        self.print_info(text_normal='Performing tests: ', text_vital='Kruskal-Wallis H-test ...', arrow='\n')
+        kruskal = self.dataset.analyze_groups(use='kruskal', qtypes=self.dataset.quantity_types, contexts=list(self.dataset.contexts(include_all_contexts=True)), unique_vals=True)
+        file_kruskal = str(self.path_test_KruskalWallis)
+        kruskal.to_csv(file_kruskal, index=False)
+        self.print_info(text_normal='Wrote result to: ', text_vital=file_kruskal)
+
         self.print_info(text_normal='Performing tests: ', text_vital='Two-Sample Kolmogorov-Smirnov (KS2) ...', arrow='\n')
         ks2samp = self.dataset.analyze_distr(qtypes=self.dataset.quantity_types, use_ks_2samp=True)
         file_ks2samp = str(self.path_test_ks2samp)
         ks2samp.to_csv(file_ks2samp, index=False)
         self.print_info(text_normal='Wrote result to: ', text_vital=file_ks2samp)
 
         self.print_info(text_normal='Performing tests: ', text_vital="Tukey's Honest Significance Test (TukeyHSD) ...", arrow='\n')
@@ -362,14 +372,22 @@
         transformed_df: pd.DataFrame = None
         self.q.print('')
         if self.q.confirm(message='Would you like to transform a data frame first?', default=False).ask():
             transformed_df = self._transform_dataset()
 
         self.manifest, self.org_df = self._create_manifest(transformed_df=transformed_df)
         self.dataset = Dataset(ds=self.manifest, df=self.org_df)
+
+        # Let's attempt to ascertain that the dataset has sufficiently many observations:
+        try:
+            self.dataset.has_sufficient_observations(raise_if_not=True)
+        except Exception as ex:
+            self.q.print(text=str(ex), style=self.style_err)
+            self.q.print(text='The dataset does not contain sufficiently many observations and cannot be used as-is with Metrics As Scores. At least two observations per feature and group are required.')
+            return
         
         # Let's create a folder for this dataset (by ID) and out the files there.
         self._make_dirs()
         
         # Let's copy specific files from the default over to the new dataset:
         self._init_dataset()
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/Download.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/Download.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/FitParametric.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/FitParametric.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from scipy.stats._distn_infrastructure import rv_continuous, rv_discrete
 from metrics_as_scores.cli.helpers import get_local_datasets, isint
 from metrics_as_scores.cli.Workflow import Workflow
 from metrics_as_scores.distribution.distribution import DistTransform, LocalDataset, Dataset
 from metrics_as_scores.distribution.fitting import Fitter, FitterPymoo, Continuous_RVs, Discrete_Problems
 from metrics_as_scores.data.pregenerate_fit import get_data_tuple
 from metrics_as_scores.data.pregenerate_distns import generate_parametric_fits
+from metrics_as_scores.tools.funcs import flatten_dict
 from questionary import Choice
 from pickle import dump
 from os import cpu_count
 from joblib import Parallel, delayed
 from tqdm import tqdm
 import pandas as pd
 
@@ -66,15 +67,15 @@
 You can now select the continuous random variables that you want to
 attempt to fit to the data. Select all in case you intend to re-
 distribute and publicize your dataset. It is often not worth to de-
 select distributions unless you have a specific reason to do so,
 because fitting a continuous distribution is comparatively cheap and
 fast.'''.strip())
         recommend_ignore = [norminvgauss_gen, gausshyper_gen, genhyperbolic_gen, geninvgauss_gen, invgauss_gen, studentized_range_gen]
-        return self.q.checkbox(message='Select continuous random variables:', choices=[Choice(title=type(rv).__name__, value=type(rv), checked=not type(rv) in recommend_ignore) for rv in Continuous_RVs]).ask()
+        return self.q.checkbox(message='Select continuous random variables:', choices=[Choice(title=f'{type(rv).__name__} [{rv.name}]', value=type(rv), checked=not type(rv) in recommend_ignore) for rv in Continuous_RVs]).ask()
 
 
     def _select_discrete_rvs(self) -> Iterable[type[rv_discrete]]:
         self.q.print('''
 You can now select the discrete random variables that you want to
 additionally attempt to fit to discrete features. Select all in
 case you intend to redistribute and publicize your dataset.
@@ -206,7 +207,14 @@
                 self.print_info(text_normal='Fits already computed for transform: ', text_vital=f'{dist_transform.value} [{dist_transform.name}]')
                 continue
             
             self.print_info(text_normal='Generating parametric fits for: ', text_vital=f'{dist_transform.value} [{dist_transform.name}]')
             res = self._fit_parametric(dist_transform=dist_transform)
             with open(file=str(result_file), mode='wb') as fp:
                 dump(obj=res, file=fp)
+            
+            # Also, let's dump a CSV with all results.
+            result_file = self.fits_dir.joinpath(f'./pregen_distns_{dist_transform.name}.csv')
+            df = pd.DataFrame([flatten_dict(d=d) for d in res])
+            df.to_csv(path_or_buf=str(result_file), index=False)
+
+
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/GenerateDensities.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/GenerateDensities.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/helpers.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,17 @@
         dir_densities.joinpath(f'./densities_{perm[0].__name__}_{perm[1].name}.pickle')
         for perm in product([
             Parametric, Parametric_discrete, Empirical, Empirical_discrete, KDE_approx
         ], list(DistTransform))
     ]) + list([
         dir_fits.joinpath(f'./pregen_distns_{dt.name}.pickle') for dt in list(DistTransform)
     ]) + list([
-        dir_stests.joinpath(f'./{file}.csv') for file in ['anova', 'ks2samp', 'tukeyhsd']
+        dir_fits.joinpath(f'./pregen_distns_{dt.name}.csv') for dt in list(DistTransform)
+    ]) + list([
+        dir_stests.joinpath(f'./{file}.csv') for file in ['anova', 'ks2samp', 'tukeyhsd', 'kruskal']
     ]) + list([
         dir_web.joinpath(f'./{file}.html') for file in ['about', 'references']
     ]) + list([
         ds_dir.joinpath(f'./{file}') for file in [
             'About.pdf',
             'manifest.json',
             'org-data.csv',
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/KnownDatasets.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/KnownDatasets.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/LocalDatasets.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/LocalDatasets.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/LocalWebserver.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/LocalWebserver.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/MainWorkflow.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/MainWorkflow.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/cli/Workflow.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/cli/Workflow.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/data/pregenerate.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/data/pregenerate.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         the value is the generated :py:class:`Union[Parametric, Parametric_discrete]` density.
     """
     df = pd.DataFrame([flatten_dict(d) for d in distns_dict.values()])
     data_df = dataset.df
 
     contexts = list(dataset.contexts(include_all_contexts=True))
     the_type = 'continuous' if use_continuous else 'discrete'
-    use_test = 'ks_2samp_ordinary' if use_continuous else 'epps_singleton_2samp_jittered'
+    use_test = 'ks_1samp_ordinary' if use_continuous else 'epps_singleton_2samp_jittered'
     use_stat = f'stat_tests_tests_{use_test}_stat'
     use_vars = Continuous_RVs_dict if use_continuous else Discrete_RVs_dict
     Use_class = Parametric if use_continuous else Parametric_discrete
 
     df_cols = list(df.columns)
     the_dict: dict[str, Parametric] = {}
     for context in contexts:
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/data/pregenerate_distns.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/data/pregenerate_distns.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/data/pregenerate_fit.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/data/pregenerate_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,21 +162,15 @@
         fitter = fitter_type(dist=RV)
         params = fitter.fit(data=data, verbose=False)
         params_tuple = tuple(params.values())
 
         ret_dict.update(dict(params = params))
 
         dist = RV()
-        def temp_cdf(x: NDArray[Shape["*"], Float]):
-            x = np.asarray(x).copy()
-            min_ = np.min(data)
-            max_ = np.max(data)
-            x[x < min_] = min_
-            x[x > max_] = max_
-            return dist.cdf(*(x, *params_tuple))
+        temp_cdf = lambda x: dist.cdf(*(x, *params_tuple))
         temp_ppf = lambda x: dist.ppf(*(x, *params_tuple))
 
         data_st = data if not unique_vals else np.rint(data) # Remove jitter for test
         st = StatisticalTest(data1=data_st, cdf=temp_cdf, ppf_or_data2=temp_ppf, max_samples=25_000)
         ret_dict.update(dict(stat_tests = dict(st)))
     except Exception: # pragma: no cover
         # print(e)
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/About.qmd` & `metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/About.qmd`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/_default/refs.bib` & `metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/_default/refs.bib`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/known-datasets.bib` & `metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/known-datasets.bib`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/datasets/known-datasets.json` & `metrics_as_scores-2.7.0/src/metrics_as_scores/datasets/known-datasets.json`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/distribution/distribution.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/distribution/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from nptyping import NDArray, Shape, Float
 from itertools import combinations
 from metrics_as_scores.distribution.fitting import StatisticalTest
 from metrics_as_scores.tools.funcs import cdf_to_ppf
 from metrics_as_scores.distribution.fitting import StatTest_Types
 from statsmodels.distributions import ECDF as SMEcdf
 from statsmodels.stats.multicomp import pairwise_tukeyhsd
-from scipy.stats import gaussian_kde, f_oneway, mode
+from scipy.stats import gaussian_kde, f_oneway, mode, kruskal
 from scipy.integrate import quad
 from scipy.optimize import direct
 from scipy.stats import ks_2samp, ttest_ind
 from scipy.stats._distn_infrastructure import rv_generic, rv_continuous
 from joblib import Parallel, delayed
 from tqdm import tqdm
 from strenum import StrEnum
@@ -801,14 +801,51 @@
         
         if sub_sample is not None and sub_sample < vals.size:
             rng = np.random.default_rng(seed=1_338)
             vals = rng.choice(a=vals, size=sub_sample, replace=False)
         
         return vals
     
+    def num_observations(self) -> Iterable[tuple[str, str, int]]:
+        """
+        Returns the number of observations for each quantity type in each context.
+
+        :rtype: ``Iterable[tuple[str, str, int]]``
+            The first element is the context, the second the quantity type, and the
+            third is the number of observations.
+
+        :return: Returns an iterable generator.
+        """
+        for ctx in self.contexts(include_all_contexts=False):
+            for qtype in self.quantity_types:
+                yield (ctx, qtype, self.data(qtype=qtype, context=ctx, unique_vals=False).shape[0])
+    
+    def has_sufficient_observations(self, raise_if_not: bool=True) -> bool:
+        """
+        Helper method to check whether each quantity type in each context has at least
+        two observations.
+
+        raise_if_not: ``bool``
+            If set to `True`, will raise an exception instead of returning `False` in
+            case there are insufficiently many observations. The exception is more
+            informative as it includes the the context and quantity type.
+        
+        :rtype: ``bool``
+
+        :return: A boolean indicating whether this Dataset has sufficiently many observations
+            for each and every quantity type.
+        """
+        for ctx, qtype, num_obs in self.num_observations():
+            if num_obs < 2:
+                if raise_if_not:
+                    raise Exception(f'The quantity type "{qtype}" in context "{ctx}" has insufficient ({num_obs}) observation(s).')
+                else:
+                    return False
+        return True
+    
     @staticmethod
     def transform(data: NDArray[Shape["*"], Float], dist_transform: DistTransform=DistTransform.NONE, continuous_value: bool=True) -> tuple[float, NDArray[Shape["*"], Float]]:
         r"""
         Transforms a distribution using an ideal value. The resulting data, therefore,
         is a distribution of distances from the designated ideal value.
 
         Given a distribution :math:`X` and an ideal value :math:`i`, the distribution of
@@ -889,21 +926,25 @@
         # Now do the convex transform: Compute the distance to the transform value!
         if transform_value is not None:
             if not continuous_value:
                 transform_value = np.rint(transform_value)
             data = np.abs(data - transform_value)
 
         return (transform_value, data)
+    
 
-
-    def analyze_ANOVA(self, qtypes: Iterable[str], contexts: Iterable[str], unique_vals: bool=True) -> pd.DataFrame:
+    def analyze_groups(self, use: Literal['anova', 'kruskal'], qtypes: Iterable[str], contexts: Iterable[str], unique_vals: bool=True) -> pd.DataFrame:
         """
         For each given type of quantity, this method performs an ANOVA across all
         given contexts.
 
+        use: ``Literal['anova', 'kruskal']``
+            Indicates which method for comparing groups to use. We can either conduct
+            an ANOVA or a Kruskal-Wallis test.
+
         qtypes: ``Iterable[str]``
             An iterable of quantity types to conduct the analysis for. For each given
             type, a separate analysis is performed and the result appended to the
             returned data frame.
         
         contexts: ``Iterable[str]``
             An iterable of contexts across which each of the quantity types shall be
@@ -917,38 +958,46 @@
         :rtype: ``pd.DataFrame``
         
         :return: A data frame with the columns ``qtype`` (name of the quantity type),
             ``stat`` (ANOVA test statistic), ``pval``, and ``across_contexts``, where
             the latter is a semicolon-separated list of contexts the quantity type was
             compared across.
         """
+        use_method: Callable = None
+        if use == 'anova':
+            use_method = f_oneway
+        elif use == 'kruskal':
+            use_method = kruskal
+        else:
+            raise Exception(f'Method "{use}" is not supported.')
+        
 
         # We first have to build the data; f_oneway requires *args, where each
         # arg is a data series.
         if len(list(qtypes)) < 1 or len(list(contexts)) < 2:
             raise Exception('Requires one or quantity types and two or more contexts.')
 
         def anova_for_qtype(qtype: str) -> dict[str, Union[str, str, float]]:
-            data_tuple = ()
+            samples = ()
             for ctx in contexts:
-                data_tuple += (self.data(qtype=qtype, context=None if ctx == '__ALL__' else ctx, unique_vals=unique_vals),)
+                samples += (self.data(qtype=qtype, context=None if ctx == '__ALL__' else ctx, unique_vals=unique_vals),)
             
-            stat, pval = f_oneway(*data_tuple)
+            stat, pval = use_method(*samples)
             return { 'qtype': qtype, 'stat': stat, 'pval': pval, 'across_contexts': ';'.join(contexts) }
 
         res_dicts = Parallel(n_jobs=-1)(delayed(anova_for_qtype)(qtype) for qtype in tqdm(qtypes))
 
         return pd.DataFrame(res_dicts)
     
 
     def analyze_TukeyHSD(self, qtypes: Iterable[str]) -> pd.DataFrame:
         r"""
         Calculate all pairwise comparisons for the given quantity types with Tukey's
         Honest Significance Test (HSD) and return the confidence intervals. For each
-        type of quantity, this method performs all of its associated contexts pair-wise
+        type of quantity, this method performs all of its associated contexts pairwise
         comparisons.
         For example, given a quantity :math:`Q` and its contexts :math:`C_1,C_2,C_3`,
         this method will examine the pairs :math:`\left[\{C_1,C_2\},\{C_1,C_3\},\{C_2,C_3\}\right]`.
         For a single type of quantity, e.g., this test is useful to understand how
         different the quantity manifests across contexts. For multiple quantities, it
         also allows understanding how contexts distinguish from one another, holistically.
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/distribution/fitting.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/distribution/fitting.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/distribution/fitting_problems.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/distribution/fitting_problems.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/pyproject.toml` & `metrics_as_scores-2.7.0/src/metrics_as_scores/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metrics-as-scores"
-version = "2.5.0"
+version = "2.7.0"
 description = "Interactive web application, tool- and analysis suite for approximating, exploring, understanding, and sampling from conditional distributions."
 authors = ["Sebastian Hönel <development@hoenel.net>"]
 license = "Dual-licensed under GNU General Public License v3 (GPLv3) and closed-source"
 readme = "README.md"
 homepage = "https://github.com/mrshoenel/metrics-as-scores"
 repository = "https://github.com/mrshoenel/metrics-as-scores/issues"
 packages = [{include = "metrics_as_scores", from = "src"}]
@@ -33,15 +33,15 @@
 python = ">=3.10, <3.12"
 bokeh = "^2.4.3"
 joblib = "^1.2.0"
 jupyterlab = "^3.4.7"
 matplotlib = "^3.6.0"
 ptvsd = "^4.3.2"
 pymoo = "^0.6.0"
-scipy = "^1.9.1"
+scipy = "1.10.1"
 statsmodels = "^0.13.2"
 StrEnum = "^0.4.8"
 tqdm = "^4.64.1"
 Sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 toml = "^0.10.2"
 rich = "^13.3.1"
@@ -54,15 +54,15 @@
 wget = "^3.2"
 myst-parser = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.1"
 build = "^0.8.0"
-poetry = "^1.2.1"
+poetry = "^1.3.2"
 pytest = "^7.1.3"
 coverage = "^6.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/tools/funcs.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/tools/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,11 +125,11 @@
         if not col_feat in df.columns:
             raise Exception(f'The feature "{col_feat}" is not a column of the given data frame.')
 
     nrow = len(df.index)
     return pd.concat(list([
         pd.DataFrame(dict(
             Feature = nrow * [col_feat],
-            Group = df[group_col],
+            Group = df[group_col].astype(str),
             Value = df[col_feat]
         )) for col_feat in feature_cols
     ])).dropna()
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/tools/lazy.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/tools/lazy.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/app_hooks.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/app_hooks.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/data.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/data.py`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/footer.html` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/footer.html`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 	<ul>
 		<li><b>Controls:</b>
 			<ul>
 				<li><b>Metric Selector:</b> Used to select a single metric for operationalization across the entire corpus and all the various domains. Metrics are grouped into discrete (if discrete, the metric is of integral type) and continuous.</li>
 				<li><b>Distribution Type Selector:</b> This application supports the four principal types <b>PDF</b> (probability density function), <b>CDF</b> (cumulative density function), <b>CCDF [<code>1-CDF</code>]</b> (<i>complementary</i> cumulative distribution function; sometimes also called survival function), and PPF (percent point or quantile function). Furthermore, the application offers different sources for each fitted random variable. These are:
 					<ul>
-						<li><b>Parametric:</b> A total of approximately 100 continuous different distributions were attempted to fit to each metric, in each domain. The best fitting distribution was selected using a two-sample Kolmogorov&mdash;Smirnow test [4]. We even fit continuous distributions to discrete data, but not vice versa.</li>
-						<li><b>Parametric (discrete):</b> For those metrics that are of discrete nature, that is, <i>integral</i>, we also attempt to fit more than approximately 20 discrete distributions and select the best fitting using the Epps&mdash;Singleton two-sample goodness-of-fit test [5].</li>
+						<li><b>Parametric:</b> A total of approximately 100 continuous different distributions were attempted to fit to each metric, in each domain. The best fitting distribution was selected using a one-sample Kolmogorov&mdash;Smirnow test [4]. We even attempt to fit continuous distributions to discrete data, but not vice versa.</li>
+						<li><b>Parametric (discrete):</b> For those metrics that are of discrete nature, that is, <i>integral</i>, we also attempt to fit more than approximately 20 discrete distributions and select the best fitting using the Epps&mdash;Singleton two-sample goodness-of-fit test [5] (the second sample is generated using the PPF of the fitted distribution).</li>
 						<li><b>Kernel Density Estimation:</b> Using a Kernel Density Estimation allows us to estimate a probability density for continuous and discrete metrics. In cases of the (C)CDF derived from KDE fit, we sample a large number inversely from the estimated density, fit a Gaussian KDE, and then obtain an ECDF in order for it to become smooth. This ECDF can be reversed (to become an ECCDF) and inversed (to become an EPPF). The smoothed versions are useful for cases when the actual data is scarce and the ECDFs have large jumps.</li>
 						<li><b>Empirical:</b> While the (C)CDF and EPPF are derived from the data's ECDF, the EPMF is a frequency table over the data. For obtaining exact scores, ECDF and EPMF should be used.</li>
 					</ul>
 				</li>
 				<li><b>Status indicator:</b> Shows "Ready." when the application is ready to be used. Some actions will require a significant amount of processing during which the status will show a throbber and a status text. It may also show errors, if any. For example, selecting a discrete distribution for a continuous metric is an error.</li>
 				<li><b>Transformation Type Selector:</b> Used to select an explicit value to transform the selected metric into a distance from that value, which is context-specific. While the infimum and supremum were taken directly from the data, the expectation (E[X]), median, and mode for continuous metrics were taken from PDFs that were obtained by fitting a Gaussian Kernel on a large individual inverse sample from the original data. This was done to obtain more real-valued data as transformation values are otherwise very similar and repetitive. For discrete metrics, these transformation values were computed ordinarily.</li>
 				<li><b>Own Metric Value / Probability Input:</b> A numeric input field that enables the user to check their own metric value or probability against the currently selected distribution- and transformation type. If no transformation is chosen or transformation using the context's ideal value is disabled, the own metric's value is shown as a vertical line on the plot. Note that when checking a probability against a PPF, the checkbox for applying the selected transform is disabled.</li>
@@ -32,15 +32,15 @@
 		<li><b>Data Table:</b> A table that shows context-specific values (according to each domain).
 			<ul>
 				<li>Domain: The domain/context.</li>
 				<li>Used Transformation Value: If a transformation other than <i>&lt;none&gt;</i> was chosen, this column shows the context-dependent value for the conditional distribution. This value is used to transform the own metric's value into a distance from the transformation value.</li>
 				<li>Metric Value / Metric Distance / Probability: If an own metric value or probability is checked against the corpus, the value is shown here. If a transformation other than <i>&lt;none&gt;</i> is chosen and the checkbox for applying transformations is selected, then the own metric's value is transformed into a distance using each domain's ideal value as <code>abs(ideal - value)</code>. The title of this column will change accordingly.</li>
 				<li>Relative Likelihood / Cumulative Probability / Corresponding Score / Value of Random Variable: Shows the (transformed) own metric's value for each domain or the predicted metric's value for a given probability. For probability densities (PDF), the column name will be "Relative Likelihood". For ECDFs the title will be "Cumulative Probability", for ECCDFs / Scores the title will be "Corresponding Score", and for PPFs the title will be "Value of Random Variable".</li>
 				<li>Parametric Distribution: Shows the name of the best-fitting parametric distribution if the selected type of distribution is a parametric PDF, CDF, or CCDF. Shows <i>&lt;not parametric&gt;</i>, otherwise. Note that in most cases, even with a significance level of <code>alpha=0.001</code>, it was not possible to fit a parametric distribution. In those cases, the value of this column shows <i>&lt;not possible&gt;</i>.</li>
-				<li>Statistic: This is the statistical test's value. For continuous random variables, we compute the two-sample Kolmogorov&mdash;Smirnov goodness-of-fit test [4], and for discrete random variables we use the Epps&mdash;Singleton two-sample goodness-of-fit test [5].</li>
+				<li>Statistic: This is the statistical test's value. For continuous random variables, we compute the one-sample Kolmogorov&mdash;Smirnov goodness-of-fit test [4], and for discrete random variables we use the Epps&mdash;Singleton two-sample goodness-of-fit test [5].</li>
 			</ul>
 		</li>
 		<li><b>Plotting Area:</b> The plot is the main interactive user element of the "Metrics As Scores" web application. It is best utilized using a mouse. Panning the plot can be achieved by using the left mouse button, zooming by using the mouse wheel. By default, x- and y-axis are zoomed simultaneously. The plot features additional controls located on top of the right edge for zooming along the x- or y-axis separately. Each domain in the legend on the right can be (de-)selected. By hovering the plot, a crosshair is shown. It allows to obtain values for relative likelihood, cumulative probability, and scores. The labels for both axes will change accordingly, based on the distribution type and whether a transformation is selected.</li>
 	</ul>
 </div>
 
 <hr/>
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/header.html` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/header.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<h1 style="margin: 0;">Metrics As Scores <small><a href="https://github.com/MrShoenel/metrics-as-scores" target="_blank">https://github.com/MrShoenel/metrics-as-scores</a></small></h1>
+<h1 style="margin: 0;">Metrics As Scores <small><code>v__VERSION__</code>, <a href="https://github.com/MrShoenel/metrics-as-scores" target="_blank">https://github.com/MrShoenel/metrics-as-scores</a></small></h1>
 
 <p>
 	This application was conceived to accompany the paper entitled <i>"Contextual Operationalization of Metrics As Scores: Is My Metric Value Good?"</i> [1].
 	In that paper, the Qualitas.class corpus [2][3] was used to transform metrics into scores.
 	This application, however, supports arbitrary datasets.
 	Head over to the <a href="https://github.com/MrShoenel/metrics-as-scores" target="_blank">repository</a> to find out which datasets are available for download.
 </p>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
-****** Metrics As Scores https://github.com/MrShoenel/metrics-as-scores ******
+****** Metrics As Scores v__VERSION__, https://github.com/MrShoenel/metrics-as-
+scores ******
 This application was conceived to accompany the paper entitled "Contextual
 Operationalization of Metrics As Scores: Is My Metric Value Good?" [1]. In that
 paper, the Qualitas.class corpus [2][3] was used to transform metrics into
 scores. This application, however, supports arbitrary datasets. Head over to
 the repository to find out which datasets are available for download.
 Jump_to_Help.
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/main.py` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     ptvsd.wait_for_attach()
 
 
 import pandas as pd
 import numpy as np
 from pathlib import Path
 from typing import Union
+from metrics_as_scores.__version__ import __version__
 from metrics_as_scores.webapp.exception import PlotException
 from metrics_as_scores.tools.funcs import nonlinspace, natsort
 from metrics_as_scores.distribution.distribution import Empirical, DistTransform, Empirical_discrete, KDE_approx, Parametric, Parametric_discrete, Dataset, LocalDataset
 from bokeh.events import MenuItemClick
 from bokeh.io import curdoc
 from bokeh.layouts import column, row
 from bokeh.models import ColumnDataSource, Dropdown, CheckboxGroup, Button, DataTable, TableColumn
@@ -119,21 +120,27 @@
 
 
 # Set up data
 source = ColumnDataSource(data=pd.DataFrame(columns=list([f'x_{ctx}' for ctx in contexts]) + contexts))
 # Set up plot
 plot = figure(sizing_mode='stretch_width', height=640,
               x_axis_label='Quantity Value', y_axis_label='Corresponding Score',
-              tools="box_zoom,crosshair,hover,pan,wheel_zoom,xwheel_zoom,ywheel_zoom,reset", x_range=[0, 1], y_range=[0 - .02, 1.02], active_scroll='wheel_zoom')
+              tools="box_zoom,crosshair,hover,pan,wheel_zoom,xwheel_zoom,ywheel_zoom,reset",
+              x_range=[0, 1], y_range=[0 - .02, 1.02], active_scroll='wheel_zoom',
+              tooltips=[
+                  ("Group", "$name"),
+                  ("X, Y", "$x, $y")
+              ])
 #plot.toolbar.active_scroll = plot.select_one('wheel_zoom') #'wheel_zoom'
 
 
 
 for idx, ctx in enumerate(contexts):
-    plot.line(f'x_{ctx}', ctx, source=source, line_width=2, line_alpha=1., color=Category20_20[idx], legend_label='[All groups combined]' if ctx == '__ALL__' else ctx)
+    plot.line(name=ctx, x=f'x_{ctx}', y=ctx, source=source, line_width=2, line_alpha=1.,
+              color=Category20_20[idx], legend_label='[All groups combined]' if ctx == '__ALL__' else ctx)
 
 # Also add a vertical line for own quantity
 line_own_source = ColumnDataSource(data=pd.DataFrame(columns=['x', 'y']))
 line_own = plot.line('x', 'y', source=line_own_source, line_alpha=1., color='black', line_width=1.5)
 def update_own_line():
     """ :meta private: """
     val = input_own.value
@@ -565,15 +572,15 @@
 btn_toggle_legend.on_click(btn_toggle_legend_click)
 btn_toggle_table.on_click(btn_toggle_table_click)
 
 
 html_about = web_dir.joinpath('./about.html')
 html_refs = web_dir.joinpath('./references.html')
 header = Div(text=f'''
-    {read_text(this_dir.joinpath('header.html'))}
+    {read_text(this_dir.joinpath('header.html')).replace('__VERSION__', __version__)}
     <h2>Loaded Dataset: <b>{ds.ds["name"]}</b></h2>
     <div id="about">
         <p><b>Author(s)</b>: {', '.join(ds.ds["author"])}</p>
         <div>
             <p><b>Description</b>: {ds.ds["desc"]}</p>
             {read_text(html_about) if html_about.exists() else ""}
         </div>
```

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/metrics-as-scores.nginx.conf`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/metrics-as-scores.service` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/metrics-as-scores.service`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/curve.ico` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/curve.ico`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/curve.png` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/curve.png`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/loading.png` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/loading.png`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/static/styles.css` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/static/styles.css`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/src/metrics_as_scores/webapp/templates/index.html` & `metrics_as_scores-2.7.0/src/metrics_as_scores/webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `metrics_as_scores-2.5.0/PKG-INFO` & `metrics_as_scores-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrics-as-scores
-Version: 2.5.0
+Version: 2.7.0
 Summary: Interactive web application, tool- and analysis suite for approximating, exploring, understanding, and sampling from conditional distributions.
 Home-page: https://github.com/mrshoenel/metrics-as-scores
 License: Dual-licensed under GNU General Public License v3 (GPLv3) and closed-source
 Keywords: distribution fitting,statistical tests,context-dependent,metrics,quality,score
 Author: Sebastian Hönel
 Author-email: development@hoenel.net
 Requires-Python: >=3.10,<3.12
@@ -32,15 +32,15 @@
 Requires-Dist: poethepoet (>=0.18.1,<0.19.0)
 Requires-Dist: ptvsd (>=4.3.2,<5.0.0)
 Requires-Dist: pymoo (>=0.6.0,<0.7.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
-Requires-Dist: scipy (>=1.9.1,<2.0.0)
+Requires-Dist: scipy (==1.10.1)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/mrshoenel/metrics-as-scores/issues
@@ -97,15 +97,15 @@
 ------------------------------------------------------------------------
 
 **Please Note**: ***Metrics As Scores*** (`MAS`) changed considerably
 between versions
 [**`v1.0.8`**](https://github.com/MrShoenel/metrics-as-scores/tree/v1.0.8)
 and **`v2.x.x`**.
 
-The current version is `v2.5.0`.
+The current version is `v2.7.0`.
 
 From version **`v2.x.x`** it has the following new features:
 
 - [Textual User Interface (TUI)](#text-based-user-interface-tui)
 - Proper documentation and testing
 - New version on PyPI. Install the package and run the command line
   interface by typing **`mas`**!
@@ -180,28 +180,30 @@
 
 ## Web Application
 
 Metrics As Scores’ main feature is perhaps the Web Application. It can
 be run directly and locally from the TUI using a selected dataset (you
 may download a known dataset or use your own). The Web Application
 allows to visually inspect each *feature* across all the defined
-*groups*. It feates the PDF/PMF, CDF and CCDF, as well as the PPF for
+*groups*. It features the PDF/PMF, CDF and CCDF, as well as the PPF for
 each feature in each group. It offers five different principal types of
 densities: Parametric, Parametric (discrete), Empirical, Empirical
 (discrete), and (approximate) Kernel Density Estimation. The Web
 Application includes a detailed [Help
 section](https://metrics-as-scores.ml/#help) that should answer most of
 your questions.
 
 ![Metrics As Scores Interactive Web
 .](./WebApp.png "Metrics As Scores Interactive Web Appliction.")
 
 ## Development Setup
 
-This project was developed using and requires Python `>=3.10`. Steps:
+This project was developed using and requires Python `>=3.10`. The
+development documentation can be found at
+<https://mrshoenel.github.io/metrics-as-scores/>. Steps:
 
 1.  Clone the Repository,
 2.  Set up a virtual environment,
 3.  Install packages.
 
 ### Setting Up a Virtual Environment
 
@@ -226,25 +228,28 @@
 ### Installing Packages
 
 The project is managed with `Poetry`. To install the required packages,
 simply run the following.
 
 ``` shell
 venv/Scripts/activate
-# First install Poetry using pip:
-(venv) C:\metrics-as-scores>pip install poetry
+# First, update pip:
+(venv) C:\metrics-as-scores>python -m pip install --upgrade pip
+# First install Poetry v1.3.2 using pip:
+(venv) C:\metrics-as-scores>pip install poetry==1.3.2
 # Install the projects and its dependencies
 (venv) C:\metrics-as-scores> poetry install
 ```
 
 The same in Linux:
 
 ``` shell
 source venv/bin/activate # Linux
-(venv) ubuntu@vm:/tmp/metrics-as-scores$ pip install poetry
+(venv) ubuntu@vm:/tmp/metrics-as-scores$ python -m pip install --upgrade pip
+(venv) ubuntu@vm:/tmp/metrics-as-scores$ pip install poetry==1.3.2
 (venv) ubuntu@vm:/tmp/metrics-as-scores$ poetry install
 ```
 
 ### Running Tests
 
 Tests are run using `poethepoet`:
 
@@ -565,15 +570,15 @@
 
 </div>
 
 <div id="ref-tukey1949anova" class="csl-entry">
 
 Tukey, John W. 1949. “Comparing Individual Means in the Analysis of
 Variance.” *Biometrics* 5 (2): 99–114.
-<http://www.jstor.org/stable/3001913>.
+<https://doi.org/10.2307/3001913>.
 
 </div>
 
 <div id="ref-ggplot2" class="csl-entry">
 
 Wickham, Hadley. 2016. *<span class="nocase">ggplot2</span>: Elegant
 Graphics for Data Analysis*. Springer-Verlag New York.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metrics-as-scores Version: 2.5.0 Summary:
+Metadata-Version: 2.1 Name: metrics-as-scores Version: 2.7.0 Summary:
 Interactive web application, tool- and analysis suite for approximating,
 exploring, understanding, and sampling from conditional distributions. Home-
 page: https://github.com/mrshoenel/metrics-as-scores License: Dual-licensed
 under GNU General Public License v3 (GPLv3) and closed-source Keywords:
 distribution fitting,statistical tests,context-dependent,metrics,quality,score
 Author: Sebastian HÃ¶nel Author-email: development@hoenel.net Requires-Python:
 >=3.10,<3.12 Classifier: Development Status :: 5 - Production/Stable
@@ -18,42 +18,42 @@
 (>=2.4.3,<3.0.0) Requires-Dist: joblib (>=1.2.0,<2.0.0) Requires-Dist:
 jupyterlab (>=3.4.7,<4.0.0) Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: myst-parser (>=1.0.0,<2.0.0) Requires-Dist: nptyping
 (>=2.4.1,<3.0.0) Requires-Dist: poethepoet (>=0.18.1,<0.19.0) Requires-Dist:
 ptvsd (>=4.3.2,<5.0.0) Requires-Dist: pymoo (>=0.6.0,<0.7.0) Requires-Dist:
 pytest-cov (>=4.0.0,<5.0.0) Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0) Requires-Dist: scikit-learn
-(>=1.2.1,<2.0.0) Requires-Dist: scipy (>=1.9.1,<2.0.0) Requires-Dist: sphinx-
-rtd-theme (>=1.1.1,<2.0.0) Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist: toml
-(>=0.10.2,<0.11.0) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Requires-Dist: wget
-(>=3.2,<4.0) Project-URL: Repository, https://github.com/mrshoenel/metrics-as-
-scores/issues Description-Content-Type: text/markdown Metrics As Scores [![DOI]
-(https://zenodo.org/badge/524333119.svg)](https://zenodo.org/badge/latestdoi/
-524333119) [![status](https://joss.theoj.org/papers/
-eb549efe6c0111490395496c68717579/status.svg)](https://joss.theoj.org/papers/
-eb549efe6c0111490395496c68717579) [![codecov](https://codecov.io/github/
-MrShoenel/metrics-as-scores/branch/master/graph/badge.svg?token=HO1GYXVEUQ)]
-(https://codecov.io/github/MrShoenel/metrics-as-scores) ================ - 1
-Usage - 1.1_Text-based_User_Interface_(TUI) - 1.2_Web_Application - 1.3
-Development_Setup - 1.3.1_Setting_Up_a_Virtual_Environment - 1.3.2_Installing
-Packages - 1.3.3_Running_Tests - 2_Example_Usage - 2.1_Concrete_Example_Using
-the_Qualitas.class_Corpus_Dataset - 2.2_Concrete_Example_Using_the_Iris_Dataset
-- 2.3_Diamonds_Example - 3_Datasets - 3.1_Use_Your_Own - 3.2_Known_Datasets - 4
-Personalizing_the_Web_Application - References --------------------------------
----------------------------------------- **Please Note**: ***Metrics As
-Scores*** (`MAS`) changed considerably between versions [**`v1.0.8`**](https://
-github.com/MrShoenel/metrics-as-scores/tree/v1.0.8) and **`v2.x.x`**. The
-current version is `v2.5.0`. From version **`v2.x.x`** it has the following new
-features: - [Textual User Interface (TUI)](#text-based-user-interface-tui) -
-Proper documentation and testing - New version on PyPI. Install the package and
-run the command line interface by typing **`mas`**! [Metrics As Scores Demo.]
-(https://user-images.githubusercontent.com/5049151/219892077-58854478-b761-
-4a3d-9faf-2fe46c122cf5.webm) --------------------------------------------------
----------------------- Contains the data and scripts needed for the application
+(>=1.2.1,<2.0.0) Requires-Dist: scipy (==1.10.1) Requires-Dist: sphinx-rtd-
+theme (>=1.1.1,<2.0.0) Requires-Dist: statsmodels (>=0.13.2,<0.14.0) Requires-
+Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0) Requires-Dist: wget (>=3.2,<4.0) Project-
+URL: Repository, https://github.com/mrshoenel/metrics-as-scores/issues
+Description-Content-Type: text/markdown Metrics As Scores [![DOI](https://
+zenodo.org/badge/524333119.svg)](https://zenodo.org/badge/latestdoi/524333119)
+[![status](https://joss.theoj.org/papers/eb549efe6c0111490395496c68717579/
+status.svg)](https://joss.theoj.org/papers/eb549efe6c0111490395496c68717579) [!
+[codecov](https://codecov.io/github/MrShoenel/metrics-as-scores/branch/master/
+graph/badge.svg?token=HO1GYXVEUQ)](https://codecov.io/github/MrShoenel/metrics-
+as-scores) ================ - 1_Usage - 1.1_Text-based_User_Interface_(TUI) -
+1.2_Web_Application - 1.3_Development_Setup - 1.3.1_Setting_Up_a_Virtual
+Environment - 1.3.2_Installing_Packages - 1.3.3_Running_Tests - 2_Example_Usage
+- 2.1_Concrete_Example_Using_the_Qualitas.class_Corpus_Dataset - 2.2_Concrete
+Example_Using_the_Iris_Dataset - 2.3_Diamonds_Example - 3_Datasets - 3.1_Use
+Your_Own - 3.2_Known_Datasets - 4_Personalizing_the_Web_Application -
+References --------------------------------------------------------------------
+---- **Please Note**: ***Metrics As Scores*** (`MAS`) changed considerably
+between versions [**`v1.0.8`**](https://github.com/MrShoenel/metrics-as-scores/
+tree/v1.0.8) and **`v2.x.x`**. The current version is `v2.7.0`. From version
+**`v2.x.x`** it has the following new features: - [Textual User Interface
+(TUI)](#text-based-user-interface-tui) - Proper documentation and testing - New
+version on PyPI. Install the package and run the command line interface by
+typing **`mas`**! [Metrics As Scores Demo.](https://user-
+images.githubusercontent.com/5049151/219892077-58854478-b761-4a3d-9faf-
+2fe46c122cf5.webm) ------------------------------------------------------------
+------------ Contains the data and scripts needed for the application
 **`Metrics as Scores`**, check out
 metrics-as-scores.ml/>. This package accompanies the paper entitled
 â*Contextual Operationalization of Metrics As Scores: Is My Metric Value
 Good?*â (HÃ¶nel et al. 2022). It seeks to answer the question whether or not
 the domain a software metric was captured in, matters. It enables the user to
 compare domains and to understand their differences. In order to answer the
 question of whether a metric value is actually good, we need to transform it
@@ -85,37 +85,41 @@
 in the [**Web-Application**](#web-application) - Bundle Own dataset so it can
 be published - Run local, interactive Web-Application using a selected dataset
 ![Metrics As Scores Text-based User Interface (TUI).](./TUI.png "Metrics As
 Scores Text-based User Interface (TUI).") ## Web Application Metrics As
 Scoresâ main feature is perhaps the Web Application. It can be run directly
 and locally from the TUI using a selected dataset (you may download a known
 dataset or use your own). The Web Application allows to visually inspect each
-*feature* across all the defined *groups*. It feates the PDF/PMF, CDF and CCDF,
-as well as the PPF for each feature in each group. It offers five different
-principal types of densities: Parametric, Parametric (discrete), Empirical,
-Empirical (discrete), and (approximate) Kernel Density Estimation. The Web
-Application includes a detailed [Help section](https://metrics-as-scores.ml/
-#help) that should answer most of your questions. ![Metrics As Scores
+*feature* across all the defined *groups*. It features the PDF/PMF, CDF and
+CCDF, as well as the PPF for each feature in each group. It offers five
+different principal types of densities: Parametric, Parametric (discrete),
+Empirical, Empirical (discrete), and (approximate) Kernel Density Estimation.
+The Web Application includes a detailed [Help section](https://metrics-as-
+scores.ml/#help) that should answer most of your questions. ![Metrics As Scores
 Interactive Web .](./WebApp.png "Metrics As Scores Interactive Web
 Appliction.") ## Development Setup This project was developed using and
-requires Python `>=3.10`. Steps: 1. Clone the Repository, 2. Set up a virtual
-environment, 3. Install packages. ### Setting Up a Virtual Environment It is
-recommended to use a virtual environment. To use a virtual environment, follow
-these steps (Windows specific; activation of the environment might differ). ```
-shell virtualenv --python=C:/Python310/python.exe venv # Use specific Python
-version for virtual environment venv/Scripts/activate ``` Here is a Linux
-example that assumes you have Python `3.10` installed (this may also require
-installing `python3.10-venv` and/or `python3.10-dev`): ``` shell python3.10 -
-m venv venv source venv/bin/activate # Linux ``` ### Installing Packages The
-project is managed with `Poetry`. To install the required packages, simply run
-the following. ``` shell venv/Scripts/activate # First install Poetry using
-pip: (venv) C:\metrics-as-scores>pip install poetry # Install the projects and
-its dependencies (venv) C:\metrics-as-scores> poetry install ``` The same in
-Linux: ``` shell source venv/bin/activate # Linux (venv) ubuntu@vm:/tmp/
-metrics-as-scores$ pip install poetry (venv) ubuntu@vm:/tmp/metrics-as-scores$
+requires Python `>=3.10`. The development documentation can be found at
+mrshoenel.github.io/metrics-as-scores/>. Steps: 1. Clone the Repository, 2. Set
+up a virtual environment, 3. Install packages. ### Setting Up a Virtual
+Environment It is recommended to use a virtual environment. To use a virtual
+environment, follow these steps (Windows specific; activation of the
+environment might differ). ``` shell virtualenv --python=C:/Python310/
+python.exe venv # Use specific Python version for virtual environment venv/
+Scripts/activate ``` Here is a Linux example that assumes you have Python
+`3.10` installed (this may also require installing `python3.10-venv` and/or
+`python3.10-dev`): ``` shell python3.10 -m venv venv source venv/bin/activate #
+Linux ``` ### Installing Packages The project is managed with `Poetry`. To
+install the required packages, simply run the following. ``` shell venv/
+Scripts/activate # First, update pip: (venv) C:\metrics-as-scores>python -m pip
+install --upgrade pip # First install Poetry v1.3.2 using pip: (venv) C:
+\metrics-as-scores>pip install poetry==1.3.2 # Install the projects and its
+dependencies (venv) C:\metrics-as-scores> poetry install ``` The same in Linux:
+``` shell source venv/bin/activate # Linux (venv) ubuntu@vm:/tmp/metrics-as-
+scores$ python -m pip install --upgrade pip (venv) ubuntu@vm:/tmp/metrics-as-
+scores$ pip install poetry==1.3.2 (venv) ubuntu@vm:/tmp/metrics-as-scores$
 poetry install ``` ### Running Tests Tests are run using `poethepoet`: ```
 shell # Runs the tests and prints coverage (venv) C:\metrics-as-scores>poe test
 ``` You can also generate coverage reports: ``` shell # Writes reports to the
 local directory htmlcov (venv) C:\metrics-as-scores>poe cov ``` ---------------
 --------------------------------------------------------- # Example Usage
 *Metrics As Scores* can be thought of an *interactive*, *multiple-ANOVA*
 analysis and explorer. The analysis of variance (ANOVA; John M. Chambers
@@ -291,11 +295,11 @@
 doi.org/10.1109/APSEC.2010.46>.
 Terra, Ricardo, Luis Fernando Miranda, Marco TÃºlio Valente, and Roberto da
 Silva Bigonha. 2013. âQualitas.class Corpus: A Compiled Version of the
 Qualitas Corpus.â *ACM SIGSOFT Softw. Eng. Notes* 38 (5): 1â4.
 doi.org/10.1145/2507288.2507314>.
 Tukey, John W. 1949. âComparing Individual Means in the Analysis of
 Variance.â *Biometrics* 5 (2): 99â114.
-www.jstor.org/stable/3001913>.
+doi.org/10.2307/3001913>.
 Wickham, Hadley. 2016. *ggplot2: Elegant Graphics for Data Analysis*. Springer-
 Verlag New York.
 ggplot2.tidyverse.org>.
```

