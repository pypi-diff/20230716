# Comparing `tmp/crypto-screening-5.2.3.tar.gz` & `tmp/crypto-screening-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.2.3.tar", last modified: Sun Jul 16 10:16:31 2023, max compression
+gzip compressed data, was "crypto-screening-5.3.0.tar", last modified: Sun Jul 16 14:20:21 2023, max compression
```

## Comparing `crypto-screening-5.2.3.tar` & `crypto-screening-5.3.0.tar`

### file list

```diff
@@ -1,51 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.182041 crypto-screening-5.2.3/
--rw-rw-rw-   0        0        0       98 2023-07-16 10:16:29.000000 crypto-screening-5.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-16 10:16:31.182041 crypto-screening-5.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.2.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.2.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.030956 crypto-screening-5.2.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.100137 crypto-screening-5.2.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.2.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.2.3/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    46167 2023-07-15 10:14:05.000000 crypto-screening-5.2.3/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.2.3/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.2.3/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.2.3/crypto_screening/collect/orders.py
--rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.2.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.2.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    16881 2023-07-15 09:52:06.000000 crypto-screening-5.2.3/crypto_screening/collect/trades.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.2.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.2.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.2.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.112645 crypto-screening-5.2.3/crypto_screening/market/
--rw-rw-rw-   0        0        0    19625 2023-07-15 09:29:18.000000 crypto-screening-5.2.3/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.135735 crypto-screening-5.2.3/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.2.3/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.181040 crypto-screening-5.2.3/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    11038 2023-07-16 10:08:59.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20288 2023-07-16 10:07:11.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.2.3/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.2.3/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.2.3/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.2.3/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.2.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:16:31.046498 crypto-screening-5.2.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-16 10:16:30.000000 crypto-screening-5.2.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-16 10:16:29.000000 crypto-screening-5.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.2.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:16:31.182041 crypto-screening-5.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-16 10:16:26.000000 crypto-screening-5.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:21.044161 crypto-screening-5.3.0/
+-rw-rw-rw-   0        0        0       98 2023-07-16 14:20:19.000000 crypto-screening-5.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-16 14:20:21.043161 crypto-screening-5.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.3.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.3.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:20.943477 crypto-screening-5.3.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:20.981031 crypto-screening-5.3.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.3.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.3.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:20.984999 crypto-screening-5.3.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.3.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19466 2023-07-16 14:10:09.000000 crypto-screening-5.3.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17285 2023-07-16 14:09:02.000000 crypto-screening-5.3.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12446 2023-07-16 14:08:36.000000 crypto-screening-5.3.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:20.988000 crypto-screening-5.3.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.3.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    21649 2023-07-16 13:58:33.000000 crypto-screening-5.3.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    12917 2023-07-16 13:52:18.000000 crypto-screening-5.3.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    20738 2023-07-16 13:59:10.000000 crypto-screening-5.3.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15009 2023-07-16 14:08:22.000000 crypto-screening-5.3.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.3.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.3.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.3.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.3.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.3.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:20.994508 crypto-screening-5.3.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.3.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:21.010618 crypto-screening-5.3.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.3.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.3.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.3.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.3.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:21.043161 crypto-screening-5.3.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-16 14:17:05.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36682 2023-07-16 13:04:17.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20288 2023-07-16 14:16:54.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18061 2023-07-16 14:05:40.000000 crypto-screening-5.3.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.3.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.3.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.3.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.3.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:20:20.958889 crypto-screening-5.3.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-16 14:20:20.000000 crypto-screening-5.3.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2023-07-16 14:20:20.000000 crypto-screening-5.3.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 14:20:20.000000 crypto-screening-5.3.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-16 14:20:20.000000 crypto-screening-5.3.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-16 14:20:20.000000 crypto-screening-5.3.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-16 14:20:19.000000 crypto-screening-5.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.3.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 14:20:21.044161 crypto-screening-5.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-16 14:20:04.000000 crypto-screening-5.3.0/setup.py
```

### Comparing `crypto-screening-5.2.3/PKG-INFO` & `crypto-screening-5.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.3
+Version: 5.3.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.3/README.md` & `crypto-screening-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/build.py` & `crypto-screening-5.3.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/assets.py` & `crypto-screening-5.3.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/exchanges.py` & `crypto-screening-5.3.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/ohlcv.py` & `crypto-screening-5.3.0/crypto_screening/collect/market/ohlcv.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.ohlcv import (
-    create_ohlcv_dataframe
-)
-from crypto_screening.collect.market import (
-    MarketBase, assets_market_values, symbols_market_data,
+from crypto_screening.collect.market.state import (
+    MarketState, assets_market_values, OHLCV_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
-    is_symbol_in_symbols_market_values, assets_market_data,
-    assets_to_symbol_market_prices, assets_market_state,
-    symbol_to_assets_market_prices, symbols_market_state,
-    merge_assets_market_states, merge_symbols_market_states,
-    OHLCV_ATTRIBUTES
+    is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
+    assets_to_symbol_market_prices, assets_market_state_data,
+    symbol_to_assets_market_prices, symbols_market_state_data,
+    merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
 )
 
 __all__ = [
     "symbols_ohlcv_market_state",
     "merge_assets_ohlcv_market_states",
     "merge_symbols_ohlcv_market_states",
     "assets_ohlcv_market_state",
@@ -39,63 +35,68 @@
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 @define(repr=False)
 @represent
-class OHLCVMarketBase(MarketBase, metaclass=ABCMeta):
+class OHLCVMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
-        **MarketBase.__modifiers__
+        **MarketState.__modifiers__
     )
     __modifiers__.excluded.extend(["open", "high", "low", "close", "volume"])
+
+    ATTRIBUTES = OHLCV_ATTRIBUTES
 # end OrderbookMarketBase
 
 AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
 AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
 
 @define(repr=False)
 @represent
-class AssetsOHLCVMarketState(OHLCVMarketBase):
+class AssetsOHLCVMarketState(OHLCVMarketState, AssetsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
 
-    - bids:
-        The bids values of the assets.
+    - opens:
+        The open price values of the symbol.
+
+    - high:
+        The open price values of the symbol.
 
-    - asks:
-        The asks values of the assets.
+    - low:
+        The low price values of the symbol.
 
-    - bids_volume:
-        The bids volume values of the assets.
+    - close:
+        The close price values of the symbol.
 
-    - asks_volume:
-        The asks volume values of the assets.
+    - volume:
+        The volume price values of the symbol.
 
-    >>> from crypto_screening.collect.orderbook import AssetsOrderbookMarketState
+    >>> from crypto_screening.collect.market.ohlcv import assets_ohlcv_market_state
     >>>
     >>> state = assets_ohlcv_market_state(...)
     """
 
     opens: AssetsPrices
     highs: AssetsPrices
     lows: AssetsPrices
@@ -112,15 +113,15 @@
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.opens,
+            exchange=exchange, symbol=symbol, data=self.opens,
             separator=separator, provider=self
         )
     # end bid
 
     def high(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -131,15 +132,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.highs,
+            exchange=exchange, symbol=symbol, data=self.highs,
             separator=separator, provider=self
         )
     # end ask
 
     def low(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -150,15 +151,15 @@
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.lows,
+            exchange=exchange, symbol=symbol, data=self.lows,
             separator=separator, provider=self
         )
     # end bid_volume
 
     def close(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -169,15 +170,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.closes,
+            exchange=exchange, symbol=symbol, data=self.closes,
             separator=separator, provider=self
         )
     # end ask_volume
 
     def volume(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -188,15 +189,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.closes,
+            exchange=exchange, symbol=symbol, data=self.closes,
             separator=separator, provider=self
         )
     # end ask_volume
 
     def in_open_prices(
             self,
             exchange: str,
@@ -211,15 +212,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.opens
+            separator=separator, data=self.opens
         )
     # end in_bids_prices
 
     def in_high_prices(
             self,
             exchange: str,
             symbol: str,
@@ -233,15 +234,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.highs
+            separator=separator, data=self.highs
         )
     # end in_asks_prices
 
     def in_low_prices(
             self,
             exchange: str,
             symbol: str,
@@ -255,15 +256,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.lows
+            separator=separator, data=self.lows
         )
     # end in_bids_volume_prices
 
     def in_close_prices(
             self,
             exchange: str,
             symbol: str,
@@ -277,15 +278,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.closes
+            separator=separator, data=self.closes
         )
     # end in_asks_volume_prices
 
     def in_volume_prices(
             self,
             exchange: str,
             symbol: str,
@@ -299,54 +300,17 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.volumes
+            separator=separator, data=self.volumes
         )
     # end in_asks_volume_prices
-
-    def data(self) -> AssetsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return assets_market_data(
-            columns=OHLCV_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in OHLCV_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> AssetsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: AssetsMarketDatasets = {}
-
-        for exchange, bases in self.data().items():
-            for base, quotes in bases.items():
-                for quote, rows in quotes.items():
-                    dataset = create_ohlcv_dataframe()
-
-                    for time, row in rows:
-                        dataset.loc[time] = row
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end assets_market_state_to_datasets
 # end AssetsMarketStates
 
 def assets_ohlcv_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
@@ -360,54 +324,57 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return AssetsOHLCVMarketState(
         screeners=screeners,
-        **assets_market_state(
-            columns=OHLCV_ATTRIBUTES,
+        **assets_market_state_data(
+            columns=OHLCVMarketState.ATTRIBUTES,
             screeners=screeners, separator=separator,
             length=length, adjust=adjust
         )
     )
 # end assets_ohlcv_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
 @define(repr=False)
 @represent
-class SymbolsOHLCVMarketState(OHLCVMarketBase):
+class SymbolsOHLCVMarketState(OHLCVMarketState, SymbolsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
 
-    - bids:
-        The bids values of the assets.
+    - opens:
+        The open price values of the symbol.
 
-    - asks:
-        The asks values of the assets.
+    - high:
+        The open price values of the symbol.
 
-    - bids_volume:
-        The bids volume values of the assets.
+    - low:
+        The low price values of the symbol.
 
-    - asks_volume:
-        The asks volume values of the assets.
+    - close:
+        The close price values of the symbol.
 
-    >>> from crypto_screening.collect.orderbook import AssetsOrderbookMarketState
+    - volume:
+        The volume price values of the symbol.
+
+    >>> from crypto_screening.collect.market.ohlcv import symbols_ohlcv_market_state
     >>>
-    >>> state = assets_ohlcv_market_state(...)
+    >>> state = symbols_ohlcv_market_state(...)
     """
 
     opens: SymbolsPrices
     highs: SymbolsPrices
     lows: SymbolsPrices
     closes: SymbolsPrices
     volumes: SymbolsPrices
@@ -420,15 +387,15 @@
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.opens, provider=self
+            data=self.opens, provider=self
         )
     # end open
 
     def high(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
@@ -436,15 +403,15 @@
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.highs, provider=self
+            data=self.highs, provider=self
         )
     # end high
 
     def low(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the bid price for the symbol.
 
@@ -452,15 +419,15 @@
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.lows, provider=self
+            data=self.lows, provider=self
         )
     # end low
 
     def close(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
@@ -468,15 +435,15 @@
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.closes, provider=self
+            data=self.closes, provider=self
         )
     # end close
 
     def volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
@@ -484,127 +451,92 @@
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.volumes, provider=self
+            data=self.volumes, provider=self
         )
     # end volume
 
     def in_open_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.opens
+            exchange=exchange, symbol=symbol, data=self.opens
         )
     # end in_open_prices
 
     def in_high_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.highs
+            exchange=exchange, symbol=symbol, data=self.highs
         )
     # end in_high_prices
 
     def in_low_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.lows
+            exchange=exchange, symbol=symbol, data=self.lows
         )
     # end in_low_prices
 
     def in_close_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The in_asks_volume_prices value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.closes
+            exchange=exchange, symbol=symbol, data=self.closes
         )
     # end in_close_prices
 
     def in_volume_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The in_asks_volume_prices value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.volumes
+            exchange=exchange, symbol=symbol, data=self.volumes
         )
     # end in_volume_prices
-
-    def data(self) -> SymbolsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return symbols_market_data(
-            columns=OHLCV_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in OHLCV_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> SymbolsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: SymbolsMarketDatasets = {}
-
-        for exchange, symbols in self.data().items():
-            for symbol, rows in symbols.items():
-                dataset = create_ohlcv_dataframe()
-
-                for time, row in rows:
-                    dataset.loc[time] = row
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end symbols_market_state_to_datasets
 # end SymbolsMarketStates
 
 def symbols_ohlcv_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsOHLCVMarketState:
@@ -616,16 +548,16 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return SymbolsOHLCVMarketState(
         screeners=screeners,
-        **symbols_market_state(
-            columns=OHLCV_ATTRIBUTES, screeners=screeners,
+        **symbols_market_state_data(
+            columns=OHLCVMarketState.ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
         )
     )
 # end symbols_ohlcv_market_state
 
 def merge_symbols_ohlcv_market_states(
         *states: SymbolsOHLCVMarketState, sort: Optional[bool] = True
@@ -643,16 +575,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOHLCVMarketState(
         screeners=set(screeners),
-        **merge_symbols_market_states(
-            *states, prices={name: {} for name in OHLCV_ATTRIBUTES}, sort=sort
+        **merge_symbols_market_states_data(
+            *states, datas={
+                name: {} for name in OHLCVMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_symbols_ohlcv_market_states
 
 def merge_assets_ohlcv_market_states(
         *states: AssetsOHLCVMarketState, sort: Optional[bool] = True
 ) -> AssetsOHLCVMarketState:
@@ -669,16 +603,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOHLCVMarketState(
         screeners=set(screeners),
-        **merge_assets_market_states(
-            *states, prices={name: {} for name in OHLCV_ATTRIBUTES}, sort=sort
+        **merge_assets_market_states_data(
+            *states, datas={
+                name: {} for name in OHLCVMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_assets_ohlcv_market_states
 
 def assets_to_symbols_ohlcv_market_state(
         state: AssetsOHLCVMarketState,
         separator: Optional[str] = None
@@ -691,16 +627,16 @@
 
     :return: The results state.
     """
 
     return SymbolsOHLCVMarketState(
         **{
             name: assets_to_symbol_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in OHLCV_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in OHLCVMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_ohlcv_market_state
 
 def symbols_to_assets_ohlcv_market_state(
         state: SymbolsOHLCVMarketState,
         separator: Optional[str] = None
@@ -713,12 +649,12 @@
 
     :return: The results state.
     """
 
     return AssetsOHLCVMarketState(
         **{
             name: symbol_to_assets_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in OHLCV_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in OHLCVMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_ohlcv_market_state
```

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/orderbook.py` & `crypto-screening-5.3.0/crypto_screening/collect/market/orderbook.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.orderbook import (
-    create_orderbook_dataframe
-)
-from crypto_screening.collect.market import (
-    MarketBase, assets_market_values, assets_market_data,
+from crypto_screening.collect.market.state import (
+    MarketState, assets_market_values, ORDERBOOK_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
-    is_symbol_in_symbols_market_values, symbols_market_data,
-    assets_to_symbol_market_prices, assets_market_state,
-    symbol_to_assets_market_prices, symbols_market_state,
-    merge_assets_market_states, merge_symbols_market_states,
-    ORDERBOOK_ATTRIBUTES
+    is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
+    assets_to_symbol_market_prices, assets_market_state_data,
+    symbol_to_assets_market_prices, symbols_market_state_data,
+    merge_assets_market_states_data, SymbolsMarketState, AssetsMarketState
 )
 
 __all__ = [
     "symbols_orderbook_market_state",
     "merge_assets_orderbook_market_states",
     "merge_symbols_orderbook_market_states",
     "assets_orderbook_market_state",
@@ -39,39 +35,38 @@
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 @define(repr=False)
 @represent
-class OrderbookMarketBase(MarketBase, metaclass=ABCMeta):
+class OrderbookMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
-        **MarketBase.__modifiers__
+        **MarketState.__modifiers__
     )
     __modifiers__.excluded.extend(["bids", "asks", "bids_volume", "asks_volume"])
-# end OrderbookMarketBase
 
-AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
-AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
+    ATTRIBUTES = ORDERBOOK_ATTRIBUTES
+# end OrderbookMarketBase
 
 @define(repr=False)
 @represent
-class AssetsOrderbookMarketState(OrderbookMarketBase):
+class AssetsOrderbookMarketState(OrderbookMarketState, AssetsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
@@ -87,15 +82,15 @@
 
     - bids_volume:
         The bids volume values of the assets.
 
     - asks_volume:
         The asks volume values of the assets.
 
-    >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
+    >>> from crypto_screening.collect.market.orderbook import assets_orderbook_market_state
     >>>
     >>> state = assets_orderbook_market_state(...)
     """
 
     bids: AssetsPrices
     asks: AssetsPrices
     bids_volume: AssetsPrices
@@ -111,15 +106,15 @@
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.bids,
+            exchange=exchange, symbol=symbol, data=self.bids,
             separator=separator, provider=self
         )
     # end bid
 
     def ask(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -130,15 +125,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.asks,
+            exchange=exchange, symbol=symbol, data=self.asks,
             separator=separator, provider=self
         )
     # end ask
 
     def bid_volume(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -149,15 +144,15 @@
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.bids_volume,
+            exchange=exchange, symbol=symbol, data=self.bids_volume,
             separator=separator, provider=self
         )
     # end bid_volume
 
     def ask_volume(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -168,15 +163,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.asks_volume,
+            exchange=exchange, symbol=symbol, data=self.asks_volume,
             separator=separator, provider=self
         )
     # end ask_volume
 
     def in_bids_prices(
             self,
             exchange: str,
@@ -191,15 +186,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.bids
+            separator=separator, data=self.bids
         )
     # end in_bids_prices
 
     def in_asks_prices(
             self,
             exchange: str,
             symbol: str,
@@ -213,15 +208,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.asks
+            separator=separator, data=self.asks
         )
     # end in_asks_prices
 
     def in_bids_volume_prices(
             self,
             exchange: str,
             symbol: str,
@@ -235,15 +230,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.bids_volume
+            separator=separator, data=self.bids_volume
         )
     # end in_bids_volume_prices
 
     def in_asks_volume_prices(
             self,
             exchange: str,
             symbol: str,
@@ -257,54 +252,17 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.asks_volume
+            separator=separator, data=self.asks_volume
         )
     # end in_asks_volume_prices
-
-    def data(self) -> AssetsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return assets_market_data(
-            columns=ORDERBOOK_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in ORDERBOOK_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> AssetsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: AssetsMarketDatasets = {}
-
-        for exchange, bases in self.data().items():
-            for base, quotes in bases.items():
-                for quote, rows in quotes.items():
-                    dataset = create_orderbook_dataframe()
-
-                    for time, row in rows:
-                        dataset.loc[time] = row
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end assets_market_state_to_datasets
 # end AssetsMarketStates
 
 def assets_orderbook_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
@@ -318,28 +276,28 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return AssetsOrderbookMarketState(
         screeners=screeners,
-        **assets_market_state(
-            columns=ORDERBOOK_ATTRIBUTES,
+        **assets_market_state_data(
+            columns=OrderbookMarketState.ATTRIBUTES,
             screeners=screeners, separator=separator,
             length=length, adjust=adjust
         )
     )
 # end assets_orderbook_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
 @define(repr=False)
 @represent
-class SymbolsOrderbookMarketState(OrderbookMarketBase):
+class SymbolsOrderbookMarketState(OrderbookMarketState, SymbolsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
@@ -355,17 +313,17 @@
 
     - bids_volume:
         The bids volume values of the assets.
 
     - asks_volume:
         The asks volume values of the assets.
 
-    >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
+    >>> from crypto_screening.collect.market.orderbook import symbols_orderbook_market_state
     >>>
-    >>> state = assets_orderbook_market_state(...)
+    >>> state = symbols_orderbook_market_state(...)
     """
 
     bids: SymbolsPrices
     asks: SymbolsPrices
     bids_volume: SymbolsPrices
     asks_volume: SymbolsPrices
 
@@ -377,15 +335,15 @@
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.bids, provider=self
+            data=self.bids, provider=self
         )
     # end bid
 
     def ask(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
@@ -393,15 +351,15 @@
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.asks, provider=self
+            data=self.asks, provider=self
         )
     # end ask
 
     def bid_volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the bid price for the symbol.
 
@@ -409,15 +367,15 @@
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.bids_volume, provider=self
+            data=self.bids_volume, provider=self
         )
     # end bid_volume
 
     def ask_volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
@@ -425,112 +383,77 @@
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.asks_volume, provider=self
+            data=self.asks_volume, provider=self
         )
     # end ask_volume
 
     def in_bids_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.bids
+            exchange=exchange, symbol=symbol, data=self.bids
         )
     # end in_bids_prices
 
     def in_asks_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.asks
+            exchange=exchange, symbol=symbol, data=self.asks
         )
     # end in_asks_prices
 
     def in_bids_volume_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.bids_volume
+            exchange=exchange, symbol=symbol, data=self.bids_volume
         )
     # end in_bids_volume_prices
 
     def in_asks_volume_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The in_asks_volume_prices value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.asks_volume
+            exchange=exchange, symbol=symbol, data=self.asks_volume
         )
     # end in_asks_prices
-
-    def data(self) -> SymbolsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return symbols_market_data(
-            columns=ORDERBOOK_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in ORDERBOOK_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> SymbolsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: SymbolsMarketDatasets = {}
-
-        for exchange, symbols in self.data().items():
-            for symbol, rows in symbols.items():
-                dataset = create_orderbook_dataframe()
-
-                for time, row in rows:
-                    dataset.loc[time] = row
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end symbols_market_state_to_datasets
 # end SymbolsMarketStates
 
 def symbols_orderbook_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsOrderbookMarketState:
@@ -542,16 +465,16 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return SymbolsOrderbookMarketState(
         screeners=screeners,
-        **symbols_market_state(
-            columns=ORDERBOOK_ATTRIBUTES, screeners=screeners,
+        **symbols_market_state_data(
+            columns=OrderbookMarketState.ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
         )
     )
 # end symbols_orderbook_market_state
 
 def merge_symbols_orderbook_market_states(
         *states: SymbolsOrderbookMarketState, sort: Optional[bool] = True
@@ -569,16 +492,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOrderbookMarketState(
         screeners=set(screeners),
-        **merge_symbols_market_states(
-            *states, prices={name: {} for name in ORDERBOOK_ATTRIBUTES}, sort=sort
+        **merge_symbols_market_states_data(
+            *states, datas={
+                name: {} for name in OrderbookMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_symbols_ohlcv_market_states
 
 def merge_assets_orderbook_market_states(
         *states: AssetsOrderbookMarketState, sort: Optional[bool] = True
 ) -> AssetsOrderbookMarketState:
@@ -595,16 +520,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOrderbookMarketState(
         screeners=set(screeners),
-        **merge_assets_market_states(
-            *states, prices={name: {} for name in ORDERBOOK_ATTRIBUTES}, sort=sort
+        **merge_assets_market_states_data(
+            *states, datas={
+                name: {} for name in OrderbookMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_assets_ohlcv_market_states
 
 def assets_to_symbols_orderbook_market_state(
         state: AssetsOrderbookMarketState,
         separator: Optional[str] = None
@@ -617,16 +544,16 @@
 
     :return: The results state.
     """
 
     return SymbolsOrderbookMarketState(
         **{
             name: assets_to_symbol_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in ORDERBOOK_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in OrderbookMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_ohlcv_market_state
 
 def symbols_to_assets_orderbook_market_state(
         state: SymbolsOrderbookMarketState,
         separator: Optional[str] = None
@@ -639,12 +566,12 @@
 
     :return: The results state.
     """
 
     return AssetsOrderbookMarketState(
         **{
             name: symbol_to_assets_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in ORDERBOOK_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in OrderbookMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_ohlcv_market_state
```

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/orders.py` & `crypto-screening-5.3.0/crypto_screening/collect/market/orders.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.orders import (
-    create_orders_dataframe
-)
-from crypto_screening.collect.market import (
-    MarketBase, assets_market_values, assets_market_data,
+from crypto_screening.collect.market.state import (
+    MarketState, assets_market_values, ORDERS_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
-    is_symbol_in_symbols_market_values, symbols_market_data,
-    assets_to_symbol_market_prices, assets_market_state,
-    symbol_to_assets_market_prices, symbols_market_state,
-    merge_assets_market_states, merge_symbols_market_states,
-    ORDERS_ATTRIBUTES
+    is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
+    assets_to_symbol_market_prices, assets_market_state_data,
+    symbol_to_assets_market_prices, symbols_market_state_data,
+    merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
 )
 
 __all__ = [
     "symbols_orders_market_state",
     "merge_assets_orders_market_states",
     "merge_symbols_orders_market_states",
     "assets_orders_market_state",
@@ -39,39 +35,41 @@
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 @define(repr=False)
 @represent
-class OrdersMarketBase(MarketBase, metaclass=ABCMeta):
+class OrdersMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
-        **MarketBase.__modifiers__
+        **MarketState.__modifiers__
     )
     __modifiers__.excluded.extend(["bids", "asks"])
+
+    ATTRIBUTES = ORDERS_ATTRIBUTES
 # end OrderbookMarketBase
 
 AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
 AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
 
 @define(repr=False)
 @represent
-class AssetsOrdersMarketState(OrdersMarketBase):
+class AssetsOrdersMarketState(OrdersMarketState, AssetsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
@@ -81,17 +79,17 @@
 
     - bids:
         The bids values of the assets.
 
     - asks:
         The asks values of the assets.
 
-    >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
+    >>> from crypto_screening.collect.market.orders import assets_orders_market_state
     >>>
-    >>> state = assets_orderbook_market_state(...)
+    >>> state = assets_orders_market_state(...)
     """
 
     bids: AssetsPrices
     asks: AssetsPrices
 
     def bid(
             self, exchange: str, symbol: str, separator: Optional[str] = None
@@ -103,15 +101,15 @@
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.bids,
+            exchange=exchange, symbol=symbol, data=self.bids,
             separator=separator, provider=self
         )
     # end bid
 
     def ask(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -122,15 +120,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.asks,
+            exchange=exchange, symbol=symbol, data=self.asks,
             separator=separator, provider=self
         )
     # end ask
 
     def in_bids_prices(
             self,
             exchange: str,
@@ -145,15 +143,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.bids
+            separator=separator, data=self.bids
         )
     # end in_bids_prices
 
     def in_asks_prices(
             self,
             exchange: str,
             symbol: str,
@@ -167,54 +165,17 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.asks
+            separator=separator, data=self.asks
         )
     # end in_asks_prices
-
-    def data(self) -> AssetsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return assets_market_data(
-            columns=ORDERS_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in ORDERS_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> AssetsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: AssetsMarketDatasets = {}
-
-        for exchange, bases in self.data().items():
-            for base, quotes in bases.items():
-                for quote, rows in quotes.items():
-                    dataset = create_orders_dataframe()
-
-                    for time, row in rows:
-                        dataset.loc[time] = row
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end assets_market_state_to_datasets
 # end AssetsMarketStates
 
 def assets_orders_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
@@ -228,28 +189,28 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return AssetsOrdersMarketState(
         screeners=screeners,
-        **assets_market_state(
-            columns=ORDERS_ATTRIBUTES,
+        **assets_market_state_data(
+            columns=OrdersMarketState.ATTRIBUTES,
             screeners=screeners, separator=separator,
             length=length, adjust=adjust
         )
     )
 # end assets_orders_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
 @define(repr=False)
 @represent
-class SymbolsOrdersMarketState(OrdersMarketBase):
+class SymbolsOrdersMarketState(OrdersMarketState, SymbolsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
@@ -259,23 +220,17 @@
 
     - bids:
         The bids values of the assets.
 
     - asks:
         The asks values of the assets.
 
-    - bids_volume:
-        The bids volume values of the assets.
-
-    - asks_volume:
-        The asks volume values of the assets.
-
-    >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
+    >>> from crypto_screening.collect.market.orders import symbols_orders_market_state
     >>>
-    >>> state = assets_orderbook_market_state(...)
+    >>> state = symbols_orders_market_state(...)
     """
 
     bids: SymbolsPrices
     asks: SymbolsPrices
 
     def bid(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
@@ -285,15 +240,15 @@
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.bids, provider=self
+            data=self.bids, provider=self
         )
     # end bid
 
     def ask(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
@@ -301,82 +256,47 @@
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.asks, provider=self
+            data=self.asks, provider=self
         )
     # end ask
 
     def in_bids_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.bids
+            exchange=exchange, symbol=symbol, data=self.bids
         )
     # end in_bids_prices
 
     def in_asks_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.asks
+            exchange=exchange, symbol=symbol, data=self.asks
         )
     # end in_asks_prices
-
-    def data(self) -> SymbolsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return symbols_market_data(
-            columns=ORDERS_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in ORDERS_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> SymbolsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: SymbolsMarketDatasets = {}
-
-        for exchange, symbols in self.data().items():
-            for symbol, rows in symbols.items():
-                dataset = create_orders_dataframe()
-
-                for time, row in rows:
-                    dataset.loc[time] = row
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end symbols_market_state_to_datasets
 # end SymbolsMarketStates
 
 def symbols_orders_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsOrdersMarketState:
@@ -388,16 +308,16 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return SymbolsOrdersMarketState(
         screeners=screeners,
-        **symbols_market_state(
-            columns=ORDERS_ATTRIBUTES, screeners=screeners,
+        **symbols_market_state_data(
+            columns=OrdersMarketState.ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
         )
     )
 # end symbols_orders_market_state
 
 def merge_symbols_orders_market_states(
         *states: SymbolsOrdersMarketState, sort: Optional[bool] = True
@@ -415,16 +335,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOrdersMarketState(
         screeners=set(screeners),
-        **merge_symbols_market_states(
-            *states, prices={name: {} for name in ORDERS_ATTRIBUTES}, sort=sort
+        **merge_symbols_market_states_data(
+            *states, datas={
+                name: {} for name in OrdersMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_symbols_orders_market_states
 
 def merge_assets_orders_market_states(
         *states: AssetsOrdersMarketState, sort: Optional[bool] = True
 ) -> AssetsOrdersMarketState:
@@ -441,16 +363,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOrdersMarketState(
         screeners=set(screeners),
-        **merge_assets_market_states(
-            *states, prices={name: {} for name in ORDERS_ATTRIBUTES}, sort=sort
+        **merge_assets_market_states_data(
+            *states, datas={
+                name: {} for name in OrdersMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_assets_orders_market_states
 
 def assets_to_symbols_orders_market_state(
         state: AssetsOrdersMarketState,
         separator: Optional[str] = None
@@ -463,16 +387,16 @@
 
     :return: The results state.
     """
 
     return SymbolsOrdersMarketState(
         **{
             name: assets_to_symbol_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in ORDERS_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in OrdersMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_orders_market_state
 
 def symbols_to_assets_orders_market_state(
         state: SymbolsOrdersMarketState,
         separator: Optional[str] = None
@@ -485,12 +409,12 @@
 
     :return: The results state.
     """
 
     return AssetsOrdersMarketState(
         **{
             name: symbol_to_assets_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in ORDERS_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in OrdersMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_orders_market_state
```

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/screeners.py` & `crypto-screening-5.3.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/symbols.py` & `crypto-screening-5.3.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/collect/trades.py` & `crypto-screening-5.3.0/crypto_screening/collect/market/trades.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.trades import (
-    create_trades_dataframe
-)
-from crypto_screening.collect.market import (
-    MarketBase, assets_market_values, assets_market_data,
+from crypto_screening.collect.market.state import (
+    MarketState, assets_market_values, TRADES_ATTRIBUTES,
     is_symbol_in_assets_market_values, symbols_market_values,
-    is_symbol_in_symbols_market_values, symbols_market_data,
-    assets_to_symbol_market_prices, assets_market_state,
-    symbol_to_assets_market_prices, symbols_market_state,
-    merge_assets_market_states, merge_symbols_market_states,
-    TRADES_ATTRIBUTES
+    is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
+    assets_to_symbol_market_prices, assets_market_state_data,
+    symbol_to_assets_market_prices, symbols_market_state_data,
+    merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
 )
 
 __all__ = [
     "symbols_trades_market_state",
     "merge_assets_trades_market_states",
     "merge_symbols_trades_market_states",
     "assets_trades_market_state",
@@ -41,59 +37,64 @@
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 AssetsSides = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, str]]]]]
 SymbolsSides = Dict[str, Dict[str, List[Tuple[dt.datetime, str]]]]
 
 @define(repr=False)
 @represent
-class TradesMarketBase(MarketBase, metaclass=ABCMeta):
+class TradesMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
-        **MarketBase.__modifiers__
+        **MarketState.__modifiers__
     )
-    __modifiers__.excluded.extend(["amounts", "prices", "sides"])
+    __modifiers__.excluded.extend(["amounts", "values", "sides"])
+
+    ATTRIBUTES = TRADES_ATTRIBUTES
 # end OrderbookMarketBase
 
 AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
 AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
 
 @define(repr=False)
 @represent
-class AssetsTradesMarketState(TradesMarketBase):
+class AssetsTradesMarketState(TradesMarketState, AssetsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
 
-    - bids:
-        The bids values of the assets.
+    - amounts:
+        The volume of the base asset of each trade.
 
-    - asks:
-        The asks values of the assets.
+    - price:
+        The price of the base asset in the trade.
 
-    >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
+    - side:
+        The side on the trade.
+
+    >>> from crypto_screening.collect.market.trades import assets_trades_market_state
     >>>
-    >>> state = assets_orderbook_market_state(...)
+    >>> state = assets_trades_market_state(...)
     """
 
     amounts: AssetsPrices
     prices: AssetsPrices
     sides: AssetsSides
 
     def amount(
@@ -106,15 +107,15 @@
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.amounts,
+            exchange=exchange, symbol=symbol, data=self.amounts,
             separator=separator, provider=self
         )
     # end amount
 
     def price(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -125,15 +126,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.pricess,
+            exchange=exchange, symbol=symbol, data=self.pricess,
             separator=separator, provider=self
         )
     # end price
 
     def side(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, str]]:
@@ -144,15 +145,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, values=self.sides,
+            exchange=exchange, symbol=symbol, data=self.sides,
             separator=separator, provider=self
         )
     # end side
 
     def in_amounts_prices(
             self,
             exchange: str,
@@ -167,15 +168,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.amounts
+            separator=separator, data=self.amounts
         )
     # end in_amounts_prices
 
     def in_prices_prices(
             self,
             exchange: str,
             symbol: str,
@@ -189,15 +190,15 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.prices
+            separator=separator, data=self.prices
         )
     # end in_prices_prices
 
     def in_sides_prices(
             self,
             exchange: str,
             symbol: str,
@@ -211,54 +212,17 @@
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
         return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, values=self.sides
+            separator=separator, data=self.sides
         )
     # end in_sides_prices
-
-    def data(self) -> AssetsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return assets_market_data(
-            columns=TRADES_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in TRADES_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> AssetsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: AssetsMarketDatasets = {}
-
-        for exchange, bases in self.data().items():
-            for base, quotes in bases.items():
-                for quote, rows in quotes.items():
-                    dataset = create_trades_dataframe()
-
-                    for time, row in rows:
-                        dataset.loc[time] = row
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end assets_market_state_to_datasets
 # end AssetsMarketStates
 
 def assets_trades_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
@@ -272,54 +236,51 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return AssetsTradesMarketState(
         screeners=screeners,
-        **assets_market_state(
-            columns=TRADES_ATTRIBUTES,
+        **assets_market_state_data(
+            columns=TradesMarketState.ATTRIBUTES,
             screeners=screeners, separator=separator,
             length=length, adjust=adjust
         )
     )
 # end assets_orders_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
 @define(repr=False)
 @represent
-class SymbolsTradesMarketState(TradesMarketBase):
+class SymbolsTradesMarketState(TradesMarketState, SymbolsMarketState):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
 
-    - bids:
-        The bids values of the assets.
-
-    - asks:
-        The asks values of the assets.
+    - amounts:
+        The volume of the base asset of each trade.
 
-    - bids_volume:
-        The bids volume values of the assets.
+    - price:
+        The price of the base asset in the trade.
 
-    - asks_volume:
-        The asks volume values of the assets.
+    - side:
+        The side on the trade.
 
-    >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
+    >>> from crypto_screening.collect.market.trades import symbols_trades_market_state
     >>>
-    >>> state = assets_orderbook_market_state(...)
+    >>> state = symbols_trades_market_state(...)
     """
 
     amounts: SymbolsPrices
     prices: SymbolsPrices
     sides: SymbolsSides
 
     def amount(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
@@ -329,15 +290,15 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.amounts,
+            exchange=exchange, symbol=symbol, data=self.amounts,
             provider=self
         )
     # end amount
 
     def price(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
@@ -345,15 +306,15 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.pricess,
+            exchange=exchange, symbol=symbol, data=self.pricess,
             provider=self
         )
     # end price
 
     def side(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, str]]:
         """
         Returns the ask price for the symbol.
@@ -362,97 +323,62 @@
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            values=self.sides, provider=self
+            data=self.sides, provider=self
         )
     # end side
 
     def in_amounts_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.amounts
+            exchange=exchange, symbol=symbol, data=self.amounts
         )
     # end in_amounts_prices
 
     def in_prices_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.prices
+            exchange=exchange, symbol=symbol, data=self.prices
         )
     # end in_prices_prices
 
     def in_sides_prices(self, exchange: str, symbol: str) -> bool:
         """
         Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
         return is_symbol_in_symbols_market_values(
-            exchange=exchange, symbol=symbol, values=self.sides
+            exchange=exchange, symbol=symbol, data=self.sides
         )
     # end in_sides_prices
-
-    def data(self) -> SymbolsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        return symbols_market_data(
-            columns=TRADES_ATTRIBUTES,
-            prices={name: getattr(self, name) for name in TRADES_ATTRIBUTES}
-        )
-    # end data
-
-    def datasets(self) -> SymbolsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: SymbolsMarketDatasets = {}
-
-        for exchange, symbols in self.data().items():
-            for symbol, rows in symbols.items():
-                dataset = create_trades_dataframe()
-
-                for time, row in rows:
-                    dataset.loc[time] = row
-                # end for
-            # end for
-        # end for
-
-        return datasets
-    # end symbols_market_state_to_datasets
 # end SymbolsMarketStates
 
 def symbols_trades_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsTradesMarketState:
@@ -464,16 +390,16 @@
     :param adjust: The value to adjust the length of the sequences.
 
     :return: The values of the assets.
     """
 
     return SymbolsTradesMarketState(
         screeners=screeners,
-        **symbols_market_state(
-            columns=TRADES_ATTRIBUTES, screeners=screeners,
+        **symbols_market_state_data(
+            columns=TradesMarketState.ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
         )
     )
 # end symbols_orders_market_state
 
 def merge_symbols_trades_market_states(
         *states: SymbolsTradesMarketState, sort: Optional[bool] = True
@@ -491,16 +417,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsTradesMarketState(
         screeners=set(screeners),
-        **merge_symbols_market_states(
-            *states, prices={name: {} for name in TRADES_ATTRIBUTES}, sort=sort
+        **merge_symbols_market_states_data(
+            *states, datas={
+                name: {} for name in TradesMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_symbols_orders_market_states
 
 def merge_assets_trades_market_states(
         *states: AssetsTradesMarketState, sort: Optional[bool] = True
 ) -> AssetsTradesMarketState:
@@ -517,16 +445,18 @@
 
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsTradesMarketState(
         screeners=set(screeners),
-        **merge_assets_market_states(
-            *states, prices={name: {} for name in TRADES_ATTRIBUTES}, sort=sort
+        **merge_assets_market_states_data(
+            *states, datas={
+                name: {} for name in TradesMarketState.ATTRIBUTES
+            }, sort=sort
         )
     )
 # end merge_assets_orders_market_states
 
 def assets_to_symbols_trades_market_state(
         state: AssetsTradesMarketState,
         separator: Optional[str] = None
@@ -539,16 +469,16 @@
 
     :return: The results state.
     """
 
     return SymbolsTradesMarketState(
         **{
             name: assets_to_symbol_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in TRADES_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in TradesMarketState.ATTRIBUTES
         }
     )
 # end assets_to_symbols_orders_market_state
 
 def symbols_to_assets_trades_market_state(
         state: SymbolsTradesMarketState,
         separator: Optional[str] = None
@@ -561,12 +491,12 @@
 
     :return: The results state.
     """
 
     return AssetsTradesMarketState(
         **{
             name: symbol_to_assets_market_prices(
-                prices=getattr(state, name), separator=separator
-            ) for name in TRADES_ATTRIBUTES
+                data=getattr(state, name), separator=separator
+            ) for name in TradesMarketState.ATTRIBUTES
         }
     )
 # end symbols_to_assets_orders_market_state
```

### Comparing `crypto-screening-5.2.3/crypto_screening/dataset.py` & `crypto-screening-5.3.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/interval.py` & `crypto-screening-5.3.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/dynamic.py` & `crypto-screening-5.3.0/crypto_screening/market/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from represent import Modifiers
 
 import pandas as pd
 
 from crypto_screening.collect.screeners import exchanges_symbols_screeners
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
-from crypto_screening.collect.orderbook import (
+from crypto_screening.collect.market.orderbook import (
     assets_orderbook_market_state, symbols_orderbook_market_state,
     SymbolsOrderbookMarketState, AssetsOrderbookMarketState
 )
-from crypto_screening.collect.ohlcv import (
+from crypto_screening.collect.market.ohlcv import (
     assets_ohlcv_market_state, symbols_ohlcv_market_state,
     SymbolsOHLCVMarketState, AssetsOHLCVMarketState
 )
-from crypto_screening.collect.orders import (
+from crypto_screening.collect.market.orders import (
     assets_orders_market_state, symbols_orders_market_state,
     SymbolsOrdersMarketState, AssetsOrdersMarketState
 )
-from crypto_screening.collect.trades import (
+from crypto_screening.collect.market.trades import (
     assets_trades_market_state, symbols_trades_market_state,
     SymbolsTradesMarketState, AssetsTradesMarketState
 )
 from crypto_screening.market.screeners.container import ScreenersContainer
 
 __all__ = [
     "DynamicScreener"
@@ -107,15 +107,15 @@
 
         except ValueError:
             screener = self.find_screeners(
                 exchange=exchange, symbol=symbol
             )[0]
 
             if isinstance(screener, OHLCVScreener):
-                market = screener.base_market
+                market = screener.orderbook_market
 
             else:
                 market = screener.market
             # end if
         # end try
 
         length = min(length or 0, len(market))
```

### Comparing `crypto-screening-5.2.3/crypto_screening/market/foundation/data.py` & `crypto-screening-5.3.0/crypto_screening/market/foundation/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         '_saving_process', '_update_process',
         '_updating', '_saving', '_blocking',
         '_screening', "location", "delay", "cancel"
     )
 
     LOCATION = "datasets"
 
-    DELAY = 0.0
+    DELAY = 0
     CANCEL = 0
 
     def __init__(
             self,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None
```

### Comparing `crypto-screening-5.2.3/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.3.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/foundation/state.py` & `crypto-screening-5.3.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.3.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/base.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     - market:
         The dataset of the market data.
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.append("market")
 
-    MINIMUM_DELAY = 0.1
+    MINIMUM_DELAY = 1
 
     __slots__ = "symbol", "exchange", "market"
 
     def __init__(
             self,
             symbol: str,
             exchange: str,
@@ -229,17 +229,15 @@
         while self.saving:
             start = time.time()
 
             self.save_dataset()
 
             end = time.time()
 
-            if delay - (end - start) <= 0:
-                time.sleep(max([delay - (end - start), self.MINIMUM_DELAY]))
-            # end if
+            time.sleep(max([delay - (end - start), self.MINIMUM_DELAY]))
         # end while
     # end saving_loop
 # end BaseScreener
 
 class BaseMultiScreener(DataCollector):
     """
     A class to represent an asset price screener.
```

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/container.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,37 +128,37 @@
             symbol: str,
             exchange: str,
             interval: Optional[str] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             market: Optional[pd.DataFrame] = None,
-            base_market: Optional[pd.DataFrame] = None
+            orderbook_market: Optional[pd.DataFrame] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param symbol: The symbol of the asset.
         :param interval: The interval for the data.
         :param exchange: The exchange to get source data from.
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         :param market: The data for the market.
-        :param base_market: The base market dataset.
+        :param orderbook_market: The base market dataset.
         """
 
         super().__init__(
             symbol=symbol, exchange=exchange, location=location,
             cancel=cancel, delay=delay, market=market
         )
 
         self.interval = self.validate_interval(interval or self.INTERVAL)
 
-        self.base_market = base_market
+        self.orderbook_market = orderbook_market
     # end __init__
 
     @staticmethod
     def validate_interval(interval: str) -> str:
         """
         Validates the symbol value.
 
@@ -167,25 +167,14 @@
         :return: The validates symbol.
         """
 
         return validate_interval(interval=interval)
     # end validate_symbol
 
     @property
-    def orderbook_market(self) -> pd.DataFrame:
-        """
-        Returns the market to hold the recorder data.
-
-        :return: The market object.
-        """
-
-        return self.base_market
-    # end orderbook_market
-
-    @property
     def ohlcv_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
@@ -327,15 +316,15 @@
         Creates the orderbook screener object.
 
         :return: The orderbook screener.
         """
 
         return OrderbookScreener(
             symbol=self.symbol, exchange=self.exchange, location=self.location,
-            cancel=self.cancel, delay=self.delay, market=self.base_market
+            cancel=self.cancel, delay=self.delay, market=self.orderbook_market
         )
     # end orderbook_screener
 # end OHLCVScreener
 
 def validate_intervals(data: Any) -> Intervals:
     """
     Validates the data.
@@ -942,15 +931,15 @@
     def connect_screeners(self) -> None:
         """Connects the screeners to the recording object."""
 
         super().connect_screeners()
 
         for screener in self.screeners:
             if isinstance(screener, OHLCVScreener):
-                screener.base_market = self.recorder.orderbook(
+                screener.orderbook_market = self.recorder.orderbook(
                     exchange=screener.exchange, symbol=screener.symbol
                 )
                 screener.market = self.recorder.ohlcv(
                     exchange=screener.exchange, symbol=screener.symbol,
                     interval=screener.interval
                 )
         # end for
@@ -1031,15 +1020,15 @@
             location=location, cancel=cancel, market=(
                 self.ohlcv(
                     exchange=exchange, symbol=symbol, interval=interval
                 ) if self.ohlcv_in_market(
                     symbol=symbol, exchange=exchange, interval=interval
                 ) else None
             ),
-            base_market=(
+            orderbook_market=(
                 self.orderbook(exchange=exchange, symbol=symbol)
                 if self.orderbook_in_market(symbol=symbol, exchange=exchange)
                 else None
             )
         )
 
         container.setdefault(exchange, {})[symbol] = screener
```

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.3.0/crypto_screening/market/screeners/trades.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,14 @@
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
     COLUMNS = TRADES_COLUMNS
 
-
     @property
     def trades_market(self) -> Market:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
```

### Comparing `crypto-screening-5.2.3/crypto_screening/market/waiting.py` & `crypto-screening-5.3.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/process.py` & `crypto-screening-5.3.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/symbols.py` & `crypto-screening-5.3.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening/validate.py` & `crypto-screening-5.3.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.3.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.3
+Version: 5.3.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.3.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,25 @@
 crypto_screening.egg-info/PKG-INFO
 crypto_screening.egg-info/SOURCES.txt
 crypto_screening.egg-info/dependency_links.txt
 crypto_screening.egg-info/requires.txt
 crypto_screening.egg-info/top_level.txt
 crypto_screening/collect/assets.py
 crypto_screening/collect/exchanges.py
-crypto_screening/collect/market.py
-crypto_screening/collect/ohlcv.py
-crypto_screening/collect/orderbook.py
-crypto_screening/collect/orders.py
 crypto_screening/collect/screeners.py
 crypto_screening/collect/symbols.py
-crypto_screening/collect/trades.py
+crypto_screening/collect/market/__init__.py
+crypto_screening/collect/market/ohlcv.py
+crypto_screening/collect/market/orderbook.py
+crypto_screening/collect/market/orders.py
+crypto_screening/collect/market/trades.py
+crypto_screening/collect/market/state/__init__.py
+crypto_screening/collect/market/state/assets.py
+crypto_screening/collect/market/state/base.py
+crypto_screening/collect/market/state/symbols.py
 crypto_screening/market/dynamic.py
 crypto_screening/market/waiting.py
 crypto_screening/market/foundation/data.py
 crypto_screening/market/foundation/protocols.py
 crypto_screening/market/foundation/state.py
 crypto_screening/market/foundation/waiting.py
 crypto_screening/market/screeners/__init__.py
```

### Comparing `crypto-screening-5.2.3/pyproject.toml` & `crypto-screening-5.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.2.3'
+version = '5.3.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.2.3/setup.py` & `crypto-screening-5.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='5.2.3',
+        version='5.3.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

