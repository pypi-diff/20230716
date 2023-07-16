# Comparing `tmp/DiscordAlertsTrader-0.9.1.tar.gz` & `tmp/DiscordAlertsTrader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiscordAlertsTrader-0.9.1.tar", last modified: Mon May 29 02:33:47 2023, max compression
+gzip compressed data, was "DiscordAlertsTrader-1.0.0.tar", last modified: Sun Jul 16 16:55:49 2023, max compression
```

## Comparing `DiscordAlertsTrader-0.9.1.tar` & `DiscordAlertsTrader-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.641187 DiscordAlertsTrader-0.9.1/
-drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.616120 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/
--rw-rw-rw-   0        0        0       47 2023-05-29 02:14:18.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/__init__.py
--rw-rw-rw-   0        0        0    13816 2023-05-27 01:57:29.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_tracker.py
--rw-rw-rw-   0        0        0    51976 2023-05-27 01:57:29.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_trader.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.630236 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/
--rw-rw-rw-   0        0        0    11921 2023-05-24 00:30:53.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/TDA_api.py
--rw-rw-rw-   0        0        0     2337 2023-05-24 01:10:46.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/__init__.py
--rw-rw-rw-   0        0        0    22459 2023-05-27 01:57:29.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/eTrade_api.py
--rw-rw-rw-   0        0        0     2776 2023-05-20 18:48:10.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/configurator.py
--rw-rw-rw-   0        0        0    10361 2023-05-24 02:30:34.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/discord_bot.py
--rw-rw-rw-   0        0        0     1730 2023-05-22 13:47:39.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/fend_bot.py
--rw-rw-rw-   0        0        0    12823 2023-05-27 21:36:28.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui.py
--rw-rw-rw-   0        0        0    20630 2023-05-25 10:54:19.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui_generator.py
--rw-rw-rw-   0        0        0    12478 2023-05-27 13:36:36.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui_layouts.py
--rw-rw-rw-   0        0        0    22302 2023-05-23 19:53:15.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/message_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.626224 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/
--rw-rw-rw-   0        0        0     7780 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      953 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       86 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1545 2023-05-16 00:10:52.000000 DiscordAlertsTrader-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     7780 2023-05-29 02:33:47.641187 DiscordAlertsTrader-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     6918 2023-05-24 03:41:23.000000 DiscordAlertsTrader-0.9.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 02:33:47.642187 DiscordAlertsTrader-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-05-29 02:33:10.000000 DiscordAlertsTrader-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.640190 DiscordAlertsTrader-0.9.1/tests/
--rw-rw-rw-   0        0        0      119 2023-04-03 23:24:29.000000 DiscordAlertsTrader-0.9.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2352 2023-05-23 17:16:45.000000 DiscordAlertsTrader-0.9.1/tests/msg_samples.py
--rw-rw-rw-   0        0        0    11167 2023-05-15 17:17:09.000000 DiscordAlertsTrader-0.9.1/tests/td_dummy.py
--rw-rw-rw-   0        0        0      622 2023-05-16 13:25:58.000000 DiscordAlertsTrader-0.9.1/tests/test_AlertsTracker.py
--rw-rw-rw-   0        0        0      872 2023-04-03 23:24:29.000000 DiscordAlertsTrader-0.9.1/tests/test_TDsession.py
--rw-rw-rw-   0        0        0      927 2023-05-16 00:15:43.000000 DiscordAlertsTrader-0.9.1/tests/test_configurator.py
--rw-rw-rw-   0        0        0     3068 2023-05-20 18:46:17.000000 DiscordAlertsTrader-0.9.1/tests/test_discord_bot.py
--rw-rw-rw-   0        0        0     2248 2023-05-20 17:13:46.000000 DiscordAlertsTrader-0.9.1/tests/test_gui_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.888747 DiscordAlertsTrader-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.783184 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/
+-rw-rw-rw-   0        0        0       47 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/__init__.py
+-rw-rw-rw-   0        0        0     2426 2023-07-15 20:38:48.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_generator.py
+-rw-rw-rw-   0        0        0    14034 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_tracker.py
+-rw-rw-rw-   0        0        0    74192 2023-07-16 16:41:57.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_trader.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.833262 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/
+-rw-rw-rw-   0        0        0    12837 2023-07-13 14:38:05.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/TDA_api.py
+-rw-rw-rw-   0        0        0     2800 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/__init__.py
+-rw-rw-rw-   0        0        0    23709 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/eTrade_api.py
+-rw-rw-rw-   0        0        0    17459 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/weBull_api.py
+-rw-rw-rw-   0        0        0     3813 2023-06-20 16:07:36.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/calc_stats.py
+-rw-rw-rw-   0        0        0    12181 2023-07-13 14:23:53.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/calc_strat.py
+-rw-rw-rw-   0        0        0     4807 2023-07-16 16:19:10.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/configurator.py
+-rw-rw-rw-   0        0        0    15905 2023-07-16 15:56:29.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/discord_bot.py
+-rw-rw-rw-   0        0        0     2345 2023-06-08 13:42:28.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/fend_bot.py
+-rw-rw-rw-   0        0        0    15655 2023-07-16 15:15:51.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui.py
+-rw-rw-rw-   0        0        0    23375 2023-07-15 18:44:04.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui_generator.py
+-rw-rw-rw-   0        0        0    15051 2023-07-16 15:11:55.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui_layouts.py
+-rw-rw-rw-   0        0        0     1834 2023-05-28 17:46:50.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/load_chn_hist.py
+-rw-rw-rw-   0        0        0    18352 2023-07-15 16:03:06.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/message_parser.py
+-rw-rw-rw-   0        0        0    15335 2023-07-15 18:48:55.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/port_sim.py
+-rw-rw-rw-   0        0        0    20395 2023-07-04 15:50:18.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/tem_etrades.py
+-rw-rw-rw-   0        0        0      327 2023-07-13 15:28:14.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/test_trader.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.810191 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/
+-rw-rw-rw-   0        0        0     9294 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1545 2023-05-17 00:51:47.000000 DiscordAlertsTrader-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     9294 2023-07-16 16:55:49.887747 DiscordAlertsTrader-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8432 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 16:55:49.888747 DiscordAlertsTrader-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.886747 DiscordAlertsTrader-1.0.0/tests/
+-rw-rw-rw-   0        0        0      119 2023-03-28 13:47:06.000000 DiscordAlertsTrader-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2694 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/mock_discord_message.py
+-rw-rw-rw-   0        0        0      974 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_AlertsTracker.py
+-rw-rw-rw-   0        0        0    12801 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_AlertsTrader.py
+-rw-rw-rw-   0        0        0     7396 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_AlertsTrader_exits.py
+-rw-rw-rw-   0        0        0     5157 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_TDA.py
+-rw-rw-rw-   0        0        0     1062 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_configurator.py
+-rw-rw-rw-   0        0        0     4680 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_discord_bot.py
+-rw-rw-rw-   0        0        0     4964 2023-07-15 17:47:09.000000 DiscordAlertsTrader-1.0.0/tests/test_msg_parsed.py
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_tracker.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_tracker.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,24 +12,26 @@
     return date
 
 
 class AlertsTracker():
 
     def __init__(self, brokerage=None,
                  portfolio_fname=cfg['portfolio_names']["tracker_portfolio_name"],
-                 dir_quotes = cfg['general']['data_dir'] + '/live_quotes' ):
+                 dir_quotes = cfg['general']['data_dir'] + '/live_quotes',
+                 cfg=cfg):
 
         self.portfolio_fname = portfolio_fname  
         self.dir_quotes = dir_quotes
-        self.bksession = brokerage    
+        self.bksession = brokerage
+        self.cfg = cfg
 
         if op.exists(self.portfolio_fname):
             self.portfolio = pd.read_csv(self.portfolio_fname)
         else:
-            self.portfolio = pd.DataFrame(columns=cfg["col_names"]['tracker_portfolio'].split(",") )
+            self.portfolio = pd.DataFrame(columns=self.cfg["col_names"]['tracker_portfolio'].split(",") )
             self.portfolio.to_csv(self.portfolio_fname, index=False)
 
     def price_now(self, symbol:str, price_type="BTO"):
         if self.bksession is None:
             return None
 
         if price_type in ["BTO", "BTC"]:
@@ -38,174 +40,177 @@
             ptype = 'bidPrice'
 
         quote = self.bksession.get_quotes([symbol])
         if quote is None:
             # Try it again in case of TDA
             quote = self.bksession.get_quotes([symbol])
             
-        if quote is not None and len(quote) and quote.get(symbol).get('description' ) != 'Symbol not found':
+        if quote is not None and len(quote) and quote.get(symbol) is not None and quote.get(symbol).get('description' ) != 'Symbol not found':
             quote = quote.get(symbol).get(ptype)
             if quote != 0:
                 return quote
             else:
                 print("quote 0 for", symbol, price_type)
 
     def trade_alert(self, order, live_alert=True, channel=None):
         open_trade, _ = find_last_trade(order, self.portfolio, open_only=True)
-        if order.get('uQty') is None:
-            order['uQty'] = 1
+        if order.get('Qty') is None:
+            order['Qty'] = 1
         
-        if order["action"] in ["BTO", "STC"] and live_alert:
+        if order["action"] in ["BTO", "STC",'STO', 'BTC'] and live_alert:
             if order.get('Actual Cost', 'None') == 'None':
                 order["Actual Cost"] = self.price_now(order["Symbol"], order["action"])
 
-        if open_trade is None and order["action"] == "BTO":
+        if open_trade is None and order["action"] in ["BTO", 'STO']:
             str_act = self.make_BTO(order, channel)
-        elif order["action"] == "BTO":
+        elif order["action"] in ["BTO", 'STO']:
             # str_act = "BTO averaging disabled as it is mostly wrong alert messages"
             str_act = self.make_BTO_Avg(order, open_trade)
-        elif order["action"] == "STC" and open_trade is None:
-            str_act = "STC without BTO"
-        elif order["action"] == "STC":
+        elif order["action"] in ["STC", "BTC"] and open_trade is None:
+            str_act = order["action"] + "without BTO"
+        elif order["action"] in ["STC", "BTC"]:
             str_act = self.make_STC(order, open_trade)
         elif order["action"] == "ExitUpdate":
             if open_trade is not None:
                 self.portfolio.loc[open_trade, "SL"] = order.get('SL')
             return 
 
         #save to csv
         self.portfolio.to_csv(self.portfolio_fname, index=False)      
         return str_act
 
     def make_BTO(self, order, chan=None):
         if order["price"] is None:
             return
         date = order.get("Date", get_date())
-        if order['uQty'] is None:
-            order['uQty'] = 1
+        if order['Qty'] is None:
+            order['Qty'] = 1
         new_trade = {
             "Date": date,
             "Symbol": order['Symbol'],
             'isOpen': 1,
             "Asset": order["asset"],
-            "Type": "BTO",
+            "Type": order["action"],
             "Price": order["price"],
-            "Amount": order['uQty'],
-            "Price-current": order.get("Actual Cost"),
+            "Qty": order['Qty'],
+            "Price-actual": order.get("Actual Cost"),
             "Trader": order['Trader'],
             "SL": order.get("SL"),
             "Channel" : chan
             }        
         self.portfolio =pd.concat([self.portfolio, pd.DataFrame.from_records(new_trade, index=[0])], ignore_index=True)
 
-        str_act = f"BTO {order['Symbol']} {order['price']}"
+        str_act = f"{order['action']} {order['Symbol']} {order['price']}"
         if order['SL'] is not None:
             str_act += f", SL:{order['SL']}"
         return str_act
 
     def make_BTO_Avg(self, order, open_trade):
-        current_Avg = self.portfolio.loc[open_trade, "Avged"]
-        if np.isnan(current_Avg):
-            current_Avg = 1
+        actual_Avg = self.portfolio.loc[open_trade, "Avged"]
+        if np.isnan(actual_Avg):
+            actual_Avg = 1
         else:
-            current_Avg = int(current_Avg + 1)
+            actual_Avg = int(actual_Avg + 1)
         
         old_price = self.portfolio.loc[open_trade, "Price"]
         old_price = eval(old_price) if isinstance(old_price, str) else old_price
-        old_qty = self.portfolio.loc[open_trade, "Amount"]
-        alert_price_old = self.portfolio.loc[open_trade, "Price-current"]
+        old_qty = self.portfolio.loc[open_trade, "Qty"]
+        alert_price_old = self.portfolio.loc[open_trade, "Price-actual"]
         alert_price_old = eval(alert_price_old) if isinstance(alert_price_old, str) else alert_price_old
         alert_price_old = None if pd.isnull(alert_price_old) else alert_price_old
         alert_price = order.get("Actual Cost", "None")
         avgs_prices_al = f"{alert_price_old}/{alert_price}".replace("None/", "").replace("/None", "").replace("None", "")
         if not len(avgs_prices_al):
             avgs_prices_al = None
     
-        self.portfolio.loc[open_trade, "Avged"] = current_Avg
-        self.portfolio.loc[open_trade, "Amount"] += order['uQty']
-        self.portfolio.loc[open_trade, "Price"] = round(((old_price*old_qty) + (order['price']*order['uQty']))/(old_qty+order['uQty']),2)
+        self.portfolio.loc[open_trade, "Avged"] = actual_Avg
+        self.portfolio.loc[open_trade, "Qty"] += order['Qty']
+        self.portfolio.loc[open_trade, "Price"] = round(((old_price*old_qty) + (order['price']*order['Qty']))/(old_qty+order['Qty']),2)
         self.portfolio.loc[open_trade, "Prices"] = f"{old_price}/{order['price']}"
         if alert_price == 'None' or alert_price is None or alert_price_old is None:
-            self.portfolio.loc[open_trade, "Price-current"] = alert_price_old
+            self.portfolio.loc[open_trade, "Price-actual"] = alert_price_old
         else:
-            self.portfolio.loc[open_trade, "Price-current"] = round(((alert_price_old*old_qty) + (alert_price*order['uQty']))/(old_qty+order['uQty']),2)
-        self.portfolio.loc[open_trade, "Prices-current"] = avgs_prices_al
+            self.portfolio.loc[open_trade, "Price-actual"] = round(((alert_price_old*old_qty) + (alert_price*order['Qty']))/(old_qty+order['Qty']),2)
+        self.portfolio.loc[open_trade, "Prices-actual"] = avgs_prices_al
         if order.get("SL"):
             self.portfolio.loc[open_trade, "SL"] =  order.get("SL")
         
-        str_act = f"BTO {order['Symbol']} {current_Avg}th averging down @ {order['price']}"
+        str_act = f"{order['action']} {order['Symbol']} {actual_Avg}th averging down @ {order['price']}"
         return str_act
 
     def make_STC(self, order, open_trade, check_trail=False):
         trade = self.portfolio.loc[open_trade]
         stc_info = calc_stc_prices(trade, order)
         #Log portfolio
         for k, v in stc_info.items():
             self.portfolio.loc[open_trade, k] = v
         
         trailstat = self.compute_trail(open_trade)
         self.portfolio.loc[open_trade, "TrailStats"] = trailstat
         self.portfolio.loc[open_trade, "STC-Date"] = order["Date"]
         stc_price =  self.portfolio.loc[open_trade,"STC-Price"]
-        stc_utotal = self.portfolio.loc[open_trade,"STC-Amount"]
+        stc_utotal = self.portfolio.loc[open_trade,"STC-Qty"]
         suffx = ''
-        if stc_utotal >= trade['Amount']:
+        if stc_utotal >= trade['Qty']:
             suffx = " Closed"
             self.portfolio.loc[open_trade, "isOpen"] = 0
             
         if stc_price == "none" or stc_price is None:
-            str_STC = f"STC {order['Symbol']}  ({order['uQty']}), no price provided" + suffx
+            str_STC = f"{order['action']} {order['Symbol']}  ({order['Qty']}), no price provided" + suffx
         else:
-            str_STC = f"STC {order['Symbol']} ({order['uQty']}),{suffx} {stc_price:.2f}"
-            if stc_info['STC-Price-current'] is not None:           
-                       str_STC += f" current: {stc_info['STC-Price-current']:.2f} " 
-            if stc_info["STC-PnL"] is not None:
-                str_STC += f'PnL:{round(stc_info["STC-PnL"])}% ${round(stc_info["STC-PnL$"])}' 
-            if stc_info["STC-PnL-current"] is not None:
-                str_STC += f' Actual:{round(stc_info["STC-PnL-current"])}% ${round(stc_info["STC-PnL$-current"])}\n\t\t'
+            # str_STC = f"STC {order['Symbol']} ({order['Qty']}),{suffx} @{stc_price:.2f}"
+            str_STC = ""
+            if stc_info['STC-Price-actual'] is not None:           
+                str_STC += f"\t@{stc_price:.2f}, actual: {stc_info['STC-Price-actual']:.2f} " 
+            if stc_info["PnL"] is not None:
+                str_STC += f'\tPnL:{round(stc_info["PnL"])}% ${round(stc_info["PnL$"])}' 
+            if stc_info["PnL-actual"] is not None:
+                str_STC += f' Actual:{round(stc_info["PnL-actual"])}% ${round(stc_info["PnL$-actual"])}\n\t\t'
 
         if eval(order.get('# Closed', "0"))==1 :
             self.portfolio.loc[open_trade, "isOpen"]=0
-        str_STC = str_STC + " " + trailstat.replace('|', '\n\t\t')
+        str_STC = str_STC + " " + trailstat.replace('| ', '\n\t')
         return str_STC
 
     def compute_trail(self, open_trade):
         trade = self.portfolio.loc[open_trade]
         fname = self.dir_quotes + f"/{trade['Symbol']}.csv"
         if not op.exists(fname):
             return ""
         
         quotes = pd.read_csv(fname, on_bad_lines='skip')
         # start after BTO date
+        quotes = quotes.dropna()
         dates = quotes['timestamp'].apply(lambda x: datetime.fromtimestamp(x))
         msk = dates >= pd.to_datetime(trade['Date'])
         quotes = quotes[msk].reset_index(drop=True)
         
         # first price will be the actual
-        if not pd.isnull(trade["Price-current"]):
-            price0 = trade["Price-current"]
+        if not pd.isnull(trade["Price-actual"]):
+            price0 = trade["Price-actual"]
         else:
             price0 = trade["Price"]
         quotes.loc[0, ' quote'] = price0
 
         # Calculate trailingStops
         res_str = "TS:{},{}%,${},in {}"
         trailing_Stop = [.2, .3, .4, .5] 
         max_trails = []      
         quotes['highest'] = quotes[' quote'].cummax() #take the cumulative max
         quotes['perc'] = round((quotes[' quote'] - quotes[' quote'].loc[0])/ quotes[' quote'].loc[0] *100,2)
         for trl in trailing_Stop:
-            quotes[f'trailingstop{trl}'] = quotes['highest']*(1-trl) 
-            trl_ix = (quotes[f' quote'] <= quotes[f'trailingstop{trl}']).idxmax()
+            # Calculate trailing stop based on constant value
+            trailing_stop = quotes['highest'] - quotes[' quote'].loc[0]* trl
+            trl_ix = (quotes[' quote'] <= trailing_stop).idxmax()
             if trl_ix:
                 tdiff_str, trl_r = self.trailing_get_time(trade['Date'], quotes, trl_ix)
                 max_trails.extend([res_str.format(trl,trl_r['perc'],trl_r[' quote'],tdiff_str)])
         max_trails = "| ".join(max_trails)
         # get min max and their time
-        quotes_stats = ""
+        quotes_stats = "| "
         for st, ix in  zip(['min', 'max'],[ quotes['perc'].idxmin(),  quotes['perc'].idxmax()]):
             tdiff_str, trl_r = self.trailing_get_time(trade['Date'], quotes, ix)
             quotes_stats += f"{st},{trl_r['perc']}%,${trl_r[' quote']},in {tdiff_str}| "
         quotes_stats +=  "| " + max_trails
         return quotes_stats
 
     def trailing_get_time(self, trade_date, quotes, inx):
@@ -232,84 +237,82 @@
                     self.portfolio.loc[i, k] = v
                 
                 self.portfolio.loc[i, "isOpen"] = 0
                 str_prt = f"{trade['Symbol']} option expired -100%"
                 print(str_prt)
         self.portfolio.to_csv(self.portfolio_fname, index=False)
 
-
-
 def calc_stc_prices(trade, order=None):
     # if order is None = expired option
     if order is None:
         order = {
             "price":0,
             "Actual Cost":0,
             "expired": True
             }
     bto_price = trade["Price"]
-    bto_price_al = trade["Price-current"]
+    bto_price_al = trade["Price-actual"]
     
     if not order.get('expired', False):
-        if order['uQty'] is None:
-            uQty = 1
+        if order['Qty'] is None:
+            Qty = 1
         else:
-            uQty = order['uQty']
+            Qty = order['Qty']
     else: 
-        if pd.isnull(trade["STC-Amount"]):
-            uQty = trade['Amount'] 
+        if pd.isnull(trade["STC-Qty"]):
+            Qty = trade['Qty'] 
         else:
-            uQty = trade['Amount'] - trade["STC-Amount"]
+            Qty = trade['Qty'] - trade["STC-Qty"]
     
     if isinstance(bto_price, str):
         bto_price =  np.mean(eval(bto_price.replace("/", ",")))
     if isinstance(bto_price_al, str):
         if bto_price_al[0] == '/':
             bto_price_al = bto_price_al[1:]
         bto_price_al =  np.mean(eval(bto_price_al.replace("/", ",")))
     
     if not pd.isnull(trade["STC-Price"]):  # previous stcs            
-        stc_wprice = trade["STC-Price"] * trade["STC-Amount"]
-        stc_utotal = trade["STC-Amount"] + uQty
-        stc_price = (order.get("price") * uQty +  stc_wprice)/stc_utotal      
+        stc_wprice = trade["STC-Price"] * trade["STC-Qty"]
+        stc_utotal = trade["STC-Qty"] + Qty
+        stc_price = (order.get("price") * Qty +  stc_wprice)/stc_utotal      
         prices = "/".join([str(trade["STC-Prices"]), str(order.get("price"))])
         
-        if pd.isnull(trade["STC-Price-current"]) or pd.isnull(order.get("Actual Cost")):
+        if pd.isnull(trade["STC-Price-actual"]) or pd.isnull(order.get("Actual Cost")):
             prices_curr = 0 if order.get('expired', False) else ""
             stc_price_al = 0 if order.get('expired', False) else None
         else:
-            stc_wprice = trade["STC-Price-current"] * trade["STC-Amount"]
-            stc_price_al = (order.get("Actual Cost") * uQty +  stc_wprice)/stc_utotal
-            prices_curr = "/".join([str(trade["STC-Prices-current"]), str(order.get("Actual Cost"))])
+            stc_wprice = trade["STC-Price-actual"] * trade["STC-Qty"]
+            stc_price_al = (order.get("Actual Cost") * Qty +  stc_wprice)/stc_utotal
+            prices_curr = "/".join([str(trade["STC-Prices-actual"]), str(order.get("Actual Cost"))])
     else:  # non-previous stcs   
         stc_price = order.get("price")
         stc_price_al = order.get("Actual Cost")
-        stc_utotal = uQty
+        stc_utotal = Qty
         prices = order.get("price")
         prices_curr = order.get("Actual Cost")
     
     mutipl = 1 if trade['Asset'] == "option" else .01  # pnl already in %
-    if stc_price is not None: 
+    if stc_price is not None and bto_price != 0: 
         stc_pnl = float((stc_price - bto_price)/bto_price) *100
         stc_pnl_u = stc_pnl* bto_price *mutipl*stc_utotal 
     else:
         stc_pnl = None
         stc_pnl_u = None
     
     if stc_price_al is None or pd.isnull(bto_price_al) or bto_price_al == 0:
         stc_pnl_al = None
         stc_pnl_al_u = None
     else:
         stc_pnl_al = float((stc_price_al - bto_price_al)/bto_price_al) *100
         stc_pnl_al_u = stc_pnl_al* bto_price_al *mutipl*stc_utotal 
 
     stc_info = {"STC-Prices":prices,
-                "STC-Prices-current": prices_curr,
+                "STC-Prices-actual": prices_curr,
                 "STC-Price": stc_price,
-                "STC-Price-current": stc_price_al,
-                "STC-Amount": stc_utotal,
-                "STC-PnL": stc_pnl,
-                "STC-PnL-current": stc_pnl_al,
-                "STC-PnL$": stc_pnl_u,
-                "STC-PnL$-current": stc_pnl_al_u,
+                "STC-Price-actual": stc_price_al,
+                "STC-Qty": stc_utotal,
+                "PnL": stc_pnl,
+                "PnL-actual": stc_pnl_al,
+                "PnL$": stc_pnl_u,
+                "PnL$-actual": stc_pnl_al_u,
                 }
     return stc_info
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_trader.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_trader.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 @author: adonay
 """
 import re
 import os.path as op
 import numpy as np
 import pandas as pd
-from datetime import datetime, date
+from datetime import datetime, timedelta, date
 import time
 import threading
 import queue
 from colorama import Fore, Back
 
 from DiscordAlertsTrader.configurator import cfg
-from DiscordAlertsTrader.message_parser import parse_exit_plan, set_exit_price_type
+from DiscordAlertsTrader.message_parser import parse_exit_plan, set_exit_price_type, ordersymb_to_str
 
 
 def find_last_trade(order, trades_log, open_only=True):
     trades_authr = trades_log["Trader"] == order["Trader"]
     trades_log = trades_log.loc[trades_authr]
 
     msk_ticker = trades_log["Symbol"].str.match(f"{order['Symbol']}$")
@@ -57,58 +57,63 @@
 
 class AlertsTrader():
     def __init__(self,
                  brokerage,
                  portfolio_fname=cfg['portfolio_names']['portfolio_fname'] ,
                  alerts_log_fname=cfg['portfolio_names']['alerts_log_fname'],
                  queue_prints=queue.Queue(maxsize=10),
-                 update_portfolio=True):
+                 update_portfolio=True,
+                 cfg=cfg
+                 ):
         self.bksession = brokerage
         self.portfolio_fname = portfolio_fname
         self.alerts_log_fname = alerts_log_fname
         self.queue_prints = queue_prints
-        
+        self.send_alert_to_discord = cfg['discord'].getboolean('notify_alerts_to_discord')
+        self.discord_channel = None # discord channel object to post trade alerts, passed on_ready discord
+        self.cfg = cfg
+        self.EOD = {} # end of day shorting actions
         # load port and log
         if op.exists(self.portfolio_fname):
             self.portfolio = pd.read_csv(self.portfolio_fname)
         else:
-            self.portfolio = pd.DataFrame(columns=cfg["col_names"]['portfolio'].split(",") )
+            self.portfolio = pd.DataFrame(columns=self.cfg["col_names"]['portfolio'].split(",") )
             self.portfolio.to_csv(self.portfolio_fname, index=False)
         if op.exists(self.alerts_log_fname):
             self.alerts_log = pd.read_csv(self.alerts_log_fname)
         else:
-            self.alerts_log = pd.DataFrame(columns=cfg["col_names"]['alerts_log'].split(","))
+            self.alerts_log = pd.DataFrame(columns=self.cfg["col_names"]['alerts_log'].split(","))
             self.alerts_log.to_csv(self.alerts_log_fname, index=False)
 
         self.update_portfolio = update_portfolio
         self.update_paused = False
         if update_portfolio:
             # first do a synch, then thread it
             self.update_orders()
             self.activate_trade_updater()
 
-    def activate_trade_updater(self, refresh_rate=30):
+    def activate_trade_updater(self, refresh_rate=10):
         self.update_portfolio = True
-        self.updater = threading.Thread(target=self.trade_updater, args=[refresh_rate])
+        self.updater = threading.Thread(target=self.trade_updater, args=[refresh_rate], daemon=True)
         self.updater.start()
         self.queue_prints.put([f"Updating portfolio orders every {refresh_rate} secs", "", "green"])
         print(Back.GREEN + f"Updating portfolio orders every {refresh_rate} secs")
 
-    def trade_updater_reset(self, refresh_rate=30):
+    def trade_updater_reset(self, refresh_rate=10):
         """ Will stop threding updater and restart.
         To avoid delays or parallel updatings. """
         self.update_portfolio = False
         time.sleep(refresh_rate)
         self.activate_trade_updater(refresh_rate)
 
     def _stop(self):
         "Lazy trick to stop updater threading"
         self.update_portfolio = False
 
-    def trade_updater(self, refresh_rate=30):
+    def trade_updater(self, refresh_rate=10):
         while self.update_portfolio is True:
             if self.update_paused is False:
                 try:
                     self.update_orders()
                 except Exception as ex:
                     str_msg = f"Error raised during port update, trying again later. Error: {ex}"
                     print(Back.RED + str_msg)
@@ -123,25 +128,66 @@
         if "port" in csvs:
             self.portfolio.to_csv(self.portfolio_fname, index=False)
         if "alert" in csvs:
             self.alerts_log.to_csv(self.alerts_log_fname, index=False)
 
     def order_to_pars(self, order):
         pars_str = f"{order['action']} {order['Symbol']} @{order['price']}"
-        if {order['action']} == "BTO":
+        if order['action'] in ["BTO", "STO"]:
             for i in range(1, 4):
                 pt = f"PT{i}"
                 if pt in order.keys() and order[pt] is not None:
                     pars_str = pars_str + f" {pt}: {order[pt]}"
                 if "SL" in order.keys() and order["SL"] is not None:
                     pars_str = pars_str + f" SL: {order['SL']}"
-        elif {order['action']} == "STC":
-            pars_str = pars_str + f" Qty:{order['uQty']}({int(order['xQty']*100)}%)"
+        elif order['action'] in ["STC", "BTC"]:
+            pars_str = pars_str + f" Qty:{order['Qty']}({int(order['xQty']*100)}%)"
         return pars_str
 
+    def disc_notifier(self,order_info):
+        from discord_webhook import DiscordWebhook
+        if not self.send_alert_to_discord:
+            return
+        
+        if order_info['status'] not in ['FILLED', 'EXECUTED', 'INDIVIDUAL_FILLS']:
+            print("order in notifier not filled")
+            return
+        
+        if order_info.get('orderLegCollection') is None:            
+            if order_info['childOrderStrategies'][0]['status'] == "FILLED":
+                order_info = order_info['childOrderStrategies'][0]
+            elif order_info['childOrderStrategies'][1]['status'] == "FILLED":
+                order_info = order_info['childOrderStrategies'][1]
+        
+        if order_info['orderLegCollection'][0]['instruction'] in ["BUY_TO_OPEN", "BUY"]:
+            action = "BTO"
+        elif order_info['orderLegCollection'][0]['instruction'] in ["SELL_TO_CLOSE", "SELL"]:
+            action = "STC"
+        elif order_info['orderLegCollection'][0]['instruction'] in ["SELL_TO_OPEN", "SELL_SHORT"]:
+            action = "STO"
+        elif order_info['orderLegCollection'][0]['instruction'] in ["BUY_TO_CLOSE", "BUY_TO_COVER"]:
+            action = "BTC"
+
+        symbol = ordersymb_to_str(order_info['orderLegCollection'][0]['instrument']['symbol'])
+        msg = f"{action} {order_info['filledQuantity']} {symbol} @{order_info.get('price')}"
+        
+        if len(self.cfg['discord']['webhook']):
+            webhook = DiscordWebhook(
+                url=self.cfg['discord']['webhook'], 
+                username=self.cfg['discord']['webhook_name'], 
+                content=f'{msg.upper()}', 
+                rate_limit_retry=True)
+            webhook.execute()
+            print("webhook sent")
+        
+        if self.discord_channel is not None:
+            # self.discord_send(msg, self.discord_channel)
+            # self.discord_channel.send(msg.upper())
+            print("discord channel message sent")
+
     def price_now(self, symbol, price_type="BTO", pflag=0):
         if price_type in ["BTO", "BTC"]:
             ptype = 'askPrice'
         else:
             ptype= 'bidPrice'
         try:
             resp = self.bksession.get_quotes([symbol])
@@ -181,84 +227,158 @@
                 color = "green" if order['action'] == "BTO" else "yellow"
                 self.queue_prints.put([str_msg, "", color])
                 return ord_resp, ord_id, order, ord_chngd
 
             elif resp in ["no", "n"]:
                 return None, None, order, None
 
+    def short_orders(self, order, pars):
+        if order['action'] == "STO":
+            # check strike
+            strike = eval(re.split("C|P", order['Symbol'].split("_")[1])[1])
+            if strike > eval(self.cfg['shorting']['max_strike']):
+                str_msg = f"STO strike too high: {strike}, order aborted"
+                print(Back.RED + str_msg)
+                self.queue_prints.put([str_msg, "", "red"])
+                return "no", order, False
+            
+            # check DTE
+            if len(self.cfg['shorting']['max_dte']):
+                if order.get('dte') is None:
+                    exp_dt = datetime.strptime(f"{order['expDate']}/{datetime.now().year}" , "%m/%d/%Y").date()
+                    dt = datetime.now().date()
+                    order['dte'] =  (exp_dt - dt).days
+                if order['dte'] > int(self.cfg['shorting']['max_dte']):
+                    str_msg = f"STO {order['dte']} DTE larger than max in config: {self.cfg['shorting']['max_dte']}, order aborted"
+                    print(Back.RED + str_msg)
+                    self.queue_prints.put([str_msg, "", "red"])
+                    return "no", order, False
+            
+            # check if above min price
+            if len(self.cfg['shorting']['min_price']):
+                min_price = float(self.cfg['shorting']['min_price'])
+                if (order['price']*100) < min_price:
+                    str_msg = f"STO price too low: {order['price']*100}, order aborted"
+                    print(Back.RED + str_msg)
+                    self.queue_prints.put([str_msg, "", "red"])
+                    return "no", order, False
+            
+            if self.cfg['shorting']['STO_trailingstop'] != "":
+                trail = (float(self.cfg['shorting']['STO_trailingstop'])/100)*order["price_actual"]  
+                order["trail_stop_const"] = -round(trail / 0.01) * 0.01
+            else:
+                # if price diff not too high, use current price
+                pdiff = round((order['price']-order["price_actual"])/order['price']*100,1)
+                if pdiff < eval(self.cfg['shorting']['max_price_diff']):
+                    order['price'] = order["price_actual"]
+                else:
+                    str_msg = f"STO alert price diff too high: {pdiff}% at {order['price_actual']}, keeping original price of {order['price']}"
+                    print(Back.GREEN + str_msg)
+                    self.queue_prints.put([str_msg, "", "green"])
+            
+            # Handle quantity            
+            if self.cfg['shorting']['default_sto_qty'] == "buy_one":
+                order['Qty'] = 1                    
+            elif self.cfg['shorting']['default_sto_qty'] == "underlying_capital":
+                order['Qty'] = eval(self.cfg['shorting']['underlying_capital'])//strike
+
+            # Handle trade too expensive
+            max_trade_val = float(self.cfg['shorting']['max_trade_capital'])
+            if order['price'] * order['Qty'] > max_trade_val:
+                Qty_ori = order['Qty']
+                order['Qty'] =  int(max(max_trade_val//order['price'], 1))
+                if order['price'] * order['Qty'] <= max_trade_val:
+                    str_msg = f"STO trade exeeded max_trade_capital of ${max_trade_val}, order quantity reduced to {order['Qty']} from {Qty_ori}"
+                    print(Back.GREEN + str_msg)
+                    self.queue_prints.put([str_msg, "", "green"])
+                else:
+                    str_msg = f"cancelled STO: trade exeeded max_trade_capital of ${max_trade_val}"
+                    print(Back.RED + str_msg)
+                    self.queue_prints.put([str_msg, "", "red"])
+                    return "no", order, False
+            return "yes", order, False
+        # decide if do BTC based on alert
+        elif order['action'] == "BTC":
+            return "yes", order, False
+        else:
+            return "no", order, False
+
     def notify_alert(self, order, pars):
         price_now = self.price_now
         symb = order['Symbol']
         ord_ori = order.copy()
         pars_ori = pars
         act = order['action']
 
         while True:
             # If symbol not found, quote val returned is -1
             if price_now(symb, act, 1 ) == -1:
                 return "no", order, False
 
-            current_price = price_now(symb, act, 1 )
-            order["price_current"] = current_price
-            pdiff = (current_price - ord_ori['price'])/ord_ori['price']
+            actual_price = price_now(symb, act, 1 )
+            order["price_actual"] = actual_price
+            pdiff = (actual_price - ord_ori['price'])/ord_ori['price']
             pdiff = round(pdiff*100,1)
 
             question = f"{pars_ori} {price_now(symb, act)}"
-            if cfg['order_configs'].getboolean('sell_current_price'):
-                if pdiff < eval(cfg['order_configs']['max_price_diff'])[order["asset"]]:
+            if order['action'] in ["STO", "BTC"]:
+                return self.short_orders(order, pars)
+            
+            elif self.cfg['order_configs'].getboolean('sell_actual_price'):
+                if pdiff < eval(self.cfg['order_configs']['max_price_diff'])[order["asset"]]:
                     order['price'] = price_now(symb, act, 1)
                     pars = self.order_to_pars(order)
                     question += f"\n new price: {pars}"
                 else:
-                    if cfg['order_configs'].getboolean('auto_trade') is True and order['action'] == "BTO":
-                        str_msg = f"BTO alert price diff too high: {pdiff}% at {current_price}, keeping original price of {ord_ori['price']}"
+                    if self.cfg['order_configs'].getboolean('auto_trade') is True and order['action'] == "BTO":
+                        str_msg = f"BTO alert price diff too high: {pdiff}% at {actual_price}, keeping original price of {ord_ori['price']}"
                         print(Back.GREEN + str_msg)
                         self.queue_prints.put([str_msg, "", "green"])
 
-            if cfg['order_configs'].getboolean('auto_trade') is True:
-                if cfg['general'].getboolean('DO_BTO_TRADES') is False and order['action'] == "BTO":
+            if self.cfg['order_configs'].getboolean('auto_trade') is True:
+                if self.cfg['general'].getboolean('DO_BTO_TRADES') is False and order['action'] == "BTO":
                     str_msg = f"BTO not accepted by config options: DO_BTO_TRADES = False"
                     print(Back.GREEN + str_msg)
                     self.queue_prints.put([str_msg, "", "green"])
                     return "no", order, False
                 elif order['action'] == "BTO":
                     price = order['price']
                     if price == 0:
                         str_msg = f"Order not accepted price is 0"
                         print(Back.GREEN + str_msg)
                         self.queue_prints.put([str_msg, "", "red"])
                         return "no", order, False
                     price = price*100 if order["asset"] == "option" else price
-                    max_trade_val = float(cfg['order_configs']['max_trade_capital'])
+                    max_trade_val = float(self.cfg['order_configs']['max_trade_capital'])
 
-                    if 'uQty' not in order.keys() or order['uQty'] is None:
-                        if cfg['order_configs']['default_bto_qty'] == "buy_one":
-                            order['uQty'] = 1                    
-                        elif cfg['order_configs']['default_bto_qty'] == "trade_capital":
-                            order['uQty'] =  int(max(round(float(cfg['order_configs']['trade_capital'])/price), 1))
-
-                    if price * order['uQty'] > max_trade_val:
-                        uQty_ori = order['uQty']
-                        order['uQty'] =  int(max(max_trade_val//price, 1))
-                        if price * order['uQty'] <= max_trade_val:
-                            str_msg = f"BTO trade exeeded max_trade_capital of ${max_trade_val}, order quantity reduced to {order['uQty']} from {uQty_ori}"
+                    if 'Qty' not in order.keys() or order['Qty'] is None:
+                        if self.cfg['order_configs']['default_bto_qty'] == "buy_one":
+                            order['Qty'] = 1                    
+                        elif self.cfg['order_configs']['default_bto_qty'] == "trade_capital":
+                            order['Qty'] =  int(max(round(float(self.cfg['order_configs']['trade_capital'])/price), 1))
+
+                    if price * order['Qty'] > max_trade_val:
+                        Qty_ori = order['Qty']
+                        order['Qty'] =  int(max(max_trade_val//price, 1))
+                        if price * order['Qty'] <= max_trade_val:
+                            str_msg = f"BTO trade exeeded max_trade_capital of ${max_trade_val}, order quantity reduced to {order['Qty']} from {Qty_ori}"
                             print(Back.GREEN + str_msg)
                             self.queue_prints.put([str_msg, "", "green"])
                         else:
                             str_msg = f"cancelled BTO: trade exeeded max_trade_capital of ${max_trade_val}"
                             print(Back.RED + str_msg)
                             self.queue_prints.put([str_msg, "", "red"])
                             return "no", order, False
                 return "yes", order, False
 
             # Manual trade 
             resp = input(Back.RED  + question + "\n Make trade? (y, n or (c)hange) \n").lower()
 
-            if resp in [ "c", "change", "y", "yes"] and 'uQty' not in order.keys():
-                order['uQty'] = int(input("Order qty not available." +
+            if resp in [ "c", "change", "y", "yes"] and 'Qty' not in order.keys():
+                order['Qty'] = int(input("Order qty not available." +
                                           f" How many units to buy? {price_now(symb, act)} \n"))
 
             if resp in [ "c", "change"]:
                 new_order = order.copy()
                 new_order['price'] = float(input(f"Change price @{order['price']}" +
                                         f" {price_now(symb, act)}? Leave blank if NO \n")
                                       or order['price'])
@@ -302,22 +422,27 @@
 
             if ord_stat not in ["FILLED", "EXECUTED", 'CANCELED','CANCEL_REQUESTED','REJECTED', 'EXPIRED']:
                 print(Back.GREEN + f"Cancelling {position['Symbol']} STC{i}")
                 self.queue_prints.put([f"Cancelling {position['Symbol']} STC{i}", "", "green"])
                 _ = self.bksession.cancel_order(order_id)
 
                 self.portfolio.loc[open_trade, f"STC{i}-Status"] = np.nan
+                self.portfolio.loc[open_trade, f"STC{i}-ordID"] = np.nan                
+                self.save_logs("port")
+                
+            elif ord_stat in ["REJECTED", 'CANCELED','CANCEL_REQUESTED', 'EXPIRED']:
+                self.portfolio.loc[open_trade, f"STC{i}-Status"] = np.nan
                 self.portfolio.loc[open_trade, f"STC{i}-ordID"] = np.nan
                 self.save_logs("port")
 
 
     def get_order_info(self, order_id):
         try:
-             order_status, order_info = self.bksession.get_order_info(order_id)
-             return order_status, order_info
+            order_status, order_info = self.bksession.get_order_info(order_id)
+            return order_status, order_info
         except Exception as ex:
             print(f"Caught Error in order info, skipping order info retr. Error: {ex}")
             self.queue_prints.put([f"Caught Error, skipping order info retr. Error: {ex}", "", "red"])
             return None, None
 
 
     ######################################################################
@@ -336,120 +461,146 @@
                      "Symbol": order['Symbol'],
                      "Trader" : order['Trader'],
                      "parsed" : pars,
                      "msg": msg
                      }
 
         if order['action'] == "ExitUpdate" and isOpen:
-            #TODO : REMOVE
             # Pause updater to avoid overlapping
             self.update_paused = True
 
             old_plan = self.portfolio.loc[open_trade, "exit_plan"]
             new_plan = parse_exit_plan(order)
 
             # check if asset if price stock or contract
             if self.portfolio.loc[open_trade, "Asset"] == "option":
                 new_plan["price"] = self.portfolio.loc[open_trade, "Price"]
                 sym_inf = self.portfolio.loc[open_trade, "Symbol"].split("_")[1]
                 strike = re.split("C|P", sym_inf)[1]
-                new_plan["strike"] = strike + "C"
+                new_plan["strike"] = strike + "C" if "C" in sym_inf else strike + "P"
                 for i in range(1,4):
                     exit_price = new_plan.get(f"PT{i}")
                     if exit_price is not None:
                         new_plan[f"PT{i}"] = set_exit_price_type(exit_price, new_plan)
                     if new_plan.get("SL"):
                         new_plan[f"SL"] = set_exit_price_type(new_plan.get("SL"), new_plan)
                 _ = [new_plan.pop(k) for k in ['price', 'strike']]
 
             # Update PT is already STCn
             istc = None
             for i in range(1,3):
-                if not pd.isnull(self.portfolio.loc[open_trade, f"STC{i}-Alerted"]):
+                if not pd.isnull(self.portfolio.loc[open_trade, f"STC{i}-alerted"]):
                     istc = i+1
             if istc is not None and any(["PT" in k for k in new_plan.keys()]):
                 new_plan_c = new_plan.copy()
                 for i in range(1,4):
                     if new_plan.get(f"PT{i}"):
                         del new_plan_c[f"PT{i}"]
                         new_plan_c[f"PT{istc}"] = new_plan[f"PT{i}"]
                         # Cancel orders previous plan if any
                         self.close_open_exit_orders(open_trade, istc)
                 new_plan = new_plan
-
+            else:
+                # Cancel orders previous plan if any
+                self.close_open_exit_orders(open_trade)
+                
             renew_plan = eval(old_plan)
             if renew_plan is not None or renew_plan != {}:
                 for k in new_plan.keys():
                     renew_plan[k] = new_plan[k]
             else:
                 renew_plan = new_plan
-
+                
             self.portfolio.loc[open_trade, "exit_plan"] = str(renew_plan)
             self.update_paused = False
 
             log_alert['action'] = "ExitUpdate"
             self.save_logs()
 
             symb = self.portfolio.loc[open_trade, "Symbol"]
             print(Back.GREEN + f"Updated {symb} exit plan from :{old_plan} to {renew_plan}")
             self.queue_prints.put([f"Updated {symb} exit plan from :{old_plan} to {renew_plan}", "", "green"])
             return
 
-        if not isOpen and order["action"] == "BTO":
-            alert_price = order['price']
-
+        elif not isOpen and order["action"] in ["BTO", "STO"]:
+            alert_price = order["price"]
+            action = order["action"]
             order_response, order_id, order, _ = self.confirm_and_send(order, pars, self.bksession.make_BTO_lim_order)
+    
             self.save_logs("port")
             if order_response is None:  #Assume trade not accepted
-                log_alert['action'] = "BTO-notAccepted"                
+                log_alert['action'] = action+"-notAccepted"                
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs(["alert"])
-                str_msg = "BTO not accepted by user, order response is none"
+                str_msg = action+" not accepted by user, order response is none"
                 print(Back.GREEN + str_msg)
                 self.queue_prints.put([str_msg, "", "green"])
                 return
 
             order_status, order_info = self.get_order_info(order_id)
             if order_status == 'REJECTED':                
                 log_alert['action'] = "REJECTED"
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs(["alert"])
-                print(Back.GREEN + "BTO REJECTED")
-                self.queue_prints.put(["BTO REJECTED", "", "green"])
+                print(Back.GREEN + action+" REJECTED")
+                self.queue_prints.put([action+" REJECTED", "", "green"])
                 return
             
+            # Get exit plan and add default vals if needed
             exit_plan = parse_exit_plan(order)
+            if order['action'] == "BTO":
+                if len(self.cfg["order_configs"]["default_exits"]) and \
+                    exit_plan.get("PT") is None and exit_plan.get("SL") is None:
+                    exit_plan = eval(self.cfg["order_configs"]["default_exits"])
+            elif order['action'] == "STO":
+                price = order_info.get("price")
+                if price is None:
+                    price = order_info.get('activationPrice')
+
             new_trade = {"Date": date,
                          "Symbol": order['Symbol'],
                          'isOpen': 1,
-                         'BTO-Status' : order_status,
-                         "uQty": order_info['quantity'],
-                         "Asset" : order["asset"],
-                         "Type" : "BTO",
-                         "Price" : order_info["price"],
-                         "Price-Alert" : alert_price,
-                         "Price-Current": order["price_current"],
-                         "ordID" : order_id,
-                         "exit_plan" : str(exit_plan),
-                         "Trader" : order['Trader'],
-                         "Risk" : order['risk'],
-                         "SL_mental" : order.get("SL_mental")
+                         'BTO-Status': order_status,
+                         "Qty": order_info['quantity'],
+                         "Asset": order["asset"],
+                         "Type": action,
+                         "Price": order_info.get("price"),
+                         "Price-alert": alert_price,
+                         "Price-actual": order["price_actual"],
+                         "ordID": order_id,
+                         "exit_plan": str(exit_plan),
+                         "Trader": order['Trader'],
+                         "Risk": order['risk'],
+                         "SL_mental": order.get("SL_mental")
                          }
 
             self.portfolio = pd.concat([self.portfolio, pd.DataFrame.from_records(new_trade, index=[0])], ignore_index=True)
             
             if order_status in ["FILLED", "EXECUTED"]:
                 ot, _ = find_last_trade(order, self.portfolio)
                 self.portfolio.loc[ot, "Price"] = order_info['price']
                 self.portfolio.loc[ot, "filledQty"] = order_info['filledQuantity']
-            print(Back.GREEN + f"BTO {order['Symbol']} executed @ {order_info['price']}. Status: {order_status}")
-            self.queue_prints.put([f"BTO {order['Symbol']} executed. Status: {order_status}", "", "green"])
-
+                self.disc_notifier(order_info)
+                if self.portfolio.loc[ot, "Type"] == "STO":
+                    price = order_info.get("price")
+                    if len(self.cfg['shorting']['BTC_PT']) and exit_plan.get("PT1") is None:
+                        exit_plan['PT1'] = round(price * (1 - float(self.cfg['shorting']['BTC_PT'])/100),2)
+                    if len(self.cfg['shorting']['BTC_SL']) and exit_plan.get("SL") is None:
+                        exit_plan['SL'] = round(price * (1 + float(self.cfg['shorting']['BTC_SL'])/100),2)
+                    self.portfolio.loc[ot,"exit_plan"]= str(exit_plan)
+                
+                # convert % to val exit plan
+                self.exit_percent_to_price(ot)
+                
+            str_msg = f"{action} {order['Symbol']} executed @ {order_info.get('price')}. Status: {order_status}"
+            print(Back.GREEN + str_msg)
+            self.queue_prints.put([str_msg, "", "green"])
+            
             #Log portfolio, trades_log
-            log_alert['action'] = "BTO"
+            log_alert['action'] = action
             log_alert["portfolio_idx"] = len(self.portfolio) - 1
             self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
             self.save_logs()
 
         elif order["action"] == "BTO" and order['avg'] is not None:
             # if PT in order: cancel previous and make_BTO_lim_rder
             # else : BTO
@@ -469,100 +620,104 @@
             self.portfolio.loc[open_trade,'BTO-avg-Status'] = order_status
             self.portfolio.loc[open_trade,"ordID"] += f',{order_id}'
 
             if pd.isnull(self.portfolio.loc[open_trade, "Avged"]):
                 self.portfolio.loc[open_trade, "Avged"] = 1
                 self.portfolio.loc[open_trade, "Avged-prices-alert"] = alert_price
                 self.portfolio.loc[open_trade, "Avged-prices"] = order_info["price"]
-                self.portfolio.loc[open_trade, "Avged-uQty"] = order_info['quantity']
+                self.portfolio.loc[open_trade, "Avged-Qty"] = order_info['quantity']
 
             else:
                 self.portfolio.loc[open_trade, "Avged"] += 1
                 al_pr = self.portfolio.loc[open_trade, "Avged-prices-alert"]
                 av_pr = self.portfolio.loc[open_trade, "Avged-prices"]
-                av_qt = self.portfolio.loc[open_trade, "Avged-uQty"]
+                av_qt = self.portfolio.loc[open_trade, "Avged-Qty"]
                 self.portfolio.loc[open_trade, "Avged-prices-alert"] = f"{al_pr},{alert_price}"
                 self.portfolio.loc[open_trade, "Avged-prices"] = f"{av_pr},{order_info['price']}"
-                self.portfolio.loc[open_trade, "Avged-uQty"] = f"{av_qt},{order_info['quantity']}"
+                self.portfolio.loc[open_trade, "Avged-Qty"] = f"{av_qt},{order_info['quantity']}"
 
             avg = self.portfolio.loc[open_trade, "Avged"]
 
-            self.portfolio.loc[open_trade, "uQty"] += order_info['quantity']
+            self.portfolio.loc[open_trade, "Qty"] += order_info['quantity']
             if  order_status in ["FILLED", "EXECUTED"]:
                 self.portfolio.loc[open_trade, "filledQty"] += order_info['filledQuantity']
+                self.disc_notifier(order_info)
                 self.close_open_exit_orders(open_trade)
-            str_msg =  f"BTO {avg} th AVG, {order['Symbol']} executed. Status: {order_status}"
+            str_msg =  f"BTO {avg} th AVG, {order['Symbol']} executed @{order_info['price']}. Status: {order_status}"
             print(Back.GREEN + str_msg)
             self.queue_prints.put([str_msg, "", "green"])
 
             #Log portfolio, trades_log
             log_alert['action'] = "BTO-avg"
             log_alert["portfolio_idx"] = len(self.portfolio) - 1
             self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
             self.save_logs()
 
-        elif order["action"] == "BTO":
-            str_act = "Repeated BTO"
-            log_alert['action'] = "BTO-Null-Repeated"
+        elif order["action"] in ["BTO", "STO"]:
+            str_act = f"Repeated {order['action']}"
+            log_alert['action'] = f"{order['action']}-Null-Repeated"
             self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
             self.save_logs(["alert"])
             print(Back.RED + str_act)
             self.queue_prints.put([str_act, "", "red"])
 
-        elif order["action"] == "STC" and isOpen == 0:
+        elif order["action"] in ["STC", "BTC"] and isOpen == 0:
             open_trade, _ = find_last_trade(order, self.portfolio, open_only=False)
             if open_trade is None:
-                log_alert['action'] = str_msg = f"STC-alerted without open position"
+                log_alert['action'] = str_msg = f"{order['action']}-alerted without open position"
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs()
-                if cfg['general'].getboolean('DO_BTO_TRADES'):
+                if (self.cfg['general'].getboolean('DO_BTO_TRADES') and order["action"] == "STC") or \
+                    (self.cfg['general'].getboolean('DO_STO_TRADES') and order["action"] == "BTC"):
                     print(Back.GREEN + str_msg)
                     self.queue_prints.put([str_msg, "", "green"])
                 return
 
             position = self.portfolio.iloc[open_trade]
             # Check if closed position was not alerted
             for i in range(1,4):
                 STC = f"STC{i}"
-                if pd.isnull(position[f"{STC}-Alerted"]):
-                    self.portfolio.loc[open_trade, f"{STC}-Alerted"] = 1
+                if pd.isnull(position[f"{STC}-alerted"]):
+                    self.portfolio.loc[open_trade, f"{STC}-alerted"] = 1
                     # If alerted and already sold
                     if not pd.isnull(position[ f"{STC}-Price"]):
                         print(Back.RED + "Position already closed")
                         self.queue_prints.put(["Position already closed", "", "red"])
                         log_alert['action'] = f"{STC}-alerterdAfterClose"
                         log_alert["portfolio_idx"] = open_trade
                         self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                         self.save_logs()
                     return
 
-            str_act = "STC without BTO, maybe alredy sold"
-            log_alert['action'] = "STC-Null-notOpen"
+            if order["action"] == "STC":
+                str_act = "STC without BTO, maybe alredy sold"
+            elif order["action"] == "BTC":
+                str_act = "BTC without STO, maybe alredy bought"
+            log_alert['action'] = f"{order['action']}-Null-notOpen"
             self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
             self.save_logs(["alert"])
             print(Back.RED + str_act)
             self.queue_prints.put([str_act, "", "red"])
 
-        elif order["action"] == "STC":
+        elif order["action"] in ["STC", "BTC"]:
             position = self.portfolio.iloc[open_trade]
             if order.get("amnt_left"):
                 order, changed = amnt_left(order, position)
                 print(Back.GREEN + f"Based on alerted amnt left, Updated order: " +
-                      f"xQty: {order['xQty']} and uQty: {order['uQty']}")
+                      f"xQty: {order['xQty']} and Qty: {order['Qty']}")
                 self.queue_prints.put([f"Based on alerted amnt left, Updated order: " +
-                      f"xQty: {order['xQty']} and uQty: {order['uQty']}", "", "green"])
+                      f"xQty: {order['xQty']} and Qty: {order['Qty']}", "", "green"])
 
             # check if position already alerted and closed
             for i in range(1,4):
                 STC = f"STC{i}"
-
                 # If not alerted, mark it
-                if pd.isnull(position[f"{STC}-Alerted"]):
-                    self.portfolio.loc[open_trade, f"{STC}-Alerted"] = 1 
-                    self.portfolio.loc[open_trade, STC + "-Price-Alerted"] = order["price"]
+                if pd.isnull(position[f"{STC}-alerted"]):
+                    self.portfolio.loc[open_trade, f"{STC}-alerted"] = 1 
+                    self.portfolio.loc[open_trade, STC + "-Price-alert"] = order["price"]
                     # If alerted and already sold
                     if not pd.isnull(position[ f"{STC}-Price"]):
                         print(Back.GREEN + "Already sold")
                         self.queue_prints.put(["Already sold", "", "green"])
 
                         log_alert['action'] = f"{STC}-DoneBefore"
                         log_alert["portfolio_idx"] = open_trade
@@ -570,18 +725,18 @@
                         self.save_logs(["alert"])
 
                         if order['xQty'] != 1:  # if partial and sold, leave
                             return
                     break
 
             else:
-                str_STC = "How many STC already?"
+                str_STC = f"How many {order['action']} already?"
                 print (Back.RED + str_STC)
                 self.queue_prints.put([str_STC, "", "red"])
-                log_alert['action'] = "STC-TooMany"
+                log_alert['action'] = f"{order['action']}-TooMany"
                 log_alert["portfolio_idx"] = open_trade
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs(["alert"])
                 return
 
             qty_bought = position["filledQty"]
 
@@ -602,33 +757,33 @@
 
                 order_status, _ =  self.get_order_info(order_id)
                 self.portfolio.loc[open_trade, "BTO-Status"] = order_status
 
                 print(Back.GREEN + f"Order Cancelled {order['Symbol']}, closed before fill")
                 self.queue_prints.put([f"Order Cancelled {order['Symbol']}, closed before fill", "", "green"])
 
-                log_alert['action'] = "STC-ClosedBeforeFill"
+                log_alert['action'] = f"{order['action']}-ClosedBeforeFill"
                 log_alert["portfolio_idx"] = open_trade
                 self.save_logs()
-                # self.activate_trade_updater()
                 return
-            # Set STC as exit plan
+            
+            # Set STC as exit plan, not bought yet
             elif qty_bought == 0:
                 exit_plan = eval(self.portfolio.loc[open_trade, "exit_plan"])
                 exit_plan[f"PT{STC[-1]}"] = order["price"]
                 self.portfolio.loc[open_trade, "exit_plan"] = str(exit_plan)
                 str_msg = f"Exit Plan {order['Symbol']} updated, with PT{STC[-1]}: {order['price']}"
                 print(Back.GREEN + str_msg)
                 self.queue_prints.put([str_msg,"", "green"])
-                log_alert['action'] = "STC-partial-BeforeFill-ExUp"
+                log_alert['action'] = f"{order['action']}-partial-BeforeFill-ExUp"
                 log_alert["portfolio_idx"] = open_trade
                 return
 
-            qty_sold = np.nansum([position[f"STC{i}-uQty"] for i in range(1,4)])
-            if position["uQty"] - qty_sold == 0:
+            qty_sold = np.nansum([position[f"STC{i}-Qty"] for i in range(1,4)])
+            if position["Qty"] - qty_sold == 0:
                 self.portfolio.loc[open_trade, "isOpen"] = 0
                 print(Back.GREEN + "Already sold")
                 self.queue_prints.put(["Already sold", "", "green"])
 
                 log_alert['action'] = f"{STC}-DoneBefore"
                 log_alert["portfolio_idx"] = open_trade
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
@@ -637,204 +792,369 @@
 
             # Sell all and close waiting stc orders
             if order['xQty'] == 1:                
                 # Stop updater to avoid overlapping
                 self.update_paused = True
                 # Sell all and close waiting stc orders
                 self.close_open_exit_orders(open_trade)
-                
-                # if no uQty get all remaining
-                if order['uQty'] is None:
+                self.update_paused = False
+                # if no Qty get all remaining
+                if order['Qty'] is None:
                     position = self.portfolio.iloc[open_trade]
-                    order['uQty'] = int(position["uQty"]) - qty_sold
+                    order['Qty'] = int(position["Qty"]) - qty_sold
 
             elif order['xQty'] < 1:  # portion
                 # Stop updater to avoid overlapping
                 self.update_paused = True
                 self.close_open_exit_orders(open_trade)
-                order['uQty'] = round(max(qty_bought * order['xQty'], 1))
+                self.update_paused = False
+                order['Qty'] = round(max(qty_bought * order['xQty'], 1))
 
-            if order['uQty'] + qty_sold > qty_bought:
-                order['uQty'] = qty_bought - qty_sold
-                str_msg = f"Order {order['Symbol']} Qty exceeded, changed to {order['uQty']}"
+            if order['Qty'] + qty_sold > qty_bought:
+                order['Qty'] = int(qty_bought - qty_sold)
+                str_msg = f"Order {order['Symbol']} Qty exceeded, changed to {order['Qty']}"
                 print(Back.RED + Fore.BLACK + str_msg)
                 self.queue_prints.put([str_msg, "", "red"])
 
+            self.update_paused = True
             order_response, order_id, order, _ = self.confirm_and_send(order, pars, self.bksession.make_STC_lim)
+            self.update_paused = False
             log_alert["portfolio_idx"] = open_trade
 
             if order_response is None:  # Assume trade rejected by user
-                log_alert['action'] = "STC-notAccepted"
+                log_alert['action'] = f"{order['action']}-notAccepted"
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs(["alert"])
-                print(Back.GREEN + "STC not accepted by user, order response null")
-                self.queue_prints.put(["STC not accepted by user, order response null", "", "green"])
-                self.update_paused = False
+                msg_str = f"{order['action']} not accepted by user, order response null"
+                print(Back.GREEN + msg_str)
+                self.queue_prints.put([msg_str, "", "green"])
                 return
 
             order_status, order_info = self.get_order_info(order_id)
             self.portfolio.loc[open_trade, STC + "-ordID"] = order_id
-            self.portfolio.loc[open_trade, STC + "-Price-Current"] = order["price_current"]
+            self.portfolio.loc[open_trade, STC + "-Price-actual"] = order["price_actual"]
 
             # Check if STC price changed
             if order_status in ["FILLED", 'EXECUTED', 'INDIVIDUAL_FILLS']:
+                self.disc_notifier(order_info)
                 self.log_filled_STC(order_id, open_trade, STC)
             else:
-                str_STC = f"Submitted: {STC} {order['Symbol']} @{order['price']} Qty:{order['uQty']} ({order['xQty']})"
+                str_STC = f"Submitted: {STC} {order['Symbol']} @{order['price']} Qty:{order['Qty']} ({order['xQty']})"
                 print(Back.GREEN + str_STC)
                 self.queue_prints.put([str_STC, "", "green"])
 
             #Log trades_log
             log_alert['action'] = "STC-partial" if order['xQty']<1 else "STC-ALL"
             self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
             self.save_logs()
 
-            self.update_paused = False
-
 
     def log_filled_STC(self, order_id, open_trade, STC):
-
         order_status, order_info = self.get_order_info(order_id)
-
-        sold_unts = order_info['orderLegCollection'][0]['quantity']
+        if order_info.get('orderLegCollection'):
+            sold_unts = order_info['orderLegCollection'][0]['quantity']
+        else: 
+            if order_info['childOrderStrategies'][0]['status'] == "FILLED":
+                order_info = order_info['childOrderStrategies'][0]
+            elif order_info['childOrderStrategies'][1]['status'] == "FILLED":
+                order_info = order_info['childOrderStrategies'][1]
+            sold_unts = order_info['orderLegCollection'][0]['quantity']
 
         if 'price' in order_info.keys():
             stc_price = order_info['price']
         elif 'stopPrice' in order_info.keys():
             stc_price = order_info['stopPrice']
-        elif "orderActivityCollection" in order_info.keys():
-            prics = []
-            for ind in order_info["orderActivityCollection"]:
-                prics.append([ind['quantity'], ind['executionLegs'][0]['price']])
-                n_tot= sum([i[0] for i in prics])
-            stc_price =  sum([i[0]*i[1] for i in prics])/ n_tot
-
+        
         bto_price = self.portfolio.loc[open_trade, "Price"]
-        bto_price_alert = self.portfolio.loc[open_trade, "Price-Alert"]
-        bto_price_current = self.portfolio.loc[open_trade, "Price-Current"]
-        stc_PnL = float((stc_price - bto_price)/bto_price) *100
+        bto_price_alert = self.portfolio.loc[open_trade, "Price-alert"]
+        bto_price_actual = self.portfolio.loc[open_trade, "Price-actual"]
+        
+        if self.portfolio.loc[open_trade, "Type"] == "BTO":
+            stc_PnL = float((stc_price - bto_price)/bto_price) *100
+        elif self.portfolio.loc[open_trade, "Type"] == "STO":
+            stc_PnL = float((bto_price - stc_price)/bto_price) *100
 
-        xQty = sold_unts/ self.portfolio.loc[open_trade, "uQty"]
+        xQty = sold_unts/ self.portfolio.loc[open_trade, "Qty"]
 
         date = order_info["closeTime"]
         #Log portfolio
         self.portfolio.loc[open_trade, STC + "-Status"] = order_status
         self.portfolio.loc[open_trade, STC + "-Price"] = stc_price
         self.portfolio.loc[open_trade, STC + "-Date"] = date
         self.portfolio.loc[open_trade, STC + "-xQty"] = xQty
-        self.portfolio.loc[open_trade, STC + "-uQty"] = sold_unts
+        self.portfolio.loc[open_trade, STC + "-Qty"] = sold_unts
         self.portfolio.loc[open_trade, STC + "-PnL"] = stc_PnL
         self.portfolio.loc[open_trade, STC + "-ordID"] = order_id
 
         trade = self.portfolio.loc[open_trade]
-        sold_tot = np.nansum([trade[f"STC{i}-uQty"] for i in range(1,4)])
-        stc_PnL_all = np.nansum([trade[f"STC{i}-PnL"]*trade[f"STC{i}-uQty"] for i in range(1,4)])/sold_tot
+        sold_tot = np.nansum([trade[f"STC{i}-Qty"] for i in range(1,4)])
+        stc_PnL_all = np.nansum([trade[f"STC{i}-PnL"]*trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
         self.portfolio.loc[open_trade, "PnL"] = stc_PnL_all
-        stc_PnL_all_alert =  np.nansum([(float((trade[f"STC{i}-Price-Alerted"] - bto_price_alert)/bto_price_alert) *100) * trade[f"STC{i}-uQty"] for i in range(1,4)])/sold_tot
-        stc_PnL_all_curr = np.nansum([(float((trade[f"STC{i}-Price-Current"] - bto_price_current)/bto_price_current) *100) * trade[f"STC{i}-uQty"] for i in range(1,4)])/sold_tot
-        self.portfolio.loc[open_trade, "PnL-Alert"] = stc_PnL_all_alert
-        self.portfolio.loc[open_trade, "PnL-Current"] = stc_PnL_all_curr
+    
+        if self.portfolio.loc[open_trade, "Type"] == "BTO":
+            stc_PnL_all_alert =  np.nansum([(float((trade[f"STC{i}-Price-alert"] - bto_price_alert)/bto_price_alert) *100) * trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
+            stc_PnL_all_curr = np.nansum([(float((trade[f"STC{i}-Price-actual"] - bto_price_actual)/bto_price_actual) *100) * trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
+        elif self.portfolio.loc[open_trade, "Type"] == "STO":
+            stc_PnL_all_alert =  np.nansum([(float((bto_price_alert - trade[f"STC{i}-Price-alert"])/bto_price_alert) *100) * trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
+            stc_PnL_all_curr = np.nansum([(float((bto_price_actual - trade[f"STC{i}-Price-actual"])/bto_price_actual) *100) * trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
+
+        self.portfolio.loc[open_trade, "PnL-alert"] = stc_PnL_all_alert
+        self.portfolio.loc[open_trade, "PnL-actual"] = stc_PnL_all_curr
         
         mutipl = 1 if trade['Asset'] == "option" else .01  # pnl already in %
-        self.portfolio.loc[open_trade, "$PnL"] =  stc_PnL_all* bto_price *mutipl*sold_tot
-        self.portfolio.loc[open_trade, "$PnL-Alert"] =  stc_PnL_all_alert* bto_price_alert *mutipl*sold_tot
-        self.portfolio.loc[open_trade, "$PnL-Current"] =  stc_PnL_all_curr* bto_price_current *mutipl*sold_tot
-        
-        
+
+        self.portfolio.loc[open_trade, "PnL$"] =  stc_PnL_all* bto_price *mutipl*sold_tot
+        self.portfolio.loc[open_trade, "PnL$-alert"] =  stc_PnL_all_alert* bto_price_alert *mutipl*sold_tot
+        self.portfolio.loc[open_trade, "PnL$-actual"] =  stc_PnL_all_curr* bto_price_actual *mutipl*sold_tot
+
         symb = self.portfolio.loc[open_trade, 'Symbol']
 
-        sold_Qty =  self.portfolio.loc[open_trade, [f"STC{i}-uQty" for i in range(1,4)]].sum()
+        sold_Qty =  self.portfolio.loc[open_trade, [f"STC{i}-Qty" for i in range(1,4)]].sum()
 
         str_STC = f"{STC} {symb} @{stc_price} Qty:" + \
             f"{sold_unts}({int(xQty*100)}%), for {stc_PnL:.2f}%"
 
-        if sold_Qty == self.portfolio.loc[open_trade, "uQty"]:
+        if sold_Qty == self.portfolio.loc[open_trade, "Qty"]:
             str_STC += " (Closed)"
             self.portfolio.loc[open_trade, "isOpen"] = 0
 
         print (Back.GREEN + f"Filled: {str_STC}")
         self.queue_prints.put([f"Filled: {str_STC}","", "green"])
         self.save_logs()
 
 
-    def update_orders(self):
+    def exit_percent_to_price(self, open_trade):
+        trade = self.portfolio.loc[open_trade]
+        if trade["BTO-Status"] not in ["FILLED", "EXECUTED"]:
+            return
+        
+        price = trade["Price"]
+        exit_plan = eval(self.portfolio.loc[open_trade, "exit_plan"])
+        exit_plan_o = exit_plan.copy()
 
+        for exit in ["PT1", "PT2", "PT3"]:
+            if exit_plan[exit] is None or not isinstance(exit_plan[exit], str)  or "%" not in exit_plan[exit]:
+                continue
+            
+            if "TS" in exit_plan[exit]: 
+                pt,ts = exit_plan[exit].split("TS")
+                if "%" in pt:  # format val%TSval%
+                    if trade["Type"] == "STO":
+                        print("\033[91mWARNING: TrailingStop in buy to close. Why? \033[0m")
+                        if "%" in pt:
+                            ptv = round(price * (1 - float(pt.replace("%", ""))/100),2)
+                    else:
+                        ptv = round(price * (1 + float(pt.replace("%", ""))/100),2)
+                else: # format valTSval%
+                    ptv = float(pt)
+                if "%" in ts: # format TSval%
+                    ts =  round(price * (float(ts.replace("%", ""))/100) ,2)
+                else: # format TSval
+                    ts = float(ts)
+                exit_plan[exit] = f"{ptv}TS{ts}"
+            else: # format val%                
+                if "%" in exit_plan[exit]:
+                    if trade["Type"] == "STO":
+                        ptv = round(price * (1 - float(exit_plan[exit].replace("%", ""))/100),2)
+                    else:
+                        ptv = round(price * (1 + float(exit_plan[exit].replace("%", ""))/100),2)
+                else:
+                    ptv = float(exit_plan[exit])
+                exit_plan[exit] = ptv
+        
+        sl = exit_plan["SL"]
+        if sl is not None and isinstance(sl, str) and "%" in sl:
+            if "TS" in sl:  # format TSval%
+                sl = round(price * (float(sl.replace("%", "").replace("TS", ""))/100),2)
+                exit_plan["SL"] = f"TS{sl}"
+            else: # format val%
+                if trade["Type"] == "STO":
+                    exit_plan["SL"] = round(price * (1 + float(sl.replace("%", ""))/100),2)
+                else:
+                    exit_plan["SL"] = round(price * (1 - float(sl.replace("%", ""))/100),2)
+                
+        self.portfolio.loc[open_trade, "exit_plan"] = str(exit_plan)
+        
+        if exit_plan_o != exit_plan:
+            str_msg = f"Updated exits for from % to value, from:{exit_plan_o}, to:{exit_plan}"
+            print(Back.GREEN + str_msg)
+            self.queue_prints.put([str_msg, "", "green"])
+
+
+    def update_orders(self):
         for i in range(len(self.portfolio)):
             self.close_expired(i)
             trade = self.portfolio.iloc[i]
             redo_orders = False
 
             if trade["isOpen"] == 0:
                 continue
 
-            if trade["BTO-Status"]  in ["QUEUED", "WORKING", 'OPEN']:
-                _, order_info = self.get_order_info(trade['ordID'])
+            if trade["BTO-Status"]  in ["QUEUED", "WORKING", 'OPEN', 'AWAITING_CONDITION', 'AWAITING_MANUAL_REVIEW']:
+                order_status, order_info = self.get_order_info(trade['ordID'])
 
                 # Check if number filled Qty changed
                 qty_fill = order_info['filledQuantity']
                 qty_fill_old = self.portfolio.loc[i, "filledQty"]
                 # If so, redo orders
                 if not (pd.isnull(qty_fill_old) or qty_fill_old == 0) and \
                     qty_fill_old != qty_fill:
                     redo_orders = True
-
+                
+                if order_status in ["FILLED", "EXECUTED"]:
+                    price = order_info.get("price")
+                    self.portfolio.loc[i, "Price"] = price
+                    self.disc_notifier(order_info)
+                    str_msg = f"BTO {order_info['orderLegCollection'][0]['instrument']['symbol']} executed @ {price}. Status: {order_status}"
+                    print(Back.GREEN + str_msg)
+                    self.queue_prints.put([str_msg, "", "green"])
+                    
+                    # Add default short exits, once filled and price is known
+                    if self.portfolio.loc[i, "Type"] == "STO":
+                        exit_plan = eval(self.portfolio.loc[i,"exit_plan"])
+                        if len(self.cfg['shorting']['BTC_PT']) and exit_plan.get("PT1") is None:
+                            exit_plan['PT1'] = round(price * (1 - float(self.cfg['shorting']['BTC_PT'])/100),2)
+                        if len(self.cfg['shorting']['BTC_SL']) and exit_plan.get("SL") is None:
+                            exit_plan['SL'] = round(price * (1 + float(self.cfg['shorting']['BTC_SL'])/100),2)
+                        self.portfolio.loc[i,"exit_plan"]= str(exit_plan)
+                    
+                    # Update exits from % to value
+                    self.portfolio.loc[i, "BTO-Status"] = order_info['status']
+                    self.exit_percent_to_price(i)
+                
                 self.portfolio.loc[i, "filledQty"] = order_info['filledQuantity']
                 self.portfolio.loc[i, "BTO-Status"] = order_info['status']
+
                 trade = self.portfolio.iloc[i]
                 self.save_logs("port")
 
             if pd.isnull(trade["filledQty"]) or trade["filledQty"] == 0:
                 continue
 
             if trade.get("BTO-avg-Status") in ["QUEUED", "WORKING", 'OPEN']:
                 ordID = trade['ordID'].split(",")[-1]
-                _, order_info = self.get_order_info(ordID)
-                if order_info['status'] == 'FILLED' :
+                order_status, order_info = self.get_order_info(ordID)
+                if order_info['status'] in ["FILLED", "EXECUTED"]:
                     self.portfolio.loc[i, "BTO-avg-Status"] = order_info['status']
                     self.portfolio.loc[i, "filledQty"] += order_info['filledQuantity']
                     redo_orders = True
                     trade = self.portfolio.iloc[i]
                     self.save_logs("port")
+                    
+                    str_msg = f"BTO-avg {order_info['orderLegCollection'][0]['instrument']['symbol']} executed @ {order_info['price']}. Status: {order_status}"
+                    print(Back.GREEN + str_msg)
+                    self.queue_prints.put([str_msg, "", "green"])
+                    self.disc_notifier(order_info)
+                    
+                    # Update exits from % to value
+                    self.exit_percent_to_price(i)
+
+            # For short positions if closed end of day           
+            if trade['Type'] == 'STO' and self.cfg['shorting'].getboolean("BTC_EOD"):
+                time_now = datetime.now().time()
+                time_closed = datetime.strptime(self.cfg['general']["off_hours"].split(",")[0], "%H")
+                time_quarter = time_closed - timedelta(minutes=15)
+                time_five = time_closed - timedelta(minutes=5)
+                # Change exits before 15 min to close
+                if time_now >= time_quarter.time() and time_now < time_five.time() and \
+                    len(self.cfg['shorting']['BTC_EOD_PT_SL']):
+                        exit_plan = eval(trade["exit_plan"])                        
+                        PT, SL = self.cfg['shorting']['BTC_EOD_PT_SL'].split(",")
+                        SL, PT = eval(SL)/100, eval(PT)/100
+                        
+                        # check if not already updated, assume 5-10% exits are the updated 
+                        # percentage_difference = round(abs(exit_plan['SL'] - exit_plan['PT1']) / exit_plan['PT1'], 2)
+                        # if abs(percentage_difference - (SL+PT)) <= 0.03:  # accept 3% rounding error
+                        if self.EOD.get(trade["Symbol"]) is not "15min":
+                            quote = self.price_now(trade["Symbol"], "BTC", 1)
+                            exit_plan = {
+                                "PT1": round(quote - PT * quote, 2),
+                                "PT2": None,
+                                "PT3": None,
+                                "SL": round(quote + SL * quote, 2)
+                                }
+                            self.portfolio.at[i,'exit_plan'] = str(exit_plan)
+                            redo_orders = True                            
+                            str_msg = f'updating exits option {trade["Symbol"]} 15 min before EOD with {SL*100}% SL and {PT*100}% PT'
+                            print(Back.GREEN + str_msg)
+                            self.queue_prints.put([str_msg, "", "green"])
+                            self.exit_percent_to_price(i)
+                            self.EOD[trade["Symbol"]] = "15min"
+                # Close position 5 min to close
+                elif time_now >= time_five.time() and time_now < time_closed.time() \
+                    and self.EOD.get(trade["Symbol"]) is not "5min":
+                    print(f'closing option {trade["Symbol"]} 5 min before EOD')
+                    quote = self.price_now(trade["Symbol"], "BTC", 1)
+                    
+                    # Close and send lim order
+                    self.close_open_exit_orders(i)       
+                    order = {}
+                    order['action'] = "BTC"
+                    order['Symbol'] = trade["Symbol"]
+                    qty_sold = np.nansum([trade[f"STC{i}-Qty"] for i in range(1,4)])
+                    order['Qty'] =  int(trade["filledQty"]) - qty_sold
+                    order['price'] = quote
+                    self.update_paused = True
+                    _, order_id, order, _ = self.confirm_and_send(order, 'pars', self.bksession.make_STC_lim)
+                    self.update_paused = False
+                    
+                    # add order id
+                    for i in range(1,4):
+                        STC = f"STC{i}"
+                        if pd.isnull(trade[STC+"-ordID"]):
+                            break
+                    self.portfolio.loc[i, STC + "-ordID"] =  order_id
+                    self.EOD[trade["Symbol"]] = "5min"
 
             if redo_orders:
                 self.close_open_exit_orders(i)
-
+            self.exit_percent_to_price(i)
+            trade = self.portfolio.iloc[i]
             exit_plan = eval(trade["exit_plan"])
-            if  exit_plan != {}:                
-                if any([isinstance(e, str) and "%" not in e for e in exit_plan.values()]) and trade['Asset'] == 'option':
+            if exit_plan != {}:                
+                if all([isinstance(e, str) and ("%" not in e and "TS" not in e) for e in exit_plan.values()]) and trade['Asset'] == 'option':
                     self.check_opt_stock_price(i, exit_plan, "STC")
                 else:
                     self.make_exit_orders(i, exit_plan)
+                self.exit_percent_to_price(i)
 
             # Go over STC orders and check status
             for ii in range(1, 4):
                 STC = f"STC{ii}"
                 trade = self.portfolio.iloc[i]
                 STC_ordID = trade[STC+"-ordID"]
 
                 if pd.isnull(STC_ordID):
                     continue
 
                 # Get status exit orders
-                STC_ordID = int(float(STC_ordID))  # Might be read as a float
+                if isinstance(STC_ordID, str) and STC_ordID.isdigit():
+                    STC_ordID = int(float(STC_ordID))  # Might be read as a float
 
-                order_status, _ =  self.get_order_info(STC_ordID)
+                order_status, order_info =  self.get_order_info(STC_ordID)
 
                 if order_status == 'CANCELED':
-                    # Try next order number. probably went through. This is for TDA OCO
-                    order_status, _ =  self.get_order_info(STC_ordID + 1)
+                    # Try next order number. OCO gets chancelled when one of child ordergets filled.
+                    # This is for TDA OCO
+                    order_status, order_info =  self.get_order_info(STC_ordID + 1)
                     if order_status == 'FILLED':
                         STC_ordID = STC_ordID + 1
                         self.portfolio.loc[i, STC + "-ordID"] =  STC_ordID
+                    else: # try the other one
+                        order_status, order_info =  self.get_order_info(STC_ordID + 2)
+                        if order_status == 'FILLED':
+                            STC_ordID = STC_ordID + 2
+                            self.portfolio.loc[i, STC + "-ordID"] =  STC_ordID
 
                 self.portfolio.loc[i, STC+"-Status"] = order_status
                 trade = self.portfolio.iloc[i]
 
                 if order_status in ["FILLED", "EXECUTED"] and np.isnan(trade[STC+"-xQty"]):
-                    self.log_filled_STC(STC_ordID, i, STC)
+                    self.log_filled_STC(STC_ordID, i, STC)                    
+                    self.disc_notifier(order_info)
 
         self.save_logs("port")
 
 
     def check_opt_stock_price(self, open_trade, exit_plan, act="STC"):
         "Option exits in stock price"
         i = open_trade
@@ -853,45 +1173,46 @@
             if v[:2] == "PT" and float(pt) <= quote:
                 exit_plan[v] = quote_opt
                 # Add another exit plan for x2
                 STCn = int(v[2])
                 if STCn < 3 and exit_plan[f"PT{STCn+1}"] is None:
                     exit_plan[f"PT{STCn+1}"] = quote_opt * 2
             elif v[:2] == "SL" and "%" not in pt and float(pt) >= quote:
-                 exit_plan[v] = quote
+                exit_plan[v] = quote
 
         if exit_plan_ori != exit_plan:
             self.portfolio.loc[i, "exit_plan"] = str(exit_plan)
             self.save_logs("port")
             self.make_exit_orders(i, exit_plan)
 
 
     def SL_below_market(self, order, new_SL_ratio=.95):
         SL = order.get("SL")
-        price_now = self.price_now(order["Symbol"], "STC", 1)
+        if order['action'] == 'STC':
+            price_now = self.price_now(order["Symbol"], "STC", 1)
 
-        if SL > price_now:
-            new_SL = round(price_now * new_SL_ratio, 2)
-            print(Back.RED + f"{order['Symbol']} SL below bid price, changed from {SL} to {new_SL}")
-            self.queue_prints.put([f"{order['Symbol']} SL below bid price, changed from {SL} to {new_SL}",
-                            "", "red"])
-            order["SL"] = new_SL
-        return order
+            if SL > price_now:
+                new_SL = round(price_now * new_SL_ratio, 2)
+                print(Back.RED + f"{order['Symbol']} SL below bid price, changed from {SL} to {new_SL}")
+                self.queue_prints.put([f"{order['Symbol']} SL below bid price, changed from {SL} to {new_SL}",
+                                "", "red"])
+                order["SL"] = new_SL
+            return order
 
 
     def make_exit_orders(self, open_trade, exit_plan):
         i = open_trade
         trade = self.portfolio.iloc[i]
 
-        # Calculate x/uQty:
-        uQty_bought = trade['filledQty']
+        # Calculate x/Qty:
+        Qty_bought = trade['filledQty']
         nPTs =  len([i for i in range(1,4) if exit_plan[f"PT{i}"] is not None])
         if nPTs != 0:
-            uQty = [round(uQty_bought/nPTs)]*nPTs
-            uQty[-1] = int(uQty_bought - sum(uQty[:-1]))
+            Qty = [round(Qty_bought/nPTs)]*nPTs
+            Qty[-1] = int(Qty_bought - sum(Qty[:-1]))
 
             xQty = [round(1/nPTs, 1)]*nPTs
             xQty[-1] = 1 - sum(xQty[:-1])
 
         # Go over exit plans and make orders
         order = {'Symbol': trade['Symbol']}
         for ii in range(1, nPTs+1):
@@ -902,175 +1223,230 @@
             if len(ord_inf) == 2:
                 opt_type = "C" if "C" in ord_inf[1] else "P"
                 strike = str(re.split('C|P', ord_inf[1])[1]) + opt_type
                 order['strike'] = strike
 
             STC_ordID = trade[STC+"-ordID"]
             if not pd.isnull(STC_ordID):
-                # Adjust if necessary uQty based on remaining shares
-                if nPTs < 2:
-                    continue
-                ord_stat, ord_inf = self.get_order_info(int(STC_ordID))
-                iord_qty = ord_inf.get('quantity')
-                if iord_qty is None:
-                    iord_qty = ord_inf['childOrderStrategies'][0]['quantity']
-                if uQty[ii - 1] != iord_qty:
-                    uQty[ii - 1] = int(iord_qty)
-                    uleft = uQty_bought - sum(uQty[:ii])
-                    if uleft == 0:
-                        break
-                    nPts = len(uQty) - ii
-                    if nPts !=0:
-                        uQty = uQty[:ii] + [round(uleft/nPts)]*nPts
-                        uQty[-1] = int(uQty_bought - sum(uQty[:-1]))
-                    else:
-                        uQty[-1] = int(uleft)
-                    xQty = [round(u/uQty_bought,1) for u in uQty]
+                # assume PT with trailing stop at lim has SL
+                if isinstance(exit_plan[f"PT{ii}"], str) and "TS" in exit_plan[f"PT{ii}"]:
+                    trigger = float(exit_plan[f"PT{ii}"].split("TS")[0])
+                    TS = eval(exit_plan[f"PT{ii}"].split("TS")[1])
+                    quote_opt = self.price_now(trade['Symbol'], "STC", 1)
+                    if quote_opt >= trigger:
+                        self.close_open_exit_orders(open_trade)
+                        ord_func = self.bksession.make_STC_SL_trailstop
+                        order = {'Symbol': trade['Symbol']}
+                        order = self.calculate_stoploss(order, trade, TS)                                            
+                        order['Qty'] = int(trade['Qty'])
+                        order['xQty'] = 1
+                        order['action'] = trade["Type"].replace("BTO", "STC").replace("STO", "BTC")
+                        
+                        _, STC_ordID = self.bksession.send_order(ord_func(**order))
+                        if order.get("price"):
+                            str_prt = f"{STC} {order['Symbol']} @{order['price']}(Qty:{order['Qty']}) sent during order update"
+                        else:
+                            str_prt = f"{STC} {order['Symbol']} TS @{order.get('trail_stop_const')} (Qty:{order['Qty']}) sent during order update"
+                        exit_plan[f"PT{ii}"] = TS
+                        self.portfolio.loc[i, 'exit_plan'] = str(exit_plan)
+                        print (Back.GREEN + str_prt)
+                        self.queue_prints.put([str_prt,"", "green"])
+                        self.portfolio.loc[i, STC+"-ordID"] = STC_ordID
+                        trade = self.portfolio.iloc[i]
+                        self.save_logs("port")
+                        
+                # Adjust if necessary Qty based on remaining shares
+                if nPTs > 1:
+                    ord_stat, ord_inf = self.get_order_info(int(STC_ordID))
+                    iord_qty = ord_inf.get('quantity')
+                    if iord_qty is None:
+                        iord_qty = ord_inf['childOrderStrategies'][0]['quantity']
+                    if Qty[ii - 1] != iord_qty:
+                        Qty[ii - 1] = int(iord_qty)
+                        uleft = Qty_bought - sum(Qty[:ii])
+                        if uleft == 0:
+                            break
+                        nPts = len(Qty) - ii
+                        if nPts !=0:
+                            Qty = Qty[:ii] + [round(uleft/nPts)]*nPts
+                            Qty[-1] = int(Qty_bought - sum(Qty[:-1]))
+                        else:
+                            Qty[-1] = int(uleft)
+                        xQty = [round(u/Qty_bought,1) for u in Qty]
 
             else:
                 SL = exit_plan["SL"]
                 # Check if exit prices are strings (stock price for option)
-                if isinstance(SL, str) and "%" not in SL: SL = None
+                if isinstance(SL, str) and "TS" not in SL: SL = None
                 if isinstance(exit_plan[f"PT{ii}"], str): exit_plan[f"PT{ii}"] = None
 
                 ord_func = None
                 # Lim and Sl OCO order
                 if exit_plan[f"PT{ii}"] is not None and SL is not None:
                     # Lim_SL order
                     ord_func = self.bksession.make_Lim_SL_order
                     order["PT"] = exit_plan[f"PT{ii}"]
                     order["SL"] = exit_plan["SL"]
-                    order['uQty'] = uQty[ii - 1]
+                    order['Qty'] = Qty[ii - 1]
                     order['xQty'] = xQty[ii - 1]
+                    order['action'] = trade["Type"].replace("STO", "BTC").replace("BTO", "STC")
 
                 # Lim order
                 elif exit_plan[f"PT{ii}"] is not None and SL is None:
                     ord_func = self.bksession.make_STC_lim
                     order["price"] = exit_plan[f"PT{ii}"]
-                    order['uQty'] = uQty[ii - 1]
+                    order['Qty'] = Qty[ii - 1]
                     order['xQty'] = xQty[ii - 1]
+                    order['action'] = trade["Type"].replace("STO", "BTC").replace("BTO", "STC")
 
                 # SL order
                 elif ii == 1 and SL is not None:
-                    if "%" in SL:
+                    if isinstance(SL, str) and "TS" in SL:
                         ord_func = self.bksession.make_STC_SL_trailstop
-                        order["trail_stop_percent"] = float(exit_plan["SL"].replace("%", ""))
+                        order = self.calculate_stoploss(order, trade, exit_plan["SL"])
                     else:
                         ord_func =self.bksession.make_STC_SL
-                        order["price"] = exit_plan["SL"]
+                        order["SL"] = exit_plan["SL"]
                     
-                    order['uQty'] = int(trade['uQty'])
+                    order['Qty'] = int(trade['Qty'])
                     order['xQty'] = 1
+                    order['action'] = trade["Type"].replace("STO", "BTC").replace("BTO", "STC")
 
                 elif ii > 1 and SL is not None:
                     break
 
                 else:
                     raise("Case not caught")
 
-                # Check that is below current price
-                if order.get("SL") is not None and "%" not in order.get("SL"):
-                    order = self.SL_below_market(order)
+                # Check that is below actual price
+                if trade["Type"] == "BTO":
+                    if order.get("SL") is not None and isinstance(order.get("SL"), (int, float)):
+                        order['action'] = trade["Type"].replace("STO", "BTC").replace("BTO", "STC")
+                        order = self.SL_below_market(order)
 
-                if ord_func is not None and order['uQty'] > 0:
+                if ord_func is not None and order['Qty'] > 0:
                     _, STC_ordID = self.bksession.send_order(ord_func(**order))
                     if order.get("price"):
-                        str_prt = f"{STC} {order['Symbol']} @{order['price']}(Qty:{order['uQty']}) sent during order update"
+                        str_prt = f"{STC} {order['Symbol']} @{order['price']}(Qty:{order['Qty']}) sent during order update"
                     else:
-                        str_prt = f"{STC} {order['Symbol']} @{order.get('PT')}/{order.get('SL')} (Qty:{order['uQty']}) sent during order update"
+                        str_prt = f"{STC} {order['Symbol']} @PT:{order.get('PT')}/SL:{order.get('SL')} (Qty:{order['Qty']}) sent during order update"
                     print (Back.GREEN + str_prt)
                     self.queue_prints.put([str_prt,"", "green"])
                     self.portfolio.loc[i, STC+"-ordID"] = STC_ordID
                     trade = self.portfolio.iloc[i]
                     self.save_logs("port")
                 else:
                     break
         # no PTs but trailing stop
-        if nPTs == 0 and exit_plan["SL"] is not None and "%" in exit_plan["SL"] and pd.isnull(trade["STC1-ordID"]):
-            order["trail_stop_percent"] = float(exit_plan["SL"].replace("%", ""))      
-            order['uQty'] = int(trade['uQty'])
+        if nPTs == 0 and exit_plan["SL"] is not None and "TS" in exit_plan["SL"] and pd.isnull(trade["STC1-ordID"]):            
+            order = self.calculate_stoploss(order, trade, exit_plan["SL"])
+            order['Qty'] = int(trade['Qty'])
             order['xQty'] = 1
+            order['action'] = trade["Type"].replace("STO", "BTC").replace("BTO", "STC")
             _, STC_ordID = self.bksession.send_order(self.bksession.make_STC_SL_trailstop(**order))
-            str_prt = f"STC1 {order['Symbol']} Trailing stop of {order['trail_stop_percent']}% sent during order update"            
+            str_prt = f"STC1 {order['Symbol']} Trailing stop of {exit_plan['SL']} constant $ sent during order update"            
             print(Back.GREEN + str_prt)
             self.queue_prints.put([str_prt,"", "green"])
             self.portfolio.loc[i, "STC1-ordID"] = STC_ordID
             trade = self.portfolio.iloc[i]
             self.save_logs("port")
 
 
     def close_expired(self, open_trade):
         i = open_trade
         trade = self.portfolio.iloc[i]
         if trade["Asset"] != "option" or trade["isOpen"] == 0:
             return
         optdate = option_date(trade['Symbol'])
         if optdate.date() < date.today():
-            expdate = date.today().strftime("%Y-%m-%dT%H:%M:%S+0000")
-            usold = np.nansum([trade[f"STC{i}-uQty"] for i in range(1,4)])
+            expdate = date.today().strftime("%Y-%m-%d %H:%M:%S+0000")
+            usold = np.nansum([trade[f"STC{i}-Qty"] for i in range(1,4)])
+            STC =  f"STC3" # default to max stc
             for stci in range(1,4):
-                if pd.isnull(trade[f"STC{stci}-uQty"]):
+                if pd.isnull(trade[f"STC{stci}-Qty"]):
                     STC = f"STC{stci}"
                     break
 
             #Log portfolio
             self.portfolio.loc[open_trade, STC + "-Status"] = 'EXPIRED'
             self.portfolio.loc[open_trade, STC + "-Price"] = 0
             self.portfolio.loc[open_trade, STC + "-Date"] = expdate
             self.portfolio.loc[open_trade, STC + "-xQty"] = 1
-            self.portfolio.loc[open_trade, STC + "-uQty"] = trade['filledQty'] - usold
+            self.portfolio.loc[open_trade, STC + "-Qty"] = trade['filledQty'] - usold
             self.portfolio.loc[open_trade, STC + "-PnL"] = -100
             self.portfolio.loc[open_trade, "isOpen"] = 0
             
             bto_price = self.portfolio.loc[open_trade, "Price"]
-            bto_price_alert = self.portfolio.loc[open_trade, "Price-Alert"]
-            bto_price_current = self.portfolio.loc[open_trade, "Price-Current"]
+            bto_price_alert = self.portfolio.loc[open_trade, "Price-alert"]
+            bto_price_actual = self.portfolio.loc[open_trade, "Price-actual"]
             
             trade = self.portfolio.loc[open_trade]
-            sold_tot = np.nansum([trade[f"STC{i}-uQty"] for i in range(1,4)])
-            stc_PnL_all = np.nansum([trade[f"STC{i}-PnL"]*trade[f"STC{i}-uQty"] for i in range(1,4)])/sold_tot
+            sold_tot = np.nansum([trade[f"STC{i}-Qty"] for i in range(1,4)])
+            stc_PnL_all = np.nansum([trade[f"STC{i}-PnL"]*trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
             self.portfolio.loc[open_trade, "PnL"] = stc_PnL_all
-            stc_PnL_all_alert =  np.nansum([(float((trade[f"STC{i}-Price-Alerted"] - bto_price_alert)/bto_price_alert) *100) * trade[f"STC{i}-uQty"] for i in range(1,4)])/sold_tot
-            stc_PnL_all_curr = np.nansum([(float((trade[f"STC{i}-Price-Current"] - bto_price_current)/bto_price_current) *100) * trade[f"STC{i}-uQty"] for i in range(1,4)])/sold_tot
-            self.portfolio.loc[open_trade, "PnL-Alert"] = stc_PnL_all_alert
-            self.portfolio.loc[open_trade, "PnL-Current"] = stc_PnL_all_curr
+            stc_PnL_all_alert =  np.nansum([(float((trade[f"STC{i}-Price-alert"] - bto_price_alert)/bto_price_alert) *100) * trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
+            stc_PnL_all_curr = np.nansum([(float((trade[f"STC{i}-Price-actual"] - bto_price_actual)/bto_price_actual) *100) * trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
+            self.portfolio.loc[open_trade, "PnL-alert"] = stc_PnL_all_alert
+            self.portfolio.loc[open_trade, "PnL-actual"] = stc_PnL_all_curr
             
             mutipl = 1 if trade['Asset'] == "option" else .01  # pnl already in %
-            self.portfolio.loc[open_trade, "$PnL"] =  stc_PnL_all* bto_price *mutipl*sold_tot
-            self.portfolio.loc[open_trade, "$PnL-Alert"] =  stc_PnL_all_alert* bto_price_alert *mutipl*sold_tot
-            self.portfolio.loc[open_trade, "$PnL-Current"] =  stc_PnL_all_curr* bto_price_current *mutipl*sold_tot
+            self.portfolio.loc[open_trade, "PnL$"] =  stc_PnL_all* bto_price *mutipl*sold_tot
+            self.portfolio.loc[open_trade, "PnL$-alert"] =  stc_PnL_all_alert* bto_price_alert *mutipl*sold_tot
+            self.portfolio.loc[open_trade, "PnL$-actual"] =  stc_PnL_all_curr* bto_price_actual *mutipl*sold_tot
         
-            str_prt = f"{trade['Symbol']} option expired -100% uQty: {trade['filledQty']}"
+            str_prt = f"{trade['Symbol']} option expired -100% Qty: {trade['filledQty']}"
             print(Back.GREEN + str_prt)
             self.queue_prints.put([str_prt,"", "green"])
             self.save_logs("port")
 
+    def calculate_stoploss(self, order, trade, SL:str):
+        "Calculate stop loss price with increment, SL: e.g. '40%" 
+        if isinstance(SL, str):
+            if "%" in SL:       
+                SL =  trade['Price']*float(SL.replace("%", ""))/100
+            else:
+                SL = float(SL)
+
+        if self.bksession.name == 'tda':
+            increment = 0.01
+        elif trade['Symbol'] in ["SPY", "QQQ", "IWM"] and self.bksession.name == 'etrade':
+            increment = 0.01  # ETFs trade in penny increments
+        else:
+            if trade['Price'] < 3.0:
+                increment = 0.05
+            else:
+                increment = 0.10
+        rounded_stop_loss_price = round(SL / increment) * increment
+        order["trail_stop_const"] = rounded_stop_loss_price
+        return order
+        
 def option_date(opt_symbol):
     sym_inf = opt_symbol.split("_")[1]
     opt_date = re.split("C|P", sym_inf)[0]
     return datetime.strptime(opt_date, "%m%d%y")
 
 def amnt_left(order, position):
     # Calculate amnt to sell based on alerted left amount
-    available = position["uQty"]
+    available = position["Qty"]
     if order.get("amnt_left"):
         left = order["amnt_left"]
         if left == "few":
             order['xQty'] =  1 - .2
-            order['uQty'] = max(round(available * order['xQty']), 1)
+            order['Qty'] = max(round(available * order['xQty']), 1)
         elif left > .99:  # unit left
-            order['uQty'] = max(available - left, 1)
-            order['xQty'] = (available - order['uQty'])/available
+            order['Qty'] = max(available - left, 1)
+            order['xQty'] = (available - order['Qty'])/available
         elif left < .99:  # percentage left
             order['xQty'] = 1 - left
-            order['uQty'] = max(round(available * order['xQty']), 1)
+            order['Qty'] = max(round(available * order['xQty']), 1)
         else:
             raise ValueError
         return order, True
     else:
         return order, False
 
+
 if __name__ == "__main__":
     from DiscordAlertsTrader.brokerages import get_brokerage
     
     bksession = get_brokerage()
     at = AlertsTrader(bksession)
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/__init__.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,34 +41,44 @@
         #     prics = []
         #     for ind in order_info["orderActivityCollection"]:
         #         prics.append([ind['quantity'], ind['executionLegs'][0]['price']])
         #         n_tot= sum([i[0] for i in prics])
         #     stc_price =  sum([i[0]*i[1] for i in prics])/ n_tot
 
         # bto_price = self.portfolio.loc[open_trade, "Price"]
-        # bto_price_alert = self.portfolio.loc[open_trade, "Price-Alert"]
-        # bto_price_current = self.portfolio.loc[open_trade, "Price-Current"]
+        # bto_price_alert = self.portfolio.loc[open_trade, "Price-alert"]
+        # bto_price_actual = self.portfolio.loc[open_trade, "Price-actual"]
         # stc_PnL = float((stc_price - bto_price)/bto_price) *100
 
-        # xQty = sold_unts/ self.portfolio.loc[open_trade, "uQty"]
+        # xQty = sold_unts/ self.portfolio.loc[open_trade, "Qty"]
 
         # date = order_info["closeTime"]
         pass
 
 
 def get_brokerage(name=cfg['general']['BROKERAGE']):
     if name.lower() == 'tda':
         from .TDA_api import TDA
-        tda = TDA()
+        accountId = cfg['TDA']['accountId']
+        accountId = None if len(accountId) == 0 else accountId
+        tda = TDA(accountId=accountId)
         tda.get_session()
         return tda
-    elif name == "webull":
-        NotImplemented
+    elif name.lower() == "webull":
+        from .weBull_api import weBull
+        wb = weBull()
+        success = wb.get_session()
+        if success:
+            return wb
+        else:
+            raise Exception("Failed to get session for weBull")
     elif name.lower() == 'etrade':
         from .eTrade_api import eTrade
-        et = eTrade()
+        accountId = cfg['etrade']['accountId']
+        accountId = None if len(accountId) == 0 else accountId
+        et = eTrade(accountId=accountId)
         try:
             et.get_session()
         except Exception as e:
             print("Got error: \n", e, "\n Trying again...if it fails again, rerun the application.")
             et.get_session()
         return et
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/eTrade_api.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/eTrade_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,51 @@
 import pyetrade
 import re
 import random
 from datetime import datetime
 import time
 import json
 import os
+import functools
 
 from ..configurator import cfg
 from . import BaseBroker
 
+def retry_on_exception(retries=3, do_raise=False, fallback_method=None):
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            for attempt in range(1, retries+1):
+                try:
+                    return func(*args, **kwargs)
+                except Exception as e:
+                    print(f"Exception occurred: {e}. Retrying... (Attempt {attempt}/{retries})")
+            
+            # if fallback_method:
+            #     try:
+            #         fallback_method()
+            #         return func(*args, **kwargs)
+            #     except Exception as e:
+            #         print("Could not execute renew access method.", e)
+            if do_raise:
+                raise Exception(f"Method {func.__name__} failed after {retries} retries.")
+            else:
+                print(f"Method {func.__name__} failed after {retries} retries. Returning...")
+        return wrapper
+    return decorator
+
 class eTrade(BaseBroker):
     def __init__(self, account_n=0, accountId=None):
+        self.name = 'etrade'
         self.base_url = cfg["etrade"]["PROD_BASE_URL"]
         self.accountId = accountId
         self.account_n = account_n
         self.consumer_key = cfg["etrade"]["CONSUMER_KEY"]
         self.consumer_secret = cfg["etrade"]["CONSUMER_SECRET"]
+        self.token_fname = os.path.join(cfg['root']['dir'], "tokens.json")
         
     def get_session(self):
         """get token and sessions, will try several times and sleep for a second between each try"""
         for ix in range(5):
             try:
                 return self._get_session()
             except:
@@ -51,40 +77,48 @@
                 'resource_owner_key': self.tokens['oauth_token'],
                 'resource_owner_secret': self.tokens['oauth_token_secret'],
                 'dev': False
                 }
             self.account_session = pyetrade.ETradeAccounts(**kwargs)
             self.market_session = pyetrade.ETradeMarket(**kwargs)     
             self.order_session = pyetrade.ETradeOrder(**kwargs)
+            kwargs.pop('dev')
+            self.accessmanager = pyetrade.ETradeAccessManager(**kwargs)
+            self.accessmanager.renew_access_token()
             self._get_account()
             return True
         
         # if tokens saved try getting session
-        if os.path.exists("tokens.json"):
-            with open("tokens.json", "r") as f:
+        if os.path.exists(self.token_fname):
+            with open(self.token_fname, "r") as f:
                 self.tokens = json.load(f)   
             try:
                 return sessions()  
             except:
                 print("Loaded tokens expired, requesting new tokens")
-                os.remove("tokens.json")  
+                os.remove(self.token_fname)  
         
         # if tokens not valid, get new ones
         oauth = pyetrade.ETradeOAuth(self.consumer_key, self.consumer_secret)
         if cfg['etrade'].getboolean('WITH_BROWSER'):
             webbrowser.open(oauth.get_request_token())
         else:
             print("Please open the following URL in your browser:")
             print(oauth.get_request_token())
         verifier_code = input("Please accept agreement and enter verification code from browser: ")
         self.tokens = self._get_access_token(oauth, verifier_code)
-        with open("tokens.json", "w") as f:
+        with open(self.token_fname, "w") as f:
             json.dump(self.tokens, f)
         return sessions() 
 
+    def renew_access(self):
+        """Renews access token"""
+        self.accessmanager.renew_access_token()
+        
+    @retry_on_exception()
     def _get_account(self):
         """
         Calls account list API to retrieve a list of the user's E*TRADE accounts
         """
         data = self.account_session.list_accounts(resp_format='json')
         self.accounts_list = data["AccountListResponse"]["Accounts"]["Account"]        
         
@@ -92,37 +126,45 @@
             self.accountIdKey = [self.accounts_list[i]['accountIdKey'] for i in range(len(self.accounts_list)) 
                                  if self.accounts_list[i]['accountId'] == self.accountId][0]
         else:
             self.accountIdKey = self.accounts_list[self.account_n]['accountIdKey']
             self.accountId = self.accounts_list[self.account_n]['accountId']
         self.account = self.accounts_list[self.account_n]
 
+    @retry_on_exception()
     def get_account_info(self):
         """
         Call portfolio API to retrieve a list of positions held in the specified account
         """
-        data = self.account_session.get_account_balance(self.accountIdKey, resp_format='json')        
-        balance= {
-            'liquidationValue': data['BalanceResponse'].get("Computed").get("RealTimeValues").get("totalAccountValue"),
-            'cashBalance': data['BalanceResponse'].get("Computed").get('cashBalance'),
-            'availableFunds': data['BalanceResponse'].get("Computed").get('cashAvailableForInvestment'),
-            }
-
-        data = self.account_session.get_account_portfolio(self.accountIdKey, resp_format='json')
-                
+        data = self.account_session.get_account_balance(self.accountIdKey, resp_format='json') 
         acc_inf ={
             'securitiesAccount':{   
                 'positions':[],
                 'accountId' : self.accountId,
                 'currentBalances':{
-                    'liquidationValue': balance.get('liquidationValue'),
-                    'cashBalance': balance.get('cashBalance'),
-                    'availableFunds': balance.get('availableFunds'),
+                    'liquidationValue': data['BalanceResponse'].get("Computed").get("RealTimeValues").get("totalAccountValue"),
+                    'cashBalance': data['BalanceResponse'].get("Computed").get('cashBalance'),
+                    'availableFunds': data['BalanceResponse'].get("Computed").get('cashAvailableForInvestment'),
                     },
         }}
+        
+        # get orders and add them to acc_inf
+        orders = self.get_orders()
+        orders_inf =[]
+        for order in orders:
+            order_status = order['OrderDetail'][0]['status'].upper()
+            if order_status in ['CANCELLED', 'REJECTED', 'EXPIRED']:
+                continue
+            orders_inf.append(self.format_order(order))
+        acc_inf['securitiesAccount']['orderStrategies'] = orders_inf
+        
+        try:
+            data = self.account_session.get_account_portfolio(self.accountIdKey, resp_format='json')
+        except:
+            return acc_inf    
         # Handle and parse response
         if data is not None and "PortfolioResponse" in data and "AccountPortfolio" in data["PortfolioResponse"]:
             for acctPortfolio in data["PortfolioResponse"]["AccountPortfolio"]:
                 if acctPortfolio is not None and "Position" in acctPortfolio:
                     for position in acctPortfolio["Position"]:
                         assetType = position['Product']["securityType"].replace('EQ', 'stock').replace('OPTN', 'OPTION')
                         pos = {
@@ -137,28 +179,22 @@
                                            'assetType': assetType,
                                            }
                         }
                         acc_inf['securitiesAccount']['positions'].append(pos)
         else:
             print("No portfolio")
             
-        # get orders and add them to acc_inf
-        orders = self.get_orders()
-        orders_inf =[]
-        for order in orders:
-            order_status = order['OrderDetail'][0]['status'].upper()
-            if order_status in ['CANCELLED', 'REJECTED', 'EXPIRED']:
-                continue
-            orders_inf.append(self.format_order(order))
-        acc_inf['securitiesAccount']['orderStrategies'] = orders_inf
         return acc_inf
 
     def get_positions_orders(self):
-        acc_inf = self.get_account_info()
-
+        try:
+            acc_inf = self.get_account_info()
+        except:
+            print("Could not get account info")
+            return [], []
         df_pos = pd.DataFrame(columns=["symbol", "asset", "type", "Qty", "Avg Price", "PnL", "PnL %"])
 
         for pos in acc_inf['securitiesAccount']['positions']:
             long = True if pos["longQuantity"]>0 else False
 
             pos_inf = {
                 "symbol":pos["instrument"]["symbol"],
@@ -180,19 +216,22 @@
 
         exp = r"(\w+)_(\d{2})(\d{2})(\d{2})([CP])([\d.]+)"        
         match = re.search(exp, opt_ticker, re.IGNORECASE)
         if match:
             symbol, mnt, day, yer, type, strike = match.groups()
             if type.lower() == 'c':
                 type = 'Call'
+            else:
+                type = 'Put'
             converted_code = f"{symbol}:20{yer}:{mnt}:{day}:{type}:{strike}"
             return converted_code
         else:
             print('No format_option match for', opt_ticker)
 
+    @retry_on_exception()
     def get_quotes(self, symbol:list):
         """
         Calls quotes API to provide quote details for equities, options, and mutual funds
         """
         # reformat option tickers
 
         symbol = [self.format_option(i) if "_" in i else i for i in symbol ]
@@ -230,242 +269,227 @@
                             'quoteTimeInLong': quote.get("dateTimeUTC")*1000,
                             "status": quote['quoteStatus']
                             }
                         if resp[ticker]['status'].upper() == 'DELAYED':
                             print("\033[91mWARNING: QUOTES ARE DELAYED by 15 min, setup realtime quotes in etrade.com. Info in github README.md \033[0m")
         return resp
 
+    @retry_on_exception()
     def get_order_info(self, order_id): 
         """ Get order info from order_id, mimicks the order_info from TDA API"""
-        orders = self.order_session.list_orders(self.accountIdKey, resp_format='json')
-        
+        orders = self.order_session.list_orders(self.accountIdKey, resp_format='json')        
         for order in orders['OrdersResponse']['Order']:
             if order['orderId'] == order_id:
-                order_status = order['OrderDetail'][0]['status'].upper()
+                order_status = order['OrderDetail'][0]['status'].upper().replace('EXECUTED','FILLED').replace('OPEN','WORKING')
                 order_info = self.format_order(order)         
                 return order_status, order_info
         return None, None
 
     def format_order(self, order:dict):
         """ output format for order_response.Order, mimicks the order_info from TDA API"""
         stopPrice= order['OrderDetail'][0]['Instrument'][0].get('stopPrice')
         timestamp = int(order['OrderDetail'][0]['placedTime'])/1000
         enteredTime = datetime.fromtimestamp(timestamp).strftime("%Y-%m-%dT%H:%M:%S+00")
+        if 'executedTime' in order['OrderDetail'][0]:
+            timestamp = int(order['OrderDetail'][0]['executedTime'])/1000
+            closeTime = datetime.fromtimestamp(timestamp).strftime("%Y-%m-%dT%H:%M:%S+00")
+        else:
+            closeTime = enteredTime
+        status = order['OrderDetail'][0]['status'].upper().replace('EXECUTED','FILLED').replace('OPEN','WORKING')
         order_info = {
-            'status': order['OrderDetail'][0]['status'].upper(),
+            'status': status,
             'quantity': order['OrderDetail'][0]['Instrument'][0]['orderedQuantity'],
             'filledQuantity': order['OrderDetail'][0]['Instrument'][0]['filledQuantity'],
             'price':order['OrderDetail'][0]['Instrument'][0].get('averageExecutionPrice'),
             'orderStrategyType': 'SINGLE',
             "order_id" : order['orderId'],
             "orderId": order['orderId'],
             "stopPrice": stopPrice if stopPrice else None,
             'orderType':  order['OrderDetail'][0]['priceType'],
             'enteredTime': enteredTime,
+            "closeTime": closeTime,
             'orderLegCollection':[{
                 'instrument':{'symbol':order['OrderDetail'][0]['Instrument'][0]['Product']['symbol']},
-                'instruction': order['OrderDetail'][0]['Instrument'][0]['orderAction']
+                'instruction': order['OrderDetail'][0]['Instrument'][0]['orderAction'],
+                'quantity': order['OrderDetail'][0]['Instrument'][0]['filledQuantity'],
             }]             
         }    
         return order_info
 
+    @retry_on_exception()
     def send_order(self, new_order:dict):        
         order_response =  self.order_session.place_equity_order(
             resp_format="xml",
             accountId = self.accountId,
             accountIdKey = self.accountIdKey,
             **new_order)
         
         order_id = int(order_response['PlaceOrderResponse']['OrderIds']['orderId'])
         _, ord_inf = self.get_order_info(order_id)
         
         order_response['quantity'] =  int(order_response['PlaceOrderResponse']['Order']['Instrument']['quantity']),
         order_response.update(ord_inf) 
         return order_response, order_id
     
-    def cancel_order(self, order_id:int):        
-        return self.order_session.cancel_order(self.accountIdKey,order_id, resp_format='xml')
+    @retry_on_exception()
+    def cancel_order(self, order_id:int):
+        time.sleep(.5)  # sleep as order status change is not instant
+        resp = self.order_session.cancel_order(self.accountIdKey,order_id, resp_format='xml')
+        time.sleep(.5)
+        return resp
 
-    def make_BTO_lim_order(self, Symbol:str, uQty:int, price:float, **kwarg):
+    def make_BTO_lim_order(self, Symbol:str, Qty:int, price:float, action="BTO", **kwarg):
         "Buy with a limit order"
         kwargs = {}
         kwargs['symbol'] = Symbol
-        kwargs['orderAction'] = "BUY"
+        if action == "BTO":
+            kwargs['orderAction'] = "BUY"
+        elif action == "STO":
+            kwargs['orderAction'] = "SELL_SHORT"
         if len(Symbol.split("_"))>1:
             Symbol = self.format_option(Symbol)            
             symbol, year, month, day, optype, strike = Symbol.split(":")
             kwargs['symbol'] = symbol
             kwargs['expiryDate'] = f"{year}-{month}-{day}"
             kwargs['strikePrice'] = float(strike)
-            kwargs['callPut'] = "CALL" if optype.lower() == 'c' else 'PUT'
+            kwargs['callPut'] = optype
             kwargs["securityType"] = "OPTN"
-            kwargs['orderAction'] = 'BUY_OPEN'        
+            if action == "BTO":
+                kwargs['orderAction'] = 'BUY_OPEN'
+            elif action == "STO":
+                kwargs['orderAction'] = 'SELL_OPEN'
         kwargs['clientOrderId'] = str(random.randint(1000000000, 9999999999))
         kwargs['priceType'] = 'LIMIT'
         kwargs['limitPrice'] = price    
         kwargs['allOrNone'] = False
-        kwargs['quantity'] = uQty       
+        kwargs['quantity'] = Qty       
         kwargs['orderTerm'] = "GOOD_FOR_DAY"
         kwargs['marketSession'] = 'REGULAR'
         return kwargs
 
-    def make_Lim_SL_order(self, Symbol:str, uQty:int,  PT:float, SL:float,  **kwarg):
+    def make_Lim_SL_order(self, Symbol:str, Qty:int,  PT:float, SL:float, action="STC",  **kwarg):
         """Sell with a limit order and a stop loss order"""
         kwargs = {}
         kwargs['symbol'] = Symbol
-        kwargs['orderAction'] = "SELL"
+        if action == "STC":
+            kwargs['orderAction'] = "SELL"
+        elif action == "STO":
+            kwargs['orderAction'] = "BUY_TO_COVER"
         if len(Symbol.split("_"))>1:
             Symbol = self.format_option(Symbol)            
             symbol, year, month, day, optype, strike = Symbol.split(":")
             kwargs['symbol'] = symbol
             kwargs['expiryDate'] = f"{year}-{month}-{day}"
             kwargs['strikePrice'] = float(strike)
-            kwargs['callPut'] = "CALL" if optype.lower() == 'c' else 'PUT'
+            kwargs['callPut'] = optype
             kwargs["securityType"] = "OPTN"
-            kwargs['orderAction'] = 'SELL_CLOSE'
+            if action == "STC":
+                kwargs['orderAction'] = 'SELL_CLOSE'
+            elif action == "STO":
+                kwargs['orderAction'] = 'BUY_CLOSE'
         kwargs['clientOrderId'] = str(random.randint(1000000000, 9999999999))
         kwargs['priceType'] = 'STOP_LIMIT'
         kwargs['limitPrice'] = PT
         kwargs['stopPrice'] = SL
         kwargs['allOrNone'] = False
-        kwargs['quantity'] = uQty       
+        kwargs['quantity'] = Qty       
         kwargs['orderTerm'] = "GOOD_UNTIL_CANCEL"
         kwargs['marketSession'] = 'REGULAR'
         return kwargs
 
-    def make_STC_lim(self, Symbol:str, uQty:int, price:float, strike=None, **kwarg):
+    def make_STC_lim(self, Symbol:str, Qty:int, price:float, strike=None, action="STC", **kwarg):
         """Sell with a limit order and a stop loss order"""
         kwargs = {}
         kwargs['symbol'] = Symbol
-        kwargs['orderAction'] = "SELL"
+        if action == "STC":
+            kwargs['orderAction'] = "SELL"
+        elif action == "STO":
+            kwargs['orderAction'] = "BUY_TO_COVER"
         if len(Symbol.split("_"))>1:
             Symbol = self.format_option(Symbol)            
             symbol, year, month, day, optype, strike = Symbol.split(":")
             kwargs['symbol'] = symbol
             kwargs['expiryDate'] = f"{year}-{month}-{day}"
             kwargs['strikePrice'] = float(strike)
-            kwargs['callPut'] = "CALL" if optype.lower() == 'c' else 'PUT'
+            kwargs['callPut'] = optype
             kwargs["securityType"] = "OPTN"
-            kwargs['orderAction'] = 'SELL_CLOSE'
+            if action == "STC":
+                kwargs['orderAction'] = 'SELL_CLOSE'
+            elif action == "STO":
+                kwargs['orderAction'] = 'BUY_CLOSE'
         kwargs['clientOrderId'] = str(random.randint(1000000000, 9999999999))
         kwargs['priceType'] = 'LIMIT'
         kwargs['limitPrice'] = price
         kwargs['allOrNone'] = False
-        kwargs['quantity'] = uQty       
+        kwargs['quantity'] = Qty       
         kwargs['orderTerm'] = "GOOD_UNTIL_CANCEL"
         kwargs['marketSession'] = 'REGULAR'
         return kwargs
 
-    def make_STC_SL(self, Symbol:str, uQty:int, SL:float, **kwarg):
+    def make_STC_SL(self, Symbol:str, Qty:int, SL:float, action="STC", **kwarg):
         """Sell with a stop loss order"""
         kwargs = {}
         kwargs['symbol'] = Symbol
-        kwargs['orderAction'] = "SELL"
+        if action == "STC":
+            kwargs['orderAction'] = "SELL"
+        elif action == "STO":
+            kwargs['orderAction'] = "BUY_TO_COVER"
         if len(Symbol.split("_"))>1:
             Symbol = self.format_option(Symbol)            
             symbol, year, month, day, optype, strike = Symbol.split(":")
             kwargs['symbol'] = symbol
             kwargs['expiryDate'] = f"{year}-{month}-{day}"
             kwargs['strikePrice'] = float(strike)
-            kwargs['callPut'] = "CALL" if optype.lower() == 'c' else 'PUT'
+            kwargs['callPut'] = optype
             kwargs["securityType"] = "OPTN"
-            kwargs['orderAction'] = 'SELL_CLOSE'
+            if action == "STC":
+                kwargs['orderAction'] = 'SELL_CLOSE'
+            elif action == "STO":
+                kwargs['orderAction'] = 'BUY_CLOSE'
         kwargs['clientOrderId'] = str(random.randint(1000000000, 9999999999))
         kwargs['priceType'] = 'STOP'
-        kwargs['stopPrice'] = SL
+        kwargs['stopPrice'] = int(SL)
         kwargs['allOrNone'] = False
-        kwargs['quantity'] = uQty       
+        kwargs['quantity'] = Qty       
         kwargs['orderTerm'] = "GOOD_UNTIL_CANCEL"
         kwargs['marketSession'] = 'REGULAR'
 
-    def make_STC_SL_trailstop(self, Symbol:str, uQty:int,  trail_stop_percent:float, **kwarg):
+    def make_STC_SL_trailstop(self, Symbol:str, Qty:int,  trail_stop_const:float, action="STC", **kwarg):
+        "trail_stop_const"
         kwargs = {}
         kwargs['symbol'] = Symbol
-        kwargs['orderAction'] = "SELL"
+        if action == "STC":
+            kwargs['orderAction'] = "SELL"
+        elif action == "STO":
+            kwargs['orderAction'] = "BUY_TO_COVER"
         if len(Symbol.split("_"))>1:
             Symbol = self.format_option(Symbol)            
             symbol, year, month, day, optype, strike = Symbol.split(":")
             kwargs['symbol'] = symbol
             kwargs['expiryDate'] = f"{year}-{month}-{day}"
             kwargs['strikePrice'] = float(strike)
-            kwargs['callPut'] = "CALL" if optype.lower() == 'c' else 'PUT'
+            kwargs['callPut'] = optype
             kwargs["securityType"] = "OPTN"
-            kwargs['orderAction'] = 'SELL_CLOSE'       
+            if action == "STC":
+                kwargs['orderAction'] = 'SELL_CLOSE'
+            elif action == "STO":
+                kwargs['orderAction'] = 'BUY_CLOSE'    
         kwargs['clientOrderId'] = str(random.randint(1000000000, 9999999999))
-        kwargs['priceType'] = 'TRAILING_STOP_PRCT'
-        kwargs['stopPrice'] = trail_stop_percent
+        kwargs['priceType'] = 'TRAILING_STOP_CNST'
+        kwargs['stopPrice'] = trail_stop_const
         kwargs['allOrNone'] = False
-        kwargs['quantity'] = uQty       
+        kwargs['quantity'] = Qty       
         kwargs['orderTerm'] = "GOOD_UNTIL_CANCEL"
         kwargs['marketSession'] = 'REGULAR'
         return kwargs
 
+    @retry_on_exception()
     def get_orders(self):
         orders = self.order_session.list_orders(self.accountIdKey, resp_format='json')
         orders = orders['OrdersResponse']['Order']
-        """   {'orderId': 3,
-    'details': 'https://api.etrade.com/v1/accounts/kx-cz1Rmn1w_MMgg2K7wCA/orders/3.json',
-    'orderType': 'EQ',
-    'OrderDetail': [{'placedTime': 1684804106634,
-      'executedTime': 1178021968,
-      'orderValue': 1.0098,
-      'status': 'CANCELLED',
-      'orderTerm': 'GOOD_UNTIL_CANCEL',
-      'priceType': 'TRAILING_STOP_PRCT',
-      'priceValue': 'Tsp * 1.01',
-      'limitPrice': 0,
-      'stopPrice': 0,
-      'offsetType': 'TRAILING_STOP_PRCT',
-      'offsetValue': 40,
-      'marketSession': 'REGULAR',
-      'bracketedLimitPrice': 0,
-      'initialStopPrice': 1.01,
-      'trailPrice': 0,
-      'triggerPrice': 0,
-      'allOrNone': False,
-      'netPrice': 0,
-      'netBid': 0,
-      'netAsk': 0,
-      'gcd': 0,
-      'ratio': '',
-      'Instrument': [{'symbolDescription': 'VERB TECHNOLOGY CO INC COM NEW',
-        'orderAction': 'SELL',
-        'quantityType': 'QUANTITY',
-        'orderedQuantity': 1,
-        'filledQuantity': 0.0,
-        'estimatedCommission': 0.0001,
-        'estimatedFees': 0.0,
-        'Product': {'symbol': 'VERB', 'securityType': 'EQ'}}]}]},
-   {'orderId': 2,
-    'details': 'https://api.etrade.com/v1/accounts/kx-cz1Rmn1w_MMgg2K7wCA/orders/2.json',
-    'orderType': 'EQ',
-    'OrderDetail': [{'placedTime': 1684414597753,
-      'executedTime': 1684416602677,
-      'orderValue': 1.75,
-      'status': 'EXECUTED',
-      'orderTerm': 'GOOD_FOR_DAY',
-      'priceType': 'MARKET',
-      'limitPrice': 0,
-      'stopPrice': 0,
-      'marketSession': 'REGULAR',
-      'allOrNone': False,
-      'netPrice': 0,
-      'netBid': 0,
-      'netAsk': 0,
-      'gcd': 0,
-      'ratio': '',
-      'Instrument': [{'symbolDescription': 'VERB TECHNOLOGY CO INC COM NEW',
-        'orderAction': 'BUY',
-        'quantityType': 'QUANTITY',
-        'orderedQuantity': 1,
-        'filledQuantity': 1.0,
-        'averageExecutionPrice': 1.76,
-        'estimatedCommission': 0.0,
-        'estimatedFees': 0.0,
-        'Product': {'symbol': 'VERB', 'securityType': 'EQ'}}]}]},"""
         return orders
 
 
 
 if 0:
     rt = eTrade()
     rt.get_session()
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/discord_bot.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/discord_bot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import os
 import time
 import pandas as pd
-from datetime import datetime, timezone
+from datetime import datetime, timezone, date
 import threading
 from colorama import Fore, init
 import discord # this is discord.py-self package not discord
 
 from .message_parser import parse_trade_alert
 from .configurator import cfg
 from .configurator import channel_ids
@@ -33,114 +33,158 @@
 
 
 class DiscordBot(discord.Client):
     def __init__(self, 
                  queue_prints=dummy_queue(maxsize=10), 
                  live_quotes=True, 
                  brokerage=None,
-                 tracker_portfolio_fname=cfg['portfolio_names']["tracker_portfolio_name"]):
+                 tracker_portfolio_fname=cfg['portfolio_names']["tracker_portfolio_name"],
+                 cfg = cfg):
         super().__init__()
         self.channel_IDS = channel_ids
         self.time_strf = "%Y-%m-%d %H:%M:%S.%f"
         self.queue_prints = queue_prints
         self.bksession = brokerage
         self.live_quotes = live_quotes
+        self.cfg = cfg
         if brokerage is not None:
-            self.trader = AlertsTrader(queue_prints=self.queue_prints, brokerage=brokerage)       
-        self.tracker = AlertsTracker(brokerage=brokerage, portfolio_fname=tracker_portfolio_fname)
+            self.trader = AlertsTrader(queue_prints=self.queue_prints, brokerage=brokerage, cfg=self.cfg)       
+        self.tracker = AlertsTracker(brokerage=brokerage, portfolio_fname=tracker_portfolio_fname, cfg=self.cfg)
         self.load_data()        
 
-        if live_quotes and brokerage is not None:
+        if live_quotes and brokerage is not None and brokerage.name != 'webull':
             self.thread_liveq =  threading.Thread(target=self.track_live_quotes)
             self.thread_liveq.start()
 
     def close_bot(self):
         if self.bksession is not None:
             self.trader.update_portfolio = False
             self.live_quotes = False
 
     def track_live_quotes(self):
-        dir_quotes = cfg['general']['data_dir'] + '/live_quotes'
+        dir_quotes = self.cfg['general']['data_dir'] + '/live_quotes'
         os.makedirs(dir_quotes, exist_ok=True)
 
         while self.live_quotes:
             # Skip closed market
             now = datetime.now()
             weekday, hour = now.weekday(), now.hour
-            if  weekday >= 5 or (hour < 9 and hour >= 17):  
+            after_hr, before_hr = self.cfg['general']['off_hours'].split(",")
+            if  weekday >= 5 or (hour < int(before_hr) or hour >= int(after_hr)):  
                 time.sleep(60)
                 continue
 
-            # get unique symbols  from portfolios
-            track_symb = set(self.tracker.portfolio.loc[self.tracker.portfolio['isOpen']==1, 'Symbol'].to_list() + \
-                self.trader.portfolio.loc[self.trader.portfolio['isOpen']==1, 'Symbol'].to_list())
+            # get unique symbols  from portfolios, either options or all, open or alerted today
+            tk_day = pd.to_datetime(self.tracker.portfolio['Date']).dt.date == date.today()
+            td_day = pd.to_datetime(self.trader.portfolio['Date']).dt.date == date.today()
+            msk_tk = ((self.tracker.portfolio['isOpen']==1) | tk_day) 
+            msk_td = ((self.trader.portfolio['isOpen']==1) | td_day) 
+            
+            if self.cfg['general']['live_quotes_options_only']:
+                msk_tk = msk_tk & (self.tracker.portfolio['Asset']=='option')
+                msk_td = msk_td & (self.trader.portfolio['Asset']=='option')
+            
+            track_symb = set(self.tracker.portfolio.loc[msk_tk, 'Symbol'].to_list() + \
+                self.trader.portfolio.loc[msk_td, 'Symbol'].to_list())
             # save quotes to file
             try:
                 quote = self.bksession.get_quotes(track_symb)
             except Exception as e:
                 print('error during live quote:', e)
                 continue
+            if quote is None:
+                continue
             
             for q in quote: 
                 if quote[q]['description'] == 'Symbol not found':
                     continue
                 timestamp = quote[q]['quoteTimeInLong']//1000  # in ms
-                do_header = not os.path.exists(f"{dir_quotes}/{quote[q]['symbol']}.csv")
-                with open(f"{dir_quotes}/{quote[q]['symbol']}.csv", "a+") as f:
+
+                # Read the last line of the file and get the last recorded timestamp for the symbol
+                file_path = f"{dir_quotes}/{quote[q]['symbol']}.csv"
+                last_line = ""
+                do_header = True
+                if os.path.exists(file_path):
+                    do_header = False
+                    with open(file_path, "r") as f:
+                        lines = f.readlines()
+                        if lines:
+                            last_line = lines[-1].strip()
+                
+                #if last recorded timestamp is the same as current, skip
+                if last_line.split(",")[0] == str(timestamp):
+                    continue
+                
+                # Write the new line to the file
+                with open(file_path, "a+") as f:
                     if do_header:
                         f.write(f"timestamp, quote\n")
                     f.write(f"{timestamp}, {quote[q]['bidPrice']}\n")
             
             # Sleep for up to 5 secs    
             toc = (datetime.now() - now).total_seconds()
             if toc < 5 and self.live_quotes:
                 time.sleep(5-toc)
 
     def load_data(self):
         self.chn_hist= {}
         self.chn_hist_fname = {}
         for ch in self.channel_IDS.keys():
-            dt_fname = f"{cfg['general']['data_dir']}/{ch}_message_history.csv"
+            dt_fname = f"{self.cfg['general']['data_dir']}/{ch}_message_history.csv"
             if not os.path.exists(dt_fname):
-                ch_dt = pd.DataFrame(columns=cfg['col_names']['chan_hist'].split(","))
+                ch_dt = pd.DataFrame(columns=self.cfg['col_names']['chan_hist'].split(","))
                 ch_dt.to_csv(dt_fname, index=False)
-                ch_dt.to_csv(f"{cfg['general']['data_dir']}/{ch}_message_history_temp.csv", index=False)
+                ch_dt.to_csv(f"{self.cfg['general']['data_dir']}/{ch}_message_history_temp.csv", index=False)
             else:
                 ch_dt = pd.read_csv(dt_fname)
 
             self.chn_hist_fname[ch] = dt_fname
             self.chn_hist[ch]= ch_dt
 
     async def on_ready(self):
         print('Logged on as', self.user , '\n loading previous messages')
+        # pass channel object to trader
+        # if self.bksession is not None and self.cfg['discord'].getboolean('notify_alerts_to_discord') and \
+        #     len(cfg['discord'].get('send_alerts_to_chan')):
+            # self.trader.discord_channel = await self.fetch_channel(cfg['discord'].get('send_alerts_to_chan'))
+            # self.trader.discord_send = self.send_msg            
         await self.load_previous_msgs()
 
+    async def send_msg(self, msg, channel=None):
+        if channel is None:
+            # channel = await self.fetch_channel(cfg['discord'].get('send_alerts_to_chan'))
+            await channel.send(msg)
+    
     async def on_message(self, message):
         # handle fend bot messages
         if with_fend:
             alert = bot_msgs(message)
             if alert is not None:
                 self.new_msg_acts(alert, False)
                 return
-        # only respond to channels in config        
-        if message.channel.id not in self.channel_IDS.values():
+        # only respond to channels in config or authorwise subscription
+        author = f"{message.author.name}#{message.author.discriminator}"    
+        if message.channel.id not in self.channel_IDS.values() and \
+            author not in self.cfg['discord']['auhtorwise_subscription'].split(","):
+            # print(author, message.channel.name, message.channel.id, message.guild.name)
             return
         if message.content == 'ping':
             await message.channel.send('pong')
         if not len(message.content):
             return
         self.new_msg_acts(message)
+        
 
     async def on_message_edit(self, before, after):
         # Ignore if the message is not from a user or if the bot itself edited the message
         if after.channel.id not in self.channel_IDS.values() or  before.author.bot:
             return
 
         str_prt = f"Message edited by {before.author}: '{before.content}' -> '{after.content}'"
-        self.queue_prints.put([str_prt, "blue"])
+        self.queue_prints.put([str_prt, "black"])
         print(Fore.BLUE + str_prt)
 
     async def load_previous_msgs(self):
         await self.wait_until_ready()
         for ch, ch_id in self.channel_IDS.items():
             channel = self.get_channel(ch_id)
             if channel is None:
@@ -154,88 +198,141 @@
             else:
                 # iterator = channel.history(oldest_first=True)
                 continue
                 
             print("In", channel)
             async for message in iterator:
                 self.new_msg_acts(message)
-        print("Done")
+        print("Done")        
         self.tracker.close_expired()
 
     def new_msg_acts(self, message, from_disc=True):
         if from_disc:
             msg_date = message.created_at.replace(tzinfo=timezone.utc).astimezone(tz=None)
             msg_date_f = msg_date.strftime(self.time_strf)    
             if message.channel.id in self.channel_IDS.values():
                 chn_ix = list(self.channel_IDS.values()).index(message.channel.id)
                 chn = list(self.channel_IDS.keys())[chn_ix]
             else:
                 chn = None
             msg = pd.Series({'AuthorID': message.author.id,
-                            'Author': f"{message.author.name}#{message.author.discriminator}",
+                            'Author': f"{message.author.name}#{message.author.discriminator}".replace("#0", ""),
                             'Date': msg_date_f, 
                             'Content': message.content,
                             'Channel': chn
                             })
         else:
             msg = message
         chn = msg['Channel']
         shrt_date = datetime.strptime(msg["Date"], self.time_strf).strftime('%Y-%m-%d %H:%M:%S')
-        self.queue_prints.put([f"{shrt_date} \t {msg['Author']}: {msg['Content']} ", "blue"])
+        self.queue_prints.put([f"\n{shrt_date} {msg['Channel']}: \n\t{msg['Author']}: {msg['Content']} ", "blue"])
         print(Fore.BLUE + f"{shrt_date} \t {msg['Author']}: {msg['Content']} ")
 
         pars, order =  parse_trade_alert(msg['Content'])
         if pars is None:
             if self.chn_hist.get(chn) is not None:
                 msg['Parsed'] = ""
                 self.chn_hist[chn] = pd.concat([self.chn_hist[chn], msg.to_frame().transpose()],axis=0, ignore_index=True)
                 self.chn_hist[chn].to_csv(self.chn_hist_fname[chn], index=False)
             return
         else:
             if order['asset'] == "option":
-                # get option date with year
-                opt_dt = datetime.strptime(f"{order['expDate']} {datetime.now().year}" , "%m/%d %Y")
-                today = datetime.now().date()
-                past = opt_dt.date() < today
-                if past:
+                try:
+                    # get option date with year
+                    exp_dt = datetime.strptime(f"{order['expDate']}/{datetime.now().year}" , "%m/%d/%Y").date()
+                except ValueError:
+                    str_msg = f"Option date is wrong: {order['expDate']}"
+                    self.queue_prints.put([f"\t {str_msg}", "green"])
+                    print(Fore.GREEN + f"\t {str_msg}")
+                    msg['Parsed'] = str_msg
+                    if self.chn_hist.get(chn) is not None:
+                        self.chn_hist[chn] = pd.concat([self.chn_hist[chn], msg.to_frame().transpose()],axis=0, ignore_index=True)
+                        self.chn_hist[chn].to_csv(self.chn_hist_fname[chn], index=False)
+                    return
+                    
+                dt = datetime.now().date()
+                order['dte'] =  (exp_dt - dt).days
+                if order['dte']<0:
                     str_msg = f"Option date in the past: {order['expDate']}"
-                    self.queue_prints.put([f"\t \t {str_msg}", "green"])
-                    print(Fore.GREEN + f"\t \t {str_msg}")
+                    self.queue_prints.put([f"\t {str_msg}", "green"])
+                    print(Fore.GREEN + f"\t {str_msg}")
                     msg['Parsed'] = str_msg
                     if self.chn_hist.get(chn) is not None:
                         self.chn_hist[chn] = pd.concat([self.chn_hist[chn], msg.to_frame().transpose()],axis=0, ignore_index=True)
                         self.chn_hist[chn].to_csv(self.chn_hist_fname[chn], index=False)
                     return
-                
+
             order['Trader'], order["Date"] = msg['Author'], msg["Date"]
             order_date = datetime.strptime(order["Date"], "%Y-%m-%d %H:%M:%S.%f")
             date_diff = datetime.now() - order_date
             print(f"time difference is {date_diff.total_seconds()}")
 
             live_alert = True if date_diff.seconds < 90 else False
             str_msg = pars
-            if live_alert and self.bksession is not None: 
-                str_msg += " " + self.trader.price_now(order['Symbol'], order["action"], pflag=0)
-            self.queue_prints.put([f"\t \t {str_msg}", "green"])
-            print(Fore.GREEN + f"\t \t {str_msg}")
-            
-            track_out = self.tracker.trade_alert(order, live_alert, chn)
-            self.queue_prints.put([f"\t \t tracker log: {track_out}", "red"])
-            if msg['Author'] in cfg['discord']['authors_subscribed'] and  self.bksession is not None:
+            if live_alert and self.bksession is not None and (order.get('price') is not None):
+                quote = self.trader.price_now(order['Symbol'], order["action"], pflag=1)
+                act_diff = (order['price'] - quote)/ quote
+                # Check if actual price is too far (100) from alerted price
+                if (quote > 0) and abs(act_diff > 1) and order.get('action') == 'BTO':
+                    str_msg = f"Alerted price is {act_diff} times larger than current price of {quote}, skipping alert"
+                    self.queue_prints.put([f"\t {str_msg}", "green"])
+                    print(Fore.GREEN + f"\t {str_msg}")
+                    msg['Parsed'] = str_msg
+                    if self.chn_hist.get(chn) is not None:
+                        self.chn_hist[chn] = pd.concat([self.chn_hist[chn], msg.to_frame().transpose()],axis=0, ignore_index=True)
+                        self.chn_hist[chn].to_csv(self.chn_hist_fname[chn], index=False)
+                    return
+                
+                str_msg += f" Actual:{quote}, diff {round(act_diff*100)}%"
+            self.queue_prints.put([f"\t {str_msg}", "green"])
+            print(Fore.GREEN + f"\t {str_msg}")
+            #Tracker
+            if chn != "GUI_user":
+                track_out = self.tracker.trade_alert(order, live_alert, chn)
+                self.queue_prints.put([f"{track_out}", "red"])
+            # Trader
+            do_trade, order = self.do_trade_alert(msg['Author'], msg['Channel'], order)
+            if do_trade and date_diff.seconds < 120:
                 order["Trader"] = msg['Author']
-                if len(cfg["order_configs"]["default_trailstop"]):
-                    order['SL'] = cfg["order_configs"]["default_trailstop"] + "%"
                 self.trader.new_trade_alert(order, pars, msg['Content'])
         
         if self.chn_hist.get(chn) is not None:
             msg['Parsed'] = pars
             self.chn_hist[chn] = pd.concat([self.chn_hist[chn], msg.to_frame().transpose()],axis=0, ignore_index=True)
             self.chn_hist[chn].to_csv(self.chn_hist_fname[chn], index=False)
+    
+    def do_trade_alert(self, author, channel, order):
+        "Decide if alert should be traded"
+        if self.bksession is None or channel == "GUI_analysts":
+            return False, order
+        # in authors subs list
+        if author in self.cfg['discord']['authors_subscribed'].split(","):
+            return True, order
+        # in channel subs list
+        elif channel in self.cfg['discord']['channelwise_subscription'].split(","):
+            return True, order
+        # in authors shorting list
+        elif author in self.cfg['shorting']['authors_subscribed'].split(","):
+            if order['asset'] != "option":
+                return False, order
+            # BTC order sent manullay from gui
+            if order["action"] in ["BTC", "STO"] and channel in ["GUI_user", "GUI_both"]:
+                return True, order
+            # Make it shorting order
+            order["action"] = "STO" if order["action"] == "BTO" else "BTC" if order["action"] == "STC" else order["action"]
+            # reject if cfg do BTO or STC is false
+            if (order["action"] == "BTC" and not self.cfg['shorting'].getboolean('DO_BTC_TRADES')) \
+                or (order["action"] == "STO" and not self.cfg['shorting'].getboolean('DO_STO_TRADES')):
+                return False, order
+            if len(self.cfg['shorting']['max_dte']):
+                if order['dte'] <= int(self.cfg['shorting']['max_dte']):
+                    return True, order
+                
+        return False, order
 
-
-
+                
 if __name__ == '__main__':
     client = DiscordBot()
     client.run(cfg['discord']['discord_token'])
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/fend_bot.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/fend_bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from datetime import timezone
+from datetime import timezone, datetime
 import pandas as pd
 
 def bot_msgs(message):
     time_strf = "%Y-%m-%d %H:%M:%S.%f"
     # only respond to ch_id
     ch_id = 862187203711074317
     if message.channel.id == ch_id:
@@ -12,36 +12,49 @@
 
         try: cont = message.embeds[0].description
         except IndexError: 
             print("no embeddings", message.content)
             return
         
         # Get algo name as author        
-        algo_names = [('algo_1', ":black_joker: Scalp Opening :black_joker:"),
-        ('algo_2', ":spy: Scalp Opening :spy:"),
-        ('algo_3', ":man_mage: Scalp Opening :man_mage:")]
+        algo_names = [
+            ('algo_1', ":black_joker: Scalp Opening :black_joker:"),
+            ('algo_2', ":spy: Scalp Opening :spy:"),
+            ('algo_3', ":man_mage: Scalp Opening :man_mage:")
+            ]
         author = None
         for name, patt in algo_names:
             if patt in cont:
                 author = name
                 break
         if author is None:
             return
         
         # get alert info
         alert =  parse_alert(cont)
+        
+        # if Friday add exits and change name to subscribed
+        if msg_date.weekday() == 4 and datetime.now().weekday() == 4:
+            if author == 'algo_1':
+                author =  'algo_1F'
+                price = re.search(r"@ ([\d.]+)", alert).group(1)
+                qty =  max(int(500//(float(price)*100)), 1)
+                alert = alert.replace("BTO", f"BTO {qty}")
+                pt = round(float(price) * 2.25, 2)
+                sl = round(float(price) * .25, 2)
+                alert += f" PT: {pt}TS30 SL: {sl}"
+            
         msg = pd.Series({'AuthorID': message.author.id,
                         'Author': author,
                         'Date': msg_date_f, 
                         'Content': alert,
                         'Channel': "fend_bot"
                             })
         return msg
 
-
 def parse_alert(msg):
     id_exp = r"Eyeing:(\w+)_(\d+)_([\d\.]+)_(C|P)"
     match = re.search(id_exp, msg)
     if match is not None:
         symbol, expdate, strike, call_put = match.groups()
         current_mark = re.search(r"Current Mark:([\d.]+)", msg).group(1)
         alert_string = f"BTO {symbol} {strike}{call_put} {expdate[:2]}/{expdate[2:4]} @ {current_mark}"
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
 from DiscordAlertsTrader.brokerages import get_brokerage
 from DiscordAlertsTrader import gui_generator as gg
 from DiscordAlertsTrader import gui_layouts as gl
 from DiscordAlertsTrader.discord_bot import DiscordBot
 from DiscordAlertsTrader.configurator import cfg, channel_ids
 
+# A fix for Macs
+os.environ['QT_MAC_WANTS_LAYER'] = '1'
+
 def match_authors(author_str:str)->str:
     """Author have an identifier in discord, it will try to find full author name
 
     Parameters
     ----------
     author_str : str
         string to match the author
@@ -60,18 +63,18 @@
 # sg.theme('Dark Blue 3')
 sg.SetOptions(font=("Helvitica 10"))
                 # element_padding=(0, 0), margins=(1, 1))
 
 fnt_b = "Arial 10"
 fnt_h = "Arial 10"
 
-ly_cons, MLINE_KEY = gl.layout_console()
-
-def mprint(*args, **kwargs):
-    window[MLINE_KEY].print(*args, **kwargs)
+ly_cons, MLINE_KEY = gl.layout_console('Discord messages from all the channels',
+                                       '-MLINE-')
+ly_cons_subs, MLINE_SUBS_KEY = gl.layout_console('Discord messages only from subscribed authors',
+                                       '-MLINEsub-')
 
 print(1)
 gui_data = {}
 gui_data['port'] = gg.get_portf_data()
 ly_port = gl.layout_portfolio(gui_data['port'], fnt_b, fnt_h)
 
 gui_data['trades'] = gg.get_tracker_data()
@@ -92,31 +95,29 @@
     ly_ch = gl.layout_chan_msg(chn, gui_data[chn], fnt_b, fnt_h)
     ly_chns.append(ly_ch)
 
 bksession = get_brokerage()
 ly_accnt = gl.layout_account(bksession, fnt_b, fnt_h)
 
 layout = [[sg.TabGroup([
-                        [sg.Tab("Console", ly_cons, font=fnt_b)],
+                        [sg.Tab("Msgs Subs", ly_cons_subs, font=fnt_b)],
+                        [sg.Tab("Msgs All", ly_cons, font=fnt_b)], 
                         [sg.Tab('Portfolio', ly_port)],
-                        [sg.Tab('Analysts portfolio', ly_track)],
-                        [sg.Tab('Analysts stats', ly_stats)],
+                        [sg.Tab('Analysts Portfolio', ly_track)],
+                        [sg.Tab('Analysts Stats', ly_stats)],
                         [sg.Tab(c, h) for c, h in zip(chns, ly_chns)],                        
                         [sg.Tab("Account", ly_accnt)]
                         ], title_color='black')],
-          [sg.Input(default_text="Author#1234, STC 1 AAA 115C 05/30 @2.5 [click portfolio row number to prefill]",
-                    size= (110,1.5), key="-subm-msg",
-                    tooltip="Click portfolio row number to prefill the STC alert"),
-           sg.Button("Trigger alert", key="-subm-alert", tooltip="Will generate alert in portfolio and tracker", size= (20,1))]
+            gl.trigger_alerts_layout()
         ]
 print(3)
-window = sg.Window('Discord Alerts Trader for BullTrades', layout,size=(100, 800), # force_toplevel=True,
+window = sg.Window('Discord Alerts Trader', layout,size=(100, 800), # force_toplevel=True,
                     auto_size_text=True, resizable=True)
 print(4)
-def mprint_queue(queue_item_list):
+def mprint_queue(queue_item_list, subscribed_author=False):
     # queue_item_list = [string, text_color, background_color]
     kwargs = {}
     text = queue_item_list[0]
     len_que = len(queue_item_list)
     if len_que == 2:
         kwargs["text_color"] = queue_item_list[1]
     elif len_que == 3:
@@ -125,14 +126,16 @@
         kwargs["text_color"] = tcol
 
         bcol = queue_item_list[2]
         bcol = "white" if bcol == "" else bcol
         kwargs["background_color"] = bcol
 
     window[MLINE_KEY].print(text, **kwargs)
+    if subscribed_author or len_que == 3:
+        window[MLINE_SUBS_KEY].print(text, **kwargs)
 
 def update_portfolios_thread(window):
     while True:
         time.sleep(60)
         window["_upd-portfolio_"].click()
         time.sleep(2)  
         window["_upd-track_"].click()
@@ -152,15 +155,15 @@
     table.setSectionResizeMode(2, QHeaderView.Stretch)
     window[f"{chn}_table"].Widget.scrollToBottom()
 
 print(6)
 event, values = window.read(.1)
 print(7)
 trade_events = queue.Queue(maxsize=20)
-alistner = DiscordBot(trade_events, brokerage=bksession)
+alistner = DiscordBot(trade_events, brokerage=bksession, cfg=cfg)
 print(8)
 threading.Thread(target=update_portfolios_thread, args=(window,), daemon=True).start()
 print(9)
 event, values = window.read(.1)
 
 # exclusion filters for the portfolio and analysts tabs
 port_exc = {"Closed":False,
@@ -178,31 +181,53 @@
 print(10)
 dt, _  = gg.get_tracker_data(track_exc, **values)
 window.Element('_track_').Update(values=dt)
 fit_table_elms(window.Element("_track_").Widget)
 dt, hdr = gg.get_portf_data(port_exc)
 window.Element('_portfolio_').Update(values=dt)
 fit_table_elms(window.Element("_portfolio_").Widget)
-dt, hdr = gg.get_stats_data(port_exc)
+dt, hdr = gg.get_stats_data(stat_exc)
 window.Element('_stat_').Update(values=dt)
 fit_table_elms(window.Element("_stat_").Widget)
 
+
 def run_gui():  
-    while True:    
+    subs_auth_msg = False
+    auth_subs = cfg['discord']['authors_subscribed'].split(',')
+    auth_subs = [i.split("#")[0].strip() for i in auth_subs]
+    
+    while True: 
         event, values = window.read(1)#.1)
 
         if event == sg.WINDOW_CLOSED:
             break
-        if '_portfolio_' in event and values['_portfolio_'] != []:
-            pix = values['_portfolio_'][0]
-            dt, hdr = gg.get_portf_data(port_exc, **values)
+
+        # Prefill trigger alert message
+        if ('_portfolio_' in event and values['_portfolio_'] != []) or \
+            ('_track_' in event and values['_track_'] != []):  
+            if '_portfolio_' in event:
+                pix = values['_portfolio_'][0] 
+                dt, hdr = gg.get_portf_data(port_exc, **values)
+                qty = dt[pix][hdr.index('filledQty')]
+            else:
+                pix = values['_track_'][0]
+                dt, hdr = gg.get_tracker_data(track_exc, **values)
+                qty = dt[pix][hdr.index('Qty')]  
+            qty = qty if qty == "" else int(qty)            
             symb = dt[pix][hdr.index('Symbol')]
             auth = match_authors(dt[pix][hdr.index('Trader')])
-            qty = dt[pix][hdr.index('filledQty')]
-            price = dt[pix][hdr.index('1-$-Current')]
+            
+            price = ""
+            if "Live" in hdr:
+                price = dt[pix][hdr.index('Live')]
+            if price == "":
+                price = dt[pix][hdr.index('S-Price-actual')]
+            if price == "":
+                price = dt[pix][hdr.index('S-Price')]
+            price = price if price == "" else float(price)
             if "_" in symb:
                 # option
                 exp = r"(\w+)_(\d{6})([CP])([\d.]+)"        
                 match = re.search(exp, symb, re.IGNORECASE)
                 if match:
                     symbol, date, type, strike = match.groups()
                     symb_str = f"{auth}, STC {qty} {symbol} {strike}{type} {date[:2]}/{date[2:4]} @{price}"
@@ -265,20 +290,15 @@
             event, values = window.read(.1)
 
             args = {}
             for k, v in values.items():
                 if k[:len(chn)] == chn:
                     args[k[len(chn)+1:]] = v
             dt, _  = gg.get_hist_msgs(chan_name=chn, **args)
-            if args['n_rows'] != "":
-                n_rows = eval(args['n_rows'])
-                n_rows = max(1, n_rows)
-                window.Element(f"{chn}_table").Update(values=dt,  num_rows=n_rows)
-            else:
-                window.Element(f"{chn}_table").Update(values=dt)
+            window.Element(f"{chn}_table").Update(values=dt)
 
             fit_table_elms(window.Element(f"{chn}_table").Widget)
             window.Element(f'{chn}_UPD').Update(button_color=ori_col)
 
         elif event == 'acc_updt':
             ori_col = window.Element("acc_updt").ButtonColor
             window.Element("acc_updt").Update(button_color=("black", "white"))
@@ -288,48 +308,88 @@
             fit_table_elms(window.Element(f"_orders_").Widget)
             window.Element("acc_updt").Update(button_color=ori_col)
 
         elif event == "-subm-alert":
             ori_col = window.Element("-subm-alert").ButtonColor
             window.Element("-subm-alert").Update(button_color=("black", "white"))
             event, values = window.read(.1)
-            try:        
+            
+            #extra comas
+            if len(values['-subm-msg'].split(','))>2:
+                splt = values['-subm-msg'].split(',')
+                author = splt[0]
+                msg = ",".join(splt[1:])
+            # one coma
+            elif len(values['-subm-msg'].split(','))==2:
                 author, msg = values['-subm-msg'].split(',')
-            except ValueError:
+            # one colon
+            elif len(values['-subm-msg'].split(':'))==2:
                 author, msg = values['-subm-msg'].split(':')
+            # extra colons
+            elif len(values['-subm-msg'].split(':'))>2:
+                splt = values['-subm-msg'].split(':')
+                author = splt[0]
+                msg = ":".join(splt[1:])
+            # no colon or coma
+            else:
+                print("No colon or coma in message, author not found")
+                
             author = match_authors(author.strip())
-            msg = msg.strip()
+            # let pass no identifier if no match
+            author = author.replace("#No match, find author identifier#1234", "")
+            author = author.replace("#Multiple matches, find author identifier#1234", "")
+            msg = msg.strip().replace("SPXW", "SPX")
             date = datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f")
+            chan = "GUI_" + values["_chan_trigg_"]
+            print(chan)
             new_msg = pd.Series({
                 'AuthorID': None,
                 'Author': author,
                 'Date': date, 
                 'Content': msg,
-                'Channel': "GUI_input"
+                'Channel': chan
                 })
             alistner.new_msg_acts(new_msg, from_disc=False)
             window.Element("-subm-alert").Update(button_color=ori_col)
 
         try:
             event_feedb = trade_events.get(False)
-            mprint_queue(event_feedb)
+            # if message from subscribed author or channel flag it to print in both consoles
+            if event_feedb[1] == "blue":
+                if any(a in event_feedb[0] for a in auth_subs):
+                    subs_auth_msg = True
+                elif cfg['discord']['channelwise_subscription'].split(",") != [""] and \
+                    any([c in event_feedb[0] for c in cfg['discord']['channelwise_subscription'].split(",")]):
+                    subs_auth_msg = True
+                elif cfg['discord']['auhtorwise_subscription'].split(",") != [""] and \
+                    any([c in event_feedb[0] for c in cfg['discord']['auhtorwise_subscription'].split(",")]):
+                    subs_auth_msg = True
+                else:
+                    subs_auth_msg = False
+            
+            mprint_queue(event_feedb, subs_auth_msg)
         except queue.Empty:
             pass
 
 
-
 def run_client():
+    if len(cfg['discord']['discord_token']) < 50:
+        str_prt = "Discord token not provided, no discord messages will be received. Add user token in config.ini"
+        print(str_prt)
+        time.sleep(3)
+        trade_events.put([str_prt,"", "red"])
+        return
     alistner.run(cfg['discord']['discord_token'])
 
 
 def gui():   
-    client_thread = threading.Thread(target=run_client)
+    client_thread = threading.Thread(target=run_client, daemon=True)
 
     # start the threads
-    client_thread.start()
+    # client_thread.start()
     run_gui()
 
     # close the GUI window
     window.close()
     alistner.close_bot()
     exit()
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui_layouts.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui_layouts.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,33 +7,51 @@
 """
 
 import PySimpleGUIQt as sg
 from . import gui_generator as gg
 
 
 tip = "coma separed patterns, e.g. string1,string2"
+tlp_date = "Date can be:\n-a date mm/dd/yyyy, mm/dd\n-a period: today, yesterday, week, biweek, month, mtd, ytd"
 
-def layout_console():
-    MLINE_KEY = '-MLINE-__WRITE ONLY__'
-    layout = [[sg.Text('Real Time Discord Alert Trader', size=(50,1))],
-              [sg.Multiline(size=(1200,None), key=MLINE_KEY, autoscroll=True, enable_events=False),sg.Stretch()]]
-    return layout, MLINE_KEY
-
+def layout_console(ttl='Discord messages from subscribed channels', 
+                   key='-MLINE-__WRITE ONLY__'):
+    layout = [[sg.Text(ttl, size=(100,1))],
+              [sg.Multiline(size=(1200,None), key=key, autoscroll=True, enable_events=False),sg.Stretch()]]
+    return layout, key
+
+def trigger_alerts_layout():
+    tp_chan = "Select portfolios to trigger alert.\'nuser' for your portfolio only. Will bypass false do_BTO and do_BTC and make the trade \n" +\
+                "'analysts' for the alerts tracker,\n'all' for both"
+    tp_trig = "Click portfolio row number to prefill the STC alert. Alerts can look like\n" +\
+                "BTO: Author#1234, BTO 1 AAA 115C 05/30 @2.5 PT 3.5TS30% PT2 4 SL TS40%, '%' for percentage, TS for Trailing Stop\n" +\
+                "STC: Author#1234, STC 1 AAA 115C 05/30 @3\n" +\
+                "STO: Author#1234, STC 1 AAA 115C 05/30 @2.5 PT 40% SL 50% \n" +\
+                "BTC: Author#1234, STC 1 AAA 115C 05/30 @2 \n" +\
+                "Exit Update: Author#1234, exit update AAA 115C 05/30 PT 80% SL 2\n"
+    lay = [sg.Text('to portfolio:', tooltip=tp_chan, size=(15,1.2)),
+           sg.Combo(['both', 'user', 'analysts'], default_value='analysts', key="_chan_trigg_",tooltip=tp_chan, readonly=True, size=(15,1.2)),
+            sg.Input(default_text="Author#1234, STC 1 AAA 115C 05/30 @2.5 [click portfolio row number to prefill]",
+                    size= (100,1.3), key="-subm-msg",
+                    tooltip=tp_trig),
+           sg.Button("Trigger alert", key="-subm-alert", 
+                     tooltip="Will generate alert in user or/and analysts portfolio, useful to close or open a position", size= (20,1.2))]
+    return lay
 
 def layout_portfolio(data_n_headers, font_body, font_header):
     if data_n_headers[0] == []: 
         values = [""*21 ]
     else:
         values=data_n_headers[0]
     
     layout = [
          [sg.Column([[
             sg.Text('Include:  Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'port_filt_author',tooltip=tip),
-            sg.Text('Date from: '), sg.Input(key=f'port_filt_date_frm', size=(16, 1), default_text='05/10/2023'),
-            sg.Text(' To: '), sg.Input(key=f'port_filt_date_to', size=(16, 1)),
+            sg.Text('Date from: ', tooltip=tlp_date), sg.Input(key=f'port_filt_date_frm', size=(16, 1), default_text='week', tooltip=tlp_date),
+            sg.Text(' To: ', tooltip=tlp_date), sg.Input(key=f'port_filt_date_to', size=(16, 1), tooltip=tlp_date),
             sg.Text(' Symbols: ', tooltip=tip), sg.Input(key=f'port_filt_sym', tooltip=tip),
             sg.Text(' Channels: ',tooltip=tip), sg.Input(key=f'port_filt_chn',tooltip=tip)
             ],                                        
             [sg.Text("Exclude: |"),
             sg.Checkbox("Closed", key="-port-Closed", enable_events=True),
             sg.Checkbox("Open", key="-port-Open", enable_events=True),
             sg.Checkbox("Cancelled", key="-port-Cancelled", default=True, enable_events=True),
@@ -69,16 +87,17 @@
     else:
         values=data_n_headers[0]
     
     layout = [[
         sg.Column([
             [
             sg.Text('Include:  Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'track_filt_author',tooltip=tip),
-            sg.Text('Date from: '), sg.Input(key=f'track_filt_date_frm', default_text='05/10/2023', size=(16, 1)),
-            sg.Text(' To: '), sg.Input(key=f'track_filt_date_to', size=(16, 1)),
+            sg.Text('Date from: ', tooltip=tlp_date), 
+            sg.Input(key=f'track_filt_date_frm', default_text='week', size=(16, 1), tooltip=tlp_date),
+            sg.Text(' To: ', tooltip=tlp_date), sg.Input(key=f'track_filt_date_to', size=(16, 1), tooltip=tlp_date),
             sg.Text(' Symbols: ',tooltip=tip), sg.Input(key=f'track_filt_sym',tooltip=tip),
             sg.Text(' Channels: ',tooltip=tip), sg.Input(key=f'track_filt_chn',tooltip=tip)
             ],[ 
             sg.Text("Exclude: |"),
             sg.Checkbox("Closed", key="-track-Closed", enable_events=True),
             sg.Checkbox("Open", key="-track-Open", enable_events=True),
             sg.Checkbox("Neg PnL", key="-track-NegPnL", enable_events=True),
@@ -97,14 +116,15 @@
                 display_row_numbers=True,
                 auto_size_columns=True,
                 header_font=font_header,
                 text_color='black',
                 font=font_body,
                 justification='left',
                 alternating_row_color='grey',
+                enable_events=True,
                 # num_rows=30, #len(data_n_headers[0]),
                 key='_track_'), sg.Stretch()]])]
          ]
     return layout
 
 
 def layout_stats(data_n_headers, font_body, font_header):
@@ -112,32 +132,42 @@
     if data_n_headers[0] == []: 
         values = [""*21 ]
     else:
         values=data_n_headers[0]
     
     layout = [
         [sg.Column([[sg.Text('Include:  Authors: ', auto_size_text=True, tooltip=tip), sg.Input(key=f'stat_filt_author', tooltip=tip),
-                     sg.Text('Date from:'), sg.Input(key=f'stat_filt_date_frm', size=(16, 1), default_text='05/10/2023'),
-                     sg.Text(' To:', size=(5, 1)), sg.Input(key=f'stat_filt_date_to', size=(16, 1)),
+                     sg.Text('Date from:', tooltip=tlp_date), 
+                     sg.Input(key=f'stat_filt_date_frm', size=(16, 1), default_text='week', tooltip=tlp_date),
+                     sg.Text(' To:', size=(5, 1), tooltip=tlp_date), 
+                     sg.Input(key=f'stat_filt_date_to', size=(16, 1), tooltip=tlp_date),
                      sg.Text(' Symbols:'), sg.Input(key=f'stat_filt_sym', tooltip=tip),
                      sg.Text(' Max $:', tooltip="calculate stats limiting trades to max $"), 
-                     sg.Input(key=f'stat_max_trade_cap', tooltip="calculate stats limiting trades to max $"),
+                     sg.Input(key=f'stat_max_trade_val', tooltip="calculate stats limiting trades to max $ amount"),
                      sg.Text(' Max quantity:', tooltip="calculate stats limiting trades to max quantity"), 
                      sg.Input(key=f'stat_max_qty', tooltip="calculate stats limiting trades to max quantity"),
+                     sg.Text(' DTE: min', tooltip="Days To Expiration min"), 
+                     sg.Input(key=f'stat_dte_min', tooltip="Days To Expiration min"),
+                     sg.Text(' max', tooltip="Days To Expiration max"), 
+                     sg.Input(key=f'stat_dte_max', tooltip="Days To Expiration max"),
+                     
                      ],
                      [sg.Text("Exclude: "),
                       sg.Checkbox("Neg PnL", key="-stat-NegPnL", enable_events=True),
                       sg.Checkbox("Pos PnL", key="-stat-PosPnL", enable_events=True),                  
                       sg.Checkbox("Stocks", key="-stat-stocks", default=True, enable_events=True),
                       sg.Checkbox("Options", key="-stat-options", enable_events=True),
                       sg.Text('| Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'stat_exc_author', tooltip=tip),
                       sg.Text('Symbols: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'stat_exc_sym',tooltip=tip),
                       sg.Text('Channels: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'stat_exc_chn',tooltip=tip),
                       ],
-                     [sg.ReadButton("Update", button_color=('white', 'black'), key="_upd-stat_")]])
+                     [sg.ReadButton("Update", button_color=('white', 'black'), key="_upd-stat_")],
+                     [sg.Text("PnL-actual = PnL from prices at the moment of alerted trade (as opposed to the prices claimed in the alert) \n" + \
+                         "diff = difference between actual and alerted, high BTO and low STC diffs is bad, alerts are delayed"
+                         )]])
                     ],
          [sg.Column([[sg.Table(values=values,
                         headings=data_n_headers[1],
                         display_row_numbers=True,
                         auto_size_columns=True,
                         header_font=font_header,
                         text_color='black',
@@ -155,19 +185,19 @@
         values = [[""*len(data_n_headers[1])] ]
     else:
         values=data_n_headers[0]
 
     layout = [
         [sg.Text('Filter:  Authors: '), sg.Input(key=f'{chn}_filt_author'),
            # sg.Text(' '*2),
-         sg.Text('Date from: '), sg.Input(key=f'{chn}_filt_date_frm', default_text='05/09/23'),
-         sg.Text(' To: '), sg.Input(key=f'{chn}_filt_date_to'),
+         sg.Text('Date from: ', tooltip=tlp_date), 
+         sg.Input(key=f'{chn}_filt_date_frm', default_text='week', tooltip=tlp_date),
+         sg.Text(' To: ', tooltip=tlp_date), sg.Input(key=f'{chn}_filt_date_to', tooltip=tlp_date),
           # sg.Text(' '*1),
          sg.Text('Message contains: '), sg.Input(key=f'{chn}_filt_cont'),
-         sg.Text('Num. rows display: '), sg.Input(key=f'{chn}_n_rows'),
          ],
         [sg.ReadFormButton("Update", button_color=('white', 'black'), key=f'{chn}_UPD', bind_return_key=True)],
         [sg.Column([[sg.Table(values=values,
                   headings=data_n_headers[1],
                   justification='left',
                   display_row_numbers=False,
                   text_color='black',
@@ -202,14 +232,16 @@
 
 
 def layout_account(bksession, font_body, font_header):
     if bksession is None:
         return [[sg.T("No brokerage API provided in config.ini")]]
     acc_inf, ainf = gg.get_acc_bals(bksession)
     pos_tab, pos_headings = gg.get_pos(acc_inf)
+    if not len(pos_tab):
+        pos_tab = ["No post"]
     ord_tab, ord_headings, _= gg.get_orders(acc_inf)
 
     layout = [[sg.Column([
         [tt_acnt("Account ID:", font_body[1]), tt_acnt(ainf["id"], font_body[1], 0, 0, font_body[0]),
          tt_acnt("Balance:", font_body[1]), tt_acnt("$" + str(ainf["balance"]), font_body[1], 0, 0, font_body[0], k="acc_b"),
          tt_acnt("Cash:", font_body[1]), tt_acnt("$" + str(ainf["cash"]), font_body[1], 0, 0, font_body[0], k="acc_c"),
          tt_acnt("Funds:", font_body[1]), tt_acnt("$" + str(ainf["funds"]), font_body[1], 0, 0, font_body[0], k="acc_f")
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/message_parser.py` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/message_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 """
 import re
 import pandas as pd
 from datetime import datetime
 import numpy as np
 
 def parse_trade_alert(msg, asset=None):
-    pattern = r'\b(BTO|STC)\b\s*(\d+)?\s*([A-Z]+)\s*(\d+[.\d+]*[cp]?)?\s*(\d{1,2}\/\d{1,2})?(?:\/2023|\/23)?\s*@\s*[$]*[ ]*(\d+(?:[,.]\d+)?|\.\d+)'
+    pattern = r'\b(BTO|STC|STO|BTC)\b\s*(\d+)?\s*([A-Z]+)\s*(\d+[.\d+]*[cp]?)?\s*(\d{1,2}\/\d{1,2})?(?:\/202\d|\/2\d)?\s*@\s*[$]*[ ]*(\d+(?:[,.]\d+)?|\.\d+)'
     match = re.search(pattern, msg, re.IGNORECASE)
     
     if match:
         action, quantity, ticker, strike, expDate, price = match.groups()
 
         asset_type = 'option' if strike and expDate else 'stock'
         symbol =  ticker.upper()
         order = {
             'action': action.upper(),
             'Symbol': symbol,
-            'uQty': int(quantity) if quantity else 1,
+            'Qty': int(quantity) if quantity else 1,
             'price': float(price.replace(',', '.')) if price else None,
             'asset': asset_type
         }
         str_ext = ""
         if asset_type == 'option':
             # fix missing strike, assume Call            
             if "c" not in strike.lower() and "p" not in strike.lower():
@@ -43,15 +43,15 @@
         order['risk'] = risk_level
 
         pars = []
         for el in [action, quantity, ticker, strike, expDate, price, risk_level, str_ext]:
             if el is not None:
                 pars.append(el)
         pars = " ".join(pars)
-        if action.upper() == "BTO":
+        if action.upper() in ["BTO", "STO"]:
             if "avg" in msg.lower() or "average" in msg.lower():
                 avg_price, _ = parse_avg(msg)
                 pars = pars + f"AVG to {avg_price} "
                 order["avg"] = avg_price
             else:
                 order["avg"] = None
             pt1_v, pt2_v, pt3_v, sl_v = parse_exits(msg)
@@ -59,32 +59,72 @@
             pts_qty = set_pt_qts(n_pts)
             order, pars = make_order_exits(order, msg, pars, asset_type)
             sl_mental = True if "mental" in msg.lower() else False
             if sl_mental: order["SL_mental"] = True
             order["n_PTs"] = n_pts
             order["PTs_Qty"] = pts_qty
 
-        elif action.upper() == "STC":
+        elif action.upper() in ["STC", "BTC"]:
             xamnt = parse_sell_ratio_amount(msg, asset_type)
-            if order["uQty"] is None:
+            if order["Qty"] is None:
                 pars = pars + f" xamount: {xamnt}"
             order["xQty"] = xamnt
         
         return pars, order
     else:
+        # try exit update
+        pattern = r'\b(exit[ ]?update)\b\s*([A-Z]+)\s*(\d+[.\d+]*[cp]?)?\s*(\d{1,2}\/\d{1,2})?(?:\/202\d|\/2\d)?\s*'
+        match = re.search(pattern, msg, re.IGNORECASE)
+        if match:
+            action, ticker, strike, expDate = match.groups()
+            
+            asset_type = 'option' if strike and expDate else 'stock'
+            symbol =  ticker.upper()
+        
+            order = {
+            'action': "ExitUpdate",
+            'Symbol': symbol,
+            'asset': asset_type
+            }
+            str_ext = f'ExitUpdate: {symbol} '
+            if asset_type == 'option':
+                # fix missing strike, assume Call            
+                if "c" not in strike.lower() and "p" not in strike.lower():
+                    strike = strike + "c"
+                    order['strike'] = strike.upper()
+                    str_ext = " No direction found in option strike, assuming Call"
+
+                order['strike'] = strike.upper()
+                order['expDate'] = expDate
+                order['Symbol'] = fix_index_symbols(symbol)            
+                order['Symbol'] = make_optionID(**order)
+                str_ext += f"{strike.upper()} {expDate}"
+            order, str_ext = make_order_exits(order, msg, str_ext, asset_type)
+            return str_ext, order
         return None, None
 
 def fix_index_symbols(symbol):
     if symbol.upper() == "SPX": 
         symbol = "SPXW"
     elif symbol.upper() == "NDX":
         symbol = "NDXP"
     return symbol
     
 
+def ordersymb_to_str(symbol):
+    "Symbol format AAA_YYMMDDCCPXXX"
+    if "_" in symbol:
+        # option
+        exp = r"(\w+)_(\d{6})([CP])([\d.]+)"        
+        match = re.search(exp, symbol, re.IGNORECASE)
+        if match:
+            symbol, date, type, strike = match.groups()
+            symbol = f"{symbol} {strike}{type} {date[:2]}/{date[2:4]}"
+    return symbol
+
 def parser_alerts(msg, asset=None):
     msg = msg.replace("STc", "STC").replace("StC", "STC").replace("stC", "STC").replace("STc", "STC")
     msg = msg.replace("BtO", "BTO").replace("btO", "BTO").replace("bTO", "BTO").replace("BTo", "BTO")
     msg = msg.replace("spx", "SPX").replace("spy", "SPY").replace("Spx", "SPX")
     act = parse_action(msg)
     if act is None:
         if "ExitUpdate" in msg:
@@ -126,15 +166,15 @@
     amnt = parse_unit_amount(msg)
     risk_level = parse_risk(msg)
 
     order = {"action": act,
              "Symbol": Symbol,
              "price": mark,
              "asset": asset,
-             "uQty": amnt,
+             "Qty": amnt,
              "risk": risk_level}
 
     str_prt = f"{act} {Symbol} @{mark} amount: {amnt}"
 
     if asset == "option":
         if Symbol == "SPX": 
             order['Symbol'] = "SPXW"
@@ -161,15 +201,15 @@
         sl_mental = True if "mental" in msg.lower() else False
         if sl_mental: order["SL_mental"] = True
         order["n_PTs"] = n_pts
         order["PTs_Qty"] = pts_qty
 
     elif act == "STC":
         xamnt = parse_sell_ratio_amount(msg, asset)
-        if order["uQty"] is None:
+        if order["Qty"] is None:
             str_prt = str_prt + f" xamount: {xamnt}"
         order["xQty"] = xamnt
     return str_prt, order
 
 def make_order_exits(order, msg, str_prt, asset):
     pt1_v, pt2_v, pt3_v, sl_v = parse_exits(msg)
     if asset == "option":
@@ -189,15 +229,19 @@
                 str_prt = str_prt + f', {ext}:{order[ext]}'
     return order, str_prt
 
 def set_exit_price_type(exit_price, order):
     """Option or stock price decided with smallest distance"""
     if exit_price is None:
         return exit_price
-    if isinstance(exit_price, str): exit_price = eval(exit_price)
+    if (isinstance(exit_price, str) and ("TS" in exit_price or "%" in exit_price)) or \
+        (isinstance(exit_price, str) and not exit_price): 
+        return exit_price
+    if isinstance(exit_price, str): 
+        exit_price = eval(exit_price)
 
     price_strk = float(order['strike'][:-1])
     order_price = order.get('price', exit_price )  # IF NO ORDER PRICE TAKE EXIT!
     rtio_stock = abs(price_strk - exit_price)
     rtio_option = abs(order_price - exit_price)
 
     if rtio_stock < rtio_option:
@@ -344,25 +388,27 @@
     avg_inf = re_avg.search(msg.lower())
     if avg_inf is None:
         return None, None
     avg = float(avg_inf.groups()[-1])
     return avg, avg_inf.span()
 
 def parse_exits_vals(msg, expr):
-    re_comp= re.compile("(" + expr + "[:]?[ ]*[$]*(\d+[\.]*[\d]*))", re.IGNORECASE)
-    exit_inf = re_comp.search(msg)
+    re_comp= re.compile("\s" +expr + "[:]?[ ]*[$]*(\d*[\.]*[\d]*[%]?)(TS[\d+\.]*[%]?)?", re.IGNORECASE) 
+    exit_inf = re_comp.search(msg) 
 
     if exit_inf is None:
-        re_comp= re.compile("(" + expr.lower() + "[:]?[ ]*[$]*(\d+[\.]*[\d]*))")
-        exit_inf = re_comp.search(msg)
+        re_comp= re.compile("(" + expr.lower() + "[:]?[ ]*[$]*(\d*[\.]*[\d]*[%]?))", re.IGNORECASE)
+        exit_inf = re_comp.search(msg)        
 
         if exit_inf is None:
             return None
-
-    exit_v = float(exit_inf.groups()[-1].replace("..", ""))
+        elif "%" in exit_inf.groups()[-1]:
+            return exit_inf.groups()[-1]
+        return float(exit_inf.groups()[-1].replace("..", ""))
+    exit_v = exit_inf.group(1) + (exit_inf.group(2) if exit_inf.group(2) else "")
     return exit_v
 
 def parse_unit_amount(msg):    
     act = parse_action(msg)
     Symbol, _ = parse_Symbol(msg, act)
     
     exprs = f"{act}\s+(\d+) {Symbol}"
@@ -435,174 +481,25 @@
 
 def parse_exit_plan(order):
     exit_plan = {}
     for p in [f"PT{i}" for i in range (1,4)] + ["SL"]:
             exit_plan[p] = order.get(p)
     return exit_plan
 
-def auhtor_parser(msg, author, asset):
-    if author not in ['ScaredShirtless#0001', 'Kevin (Momentum)#4441']:
-        new_order = {}
-        def stc_amount(msg):
-            ######### Leave N untis
-            units = ["one", "two", "three"]
-            units_left = f'(?:(?:L|l)eaving|leave)[ ]*(?:only|just)?[ ]*({"|".join(units)})'
-            mtch = re.compile(units_left, re.IGNORECASE)
-            mtch = mtch.search(msg)
-            if mtch is not None:
-                strnum = mtch.groups()[0]
-                qty_left, = [i for i, v in enumerate(units) if v==strnum]
-                return qty_left
-
-            ######### Leave a few untis
-            left_few = '(?:(?:L|l)eaving|leave)[ ]*(?:only|just)?[ ]*[a]? (few)'
-            mtch = re.compile(left_few, re.IGNORECASE)
-            mtch = mtch.search(msg)
-            if mtch is not None:
-                return "few"
-
-            ######### Leave % amount
-            left_perc = '(?:(?:L|l)eaving|leave) (?:about|only)?[ ]*(\d{1,2})%'
-            mtch = re.compile(left_perc, re.IGNORECASE)
-            mtch = mtch.search(msg)
-            if mtch is not None:
-                perc = mtch.groups()[0]
-                return eval(perc)/100
-
-            return None
-
-        def match_exp(exp, msg):
-            mtch = re.compile(exp, re.IGNORECASE)
-            mtch = mtch.search(msg)
-            if mtch is not None:
-                return mtch.groups()[0]
-            return None
-
-        # in STC target might not be PT2
-        if "STC" not in msg:
-            pt1_exps = ['Target: (\d+[\.]*[\d]*)', 'target: (\d+[\.]*[\d]*)', 'target[a-zA-Z\s\,\.]*(\d+[\.]*[\d]*)',
-                   '(\d+[\.]*[\d]*)[a-zA-Z\s\,\.]*target',
-                   'looking for (\d+[\.]*[\d]*)']
-            for exp in pt1_exps:
-                pt1 = match_exp(exp, msg)
-                if pt1:
-                    pt1 = pt1[:-1] if pt1[-1] == '.' else pt1
-                    new_order["PT1"] = pt1
-                    msg = msg.replace(pt1, " ")
-                    break
-
-            pt2 = "target[a-zA-Z0-9\.\s\,]*then (\d+[\.]*[\d]*)"
-            pt2 = match_exp(pt2, msg)
-            if pt2:
-                pt2 = pt2[:-1] if pt2[-1] == '.' else pt2
-                new_order["PT2"] = pt2
-                msg = msg.replace(pt2, " ")
-        else:
-            pt2 = "second target[a-zA-Z0-9\.\s\,]*(\d+[\.]*[\d]*)"
-            pt2 = match_exp(pt2, msg)
-            if pt2:
-                new_order["PT2"] = pt2
-                msg = msg.replace(pt2, " ")
-
-        sl_exps = ['Stop: (\d+[\.]*[\d]*)', 'stop: (\d+[\.]*[\d]*)', '(\d+[\.]*[\d]*)[a-zA-Z\s\,\.]{0,5}?stop',
-                   'stop[a-zA-Z\s\,\.]*(\d+[\.]*[\d]*)']
-        for exp in sl_exps:
-            sl = match_exp(exp, msg)
-            if sl:
-                sl = sl[:-1] if sl[-1] == '.' else sl
-                new_order["SL"] = sl
-                break
-
-        if "BTO" not in msg:
-            amnt_left = stc_amount(msg)
-            if amnt_left:
-                new_order["amnt_left"] = amnt_left
-
-            if "STC" not in msg:
-                stc = "([^a-z]selling|[^a-z]sold|all out|(:?(out|took)[a-zA-Z\s]*last)|sell here|took some off)"
-                mtch = re.compile(stc, re.IGNORECASE)
-                mtch = mtch.search(msg)
-                no_Sell = ["not selling yet", "Over Sold", "contracts sold", "How many sold it?", 'No need to ask me if I’m selling']
-                if mtch is not None and not any([True if s in msg else False for s  in no_Sell]):
-                    new_order['action'] = "STC"
-                    new_order["xQty"]  = parse_sell_ratio_amount(msg, asset)
-
-        if len(list(new_order.values())):
-            symbol, _ = parse_Symbol(msg, parse_action(msg))
-            if symbol:
-                new_order["Symbol"] = symbol
-            return new_order
-        else:
-            return None
-    return None
-
-def get_symb_prev_msg(df_hist, msg_ix, author):
-    # df_hist["Author"]  = df_hist["Author"].apply(lambda x: x.split("#")[0])
-
-    df_hist_auth = df_hist[df_hist["Author"]==author]
-    msg_inx_auth, = np.nonzero(df_hist_auth.index == msg_ix)
-    indexes = df_hist_auth.index.values
-
-    for n in range(1,6):
-        inx = indexes[msg_inx_auth - n]
-        msg, = df_hist_auth.loc[inx, 'Content'].values
-        if pd.isnull(msg):
-            continue
-        symbol, _ = parse_Symbol(msg, parse_action(msg))
-        if symbol is not None:
-            return symbol, inx
-    return None, None
 
 def make_optionID(Symbol:str, expDate:str, strike=str, **kwarg):
     """
     date: "[M]M/[D]D" or "[M]M/[D]D/YY[YY]"
     """
     strike, opt_type = float(strike[:-1]), strike[-1]
     date_elms = expDate.split("/")
     date_frm = f"{int(date_elms[0]):02d}{int(date_elms[1]):02d}"
-    if len(date_elms) == 2: # MM/DD, year = current year
+    if len(date_elms) == 2: # MM/DD, year = actual year
         year = str(datetime.today().year)[-2:]
         date_frm = date_frm + year
     elif len(date_elms) == 3:
         date_frm = date_frm + f"{int(date_elms[2][-2:]):02d}"
 
     # Strike in interger if no decimals
     if strike == int(strike):
         return f"{Symbol}_{date_frm}{opt_type}{int(strike)}"
     return f"{Symbol}_{date_frm}{opt_type}{strike}"
-
-def combine_new_old_orders(msg, order_old, pars, author, asset="option"):
-    order_author = auhtor_parser(msg, author, asset)
-    if order_author is None:
-        return order_old, pars
-
-    if order_old is not None:
-        for k in order_author.keys():
-            # If
-            if order_author[k] == order_old.get(k) and k != "Symbol" or \
-                order_author[k] != order_old.get(k) and k == "Symbol":
-                if k == "Symbol":
-                    # in case of ticker vs option symbol ID
-                    if order_author[k] == order_old[k][:len(order_author[k])]:
-                        order_author[k] = order_old[k]
-                        continue
-                resp = input(f"Found diff vals for {k}: new= {order_author[k]}, old= {order_old[k]} " +
-                             "[1- new, 2- old, 0- break and fix]")
-                if resp == '2':
-                    order_author[k] = order_old.get(k)
-                elif resp == '0':
-                    raise "error"
-        order = {**order_old, **order_author}
-    else:
-        order = order_author
-
-    if order.get("action") is None:
-        order["asset"] = asset
-        exits = ["PT1", "PT2", "PT3", "SL"]
-        if any([order.get(k) for k in exits]):
-            order['action'] = "ExitUpdate"
-            pars = f"ExitUpdate: {pars}"
-            for ex in exits:
-                val = order.get(ex)
-                if val is not None:
-                    pars = pars + f" {ex}:{val},"
-    return order, pars
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/PKG-INFO` & `DiscordAlertsTrader-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,69 @@
-Metadata-Version: 2.1
-Name: DiscordAlertsTrader
-Version: 0.9.1
-Summary: Package for automating discord trade alerts in TDA or eTrade.
-Home-page: 
-Download-URL: https://github.com/AdoNunes/DiscordAlertsTrader
-Author: Adonay Nunes
-Author-email: adonays.nunes@gmail.com
-License: BSD (3-clause)
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Office/Business :: Financial
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
+![PyPI](https://img.shields.io/pypi/v/DiscordAlertsTrader)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/DiscordAlertsTrader)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/DiscordAlertsTrader)
+![GitHub](https://img.shields.io/github/license/AdoNunes/DiscordAlertsTrader)
+[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Zb4ymtF "realtime support / chat with the community and the team.")
+
+
+A Python package to automate trades from alerts shared in a Discord channel by analysts.
+The package parses these messages and executes trades from traders specified in the configuration file. 
+It tracks messages from all the channels, generates a portfolio from analysts and from trades executed, 
+provides live quotes to see actual alert profits (rather than prices stated in the alert), and can trigger
+an alert to open long or short a position, close it or update exits (target profit, stop loss).
 
-DiscordAlertsTrader is a python package to get messages from a subscribed discord channel where buy
- and sell stock and options signals are messaged. The package will parse the messages and execute
- the trades for traders specified in the config file. It will track the messages from all channels,
- the analysts portfolio and the bot portfolio.
+Trades are done through APIs of TDAmeritrade (full functionality), eTrade (long positions for now) or webull (long, no OCO, live quotes).
+If no brokerage API key is provided, it will just print the discord messages and track the 
+analysts portfolio. With an API key, it will track the current price of the alerts, besides executing trades.
 
-If no brokerage API key is provided, it will just print the discord messages and track the analysts
- portfolio. With a TDA API key, it will track current price of the alerts, and calculated PnL-current.
+If in `config.ini`, `DO_BTO_TRADES = false`, no trades will be executed. 
 
-If in config.ini DO_BTO_TRADES = false, not trades will be executed. 
 
-Trades are done through TDAmeritrade API, implementing webull and etrade.  
+## GUI capabilities ##
 
-What this package does:
+- Parsing trading signals from messages (e.g., BTO, STC, SL, PT).
+- Tracking trading signals with a message history tab for the channel
+- Tracking performance with real-time actual prices and returns.
+- Opening, closing, and updating trades through the GUI.
+- Calculate analysts' stats and provide options to test stats with maximum capital 
+- Checking order and account status, and accessing current ticker prices.
+- Supporting manual trade execution through prompts if `auto_trade` is set to False in `config.ini`.
 
-- Read messages and parse trading singals, e.g. BTO (Buy to Open), STC (Sell to Close), partial STC, SL (Stop Limits), PT (Profit Taking)
-- Track trading signals and performance of traders using message history and realtime price
-- Execute and cancel orders, check order status, account status and current ticker prices
-- If in config.ini auto_trade = False, trades are executed manually through promts and optionally choose QTY, price, etc
 
-**Currently, the package is for parsing signals of the discord server BullTrades.** 
+Supports any Discord channel with structured alerts BTO and STC as message contents (not embedded)
 
-Invite link to BullTrades with referral: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
+**Currently, version control for analysts portfolio is from server BullTrades.[you can see all historical stats]** 
+  - Invite link to BullTrades: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
 
+
+Let me know if you find the package useful or need support by dropping me an email or visiting the [discord server](https://discord.gg/9ejghcjpar)
+
+ ________________________
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
-<img src="media/xtrader_console.png" alt="Console with discord mesages" width="500" height="300">
+<img src="media/xtrader_console.png" alt="Console with discord messages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
 
 
  ## Discord user token and channel IDs
  ______________________________
 
-It requires a user discord token, once installed the package save the token in config.ini[discord], as well as the channel ID where alerts are posted.
-To get discord token and channels IDs follow the instructions in: https://github.com/Tyrrrz/DiscordChatExporter/blob/master/.docs/Token-and-IDs.md
+It requires a user discord token, once installed the package saves the token in config.ini[discord], as well as the channel ID where alerts are posted.
+To get the discord token follow the instructions: https://www.androidauthority.com/get-discord-token-3149920/
+To get the channel ID, in Discord right click on the channel and click "Copy Channel ID"
 
 
 ## Installation and Setup
  ______________________________
 
 1. Install Python:
-   - For Windows, open PowerShell and run the following command:
+   - For Windows, open PowerShell and run the following command, verify that it prints out "Hello World!":
      ```powershell
      if (-not (Test-Path $env:USERPROFILE\scoop)) {
          # Install Scoop
          Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
          irm get.scoop.sh | iex
      }
      scoop install git
@@ -75,17 +71,15 @@
      $extras = scoop bucket list | Select-String -Pattern '^extras$'
      if (-not $extras) {
          # Add the extras bucket    
          scoop bucket add extras
      }
      # Install Miniconda3
      scoop install miniconda3
-     ```
-   - Run the following command to verify that Python with Conda is installed:
-     ```powershell
+     # Check python is installed
      python -c "print('Hello, World!')"
      ```
 
 2. In the PowerShell terminal navigate to the directory where you want to clone the DiscordAlertsTrader package, e.g. type: `cd Desktop`.
 
 3. Clone the package from the GitHub repository and install the package and its dependencies using pip:
    ```shell
@@ -98,15 +92,15 @@
    ```shell
    cp DiscordAlertsTrader/config_example.ini DiscordAlertsTrader/config.ini
    ```
 
 6. Edit the `DiscordAlertsTrader/config.ini` file to add your Discord token and configure other settings:
    - Add your Discord token in the appropriate field.
    - (Optional) Modify other configurations as needed, such as authors to follow, trailing stop, etc.
-   - (Optional) If you have a TDA API, add it to the configuration.
+   - (Optional) If you have a TDA/etrade API, add it to the configuration. See next sections.
 
 **Running the DiscordAlertsTrader**
 
 To run the DiscordAlertsTrader, execute the following command in the terminal:
 
 ```shell
 DiscordAlertsTrader
@@ -116,26 +110,36 @@
 
 Make sure to keep the terminal or command prompt window open while the application is running to see any output or errors.
 
 **Closing the Application**
 
 To stop the DiscordAlertsTrader application, simply close the terminal or command prompt window where it is running.
 
-## Etrade
+## Etrade API
+____________
 
-create a sandbox (mock) api key:
+Create a sandbox (mock) api key:
 https://us.etrade.com/etx/ris/apikey
-then fill out the forms at the bottom of:
+
+To get the production (real) keys, fill out the forms at the bottom of:
 https://developer.etrade.com/getting-started
 
 Make sure to select free real-time quote data:
 https://us.etrade.com/etx/hw/subscriptioncenter#/subscription
 
 Before running the package and send orders, in etrade make a trailing stop order and preview to sign an Advanced Order Disclosure, otherwise an error will rise when posting the order
 
+## Webull API
+____________
+
+You will need to get a device ID, follow these steps to get DID, and then save it in the config.ini, along with credential details: 
+https://github.com/tedchou12/webull/wiki/Workaround-for-Login-Method-2
+
+Trading pin is the 6 digit code used to unlock webull
+
 ## TDAmeritrade
 _______________
 
 *CURRENTLY NO NEW DEVELOPER ACCOUNT ARE CREATED UNTIL THE MERGE*
 
 To access the TDAmeritrade account for trading and info is necessary to install 
 td-ameritrade-python-api from:
@@ -156,15 +160,15 @@
 ```
 
 then, run the script:
 ```python setup_TDA.py```
 it will prompt to:
 
 ```
-$ Please go to URL provided authorize your account: https://auth.tdameritrade.com/auth?response_type=code&redirect_uri=.......OAUTHAP
+$Go to URL provided authorize your account: https://auth.tdameritrade.com/auth?response_type=code&redirect_uri=.......OAUTHAP
 $ Paste the full URL redirect here:
 ```
 
 In your browser go to the link, accept TD ameritrade pop-up and copy the link you get re-directed. Once entered you will have your secrets_td.json
 
 ## Disclaimer
 _________
```

### Comparing `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/SOURCES.txt` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 LICENSE
 README.md
 setup.py
 DiscordAlertsTrader/__init__.py
+DiscordAlertsTrader/alerts_generator.py
 DiscordAlertsTrader/alerts_tracker.py
 DiscordAlertsTrader/alerts_trader.py
+DiscordAlertsTrader/calc_stats.py
+DiscordAlertsTrader/calc_strat.py
 DiscordAlertsTrader/configurator.py
 DiscordAlertsTrader/discord_bot.py
 DiscordAlertsTrader/fend_bot.py
 DiscordAlertsTrader/gui.py
 DiscordAlertsTrader/gui_generator.py
 DiscordAlertsTrader/gui_layouts.py
+DiscordAlertsTrader/load_chn_hist.py
 DiscordAlertsTrader/message_parser.py
+DiscordAlertsTrader/port_sim.py
+DiscordAlertsTrader/tem_etrades.py
+DiscordAlertsTrader/test_trader.py
 DiscordAlertsTrader.egg-info/PKG-INFO
 DiscordAlertsTrader.egg-info/SOURCES.txt
 DiscordAlertsTrader.egg-info/dependency_links.txt
 DiscordAlertsTrader.egg-info/entry_points.txt
 DiscordAlertsTrader.egg-info/requires.txt
 DiscordAlertsTrader.egg-info/top_level.txt
 DiscordAlertsTrader/brokerages/TDA_api.py
 DiscordAlertsTrader/brokerages/__init__.py
 DiscordAlertsTrader/brokerages/eTrade_api.py
+DiscordAlertsTrader/brokerages/weBull_api.py
 tests/__init__.py
-tests/msg_samples.py
-tests/td_dummy.py
+tests/mock_discord_message.py
 tests/test_AlertsTracker.py
-tests/test_TDsession.py
+tests/test_AlertsTrader.py
+tests/test_AlertsTrader_exits.py
+tests/test_TDA.py
 tests/test_configurator.py
 tests/test_discord_bot.py
-tests/test_gui_generator.py
+tests/test_msg_parsed.py
```

### Comparing `DiscordAlertsTrader-0.9.1/LICENSE` & `DiscordAlertsTrader-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-0.9.1/PKG-INFO` & `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiscordAlertsTrader
-Version: 0.9.1
+Version: 1.0.0
 Summary: Package for automating discord trade alerts in TDA or eTrade.
 Home-page: 
 Download-URL: https://github.com/AdoNunes/DiscordAlertsTrader
 Author: Adonay Nunes
 Author-email: adonays.nunes@gmail.com
 License: BSD (3-clause)
 Classifier: License :: OSI Approved :: BSD License
@@ -17,57 +17,74 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
+![PyPI](https://img.shields.io/pypi/v/DiscordAlertsTrader)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/DiscordAlertsTrader)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/DiscordAlertsTrader)
+![GitHub](https://img.shields.io/github/license/AdoNunes/DiscordAlertsTrader)
+[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Zb4ymtF "realtime support / chat with the community and the team.")
 
-DiscordAlertsTrader is a python package to get messages from a subscribed discord channel where buy
- and sell stock and options signals are messaged. The package will parse the messages and execute
- the trades for traders specified in the config file. It will track the messages from all channels,
- the analysts portfolio and the bot portfolio.
 
-If no brokerage API key is provided, it will just print the discord messages and track the analysts
- portfolio. With a TDA API key, it will track current price of the alerts, and calculated PnL-current.
+A Python package to automate trades from alerts shared in a Discord channel by analysts.
+The package parses these messages and executes trades from traders specified in the configuration file. 
+It tracks messages from all the channels, generates a portfolio from analysts and from trades executed, 
+provides live quotes to see actual alert profits (rather than prices stated in the alert), and can trigger
+an alert to open long or short a position, close it or update exits (target profit, stop loss).
 
-If in config.ini DO_BTO_TRADES = false, not trades will be executed. 
+Trades are done through APIs of TDAmeritrade (full functionality), eTrade (long positions for now) or webull (long, no OCO, live quotes).
+If no brokerage API key is provided, it will just print the discord messages and track the 
+analysts portfolio. With an API key, it will track the current price of the alerts, besides executing trades.
 
-Trades are done through TDAmeritrade API, implementing webull and etrade.  
+If in `config.ini`, `DO_BTO_TRADES = false`, no trades will be executed. 
 
-What this package does:
 
-- Read messages and parse trading singals, e.g. BTO (Buy to Open), STC (Sell to Close), partial STC, SL (Stop Limits), PT (Profit Taking)
-- Track trading signals and performance of traders using message history and realtime price
-- Execute and cancel orders, check order status, account status and current ticker prices
-- If in config.ini auto_trade = False, trades are executed manually through promts and optionally choose QTY, price, etc
+## GUI capabilities ##
 
-**Currently, the package is for parsing signals of the discord server BullTrades.** 
+- Parsing trading signals from messages (e.g., BTO, STC, SL, PT).
+- Tracking trading signals with a message history tab for the channel
+- Tracking performance with real-time actual prices and returns.
+- Opening, closing, and updating trades through the GUI.
+- Calculate analysts' stats and provide options to test stats with maximum capital 
+- Checking order and account status, and accessing current ticker prices.
+- Supporting manual trade execution through prompts if `auto_trade` is set to False in `config.ini`.
 
-Invite link to BullTrades with referral: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
 
+Supports any Discord channel with structured alerts BTO and STC as message contents (not embedded)
+
+**Currently, version control for analysts portfolio is from server BullTrades.[you can see all historical stats]** 
+  - Invite link to BullTrades: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
+
+
+Let me know if you find the package useful or need support by dropping me an email or visiting the [discord server](https://discord.gg/9ejghcjpar)
+
+ ________________________
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
-<img src="media/xtrader_console.png" alt="Console with discord mesages" width="500" height="300">
+<img src="media/xtrader_console.png" alt="Console with discord messages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
 
 
  ## Discord user token and channel IDs
  ______________________________
 
-It requires a user discord token, once installed the package save the token in config.ini[discord], as well as the channel ID where alerts are posted.
-To get discord token and channels IDs follow the instructions in: https://github.com/Tyrrrz/DiscordChatExporter/blob/master/.docs/Token-and-IDs.md
+It requires a user discord token, once installed the package saves the token in config.ini[discord], as well as the channel ID where alerts are posted.
+To get the discord token follow the instructions: https://www.androidauthority.com/get-discord-token-3149920/
+To get the channel ID, in Discord right click on the channel and click "Copy Channel ID"
 
 
 ## Installation and Setup
  ______________________________
 
 1. Install Python:
-   - For Windows, open PowerShell and run the following command:
+   - For Windows, open PowerShell and run the following command, verify that it prints out "Hello World!":
      ```powershell
      if (-not (Test-Path $env:USERPROFILE\scoop)) {
          # Install Scoop
          Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
          irm get.scoop.sh | iex
      }
      scoop install git
@@ -75,17 +92,15 @@
      $extras = scoop bucket list | Select-String -Pattern '^extras$'
      if (-not $extras) {
          # Add the extras bucket    
          scoop bucket add extras
      }
      # Install Miniconda3
      scoop install miniconda3
-     ```
-   - Run the following command to verify that Python with Conda is installed:
-     ```powershell
+     # Check python is installed
      python -c "print('Hello, World!')"
      ```
 
 2. In the PowerShell terminal navigate to the directory where you want to clone the DiscordAlertsTrader package, e.g. type: `cd Desktop`.
 
 3. Clone the package from the GitHub repository and install the package and its dependencies using pip:
    ```shell
@@ -98,15 +113,15 @@
    ```shell
    cp DiscordAlertsTrader/config_example.ini DiscordAlertsTrader/config.ini
    ```
 
 6. Edit the `DiscordAlertsTrader/config.ini` file to add your Discord token and configure other settings:
    - Add your Discord token in the appropriate field.
    - (Optional) Modify other configurations as needed, such as authors to follow, trailing stop, etc.
-   - (Optional) If you have a TDA API, add it to the configuration.
+   - (Optional) If you have a TDA/etrade API, add it to the configuration. See next sections.
 
 **Running the DiscordAlertsTrader**
 
 To run the DiscordAlertsTrader, execute the following command in the terminal:
 
 ```shell
 DiscordAlertsTrader
@@ -116,26 +131,36 @@
 
 Make sure to keep the terminal or command prompt window open while the application is running to see any output or errors.
 
 **Closing the Application**
 
 To stop the DiscordAlertsTrader application, simply close the terminal or command prompt window where it is running.
 
-## Etrade
+## Etrade API
+____________
 
-create a sandbox (mock) api key:
+Create a sandbox (mock) api key:
 https://us.etrade.com/etx/ris/apikey
-then fill out the forms at the bottom of:
+
+To get the production (real) keys, fill out the forms at the bottom of:
 https://developer.etrade.com/getting-started
 
 Make sure to select free real-time quote data:
 https://us.etrade.com/etx/hw/subscriptioncenter#/subscription
 
 Before running the package and send orders, in etrade make a trailing stop order and preview to sign an Advanced Order Disclosure, otherwise an error will rise when posting the order
 
+## Webull API
+____________
+
+You will need to get a device ID, follow these steps to get DID, and then save it in the config.ini, along with credential details: 
+https://github.com/tedchou12/webull/wiki/Workaround-for-Login-Method-2
+
+Trading pin is the 6 digit code used to unlock webull
+
 ## TDAmeritrade
 _______________
 
 *CURRENTLY NO NEW DEVELOPER ACCOUNT ARE CREATED UNTIL THE MERGE*
 
 To access the TDAmeritrade account for trading and info is necessary to install 
 td-ameritrade-python-api from:
@@ -156,15 +181,15 @@
 ```
 
 then, run the script:
 ```python setup_TDA.py```
 it will prompt to:
 
 ```
-$ Please go to URL provided authorize your account: https://auth.tdameritrade.com/auth?response_type=code&redirect_uri=.......OAUTHAP
+$Go to URL provided authorize your account: https://auth.tdameritrade.com/auth?response_type=code&redirect_uri=.......OAUTHAP
 $ Paste the full URL redirect here:
 ```
 
 In your browser go to the link, accept TD ameritrade pop-up and copy the link you get re-directed. Once entered you will have your secrets_td.json
 
 ## Disclaimer
 _________
```

### Comparing `DiscordAlertsTrader-0.9.1/setup.py` & `DiscordAlertsTrader-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     for line in (line.strip() for line in fid):
         if line.startswith('__version__'):
             version = line.split('=')[1].strip().strip('\'')
             break
 
 setup(
     name='DiscordAlertsTrader',
-    version='0.9.1',
+    version='1.0.0',
     author='Adonay Nunes',
     author_email='adonays.nunes@gmail.com',
     description='Package for automating discord trade alerts in TDA or eTrade.',
     license='BSD (3-clause)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='',
```

### Comparing `DiscordAlertsTrader-0.9.1/tests/test_configurator.py` & `DiscordAlertsTrader-1.0.0/tests/test_configurator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 
 import unittest
+import ast
 from DiscordAlertsTrader.configurator import cfg
 
 class TestConfigurator(unittest.TestCase):
 
-    def test_trailstop_val(self):
-        trailstop_val = cfg['order_configs']['default_trailstop']
-        self.assertTrue(trailstop_val == '' or eval(trailstop_val) > .9)
+    def test_defaul_exit(self):
+        print('default_exits:', cfg['order_configs']['default_exits'])
+        trailstop_val = ast.literal_eval(cfg['order_configs']['default_exits'])
+        vals = list(trailstop_val.keys())
+        self.assertTrue(["PT1", "PT2", "PT3", "SL"] ==  vals)
 
     def test_general_options(self):
         cfg['general'].getboolean('DO_BTO_TRADES')
         cfg['order_configs'].getboolean('sell_current_price')
         cfg['order_configs'].getboolean('auto_trade')
 
     def test_portfolio_names(self):
         for v in cfg['portfolio_names'].values():
             self.assertTrue(v.endswith(".csv"))
 
     def test_cfg_options_set(self):
-        self.assertTrue(cfg['general']['BROKERAGE'] in ['', 'TDA', "webull", 'etrades'])
+        self.assertTrue(cfg['general']['BROKERAGE'].lower() in ['', 'tda', "webull", 'etrade'])
         self.assertTrue(cfg['order_configs']['default_bto_qty'] in ['buy_one', 'trade_capital'])
         
 if __name__ == '__main__':
     unittest.main()
```

