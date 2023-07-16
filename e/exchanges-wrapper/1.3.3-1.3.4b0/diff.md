# Comparing `tmp/exchanges_wrapper-1.3.3.tar.gz` & `tmp/exchanges-wrapper-1.3.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges-wrapper-1.3.4b0.tar", last modified: Sun Jul 16 16:11:52 2023, max compression
```

## Comparing `exchanges_wrapper-1.3.3.tar` & `exchanges-wrapper-1.3.4b0.tar`

### file list

```diff
@@ -1,20 +1,31 @@
--rw-r--r--   0        0        0     1114 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/LICENSE.md
--rw-r--r--   0        0        0     7142 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/README.md
--rw-r--r--   0        0        0     1317 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45215 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19609 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6184 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    62056 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2768 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12485 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    47721 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4429 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10260 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15714 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16089 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22397 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0     1175 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     8090 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.4b0/.deepsource.toml
+-rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.4b0/.dockerignore
+-rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.4b0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.4b0/.github/dependabot.yml
+-rw-r--r--   0        0        0      950 2023-06-21 13:50:12.422384 exchanges-wrapper-1.3.4b0/.github/workflows/docker-image.yml
+-rw-r--r--   0        0        0     1105 2023-06-21 11:56:25.815510 exchanges-wrapper-1.3.4b0/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0     6960 2023-07-11 17:04:46.392454 exchanges-wrapper-1.3.4b0/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.4b0/Dockerfile
+-rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.4b0/LICENSE.md
+-rw-r--r--   0        0        0     7068 2023-07-06 10:11:57.993253 exchanges-wrapper-1.3.4b0/README.md
+-rw-r--r--   0        0        0    15398 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.4b0/example/exch_client.py
+-rwxr-xr-x   0        0        0      216 2023-06-20 16:57:56.566218 exchanges-wrapper-1.3.4b0/example/ms_cfg.toml
+-rw-r--r--   0        0        0     1319 2023-07-16 16:05:47.206493 exchanges-wrapper-1.3.4b0/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    25161 2023-07-16 16:08:14.630475 exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-07-16 16:08:14.634480 exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19609 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6184 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    61849 2023-07-12 07:21:31.626804 exchanges-wrapper-1.3.4b0/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.4b0/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12485 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    47721 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4429 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10260 2023-07-08 19:35:27.596549 exchanges-wrapper-1.3.4b0/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15714 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16089 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.4b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22397 2023-06-29 16:57:42.989839 exchanges-wrapper-1.3.4b0/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1147 2023-07-16 16:05:47.190524 exchanges-wrapper-1.3.4b0/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-07-16 16:05:47.198509 exchanges-wrapper-1.3.4b0/requirements.txt
+-rw-r--r--   0        0        0     7982 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.4b0/PKG-INFO
```

### Comparing `exchanges_wrapper-1.3.3/LICENSE.md` & `exchanges-wrapper-1.3.4b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/README.md` & `exchanges-wrapper-1.3.4b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-
-<p align="center"><img src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="300"></p>
-
-***
-<h1 align="center">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
+<h1 align="center"><img align="center" src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="75">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
 
 <h2 align="center">Binance, Bitfinex, Huobi, OKX,</h2>
 
 <h3 align="center">For SPOT markets</h3>
 
 ***
-<a href="https://badge.fury.io/py/exchanges-wrapper"><img src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version"></a>
+<a href="https://pypi.org/project/exchanges-wrapper/"><img src="https://img.shields.io/pypi/v/exchanges-wrapper" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/exchanges-wrapper/maintainability"><img src="https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/maintainability" /></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=resolved+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
 From 1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-features) for details)
@@ -122,11 +118,11 @@
 
 ## Donate
 *BNB*, *BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92
 
 *USDT* (TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
 
 ## Powered by exchanges-wrapper
-<p align="left"><a href="https://github.com/DogsTailFarmer/martin-binance"></a><img src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="50"></p>
-
+<a><img align="middle" src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="50"></a>
 [martin-binance](https://github.com/DogsTailFarmer/martin-binance)
+
 Free trading system for crypto exchanges SPOT markets. Adaptive customizable reverse grid strategy based on martingale.
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
-            [https://raw.githubusercontent.com/gist/DogsTailFarmer/
+        ****** [https://raw.githubusercontent.com/gist/DogsTailFarmer/
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
-                                Logo%202v3.svg]
-***
-    ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
+Logo%202v3.svg]Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** From
 1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/
 DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-
 features) for details) *** ## exchanges-wrapper vs binance.py The main
@@ -69,13 +67,12 @@
 restart=always \ --name=exchanges-wrapper \ exchanges-wrapper ``` ###
 Documentations * For [binance.py](https://th0rgal.gitbook.io/binance-py/) use
 original * Served methods and examples of their use are described at
 ```example/exch_client.py``` * For [Protocol Buffers](https://
 developers.google.com/protocol-buffers/docs/overview) serializing structured
 data see ```proto/exchanges_wrapper/api.proto``` ## Donate *BNB*, *BUSD*,
 *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT* (TRC20)
-TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-wrapper
-[https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/
-Modified%20martingale.svg]
-[martin-binance](https://github.com/DogsTailFarmer/martin-binance) Free trading
-system for crypto exchanges SPOT markets. Adaptive customizable reverse grid
-strategy based on martingale.
+TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-wrapper [https://
+github.com/DogsTailFarmer/martin-binance/raw/public/doc/
+Modified%20martingale.svg] [martin-binance](https://github.com/DogsTailFarmer/
+martin-binance) Free trading system for crypto exchanges SPOT markets. Adaptive
+customizable reverse grid strategy based on martingale.
```

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/__init__.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.3"
+__version__ = "1.3.4b0"
 
 from pathlib import Path
 import shutil
 
 WORK_PATH = Path(Path.home(), ".MartinBinance")
 CONFIG_PATH = Path(WORK_PATH, "config")
 CONFIG_FILE = Path(CONFIG_PATH, "exch_srv_cfg.toml")
```

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/api_pb2_grpc.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/bitfinex_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/c_structures.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/c_structures.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/client.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -947,19 +947,15 @@
             params = {'all': 1}
             res = await self.http.send_api_call(
                 "v2/auth/w/order/cancel/multi",
                 method="POST",
                 signed=True,
                 **params,
             )
-            active_orders = 1
-            while active_orders:
-                active_orders = await self.fetch_open_orders(symbol=symbol, receive_window=receive_window)
-                if active_orders:
-                    await asyncio.sleep(STATUS_TIMEOUT / 10)
+            logger.debug(f"cancel_all_orders.res: {res}")
             if res and res[6] == 'SUCCESS':
                 res = res[4]
                 binance_res = bfx.orders(res, response_type=True, cancelled=True)
         elif self.exchange == 'huobi':
             orders = await self.fetch_open_orders(symbol=symbol, receive_window=receive_window, response_type=True)
             orders_id = []
             for order in orders:
```

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/definitions.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/errors.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/events.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/http_client.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/huobi_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/okx_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/exchanges_wrapper/web_sockets.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/web_sockets.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.3/pyproject.toml` & `exchanges-wrapper-1.3.4b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,15 @@
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
     "aiohttp==3.8.4",
-    "grpcio==1.48.1",
-    "grpcio-tools==1.48.1",
+    "grpcio==1.56.0",
     "toml==0.10.2",
     "idna==3.4",
     "pyotp~=2.8.0",
     "simplejson==3.19.1",
     "shortuuid~=1.0.11",
     "crypto_ws_api~=1.0.1",
 ]
```

### Comparing `exchanges_wrapper-1.3.3/PKG-INFO` & `exchanges-wrapper-1.3.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.3
+Version: 1.3.4b0
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: aiohttp==3.8.4
-Requires-Dist: grpcio==1.48.1
-Requires-Dist: grpcio-tools==1.48.1
+Requires-Dist: grpcio==1.56.0
 Requires-Dist: toml==0.10.2
 Requires-Dist: idna==3.4
 Requires-Dist: pyotp~=2.8.0
 Requires-Dist: simplejson==3.19.1
 Requires-Dist: shortuuid~=1.0.11
 Requires-Dist: crypto_ws_api~=1.0.1
 Project-URL: Source, https://github.com/DogsTailFarmer/exchanges-wrapper
 
-
-<p align="center"><img src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="300"></p>
-
-***
-<h1 align="center">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
+<h1 align="center"><img align="center" src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="75">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
 
 <h2 align="center">Binance, Bitfinex, Huobi, OKX,</h2>
 
 <h3 align="center">For SPOT markets</h3>
 
 ***
-<a href="https://badge.fury.io/py/exchanges-wrapper"><img src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version"></a>
+<a href="https://pypi.org/project/exchanges-wrapper/"><img src="https://img.shields.io/pypi/v/exchanges-wrapper" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/exchanges-wrapper/maintainability"><img src="https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/maintainability" /></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=resolved+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
 From 1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-features) for details)
@@ -146,12 +141,12 @@
 
 ## Donate
 *BNB*, *BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92
 
 *USDT* (TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
 
 ## Powered by exchanges-wrapper
-<p align="left"><a href="https://github.com/DogsTailFarmer/martin-binance"></a><img src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="50"></p>
-
+<a><img align="middle" src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="50"></a>
 [martin-binance](https://github.com/DogsTailFarmer/martin-binance)
+
 Free trading system for crypto exchanges SPOT markets. Adaptive customizable reverse grid strategy based on martingale.
```

#### html2text {}

```diff
@@ -1,26 +1,24 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.3 Summary: REST API
-and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.4b0 Summary: REST
+API and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
 email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist: grpcio-
-tools==1.48.1 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.4 Requires-
-Dist: pyotp~=2.8.0 Requires-Dist: simplejson==3.19.1 Requires-Dist:
-shortuuid~=1.0.11 Requires-Dist: crypto_ws_api~=1.0.1 Project-URL: Source,
-https://github.com/DogsTailFarmer/exchanges-wrapper
-            [https://raw.githubusercontent.com/gist/DogsTailFarmer/
+Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.56.0 Requires-Dist: toml==0.10.2
+Requires-Dist: idna==3.4 Requires-Dist: pyotp~=2.8.0 Requires-Dist:
+simplejson==3.19.1 Requires-Dist: shortuuid~=1.0.11 Requires-Dist:
+crypto_ws_api~=1.0.1 Project-URL: Source, https://github.com/DogsTailFarmer/
+exchanges-wrapper
+        ****** [https://raw.githubusercontent.com/gist/DogsTailFarmer/
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
-                                Logo%202v3.svg]
-***
-    ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
+Logo%202v3.svg]Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** From
 1.3.2 update exch_srv_cfg.toml (see [CHANGELOG](https://github.com/
 DogsTailFarmer/exchanges-wrapper/blob/master/CHANGELOG.md#added-for-new-
 features) for details) *** ## exchanges-wrapper vs binance.py The main
@@ -83,13 +81,12 @@
 restart=always \ --name=exchanges-wrapper \ exchanges-wrapper ``` ###
 Documentations * For [binance.py](https://th0rgal.gitbook.io/binance-py/) use
 original * Served methods and examples of their use are described at
 ```example/exch_client.py``` * For [Protocol Buffers](https://
 developers.google.com/protocol-buffers/docs/overview) serializing structured
 data see ```proto/exchanges_wrapper/api.proto``` ## Donate *BNB*, *BUSD*,
 *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT* (TRC20)
-TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-wrapper
-[https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/
-Modified%20martingale.svg]
-[martin-binance](https://github.com/DogsTailFarmer/martin-binance) Free trading
-system for crypto exchanges SPOT markets. Adaptive customizable reverse grid
-strategy based on martingale.
+TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-wrapper [https://
+github.com/DogsTailFarmer/martin-binance/raw/public/doc/
+Modified%20martingale.svg] [martin-binance](https://github.com/DogsTailFarmer/
+martin-binance) Free trading system for crypto exchanges SPOT markets. Adaptive
+customizable reverse grid strategy based on martingale.
```

