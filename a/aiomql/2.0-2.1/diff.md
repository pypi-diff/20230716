# Comparing `tmp/aiomql-2.0.tar.gz` & `tmp/aiomql-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomql-2.0.tar", last modified: Mon Jun 19 00:29:56 2023, max compression
+gzip compressed data, was "aiomql-2.1.tar", last modified: Sun Jul 16 19:21:41 2023, max compression
```

## Comparing `aiomql-2.0.tar` & `aiomql-2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.243166 aiomql-2.0/
--rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-2.0/LICENSE
--rw-rw-rw-   0        0        0     2279 2023-06-19 00:29:56.217265 aiomql-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-06-19 00:06:32.000000 aiomql-2.0/README.md
--rw-rw-rw-   0        0        0      805 2023-06-19 00:12:54.000000 aiomql-2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 00:29:56.244175 aiomql-2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:55.972977 aiomql-2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.080952 aiomql-2.0/src/aiomql/
--rw-rw-rw-   0        0        0      596 2023-06-18 23:07:33.000000 aiomql-2.0/src/aiomql/__init__.py
--rw-rw-rw-   0        0        0     3453 2023-06-18 23:08:38.000000 aiomql-2.0/src/aiomql/account.py
--rw-rw-rw-   0        0        0     3942 2023-06-18 23:07:05.000000 aiomql-2.0/src/aiomql/bot_builder.py
--rw-rw-rw-   0        0        0     6495 2023-06-18 23:07:05.000000 aiomql-2.0/src/aiomql/candle.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.137174 aiomql-2.0/src/aiomql/core/
--rw-rw-rw-   0        0        0       63 2023-06-13 22:43:24.000000 aiomql-2.0/src/aiomql/core/__init__.py
--rw-rw-rw-   0        0        0     4805 2023-06-18 23:45:07.000000 aiomql-2.0/src/aiomql/core/base.py
--rw-rw-rw-   0        0        0     4283 2023-06-18 22:58:34.000000 aiomql-2.0/src/aiomql/core/config.py
--rw-rw-rw-   0        0        0    38105 2023-06-18 22:58:34.000000 aiomql-2.0/src/aiomql/core/constants.py
--rw-rw-rw-   0        0        0    11636 2023-06-18 21:01:29.000000 aiomql-2.0/src/aiomql/core/meta_trader.py
--rw-rw-rw-   0        0        0    16685 2023-06-18 23:45:07.000000 aiomql-2.0/src/aiomql/core/models.py
--rw-rw-rw-   0        0        0     2241 2023-06-17 14:58:44.000000 aiomql-2.0/src/aiomql/executor.py
--rw-rw-rw-   0        0        0     5069 2023-06-17 15:12:23.000000 aiomql-2.0/src/aiomql/history.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.140691 aiomql-2.0/src/aiomql/lib/
--rw-rw-rw-   0        0        0      198 2023-06-13 22:14:26.000000 aiomql-2.0/src/aiomql/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.150924 aiomql-2.0/src/aiomql/lib/strategies/
--rw-rw-rw-   0        0        0        0 2023-05-06 20:55:40.000000 aiomql-2.0/src/aiomql/lib/strategies/__init__.py
--rw-rw-rw-   0        0        0     6913 2023-06-19 00:04:09.000000 aiomql-2.0/src/aiomql/lib/strategies/finger_trap.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.166616 aiomql-2.0/src/aiomql/lib/symbols/
--rw-rw-rw-   0        0        0       86 2023-06-10 11:42:24.000000 aiomql-2.0/src/aiomql/lib/symbols/__init__.py
--rw-rw-rw-   0        0        0     1581 2023-06-18 22:00:12.000000 aiomql-2.0/src/aiomql/lib/symbols/forex_symbol.py
--rw-rw-rw-   0        0        0     1376 2023-06-18 23:46:29.000000 aiomql-2.0/src/aiomql/lib/symbols/synthetic_symbol.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.213254 aiomql-2.0/src/aiomql/lib/traders/
--rw-rw-rw-   0        0        0     3079 2023-06-18 23:53:33.000000 aiomql-2.0/src/aiomql/lib/traders/simple_deal_trader.py
--rw-rw-rw-   0        0        0      927 2023-06-18 22:11:18.000000 aiomql-2.0/src/aiomql/lib/traders/trade_result.py
--rw-rw-rw-   0        0        0     3713 2023-06-18 23:53:33.000000 aiomql-2.0/src/aiomql/order.py
--rw-rw-rw-   0        0        0     2537 2023-06-17 17:16:06.000000 aiomql-2.0/src/aiomql/positions.py
--rw-rw-rw-   0        0        0     2822 2023-06-17 17:16:06.000000 aiomql-2.0/src/aiomql/records.py
--rw-rw-rw-   0        0        0     1596 2023-06-17 17:28:36.000000 aiomql-2.0/src/aiomql/result.py
--rw-rw-rw-   0        0        0     3284 2023-06-18 23:15:46.000000 aiomql-2.0/src/aiomql/strategy.py
--rw-rw-rw-   0        0        0    11721 2023-06-18 21:32:40.000000 aiomql-2.0/src/aiomql/symbol.py
--rw-rw-rw-   0        0        0     2698 2023-06-18 21:41:02.000000 aiomql-2.0/src/aiomql/terminal.py
--rw-rw-rw-   0        0        0     3127 2023-06-18 23:07:05.000000 aiomql-2.0/src/aiomql/ticks.py
--rw-rw-rw-   0        0        0     1160 2023-06-18 23:46:29.000000 aiomql-2.0/src/aiomql/trader.py
--rw-rw-rw-   0        0        0      246 2023-06-18 21:41:01.000000 aiomql-2.0/src/aiomql/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.102916 aiomql-2.0/src/aiomql.egg-info/
--rw-rw-rw-   0        0        0     2279 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1033 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:41.098870 aiomql-2.1/
+-rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-2.1/LICENSE
+-rw-rw-rw-   0        0        0     2279 2023-07-16 19:21:41.097866 aiomql-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2023-06-19 00:06:32.000000 aiomql-2.1/README.md
+-rw-rw-rw-   0        0        0      805 2023-07-16 19:09:36.000000 aiomql-2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 19:21:41.098870 aiomql-2.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:40.612865 aiomql-2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:40.913866 aiomql-2.1/src/aiomql/
+-rw-rw-rw-   0        0        0      596 2023-06-18 23:07:33.000000 aiomql-2.1/src/aiomql/__init__.py
+-rw-rw-rw-   0        0        0     3453 2023-07-15 18:28:37.000000 aiomql-2.1/src/aiomql/account.py
+-rw-rw-rw-   0        0        0     3942 2023-06-18 23:07:05.000000 aiomql-2.1/src/aiomql/bot_builder.py
+-rw-rw-rw-   0        0        0     6487 2023-07-16 18:41:03.000000 aiomql-2.1/src/aiomql/candle.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:41.009869 aiomql-2.1/src/aiomql/core/
+-rw-rw-rw-   0        0        0       63 2023-06-13 22:43:24.000000 aiomql-2.1/src/aiomql/core/__init__.py
+-rw-rw-rw-   0        0        0     4839 2023-07-16 18:44:12.000000 aiomql-2.1/src/aiomql/core/base.py
+-rw-rw-rw-   0        0        0     4355 2023-07-15 17:27:35.000000 aiomql-2.1/src/aiomql/core/config.py
+-rw-rw-rw-   0        0        0    38105 2023-06-18 22:58:34.000000 aiomql-2.1/src/aiomql/core/constants.py
+-rw-rw-rw-   0        0        0    12134 2023-07-16 19:14:53.000000 aiomql-2.1/src/aiomql/core/meta_trader.py
+-rw-rw-rw-   0        0        0    16685 2023-06-18 23:45:07.000000 aiomql-2.1/src/aiomql/core/models.py
+-rw-rw-rw-   0        0        0     2241 2023-06-17 14:58:44.000000 aiomql-2.1/src/aiomql/executor.py
+-rw-rw-rw-   0        0        0     5069 2023-06-17 15:12:23.000000 aiomql-2.1/src/aiomql/history.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:41.045866 aiomql-2.1/src/aiomql/lib/
+-rw-rw-rw-   0        0        0      198 2023-06-13 22:14:26.000000 aiomql-2.1/src/aiomql/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:41.048863 aiomql-2.1/src/aiomql/lib/strategies/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:55:40.000000 aiomql-2.1/src/aiomql/lib/strategies/__init__.py
+-rw-rw-rw-   0        0        0     6913 2023-06-19 00:04:09.000000 aiomql-2.1/src/aiomql/lib/strategies/finger_trap.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:41.079868 aiomql-2.1/src/aiomql/lib/symbols/
+-rw-rw-rw-   0        0        0       86 2023-06-10 11:42:24.000000 aiomql-2.1/src/aiomql/lib/symbols/__init__.py
+-rw-rw-rw-   0        0        0     1581 2023-06-18 22:00:12.000000 aiomql-2.1/src/aiomql/lib/symbols/forex_symbol.py
+-rw-rw-rw-   0        0        0     1376 2023-06-18 23:46:29.000000 aiomql-2.1/src/aiomql/lib/symbols/synthetic_symbol.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:41.084865 aiomql-2.1/src/aiomql/lib/traders/
+-rw-rw-rw-   0        0        0     3079 2023-06-18 23:53:33.000000 aiomql-2.1/src/aiomql/lib/traders/simple_deal_trader.py
+-rw-rw-rw-   0        0        0      927 2023-06-18 22:11:18.000000 aiomql-2.1/src/aiomql/lib/traders/trade_result.py
+-rw-rw-rw-   0        0        0     3713 2023-06-18 23:53:33.000000 aiomql-2.1/src/aiomql/order.py
+-rw-rw-rw-   0        0        0     2537 2023-06-17 17:16:06.000000 aiomql-2.1/src/aiomql/positions.py
+-rw-rw-rw-   0        0        0     2822 2023-06-17 17:16:06.000000 aiomql-2.1/src/aiomql/records.py
+-rw-rw-rw-   0        0        0     1596 2023-06-17 17:28:36.000000 aiomql-2.1/src/aiomql/result.py
+-rw-rw-rw-   0        0        0     3284 2023-06-18 23:15:46.000000 aiomql-2.1/src/aiomql/strategy.py
+-rw-rw-rw-   0        0        0    11720 2023-07-15 18:28:37.000000 aiomql-2.1/src/aiomql/symbol.py
+-rw-rw-rw-   0        0        0     2698 2023-06-18 21:41:02.000000 aiomql-2.1/src/aiomql/terminal.py
+-rw-rw-rw-   0        0        0     3127 2023-06-18 23:07:05.000000 aiomql-2.1/src/aiomql/ticks.py
+-rw-rw-rw-   0        0        0     1160 2023-06-18 23:46:29.000000 aiomql-2.1/src/aiomql/trader.py
+-rw-rw-rw-   0        0        0      246 2023-06-18 21:41:01.000000 aiomql-2.1/src/aiomql/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:40.942924 aiomql-2.1/src/aiomql.egg-info/
+-rw-rw-rw-   0        0        0     2279 2023-07-16 19:21:40.000000 aiomql-2.1/src/aiomql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1033 2023-07-16 19:21:40.000000 aiomql-2.1/src/aiomql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 19:21:40.000000 aiomql-2.1/src/aiomql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-16 19:21:40.000000 aiomql-2.1/src/aiomql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 19:21:40.000000 aiomql-2.1/src/aiomql.egg-info/top_level.txt
```

### Comparing `aiomql-2.0/LICENSE` & `aiomql-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/PKG-INFO` & `aiomql-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 2.0
+Version: 2.1
 Summary: Asynchronous MetaTrader5 library and Bot Builder
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiomql-2.0/README.md` & `aiomql-2.1/README.md`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/pyproject.toml` & `aiomql-2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiomql"
-version = "2.0"
+version = "2.1"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `aiomql-2.0/src/aiomql/__init__.py` & `aiomql-2.1/src/aiomql/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/account.py` & `aiomql-2.1/src/aiomql/account.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/bot_builder.py` & `aiomql-2.1/src/aiomql/bot_builder.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/candle.py` & `aiomql-2.1/src/aiomql/candle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
-from typing import Type, TypeVar, Generic, Self
-
+from typing import Type, TypeVar, Generic
 from pandas import DataFrame, Series
 
 from .core.constants import TimeFrame
 
 _Candles = TypeVar('_Candles', bound='Candles')
 _Candle = TypeVar('_Candle', bound='Candle')
```

### Comparing `aiomql-2.0/src/aiomql/core/base.py` & `aiomql-2.1/src/aiomql/core/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Keyword Args:
         **kwargs: Object attributes and values as keyword arguments. Only added if they are annotated on the class body.
 
     Class Attributes:
         mt5 (MetaTrader): An instance of the MetaTrader class
         config (Config): An instance of the Config class
-        Config (Type[Config]): The Config class
+        Meta (Type[Meta]): The Meta class for configuration of the data model class
     """
     mt5: MetaTrader = MetaTrader()
     config = Config()
 
     def __init__(self, **kwargs):
         self.set_attributes(**kwargs)
 
@@ -37,15 +37,14 @@
         
         Keyword Args:
             **kwargs: Object attributes and values as keyword arguments
 
         Raises:
             AttributeError: When assigning an attribute that does not belong to the class or any parent class
 
-
         Notes:
             Only sets attributes that have been annotated on the class body.
         """
         for i, j in kwargs.items():
             try:
                 setattr(self, i, self.annotations[i](j))
             except KeyError:
```

### Comparing `aiomql-2.0/src/aiomql/core/config.py` & `aiomql-2.1/src/aiomql/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         if not hasattr(cls, '_instance'):
             cls._instance = super().__new__(cls)
         return cls._instance
     
     def __init__(self, **kwargs):
         self.file = kwargs.get('file', None)
         self.filename = kwargs.get('filename', None) or self.filename
+        kwargs.pop('file', None)
+        kwargs.pop('filename', None)
         self.load_config(reload=False)
         self.set_attributes(**kwargs)
 
     @staticmethod
     def walk_to_root(path: str) -> Iterator[str]:
         
         if not os.path.exists(path):
```

### Comparing `aiomql-2.0/src/aiomql/core/constants.py` & `aiomql-2.1/src/aiomql/core/constants.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/core/meta_trader.py` & `aiomql-2.1/src/aiomql/core/meta_trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,30 @@
         defaults = {f'_{key}': value for key, value in defaults.items() if not key.startswith('_')}
         cls_dict |= defaults
         return super().__new__(mcs, cls_name, bases, cls_dict)
 
 
 class MetaTrader(metaclass=BaseMeta):
 
+    async def __aenter__(self):
+        """
+        Async context manager entry point.
+        Initializes the connection to the MetaTrader terminal.
+        Returns: An instance of the MetaTrader class.
+        """
+        await self.initialize()
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        """
+        Async context manager exit point.
+        Closes the connection to the MetaTrader terminal.
+        """
+        await self.shutdown()
+
     async def login(self, login: int, password: str, server: str, timeout: int = 60000) -> bool:
         """"""
         return await asyncio.to_thread(self._login, login, password=password, server=server, timeout=timeout)
 
     async def initialize(self, path: str = "", login: int = 0, password: str = "", server: str = "",
                          timeout: int | None = None, portable=False) -> bool:
         """"""
```

### Comparing `aiomql-2.0/src/aiomql/core/models.py` & `aiomql-2.1/src/aiomql/core/models.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/executor.py` & `aiomql-2.1/src/aiomql/executor.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/history.py` & `aiomql-2.1/src/aiomql/history.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/lib/strategies/finger_trap.py` & `aiomql-2.1/src/aiomql/lib/strategies/finger_trap.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/lib/symbols/forex_symbol.py` & `aiomql-2.1/src/aiomql/lib/symbols/forex_symbol.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/lib/symbols/synthetic_symbol.py` & `aiomql-2.1/src/aiomql/lib/symbols/synthetic_symbol.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/lib/traders/simple_deal_trader.py` & `aiomql-2.1/src/aiomql/lib/traders/simple_deal_trader.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/lib/traders/trade_result.py` & `aiomql-2.1/src/aiomql/lib/traders/trade_result.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/order.py` & `aiomql-2.1/src/aiomql/order.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/positions.py` & `aiomql-2.1/src/aiomql/positions.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/records.py` & `aiomql-2.1/src/aiomql/records.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/result.py` & `aiomql-2.1/src/aiomql/result.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/strategy.py` & `aiomql-2.1/src/aiomql/strategy.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/symbol.py` & `aiomql-2.1/src/aiomql/symbol.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .ticks import Tick
 from .account import Account
 
 logger = getLogger()
 
 
 class Symbol(SymbolInfo):
-    """Main class for handling a financial instrument. A subclass of SymbolInfo and Base it have properties and methods
+    """Main class for handling a financial instrument. A subclass of SymbolInfo and Base it has attributes and methods
     for working with a financial instrument.
 
     Attributes:
         tick (Tick): Price tick object for instrument
         account: An instance of the current trading account
 
     Notes:
```

### Comparing `aiomql-2.0/src/aiomql/terminal.py` & `aiomql-2.1/src/aiomql/terminal.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/ticks.py` & `aiomql-2.1/src/aiomql/ticks.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql/trader.py` & `aiomql-2.1/src/aiomql/trader.py`

 * *Files identical despite different names*

### Comparing `aiomql-2.0/src/aiomql.egg-info/PKG-INFO` & `aiomql-2.1/src/aiomql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 2.0
+Version: 2.1
 Summary: Asynchronous MetaTrader5 library and Bot Builder
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiomql-2.0/src/aiomql.egg-info/SOURCES.txt` & `aiomql-2.1/src/aiomql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

