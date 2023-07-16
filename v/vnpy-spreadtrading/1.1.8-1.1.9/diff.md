# Comparing `tmp/vnpy_spreadtrading-1.1.8.tar.gz` & `tmp/vnpy_spreadtrading-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_spreadtrading-1.1.8.tar", last modified: Sun Apr 23 04:36:18 2023, max compression
+gzip compressed data, was "vnpy_spreadtrading-1.1.9.tar", last modified: Sun Jul 16 07:44:40 2023, max compression
```

## Comparing `vnpy_spreadtrading-1.1.8.tar` & `vnpy_spreadtrading-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.563910 vnpy_spreadtrading-1.1.8/
--rw-rw-rw-   0        0        0     1107 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     2020 2023-04-23 04:36:18.563910 vnpy_spreadtrading-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-04-23 04:35:29.000000 vnpy_spreadtrading-1.1.8/README.md
--rw-rw-rw-   0        0        0     1100 2023-04-23 04:36:18.565956 vnpy_spreadtrading-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.496542 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/
--rw-rw-rw-   0        0        0     1988 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/__init__.py
--rw-rw-rw-   0        0        0     5773 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/algo.py
--rw-rw-rw-   0        0        0    26351 2023-03-27 06:55:55.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/backtesting.py
--rw-rw-rw-   0        0        0    17129 2023-03-27 06:55:11.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/base.py
--rw-rw-rw-   0        0        0    35634 2023-02-16 00:38:43.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/engine.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.559289 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/__init__.py
--rw-rw-rw-   0        0        0     5102 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/basic_spread_strategy.py
--rw-rw-rw-   0        0        0     4556 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py
--rw-rw-rw-   0        0        0    22457 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/template.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.562889 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/
--rw-rw-rw-   0        0        0       35 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/__init__.py
--rw-rw-rw-   0        0        0    67646 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/spread.ico
--rw-rw-rw-   0        0        0    29116 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.553134 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/
--rw-rw-rw-   0        0        0     2020 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 07:44:40.236909 vnpy_spreadtrading-1.1.9/
+-rw-rw-rw-   0        0        0     1107 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2020 2023-07-16 07:44:40.236909 vnpy_spreadtrading-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2023-07-16 07:43:49.000000 vnpy_spreadtrading-1.1.9/README.md
+-rw-rw-rw-   0        0        0     1100 2023-07-16 07:44:40.237904 vnpy_spreadtrading-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:44:40.169214 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/
+-rw-rw-rw-   0        0        0     1988 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/__init__.py
+-rw-rw-rw-   0        0        0     5773 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/algo.py
+-rw-rw-rw-   0        0        0    27229 2023-07-16 07:41:15.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/backtesting.py
+-rw-rw-rw-   0        0        0    18298 2023-07-16 07:41:15.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/base.py
+-rw-rw-rw-   0        0        0    37243 2023-07-16 07:41:15.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/engine.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:44:40.231804 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/strategies/
+-rw-rw-rw-   0        0        0        0 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5102 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/strategies/basic_spread_strategy.py
+-rw-rw-rw-   0        0        0     4556 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py
+-rw-rw-rw-   0        0        0    23134 2023-07-16 07:41:15.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/template.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:44:40.235886 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/ui/
+-rw-rw-rw-   0        0        0       35 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/ui/__init__.py
+-rw-rw-rw-   0        0        0    67646 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/ui/spread.ico
+-rw-rw-rw-   0        0        0    29690 2023-07-16 07:41:15.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:44:40.228202 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/
+-rw-rw-rw-   0        0        0     2020 2023-07-16 07:44:39.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2023-07-16 07:44:40.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:44:39.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-16 07:44:39.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-07-16 07:44:39.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-16 07:44:39.000000 vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/top_level.txt
```

### Comparing `vnpy_spreadtrading-1.1.8/LICENSE` & `vnpy_spreadtrading-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.8/PKG-INFO` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vnpy_spreadtrading
-Version: 1.1.8
+Name: vnpy-spreadtrading
+Version: 1.1.9
 Summary: Spread trading application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的价差交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_spreadtrading-1.1.8/README.md` & `vnpy_spreadtrading-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的价差交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_spreadtrading-1.1.8/setup.cfg` & `vnpy_spreadtrading-1.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7370 7265 6164 7472   = vnpy_spreadtr
 00000020: 6164 696e 670d 0a76 6572 7369 6f6e 203d  ading..version =
-00000030: 2031 2e31 2e38 0d0a 7572 6c20 3d20 6874   1.1.8..url = ht
+00000030: 2031 2e31 2e39 0d0a 7572 6c20 3d20 6874   1.1.9..url = ht
 00000040: 7470 733a 2f2f 7777 772e 766e 7079 2e63  tps://www.vnpy.c
 00000050: 6f6d 0d0a 6c69 6365 6e73 6520 3d20 4d49  om..license = MI
 00000060: 540d 0a61 7574 686f 7220 3d20 5869 616f  T..author = Xiao
 00000070: 796f 7520 4368 656e 0d0a 6175 7468 6f72  you Chen..author
 00000080: 5f65 6d61 696c 203d 2078 6961 6f79 6f75  _email = xiaoyou
 00000090: 2e63 6865 6e40 6d61 696c 2e76 6e70 792e  .chen@mail.vnpy.
 000000a0: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
```

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/__init__.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/algo.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/algo.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/backtesting.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/backtesting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import traceback
 from collections import defaultdict
-from datetime import date, datetime
+from datetime import date, datetime, timedelta
 from typing import Callable, Type, Dict, List, Optional
 from functools import partial
 
 import numpy as np
 from pandas import DataFrame
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
@@ -20,20 +21,35 @@
     OptimizationSetting,
     check_optimization_setting,
     run_bf_optimization,
     run_ga_optimization
 )
 
 from .template import SpreadStrategyTemplate, SpreadAlgoTemplate
-from .base import SpreadData, BacktestingMode, load_bar_data, load_tick_data
+from .base import (
+    SpreadData,
+    BacktestingMode,
+    load_bar_data,
+    load_tick_data,
+    EngineType
+)
+
+
+INTERVAL_DELTA_MAP: Dict[Interval, timedelta] = {
+    Interval.TICK: timedelta(milliseconds=1),
+    Interval.MINUTE: timedelta(minutes=1),
+    Interval.HOUR: timedelta(hours=1),
+    Interval.DAILY: timedelta(days=1),
+}
 
 
 class BacktestingEngine:
     """"""
 
+    engine_type: EngineType = EngineType.BACKTESTING
     gateway_name: str = "BACKTESTING"
 
     def __init__(self) -> None:
         """"""
         self.spread: SpreadData = None
 
         self.start: datetime = None
@@ -162,48 +178,37 @@
         """"""
         if self.mode == BacktestingMode.BAR:
             func = self.new_bar
         else:
             func = self.new_tick
 
         self.strategy.on_init()
-
-        # Use the first [days] of history data for initializing strategy
-        day_count: int = 0
-        ix: int = 0
-
-        for ix, data in enumerate(self.history_data):
-            if self.datetime and data.datetime.day != self.datetime.day:
-                day_count += 1
-                if day_count >= self.days:
-                    break
-
-            self.datetime = data.datetime
-            self.callback(data)
-
         self.strategy.inited = True
         self.output("策略初始化完成")
 
         self.strategy.on_start()
         self.strategy.trading = True
         self.output("开始回放历史数据")
 
-        # Use the rest of history data for running backtesting
-        for data in self.history_data[ix:]:
-            func(data)
+        for data in self.history_data:
+            try:
+                func(data)
+            except Exception:
+                self.output("触发异常，回测终止")
+                self.output(traceback.format_exc())
+                return
 
         self.output("历史数据回放结束")
 
     def calculate_result(self) -> DataFrame:
         """"""
         self.output("开始计算逐日盯市盈亏")
 
         if not self.trades:
-            self.output("成交记录为空，无法计算")
-            return
+            self.output("回测成交记录为空")
 
         # Add trade data into daily reuslt.
         for trade in self.trades.values():
             d: date = trade.datetime.date()
             daily_result = self.daily_results[d]
             daily_result.add_trade(trade)
 
@@ -587,21 +592,50 @@
 
             self.trades[trade.vt_tradeid] = trade
 
     def load_bar(
         self, spread: SpreadData, days: int, interval: Interval, callback: Callable
     ) -> None:
         """"""
-        self.days = days
         self.callback = callback
 
+        init_end = self.start - INTERVAL_DELTA_MAP[interval]
+        init_start = self.start - timedelta(days=days)
+
+        bars: List[BarData] = load_bar_data(
+            spread=self.spread,
+            interval=self.interval,
+            start=init_start,
+            end=init_end,
+            pricetick=self.pricetick,
+            backtesting=True
+        )
+
+        for bar in bars:
+            callback(bar)
+
+        return bars
+
     def load_tick(self, spread: SpreadData, days: int, callback: Callable) -> None:
         """"""
         self.days = days
-        self.callback = callback
+
+        init_end = self.start - INTERVAL_DELTA_MAP[Interval.TICK]
+        init_start = self.start - timedelta(days=days)
+
+        ticks: List[TickData] = load_tick_data(
+            self.spread,
+            init_start,
+            init_end
+        )
+
+        for tick in ticks:
+            callback(callback)
+
+        return ticks
 
     def start_algo(
         self,
         strategy: SpreadStrategyTemplate,
         spread_name: str,
         direction: Direction,
         price: float,
@@ -674,14 +708,20 @@
 
     def send_email(self, msg: str, strategy: SpreadStrategyTemplate = None) -> None:
         """
         Send email to default receiver.
         """
         pass
 
+    def get_engine_type(self) -> EngineType:
+        """
+        Return engine type.
+        """
+        return self.engine_type
+
     def put_strategy_event(self, strategy: SpreadStrategyTemplate) -> None:
         """
         Put an event to update strategy status.
         """
         pass
 
     def write_algo_log(self, algo: SpreadAlgoTemplate, msg: str) -> None:
@@ -797,15 +837,15 @@
     engine.add_strategy(strategy_class, setting)
     engine.load_data()
     engine.run_backtesting()
     engine.calculate_result()
     statistics: dict = engine.calculate_statistics(output=False)
 
     target_value: float = statistics[target_name]
-    return (str(setting), target_value, statistics)
+    return (setting, target_value, statistics)
 
 
 def wrap_evaluate(engine: BacktestingEngine, target_name: str) -> callable:
     """
     Wrap evaluate function with given setting from backtesting engine.
     """
     func: callable = partial(
```

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/base.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Callable
 from datetime import datetime
 from enum import Enum
 from tzlocal import get_localzone_name
+from dataclasses import dataclass
 
 from vnpy.trader.object import (
     HistoryRequest, TickData, PositionData, TradeData, ContractData, BarData
 )
-from vnpy.trader.constant import Direction, Offset, Exchange, Interval
+from vnpy.trader.constant import Direction, Offset, Exchange, Interval, Status
 from vnpy.trader.utility import floor_to, ceil_to, round_to, extract_vt_symbol, ZoneInfo
 from vnpy.trader.database import BaseDatabase, get_database
 from vnpy.trader.datafeed import BaseDatafeed, get_datafeed
 
 
 EVENT_SPREAD_DATA = "eSpreadData"
 EVENT_SPREAD_POS = "eSpreadPos"
@@ -382,14 +383,34 @@
 
     def parse_formula(self, formula: str, data: Dict[str, float]) -> Any:
         """"""
         locals().update(data)
         value = eval(formula)
         return value
 
+    def get_item(self) -> None:
+        """获取数据对象"""
+        item: SpreadItem = SpreadItem(
+            name=self.name,
+            bid_volume=self.bid_volume,
+            bid_price=self.bid_price,
+            ask_price=self.ask_price,
+            ask_volume=self.ask_volume,
+            net_pos=self.net_pos,
+            datetime=self.datetime,
+            price_formula=self.price_formula,
+            trading_formula=self.trading_formula,
+        )
+        return item
+
+
+class EngineType(Enum):
+    LIVE = "实盘"
+    BACKTESTING = "回测"
+
 
 class BacktestingMode(Enum):
     BAR = 1
     TICK = 2
 
 
 def load_bar_data(
@@ -407,15 +428,15 @@
     # Load bar data of each spread leg
     leg_bars: Dict[str, Dict] = {}
 
     for vt_symbol in spread.legs.keys():
         symbol, exchange = extract_vt_symbol(vt_symbol)
 
         # 初始化K线列表
-        bar_data: List[BarData] = [] 
+        bar_data: List[BarData] = []
 
         # 只有实盘才优先尝试从数据服务查询
         if not backtesting:
             bar_data = query_bar_from_datafeed(
                 symbol, exchange, interval, start, end, output
             )
 
@@ -502,7 +523,39 @@
         exchange=exchange,
         interval=interval,
         start=start,
         end=end
     )
     data: List[BarData] = datafeed.query_bar_history(req, output)
     return data
+
+
+@dataclass
+class SpreadItem:
+    """价差数据容器"""
+
+    name: str
+    bid_volume: int
+    bid_price: float
+    ask_price: float
+    ask_volume: int
+    net_pos: int
+    datetime: datetime
+    price_formula: str
+    trading_formula: str
+
+
+@dataclass
+class AlgoItem:
+    """算法数据容器"""
+
+    algoid: str
+    spread_name: str
+    direction: Direction
+    price: float
+    payup: int
+    volume: float
+    traded_volume: float
+    traded_price: float
+    interval: int
+    count: int
+    status: Status
```

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/engine.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 )
 
 from .base import (
     LegData, SpreadData,
     EVENT_SPREAD_DATA, EVENT_SPREAD_POS,
     EVENT_SPREAD_ALGO, EVENT_SPREAD_LOG,
     EVENT_SPREAD_STRATEGY,
-    load_bar_data, load_tick_data
+    load_bar_data, load_tick_data,
+    EngineType
 )
 from .template import SpreadAlgoTemplate, SpreadStrategyTemplate
 from .algo import SpreadTakerAlgo
 
 
 APP_NAME = "SpreadTrading"
 
@@ -43,26 +44,51 @@
 
     def __init__(self, main_engine: MainEngine, event_engine: EventEngine) -> None:
         """Constructor"""
         super().__init__(main_engine, event_engine, APP_NAME)
 
         self.active: bool = False
 
+        self.init_data_engine()
+        self.init_algo_engine()
+        self.init_strategy_engine()
+
+    def init_data_engine(self) -> None:
+        """初始化数据引擎"""
         self.data_engine: SpreadDataEngine = SpreadDataEngine(self)
-        self.algo_engine: SpreadAlgoEngine = SpreadAlgoEngine(self)
-        self.strategy_engine: SpreadStrategyEngine = SpreadStrategyEngine(self)
 
         self.add_spread = self.data_engine.add_spread
         self.remove_spread = self.data_engine.remove_spread
         self.get_spread = self.data_engine.get_spread
-        self.get_all_spreads = self.data_engine.get_all_spreads
+        self.get_all_spread_names = self.data_engine.get_all_spread_names
+
+    def init_algo_engine(self) -> None:
+        """初始化算法引擎"""
+        self.algo_engine: SpreadAlgoEngine = SpreadAlgoEngine(self)
 
         self.start_algo = self.algo_engine.start_algo
         self.stop_algo = self.algo_engine.stop_algo
 
+    def init_strategy_engine(self) -> None:
+        """初始化策略引擎"""
+        self.strategy_engine: SpreadStrategyEngine = SpreadStrategyEngine(self)
+
+        self.get_all_strategy_class_names = self.strategy_engine.get_all_strategy_class_names
+        self.get_strategy_class_parameters = self.strategy_engine.get_strategy_class_parameters
+        self.init_all_strategies = self.strategy_engine.init_all_strategies
+        self.start_all_strategies = self.strategy_engine.start_all_strategies
+        self.stop_all_strategies = self.strategy_engine.stop_all_strategies
+        self.add_strategy = self.strategy_engine.add_strategy
+        self.init_strategy = self.strategy_engine.init_strategy
+        self.start_strategy = self.strategy_engine.start_strategy
+        self.stop_strategy = self.strategy_engine.stop_strategy
+        self.get_strategy_parameters = self.strategy_engine.get_strategy_parameters
+        self.edit_strategy = self.strategy_engine.edit_strategy
+        self.remove_strategy = self.strategy_engine.remove_strategy
+
     def start(self) -> None:
         """"""
         if self.active:
             return
         self.active = True
 
         self.data_engine.start()
@@ -80,14 +106,27 @@
         log: LegData = LogData(
             msg=msg,
             gateway_name=APP_NAME
         )
         event: Event = Event(EVENT_SPREAD_LOG, log)
         self.event_engine.put(event)
 
+    def update_spread_data(self, spread: SpreadData) -> None:
+        """"""
+        self.algo_engine.update_spread_data(spread)
+        self.strategy_engine.update_spread_data(spread)
+
+    def update_spread_pos(self, spread: SpreadData) -> None:
+        """"""
+        self.strategy_engine.update_spread_pos(spread)
+
+    def update_spread_algo(self, algo: SpreadAlgoTemplate) -> None:
+        """"""
+        self.strategy_engine.update_spread_algo(algo)
+
 
 class SpreadDataEngine:
     """"""
     setting_filename: str = "spread_trading_setting.json"
     pos_filename: str = "spread_trading_pos.json"
 
     def __init__(self, spread_engine: SpreadEngine) -> None:
@@ -242,20 +281,24 @@
             req: SubscribeRequest = SubscribeRequest(
                 contract.symbol, contract.exchange
             )
             self.main_engine.subscribe(req, contract.gateway_name)
 
     def put_data_event(self, spread: SpreadData) -> None:
         """"""
-        event: Event = Event(EVENT_SPREAD_DATA, spread)
+        self.spread_engine.update_spread_data(spread)
+
+        event: Event = Event(EVENT_SPREAD_DATA, spread.get_item())
         self.event_engine.put(event)
 
     def put_pos_event(self, spread: SpreadData) -> None:
         """"""
-        event: Event = Event(EVENT_SPREAD_POS, spread)
+        self.spread_engine.update_spread_pos(spread)
+
+        event: Event = Event(EVENT_SPREAD_POS, spread.get_item())
         self.event_engine.put(event)
 
     def get_leg(self, vt_symbol: str) -> LegData:
         """"""
         leg: LegData = self.legs.get(vt_symbol, None)
 
         if not leg:
@@ -345,17 +388,17 @@
         self.write_log("价差移除成功：{}，重启后生效".format(name))
 
     def get_spread(self, name: str) -> Optional[SpreadData]:
         """"""
         spread: SpreadData = self.spreads.get(name, None)
         return spread
 
-    def get_all_spreads(self) -> List[SpreadData]:
+    def get_all_spread_names(self) -> List[str]:
         """"""
-        return list(self.spreads.values())
+        return list(self.spreads.keys())
 
     def update_order_spread_map(self, vt_orderid: str, spread: SpreadData) -> None:
         """更新委托号对应的价差映射关系"""
         self.order_spread_map[vt_orderid] = spread
 
 
 class SpreadAlgoEngine:
@@ -393,21 +436,17 @@
 
     def register_event(self) -> None:
         """"""
         self.event_engine.register(EVENT_TICK, self.process_tick_event)
         self.event_engine.register(EVENT_ORDER, self.process_order_event)
         self.event_engine.register(EVENT_TRADE, self.process_trade_event)
         self.event_engine.register(EVENT_TIMER, self.process_timer_event)
-        self.event_engine.register(
-            EVENT_SPREAD_DATA, self.process_spread_event
-        )
 
-    def process_spread_event(self, event: Event) -> None:
+    def update_spread_data(self, spread: SpreadData) -> None:
         """"""
-        spread: SpreadData = event.data
         self.spreads[spread.name] = spread
 
     def process_tick_event(self, event: Event) -> None:
         """"""
         tick: TickData = event.data
         algos: List[SpreadAlgoTemplate] = self.symbol_algo_map[tick.vt_symbol]
         if not algos:
@@ -507,15 +546,17 @@
             self.write_log("停止价差算法失败，找不到算法：{}".format(algoid))
             return
 
         algo.stop()
 
     def put_algo_event(self, algo: SpreadAlgoTemplate) -> None:
         """"""
-        event: Event = Event(EVENT_SPREAD_ALGO, algo)
+        self.spread_engine.update_spread_algo(algo)
+
+        event: Event = Event(EVENT_SPREAD_ALGO, algo.get_item())
         self.event_engine.put(event)
 
     def write_algo_log(self, algo: SpreadAlgoTemplate, msg: str) -> None:
         """"""
         msg: str = f"{algo.algoid}：{msg}"
         self.write_log(msg)
 
@@ -601,14 +642,16 @@
         """"""
         return self.main_engine.get_contract(vt_symbol)
 
 
 class SpreadStrategyEngine:
     """"""
 
+    engine_type: EngineType = EngineType.LIVE
+
     setting_filename: str = "spread_trading_strategy.json"
 
     def __init__(self, spread_engine: SpreadEngine) -> None:
         """"""
         self.spread_engine: SpreadEngine = spread_engine
         self.main_engine: MainEngine = spread_engine.main_engine
         self.event_engine: EventEngine = spread_engine.event_engine
@@ -716,39 +759,33 @@
         save_json(self.setting_filename, self.strategy_setting)
 
     def register_event(self) -> None:
         """"""
         ee: EventEngine = self.event_engine
         ee.register(EVENT_ORDER, self.process_order_event)
         ee.register(EVENT_TRADE, self.process_trade_event)
-        ee.register(EVENT_SPREAD_DATA, self.process_spread_data_event)
-        ee.register(EVENT_SPREAD_POS, self.process_spread_pos_event)
-        ee.register(EVENT_SPREAD_ALGO, self.process_spread_algo_event)
 
-    def process_spread_data_event(self, event: Event) -> None:
+    def update_spread_data(self, spread: SpreadData) -> None:
         """"""
-        spread: SpreadData = event.data
         strategies: List[SpreadStrategyTemplate] = self.spread_strategy_map[spread.name]
 
         for strategy in strategies:
             if strategy.inited:
                 self.call_strategy_func(strategy, strategy.on_spread_data)
 
-    def process_spread_pos_event(self, event: Event) -> None:
+    def update_spread_pos(self, spread: SpreadData) -> None:
         """"""
-        spread: SpreadData = event.data
         strategies: List[SpreadStrategyTemplate] = self.spread_strategy_map[spread.name]
 
         for strategy in strategies:
             if strategy.inited:
                 self.call_strategy_func(strategy, strategy.on_spread_pos)
 
-    def process_spread_algo_event(self, event: Event) -> None:
+    def update_spread_algo(self, algo: SpreadAlgoTemplate) -> None:
         """"""
-        algo: SpreadAlgoTemplate = event.data
         strategy: SpreadStrategyTemplate = self.algo_strategy_map.get(algo.algoid, None)
 
         if strategy:
             self.call_strategy_func(
                 strategy, strategy.update_spread_algo, algo)
 
     def process_order_event(self, event: Event) -> None:
@@ -1044,14 +1081,18 @@
         if strategy:
             subject: str = f"{strategy.strategy_name}"
         else:
             subject: str = "价差策略引擎"
 
         self.main_engine.send_email(subject, msg)
 
+    def get_engine_type(self) -> EngineType:
+        """"""
+        return self.engine_type
+
     def load_bar(
         self, spread: SpreadData, days: int, interval: Interval, callback: Callable
     ) -> None:
         """"""
         end: datetime = datetime.now()
         start: datetime = end - timedelta(days)
```

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/basic_spread_strategy.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/strategies/basic_spread_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/template.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from vnpy.trader.object import (
     TickData, TradeData, OrderData, ContractData, BarData
 )
 from vnpy.trader.constant import Direction, Status, Offset, Interval
 from vnpy.trader.utility import virtual, floor_to, ceil_to, round_to
 
-from .base import SpreadData, LegData
+from .base import SpreadData, LegData, EngineType, AlgoItem
 
 if TYPE_CHECKING:
     from .engine import SpreadAlgoEngine, SpreadStrategyEngine
 
 
 class SpreadAlgoTemplate:
     """
@@ -64,14 +64,31 @@
         self.leg_orders: defaultdict = defaultdict(list)
 
         self.order_trade_volume: defaultdict = defaultdict(int)
         self.orders: Dict[str, OrderData] = {}
 
         self.write_log("算法已启动")
 
+    def get_item(self) -> AlgoItem:
+        """获取数据对象"""
+        item: AlgoItem = AlgoItem(
+            algoid=self.algoid,
+            spread_name=self.spread_name,
+            direction=self.direction,
+            price=self.price,
+            payup=self.payup,
+            volume=self.volume,
+            traded_volume=self.traded_volume,
+            traded_price=self.traded_price,
+            interval=self.interval,
+            count=self.count,
+            status=self.status
+        )
+        return item
+
     def is_active(self) -> bool:
         """判断算法是否处于运行中"""
         if self.status not in [Status.CANCELLED, Status.ALLTRADED]:
             return True
         else:
             return False
 
@@ -696,14 +713,18 @@
         """"""
         self.strategy_engine.put_strategy_event(self)
 
     def write_log(self, msg: str) -> None:
         """"""
         self.strategy_engine.write_strategy_log(self, msg)
 
+    def get_engine_type(self) -> EngineType:
+        """"""
+        self.strategy_engine.get_engine_type()
+
     def get_spread_tick(self) -> TickData:
         """"""
         return self.spread.to_tick()
 
     def get_spread_pos(self) -> float:
         """"""
         return self.spread.net_pos
```

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/spread.ico` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/ui/spread.ico`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/widget.py` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading/ui/widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     BaseMonitor, BaseCell,
     BidCell, AskCell,
     TimeCell, PnlCell,
     DirectionCell, EnumCell,
 )
 
 from ..engine import (
-    BaseEngine,
     SpreadEngine,
     SpreadStrategyEngine,
     SpreadData,
     APP_NAME,
     EVENT_SPREAD_DATA,
     EVENT_SPREAD_POS,
     EVENT_SPREAD_LOG,
@@ -36,15 +35,15 @@
     def __init__(self, main_engine: MainEngine, event_engine: EventEngine) -> None:
         """"""
         super().__init__()
 
         self.main_engine: MainEngine = main_engine
         self.event_engine: EventEngine = event_engine
 
-        self.spread_engine: BaseEngine = main_engine.get_engine(APP_NAME)
+        self.spread_engine: SpreadEngine = main_engine.get_engine(APP_NAME)
 
         self.init_ui()
 
     def init_ui(self) -> None:
         """"""
         self.setWindowTitle("价差交易")
 
@@ -57,19 +56,21 @@
             self.event_engine
         )
         self.log_monitor: SpreadLogMonitor = SpreadLogMonitor(
             self.main_engine,
             self.event_engine
         )
         self.algo_monitor: SpreadAlgoMonitor = SpreadAlgoMonitor(
-            self.spread_engine
+            self.main_engine,
+            self.event_engine
         )
 
         self.strategy_monitor: SpreadStrategyMonitor = SpreadStrategyMonitor(
-            self.spread_engine
+            self.main_engine,
+            self.event_engine
         )
 
         grid: QtWidgets.QGridLayout = QtWidgets.QGridLayout()
         grid.addWidget(self.create_group("价差", self.data_monitor), 0, 0)
         grid.addWidget(self.create_group("日志", self.log_monitor), 1, 0)
         grid.addWidget(self.create_group("算法", self.algo_monitor), 0, 1)
         grid.addWidget(self.create_group("策略", self.strategy_monitor), 1, 1)
@@ -180,19 +181,19 @@
         "traded_volume": {"display": "成交数量", "cell": BaseCell, "update": True},
         "traded_price": {"display": "成交均价", "cell": BaseCell, "update": True},
         "interval": {"display": "间隔", "cell": BaseCell, "update": False},
         "count": {"display": "计数", "cell": BaseCell, "update": True},
         "status": {"display": "状态", "cell": EnumCell, "update": True},
     }
 
-    def __init__(self, spread_engine: SpreadEngine) -> None:
+    def __init__(self, main_engine: MainEngine, event_engine: EventEngine) -> None:
         """"""
-        super().__init__(spread_engine.main_engine, spread_engine.event_engine)
+        super().__init__(main_engine, event_engine)
 
-        self.spread_engine: SpreadEngine = spread_engine
+        self.spread_engine: SpreadEngine = main_engine.get_engine(APP_NAME)
 
     def init_ui(self) -> None:
         """
         Connect signal.
         """
         super().init_ui()
 
@@ -258,21 +259,21 @@
 
         self.class_combo: QtWidgets.QComboBox = QtWidgets.QComboBox()
 
         add_button: QtWidgets.QPushButton = QtWidgets.QPushButton("添加策略")
         add_button.clicked.connect(self.add_strategy)
 
         init_button: QtWidgets.QPushButton = QtWidgets.QPushButton("全部初始化")
-        init_button.clicked.connect(self.strategy_engine.init_all_strategies)
+        init_button.clicked.connect(self.spread_engine.init_all_strategies)
 
         start_button: QtWidgets.QPushButton = QtWidgets.QPushButton("全部启动")
-        start_button.clicked.connect(self.strategy_engine.start_all_strategies)
+        start_button.clicked.connect(self.spread_engine.start_all_strategies)
 
         stop_button: QtWidgets.QPushButton = QtWidgets.QPushButton("全部停止")
-        stop_button.clicked.connect(self.strategy_engine.stop_all_strategies)
+        stop_button.clicked.connect(self.spread_engine.stop_all_strategies)
 
         add_spread_button: QtWidgets.QPushButton = QtWidgets.QPushButton("创建价差")
         add_spread_button.clicked.connect(self.add_spread)
 
         remove_spread_button: QtWidgets.QPushButton = QtWidgets.QPushButton("移除价差")
         remove_spread_button.clicked.connect(self.remove_spread)
 
@@ -304,21 +305,41 @@
         """"""
         lock_str: str = self.mode_combo.currentText()
         if lock_str == "锁仓":
             lock: bool = True
         else:
             lock: bool = False
 
+        price_text = self.price_line.text()
+        volume_text = self.volume_line.text()
+        payup_text = self.payup_line.text()
+        interval_text = self.interval_line.text()
+
+        for text, name in [
+            (price_text, "价格"),
+            (volume_text, "数量"),
+            (payup_text, "超价"),
+            (interval_text, "间隔"),
+        ]:
+            if not text:
+                QtWidgets.QMessageBox.warning(
+                    self,
+                    "启动失败",
+                    f"请输入【{name}】",
+                    QtWidgets.QMessageBox.Ok
+                )
+                return
+
         self.spread_engine.start_algo(
             spread_name=self.name_line.text(),
             direction=Direction(self.direction_combo.currentText()),
-            price=float(self.price_line.text()),
-            volume=float(self.volume_line.text()),
-            payup=int(self.payup_line.text()),
-            interval=int(self.interval_line.text()),
+            price=float(price_text),
+            volume=float(volume_text),
+            payup=int(payup_text),
+            interval=int(interval_text),
             lock=lock,
             extra={}
         )
 
     def add_spread(self) -> None:
         """"""
         dialog: SpreadDataDialog = SpreadDataDialog(self.spread_engine)
@@ -329,39 +350,39 @@
         dialog: SpreadRemoveDialog = SpreadRemoveDialog(self.spread_engine)
         dialog.exec_()
 
     def update_class_combo(self) -> None:
         """"""
         self.class_combo.clear()
         self.class_combo.addItems(
-            self.strategy_engine.get_all_strategy_class_names()
+            self.spread_engine.get_all_strategy_class_names()
         )
 
     def remove_strategy(self, strategy_name) -> None:
         """"""
         manager = self.managers.pop(strategy_name)
         manager.deleteLater()
 
     def add_strategy(self) -> None:
         """"""
         class_name: str = str(self.class_combo.currentText())
         if not class_name:
             return
 
-        parameters: dict = self.strategy_engine.get_strategy_class_parameters(
+        parameters: dict = self.spread_engine.get_strategy_class_parameters(
             class_name)
         editor: SettingEditor = SettingEditor(parameters, class_name=class_name)
         n: int = editor.exec_()
 
         if n == editor.Accepted:
             setting: dict = editor.get_setting()
             spread_name: str = setting.pop("spread_name")
             strategy_name: str = setting.pop("strategy_name")
 
-            self.strategy_engine.add_strategy(
+            self.spread_engine.add_strategy(
                 class_name, strategy_name, spread_name, setting
             )
 
 
 class SpreadRemoveDialog(QtWidgets.QDialog):
     """"""
 
@@ -375,17 +396,16 @@
 
     def init_ui(self) -> None:
         """"""
         self.setWindowTitle("移除价差")
         self.setMinimumWidth(300)
 
         self.name_combo: QtWidgets.QComboBox = QtWidgets.QComboBox()
-        spreads: List[SpreadData] = self.spread_engine.get_all_spreads()
-        for spread in spreads:
-            self.name_combo.addItem(spread.name)
+        names: List[SpreadData] = self.spread_engine.get_all_spread_names()
+        self.name_combo.addItems(names)
 
         button_remove: QtWidgets.QPushButton = QtWidgets.QPushButton("移除")
         button_remove.clicked.connect(self.remove_spread)
 
         hbox: QtWidgets.QHBoxLayout = QtWidgets.QHBoxLayout()
         hbox.addWidget(self.name_combo)
         hbox.addWidget(button_remove)
@@ -400,20 +420,21 @@
 
 
 class SpreadStrategyMonitor(QtWidgets.QWidget):
     """"""
 
     signal_strategy: QtCore.pyqtSignal = QtCore.pyqtSignal(Event)
 
-    def __init__(self, spread_engine: SpreadEngine) -> None:
+    def __init__(self, main_engine: MainEngine, event_engine: EventEngine) -> None:
         super().__init__()
 
-        self.strategy_engine: SpreadStrategyEngine = spread_engine.strategy_engine
-        self.main_engine: MainEngine = spread_engine.main_engine
-        self.event_engine: EventEngine = spread_engine.event_engine
+        self.main_engine: MainEngine = main_engine
+        self.event_engine: EventEngine = event_engine
+
+        self.spread_engine: SpreadEngine = main_engine.get_engine(APP_NAME)
 
         self.managers: Dict[str, SpreadStrategyWidget] = {}
 
         self.init_ui()
         self.register_event()
 
     def init_ui(self) -> None:
@@ -447,15 +468,15 @@
         data: dict = event.data
         strategy_name: str = data["strategy_name"]
 
         if strategy_name in self.managers:
             manager: SpreadStrategyWidget = self.managers[strategy_name]
             manager.update_data(data)
         else:
-            manager: SpreadStrategyWidget = SpreadStrategyWidget(self, self.strategy_engine, data)
+            manager: SpreadStrategyWidget = SpreadStrategyWidget(self, self.spread_engine, data)
             self.scroll_layout.insertWidget(0, manager)
             self.managers[strategy_name] = manager
 
     def remove_strategy(self, strategy_name) -> None:
         """"""
         manager: SpreadStrategyWidget = self.managers.pop(strategy_name)
         manager.deleteLater()
@@ -465,22 +486,22 @@
     """
     Manager for a strategy
     """
 
     def __init__(
         self,
         strategy_monitor: SpreadStrategyMonitor,
-        strategy_engine: SpreadStrategyEngine,
+        spread_engine: SpreadEngine,
         data: dict
     ) -> None:
         """"""
         super().__init__()
 
         self.strategy_monitor: SpreadStrategyMonitor = strategy_monitor
-        self.strategy_engine: SpreadStrategyEngine = strategy_engine
+        self.spread_engine: SpreadEngine = spread_engine
 
         self.strategy_name: str = data["strategy_name"]
         self._data: dict = data
 
         self.init_ui()
 
     def init_ui(self) -> None:
@@ -537,40 +558,40 @@
         self._data = data
 
         self.parameters_monitor.update_data(data["parameters"])
         self.variables_monitor.update_data(data["variables"])
 
     def init_strategy(self) -> None:
         """"""
-        self.strategy_engine.init_strategy(self.strategy_name)
+        self.spread_engine.init_strategy(self.strategy_name)
 
     def start_strategy(self) -> None:
         """"""
-        self.strategy_engine.start_strategy(self.strategy_name)
+        self.spread_engine.start_strategy(self.strategy_name)
 
     def stop_strategy(self) -> None:
         """"""
-        self.strategy_engine.stop_strategy(self.strategy_name)
+        self.spread_engine.stop_strategy(self.strategy_name)
 
     def edit_strategy(self) -> None:
         """"""
         strategy_name: str = self._data["strategy_name"]
 
-        parameters: dict = self.strategy_engine.get_strategy_parameters(
+        parameters: dict = self.spread_engine.get_strategy_parameters(
             strategy_name)
         editor: SettingEditor = SettingEditor(parameters, strategy_name=strategy_name)
         n: int = editor.exec_()
 
         if n == editor.Accepted:
             setting: dict = editor.get_setting()
-            self.strategy_engine.edit_strategy(strategy_name, setting)
+            self.spread_engine.edit_strategy(strategy_name, setting)
 
     def remove_strategy(self) -> None:
         """"""
-        result: bool = self.strategy_engine.remove_strategy(self.strategy_name)
+        result: bool = self.spread_engine.remove_strategy(self.strategy_name)
 
         # Only remove strategy gui manager if it has been removed from engine
         if result:
             self.strategy_monitor.remove_strategy(self.strategy_name)
 
 
 class StrategyDataMonitor(QtWidgets.QTableWidget):
```

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/PKG-INFO` & `vnpy_spreadtrading-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vnpy-spreadtrading
-Version: 1.1.8
+Name: vnpy_spreadtrading
+Version: 1.1.9
 Summary: Spread trading application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的价差交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/SOURCES.txt` & `vnpy_spreadtrading-1.1.9/vnpy_spreadtrading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

