# Comparing `tmp/python-kraken-sdk-1.4.1.tar.gz` & `tmp/python-kraken-sdk-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kraken-sdk-1.4.1.tar", last modified: Thu Jun 29 05:10:32 2023, max compression
+gzip compressed data, was "python-kraken-sdk-1.5.0.tar", last modified: Sun Jul 16 13:19:08 2023, max compression
```

## Comparing `python-kraken-sdk-1.4.1.tar` & `python-kraken-sdk-1.5.0.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.306157 python-kraken-sdk-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.290157 python-kraken-sdk-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.290157 python-kraken-sdk-1.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/self-review.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_build_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_test_futures_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_test_futures_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_test_spot_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/_test_spot_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/manual_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/manual_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/manual_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/manual_test_futures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/manual_test_spot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    54493 2023-06-29 05:10:32.306157 python-kraken-sdk-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/links.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/about/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/about/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/base_api/base_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/examples/futures_bot_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/examples/spot_bot_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/examples/spot_orderbook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/examples/trading_bot_templates.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/futures/rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/futures/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/issues.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/krakenexceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/krakenexceptions/krakenexceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.294157 python-kraken-sdk-1.4.1/docs/src/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/spot/rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/docs/src/spot/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.298157 python-kraken-sdk-1.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/futures_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/futures_trading_bot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/futures_ws_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/market_client_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/spot_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/spot_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/spot_trading_bot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/examples/spot_ws_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.298157 python-kraken-sdk-1.4.1/kraken/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 05:10:32.000000 python-kraken-sdk-1.4.1/kraken/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.298157 python-kraken-sdk-1.4.1/kraken/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/base_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.298157 python-kraken-sdk-1.4.1/kraken/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.298157 python-kraken-sdk-1.4.1/kraken/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/futures/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)    39217 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)    26338 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/futures/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/futures/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.298157 python-kraken-sdk-1.4.1/kraken/futures/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/futures/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/futures/ws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.298157 python-kraken-sdk-1.4.1/kraken/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/market.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    39336 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.302157 python-kraken-sdk-1.4.1/kraken/spot/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/kraken/spot/ws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.302157 python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54493 2023-06-29 05:10:32.000000 python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-29 05:10:32.000000 python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 05:10:32.000000 python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-29 05:10:32.000000 python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 05:10:32.000000 python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 05:10:32.306157 python-kraken-sdk-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.302157 python-kraken-sdk-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.302157 python-kraken-sdk-1.4.1/tests/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/test_futures_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/test_futures_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/test_futures_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/test_futures_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/test_futures_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/futures/test_futures_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.306157 python-kraken-sdk-1.4.1/tests/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:10:32.306157 python-kraken-sdk-1.4.1/tests/spot/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/fixture/orderbook.json
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-29 05:10:19.000000 python-kraken-sdk-1.4.1/tests/spot/test_spot_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.274067 python-kraken-sdk-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.274067 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/self-review.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_build_doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_futures_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_futures_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_spot_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_spot_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_test_futures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_test_spot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    54493 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/links.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/about/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/base_api/base_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/futures_bot_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/spot_bot_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/spot_orderbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/trading_bot_templates.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/futures/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/futures/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/issues.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/krakenexceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/krakenexceptions/krakenexceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/spot/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/spot/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/futures_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/futures_trading_bot_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/futures_ws_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/market_client_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_trading_bot_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_ws_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/kraken/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/kraken/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/kraken/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/base_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/kraken/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39217 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26338 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/futures/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39336 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/spot/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/ws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54493 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/tests/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/tests/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/tests/spot/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/fixture/orderbook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_websocket.py
```

### Comparing `python-kraken-sdk-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 name: Feature request
 about: Suggest an idea for this project
 title: ""
-labels: ""
+labels: "Feature"
 assignees: ""
 ---
 
 **Is your feature request related to a problem? Please describe.**
 A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
 
 **Describe the solution you'd like**
```

### Comparing `python-kraken-sdk-1.4.1/.github/codecov.yml` & `python-kraken-sdk-1.5.0/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/pull_request_template.md` & `python-kraken-sdk-1.5.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/release.yaml` & `python-kraken-sdk-1.5.0/.github/release.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/self-review.md` & `python-kraken-sdk-1.5.0/.github/self-review.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_build.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_build.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_build_doc.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_build_doc.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_codecov.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_codecov.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_codeql.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_codeql.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_pypi_publish.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_test_futures_private.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_test_futures_private.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_test_futures_public.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_test_futures_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_test_spot_private.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_test_spot_private.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/_test_spot_public.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/_test_spot_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/cicd.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/manual_build.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/manual_build.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/manual_test_futures.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/manual_test_futures.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/manual_test_spot.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/manual_test_spot.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.github/workflows/release.yaml` & `python-kraken-sdk-1.5.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.gitignore` & `python-kraken-sdk-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.pre-commit-config.yaml` & `python-kraken-sdk-1.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.pylintrc` & `python-kraken-sdk-1.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/.readthedocs.yaml` & `python-kraken-sdk-1.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/CHANGELOG.md` & `python-kraken-sdk-1.5.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,50 @@
 # Changelog
 
 ## [Unreleased](https://github.com/btschwertfeger/python-kraken-sdk/tree/HEAD)
 
-[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.3.0...HEAD)
+[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.4.1...HEAD)
+
+Uncategorized merged pull requests:
+
+- Add "Question" issue template [\#122](https://github.com/btschwertfeger/python-kraken-sdk/pull/122) ([btschwertfeger](https://github.com/btschwertfeger))
+
+## [v1.4.1](https://github.com/btschwertfeger/python-kraken-sdk/tree/v1.4.1) (2023-06-28)
+
+[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.4.0...v1.4.1)
+
+**Fixed bugs:**
+
+- `kraken.spot.Market.get_recent_trades`: 'since' parameter does not work [\#119](https://github.com/btschwertfeger/python-kraken-sdk/issues/119)
+- Fix `kraken.spot.Market.get_recent_trades` parameter 'since' [\#120](https://github.com/btschwertfeger/python-kraken-sdk/pull/120) ([btschwertfeger](https://github.com/btschwertfeger))
+
+**Closed issues:**
+
+- Create `.github/release.yaml` [\#108](https://github.com/btschwertfeger/python-kraken-sdk/issues/108)
+
+## [v1.4.0](https://github.com/btschwertfeger/python-kraken-sdk/tree/v1.4.0) (2023-06-16)
+
+[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.3.0...v1.4.0)
 
 **Implemented enhancements:**
 
 - Add the `truncate` parameter to `create_order` of the Spot websocket client [\#111](https://github.com/btschwertfeger/python-kraken-sdk/issues/111)
-- Add the `truncate` parameter to create_order of the Spot websocket clients' `create_order` and `cancel_order`+ `kraken.spot.Trade.edit_order` [\#113](https://github.com/btschwertfeger/python-kraken-sdk/pull/113) ([btschwertfeger](https://github.com/btschwertfeger))
+- Add a Spot Orderbook client that handles a realtime order book [\#104](https://github.com/btschwertfeger/python-kraken-sdk/issues/104)
+- A the Spot order book client \(`kraken.spot.OrderbookClient`\) [\#106](https://github.com/btschwertfeger/python-kraken-sdk/pull/106) ([btschwertfeger](https://github.com/btschwertfeger))
+- Add the `truncate` parameter to the Spot websocket clients' `create_order` and `cancel_order`+ `kraken.spot.Trade.edit_order` [\#113](https://github.com/btschwertfeger/python-kraken-sdk/pull/113) ([btschwertfeger](https://github.com/btschwertfeger))
+
+**Fixed bugs:**
+
+- user.get_trade_volume\(\) says it supports multiple currencies as a list, but it does not seem to. [\#115](https://github.com/btschwertfeger/python-kraken-sdk/issues/115)
+- kraken.exceptions.KrakenException.KrakenInvalidNonceError: An invalid nonce was supplied. [\#114](https://github.com/btschwertfeger/python-kraken-sdk/issues/114)
 
 Uncategorized merged pull requests:
 
 - Update `/examples/spot_orderbook.py` [\#110](https://github.com/btschwertfeger/python-kraken-sdk/pull/110) ([btschwertfeger](https://github.com/btschwertfeger))
+- Create `release.yaml` [\#116](https://github.com/btschwertfeger/python-kraken-sdk/pull/116) ([btschwertfeger](https://github.com/btschwertfeger))
 
 ## [v1.3.0](https://github.com/btschwertfeger/python-kraken-sdk/tree/v1.3.0) (2023-05-24)
 
 [Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.2.0...v1.3.0)
 
 **Breaking changes:**
```

### Comparing `python-kraken-sdk-1.4.1/CODE_OF_CONDUCT.md` & `python-kraken-sdk-1.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/CONTRIBUTING.md` & `python-kraken-sdk-1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/LICENSE` & `python-kraken-sdk-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/Makefile` & `python-kraken-sdk-1.5.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,24 @@
 ## ======= I N S T A L L A T I O N =======
 ## install	Install the package
 ##
 install:
 	$(PYTHON) -m pip install .
 
 ## ======= T E S T I N G =======
-## test		Run the unittests
+## test		Run the unit tests
 ##
 test:
 	$(PYTEST) $(PYTEST_OPTS) $(TEST_DIR)
 
 tests: test
 
+test-wip:
+	$(PYTEST) -m "wip" -vv $(TEST_DIR)
+
 coverage:
 	$(PYTEST) $(PYTEST_COV_OPTS) $(TEST_DIR)
 
 ## doctest	Run the documentation tests
 ##
 doctest:
 	cd docs && make doctest
```

### Comparing `python-kraken-sdk-1.4.1/PKG-INFO` & `python-kraken-sdk-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.4.1
+Version: 1.5.0
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `python-kraken-sdk-1.4.1/README.md` & `python-kraken-sdk-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/Makefile` & `python-kraken-sdk-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/conf.py` & `python-kraken-sdk-1.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/index.rst` & `python-kraken-sdk-1.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/links.rst` & `python-kraken-sdk-1.5.0/docs/links.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/make.bat` & `python-kraken-sdk-1.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/src/examples/futures_bot_template.rst` & `python-kraken-sdk-1.5.0/docs/src/examples/futures_bot_template.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/src/examples/spot_bot_template.rst` & `python-kraken-sdk-1.5.0/docs/src/examples/spot_bot_template.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/src/examples/trading_bot_templates.rst` & `python-kraken-sdk-1.5.0/docs/src/examples/trading_bot_templates.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/src/getting_started/getting_started.rst` & `python-kraken-sdk-1.5.0/docs/src/getting_started/getting_started.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/src/introduction.rst` & `python-kraken-sdk-1.5.0/docs/src/introduction.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/docs/src/issues.rst` & `python-kraken-sdk-1.5.0/docs/src/issues.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/examples/futures_examples.py` & `python-kraken-sdk-1.5.0/examples/futures_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/examples/futures_trading_bot_template.py` & `python-kraken-sdk-1.5.0/examples/futures_trading_bot_template.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/examples/futures_ws_examples.py` & `python-kraken-sdk-1.5.0/examples/futures_ws_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/examples/market_client_example.ipynb` & `python-kraken-sdk-1.5.0/examples/market_client_example.ipynb`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/examples/spot_examples.py` & `python-kraken-sdk-1.5.0/examples/spot_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/examples/spot_orderbook.py` & `python-kraken-sdk-1.5.0/examples/spot_orderbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """
-NOTE: * The Spot Orderbook client is not released yet. It will be released
-        in python-kraken-sdk=v1.4.0.
-      * Have a look at https://gist.github.com/btschwertfeger/6eea0eeff193f7cd1b262cfce4f0eb51
-        for an example that works now.
-
 This module provides an example on how to use the Spot Orderbook
 client of the python-kraken-sdk (https://github.com/btschwertfeger/python-kraken-sdk)
 to retrieve and maintain a valid Spot order book for (a) specific
 asset pair(s). It can be run directly without any credentials if the
 python-kraken-sdk is installed.
 
     python3 -m pip install python-kraken-sdk
@@ -70,15 +65,15 @@
         book: Dict[str, Any] = self.get(pair=pair)
         bid: List[Tuple[str, str]] = list(book["bid"].items())
         ask: List[Tuple[str, str]] = list(book["ask"].items())
 
         print("Bid         Volume\t\t Ask         Volume")
         for level in range(self.depth):
             print(
-                f"{bid[level][0]} ({bid[level][1]}) \t {ask[level][0]} ({ask[level][1]})"
+                f"{bid[level][0]} ({bid[level][1][0]}) \t {ask[level][0]} ({ask[level][1][0]})"
             )
 
         assert book["valid"]  # ensure that the checksum is valid
 
 
 async def main() -> None:
     """
```

### Comparing `python-kraken-sdk-1.4.1/examples/spot_trading_bot_template.py` & `python-kraken-sdk-1.5.0/examples/spot_trading_bot_template.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/examples/spot_ws_examples.py` & `python-kraken-sdk-1.5.0/examples/spot_ws_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/base_api/__init__.py` & `python-kraken-sdk-1.5.0/kraken/base_api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/exceptions/__init__.py` & `python-kraken-sdk-1.5.0/kraken/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/futures/funding.py` & `python-kraken-sdk-1.5.0/kraken/futures/funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/futures/market.py` & `python-kraken-sdk-1.5.0/kraken/futures/market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/futures/trade.py` & `python-kraken-sdk-1.5.0/kraken/futures/trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/futures/user.py` & `python-kraken-sdk-1.5.0/kraken/futures/user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/futures/websocket/__init__.py` & `python-kraken-sdk-1.5.0/kraken/futures/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/futures/ws_client.py` & `python-kraken-sdk-1.5.0/kraken/futures/ws_client.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/__init__.py` & `python-kraken-sdk-1.5.0/kraken/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/funding.py` & `python-kraken-sdk-1.5.0/kraken/spot/funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/market.py` & `python-kraken-sdk-1.5.0/kraken/spot/market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/orderbook.py` & `python-kraken-sdk-1.5.0/kraken/spot/orderbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -253,24 +253,42 @@
         and the client instance is most likely not useable anymore. So this
         is the switch lets the user know, when to delete the current one and
         create a new one.
 
         :return: ``True`` if any critical error occurred else ``False``
         :rtype: bool
         """
-        return self.ws_client.exception_occur
+        return bool(self.ws_client.exception_occur)
 
     def get(self: "OrderbookClient", pair: str) -> Optional[dict]:
         """
         Returns the orderbook for a specific ``pair``.
 
         :param pair: The pair to get the orderbook from
         :type pair: str
         :return: The orderbook of that ``pair``.
         :rtype: dict
+
+        .. code-block::python
+            :linenos:
+            :caption: Orderbook: Get ask and bid
+
+            …
+            class Orderbook(OrderbookClient):
+
+                async def on_book_update(
+                    self: "Orderbook",
+                    pair: str,
+                    message: list
+                ) -> None:
+                    book: Dict[str, Any] = self.get(pair="XBT/USD")
+                    ask: List[Tuple[str, str]] = list(book["ask"].items())
+                    bid: List[Tuple[str, str]] = list(book["bid"].items())
+                    # ask and bid are now in format [price, (volume, timestamp)]
+                    # … and include the whole orderbook
         """
         return self.__book.get(pair)
 
     def __update_book(
         self: "OrderbookClient", pair: str, side: str, snapshot: list
     ) -> None:
         """
@@ -282,30 +300,31 @@
         [
             ['25026.00000', '2.77183035', '1684658128.013525'],
             ['25028.50000', '0.04725650', '1684658121.180535'],
             ['25030.20000', '0.29527502', '1684658128.018182'],
             ['25030.40000', '2.77134976', '1684658131.751539'],
             ['25032.20000', '0.13978808', '1684658131.751577']
         ]
-        ... where the first value is the ask or bid price, the second
-            represents the volume and the last one is the time stamp.
+        … where the first value is the ask or bid price, the second
+          represents the volume and the last one is the timestamp.
 
         :param side: The side to assign the data to,
             either ``ask`` or ``bid``
         :type side: str
         :param data: The data that needs to be assigned.
         :type data: list
         """
         for entry in snapshot:
             price: str = entry[0]
             volume: str = entry[1]
+            timestamp: str = entry[2]
 
             if float(volume) > 0.0:
                 # Price level exist or is new
-                self.__book[pair][side][price] = volume
+                self.__book[pair][side][price] = (volume, timestamp)
             else:
                 # Price level moved out of range
                 self.__book[pair][side].pop(price)
 
             if side == "ask":
                 self.__book[pair]["ask"] = OrderedDict(
                     sorted(self.__book[pair]["ask"].items(), key=self.get_first)[
@@ -329,36 +348,29 @@
 
         :param pair: The pair that's orderbook checksum should be validated.
         :type pair: str
         :param checksum: The checksum sent by the Kraken API
         :type checksum: str
         """
         book: dict = self.__book[pair]
-
-        # sort ask (desc) and bid (asc)
-        ask: List[tuple] = sorted(book["ask"].items(), key=self.get_first)
-        bid: List[tuple] = sorted(
-            book["bid"].items(),
-            key=self.get_first,
-            reverse=True,
-        )
+        ask = list(book["ask"].items())
+        bid = list(book["bid"].items())
 
         local_checksum: str = ""
-        for price_level, volume in ask[:10]:
+        for price_level, (volume, _) in ask[:10]:
             local_checksum += price_level.replace(".", "").lstrip("0") + volume.replace(
                 ".", ""
             ).lstrip("0")
 
-        for price_level, volume in bid[:10]:
+        for price_level, (volume, _) in bid[:10]:
             local_checksum += price_level.replace(".", "").lstrip("0") + volume.replace(
                 ".", ""
             ).lstrip("0")
 
         self.__book[pair]["valid"] = checksum == str(crc32(local_checksum.encode()))
-        # assert self.__book[pair]["valid"]
 
     @staticmethod
     def get_first(values: tuple) -> float:
         """
         This function is used as callback for the ``sorted`` method
         to sort a tuple/list by its first value and while ensuring
         that the values are floats and comparable.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/staking.py` & `python-kraken-sdk-1.5.0/kraken/spot/staking.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/trade.py` & `python-kraken-sdk-1.5.0/kraken/spot/trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/user.py` & `python-kraken-sdk-1.5.0/kraken/spot/user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/websocket/__init__.py` & `python-kraken-sdk-1.5.0/kraken/spot/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/kraken/spot/ws_client.py` & `python-kraken-sdk-1.5.0/kraken/spot/ws_client.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/pyproject.toml` & `python-kraken-sdk-1.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2", "wheel"]
+requires = ["setuptools>=65.5.1", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-kraken-sdk"
 dynamic = ["version"]
 authors = [
   {name = "Benjamin Thomas Schwertfeger", email = "contact@b-schwertfeger.de"},
@@ -61,31 +61,38 @@
 ]
 examples = ["matplotlib"]
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
-include = ["kraken*"]
-exclude = ["docs*", "tests*", "examples*", ".env"]
+include = [
+  "kraken*"
+]
+exclude = [
+  "docs*",
+  "tests*",
+  "examples*",
+  ".env"
+]
 
 [tool.setuptools_scm]
 write_to = "kraken/_version.py"
 version_scheme = "guess-next-dev"
 local_scheme = "no-local-version"
 
 # ========= T E S T I N G =====================================================
 #
 [tool.pytest]
 junit_family = "xunit2"
 testpaths = ["tests"]
 
 [tool.pytest.ini_options]
 markers = [
-    "select: Used to run a specific test by hand.",
+    "wip: Used to run a specific test by hand.",
     "spot: mark a test that tests a Spot endpoint.",
     "spot_auth: mark a test that tests a authenticaed Spot endpoint.",
     "spot_trade: mark a test that tests a Spot Trade endpoint.",
     "spot_user: mark a test that tests a Spot User endpoint.",
     "spot_market: mark a test that tests a Spot Market endpoint.",
     "spot_funding: mark a test that tests a Spot Funding endpoint.",
     "spot_staking: mark a test that tests a Spot Staking endpoint.",
```

### Comparing `python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/PKG-INFO` & `python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.4.1
+Version: 1.5.0
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `python-kraken-sdk-1.4.1/python_kraken_sdk.egg-info/SOURCES.txt` & `python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 setup.py
 .github/codecov.yml
 .github/pull_request_template.md
 .github/release.yaml
 .github/self-review.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/ISSUE_TEMPLATE/question.md
 .github/workflows/_build.yaml
 .github/workflows/_build_doc.yaml
 .github/workflows/_codecov.yaml
 .github/workflows/_codeql.yaml
 .github/workflows/_pre_commit.yaml
 .github/workflows/_pypi_publish.yaml
 .github/workflows/_test_futures_private.yaml
```

### Comparing `python-kraken-sdk-1.4.1/tests/futures/conftest.py` & `python-kraken-sdk-1.5.0/tests/futures/conftest.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/futures/helper.py` & `python-kraken-sdk-1.5.0/tests/futures/helper.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/futures/test_futures_base_api.py` & `python-kraken-sdk-1.5.0/tests/futures/test_futures_base_api.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/futures/test_futures_funding.py` & `python-kraken-sdk-1.5.0/tests/futures/test_futures_funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/futures/test_futures_market.py` & `python-kraken-sdk-1.5.0/tests/futures/test_futures_market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/futures/test_futures_trade.py` & `python-kraken-sdk-1.5.0/tests/futures/test_futures_trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/futures/test_futures_user.py` & `python-kraken-sdk-1.5.0/tests/futures/test_futures_user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/futures/test_futures_websocket.py` & `python-kraken-sdk-1.5.0/tests/futures/test_futures_websocket.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/conftest.py` & `python-kraken-sdk-1.5.0/tests/spot/conftest.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/fixture/orderbook.json` & `python-kraken-sdk-1.5.0/tests/spot/fixture/orderbook.json`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/helper.py` & `python-kraken-sdk-1.5.0/tests/spot/helper.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_base_api.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_base_api.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_funding.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_market.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_orderbook.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_orderbook.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_staking.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_staking.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_trade.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_user.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.4.1/tests/spot/test_spot_websocket.py` & `python-kraken-sdk-1.5.0/tests/spot/test_spot_websocket.py`

 * *Files identical despite different names*

