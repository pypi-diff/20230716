# Comparing `tmp/fa-models-1.0.77.tar.gz` & `tmp/fa-models-1.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.77.tar", last modified: Wed Jul 12 07:34:30 2023, max compression
+gzip compressed data, was "fa-models-1.0.78.tar", last modified: Sun Jul 16 20:02:23 2023, max compression
```

## Comparing `fa-models-1.0.77.tar` & `fa-models-1.0.78.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-12 07:34:30.687567 fa-models-1.0.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-12 07:33:53.000000 fa-models-1.0.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.683566 fa-models-1.0.77/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.683566 fa-models-1.0.77/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/famodels/models/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-12 07:34:20.000000 fa-models-1.0.77/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 07:34:30.687567 fa-models-1.0.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-12 07:33:53.000000 fa-models-1.0.77/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-12 07:33:53.000000 fa-models-1.0.77/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-12 07:33:53.000000 fa-models-1.0.77/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:02:23.398748 fa-models-1.0.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-16 20:01:52.000000 fa-models-1.0.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.394748 fa-models-1.0.78/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 20:02:23.000000 fa-models-1.0.78/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.394748 fa-models-1.0.78/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-16 20:01:52.000000 fa-models-1.0.78/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-16 20:02:15.000000 fa-models-1.0.78/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:02:23.398748 fa-models-1.0.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-16 20:01:52.000000 fa-models-1.0.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:02:23.398748 fa-models-1.0.78/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-16 20:01:52.000000 fa-models-1.0.78/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-16 20:01:52.000000 fa-models-1.0.78/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.77/PKG-INFO` & `fa-models-1.0.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.77
+Version: 1.0.78
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.77/README.md` & `fa-models-1.0.78/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.78/fa_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.77
+Version: 1.0.78
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.77/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.78/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/algorithm.py` & `fa-models-1.0.78/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/investor.py` & `fa-models-1.0.78/famodels/models/investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/investor_statement.py` & `fa-models-1.0.78/famodels/models/investor_statement.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/market/public_trade.py` & `fa-models-1.0.78/famodels/models/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/person.py` & `fa-models-1.0.78/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/processed_signal.py` & `fa-models-1.0.78/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/signal_provider.py` & `fa-models-1.0.78/famodels/models/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/famodels/models/trade.py` & `fa-models-1.0.78/famodels/models/trade.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,27 +40,30 @@
 
 class Order(EmbeddedJsonModel):
     """This model is for hot orders ONLY! Use ColdOrder for paper trading.
     """
     id: str = Field(index=True)
     signal_id: str = Field(index=True)
     algo_id: str = Field(index=True)
-    trade_id: str = Field(index=True)
+    # trade_id: str = Field(index=True)
     state: StateOfOrder = Field(index=True, default=StateOfOrder.NEW)
+    """A order that is marked as new, needs a mirrored order created on the exchange."""
     order_type: OrderType = Field(index=True, default=OrderType.LIMIT)        
     market: str = Field(index=True)
     exchange: str = Field(index=True)
     direction: Direction = Field(index=True)
     side: Side = Field(index=True)
     price: float
-    amount: float    
-    account: str = Field(index=True)
-    pos_idx: int = Field(index=True)
+    amount: float = Field(index=True)
+    tp: float
+    sl: float
+    # account: str = Field(index=True)
+    # pos_idx: int = Field(index=True)
     timestamp_of_order: int = Field(index=True)
-    comission: float    
+    # comission: float    
 
     class Meta:
         # global_key_prefix="order-and-trade-processing"
         model_key_prefix="order"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
     def __getitem__(self, key):
@@ -90,14 +93,19 @@
     id: str = Field(primary_key=True)
     # sort_index:int = field(init=False, repr=False)
     #trade_id: Optional[str] = Field(default=uuid.uuid4(), primary_key=True)
     """The trade id is the reference that keeps the state updates correlated. It will generate a UUID by default.
         Use this for the first record you insert. Inserting updated records (new records should then have the trade_id
         provided to create the correlation.)"""
     investor_id: str = Field(index=True)
+    provider_id: str = Field(index=True)
+    provider_trade_id: Optional[str] = Field(index=False)
+    """ This id can be sent optionally (together with position_size_in_percent) by the signal provider to make this a multi-position-trade.
+        CAUTION: This trade id has to be unique for each multi-position-trade one is attempting to run.
+    """
     fund_id: str = Field(index=True)
     fund_pos_idx:int
     """ This is one position of the fund. Which can consist of extra partial/scaled orders, if a provider_trade_id is supplied.
         The partial/scaled orders are tracked as orders.
     """
     market:str = Field(index=True)    
     state:StateOfTrade = Field(index=True, default=StateOfTrade.NEW)
```

### Comparing `fa-models-1.0.77/famodels/models/trading_signal.py` & `fa-models-1.0.78/famodels/models/trading_signal.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     algo_id: str = Field(index=True)
     """Provide the id of your algorithm id (you might have more than one algorithm), which is sending a signal. """
     provider_signal_id: Optional[str]
     """You can use this correlation id as your own 'signal id' of your internal system. 
     #Do not mistaken this correlation id with the trade correlation id."""    
     provider_trade_id: str = Field(index=True)
     """ FA Models describes a Trade as a buy and a sell (not soley a buy or a sell). 
-        Every trade is expected to consist of at least one buy order and zero or more sell orders. 
-        Thus, the provider_trade_id is mandatory if a provider wants to scale in and out on positions. 
+        Every trade is expected to consist of at least one buy order and at least one sell order. 
+        Thus, the provider_trade_id is mandatory if a provider wants to scale in and out on a fund-position. This will create a multi-position-trade.
         E.g. one can send one long signal with a provider_trade_id 77 and another long signal a few hours later also with the provider_trade_id 77. 
         Provided that the position_size_in_percentage is less than 100 on the first one.
         All updates provided by the system will hold the trade id."""    
     is_hot_signal: int = Field(default=0, index=True)
     """By default, every signal is marked as a cold signal. Thus, set to 0. That is a paper-trading signal and will only be processed for forward-performance testing. 
     Hot signals are suggested to be processed by the order engines - provided all other requirements for hot trading are fulfilled.
     Set 1 (not true) to this value to suggest a hot trade."""    
@@ -51,17 +51,20 @@
     price: float
     """The price to buy use for the limit-order or limit-stop-order"""
     tp: float
     """Take-profit in absolute price."""
     sl: float
     """Stop-loss in absolute price."""
     position_size_in_percentage: float = 100
-    """Percentage of the trade position this algortihm is allowed to trade. 
+    """ Caution, if one chooses another value than 100, the system will create a multi-position-trade (for scaling-in and scaling-out on a trade).
+    In addition, one has to provide a provider_trade_id in order for the system to create a multi-position-trade. 
+    Any consecutive trades (scale-in/out), need to have provide the same provider_trade_id.
+    Percentage of the trade position this algortihm is allowed to trade. 
     Default is 100%, which is 1 position of your fund's positions.
-    Another number than 100, will assume this provider-trade has multiple positions. 
+    Another number than 100, will assume this trade has multiple positions. 
     If a signal provider has one partial position open and then closes it, it will also regard the trade as fully closed."""  
     # datatime.datetime would be fully serializable in REDIS. 
     # https://www.youtube.com/watch?v=ZP2j7bmWfmU
     timestamp_of_creation: int = Field(index=True)
     """The timestamp in milliseconds when the signal was created by the signal supplier."""
     timestamp_of_registration: Optional[int]
     """The timestamp in milliseconds when the signal was entering our interface. This will be overridden."""
```

### Comparing `fa-models-1.0.77/famodels/models/virtual_order.py` & `fa-models-1.0.78/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/pyproject.toml` & `fa-models-1.0.78/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.77"
+version = "1.0.78"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.77"
+current_version = "1.0.78"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.77/setup.py` & `fa-models-1.0.78/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/tests/test_investor.py` & `fa-models-1.0.78/tests/test_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.77/tests/test_processed_trading_signal.py` & `fa-models-1.0.78/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

