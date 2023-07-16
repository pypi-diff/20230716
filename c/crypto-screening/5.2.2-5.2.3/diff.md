# Comparing `tmp/crypto-screening-5.2.2.tar.gz` & `tmp/crypto-screening-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.2.2.tar", last modified: Sat Jul 15 10:26:59 2023, max compression
+gzip compressed data, was "crypto-screening-5.2.3.tar", last modified: Sun Jul 16 10:16:31 2023, max compression
```

## Comparing `crypto-screening-5.2.2.tar` & `crypto-screening-5.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.286264 crypto-screening-5.2.2/
--rw-rw-rw-   0        0        0       98 2023-07-15 10:26:57.000000 crypto-screening-5.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-15 10:26:59.286264 crypto-screening-5.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.2.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.2.2/build.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.134692 crypto-screening-5.2.2/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.196630 crypto-screening-5.2.2/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.2.2/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.2.2/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    46167 2023-07-15 10:14:05.000000 crypto-screening-5.2.2/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.2.2/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.2.2/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.2.2/crypto_screening/collect/orders.py
--rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.2.2/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.2.2/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    16881 2023-07-15 09:52:06.000000 crypto-screening-5.2.2/crypto_screening/collect/trades.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.2.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.2.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.2.2/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.206635 crypto-screening-5.2.2/crypto_screening/market/
--rw-rw-rw-   0        0        0    19625 2023-07-15 09:29:18.000000 crypto-screening-5.2.2/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.230665 crypto-screening-5.2.2/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.285263 crypto-screening-5.2.2/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20288 2023-07-14 23:48:05.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.2.2/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.2.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.2.2/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.2.2/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.149599 crypto-screening-5.2.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-15 10:26:57.000000 crypto-screening-5.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.2.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 10:26:59.286264 crypto-screening-5.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-15 10:26:50.000000 crypto-screening-5.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.182041 crypto-screening-5.2.3/
+-rw-rw-rw-   0        0        0       98 2023-07-16 10:16:29.000000 crypto-screening-5.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-16 10:16:31.182041 crypto-screening-5.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.2.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.2.3/build.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.030956 crypto-screening-5.2.3/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.100137 crypto-screening-5.2.3/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.2.3/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.2.3/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    46167 2023-07-15 10:14:05.000000 crypto-screening-5.2.3/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.2.3/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.2.3/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.2.3/crypto_screening/collect/orders.py
+-rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.2.3/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.2.3/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    16881 2023-07-15 09:52:06.000000 crypto-screening-5.2.3/crypto_screening/collect/trades.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.2.3/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.2.3/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.2.3/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.112645 crypto-screening-5.2.3/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19625 2023-07-15 09:29:18.000000 crypto-screening-5.2.3/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.135735 crypto-screening-5.2.3/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.181040 crypto-screening-5.2.3/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    11038 2023-07-16 10:08:59.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20288 2023-07-16 10:07:11.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.2.3/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.2.3/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.2.3/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.2.3/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.046498 crypto-screening-5.2.3/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-16 10:16:29.000000 crypto-screening-5.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.2.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:16:31.182041 crypto-screening-5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-16 10:16:26.000000 crypto-screening-5.2.3/setup.py
```

### Comparing `crypto-screening-5.2.2/PKG-INFO` & `crypto-screening-5.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.2
+Version: 5.2.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.2/README.md` & `crypto-screening-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/build.py` & `crypto-screening-5.2.3/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/assets.py` & `crypto-screening-5.2.3/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/exchanges.py` & `crypto-screening-5.2.3/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/market.py` & `crypto-screening-5.2.3/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/ohlcv.py` & `crypto-screening-5.2.3/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/orderbook.py` & `crypto-screening-5.2.3/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/orders.py` & `crypto-screening-5.2.3/crypto_screening/collect/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/screeners.py` & `crypto-screening-5.2.3/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/symbols.py` & `crypto-screening-5.2.3/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/collect/trades.py` & `crypto-screening-5.2.3/crypto_screening/collect/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/dataset.py` & `crypto-screening-5.2.3/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/interval.py` & `crypto-screening-5.2.3/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/dynamic.py` & `crypto-screening-5.2.3/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/foundation/data.py` & `crypto-screening-5.2.3/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.2.3/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/foundation/state.py` & `crypto-screening-5.2.3/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.2.3/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/base.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     - market:
         The dataset of the market data.
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.append("market")
 
-    MINIMUM_DELAY = 1
+    MINIMUM_DELAY = 0.1
 
     __slots__ = "symbol", "exchange", "market"
 
     def __init__(
             self,
             symbol: str,
             exchange: str,
@@ -229,15 +229,17 @@
         while self.saving:
             start = time.time()
 
             self.save_dataset()
 
             end = time.time()
 
-            time.sleep(max([delay - (end - start), self.MINIMUM_DELAY]))
+            if delay - (end - start) <= 0:
+                time.sleep(max([delay - (end - start), self.MINIMUM_DELAY]))
+            # end if
         # end while
     # end saving_loop
 # end BaseScreener
 
 class BaseMultiScreener(DataCollector):
     """
     A class to represent an asset price screener.
```

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/container.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
         "handler", 'amount', "loop", "limited", "_feeds_parameters",
         "_run_parameters", 'refresh'
     )
 
     screeners: List[BaseScreener]
     recorder: MarketRecorder
 
-    DELAY = 5
+    DELAY = 1
     AMOUNT = FEED_GROUP_SIZE
 
     REFRESH = dt.timedelta(minutes=5)
 
     def __init__(
             self,
             screeners: Optional[Iterable[BaseScreener]] = None,
```

### Comparing `crypto-screening-5.2.2/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.2.3/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/market/waiting.py` & `crypto-screening-5.2.3/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/process.py` & `crypto-screening-5.2.3/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/symbols.py` & `crypto-screening-5.2.3/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening/validate.py` & `crypto-screening-5.2.3/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.2.3/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.2
+Version: 5.2.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.2.3/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.2/pyproject.toml` & `crypto-screening-5.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.2.2'
+version = '5.2.3'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.2.2/setup.py` & `crypto-screening-5.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='5.2.2',
+        version='5.2.3',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

