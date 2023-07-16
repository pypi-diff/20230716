# Comparing `tmp/martin_binance-1.3.3.tar.gz` & `tmp/martin-binance-1.3.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin-binance-1.3.4b0.tar", last modified: Sun Jul 16 16:19:54 2023, max compression
```

## Comparing `martin_binance-1.3.3.tar` & `martin-binance-1.3.4b0.tar`

### file list

```diff
@@ -1,27 +1,46 @@
--rw-r--r--   0        0        0     1079 2023-07-04 17:38:43.607429 martin_binance-1.3.3/LICENSE
--rwxr-xr-x   0        0        0     4025 2023-07-04 17:38:43.607429 martin_binance-1.3.3/README.md
--rw-r--r--   0        0        0     2013 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/__init__.py
--rw-r--r--   0        0        0     4642 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2946 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    14575 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6721 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6716 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6722 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4707 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/client.py
--rw-r--r--   0        0        0   186647 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    83215 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16282 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1282 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1427 2023-07-04 17:38:43.663433 martin_binance-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 martin_binance-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.4b0/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.4b0/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.4b0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.4b0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.4b0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.4b0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      950 2023-07-14 16:30:57.253147 martin-binance-1.3.4b0/.github/workflows/docker-image.yml
+-rw-r--r--   0        0        0      910 2023-07-14 16:30:57.253147 martin-binance-1.3.4b0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.4b0/.gitignore
+-rwxr-xr-x   0        0        0    21556 2023-07-16 15:37:30.001288 martin-binance-1.3.4b0/CHANGELOG.md
+-rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.4b0/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.4b0/LICENSE
+-rwxr-xr-x   0        0        0     3948 2023-07-14 16:30:57.257140 martin-binance-1.3.4b0/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.4b0/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.4b0/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.4b0/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.4b0/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.4b0/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.4b0/doc/tmux.png
+-rw-r--r--   0        0        0     2015 2023-07-16 12:56:55.232116 martin-binance-1.3.4b0/martin_binance/__init__.py
+-rw-r--r--   0        0        0     5825 2023-07-16 12:56:55.228119 martin-binance-1.3.4b0/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-07-14 16:30:57.257140 martin-binance-1.3.4b0/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:30:57.257140 martin-binance-1.3.4b0/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14575 2023-07-14 16:30:57.257140 martin-binance-1.3.4b0/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6630 2023-07-16 12:54:32.155177 martin-binance-1.3.4b0/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6625 2023-07-16 12:54:44.083531 martin-binance-1.3.4b0/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6631 2023-07-16 12:54:55.694422 martin-binance-1.3.4b0/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-07-14 16:30:57.261133 martin-binance-1.3.4b0/martin_binance/client.py
+-rw-r--r--   0        0        0   183703 2023-07-16 12:56:55.260095 martin-binance-1.3.4b0/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.4b0/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.4b0/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.4b0/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.4b0/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    82236 2023-07-16 12:56:55.244107 martin-binance-1.3.4b0/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.4b0/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.4b0/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.4b0/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16282 2023-07-14 16:30:57.261133 martin-binance-1.3.4b0/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-07-14 16:30:57.261133 martin-binance-1.3.4b0/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1282 2023-07-14 16:30:57.261133 martin-binance-1.3.4b0/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.4b0/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.4b0/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1401 2023-07-16 16:16:41.075391 martin-binance-1.3.4b0/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-07-16 16:15:46.514693 martin-binance-1.3.4b0/requirements.txt
+-rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.4b0/uml/architecture.puml
+-rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 martin-binance-1.3.4b0/PKG-INFO
```

### Comparing `martin_binance-1.3.3/LICENSE` & `martin-binance-1.3.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/README.md` & `martin-binance-1.3.4b0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-<p align="center"><img src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="250"></p>
+<p align="center"><img src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="200"></p>
 <h3 align="center">Profitable, fault-tolerant, adaptable to the market</h3>
 
 ***
 <h1 align="center">Modified Martingale</h1>
 
 <h2 align="center">Cyclic grid strategy for SPOT market</h2>
 
 <h3 align="center">Free trading system for crypto exchanges (Binance, Bitfinex, Huobi, OKX,)</h3>
 
 <h4 align="center">Other crypto exchanges available through multi-exchange terminal MARGIN https://margin.de</h4>
 
 ***
-<h4 align="center" vertical-align="top">martin-binance <a href="https://badge.fury.io/py/martin-binance"><img style="vertical-align:middle" src="https://badge.fury.io/py/martin-binance.svg" alt="PyPI version" height="20"></a> <--> exchanges-wrapper <a href="https://badge.fury.io/py/exchanges-wrapper"><img style="vertical-align:middle" src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version" height="20"></a></h4>
+<h4 align="center">martin-binance <a href="https://pypi.org/project/martin-binance/"><img align="top" src="https://img.shields.io/pypi/v/martin-binance" alt="PyPI version"></a> <--> exchanges-wrapper <a href="https://pypi.org/project/exchanges-wrapper/"><img align="top" src="https://img.shields.io/pypi/v/exchanges-wrapper" alt="PyPI version"></a></h4>
 
 ***
 <h1 align="center"><a href="https://codeclimate.com/github/DogsTailFarmer/martin-binance/maintainability"><img src="https://api.codeclimate.com/v1/badges/bfa43f47d1c9a385fd8a/maintainability"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/martin-binance/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/martin-binance.svg/?label=resolved+issues&token=ONJLSJHeeBvXyuaAjG1OWUhG"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/martin-binance/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/martin-binance.svg/?label=active+issues&token=ONJLSJHeeBvXyuaAjG1OWUhG"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_martin-binance" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_martin-binance&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/martin-binance" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/martin-binance/month"/></a>
```

### Comparing `martin_binance-1.3.3/martin_binance/__init__.py` & `martin-binance-1.3.4b0/martin_binance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.3"
+__version__ = "1.3.4b0"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 STANDALONE = True
```

### Comparing `martin_binance-1.3.3/martin_binance/backtest/OoTSP.py` & `martin-binance-1.3.4b0/martin_binance/backtest/OoTSP.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Optimization of Trading Strategy Parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.1-2"
+__version__ = "1.3.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 
 from pathlib import Path
 import importlib.util
 from decimal import Decimal
@@ -57,21 +57,21 @@
         inquirer.List(
             "path",
             message="Select from saved: exchange_PAIR with the strategy you want to optimize",
             choices=[f.name for f in BACKTEST_PATH.iterdir() if f.is_dir() and f.name.count('_') == 1],
         ),
         inquirer.List(
             "mode",
-            message="New study session or optimization history plot from saved one",
-            choices=["New", "Plot from saved"],
+            message="New study session or analise from saved one",
+            choices=["New", "Analise saved study session"],
         ),
         inquirer.Text(
             "n_trials",
             message="Enter number of cycles, from 50 to 500",
-            ignore=lambda x: x["mode"] == "Plot from saved",
+            ignore=lambda x: x["mode"] == "Analise saved study session",
             default='150',
             validate=lambda _, c: 10 <= int(c) <= 500,
         ),
     ]
 
     answers = inquirer.prompt(questions, theme=GreenPassion())
 
@@ -87,35 +87,57 @@
         spec = importlib.util.spec_from_file_location("strategy", strategy)
         mbs = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(mbs)
         study = optuna.create_study(study_name=study_name, storage=storage_name, direction="maximize")
         study.optimize(objective, n_trials=int(answers.get('n_trials', '0')))
         print_study_result(study)
         print(f"Study instance saved to {storage_name} for later use")
-    else:
+    elif answers.get('mode') == 'Analise saved study session':
         study = optuna.load_study(study_name=study_name, storage=storage_name)
-    #
-    i_params = print_study_result(study)
-    for index, p in enumerate(i_params.items()):
-        ii_params.append(p[0])
-        if index == 2:
-            break
-    #
-    try:
-        fig = vis.plot_optimization_history(study)
-        fig.show()
-
-        contour_plot = vis.plot_contour(study, params=ii_params)
-        contour_plot.show()
-
-        slice_plot = vis.plot_slice(study, params=ii_params)
-        slice_plot.show()
-    except ImportError:
-        print("Can't find GUI, you can copy study instance to another environment for analyze it")
 
+        while 1:
+
+            questions = [
+                inquirer.List(
+                    "mode",
+                    message="Make a choice",
+                    choices=["Plot from saved", "Get parameters for specific trial", "Exit"],
+                ),
+                inquirer.Text(
+                    "n_trial",
+                    message="Enter the trial number",
+                    ignore=lambda x: x["mode"] in ("Plot from saved", "Exit"),
+                ),
+            ]
+
+            answers = inquirer.prompt(questions, theme=GreenPassion())
+            if answers.get('mode') == 'Plot from saved':
+                i_params = print_study_result(study)
+                for index, p in enumerate(i_params.items()):
+                    ii_params.append(p[0])
+                    if index == 2:
+                        break
+                #
+                try:
+                    fig = vis.plot_optimization_history(study)
+                    fig.show()
+                    contour_plot = vis.plot_contour(study, params=ii_params)
+                    contour_plot.show()
+                    slice_plot = vis.plot_slice(study, params=ii_params)
+                    slice_plot.show()
+                except ImportError:
+                    print("Can't find GUI, you can copy study instance to another environment for analyze it")
+            elif answers.get('mode') == 'Get parameters for specific trial':
+                trial = study.get_trials()[int(answers.get('n_trial', '0'))]
+                print(trial.number)
+                print(trial.state)
+                print(trial.value)
+                print(trial.params)
+            else:
+                break
 
 def print_study_result(study):
     print(f"Optimal parameters: {study.best_params} for get {study.best_value}")
     importance_params = optuna.importance.get_param_importances(study)
     print("Evaluate parameter importance based on completed trials in the given study:")
     for p in importance_params.items():
         print(p)
```

### Comparing `martin_binance-1.3.3/martin_binance/backtest/VCoSEL.py` & `martin-binance-1.3.4b0/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/backtest/exchange_simulator.py` & `martin-binance-1.3.4b0/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/cli_0_BTCUSDT.py.template` & `martin-binance-1.3.4b0/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-2"
+__version__ = "1.3.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
@@ -38,15 +38,14 @@
 ex.ID_EXCHANGE = 0  # See ms_cfg.toml Use for collection of statistics *and get client connection*
 ex.FEE_IN_PAIR = True  # Fee pays in pair
 ex.FEE_MAKER = Decimal('0.0751')  # standard exchange Fee for maker
 ex.FEE_TAKER = Decimal('0.0751')  # standard exchange Fee for taker
 ex.FEE_SECOND = False  # On KRAKEN fee always in second coin
 ex.FEE_BNB_IN_PAIR = False  # Binance fee in BNB and BNB is base asset
 ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
-ex.EXTRA_CHECK_ORDER_STATE = False  # Additional check for filled order(s), for (OKEX, )
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
 ex.AMOUNT_FIRST = Decimal('0.05')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
 ex.PRICE_SHIFT = 0.05  # 'No market' shift price in % from current bid/ask price
 # Round pattern, set pattern 1.0123456789 or if not set used exchange settings
```

### Comparing `martin_binance-1.3.3/martin_binance/cli_1_BTCUSDT.py.template` & `martin-binance-1.3.4b0/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-2"
+__version__ = "1.3.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
@@ -38,15 +38,14 @@
 ex.ID_EXCHANGE = 1  # See ms_cfg.toml Use for collection of statistics *and get client connection*
 ex.FEE_IN_PAIR = True  # Fee pays in pair
 ex.FEE_MAKER = Decimal('0.08')  # standard exchange Fee for maker
 ex.FEE_TAKER = Decimal('0.1')  # standard exchange Fee for taker
 ex.FEE_SECOND = False  # On KRAKEN fee always in second coin
 ex.FEE_BNB_IN_PAIR = False  # Binance fee in BNB and BNB is base asset
 ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
-ex.EXTRA_CHECK_ORDER_STATE = False  # Additional check for filled order(s), for (OKEX, )
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
 ex.AMOUNT_FIRST = Decimal('0.05')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
 ex.PRICE_SHIFT = 0.01  # 'No market' shift price in % from current bid/ask price
 # Round pattern, set pattern 1.0123456789 or if not set used exchange settings
```

### Comparing `martin_binance-1.3.3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin-binance-1.3.4b0/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-2"
+__version__ = "1.3.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
@@ -38,15 +38,14 @@
 ex.ID_EXCHANGE = 2  # See ms_cfg.toml Use for collection of statistics *and get client connection*
 ex.FEE_IN_PAIR = True  # Fee pays in pair
 ex.FEE_MAKER = Decimal('0.1')  # standard exchange Fee for maker
 ex.FEE_TAKER = Decimal('0.17')  # standard exchange Fee for taker
 ex.FEE_SECOND = False  # On KRAKEN fee always in second coin
 ex.FEE_BNB_IN_PAIR = False  # Binance fee in BNB and BNB is base asset
 ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
-ex.EXTRA_CHECK_ORDER_STATE = False  # Additional check for filled order(s), for (OKEX, )
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
 ex.AMOUNT_FIRST = Decimal('0.1')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
 ex.PRICE_SHIFT = 0.01  # 'No market' shift price in % from current bid/ask price
 # Round pattern, set pattern 1.0123456789 or if not set used exchange settings
```

### Comparing `martin_binance-1.3.3/martin_binance/client.py` & `martin-binance-1.3.4b0/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/executor.py` & `martin-binance-1.3.4b0/martin_binance/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.3"
+__version__ = "1.3.4b0"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -45,15 +45,14 @@
 FEE_IN_PAIR = bool()
 FEE_MAKER = Decimal()
 FEE_TAKER = Decimal()
 FEE_SECOND = bool()
 FEE_BNB_IN_PAIR = bool()
 FEE_FTX = bool()
 GRID_MAX_COUNT = int()
-EXTRA_CHECK_ORDER_STATE = bool()
 # Trade parameter
 START_ON_BUY = bool()
 AMOUNT_FIRST = Decimal()
 USE_ALL_FUND = bool()
 AMOUNT_SECOND = Decimal()
 PRICE_SHIFT = float()
 # Round pattern
@@ -583,25 +582,25 @@
         orders = []
         for i in self.orders_list:
             orders.append(i['id'])
         return orders
 
     def get_first(self) -> ():
         """
-        Get Dict[0]  for order
-        :return: (buy, amount, price)
+        Get first order as tuple
+        :return: (id, buy, amount, price)
         """
-        return self.orders_list[0]['buy'], self.orders_list[0]['amount'], self.orders_list[0]['price']
+        return tuple(self.orders_list[0].values())
 
     def get_last(self) -> ():
         """
-        Get Dict[-1]  for order
-        :return: (buy, amount, price)
+        Get last order as tuple
+        :return: (id, buy, amount, price)
         """
-        return self.orders_list[-1]['buy'], self.orders_list[-1]['amount'], self.orders_list[-1]['price']
+        return tuple(self.orders_list[-1].values())
 
     def restore(self, order_list: []):
         self.orders_list.clear()
         for i in order_list:
             i_dec = {'id': i.get('id'),
                      'buy': i.get('buy'),
                      'amount': f2d(i.get('amount')),
@@ -626,14 +625,15 @@
     # strategy control methods
     ##############################################################
     __slots__ = (
         "cycle_buy",
         "orders_grid",
         "orders_init",
         "orders_hold",
+        "orders_save",
         # Take profit variables
         "tp_order_id",
         "tp_wait_id",
         "tp_order",
         "tp_error",
         "tp_order_hold",
         "tp_hold",
@@ -700,19 +700,17 @@
         "reverse_hold",
         "reverse_price",
         "round_base",
         "round_quote",
         "order_q",
         "order_q_placed",
         "martin",
-        "orders_save",
         "first_run",
         "grid_remove",
         "heartbeat_counter",
-        "grid_order_canceled",
         "cycle_status",
         "grid_update_started",
         "start_reverse_time",
         "last_ticker_update",
         "grid_only_restart",
         "local_time",
         "wait_wss_refresh",
@@ -722,14 +720,15 @@
     def __init__(self):
         super().__init__()
         print(f"Init Strategy, ver: {HEAD_VERSION} + {__version__} + {msb_ver}")
         self.cycle_buy = not START_ON_BUY if REVERSE else START_ON_BUY  # + Direction (Buy/Sell) for current cycle
         self.orders_grid = Orders()  # + List of grid orders
         self.orders_init = Orders()  # - List of initial grid orders
         self.orders_hold = Orders()  # + List of grid orders for later place
+        self.orders_save = Orders()  # + Save for the time of cancellation
         # Take profit variables
         self.tp_order_id = None  # + Take profit order id
         self.tp_wait_id = None  # -
         self.tp_order = ()  # - (id, buy, amount, price) Placed take profit order
         self.tp_error = False  # Flag when can't place tp
         self.tp_order_hold = {}  # - Save unreleased take profit order
         self.tp_hold = False  # - Flag for replace take profit order
@@ -796,19 +795,17 @@
         self.reverse_hold = False  # + Exist unreleased reverse state
         self.reverse_price = None  # + Price when execute last grid order and hold reverse cycle
         self.round_base = '1.0123456789'  # - Round pattern for 0.00000 = 0.00
         self.round_quote = '1.0123456789'  # - Round pattern for 0.00000 = 0.00
         self.order_q = None  # + Adaptive order quantity
         self.order_q_placed = False  # - Flag initial number of orders placed
         self.martin = Decimal(0)  # + Operational increment volume of orders in the grid
-        self.orders_save = Orders()  # + Save for cancel time
         self.first_run = True  # -
         self.grid_remove = None  # - Flag when starting cancel grid orders
         self.heartbeat_counter = 0  # -
-        self.grid_order_canceled = None  # -
         self.cycle_status = ()  # - Operational status for current cycle, orders count
         self.grid_update_started = None  # - Flag when grid update process started
         self.start_reverse_time = None  # -
         self.last_ticker_update = 0  # -
         self.grid_only_restart = None  # -
         self.local_time = self.get_time if STANDALONE else time.time
         self.wait_wss_refresh = {}  # -
@@ -902,27 +899,18 @@
                             and not self.reverse_hold
                             and not GRID_ONLY
                             and not self.grid_update_started
                             and not self.start_after_shift
                             and not self.tp_hold
                             and not self.tp_was_filled
                             and not self.orders_init)
-            if (MODE in ('T', 'TC')
-                    and (
-                    stable_state
-                    or (
-                    self.grid_hold.get('timestamp')
-                    and int(self.local_time() - self.grid_hold['timestamp']) > HOLD_TP_ORDER_TIMEOUT
-                    )
-                    or (
-                    self.tp_order_hold.get('timestamp')
-                    and int(self.local_time() - self.tp_order_hold['timestamp']) > HOLD_TP_ORDER_TIMEOUT
-                    )
-                )
-            ):
+            if (MODE in ('T', 'TC') and (stable_state or (self.grid_hold.get('timestamp') and
+                int(self.local_time() - self.grid_hold['timestamp']) > HOLD_TP_ORDER_TIMEOUT) or
+                    (self.tp_order_hold.get('timestamp') and
+                     int(self.local_time() - self.tp_order_hold['timestamp']) > HOLD_TP_ORDER_TIMEOUT))):
                 orders = self.get_buffered_open_orders()
                 order_buy = len([i for i in orders if i.buy is True])
                 order_sell = len([i for i in orders if i.buy is False])
                 order_hold = len(self.orders_hold)
                 cycle_status = (self.cycle_buy, order_buy, order_sell, order_hold)
                 if self.cycle_status != cycle_status:
                     self.cycle_status = cycle_status
@@ -1065,16 +1053,14 @@
                 self.place_grid(self.wait_wss_refresh['buy_side'],
                                 self.wait_wss_refresh['depo'],
                                 self.reverse_target_amount,
                                 self.wait_wss_refresh['allow_grid_shift'],
                                 self.wait_wss_refresh['additional_grid'],
                                 self.wait_wss_refresh['grid_update'])
             self.heartbeat_counter += 1
-            if self.heartbeat_counter % 5 == 0 and not STANDALONE and EXTRA_CHECK_ORDER_STATE:
-                self.check_order_status()
             if (stable_state
                     and ADAPTIVE_TRADE_CONDITION
                     and not self.reverse
                     and not self.part_amount
                     and self.command not in ('stopped', 'stop', 'end')
                     and (self.orders_grid or self.orders_hold)):
                 if self.heartbeat_counter % 150 == 0:
@@ -1160,15 +1146,15 @@
                     'tp_part_amount_first': json.dumps(self.tp_part_amount_first),
                     'tp_part_amount_second': json.dumps(self.tp_part_amount_second),
                     'tp_target': json.dumps(self.tp_target),
                     'tp_order': json.dumps(str(self.tp_order)),
                     'tp_wait_id': json.dumps(self.tp_wait_id)}
         return {}
 
-    def restore_strategy_state(self, strategy_state: Dict[str, str] = None) -> None:
+    def restore_strategy_state(self, strategy_state: Dict[str, str] = None, restore=True) -> None:
         if strategy_state:
             # Restore from file if lose state only
             self.message_log("restore_strategy_state from saved state:", log_level=LogLevel.DEBUG)
             self.message_log("\n".join(f"{k}\t{v}" for k, v in strategy_state.items()), log_level=LogLevel.DEBUG)
             #
             self.command = json.loads(strategy_state.get('command'))
             self.cycle_buy = json.loads(strategy_state.get('cycle_buy'))
@@ -1214,234 +1200,240 @@
             self.tp_part_amount_second = f2d(json.loads(strategy_state.get('tp_part_amount_second')))
             self.tp_target = f2d(json.loads(strategy_state.get('tp_target')))
             self.tp_order = eval(json.loads(strategy_state.get('tp_order')))
             self.tp_wait_id = json.loads(strategy_state.get('tp_wait_id'))
             self.first_run = False
             self.start_after_shift = False if GRID_ONLY and USE_ALL_FUND else self.start_after_shift
         #
-        self.start_process()
-        if self.command == 'stopped':
-            self.message_log("Restore, strategy stopped. Need manual action", tlg=True)
-            return
-        self.avg_rate = f2d(self.get_buffered_ticker().last_price)
-        #
-        open_orders = self.get_buffered_open_orders()
-        tp_order = None
-        # Separate TP order
-        if self.tp_order_id:
-            for i, o in enumerate(open_orders):
-                if o.id == self.tp_order_id:
-                    tp_order = open_orders[i]
-                    del open_orders[i]  # skipcq: PYL-E1138
-                    break
-        # Possible strategy states in compare with saved one
-        grid_orders_len = len(self.orders_grid)
-        open_orders_len = len(open_orders)
-        grid_no_change = grid_orders_len == open_orders_len  # Grid No change
-        grid_less = grid_orders_len > open_orders_len > 0
-        grid_hold = open_orders_len == 0 and self.orders_hold
-        grid_more = grid_orders_len < open_orders_len  # Grid more, some order(s) was placed
-        grid_filled = grid_orders_len > 0 and open_orders_len == 0 and not self.orders_hold and not self.orders_save
-        tp_no_change = (tp_order and self.tp_order_id) or (not tp_order and not self.tp_order_id)
-        tp_placed = tp_order and not self.tp_order_id
-        tp_filled = not tp_order and self.tp_order_id
-        no_orders = grid_orders_len == 0 and not self.tp_order_id
-        #
-        part_amount_first = Decimal('0')
-        part_amount_second = Decimal('0')
-        if grid_filled:
-            for v in self.part_amount.values():
-                part_amount_first += v[0]
-                part_amount_second += v[1]
-        #
-        if STANDALONE or (grid_no_change and tp_no_change):
-            if grid_hold:
-                self.message_log("Restore, no grid orders, place from hold now", tlg=True)
-                self.place_grid_part()
-            elif no_orders:
-                self.restart = True
-                self.message_log("Restore, no orders, restart", tlg=True)
-                self.start()
-            elif not GRID_ONLY and not self.tp_order_id and self.check_min_amount():
-                self.message_log("Restore, replace TP", tlg=True)
-                self.place_profit_order()
-            else:
-                self.message_log("Restore, No difference, go work", tlg=True)
-        elif not STANDALONE:
-            # For MARGINE mode compatibility
-            # Variants are processed when the actual order is equal to or less than it should be
-            # Exotic when dropped during grid placement or unconfirmed TP, left for later
-            if grid_filled and tp_filled:
-                self.message_log("Restore, all grid orders and TP was filled", tlg=True)
-                # Get actual parameter of filled tp order
-                market_order = self.get_buffered_completed_trades(True)
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for o in market_order:
-                    if o.order_id == self.tp_order_id:
-                        amount_first += f2d(o.amount)
-                        amount_second += f2d(o.amount) * f2d(o.price)
-                if amount_first == 0:
-                    # If execution event was missed
-                    _buy, _amount, _price = self.tp_order
-                    amount_first = self.round_truncate(_amount, base=True)
-                    amount_second = self.round_truncate(_amount * _price, base=False)
-                self.tp_was_filled = (amount_first, amount_second, True)
-                self.tp_order_id = None
-                self.tp_order = ()
-                self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
-                # Calculate sum trade amount for both currency
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for i in self.orders_grid:
-                    amount_first += i['amount']
-                    amount_second += i['amount'] * i['price']
-                    print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-                amount_first += part_amount_first
-                amount_second += part_amount_second
-                self.part_amount.clear()
-                print(f"Total grid amount first: {amount_first}, second: {amount_second}")
-                # Clear list of grid order
-                self.orders_grid.orders_list.clear()
-                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-
-            elif grid_filled and tp_no_change:
-                self.message_log('Restore, No grid orders -> Reverse', tlg=True)
-                self.shift_grid_threshold = None
-                # Admit that missing orders were executed on conditions no worse than those saved
-                # Calculate sum trade amount for both currency
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for i in self.orders_grid:
-                    amount_first += i['amount']
-                    amount_second += i['amount'] * i['price']
-                    print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-                amount_first += part_amount_first
-                amount_second += part_amount_second
-                self.part_amount.clear()
-                print(f"Total amount first: {amount_first}, second: {amount_second}")
-                # Clear list of grid order
-                self.orders_grid.orders_list.clear()
-                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-
-            elif grid_less and tp_filled:
-                self.message_log("Restore, some grid orders and TP was filled", tlg=True)
-                # Get actual parameter of filled tp order
-                market_order = self.get_buffered_completed_trades(True)
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for o in market_order:
-                    if o.order_id == self.tp_order_id:
-                        amount_first += f2d(o.amount)
-                        amount_second += f2d(o.amount) * f2d(o.price)
-                        print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
-                if amount_first == 0:
-                    # If execution event was missed
-                    _buy, _amount, _price = self.tp_order
-                    amount_first = self.round_truncate(f2d(_amount), base=True)
-                    amount_second = self.round_truncate(f2d(_amount * _price), base=False)
-                self.tp_was_filled = (amount_first, amount_second, True)
-                self.tp_order_id = None
-                self.tp_order = ()
-                self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
-                # Calculate sum trade amount for both currency
-                exch_orders_id = []
-                save_orders_id = []
-                for i in open_orders:
-                    exch_orders_id.append(i.id)
-                for i in self.orders_grid:
-                    save_orders_id.append(i.get('id'))
-                print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
-                print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
-                diff_id = list(set(save_orders_id).difference(exch_orders_id))
-                print(f"Executed order id is: {diff_id}")
-                # Calculate sum trade amount for both currency
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for i in self.orders_grid:
-                    if i['id'] in diff_id:
+        if restore:
+            self.start_process()
+            if self.command == 'stopped':
+                self.message_log("Restore, strategy stopped. Need manual action", tlg=True)
+                return
+            self.avg_rate = f2d(self.get_buffered_ticker().last_price)
+            #
+            open_orders = self.get_buffered_open_orders()
+            tp_order = None
+            # Separate TP order
+            if self.tp_order_id:
+                for i, o in enumerate(open_orders):
+                    if o.id == self.tp_order_id:
+                        tp_order = open_orders[i]
+                        del open_orders[i]  # skipcq: PYL-E1138
+                        break
+            # Possible strategy states in compare with saved one
+            grid_orders_len = len(self.orders_grid)
+            open_orders_len = len(open_orders)
+            grid_no_change = grid_orders_len == open_orders_len  # Grid No change
+            grid_less = grid_orders_len > open_orders_len > 0
+            grid_hold = open_orders_len == 0 and self.orders_hold
+            grid_more = grid_orders_len < open_orders_len  # Grid more, some order(s) was placed
+            grid_filled = grid_orders_len > 0 and open_orders_len == 0 and not self.orders_hold and not self.orders_save
+            tp_no_change = (tp_order and self.tp_order_id) or (not tp_order and not self.tp_order_id)
+            tp_placed = tp_order and not self.tp_order_id
+            tp_filled = not tp_order and self.tp_order_id
+            no_orders = grid_orders_len == 0 and not self.tp_order_id
+            #
+            part_amount_first = Decimal('0')
+            part_amount_second = Decimal('0')
+            if grid_filled:
+                for v in self.part_amount.values():
+                    part_amount_first += v[0]
+                    part_amount_second += v[1]
+            #
+            if STANDALONE or (grid_no_change and tp_no_change):
+                if grid_hold:
+                    self.message_log("Restore, no grid orders, place from hold now", tlg=True)
+                    self.place_grid_part()
+                elif no_orders:
+                    self.restart = True
+                    self.message_log("Restore, no orders, restart", tlg=True)
+                    self.start()
+                elif not GRID_ONLY and not self.tp_order_id and self.check_min_amount():
+                    self.message_log("Restore, replace TP", tlg=True)
+                    self.place_profit_order()
+                else:
+                    self.message_log("Restore, No difference, go work", tlg=True)
+            elif not STANDALONE:
+                # For MARGINE mode compatibility
+                # Variants are processed when the actual order is equal to or less than it should be
+                # Exotic when dropped during grid placement or unconfirmed TP, left for later
+                if grid_filled and tp_filled:
+                    self.message_log("Restore, all grid orders and TP was filled", tlg=True)
+                    # Get actual parameter of filled tp order
+                    market_order = self.get_buffered_completed_trades(True)
+                    amount_first = Decimal('0')
+                    amount_second = Decimal('0')
+                    for o in market_order:
+                        if o.order_id == self.tp_order_id:
+                            amount_first += f2d(o.amount)
+                            amount_second += f2d(o.amount) * f2d(o.price)
+                    if amount_first == 0:
+                        # If execution event was missed
+                        _buy, _amount, _price = self.tp_order
+                        amount_first = self.round_truncate(_amount, base=True)
+                        amount_second = self.round_truncate(_amount * _price, base=False)
+                    self.tp_was_filled = (amount_first, amount_second, True)
+                    self.tp_order_id = None
+                    self.tp_order = ()
+                    self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}",
+                                     log_level=LogLevel.DEBUG)
+                    # Calculate sum trade amount for both currency
+                    amount_first = Decimal('0')
+                    amount_second = Decimal('0')
+                    for i in self.orders_grid:
                         amount_first += i['amount']
                         amount_second += i['amount'] * i['price']
                         print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-                        part_amount_first, part_amount_second = self.part_amount.pop(i['id'], (Decimal('0'), Decimal('0')))
-                amount_first += part_amount_first
-                amount_second += part_amount_second
-                self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}", color=Style.B_WHITE)
-                # Remove from list of grid order
-                for i in diff_id:
-                    self.orders_grid.remove(i)
-                # Calculate trade amount with Fee
-                amount_first_fee, amount_second_fee = self.fee_for_grid(amount_first, amount_second)
-                # Calculate cycle sum trading for both currency
-                self.sum_amount_first += amount_first_fee
-                self.sum_amount_second += amount_second_fee
-                if open_orders_len == 0 and self.orders_hold:
-                    self.place_grid_part()
-                self.after_filled_tp(one_else_grid=True)
+                    amount_first += part_amount_first
+                    amount_second += part_amount_second
+                    self.part_amount.clear()
+                    print(f"Total grid amount first: {amount_first}, second: {amount_second}")
+                    # Clear list of grid order
+                    self.orders_grid.orders_list.clear()
+                    self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
 
-            elif grid_less:
-                self.message_log("Restore, Less grid orders -> replace tp order", tlg=True)
-                self.shift_grid_threshold = None
-                exch_orders_id = []
-                save_orders_id = []
-                for i in open_orders:
-                    exch_orders_id.append(i.id)
-                for i in self.orders_grid:
-                    save_orders_id.append(i.get('id'))
-                print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
-                print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
-                diff_id = list(set(save_orders_id).difference(exch_orders_id))
-                print(f"Executed order id is: {diff_id}")
-                # Calculate sum trade amount for both currency
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for i in self.orders_grid:
-                    if i['id'] in diff_id:
+                elif grid_filled and tp_no_change:
+                    self.message_log('Restore, No grid orders -> Reverse', tlg=True)
+                    self.shift_grid_threshold = None
+                    # Admit that missing orders were executed on conditions no worse than those saved
+                    # Calculate sum trade amount for both currency
+                    amount_first = Decimal('0')
+                    amount_second = Decimal('0')
+                    for i in self.orders_grid:
                         amount_first += i['amount']
                         amount_second += i['amount'] * i['price']
                         print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
-                        part_amount_first, part_amount_second = self.part_amount.pop(i['id'], (Decimal('0'), Decimal('0')))
-                amount_first += part_amount_first
-                amount_second += part_amount_second
-                self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}", color=Style.B_WHITE)
-                # Remove from list of grid order
-                for i in diff_id:
-                    self.orders_grid.remove(i)
-                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-
-            elif tp_filled:
-                self.message_log('Restore, TP order was filled -> Restart', tlg=True)
-                # Get actual parameter of filled tp order
-                market_order = self.get_buffered_completed_trades(True)
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for o in market_order:
-                    if o.order_id == self.tp_order_id:
-                        amount_first += f2d(o.amount)
-                        amount_second += f2d(o.amount) * f2d(o.price)
-                        print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
-                if amount_first == 0:
-                    # If execution event was missed
-                    _buy, _amount, _price = self.tp_order
-                    amount_first = self.round_truncate(f2d(_amount), base=True)
-                    amount_second = self.round_truncate(f2d(_amount * _price), base=False)
-                self.tp_was_filled = (amount_first, amount_second, True)
-                self.tp_order_id = None
-                self.tp_order = ()
-                self.grid_remove = True
-                self.cancel_grid(cancel_all=True)
+                    amount_first += part_amount_first
+                    amount_second += part_amount_second
+                    self.part_amount.clear()
+                    print(f"Total amount first: {amount_first}, second: {amount_second}")
+                    # Clear list of grid order
+                    self.orders_grid.orders_list.clear()
+                    self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
+
+                elif grid_less and tp_filled:
+                    self.message_log("Restore, some grid orders and TP was filled", tlg=True)
+                    # Get actual parameter of filled tp order
+                    market_order = self.get_buffered_completed_trades(True)
+                    amount_first = Decimal('0')
+                    amount_second = Decimal('0')
+                    for o in market_order:
+                        if o.order_id == self.tp_order_id:
+                            amount_first += f2d(o.amount)
+                            amount_second += f2d(o.amount) * f2d(o.price)
+                            print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
+                    if amount_first == 0:
+                        # If execution event was missed
+                        _buy, _amount, _price = self.tp_order
+                        amount_first = self.round_truncate(f2d(_amount), base=True)
+                        amount_second = self.round_truncate(f2d(_amount * _price), base=False)
+                    self.tp_was_filled = (amount_first, amount_second, True)
+                    self.tp_order_id = None
+                    self.tp_order = ()
+                    self.message_log(f"restore_strategy_state.was_filled_tp: {self.tp_was_filled}",
+                                     log_level=LogLevel.DEBUG)
+                    # Calculate sum trade amount for both currency
+                    exch_orders_id = []
+                    save_orders_id = []
+                    for i in open_orders:
+                        exch_orders_id.append(i.id)
+                    for i in self.orders_grid:
+                        save_orders_id.append(i.get('id'))
+                    print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
+                    print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
+                    diff_id = list(set(save_orders_id).difference(exch_orders_id))
+                    print(f"Executed order id is: {diff_id}")
+                    # Calculate sum trade amount for both currency
+                    amount_first = Decimal('0')
+                    amount_second = Decimal('0')
+                    for i in self.orders_grid:
+                        if i['id'] in diff_id:
+                            amount_first += i['amount']
+                            amount_second += i['amount'] * i['price']
+                            print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
+                            part_amount_first, part_amount_second = self.part_amount.pop(i['id'],
+                                                                                         (Decimal('0'), Decimal('0')))
+                    amount_first += part_amount_first
+                    amount_second += part_amount_second
+                    self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}",
+                                     color=Style.B_WHITE)
+                    # Remove from list of grid order
+                    for i in diff_id:
+                        self.orders_grid.remove(i)
+                    # Calculate trade amount with Fee
+                    amount_first_fee, amount_second_fee = self.fee_for_grid(amount_first, amount_second)
+                    # Calculate cycle sum trading for both currency
+                    self.sum_amount_first += amount_first_fee
+                    self.sum_amount_second += amount_second_fee
+                    if open_orders_len == 0 and self.orders_hold:
+                        self.place_grid_part()
+                    self.after_filled_tp(one_else_grid=True)
 
-            elif grid_more and self.orders_init:
-                self.message_log('Restored, some grid order(s) was placed', tlg=True)
+                elif grid_less:
+                    self.message_log("Restore, Less grid orders -> replace tp order", tlg=True)
+                    self.shift_grid_threshold = None
+                    exch_orders_id = []
+                    save_orders_id = []
+                    for i in open_orders:
+                        exch_orders_id.append(i.id)
+                    for i in self.orders_grid:
+                        save_orders_id.append(i.get('id'))
+                    print(f"restore_strategy_state.exch_orders_id: {exch_orders_id}")
+                    print(f"restore_strategy_state.save_orders_id: {save_orders_id}")
+                    diff_id = list(set(save_orders_id).difference(exch_orders_id))
+                    print(f"Executed order id is: {diff_id}")
+                    # Calculate sum trade amount for both currency
+                    amount_first = Decimal('0')
+                    amount_second = Decimal('0')
+                    for i in self.orders_grid:
+                        if i['id'] in diff_id:
+                            amount_first += i['amount']
+                            amount_second += i['amount'] * i['price']
+                            print(f"id={i['id']}, first: {i['amount']}, price: {i['price']}")
+                            part_amount_first, part_amount_second = self.part_amount.pop(i['id'],
+                                                                                         (Decimal('0'), Decimal('0')))
+                    amount_first += part_amount_first
+                    amount_second += part_amount_second
+                    self.message_log(f"Total amount first: {amount_first:f}, second: {amount_second:f}",
+                                     color=Style.B_WHITE)
+                    # Remove from list of grid order
+                    for i in diff_id:
+                        self.orders_grid.remove(i)
+                    self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
+
+                elif tp_filled:
+                    self.message_log('Restore, TP order was filled -> Restart', tlg=True)
+                    # Get actual parameter of filled tp order
+                    market_order = self.get_buffered_completed_trades(True)
+                    amount_first = Decimal('0')
+                    amount_second = Decimal('0')
+                    for o in market_order:
+                        if o.order_id == self.tp_order_id:
+                            amount_first += f2d(o.amount)
+                            amount_second += f2d(o.amount) * f2d(o.price)
+                            print(f"order_id={o.order_id}, first: {o.amount}, price: {o.price}")
+                    if amount_first == 0:
+                        # If execution event was missed
+                        _buy, _amount, _price = self.tp_order
+                        amount_first = self.round_truncate(f2d(_amount), base=True)
+                        amount_second = self.round_truncate(f2d(_amount * _price), base=False)
+                    self.tp_was_filled = (amount_first, amount_second, True)
+                    self.tp_order_id = None
+                    self.tp_order = ()
+                    self.cancel_grid(cancel_all=True)
 
-            elif tp_placed:
-                self.message_log('Restored, take profit order(s) was placed', tlg=True)
+                elif grid_more and self.orders_init:
+                    self.message_log('Restored, some grid order(s) was placed', tlg=True)
 
-            else:
-                self.message_log('Restored', tlg=True)
+                elif tp_placed:
+                    self.message_log('Restored, take profit order(s) was placed', tlg=True)
+
+                else:
+                    self.message_log('Restored', tlg=True)
 
     def start(self, profit_f: Decimal = f2d(0), profit_s: Decimal = f2d(0)) -> None:
         self.message_log('Start')
         if self.command == 'stopped':
             self.message_log('Strategy stopped, waiting manual action')
             return
         # Cancel take profit order in all state
@@ -1450,15 +1442,15 @@
         self.tp_was_filled = ()
         self.order_q_placed = False
         self.grid_place_flag = False
         if self.tp_order_id:
             self.tp_cancel = True
             if not self.cancel_order_id:
                 self.cancel_order_id = self.tp_order_id
-                self.cancel_order(self.tp_order_id)
+                self.cancel_order_exp(self.tp_order_id)
             return
         if self.tp_wait_id:
             # Wait tp order and cancel in on_cancel_order_success and restart
             self.tp_cancel = True
             return
         ff, fs, _, _ = self.get_free_assets(mode='available')
         # Save initial funds and cycle statistics to .db for external analytics
@@ -1699,14 +1691,41 @@
         if MODE in ('T', 'TC'):
             write_log(log_level, msg)
             if tlg and self.queue_to_tlg:
                 msg = self.tlg_header + msg
                 self.status_time = self.local_time()
                 self.queue_to_tlg.put(msg)
 
+    def start_process(self):
+        # Init analytic
+        self.connection_analytic = self.connection_analytic or sqlite3.connect(DB_FILE,
+                                                                               check_same_thread=False,
+                                                                               timeout=10)
+        # Create processes for save to .db and send Telegram message
+        self.pr_db = Thread(target=save_to_db, args=(self.queue_to_db,))
+        self.pr_tlg = Thread(target=telegram, args=(self.queue_to_tlg, self.tlg_header.split('.')[0],))
+        if not self.pr_db.is_alive():
+            self.message_log('Start process for .db save')
+            try:
+                self.pr_db.start()
+            except AssertionError as error:
+                self.message_log(str(error), log_level=LogLevel.ERROR, color=Style.B_RED)
+        if not self.pr_tlg.is_alive():
+            self.message_log('Start process for Telegram')
+            try:
+                self.pr_tlg.start()
+            except AssertionError as error:
+                self.message_log(str(error), log_level=LogLevel.ERROR, color=Style.B_RED)
+
+    def cancel_order_exp(self, order_id: int, cancel_all=False) -> None:
+        if STANDALONE:
+            self.cancel_order(order_id, cancel_all=cancel_all)
+        else:
+            self.cancel_order(order_id)
+
     ##############################################################
     # Technical analysis
     ##############################################################
 
     def atr(self, interval: int = 14):
         """
         Average True Range
@@ -1864,15 +1883,15 @@
             _fs = funds.get(self.s_currency, 0)
             ff = Decimal('0')
             fs = Decimal('0')
             if _ff and _fs:
                 if mode == 'total':
                     ff = f2d(_ff.total_for_currency)
                     fs = f2d(_fs.total_for_currency)
-                elif mode == 'available':
+                elif mode in ('available', 'free'):
                     ff = f2d(_ff.available)
                     fs = f2d(_fs.available)
                 elif mode == 'reserved':
                     ff = f2d(_ff.reserved)
                     fs = f2d(_fs.reserved)
         #
         if mode == 'free':
@@ -1886,15 +1905,15 @@
                     fs = self.initial_reverse_second if self.reverse else self.initial_second
         ff = self.round_truncate(ff, base=True)
         fs = self.round_truncate(fs, base=False)
         ft = ff * self.avg_rate + fs
         assets = f"{mode.capitalize()}: First: {ff}, Second: {fs}"
         return ff, fs, ft, assets
 
-    def round_truncate(self, _x: Decimal, base: bool, fee: bool = False, _rounding=ROUND_FLOOR) -> Decimal:
+    def round_truncate(self, _x: Decimal, base: bool = None, fee=False, _rounding=ROUND_FLOOR) -> Decimal:
         if fee:
             round_pattern = "1.01234567"
         else:
             round_pattern = self.round_base if base else self.round_quote
         xr = _x.quantize(Decimal(round_pattern), rounding=_rounding)
         return xr
 
@@ -2169,17 +2188,17 @@
         try:
             bb = self.bollinger_band(BB_CANDLE_SIZE_IN_MINUTES, BB_NUMBER_OF_CANDLES)
         except Exception as ex:
             self.message_log(f"Can't get BB in grid update: {ex}", log_level=LogLevel.INFO)
         else:
             do_it = False
             if self.orders_hold:
-                last_price = float(self.orders_hold.get_last()[2])
+                last_price = float(self.orders_hold.get_last()[3])
             else:
-                last_price = float(self.orders_grid.get_last()[2])
+                last_price = float(self.orders_grid.get_last()[3])
             predicted_price = bb.get('bbb') if self.cycle_buy else bb.get('tbb')
             if self.cycle_buy:
                 delta = 100 * (last_price - predicted_price) / last_price
             else:
                 delta = 100 * (predicted_price - last_price) / last_price
             depo_remaining = ((self.orders_grid.sum_amount(self.cycle_buy) +
                                self.orders_hold.sum_amount(self.cycle_buy)) /
@@ -2208,15 +2227,15 @@
                 # Waiting confirm or cancel old or processing ending and replace it
                 self.tp_hold = True
                 self.message_log('Waiting finished TP order for replace', color=Style.B_WHITE)
             elif self.tp_order_id:
                 # Cancel take profit order, place new
                 self.tp_hold = True
                 self.cancel_order_id = self.tp_order_id
-                self.cancel_order(self.tp_order_id)
+                self.cancel_order_exp(self.tp_order_id)
                 self.message_log('Hold take profit order, replace existing', color=Style.B_WHITE)
             else:
                 buy_side = not self.cycle_buy
                 # Calculate take profit order
                 tp = self.calc_profit_order(buy_side, by_market=by_market)
                 price = tp.get('price')
                 amount = tp.get('amount')
@@ -2459,35 +2478,14 @@
                 self.message_log("Can't calculate over price for reverse cycle,"
                                  " use previous or over_price_coarse * 3", log_level=LogLevel.ERROR)
                 over_price = over_price_previous or 3 * over_price_coarse
         else:
             over_price = over_price_coarse
         return over_price
 
-    def start_process(self):
-        # Init analytic
-        self.connection_analytic = self.connection_analytic or sqlite3.connect(DB_FILE,
-                                                                               check_same_thread=False,
-                                                                               timeout=10)
-        # Create processes for save to .db and send Telegram message
-        self.pr_db = Thread(target=save_to_db, args=(self.queue_to_db,))
-        self.pr_tlg = Thread(target=telegram, args=(self.queue_to_tlg, self.tlg_header.split('.')[0],))
-        if not self.pr_db.is_alive():
-            self.message_log('Start process for .db save')
-            try:
-                self.pr_db.start()
-            except AssertionError as error:
-                self.message_log(str(error), log_level=LogLevel.ERROR, color=Style.B_RED)
-        if not self.pr_tlg.is_alive():
-            self.message_log('Start process for Telegram')
-            try:
-                self.pr_tlg.start()
-            except AssertionError as error:
-                self.message_log(str(error), log_level=LogLevel.ERROR, color=Style.B_RED)
-
     def fee_for_grid(self,
                      amount_first: Decimal,
                      amount_second: Decimal,
                      by_market: bool = False,
                      print_info: bool = True) -> (Decimal, Decimal):
         """
         Calculate trade amount with Fee for grid order for both currency
@@ -2511,15 +2509,15 @@
                         amount_first -= self.round_fee(fee, amount_first, base=True)
                         message = f"For grid order First - fee: {amount_first}"
                 else:
                     amount_second -= self.round_fee(fee, amount_second, base=False)
                     message = f"For grid order Second - fee: {amount_second}"
         if print_info and message:
             self.message_log(message, log_level=LogLevel.DEBUG)
-        return self.round_truncate(amount_first, base=True), self.round_truncate(amount_second, base=False)
+        return self.round_truncate(amount_first, fee=True), self.round_truncate(amount_second, fee=True)
 
     def fee_for_tp(self,
                    amount_first: Decimal,
                    amount_second: Decimal,
                    by_market=False,
                    log_output=True) -> (Decimal, Decimal):
         """
@@ -2543,15 +2541,15 @@
                         amount_second += self.round_fee(fee, amount_second, base=False)
                         log_text = f"Take profit order Second + fee: {amount_second}"
                     else:
                         amount_first -= self.round_fee(fee, amount_first, base=True)
                         log_text = f"Take profit order First - fee: {amount_first}"
             if log_output:
                 self.message_log(log_text, log_level=LogLevel.DEBUG)
-        return self.round_truncate(amount_first, base=True), self.round_truncate(amount_second, base=False)
+        return self.round_truncate(amount_first, fee=True), self.round_truncate(amount_second, fee=True)
 
     def after_filled_tp(self, one_else_grid: bool = False):
         """
         After filling take profit order calculate profit, deposit and restart or place additional TP
         """
         # noinspection PyTupleAssignmentBalance
         amount_first, amount_second, by_market = self.tp_was_filled  # skipcq: PYL-W0632
@@ -2844,15 +2842,15 @@
         no_grid = not self.orders_grid and not self.orders_hold and not self.orders_init
         if no_grid and not self.orders_save:
             if self.tp_order_id:
                 self.tp_hold = False
                 self.tp_cancel_from_grid_handler = True
                 if not self.cancel_order_id:
                     self.cancel_order_id = self.tp_order_id
-                    self.cancel_order(self.tp_order_id)
+                    self.cancel_order_exp(self.tp_order_id)
                 return
             if self.tp_wait_id:
                 # Wait tp order and cancel in on_cancel_order_success and restart
                 self.tp_cancel_from_grid_handler = True
                 return
             if GRID_ONLY:
                 self.shift_grid_threshold = None
@@ -2916,25 +2914,24 @@
                 self.message_log("grid_handler: Was filled TP and all grid orders, converse TP to grid", tlg=True)
                 self.after_filled_tp(one_else_grid=True)
             else:
                 # Ended grid order, calculate depo and Reverse
                 self.reverse_after_grid_ending()
         else:
             if self.orders_save:
-                self.grid_remove = False if self.grid_order_canceled else None
                 self.start_hold = False
                 self.message_log("grid_handler: Restore deleted and unplaced grid orders")
                 self.orders_hold.orders_list.extend(self.orders_save)
                 # Sort restored hold orders
                 self.orders_hold.sort(self.cycle_buy)
                 self.orders_save.orders_list.clear()
                 self.order_q_placed = False
             if after_full_fill and self.orders_hold and self.order_q_placed:
                 # PLace one hold grid order and remove it from hold list
-                _buy, _amount, _price = self.orders_hold.get_first()
+                _, _buy, _amount, _price = self.orders_hold.get_first()
                 check = (len(self.orders_grid) + len(self.orders_hold)) <= 2
                 waiting_order_id = self.place_limit_order_check(_buy, _amount, _price, check=check)
                 self.orders_init.append(waiting_order_id, _buy, _amount, _price)
                 del self.orders_hold.orders_list[0]
             # Exist filled but non processing TP
             if self.tp_was_filled:
                 self.after_filled_tp(one_else_grid=True)
@@ -2955,27 +2952,23 @@
                 self.orders_hold.orders_list.clear()
             if self.orders_init:
                 # Exist not accepted grid order(s), wait msg from exchange
                 self.start_hold = True
             elif self.orders_grid:
                 # Sequential removal orders from grid and make this 'atomic'
                 # - on_cancel_order_success: save canceled order to orders_save
-                _id = self.orders_grid.orders_list[0]['id']
+                _id, _, _, _ = self.orders_grid.get_first()
                 self.message_log(f"cancel_grid order: {_id}", log_level=LogLevel.DEBUG)
-                self.grid_order_canceled = _id
-                if cancel_all and STANDALONE and MODE in ('T', 'TC'):
-                    self.cancel_all_order(_id)
-                else:
-                    self.cancel_order(_id)
+                self.cancel_order_exp(_id, cancel_all=cancel_all)
             elif self.grid_remove:
                 self.message_log("cancel_grid: Ended", log_level=LogLevel.DEBUG)
-                self.grid_remove = None
-                self.order_q_placed = None
                 sum_amount = self.orders_save.sum_amount(self.cycle_buy) if self.grid_update_started else Decimal('0.0')
                 self.orders_save.orders_list.clear()
+                self.grid_remove = None
+                self.order_q_placed = None
                 if self.tp_was_filled:
                     self.grid_update_started = None
                     self.after_filled_tp(one_else_grid=False)
                 elif self.grid_update_started:
                     self.message_log(f"Start update grid orders, depo: {sum_amount}", log_level=LogLevel.DEBUG)
                     self.place_grid(self.cycle_buy,
                                     sum_amount,
@@ -2984,49 +2977,14 @@
                                     grid_update=True)
                 else:
                     self.grid_update_started = None
                     self.start()
         else:
             self.grid_remove = None
 
-    def check_order_status(self):
-        market_orders = self.get_buffered_open_orders()
-        market_orders_id = []
-        for order in market_orders:
-            market_orders_id.append(order.id)
-        strategy_orders_id = self.orders_grid.get_id_list()
-        if self.tp_order_id and not self.cancel_order_id:
-            strategy_orders_id.append(self.tp_order_id)
-        if self.grid_order_canceled in strategy_orders_id:
-            strategy_orders_id.remove(self.grid_order_canceled)
-        diff_id = list(set(strategy_orders_id).difference(market_orders_id))
-        if diff_id:
-            self.message_log(f"Orders not present on exchange: {diff_id}", tlg=True)
-            if diff_id.count(self.tp_order_id):
-                diff_id.remove(self.tp_order_id)
-                amount_first = self.tp_order[1]
-                amount_second = self.tp_order[1] * self.tp_order[2]
-                self.tp_was_filled = (amount_first, amount_second, True)
-                self.tp_order_id = None
-                self.tp_order = ()
-                self.message_log(f"Was filled TP: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
-            if diff_id:
-                self.shift_grid_threshold = None
-                amount_first = Decimal('0')
-                amount_second = Decimal('0')
-                for _id in diff_id:
-                    _buy, _amount, _price = self.orders_grid.get_by_id(_id)
-                    self.orders_grid.remove(_id)
-                    amount_first += _amount
-                    amount_second += _amount * _price
-                self.message_log(f"Grid amount: First: {amount_first}, Second: {amount_second}")
-                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-            elif self.tp_was_filled:
-                self.cancel_grid()
-
     def check_min_amount(self, for_tp=True) -> bool:
         res = False
         if self.avg_rate:
             tcm = self.get_trading_capability_manager()
             if self.cycle_buy:
                 min_trade_amount = f2d(tcm.get_min_sell_amount(float(self.avg_rate)))
                 amount = self.sum_amount_first if for_tp else (self.deposit_second / self.avg_rate)
@@ -3248,15 +3206,14 @@
                         # After place but before execute TP was filled some grid
                         self.tp_hold = False
                         self.after_filled_tp(one_else_grid=True)
                     elif self.tp_cancel_from_grid_handler:
                         self.tp_cancel_from_grid_handler = False
                         self.grid_handler()
                     else:
-                        self.grid_remove = True
                         self.cancel_grid(cancel_all=True)
                 else:
                     self.message_log('Wild order, do not know it', tlg=True)
             elif update.status == OrderUpdate.PARTIALLY_FILLED:
                 if self.tp_order_id == update.original_order.id:
                     self.message_log("Take profit partially filled", color=Style.B_WHITE)
                     amount_first_fee, amount_second_fee = self.fee_for_tp(amount_first, amount_second)
@@ -3379,15 +3336,14 @@
                 self.tp_was_filled = (amount_first, amount_second, True)
                 if self.tp_hold or self.tp_cancel_from_grid_handler:
                     self.tp_cancel_from_grid_handler = False
                     self.tp_hold = False
                     # After place but before accept TP was filled some grid
                     self.after_filled_tp(one_else_grid=True)
                 else:
-                    self.grid_remove = True
                     self.cancel_grid(cancel_all=True)
             else:
                 self.message_log(f"Did not have waiting order id for {place_order_id}", LogLevel.ERROR,
                                  color=Style.B_RED)
         else:
             if self.orders_init.exist(place_order_id):
                 self.orders_grid.append(order.id, order.buy, f2d(order.amount), f2d(order.price))
@@ -3413,22 +3369,21 @@
                                 self.order_q_placed = True
                                 self.message_log('All grid orders place successfully', color=Style.B_WHITE)
                         elif not self.order_q_placed and not self.shift_grid_threshold:
                             self.place_grid_part()
                         if self.start_hold:
                             self.message_log('Release hold Start, continue remove grid orders', color=Style.B_WHITE)
                             self.start_hold = False
-                            self.grid_remove = True
                             self.cancel_grid()
             elif place_order_id == self.tp_wait_id:
                 self.tp_wait_id = None
                 self.tp_order_id = order.id
                 if self.tp_hold or self.tp_cancel or self.tp_cancel_from_grid_handler:
                     self.cancel_order_id = self.tp_order_id
-                    self.cancel_order(self.tp_order_id)
+                    self.cancel_order_exp(self.tp_order_id)
                 else:
                     # Place next part of grid orders
                     if self.orders_hold and not self.order_q_placed and not self.orders_init:
                         self.place_grid_part()
             else:
                 self.message_log(F"Did not have waiting order id for {place_order_id}", LogLevel.ERROR)
 
@@ -3463,15 +3418,14 @@
             elif place_order_id == self.tp_wait_id:
                 self.tp_wait_id = None
 
     def on_cancel_order_success(self, order_id: int, canceled_order: Order, cancel_all=False) -> None:
         if self.orders_grid.exist(order_id):
             self.message_log(f"Processing canceled grid order {order_id}", log_level=LogLevel.INFO)
             self.part_amount.pop(order_id, None)
-            self.grid_order_canceled = None
             self.orders_grid.remove(order_id)
             save = True
             for o in self.get_buffered_completed_trades():
                 if o.order_id == order_id:
                     save = False
                     break
             if save:
@@ -3514,40 +3468,14 @@
                 self.place_profit_order()
                 return
             if self.tp_cancel:
                 # Restart
                 self.tp_cancel = False
                 self.start()
 
-    def on_cancel_order_error_string(self, order_id: int, error: str) -> None:
-        # Check all orders on exchange if not exists required
-        open_orders = self.get_buffered_open_orders()
-        if any(i.id == order_id for i in open_orders):
-            self.message_log(f"On cancel order {order_id} {error}, retry", LogLevel.ERROR)
-            self.cancel_order(order_id)
-        elif not STANDALONE:
-            self.message_log(f"On cancel order {order_id} {error}", LogLevel.ERROR)
-            if self.orders_grid.exist(order_id):
-                self.message_log("It's was grid order, probably filled", LogLevel.WARNING)
-                self.grid_order_canceled = None
-                _buy, _amount, _price = self.orders_grid.get_by_id(order_id)
-                amount_first = _amount
-                amount_second = _amount * _price
-                self.avg_rate = amount_second / amount_first
-                self.message_log(f"Executed amount: First: {amount_first}, Second: {amount_second},"
-                                 f" price: {self.avg_rate}")
-                # Remove grid order with =id from order list
-                self.orders_grid.remove(order_id)
-                self.grid_handler(_amount_first=amount_first, _amount_second=amount_second, after_full_fill=True)
-            elif order_id == self.cancel_order_id:
-                self.message_log("It's was take profit", LogLevel.ERROR)
-                amount_first = self.tp_order[1]
-                amount_second = self.tp_order[1] * self.tp_order[2]
-                self.tp_was_filled = (amount_first, amount_second, True)
-                self.tp_order_id = None
-                self.tp_order = ()
-                self.message_log(f"Was filled TP: {self.tp_was_filled}", log_level=LogLevel.DEBUG)
-                self.cancel_grid()
-            else:
-                self.message_log("It's unknown", LogLevel.ERROR)
-        else:
-            self.message_log(f"On cancel order {order_id} {error}", LogLevel.ERROR)
+    def on_cancel_order_error_string(self, order_id: int, error: str, cancel_all=False) -> None:
+        self.message_log(f"On cancel order {order_id} {error}", LogLevel.ERROR)
+        if self.orders_grid.exist(order_id):
+            order = self.orders_grid.get_by_id(order_id)
+            self.orders_grid.remove(order_id)
+            self.orders_grid.append(order_id, *order)
+            self.cancel_grid(cancel_all=cancel_all)
```

### Comparing `martin_binance-1.3.3/martin_binance/funds_rate.db.template` & `martin-binance-1.3.4b0/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.3.4b0/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/margin_wrapper.py` & `martin-binance-1.3.4b0/martin_binance/margin_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 margin.de <-> Python strategy <-> <margin_wrapper> <-> exchanges-wrapper <-> Exchanges API/WSS
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.3"
+__version__ = "1.3.4b0"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import simplejson as json
 import logging
@@ -420,15 +420,15 @@
     base_asset = str()
     quote_asset = str()
     ticker = {}
     funds = {}
     order_book = {}
     order_id = int(datetime.now().strftime("%S%M")) * 1000
     wait_order_id = []  # List of placed orders for time-out detect
-    canceled_order_id = []  # List canceled orders  for time-out detect
+    canceled_order_id = []  # List canceled orders for time-out detect
     trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
     orders = {}  # {int(id): Order(), } of orders associated with strategy
     tcm = None  # TradingCapabilityManager
     last_state = None
     rate_limiter = RATE_LIMITER
     start_time_ms = int(time.time() * 1000)
     send_request = None
@@ -601,22 +601,17 @@
         kline = StrategyBase.Klines.get_kline(size)
         if len(kline) > number_of_candles+1:
             return kline[-number_of_candles-(0 if include_current_building_candle else 1):
                          None if include_current_building_candle else -1]
         return kline[:None if include_current_building_candle else -1]
 
     @staticmethod
-    def cancel_order(order_id: int) -> None:
+    def cancel_order(order_id: int, cancel_all=False) -> None:
         loop.create_task(cancel_order_timeout(order_id))
-        loop.create_task(cancel_order_call(order_id))
-
-    @staticmethod
-    def cancel_all_order(order_id: int) -> None:
-        loop.create_task(cancel_order_timeout(order_id))
-        loop.create_task(cancel_all_order_call(order_id))
+        loop.create_task(cancel_order_call(order_id, cancel_all))
 
     @staticmethod
     def transfer_to_master(symbol: str, amount: str):
         if ms.MODE in ('T', 'TC'):
             loop.create_task(transfer2master(symbol, amount))
 
 
@@ -992,14 +987,15 @@
             cls.strategy.on_new_funds(funds)
 
 
 async def buffered_orders():
     cls = StrategyBase
     exch_orders = {}
     save_orders_id = []
+    diff_id = set()
     restore = False
     run = False
     while not run:
         try:
             res = await cls.send_request(cls.stub.CheckStream, api_pb2.MarketRequest, symbol=cls.symbol)
         except Exception as ex:
             logger.warning(f"Exception on Check WSS: {ex}")
@@ -1026,71 +1022,62 @@
                 _orders_from_save = jsonpickle.decode(cls.last_state.pop(ms_orders, '{}'), keys=True)
                 if isinstance(_orders_from_save, list):
                     for _o in _orders_from_save:
                         cls.orders[_o.id] = _o
                 else:
                     cls.orders = _orders_from_save
                 #
-                cls.strategy.restore_strategy_state(cls.last_state)
+                cls.strategy.restore_strategy_state(cls.last_state, restore=False)
 
             if restore:
                 cls.strategy.message_log("Trying restore saved state after lost connection to host",
                                          color=ms.Style.GREEN)
 
             _orders = await cls.send_request(cls.stub.FetchOpenOrders, api_pb2.MarketRequest, symbol=cls.symbol)
             if _orders is None:
                 raise UserWarning("Can't fetch open orders")
             StrategyBase.rate_limiter = max(StrategyBase.rate_limiter, _orders.rate_limiter)
+
             orders = json_format.MessageToDict(_orders).get('items', [])
-            part_id = []
             for order in orders:
                 _id = int(order['orderId'])
                 exch_orders[_id] = Order(order)
                 if (order.get('status', None) == 'PARTIALLY_FILLED'
                         and order_trades_sum(_id) < Decimal(order['executedQty'])):
-                    part_id.append(_id)
+                    diff_id.add(_id)
+            # Add saved orders id's
+            save_orders_id.extend(list(cls.orders))
             # Add TP id
-            if cls.strategy.tp_order_id:
+            if cls.strategy.tp_order_id and cls.strategy.tp_order_id not in save_orders_id:
                 save_orders_id.append(cls.strategy.tp_order_id)
-            # Add grid id's
-            save_orders_id.extend(list(cls.orders))
+            # print(f"buffered_orders.save_orders_id: {save_orders_id}")
+
             # Missed fill event list
-            diff_id = list(set(save_orders_id).difference(set(exch_orders)))
-            # Erroneously not deleted order
-            diff_excess_id = list(set(exch_orders).
-                                  difference(save_orders_id).
-                                  intersection(cls.canceled_order_id))
-            # print(f"buffered_orders.diff_excess_id: {diff_excess_id}")
+            diff_id.update(set(save_orders_id).difference(set(exch_orders)))
+            # print(f"buffered_orders.diff_id: {diff_id}")
 
-            if diff_id or part_id:
-                cls.strategy.message_log(f"Perhaps was missed event for order(s): {diff_id + part_id},"
+            if diff_id:
+                cls.strategy.message_log(f"Perhaps was missed event for order(s): {diff_id},"
                                          f" checking it", log_level=LogLevel.WARNING, tlg=False)
-                for _id in list(set(diff_id + part_id)):
+                for _id in diff_id:
                     await fetch_order(_id, _filled_update_call=True)
-                part_id.clear()
-            if diff_excess_id:
-                cls.strategy.message_log(f"Find excess order(s): {diff_excess_id}, checking it",
-                                         log_level=LogLevel.WARNING, tlg=False)
-                for _id in diff_excess_id:
-                    check_status = await fetch_order(_id, _filled_update_call=False)
-                    if check_status and check_status.get('status') not in ('FILLED', 'CANCELED'):
-                        cls.strategy.message_log(f"buffered_orders.create_task: cancel_order: {_id}",
-                                                 log_level=LogLevel.INFO)
-                        loop.create_task(cancel_order_timeout(_id))
-                        loop.create_task(cancel_order_call(_id))
+
+            if cls.last_state:
+                cls.strategy.restore_strategy_state(restore=True)
 
             if ms.MODE == 'TC' and cls.last_state:
                 last_state = cls.strategy.save_strategy_state(return_only=True)
                 last_state_update(cls, last_state)
                 with cls.state_file.open(mode='w') as outfile:
                     json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
                 cls.strategy.start_collect = True
             cls.orders.update(exch_orders)
             exch_orders.clear()
             save_orders_id.clear()
+            diff_id.clear()
             cls.last_state = None
             restore = False
 
         except asyncio.CancelledError:
             # print("buffered_orders.Cancelled")
             run = False
         except UserWarning as ex:
@@ -1198,18 +1185,22 @@
                 price = str(Decimal(ed['quote_asset_transacted']) / Decimal(ed['cumulative_filled_quantity']))
                 trade.update({"qty": ed['cumulative_filled_quantity'], "price": price})
                 # cls.strategy.message_log(f"on_order_update.trade: {trade}",
                 #                                  log_level=LogLevel.DEBUG, color=ms.Style.YELLOW)
                 # Append to list
                 cls.trades.append(PrivateTrade(trade))
             cls.strategy.on_order_update(OrderUpdate(ed))
+            if ms.MODE == 'TC' and cls.strategy.start_collect:
+                cls.strategy.s_ticker[list(cls.strategy.s_ticker)[-1]].update({'lastPrice': ed['last_executed_price']})
+                cls.strategy.open_orders_snapshot()
 
 
 async def create_limit_order(_id: int, buy: bool, amount: str, price: str) -> None:
     cls = StrategyBase
+    cls.wait_order_id.append(_id)
     try:
         if ms.MODE in ('T', 'TC'):
             ts = time.time()
             res = await cls.send_request(cls.stub.CreateLimitOrder, api_pb2.CreateLimitOrderRequest,
                                          symbol=cls.symbol,
                                          buy_side=buy,
                                          quantity=amount,
@@ -1228,23 +1219,23 @@
     except asyncio.CancelledError:
         pass  # Task cancellation should not be logged as an error
     except grpc.RpcError as ex:
         status_code = ex.code()
         cls.strategy.message_log(f"Exception creating order {_id}: {status_code.name}, {ex.details()}")
         if status_code == grpc.StatusCode.FAILED_PRECONDITION:
             # Supress order timeout message
-            cls.wait_order_id.append(_id)
+            cls.wait_order_id.remove(_id)
             cls.strategy.on_place_order_error_string(_id, error=f"FAILED_PRECONDITION: {ex.details()}")
     except Exception as _ex:
         cls.strategy.message_log(f"Exception creating order {_id}: {_ex}")
     else:
         # cls.strategy.message_log(f"Create_limit_order.result: {result}",
         #                          log_level=LogLevel.DEBUG, color=ms.Style.UNDERLINE)
         if result:
-            cls.wait_order_id.append(_id)
+            cls.wait_order_id.remove(_id)
             order = Order(result)
             cls.strategy.message_log(
                 f"Order placed {order.id}({result.get('clientOrderId') or _id}) for {result.get('side')}"
                 f" {any2str(order.amount)} by {any2str(order.price)}"
                 f" Remaining amount {any2str(order.remaining_amount)}",
                 color=ms.Style.GREEN)
             orig_qty = Decimal(result['origQty'])
@@ -1258,126 +1249,110 @@
                          "orderId": order.id,
                          "price": price,
                          "time": order.timestamp}
                 # cls.strategy.message_log(f"place_limit_order_callback.trade: {trade}", color=ms.Style.YELLOW)
                 if len(cls.trades) > TRADES_LIST_LIMIT:
                     del cls.trades[0]
                 cls.trades.append(PrivateTrade(trade))
+
+                if ms.MODE == 'TC' and cls.strategy.start_collect:
+                    cls.strategy.s_ticker[list(cls.strategy.s_ticker)[-1]].update({'lastPrice': str(price)})
+
             if executed_qty < orig_qty:
                 cls.orders[order.id] = order
             if ms.MODE == 'TC' and cls.strategy.start_collect:
                 cls.strategy.open_orders_snapshot()
             elif ms.MODE == 'S':
                 await on_funds_update()
             cls.strategy.on_place_order_success(_id, order)
 
 
 async def place_limit_order_timeout(_id):
     cls = StrategyBase
     await asyncio.sleep(ORDER_TIMEOUT)
     if _id in cls.wait_order_id:
         cls.wait_order_id.remove(_id)
-    else:
         cls.strategy.on_place_order_error_string(_id, 'Place order timeout')
 
 
-async def cancel_order_call(_id: int):
+async def cancel_order_call(_id: int, cancel_all: bool):
     cls = StrategyBase
+    cls.canceled_order_id.append(_id)
     try:
         if ms.MODE in ('T', 'TC'):
-            res = await cls.send_request(cls.stub.CancelOrder, api_pb2.CancelOrderRequest,
-                                         symbol=cls.symbol,
-                                         order_id=_id)
-            result = json_format.MessageToDict(res)
+            if cancel_all:
+                if cls.bulk_orders_cancel.get(_id) is None:
+                    res = await cls.send_request(cls.stub.CancelAllOrders, api_pb2.MarketRequest, symbol=cls.symbol)
+                    [cls.bulk_orders_cancel.update({v['orderId']: v}) for v in ast.literal_eval(json.loads(res.result))]
+                result = cls.bulk_orders_cancel.pop(_id, None)
+            else:
+                res = await cls.send_request(cls.stub.CancelOrder, api_pb2.CancelOrderRequest,
+                                             symbol=cls.symbol,
+                                             order_id=_id)
+                result = json_format.MessageToDict(res)
         else:
             result = cls.strategy.account.cancel_order(order_id=_id, ts=int(cls.strategy.local_time()*1000))
     except asyncio.CancelledError:
         pass  # Task cancellation should not be logged as an error.
     except grpc.RpcError as ex:
         status_code = ex.code()
         cls.strategy.message_log(f"Exception on cancel order for {_id}: {status_code.name}, {ex.details()}")
         await asyncio.sleep(HEARTBEAT)
         if status_code == grpc.StatusCode.UNKNOWN:
             check_status = await fetch_order(_id, _filled_update_call=True)
             if check_status.get('status') == 'CANCELED':
                 # For stop timeout firing
-                cls.canceled_order_id.append(_id)
+                cls.canceled_order_id.remove(_id)
     except Exception as _ex:
         cls.strategy.message_log(f"Exception on cancel order call for {_id}:\n{_ex}")
     else:
         # print(f"cancel_order_call.result: {result}")
         # Remove from orders lists
-        if result:
+        cls.canceled_order_id.remove(_id)
+        if result and result.get('status') == 'CANCELED':
             remove_from_orders_lists([_id])
             cls.strategy.message_log(f"Cancel order {_id} success", color=ms.Style.GREEN)
-            cls.strategy.on_cancel_order_success(_id, Order(result))
-            cls.canceled_order_id.append(_id)
+            cls.strategy.on_cancel_order_success(_id, Order(result), cancel_all=cancel_all)
             if ms.MODE == 'TC' and cls.strategy.start_collect:
                 cls.strategy.open_orders_snapshot()
             elif ms.MODE == 'S':
                 await on_funds_update()
-
-
-async def cancel_all_order_call(_id: int):
-    cls = StrategyBase
-    try:
-        if cls.bulk_orders_cancel.get(_id) is None:
-            res = await cls.send_request(cls.stub.CancelAllOrders, api_pb2.MarketRequest, symbol=cls.symbol)
-            [cls.bulk_orders_cancel.update({v['orderId']: v}) for v in ast.literal_eval(json.loads(res.result))]
-        result = cls.bulk_orders_cancel.pop(_id, None)
-    except asyncio.CancelledError:
-        pass  # Task cancellation should not be logged as an error.
-    except grpc.RpcError as ex:
-        status_code = ex.code()
-        cls.strategy.message_log(f"Exception on cancel all orders for {_id}: {status_code.name}, {ex.details()}")
-    except Exception as _ex:
-        cls.strategy.message_log(f"Exception on cancel all orders for {_id}:\n{_ex}")
-    else:
-        # print(f"cancel_all_order_call.result: {result}")
-        # Remove from orders lists
-        if result and result.get('status') == 'CANCELED':
-            remove_from_orders_lists([_id])
-            cls.strategy.message_log(f"Cancel order {_id} success", color=ms.Style.GREEN)
-            cls.canceled_order_id.append(_id)
-            cls.strategy.on_cancel_order_success(_id, Order(result), cancel_all=True)
+        else:
+            cls.strategy.on_cancel_order_error_string(_id, 'Cancel order warning', cancel_all=cancel_all)
 
 
 async def cancel_order_timeout(_id):
     cls = StrategyBase
     await asyncio.sleep(ORDER_TIMEOUT)
     if _id in cls.canceled_order_id:
         cls.canceled_order_id.remove(_id)
-    else:
         cls.strategy.on_cancel_order_error_string(_id, 'Cancel order timeout')
 
 
-async def fetch_order(_id: int, _filled_update_call: bool = False):
+async def fetch_order(_id: int, _filled_update_call=False):
     cls = StrategyBase
     try:
         res = await cls.send_request(cls.stub.FetchOrder, api_pb2.FetchOrderRequest,
                                      symbol=cls.symbol,
                                      order_id=_id,
                                      filled_update_call=_filled_update_call)
         result = json_format.MessageToDict(res)
     except asyncio.CancelledError:
         pass  # Task cancellation should not be logged as an error.
     except Exception as _ex:
         cls.strategy.message_log(f"Exception in fetch_order: {_ex}", log_level=LogLevel.ERROR)
         return {}
     else:
         cls.strategy.message_log(f"For order {_id} fetched status is {result.get('status')}",
-                                 log_level=LogLevel.INFO)
+                                 log_level=LogLevel.INFO, color=ms.Style.GREEN)
         if _filled_update_call and result.get('status') == 'CANCELED':
             remove_from_orders_lists([_id])
-            cls.canceled_order_id.append(_id)
-            cls.strategy.message_log(f"Order {_id} has already been deleted", color=ms.Style.GREEN)
             cls.strategy.on_cancel_order_success(_id, Order(result))
         elif not result:
-            remove_from_orders_lists([_id])
-            cls.strategy.message_log(f"Order {_id} status fixed", color=ms.Style.GREEN)
+            raise UserWarning(f"For order {_id} can't get status")
         return result
 
 
 async def transfer2master(symbol: str, amount: str):
     cls = StrategyBase
     try:
         res = await cls.send_request(cls.stub.TransferToMaster,
@@ -1616,15 +1591,25 @@
     cls.for_request = _session.for_request
 
 
 def restore_state_before_backtesting(cls):
     saved_state = load_file(cls.state_file)
     cls.order_id = json.loads(saved_state.pop(ms_order_id, "0"))
     cls.trades = jsonpickle.decode(saved_state.pop('ms_trades', '[]'))
-    cls.orders = jsonpickle.decode(saved_state.pop(ms_orders, '{}'))
+
+    # TODO change after update and restart
+    # cls.orders = jsonpickle.decode(saved_state.pop(ms_orders, '{}'))
+    #
+    _orders_from_save = jsonpickle.decode(saved_state.pop(ms_orders, '{}'), keys=True)
+    if isinstance(_orders_from_save, list):
+        for _o in _orders_from_save:
+            cls.orders[_o.id] = _o
+    else:
+        cls.orders = _orders_from_save
+    #
     orders = json.loads(saved_state.get('orders'))
     # Restore initial state
     cls.strategy.cycle_buy = json.loads(saved_state.get('cycle_buy'))
     cls.strategy.reverse = json.loads(saved_state.get('reverse'))
     cls.strategy.deposit_first = ms.f2d(json.loads(saved_state.get('deposit_first')))
     cls.strategy.deposit_second = ms.f2d(json.loads(saved_state.get('deposit_second')))
     if cls.strategy.reverse:
```

### Comparing `martin_binance-1.3.3/martin_binance/ms_cfg.toml.template` & `martin-binance-1.3.4b0/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.3.4b0/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/service/grafana.json` & `martin-binance-1.3.4b0/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/martin_binance/service/relaunch.py` & `martin-binance-1.3.4b0/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.3/pyproject.toml` & `martin-binance-1.3.4b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,18 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper==1.3.3",
+    "exchanges-wrapper==1.3.4b0",
     "margin-strategy-sdk==0.0.11",
     "aiohttp==3.8.4",
-    "grpcio==1.48.1",
-    "grpcio-tools==1.48.1",
+    "grpcio==1.56.0",
     "jsonpickle==3.0.1",
     "psutil==5.9.5",
     "requests==2.31.0",
     "simplejson==3.19.1",
     "toml==0.10.2",
     "libtmux==0.22.1",
     "colorama==0.4.6",
```

### Comparing `martin_binance-1.3.3/PKG-INFO` & `martin-binance-1.3.4b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.3
+Version: 1.3.4b0
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==1.3.3
+Requires-Dist: exchanges-wrapper==1.3.4b0
 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4
-Requires-Dist: grpcio==1.48.1
-Requires-Dist: grpcio-tools==1.48.1
+Requires-Dist: grpcio==1.56.0
 Requires-Dist: jsonpickle==3.0.1
 Requires-Dist: psutil==5.9.5
 Requires-Dist: requests==2.31.0
 Requires-Dist: simplejson==3.19.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: libtmux==0.22.1
 Requires-Dist: colorama==0.4.6
@@ -31,28 +30,28 @@
 Requires-Dist: future==0.18.3
 Requires-Dist: inquirer==3.1.3
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: shortuuid==1.0.11
 Project-URL: Source, https://github.com/DogsTailFarmer/martin-binance
 
-<p align="center"><img src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="250"></p>
+<p align="center"><img src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="200"></p>
 <h3 align="center">Profitable, fault-tolerant, adaptable to the market</h3>
 
 ***
 <h1 align="center">Modified Martingale</h1>
 
 <h2 align="center">Cyclic grid strategy for SPOT market</h2>
 
 <h3 align="center">Free trading system for crypto exchanges (Binance, Bitfinex, Huobi, OKX,)</h3>
 
 <h4 align="center">Other crypto exchanges available through multi-exchange terminal MARGIN https://margin.de</h4>
 
 ***
-<h4 align="center" vertical-align="top">martin-binance <a href="https://badge.fury.io/py/martin-binance"><img style="vertical-align:middle" src="https://badge.fury.io/py/martin-binance.svg" alt="PyPI version" height="20"></a> <--> exchanges-wrapper <a href="https://badge.fury.io/py/exchanges-wrapper"><img style="vertical-align:middle" src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version" height="20"></a></h4>
+<h4 align="center">martin-binance <a href="https://pypi.org/project/martin-binance/"><img align="top" src="https://img.shields.io/pypi/v/martin-binance" alt="PyPI version"></a> <--> exchanges-wrapper <a href="https://pypi.org/project/exchanges-wrapper/"><img align="top" src="https://img.shields.io/pypi/v/exchanges-wrapper" alt="PyPI version"></a></h4>
 
 ***
 <h1 align="center"><a href="https://codeclimate.com/github/DogsTailFarmer/martin-binance/maintainability"><img src="https://api.codeclimate.com/v1/badges/bfa43f47d1c9a385fd8a/maintainability"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/martin-binance/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/martin-binance.svg/?label=resolved+issues&token=ONJLSJHeeBvXyuaAjG1OWUhG"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/martin-binance/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/martin-binance.svg/?label=active+issues&token=ONJLSJHeeBvXyuaAjG1OWUhG"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_martin-binance" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_martin-binance&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/martin-binance" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/martin-binance/month"/></a>
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.3 Summary: Free trading
-system for Binance SPOT API Author-email: Jerry Fedorenko
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.4b0 Summary: Free
+trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper==1.3.3 Requires-Dist: margin-strategy-sdk==0.0.11
-Requires-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist:
-grpcio-tools==1.48.1 Requires-Dist: jsonpickle==3.0.1 Requires-Dist:
-psutil==5.9.5 Requires-Dist: requests==2.31.0 Requires-Dist: simplejson==3.19.1
-Requires-Dist: toml==0.10.2 Requires-Dist: libtmux==0.22.1 Requires-Dist:
-colorama==0.4.6 Requires-Dist: prometheus-client==0.17.0 Requires-Dist:
-optuna==3.2.0 Requires-Dist: plotly==5.15.0 Requires-Dist: pandas==2.0.2
-Requires-Dist: dash==2.10.2 Requires-Dist: future==0.18.3 Requires-Dist:
-inquirer==3.1.3 Requires-Dist: scikit-learn==1.2.2 Requires-Dist: tqdm==4.65.0
-Requires-Dist: shortuuid==1.0.11 Project-URL: Source, https://github.com/
-DogsTailFarmer/martin-binance
+Dist: exchanges-wrapper==1.3.4b0 Requires-Dist: margin-strategy-sdk==0.0.11
+Requires-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.56.0 Requires-Dist:
+jsonpickle==3.0.1 Requires-Dist: psutil==5.9.5 Requires-Dist: requests==2.31.0
+Requires-Dist: simplejson==3.19.1 Requires-Dist: toml==0.10.2 Requires-Dist:
+libtmux==0.22.1 Requires-Dist: colorama==0.4.6 Requires-Dist: prometheus-
+client==0.17.0 Requires-Dist: optuna==3.2.0 Requires-Dist: plotly==5.15.0
+Requires-Dist: pandas==2.0.2 Requires-Dist: dash==2.10.2 Requires-Dist:
+future==0.18.3 Requires-Dist: inquirer==3.1.3 Requires-Dist: scikit-
+learn==1.2.2 Requires-Dist: tqdm==4.65.0 Requires-Dist: shortuuid==1.0.11
+Project-URL: Source, https://github.com/DogsTailFarmer/martin-binance
        [https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/
                           Modified%20martingale.svg]
          **** Profitable, fault-tolerant, adaptable to the market ****
 ***
                        ****** Modified Martingale ******
                ***** Cyclic grid strategy for SPOT market *****
 **** Free trading system for crypto exchanges (Binance, Bitfinex, Huobi, OKX,)
```

