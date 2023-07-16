# Comparing `tmp/areixlib-0.1.8.tar.gz` & `tmp/areixlib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "areixlib-0.1.8.tar", last modified: Mon Jun 27 08:01:42 2022, max compression
+gzip compressed data, was "areixlib-0.1.9.tar", last modified: Sun Jul  3 15:26:35 2022, max compression
```

## Comparing `areixlib-0.1.8.tar` & `areixlib-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 charon     (501) staff       (20)        0 2022-06-27 08:01:42.296748 areixlib-0.1.8/
--rw-r--r--   0 charon     (501) staff       (20)     1728 2022-06-27 08:01:42.296601 areixlib-0.1.8/PKG-INFO
--rw-r--r--   0 charon     (501) staff       (20)      319 2022-06-27 08:01:41.000000 areixlib-0.1.8/README.md
-drwxr-xr-x   0 charon     (501) staff       (20)        0 2022-06-27 08:01:42.294631 areixlib-0.1.8/areixlib/
--rw-r--r--   0 charon     (501) staff       (20)  1249378 2022-06-27 08:01:41.000000 areixlib-0.1.8/areixlib/__init__.py
-drwxr-xr-x   0 charon     (501) staff       (20)        0 2022-06-27 08:01:42.296403 areixlib-0.1.8/areixlib.egg-info/
--rw-r--r--   0 charon     (501) staff       (20)     1728 2022-06-27 08:01:41.000000 areixlib-0.1.8/areixlib.egg-info/PKG-INFO
--rw-r--r--   0 charon     (501) staff       (20)      229 2022-06-27 08:01:42.000000 areixlib-0.1.8/areixlib.egg-info/SOURCES.txt
--rw-r--r--   0 charon     (501) staff       (20)        1 2022-06-27 08:01:41.000000 areixlib-0.1.8/areixlib.egg-info/dependency_links.txt
--rw-r--r--   0 charon     (501) staff       (20)        1 2022-06-27 08:01:41.000000 areixlib-0.1.8/areixlib.egg-info/not-zip-safe
--rw-r--r--   0 charon     (501) staff       (20)       46 2022-06-27 08:01:42.000000 areixlib-0.1.8/areixlib.egg-info/requires.txt
--rw-r--r--   0 charon     (501) staff       (20)        9 2022-06-27 08:01:42.000000 areixlib-0.1.8/areixlib.egg-info/top_level.txt
--rw-r--r--   0 charon     (501) staff       (20)       38 2022-06-27 08:01:42.296799 areixlib-0.1.8/setup.cfg
--rw-r--r--   0 charon     (501) staff       (20)     2853 2022-06-27 08:01:41.000000 areixlib-0.1.8/setup.py
+drwxr-xr-x   0 charon     (501) staff       (20)        0 2022-07-03 15:26:35.492780 areixlib-0.1.9/
+-rw-r--r--   0 charon     (501) staff       (20)     1691 2022-07-03 15:26:35.492625 areixlib-0.1.9/PKG-INFO
+-rw-r--r--   0 charon     (501) staff       (20)      319 2022-07-03 15:26:34.000000 areixlib-0.1.9/README.md
+drwxr-xr-x   0 charon     (501) staff       (20)        0 2022-07-03 15:26:35.487072 areixlib-0.1.9/areixlib/
+-rw-r--r--   0 charon     (501) staff       (20)  1242058 2022-07-03 15:26:34.000000 areixlib-0.1.9/areixlib/__init__.py
+drwxr-xr-x   0 charon     (501) staff       (20)        0 2022-07-03 15:26:35.492434 areixlib-0.1.9/areixlib.egg-info/
+-rw-r--r--   0 charon     (501) staff       (20)     1691 2022-07-03 15:26:35.000000 areixlib-0.1.9/areixlib.egg-info/PKG-INFO
+-rw-r--r--   0 charon     (501) staff       (20)      229 2022-07-03 15:26:35.000000 areixlib-0.1.9/areixlib.egg-info/SOURCES.txt
+-rw-r--r--   0 charon     (501) staff       (20)        1 2022-07-03 15:26:35.000000 areixlib-0.1.9/areixlib.egg-info/dependency_links.txt
+-rw-r--r--   0 charon     (501) staff       (20)        1 2022-07-03 15:26:35.000000 areixlib-0.1.9/areixlib.egg-info/not-zip-safe
+-rw-r--r--   0 charon     (501) staff       (20)       46 2022-07-03 15:26:35.000000 areixlib-0.1.9/areixlib.egg-info/requires.txt
+-rw-r--r--   0 charon     (501) staff       (20)        9 2022-07-03 15:26:35.000000 areixlib-0.1.9/areixlib.egg-info/top_level.txt
+-rw-r--r--   0 charon     (501) staff       (20)       38 2022-07-03 15:26:35.492833 areixlib-0.1.9/setup.cfg
+-rw-r--r--   0 charon     (501) staff       (20)     2853 2022-07-03 15:26:34.000000 areixlib-0.1.9/setup.py
```

### Comparing `areixlib-0.1.8/PKG-INFO` & `areixlib-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: areixlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Areix Utils Library
 Home-page: https://alphagen.areix-ai.com
 Author: Areix
 Author-email: hellohk@areix-ai.com
-License: UNKNOWN
 Project-URL: Documentation, https://alphagen.areix-ai.com/doc
 Keywords: areix,areixio,alpha_gen,alphagen,wealthx,algo,algorithmic,backtest,backtesting,bitcoin,crypto,bokeh,bonds,candle,candlestick,cboe,chart,cme,commodities,crash,currency,drawdown,equity,etf,ethereum,exchange,finance,financial,forecast,forex,fund,futures,fx,gold,historical,indicator,invest,investing,investment,macd,market,money,ohlc,ohlcv,order,price,profit,quant,quantitative,rsi,pnl,stocks,strategy,ticker,trader,trading,tradingview,usd,binance
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 3.7
@@ -43,9 +41,7 @@
 ```
 deactivate
 ```
 Install areixlib package
 ```
 pip install areixlib
 ```
-
-
```

### Comparing `areixlib-0.1.8/areixlib/__init__.py` & `areixlib-0.1.9/areixlib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-exec(CMPJSyJeScCQHLpPBpxcxAzZWYkNDRGS)
+exec(llHSldAZTfaxmQKzcLhnGVLJKDnYJPPD)
```

### Comparing `areixlib-0.1.8/areixlib.egg-info/PKG-INFO` & `areixlib-0.1.9/areixlib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: areixlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Areix Utils Library
 Home-page: https://alphagen.areix-ai.com
 Author: Areix
 Author-email: hellohk@areix-ai.com
-License: UNKNOWN
 Project-URL: Documentation, https://alphagen.areix-ai.com/doc
 Keywords: areix,areixio,alpha_gen,alphagen,wealthx,algo,algorithmic,backtest,backtesting,bitcoin,crypto,bokeh,bonds,candle,candlestick,cboe,chart,cme,commodities,crash,currency,drawdown,equity,etf,ethereum,exchange,finance,financial,forecast,forex,fund,futures,fx,gold,historical,indicator,invest,investing,investment,macd,market,money,ohlc,ohlcv,order,price,profit,quant,quantitative,rsi,pnl,stocks,strategy,ticker,trader,trading,tradingview,usd,binance
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 3.7
@@ -43,9 +41,7 @@
 ```
 deactivate
 ```
 Install areixlib package
 ```
 pip install areixlib
 ```
-
-
```

### Comparing `areixlib-0.1.8/setup.py` & `areixlib-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name='areixlib',
-    version='0.1.8',
+    version='0.1.9',
     description='Areix Utils Library',
     long_description_content_type='text/markdown',
     long_description=open(os.path.join(os.path.dirname(__file__), 'README.md'),encoding='utf-8').read(),
     author='Areix',
     author_email='hellohk@areix-ai.com',
     packages=find_packages(),
     # packages=['areixio'],
```
