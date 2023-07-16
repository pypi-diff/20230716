# Comparing `tmp/volstreet-1.0.0.tar.gz` & `tmp/volstreet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.0.0.tar", last modified: Sun Jul 16 12:55:25 2023, max compression
+gzip compressed data, was "volstreet-1.0.1.tar", last modified: Sun Jul 16 21:45:46 2023, max compression
```

## Comparing `volstreet-1.0.0.tar` & `volstreet-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 12:55:25.771697 volstreet-1.0.0/
--rw-rw-rw-   0        0        0      497 2023-07-16 12:55:25.771697 volstreet-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.0/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-07-16 12:55:25.774111 volstreet-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 12:55:25.765208 volstreet-1.0.0/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.0/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.0/volstreet/__init__.py
--rw-rw-rw-   0        0        0     8889 2023-07-08 15:26:12.000000 volstreet-1.0.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.0/volstreet/constants.py
--rw-rw-rw-   0        0        0    41203 2023-07-14 15:07:17.000000 volstreet-1.0.0/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   185952 2023-07-16 12:37:53.000000 volstreet-1.0.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-1.0.0/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.0/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    13073 2023-07-15 16:36:10.000000 volstreet-1.0.0/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-16 12:55:25.771697 volstreet-1.0.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 21:45:46.169169 volstreet-1.0.1/
+-rw-rw-rw-   0        0        0      497 2023-07-16 21:45:46.170166 volstreet-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.1/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-07-16 21:45:46.171162 volstreet-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 21:45:46.162808 volstreet-1.0.1/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.1/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.1/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.1/volstreet/constants.py
+-rw-rw-rw-   0        0        0    42479 2023-07-16 12:56:47.000000 volstreet-1.0.1/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   192015 2023-07-16 21:34:09.000000 volstreet-1.0.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.1/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.1/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    13111 2023-07-16 12:56:47.000000 volstreet-1.0.1/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:45:46.169169 volstreet-1.0.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-16 21:45:46.000000 volstreet-1.0.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-16 21:45:46.000000 volstreet-1.0.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 21:45:46.000000 volstreet-1.0.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-07-16 21:45:46.000000 volstreet-1.0.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 21:45:46.000000 volstreet-1.0.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.0.0/setup.cfg` & `volstreet-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 300d 0a61  rsion = 1.0.0..a
+00000020: 7273 696f 6e20 3d20 312e 302e 310d 0a61  rsion = 1.0.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.0.0/volstreet/SmartWebSocketV2.py` & `volstreet-1.0.1/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.0/volstreet/blackscholes.py` & `volstreet-1.0.1/volstreet/blackscholes.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,130 +167,157 @@
             "implied_volatility": ivs,
         }
     )
 
 
 def iv_transformer_coeffs(tte):
     adjuster = 3 if tte < (0.8 / 365) else 1
-    dfs2 = 1 / ((tte ** 1.2) * adjuster)
+    dfs2 = 1 / ((tte**1.2) * adjuster)
     dfs2 = min(dfs2, 20000)
 
-    dfs = 1 / ((tte ** 0.45) * 5)
+    dfs = 1 / ((tte**0.45) * 5)
     dfs = min(dfs, 5)
     dfs = -6 + dfs
-    return dfs2, dfs, .97
+    return dfs2, dfs, 0.97
 
 
 def iv_transformer_coeffs_wip(tte):
-
     # distance squared coefficient
-    dfs2 = 3270.27*np.exp(-384.38*tte) + 100
+    dfs2 = 3270.27 * np.exp(-384.38 * tte) + 100
     dfs2 = min(dfs2, 20000)
 
     # distance coefficient
-    if tte < 0.26/365:
+    if tte < 0.26 / 365:
         dfs = 1
     else:
-        dfs = 1 / ((tte ** 0.45) * 5)
+        dfs = 1 / ((tte**0.45) * 5)
         dfs = min(dfs, 5)
         dfs = -6 + dfs
 
     # intercept
-    if tte < 3/(24*365):
+    if tte < 3 / (24 * 365):
         intercept = 1.07
-    elif tte < 0.27/365:
+    elif tte < 0.27 / 365:
         intercept = 1
     else:
         intercept = 0.98
     return dfs2, dfs, intercept
 
 
-def iv_curve_adjustor(movement, time_to_expiry, iv: int | tuple = 1, spot=100, strike=100, _print_details=False):
-
+def iv_curve_adjustor(
+    movement,
+    time_to_expiry,
+    iv: int | tuple = 1,
+    spot=100,
+    strike=100,
+    _print_details=False,
+):
     """
     This function returns the adjusted implied volatility accounting for the curve effect.
     :param movement: movement of the underlying in percentage with sign
     :param time_to_expiry: time to expiry in years
     :param iv: implied volatility of the strike
     :param spot: spot price
     :param strike: strike price
     :param _print_details: print details of the adjustment
     :return: adjusted implied volatility for the strike after the movement
     """
 
     coefs = iv_transformer_coeffs_wip(time_to_expiry)
-    current_diff = (strike/spot - 1)
-    current_iv_multiple = coefs[0] * current_diff ** 2 + coefs[1] * current_diff + coefs[2]
+    current_diff = strike / spot - 1
+    current_iv_multiple = (
+        coefs[0] * current_diff**2 + coefs[1] * current_diff + coefs[2]
+    )
     atm_iv = iv / current_iv_multiple
 
     new_spot = spot * (1 + movement)
-    total_displacement = (strike / new_spot - 1)
-    premium_to_atm_iv = coefs[0] * total_displacement ** 2 + coefs[1] * total_displacement + coefs[2]
+    total_displacement = strike / new_spot - 1
+    premium_to_atm_iv = (
+        coefs[0] * total_displacement**2 + coefs[1] * total_displacement + coefs[2]
+    )
     new_iv = atm_iv * premium_to_atm_iv
 
     if _print_details:
         print(
-            f'New iv: {new_iv} for strike {strike} spot {new_spot} '
-            f'iv {iv} atm_iv {atm_iv} movement {movement} '
-            f'time_to_expiry {time_to_expiry}'
+            f"New iv: {new_iv} for strike {strike} spot {new_spot} "
+            f"iv {iv} atm_iv {atm_iv} movement {movement} "
+            f"time_to_expiry {time_to_expiry}"
         )
 
     return new_iv
 
 
 def target_movement(
-        flag, current_price, target_price, current_spot, strike, timeleft, time_delta=None, _print_details=False
+    flag,
+    current_price,
+    target_price,
+    current_spot,
+    strike,
+    timeleft,
+    time_delta=None,
+    _print_details=False,
 ):
     """
     :param flag: 'c' or 'p'
     :param current_price: current price of the option
     :param target_price: target price of the option
     :param current_spot: current spot price
     :param strike: strike price
     :param timeleft: time left to expiry in years
     :param time_delta: in minutes
     :param _print_details: print details of the adjustment
     :return:
     """
     flag = flag.lower()[0]
-    price_func = call if flag == 'c' else put
+    price_func = call if flag == "c" else put
     vol = implied_volatility(current_price, current_spot, strike, timeleft, 0.06, flag)
     delta_ = delta(current_spot, strike, timeleft, 0.06, vol, flag)
     estimated_movement_points = (target_price - current_price) / delta_
     estimated_movement = estimated_movement_points / current_spot
     timeleft = timeleft - (time_delta / 525600) if time_delta else timeleft
 
-    if timeleft < 0.0008:  # On expiry day we need to adjust the vol as iv increases steadily as we approach expiry
+    if (
+        timeleft < 0.0008
+    ):  # On expiry day we need to adjust the vol as iv increases steadily as we approach expiry
         vol_multiple = 2 - (1401.74 * timeleft)
         vol = vol * vol_multiple
 
     modified_vol = iv_curve_adjustor(
-        estimated_movement, timeleft, iv=vol, spot=current_spot, strike=strike, _print_details=_print_details
+        estimated_movement,
+        timeleft,
+        iv=vol,
+        spot=current_spot,
+        strike=strike,
+        _print_details=_print_details,
     )
 
     if _print_details:
-        print(f'estimated movement: {estimated_movement}, vol: {vol}, modified vol: {modified_vol}')
+        print(
+            f"estimated movement: {estimated_movement}, vol: {vol}, modified vol: {modified_vol}"
+        )
 
     f = lambda s1: price_func(s1, strike, timeleft, 0.06, modified_vol) - target_price
 
     if target_price > current_price:
-        if flag == 'c':
+        if flag == "c":
             a = current_spot
             b = 2 * current_spot
         else:
             a = 0.05
             b = current_spot
     else:
-        if flag == 'c':
+        if flag == "c":
             a = 0.05
             b = current_spot
         else:
             a = current_spot
             b = 2 * current_spot
 
-    target_spot = brentq(f, a=a, b=b, xtol=1e-15, rtol=1e-15, maxiter=1000, full_output=False)
+    target_spot = brentq(
+        f, a=a, b=b, xtol=1e-15, rtol=1e-15, maxiter=1000, full_output=False
+    )
 
     assert isinstance(target_spot, float)
 
-    movement = (target_spot/current_spot) - 1
+    movement = (target_spot / current_spot) - 1
 
     return movement
```

### Comparing `volstreet-1.0.0/volstreet/constants.py` & `volstreet-1.0.1/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.0/volstreet/datamodule.py` & `volstreet-1.0.1/volstreet/datamodule.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,18 @@
         if api_key is None:
             raise ApiKeyNotFound("EOD API Key not found")
         self.api_key = api_key
         self.client = EodHistoricalData(api_key=api_key)
 
     @staticmethod
     def parse_symbol(symbol):
-
         symbol_dict = {
             "NIFTY": "NSEI.INDX",
             "NIFTY 50": "NSEI.INDX",
-            "NIFTY50" : "NSEI.INDX",
+            "NIFTY50": "NSEI.INDX",
             "BANKNIFTY": "NSEBANK.INDX",
             "NIFTY BANK": "NSEBANK.INDX",
             "NIFTYBANK": "NSEBANK.INDX",
             "FINNIFTY": "CNXFIN.INDX",
             "NIFTY FIN SERVICE": "CNXFIN.INDX",
             "VIX": "NIFVIX.INDX",
         }
@@ -42,15 +41,14 @@
             if symbol in symbol_dict:
                 symbol = symbol_dict[symbol]
             else:
                 symbol = symbol + ".NSE"
         return symbol
 
     def get_data(self, symbol, from_date="2011-01-01", return_columns=None):
-
         name = symbol.split(".")[0] if "." in symbol else symbol
 
         symbol = self.parse_symbol(symbol)
 
         if return_columns is None:
             return_columns = ["open", "close", "gap", "intra", "abs_gap", "abs_intra"]
 
@@ -65,38 +63,40 @@
         df["intra"] = (df.close / df.open - 1) * 100
         df["abs_gap"] = abs(df.gap)
         df["abs_intra"] = abs(df.intra)
         df = df.loc[:, return_columns]
         df.name = name
         return df
 
-    def get_intraday_data(self, symbol, interval, from_date="2011-01-01", return_columns=None):
-
+    def get_intraday_data(
+        self, symbol, interval, from_date="2011-01-01", return_columns=None
+    ):
         name = symbol.split(".")[0] if "." in symbol else symbol
 
         symbol = self.parse_symbol(symbol)
 
         if return_columns is None:
-            return_columns = ['open', 'high', 'low', 'close']
+            return_columns = ["open", "high", "low", "close"]
 
         resp_list = []
         from_date = pd.to_datetime(from_date)
         while datetime.now().date() > from_date.date():
             to_date = from_date + timedelta(days=120)
             resp = self.client.get_prices_intraday(
-                symbol, interval=interval,
+                symbol,
+                interval=interval,
                 from_=str(int(from_date.timestamp())),
-                to=str(int(to_date.timestamp()))
+                to=str(int(to_date.timestamp())),
             )
 
             resp_list.extend(resp)
             from_date += timedelta(days=120)
 
         df = pd.DataFrame(resp_list)
-        df.index = pd.to_datetime(df['datetime'])
+        df.index = pd.to_datetime(df["datetime"])
         df = df.drop_duplicates()
         df.index = df.index + timedelta(hours=5, minutes=30)
         df = df[return_columns]
         df.name = name
         return df
 
 
@@ -116,15 +116,15 @@
 def analyser(df, frequency=None, date_filter=None, _print=False):
     name = df.name
     if date_filter is None:
         pass
     else:
         dates = date_filter.split("to")
         if len(dates) > 1:
-            df = df.loc[dates[0]: dates[1]]
+            df = df.loc[dates[0] : dates[1]]
         else:
             df = df.loc[dates[0]]
 
     frequency = frequency.upper() if frequency is not None else None
 
     if frequency is None or frequency.startswith("D") or frequency == "B":
         custom_frequency = "B"
@@ -223,21 +223,20 @@
             symbol_monthly_data, periods=periods, ignore_last=ignore_last
         )
         df_dict[symbol] = recent_vol
     return df_dict
 
 
 def ratio_analysis(
-        x_df: pd.DataFrame,
-        y_df: pd.DataFrame,
-        periods_to_avg: int = None,
-        return_summary=True,
-        add_rolling: bool | int = False
+    x_df: pd.DataFrame,
+    y_df: pd.DataFrame,
+    periods_to_avg: int = None,
+    return_summary=True,
+    add_rolling: bool | int = False,
 ):
-
     if periods_to_avg is None:
         periods_to_avg = len(x_df)
 
     x_close = x_df.iloc[-periods_to_avg:].close
     x_array = x_df.iloc[-periods_to_avg:].abs_change
     x_avg = x_array.mean()
 
@@ -270,33 +269,34 @@
         rolling_y_avg = y_array.rolling(add_rolling, min_periods=1).mean()
         rolling_ratio = rolling_x_avg / rolling_y_avg
         ratio_summary[f"Rolling {add_rolling} Ratio"] = rolling_ratio
 
     return ratio_summary
 
 
-def get_summary_ratio(target_symbol, benchmark_symbol, frequency='D', periods_to_avg=50, client=None):
-
+def get_summary_ratio(
+    target_symbol, benchmark_symbol, frequency="D", periods_to_avg=50, client=None
+):
     try:
         if client is None:
             try:
-                dc = DataClient(__import__('os').getenv('EOD_API_KEY'))
+                dc = DataClient(__import__("os").getenv("EOD_API_KEY"))
             except ApiKeyNotFound:
                 return None
         else:
             dc = client
 
         benchmark = dc.get_data(benchmark_symbol)
         target = dc.get_data(target_symbol)
         benchmark = analyser(benchmark, frequency=frequency)
         target = analyser(target, frequency=frequency)
         ratio = ratio_analysis(target, benchmark, periods_to_avg=periods_to_avg)
-        return ratio.loc['Summary', 'Ratio']
+        return ratio.loc["Summary", "Ratio"]
     except Exception as e:
-        vs.logger.error(f'Error in get_summary_ratio: {e}')
+        vs.logger.error(f"Error in get_summary_ratio: {e}")
         return None
 
 
 @retain_name
 def generate_streak(df, query):
     df = df.copy(deep=True)
 
@@ -331,15 +331,14 @@
                 return [f"{frequency}-{day}" for day in days]
             else:
                 return [frequency]
         else:
             return [frequency]
 
     def _calculate_streak_summary(df, frequency, query):
-
         # Calculate the streak summary
 
         if df.index[-1].replace(hour=15, minute=30) > vs.currenttime():
             df = df.iloc[:-1]
         check_date = df.index[-1]
         total_instances = len(df)
         df = generate_streak(df, query)
@@ -359,15 +358,16 @@
         current_streak = (
             df.iloc[-1].streak_count if df.iloc[-1].end_date == check_date else None
         )
 
         # Calculating the percentile of the current streak
         if current_streak:
             current_streak_percentile = (
-                    df.streak_count.sort_values().values.searchsorted(current_streak) / len(df)
+                df.streak_count.sort_values().values.searchsorted(current_streak)
+                / len(df)
             )
         else:
             current_streak_percentile = 0
 
         return {
             "freq": frequency,  # Use the given freq value instead of df.iloc[-1].name
             "total_instances": total_instances,
@@ -396,18 +396,22 @@
         )
 
     freqs = generate_frequency(freq)
     streaks = []
     for freq in freqs:
         dataframe = analyser(instrument, frequency=freq)
         if query == "abs_change":
-            recommended_threshold = dataframe.abs_change.mean() * 0.70  # 0.70 should cover 50% of the data
+            recommended_threshold = (
+                dataframe.abs_change.mean() * 0.70
+            )  # 0.70 should cover 50% of the data
             # (mildly adjusted for abnormal distribution)
             recommended_threshold = round(recommended_threshold, 2)
-            recommended_sign = ">" if dataframe.iloc[-2].abs_change > recommended_threshold else "<"
+            recommended_sign = (
+                ">" if dataframe.iloc[-2].abs_change > recommended_threshold else "<"
+            )
             query = f"abs_change {recommended_sign} {recommended_threshold}"
             print(f"Recommended query: {query}\n")
         streak_summary = _calculate_streak_summary(dataframe, freq, query)
         streaks.append(streak_summary)
         print_streak_summary(streak_summary)
     # Convert the list of dictionaries to a list of DataFrames
     streaks_df = [pd.DataFrame([streak]) for streak in streaks]
@@ -425,15 +429,14 @@
     iv: pd.Series,
     time_to_expiry: pd.Series,
     strike_offset: float,
     base: float = 100,
     label: str = "",
     action="buy",
 ):
-
     if label:
         label = f"{label}_"
 
     action = action.lower()
 
     if action not in ["buy", "sell"]:
         raise ValueError("action must be either 'buy' or 'sell'")
@@ -497,15 +500,15 @@
 def get_index_vs_constituents_recent_vols(
     index_symbol,
     return_all=False,
     simulate_backtest=False,
     strike_offset=0,
     hedge_offset=0,
     stock_vix_adjustment=0.7,
-    index_action="sell"
+    index_action="sell",
 ):
     """
     Get the recent volatility of the index and its constituents
     """
     if return_all is False:
         simulate_backtest = False
 
@@ -543,41 +546,55 @@
             index_monthly_data["time_to_expiry"] = (
                 index_monthly_data.index.to_series().diff().dt.days / 365
             )
 
             index_hedge_action = "buy" if index_action == "sell" else "sell"
 
             # The main strike
-            simulated_data = simulate_strike_premium_payoff(index_monthly_data["index_close"],
-                                                            index_monthly_data["index_iv"],
-                                                            index_monthly_data["time_to_expiry"], strike_offset, 100,
-                                                            label="index", action=index_action)
+            simulated_data = simulate_strike_premium_payoff(
+                index_monthly_data["index_close"],
+                index_monthly_data["index_iv"],
+                index_monthly_data["time_to_expiry"],
+                strike_offset,
+                100,
+                label="index",
+                action=index_action,
+            )
             index_monthly_data = index_monthly_data.merge(
                 simulated_data, left_index=True, right_index=True, how="left"
             )
 
             index_monthly_data["index_initial_premium_pct"] = (
-                    index_monthly_data["index_initial_premium"] / index_monthly_data["index_close"]
+                index_monthly_data["index_initial_premium"]
+                / index_monthly_data["index_close"]
             )
 
             # The hedge strike
-            simulated_data = simulate_strike_premium_payoff(index_monthly_data["index_close"],
-                                                            index_monthly_data["index_iv"],
-                                                            index_monthly_data["time_to_expiry"], hedge_offset, 100,
-                                                            label="index_hedge", action=index_hedge_action)
+            simulated_data = simulate_strike_premium_payoff(
+                index_monthly_data["index_close"],
+                index_monthly_data["index_iv"],
+                index_monthly_data["time_to_expiry"],
+                hedge_offset,
+                100,
+                label="index_hedge",
+                action=index_hedge_action,
+            )
 
-            index_monthly_data = index_monthly_data.merge(simulated_data, left_index=True, right_index=True, how="left")
+            index_monthly_data = index_monthly_data.merge(
+                simulated_data, left_index=True, right_index=True, how="left"
+            )
 
             index_monthly_data["index_hedge_initial_premium_pct"] = (
-                    index_monthly_data["index_hedge_initial_premium"] / index_monthly_data["index_close"]
+                index_monthly_data["index_hedge_initial_premium"]
+                / index_monthly_data["index_close"]
             )
 
             index_monthly_data["index_bep_pct"] = (
-                    index_monthly_data["index_initial_premium_pct"] -
-                    index_monthly_data["index_hedge_initial_premium_pct"]
+                index_monthly_data["index_initial_premium_pct"]
+                - index_monthly_data["index_hedge_initial_premium_pct"]
             )
 
         else:
             raise NotImplementedError
 
     constituent_dfs = []
     for i, constituent in enumerate(constituents):
@@ -592,176 +609,205 @@
             constituent_monthly_data[f"{constituent}_abs_change"] * weights[i]
         )
 
         if simulate_backtest:
             constituent_monthly_data[f"{constituent}_iv"] = index_monthly_data[
                 "iv_diff_from_mean"
             ] * (
-                (constituent_monthly_data[f"{constituent}_abs_change"].mean() - stock_vix_adjustment) * 4.4
+                (
+                    constituent_monthly_data[f"{constituent}_abs_change"].mean()
+                    - stock_vix_adjustment
+                )
+                * 4.4
             )  # the adjustment factor is to account for the spurious volatility on account of splits
 
             constituent_action = "buy" if index_action == "sell" else "sell"
             constituent_hedge_action = "sell" if constituent_action == "buy" else "sell"
 
             # The main strike
-            simulated_data = simulate_strike_premium_payoff(constituent_monthly_data[f"{constituent}_close"],
-                                                            constituent_monthly_data[f"{constituent}_iv"],
-                                                            index_monthly_data["time_to_expiry"], strike_offset, 5,
-                                                            label=constituent, action=constituent_action)
+            simulated_data = simulate_strike_premium_payoff(
+                constituent_monthly_data[f"{constituent}_close"],
+                constituent_monthly_data[f"{constituent}_iv"],
+                index_monthly_data["time_to_expiry"],
+                strike_offset,
+                5,
+                label=constituent,
+                action=constituent_action,
+            )
             constituent_monthly_data = constituent_monthly_data.merge(
                 simulated_data, left_index=True, right_index=True, how="left"
             )
 
             constituent_monthly_data[f"{constituent}_initial_premium_pct"] = (
-                constituent_monthly_data[f"{constituent}_initial_premium"] /
-                constituent_monthly_data[f"{constituent}_close"]
+                constituent_monthly_data[f"{constituent}_initial_premium"]
+                / constituent_monthly_data[f"{constituent}_close"]
             )
 
             # The hedge strike
-            simulated_data = simulate_strike_premium_payoff(constituent_monthly_data[f"{constituent}_close"],
-                                                            constituent_monthly_data[f"{constituent}_iv"],
-                                                            index_monthly_data["time_to_expiry"], hedge_offset, 5,
-                                                            label=f'{constituent}_hedge',
-                                                            action=constituent_hedge_action)
+            simulated_data = simulate_strike_premium_payoff(
+                constituent_monthly_data[f"{constituent}_close"],
+                constituent_monthly_data[f"{constituent}_iv"],
+                index_monthly_data["time_to_expiry"],
+                hedge_offset,
+                5,
+                label=f"{constituent}_hedge",
+                action=constituent_hedge_action,
+            )
             constituent_monthly_data = constituent_monthly_data.merge(
                 simulated_data, left_index=True, right_index=True, how="left"
             )
 
             constituent_monthly_data[f"{constituent}_hedge_initial_premium_pct"] = (
-                constituent_monthly_data[f"{constituent}_hedge_initial_premium"] /
-                constituent_monthly_data[f"{constituent}_close"]
+                constituent_monthly_data[f"{constituent}_hedge_initial_premium"]
+                / constituent_monthly_data[f"{constituent}_close"]
             )
 
             constituent_monthly_data[f"{constituent}_bep_pct"] = (
                 constituent_monthly_data[f"{constituent}_initial_premium_pct"]
                 - constituent_monthly_data[f"{constituent}_hedge_initial_premium_pct"]
             )
 
             constituent_monthly_data[f"{constituent}_total_payoff"] = (
                 constituent_monthly_data[f"{constituent}_payoff"]
                 + constituent_monthly_data[f"{constituent}_hedge_payoff"]
             )
             constituent_monthly_data[f"{constituent}_total_payoff_pct"] = (
-                constituent_monthly_data[f"{constituent}_total_payoff"] /
-                constituent_monthly_data[f"{constituent}_close"]
+                constituent_monthly_data[f"{constituent}_total_payoff"]
+                / constituent_monthly_data[f"{constituent}_close"]
             )
             constituent_monthly_data[f"{constituent}_total_payoff_pct_weighted"] = (
                 constituent_monthly_data[f"{constituent}_total_payoff_pct"] * weights[i]
             )
 
         constituent_dfs.append(constituent_monthly_data)
 
     index_monthly_data = index_monthly_data.merge(
-        pd.concat(constituent_dfs, axis=1), left_index=True, right_index=True, how="inner"
+        pd.concat(constituent_dfs, axis=1),
+        left_index=True,
+        right_index=True,
+        how="inner",
     )
     index_monthly_data = index_monthly_data.copy()
     index_monthly_data["sum_constituent_movement"] = index_monthly_data.filter(
         regex="abs_change_weighted"
     ).sum(axis=1)
     index_monthly_data["ratio_of_movements"] = (
         index_monthly_data["sum_constituent_movement"]
         / index_monthly_data["index_abs_change"]
     )
 
     if simulate_backtest:
         index_monthly_data["index_total_payoff"] = (
-                index_monthly_data["index_payoff"] + index_monthly_data["index_hedge_payoff"]
+            index_monthly_data["index_payoff"]
+            + index_monthly_data["index_hedge_payoff"]
         )
         index_monthly_data["index_total_payoff_pct"] = (
-                index_monthly_data["index_total_payoff"] / index_monthly_data["index_close"]
+            index_monthly_data["index_total_payoff"] / index_monthly_data["index_close"]
         )
         index_monthly_data["sum_constituent_payoff_pct"] = index_monthly_data.filter(
             regex="total_payoff_pct_weighted"
         ).sum(axis=1)
 
-        index_monthly_data['total_combined_payoff_pct'] = (
-                index_monthly_data["index_total_payoff_pct"] + index_monthly_data["sum_constituent_payoff_pct"]
+        index_monthly_data["total_combined_payoff_pct"] = (
+            index_monthly_data["index_total_payoff_pct"]
+            + index_monthly_data["sum_constituent_payoff_pct"]
         )
 
     if return_all:
         return index_monthly_data
     else:
         summary_df = index_monthly_data[
             ["index_abs_change", "sum_constituent_movement", "ratio_of_movements"]
         ]
         return summary_df
 
 
 def get_greenlit_kite(
-        kite_api_key,
-        kite_api_secret,
-        kite_user_id,
-        kite_password,
-        kite_auth_key,
-        chrome_path=None
+    kite_api_key,
+    kite_api_secret,
+    kite_user_id,
+    kite_password,
+    kite_auth_key,
+    chrome_path=None,
 ):
     if chrome_path is None:
         driver = webdriver.Chrome()
     else:
         driver = webdriver.Chrome(chrome_path)
 
     authkey_obj = pyotp.TOTP(kite_auth_key)
     kite = KiteConnect(api_key=kite_api_key)
     login_url = kite.login_url()
 
     driver.get(login_url)
     wait = WebDriverWait(driver, 10)  # waits for up to 10 seconds
 
-    userid = wait.until(EC.presence_of_element_located((By.ID, 'userid')))
+    userid = wait.until(EC.presence_of_element_located((By.ID, "userid")))
     userid.send_keys(kite_user_id)
 
-    password = wait.until(EC.presence_of_element_located((By.ID, 'password')))
+    password = wait.until(EC.presence_of_element_located((By.ID, "password")))
     password.send_keys(kite_password)
 
-    submit = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'button-orange')))
+    submit = wait.until(
+        EC.presence_of_element_located((By.CLASS_NAME, "button-orange"))
+    )
     submit.click()
 
     sleep(10)  # wait for the OTP input field to be clickable
-    otp_input = wait.until(EC.element_to_be_clickable((By.TAG_NAME, 'input')))
+    otp_input = wait.until(EC.element_to_be_clickable((By.TAG_NAME, "input")))
     otp_input.send_keys(authkey_obj.now())
 
     # wait until the URL changes
     wait.until(url_changes(driver.current_url))
 
     # now you can safely get the current URL
     current_url = driver.current_url
 
-    split_url = current_url.split('=')
+    split_url = current_url.split("=")
     request_token = None
     for i, string in enumerate(split_url):
-        if 'request_token' in string:
+        if "request_token" in string:
             request_token = split_url[i + 1]
-            request_token = request_token.split('&')[0] if '&' in request_token else request_token
+            request_token = (
+                request_token.split("&")[0] if "&" in request_token else request_token
+            )
             break
 
     driver.quit()
 
     if request_token is None:
-        raise Exception('Request token not found')
+        raise Exception("Request token not found")
 
     data = kite.generate_session(request_token, api_secret=kite_api_secret)
     kite.set_access_token(data["access_token"])
 
     return kite
 
 
-def get_1m_data(kite, symbol, path='C:\\Users\\Administrator\\'):
-
+def get_1m_data(kite, symbol, path="C:\\Users\\Administrator\\"):
     def fetch_minute_data_from_kite(_kite, _token, _from_date, _to_date):
-        date_format = '%Y-%m-%d %H:%M:%S'
-        _prices = _kite.historical_data(_token, from_date=_from_date.strftime(date_format),
-                                        to_date=_to_date.strftime(date_format), interval='minute')
+        date_format = "%Y-%m-%d %H:%M:%S"
+        _prices = _kite.historical_data(
+            _token,
+            from_date=_from_date.strftime(date_format),
+            to_date=_to_date.strftime(date_format),
+            interval="minute",
+        )
         return _prices
 
-    instruments = kite.instruments(exchange='NSE')
-    token = [instrument['instrument_token'] for instrument in instruments if instrument['tradingsymbol'] == symbol][0]
+    instruments = kite.instruments(exchange="NSE")
+    token = [
+        instrument["instrument_token"]
+        for instrument in instruments
+        if instrument["tradingsymbol"] == symbol
+    ][0]
 
     try:
         main_df = pd.read_csv(
-            f'{path}{symbol}_onemin_prices.csv', index_col=0, parse_dates=True
+            f"{path}{symbol}_onemin_prices.csv", index_col=0, parse_dates=True
         )
         from_date = main_df.index[-1] + timedelta(minutes=1)
     except FileNotFoundError:
         print(f"No existing data for {symbol}, starting from scratch.")
         main_df = False
         from_date = datetime(2015, 1, 1, 9, 16)
 
@@ -769,232 +815,350 @@
     mainlist = []
 
     fetch_data_partial = partial(fetch_minute_data_from_kite, kite, token)
 
     while from_date < end_date:
         to_date = from_date + timedelta(days=60)
         prices = fetch_data_partial(from_date, to_date)
-        if len(prices) < 2 and not mainlist:  # if there is no data for the period and no data at all
-            print(f'No data for {from_date.strftime("%Y-%m-%d %H:%M:%S")} to {to_date.strftime("%Y-%m-%d %H:%M:%S")}')
+        if (
+            len(prices) < 2 and not mainlist
+        ):  # if there is no data for the period and no data at all
+            print(
+                f'No data for {from_date.strftime("%Y-%m-%d %H:%M:%S")} to {to_date.strftime("%Y-%m-%d %H:%M:%S")}'
+            )
             if to_date > vs.currenttime():
                 return None
             else:
                 from_date += timedelta(days=60)
                 continue
         else:  # if there is data for the period
             mainlist.extend(prices)
             from_date += timedelta(days=60)
 
-    df = pd.DataFrame(mainlist).set_index('date')
+    df = pd.DataFrame(mainlist).set_index("date")
     df.index = df.index.tz_localize(None)
-    df = df[~df.index.duplicated(keep='first')]
+    df = df[~df.index.duplicated(keep="first")]
     df = df[(df.index.time >= time(9, 15)) & (df.index.time <= time(15, 30))]
-    df.to_csv(f'{path}{symbol}_onemin_prices.csv', mode='a', header=not isinstance(main_df, pd.DataFrame))
-    print(f'Finished fetching data for {symbol}. Fetched data from {df.index[0]} to {df.index[-1]}')
+    df.to_csv(
+        f"{path}{symbol}_onemin_prices.csv",
+        mode="a",
+        header=not isinstance(main_df, pd.DataFrame),
+    )
+    print(
+        f"Finished fetching data for {symbol}. Fetched data from {df.index[0]} to {df.index[-1]}"
+    )
     full_df = pd.concat([main_df, df]) if isinstance(main_df, pd.DataFrame) else df
     return full_df
 
 
-def get_constituent_1m_data(kite_object, index_name, path='C:\\Users\\Administrator\\'):
+def get_constituent_1m_data(kite_object, index_name, path="C:\\Users\\Administrator\\"):
     tickers, _weights = vs.get_index_constituents(index_name)
     for ticker in tickers:
-        print(f'Fetching data for {ticker}')
+        print(f"Fetching data for {ticker}")
         get_1m_data(kite_object, ticker, path=path)
 
 
 def backtest_intraday_trend(
-        one_min_df, beta=1, trend_threshold=1, max_entries=3, eod_client=None, rolling_days=60
+    one_min_df,
+    beta=1,
+    trend_threshold=1,
+    max_entries=3,
+    eod_client=None,
+    rolling_days=60,
 ):
-
     one_min_df = one_min_df.copy()
-    if one_min_df.index.name == 'date':
+    if one_min_df.index.name == "date":
         one_min_df = one_min_df.reset_index()
-    one_min_df = one_min_df[(one_min_df['date'].dt.time > time(9, 15)) & (one_min_df['date'].dt.time < time(15, 30))]
+    one_min_df = one_min_df[
+        (one_min_df["date"].dt.time > time(9, 15))
+        & (one_min_df["date"].dt.time < time(15, 30))
+    ]
 
     unavailable_dates = [
         datetime(2015, 2, 28).date(),
         datetime(2016, 10, 30).date(),
         datetime(2019, 10, 27).date(),
         datetime(2020, 2, 1).date(),
-        datetime(2020, 11, 14).date()
+        datetime(2020, 11, 14).date(),
     ]
 
     # Fetching vix data and calculating beta
     if eod_client is None:
         client = DataClient(api_key=__import__("os").environ.get("EOD_API_KEY"))
     else:
         client = eod_client
 
     vix = client.get_data("VIX", return_columns=["open", "close"])
-    vix = vix.resample('B').ffill()
-    vix['open'] = vix['open'] * beta
-    vix['close'] = vix['close'] * beta
-
-    one_min_df.drop(one_min_df[one_min_df['date'].dt.date.isin(unavailable_dates)].index, inplace=True)
-    open_prices = one_min_df.groupby(one_min_df['date'].dt.date).close.first().to_frame()
-    open_data = open_prices.merge(vix['open'].to_frame(), left_index=True, right_index=True)
-    open_data['threshold_movement'] = (open_data['open'] / 48) * trend_threshold
-    open_data['upper_bound'] = open_data['close'] * (1 + open_data['threshold_movement'] / 100)
-    open_data['lower_bound'] = open_data['close'] * (1 - open_data['threshold_movement'] / 100)
-    open_data['day_close'] = one_min_df.groupby(one_min_df['date'].dt.date).close.last()
-    open_data.columns = ['day_open', 'open_vix', 'threshold_movement', 'upper_bound', 'lower_bound', 'day_close']
+    vix = vix.resample("B").ffill()
+    vix["open"] = vix["open"] * beta
+    vix["close"] = vix["close"] * beta
+
+    one_min_df.drop(
+        one_min_df[one_min_df["date"].dt.date.isin(unavailable_dates)].index,
+        inplace=True,
+    )
+    open_prices = (
+        one_min_df.groupby(one_min_df["date"].dt.date).close.first().to_frame()
+    )
+    open_data = open_prices.merge(
+        vix["open"].to_frame(), left_index=True, right_index=True
+    )
+    open_data["threshold_movement"] = (open_data["open"] / 48) * trend_threshold
+    open_data["upper_bound"] = open_data["close"] * (
+        1 + open_data["threshold_movement"] / 100
+    )
+    open_data["lower_bound"] = open_data["close"] * (
+        1 - open_data["threshold_movement"] / 100
+    )
+    open_data["day_close"] = one_min_df.groupby(one_min_df["date"].dt.date).close.last()
+    open_data.columns = [
+        "day_open",
+        "open_vix",
+        "threshold_movement",
+        "upper_bound",
+        "lower_bound",
+        "day_close",
+    ]
     one_min_df[
-        ['day_open', 'open_vix', 'threshold_movement', 'upper_bound', 'lower_bound', 'day_close']
-    ] = open_data.loc[one_min_df['date'].dt.date].values
-    one_min_df['change_from_open'] = ((one_min_df['close']/one_min_df['day_open']) - 1)*100
+        [
+            "day_open",
+            "open_vix",
+            "threshold_movement",
+            "upper_bound",
+            "lower_bound",
+            "day_close",
+        ]
+    ] = open_data.loc[one_min_df["date"].dt.date].values
+    one_min_df["change_from_open"] = (
+        (one_min_df["close"] / one_min_df["day_open"]) - 1
+    ) * 100
 
     def calculate_daily_trade_data(group):
         all_entries_in_a_day = {}
         # Find the first index where the absolute price change crosses the threshold
         entry = 1
         while entry <= max_entries:
-            idx = group[abs(group['change_from_open']) >= group['threshold_movement']].first_valid_index()
+            idx = group[
+                abs(group["change_from_open"]) >= group["threshold_movement"]
+            ].first_valid_index()
             if idx is not None:  # if there is a crossing
                 result_dict = {
-                    'returns': 0,
-                    'trigger_time': np.nan,
-                    'trigger_price': np.nan,
-                    'trend_direction': np.nan,
-                    'stop_loss_price': np.nan,
-                    'stop_loss_time': np.nan
+                    "returns": 0,
+                    "trigger_time": np.nan,
+                    "trigger_price": np.nan,
+                    "trend_direction": np.nan,
+                    "stop_loss_price": np.nan,
+                    "stop_loss_time": np.nan,
                 }
                 # Record the price and time of crossing the threshold
-                cross_price = group.loc[idx, 'close']
-                cross_time = group.loc[idx, 'date']
+                cross_price = group.loc[idx, "close"]
+                cross_time = group.loc[idx, "date"]
 
                 # Determine the direction of the movement
-                direction = np.sign(group.loc[idx, 'change_from_open'])
+                direction = np.sign(group.loc[idx, "change_from_open"])
 
                 # Calculate the stoploss price
                 stoploss_price = cross_price * (1 - 0.003 * direction)
-                result_dict.update({
-                    'trigger_time': cross_time,
-                    'trigger_price': cross_price,
-                    'trend_direction': direction,
-                    'stop_loss_price': stoploss_price
-                })
-                future_prices = group.loc[idx:, 'close']
-
-                if (
-                        (direction == 1 and future_prices.min() <= stoploss_price)
-                        or (direction == -1 and future_prices.max() >= stoploss_price)
+                result_dict.update(
+                    {
+                        "trigger_time": cross_time,
+                        "trigger_price": cross_price,
+                        "trend_direction": direction,
+                        "stop_loss_price": stoploss_price,
+                    }
+                )
+                future_prices = group.loc[idx:, "close"]
+
+                if (direction == 1 and future_prices.min() <= stoploss_price) or (
+                    direction == -1 and future_prices.max() >= stoploss_price
                 ):  # Stop loss was breached
-                    result_dict['returns'] = -0.30
-                    stoploss_time_idx = future_prices[future_prices <= stoploss_price].first_valid_index() \
-                        if direction == 1 else future_prices[future_prices >= stoploss_price].first_valid_index()
-                    stoploss_time = group.loc[stoploss_time_idx, 'date']
-                    result_dict['stop_loss_time'] = stoploss_time
-                    all_entries_in_a_day[f'entry_{entry}'] = result_dict
+                    result_dict["returns"] = -0.30
+                    stoploss_time_idx = (
+                        future_prices[
+                            future_prices <= stoploss_price
+                        ].first_valid_index()
+                        if direction == 1
+                        else future_prices[
+                            future_prices >= stoploss_price
+                        ].first_valid_index()
+                    )
+                    stoploss_time = group.loc[stoploss_time_idx, "date"]
+                    result_dict["stop_loss_time"] = stoploss_time
+                    all_entries_in_a_day[f"entry_{entry}"] = result_dict
                     group = group.loc[stoploss_time_idx:]
                     entry += 1
                 else:  # Stop loss was not breached
                     if direction == 1:
-                        result_dict['returns'] = ((group['close'].iloc[-1] - cross_price) / cross_price)*100
+                        result_dict["returns"] = (
+                            (group["close"].iloc[-1] - cross_price) / cross_price
+                        ) * 100
                     else:
-                        result_dict['returns'] = ((group['close'].iloc[-1] - cross_price) / cross_price)*-100
-                    all_entries_in_a_day[f'entry_{entry}'] = result_dict
+                        result_dict["returns"] = (
+                            (group["close"].iloc[-1] - cross_price) / cross_price
+                        ) * -100
+                    all_entries_in_a_day[f"entry_{entry}"] = result_dict
                     break
             else:
                 break
 
-        all_entries_in_a_day['total_returns'] = sum([v['returns'] for v in all_entries_in_a_day.values()])
+        all_entries_in_a_day["total_returns"] = sum(
+            [v["returns"] for v in all_entries_in_a_day.values()]
+        )
         return all_entries_in_a_day
 
     # Applying the function to each day's worth of data
-    returns = one_min_df.groupby(one_min_df['date'].dt.date).apply(calculate_daily_trade_data)
+    returns = one_min_df.groupby(one_min_df["date"].dt.date).apply(
+        calculate_daily_trade_data
+    )
     returns = returns.to_frame()
     returns.index = pd.to_datetime(returns.index)
-    returns.columns = ['trade_data']
+    returns.columns = ["trade_data"]
 
     # merging with open_data
     merged = returns.merge(open_data, left_index=True, right_index=True)
-    merged['total_returns'] = merged['trade_data'].apply(lambda x: x['total_returns'])
-    merged = nav_drawdown_analyser(merged, column_to_convert='total_returns', profit_in_pct=True)
+    merged["total_returns"] = merged["trade_data"].apply(lambda x: x["total_returns"])
+    merged = nav_drawdown_analyser(
+        merged, column_to_convert="total_returns", profit_in_pct=True
+    )
 
     # calculating the minute vol
-    merged['minute_vol'] = one_min_df.groupby(one_min_df['date'].dt.date).apply(
-        lambda x: x['close'].pct_change().abs().mean() * 100).to_frame()
+    merged["minute_vol"] = (
+        one_min_df.groupby(one_min_df["date"].dt.date)
+        .apply(lambda x: x["close"].pct_change().abs().mean() * 100)
+        .to_frame()
+    )
 
     # calculating the open to close trend
-    merged['open_to_close_trend'] = one_min_df.close.groupby(one_min_df['date'].dt.date).apply(
-        lambda x: (x.iloc[-1] / x.iloc[0] - 1) * 100).abs().to_frame()
+    merged["open_to_close_trend"] = (
+        one_min_df.close.groupby(one_min_df["date"].dt.date)
+        .apply(lambda x: (x.iloc[-1] / x.iloc[0] - 1) * 100)
+        .abs()
+        .to_frame()
+    )
 
     # calculating the ratio and rolling mean
     rolling_days = rolling_days
-    merged['minute_vol_rolling'] = merged['minute_vol'].rolling(rolling_days,
-                                                                min_periods=1).mean()
-    merged['open_to_close_trend_rolling'] = merged['open_to_close_trend'].rolling(
-        rolling_days, min_periods=1).mean()
-    merged['ratio'] = merged['open_to_close_trend'] / merged['minute_vol']
-    merged['rolling_ratio'] = merged['open_to_close_trend_rolling'] / merged[
-        'minute_vol_rolling']
+    merged["minute_vol_rolling"] = (
+        merged["minute_vol"].rolling(rolling_days, min_periods=1).mean()
+    )
+    merged["open_to_close_trend_rolling"] = (
+        merged["open_to_close_trend"].rolling(rolling_days, min_periods=1).mean()
+    )
+    merged["ratio"] = merged["open_to_close_trend"] / merged["minute_vol"]
+    merged["rolling_ratio"] = (
+        merged["open_to_close_trend_rolling"] / merged["minute_vol_rolling"]
+    )
 
     return merged
 
 
-def calculate_intraday_return_drivers(symbol_one_min_df, day_wise_summary_df, rolling_days=60):
-
+def calculate_intraday_return_drivers(
+    symbol_one_min_df, day_wise_summary_df, rolling_days=60
+):
     symbol_one_min_df = symbol_one_min_df[
-        (symbol_one_min_df.index.time > time(9, 15)) & (symbol_one_min_df.index.time < time(15, 30))
-        ]
-    minute_vol = symbol_one_min_df.groupby(symbol_one_min_df.index.date).apply(
-        lambda x: x['close'].pct_change().abs().mean() * 100).to_frame()
+        (symbol_one_min_df.index.time > time(9, 15))
+        & (symbol_one_min_df.index.time < time(15, 30))
+    ]
+    minute_vol = (
+        symbol_one_min_df.groupby(symbol_one_min_df.index.date)
+        .apply(lambda x: x["close"].pct_change().abs().mean() * 100)
+        .to_frame()
+    )
     minute_vol.index = pd.to_datetime(minute_vol.index)
-    minute_vol.columns = ['minute_vol']
+    minute_vol.columns = ["minute_vol"]
 
-    open_to_close_trend = symbol_one_min_df.close.groupby(symbol_one_min_df.index.date).apply(
-        lambda x: (x.iloc[-1] / x.iloc[0] - 1) * 100).abs().to_frame()
+    open_to_close_trend = (
+        symbol_one_min_df.close.groupby(symbol_one_min_df.index.date)
+        .apply(lambda x: (x.iloc[-1] / x.iloc[0] - 1) * 100)
+        .abs()
+        .to_frame()
+    )
     open_to_close_trend.index = pd.to_datetime(open_to_close_trend.index)
-    open_to_close_trend.columns = ['open_to_close_trend']
-    drivers_of_returns = minute_vol.merge(open_to_close_trend, left_index=True, right_index=True)
+    open_to_close_trend.columns = ["open_to_close_trend"]
+    drivers_of_returns = minute_vol.merge(
+        open_to_close_trend, left_index=True, right_index=True
+    )
     drivers_of_returns = drivers_of_returns.merge(
         day_wise_summary_df.total_returns.to_frame(), left_index=True, right_index=True
     )
 
     # Rolling the minute vol and open to close trend
     rolling_days = rolling_days
-    drivers_of_returns['minute_vol_rolling'] = drivers_of_returns['minute_vol'].rolling(rolling_days,
-                                                                                        min_periods=1).mean()
-    drivers_of_returns['open_to_close_trend_rolling'] = drivers_of_returns['open_to_close_trend'].rolling(
-        rolling_days, min_periods=1).mean()
-    drivers_of_returns['ratio'] = drivers_of_returns['open_to_close_trend'] / drivers_of_returns['minute_vol']
-    drivers_of_returns['rolling_ratio'] = drivers_of_returns['open_to_close_trend_rolling'] / drivers_of_returns[
-        'minute_vol_rolling']
-    drivers_of_returns['returns_rolling'] = (drivers_of_returns['returns'] / 100 + 1).cumprod()
+    drivers_of_returns["minute_vol_rolling"] = (
+        drivers_of_returns["minute_vol"].rolling(rolling_days, min_periods=1).mean()
+    )
+    drivers_of_returns["open_to_close_trend_rolling"] = (
+        drivers_of_returns["open_to_close_trend"]
+        .rolling(rolling_days, min_periods=1)
+        .mean()
+    )
+    drivers_of_returns["ratio"] = (
+        drivers_of_returns["open_to_close_trend"] / drivers_of_returns["minute_vol"]
+    )
+    drivers_of_returns["rolling_ratio"] = (
+        drivers_of_returns["open_to_close_trend_rolling"]
+        / drivers_of_returns["minute_vol_rolling"]
+    )
+    drivers_of_returns["returns_rolling"] = (
+        drivers_of_returns["returns"] / 100 + 1
+    ).cumprod()
 
     return drivers_of_returns
 
 
-def nav_drawdown_analyser(df, column_to_convert='profit', base_price_col='close', nav_start=100, profit_in_pct=False):
-    """ Supply an analysed dataframe with a column that has the profit/loss in percentage or absolute value.
+def nav_drawdown_analyser(
+    df,
+    column_to_convert="profit",
+    base_price_col="close",
+    nav_start=100,
+    profit_in_pct=False,
+):
+    """Supply an analysed dataframe with a column that has the profit/loss in percentage or absolute value.
     Params:
     df: Dataframe with the column to be converted to NAV
     column_to_convert: Column name to be converted to NAV (default: 'profit')
     nav_start: Starting NAV (default: 100)
     profit_in_pct: If the column is in percentage or absolute value (default: False)
     """
 
     df = df.copy(deep=True)
     if column_to_convert in df.columns:
         if profit_in_pct == False:
-            df['profit_pct'] = (df[column_to_convert] / df[base_price_col]) * 100
+            df["profit_pct"] = (df[column_to_convert] / df[base_price_col]) * 100
         else:
-            df['profit_pct'] = df[column_to_convert]
-        df['strat_nav'] = ((df.profit_pct + 100) / 100).dropna().cumprod() * nav_start
-        df['cum_max'] = df.strat_nav.cummax()
-        df['drawdown'] = ((df.strat_nav / df.cum_max) - 1) * 100
-        df['rolling_cagr'] = df[:-1].apply(lambda row: ((df.strat_nav[-1] / row.strat_nav) ** (1 / (
-                (df.iloc[-1].name - row.name).days / 365)) - 1) * 100, axis=1)
+            df["profit_pct"] = df[column_to_convert]
+        df["strat_nav"] = ((df.profit_pct + 100) / 100).dropna().cumprod() * nav_start
+        df["cum_max"] = df.strat_nav.cummax()
+        df["drawdown"] = ((df.strat_nav / df.cum_max) - 1) * 100
+        df["rolling_cagr"] = df[:-1].apply(
+            lambda row: (
+                (df.strat_nav[-1] / row.strat_nav)
+                ** (1 / ((df.iloc[-1].name - row.name).days / 365))
+                - 1
+            )
+            * 100,
+            axis=1,
+        )
 
         # Drawdown ID below
-        df['drawdown_checker'] = np.where(df.drawdown != 0, 1, 0)
-        df['change_in_trend'] = df.drawdown_checker.ne(df.drawdown_checker.shift(1))
+        df["drawdown_checker"] = np.where(df.drawdown != 0, 1, 0)
+        df["change_in_trend"] = df.drawdown_checker.ne(df.drawdown_checker.shift(1))
         # df['streak_id'] = df.change_in_trend.cumsum()
-        df['start_of_drawdown'] = np.where((df.change_in_trend == True) &
-                                           (df.drawdown_checker == 1), True, False)
-        df['end_of_drawdown'] = np.where((df.change_in_trend == True) &
-                                         (df.drawdown_checker == 0), True, False)
-        df['drawdown_id'] = df.start_of_drawdown.cumsum()
+        df["start_of_drawdown"] = np.where(
+            (df.change_in_trend == True) & (df.drawdown_checker == 1), True, False
+        )
+        df["end_of_drawdown"] = np.where(
+            (df.change_in_trend == True) & (df.drawdown_checker == 0), True, False
+        )
+        df["drawdown_id"] = df.start_of_drawdown.cumsum()
         df.drawdown_id = np.where(df.drawdown_checker == 1, df.drawdown_id, None)
-        return df.drop(['start_of_drawdown', 'end_of_drawdown', 'drawdown_checker', 'change_in_trend'], axis=1)
+        return df.drop(
+            [
+                "start_of_drawdown",
+                "end_of_drawdown",
+                "drawdown_checker",
+                "change_in_trend",
+            ],
+            axis=1,
+        )
     else:
-        print('No profit column found in df.')
+        print("No profit column found in df.")
```

### Comparing `volstreet-1.0.0/volstreet/dealingroom.py` & `volstreet-1.0.1/volstreet/dealingroom.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,45 +19,49 @@
 import functools
 import itertools
 import traceback
 
 global login_data, obj
 
 LARGE_ORDER_THRESHOLD = 10
-ERROR_NOTIFICATION_SETTINGS = {'url': None}
+ERROR_NOTIFICATION_SETTINGS = {"url": None}
 
 
 def set_error_notification_settings(key, value):
     global ERROR_NOTIFICATION_SETTINGS
     ERROR_NOTIFICATION_SETTINGS[key] = value
 
 
 def time_the_function(func):
     def wrapper(*args, **kwargs):
         start = datetime.now()
         result = func(*args, **kwargs)
         end = (datetime.now() - start).total_seconds()
         logger.info(f"Time taken for {func.__name__}: {end:.2f} seconds")
         return result
+
     return wrapper
 
 
 def log_errors(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
-            user_prefix = ERROR_NOTIFICATION_SETTINGS.get('user', '')
-            logger.error(f"{user_prefix}Error in function {func.__name__}: {e}\nTraceback:{traceback.format_exc()}")
+            user_prefix = ERROR_NOTIFICATION_SETTINGS.get("user", "")
+            logger.error(
+                f"{user_prefix}Error in function {func.__name__}: {e}\nTraceback:{traceback.format_exc()}"
+            )
             notifier(
                 f"{user_prefix}Error in function {func.__name__}: {e}\nTraceback:{traceback.format_exc()}",
-                ERROR_NOTIFICATION_SETTINGS['url']
+                ERROR_NOTIFICATION_SETTINGS["url"],
             )
             raise e
+
     return wrapper
 
 
 class OptionChains(defaultdict):
     """An object for having option chains for multiple expiries.
     Each expiry is a dictionary with integer default values"""
 
@@ -124,15 +128,17 @@
         self.last_update_time = currenttime()
 
     def parse_price_dict(self):
         new_price_dict = {
             scrips.loc[scrips.token == token]["symbol"].values[0]: value
             for token, value in self.price_dict.items()
         }
-        new_price_dict.update({"FINNIFTY": {"ltp": self.finnifty_index.fetch_ltp()}})  # Finnifty temp fix
+        new_price_dict.update(
+            {"FINNIFTY": {"ltp": self.finnifty_index.fetch_ltp()}}
+        )  # Finnifty temp fix
         return new_price_dict
 
     def add_options(self, *underlyings, range_of_strikes=10, expiries=None, mode=1):
         """Adds options for the given underlyings to the symbol_option_chains dictionary.
         Params:
         underlyings is a list of underlying objects not strings
         If expiries is None, then the current, next and month expiry are added.
@@ -503,15 +509,22 @@
 
     def fetch_ltp(self):
         return fetchltp("NFO", self.symbol, self.token)
 
     def fetch_symbol_token(self):
         return self.symbol, self.token
 
-    def place_order(self, transaction_type, quantity_in_lots, price="LIMIT", stop_loss_order=False, order_tag=""):
+    def place_order(
+        self,
+        transaction_type,
+        quantity_in_lots,
+        price="LIMIT",
+        stop_loss_order=False,
+        order_tag="",
+    ):
         if isinstance(price, str):
             if price.upper() == "LIMIT":
                 price = self.fetch_ltp()
                 modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
                 price = price * modifier
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         order_ids = []
@@ -519,29 +532,31 @@
             order_id = place_order(
                 self.symbol,
                 self.token,
                 qty * self.lot_size,
                 transaction_type,
                 price,
                 stop_loss_order=stop_loss_order,
-                order_tag=order_tag
+                order_tag=order_tag,
             )
             order_ids.append(order_id)
         self.order_id_log.append(order_ids)
         return order_ids
 
 
 class Strangle:
     def __init__(self, call_strike, put_strike, underlying, expiry):
         self.call_option = Option(call_strike, "CE", underlying, expiry)
         self.put_option = Option(put_strike, "PE", underlying, expiry)
         self.call_strike = self.call_option.strike
         self.put_strike = self.put_option.strike
         self.underlying = underlying
-        self.underlying_exchange = "NFO" if self.underlying in ["FINNIFTY", "MIDCPNIFTY"] else "NSE"  # Fin/Mid temp fix
+        self.underlying_exchange = (
+            "NFO" if self.underlying in ["FINNIFTY", "MIDCPNIFTY"] else "NSE"
+        )  # Fin/Mid temp fix
         self.expiry = expiry
         self.call_symbol, self.call_token = self.call_option.fetch_symbol_token()
         self.put_symbol, self.put_token = self.put_option.fetch_symbol_token()
         self.freeze_qty_in_shares = self.call_option.freeze_qty_in_shares
         self.freeze_qty_in_lots = self.call_option.freeze_qty_in_lots
         self.lot_size = self.call_option.lot_size
 
@@ -576,58 +591,68 @@
         call_ltp, put_ltp = fetchltp(
             "NFO", self.call_symbol, self.call_token
         ), fetchltp("NFO", self.put_symbol, self.put_token)
         return call_ltp + put_ltp
 
     def price_disparity(self):
         call_ltp, put_ltp = self.fetch_ltp()
-        disparity = abs(call_ltp - put_ltp)/min(call_ltp, put_ltp)
+        disparity = abs(call_ltp - put_ltp) / min(call_ltp, put_ltp)
         return disparity
 
     def fetch_symbol_token(self):
         return self.call_symbol, self.call_token, self.put_symbol, self.put_token
 
-    def place_order(self, transaction_type, quantity_in_lots, prices="LIMIT", stop_loss_order=False, order_tag=""):
-
+    def place_order(
+        self,
+        transaction_type,
+        quantity_in_lots,
+        prices="LIMIT",
+        stop_loss_order=False,
+        order_tag="",
+    ):
         if stop_loss_order:
-            assert isinstance(prices, (tuple, list, np.ndarray)), "Prices must be a tuple of prices for stop loss order"
+            assert isinstance(
+                prices, (tuple, list, np.ndarray)
+            ), "Prices must be a tuple of prices for stop loss order"
             call_price, put_price = prices
         else:
             if isinstance(prices, (tuple, list, np.ndarray)):
                 call_price, put_price = prices
             elif prices.upper() == "LIMIT":
                 call_price, put_price = self.fetch_ltp()
                 modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
                 call_price, put_price = call_price * modifier, put_price * modifier
             elif prices.upper() == "MARKET":
                 call_price = put_price = prices
             else:
-                raise ValueError("Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices")
+                raise ValueError(
+                    "Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices"
+                )
 
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         call_order_ids = []
         put_order_ids = []
         for qty in spliced_orders:
             call_order_id = place_order(
                 self.call_symbol,
                 self.call_token,
                 qty * self.lot_size,
                 transaction_type,
                 call_price,
                 stop_loss_order=stop_loss_order,
-                order_tag=order_tag
+                order_tag=order_tag,
             )
             put_order_id = place_order(
                 self.put_symbol,
                 self.put_token,
                 qty * self.lot_size,
                 transaction_type,
                 put_price,
                 stop_loss_order=stop_loss_order,
-                order_tag=order_tag
+                order_tag=order_tag,
             )
             call_order_ids.append(call_order_id)
             put_order_ids.append(put_order_id)
         return call_order_ids, put_order_ids
 
 
 class Straddle(Strangle):
@@ -636,49 +661,58 @@
 
 
 class SyntheticFuture(Strangle):
     def __init__(self, strike, underlying, expiry):
         super().__init__(strike, strike, underlying, expiry)
 
     def place_order(
-            self, transaction_type, quantity_in_lots, prices: str | tuple = "LIMIT", stop_loss_order=False, order_tag=""
+        self,
+        transaction_type,
+        quantity_in_lots,
+        prices: str | tuple = "LIMIT",
+        stop_loss_order=False,
+        order_tag="",
     ):
         if isinstance(prices, (tuple, list, np.ndarray)):
             call_price, put_price = prices
         elif prices.upper() == "LIMIT":
             call_price, put_price = self.fetch_ltp()
-            c_modifier, p_modifier = (1.05, 0.95) if transaction_type.upper() == "BUY" else (0.95, 1.05)
+            c_modifier, p_modifier = (
+                (1.05, 0.95) if transaction_type.upper() == "BUY" else (0.95, 1.05)
+            )
             call_price, put_price = call_price * c_modifier, put_price * p_modifier
         elif prices.upper() == "MARKET":
             call_price = put_price = prices
         else:
-            raise ValueError("Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices")
+            raise ValueError(
+                "Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices"
+            )
 
         call_transaction_type = "BUY" if transaction_type.upper() == "BUY" else "SELL"
         put_transaction_type = "SELL" if transaction_type.upper() == "BUY" else "BUY"
 
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         call_order_ids = []
         put_order_ids = []
         for qty in spliced_orders:
             call_order_id = place_order(
                 self.call_symbol,
                 self.call_token,
                 qty * self.lot_size,
                 call_transaction_type,
                 call_price,
-                order_tag=order_tag
+                order_tag=order_tag,
             )
             put_order_id = place_order(
                 self.put_symbol,
                 self.put_token,
                 qty * self.lot_size,
                 put_transaction_type,
                 put_price,
-                order_tag=order_tag
+                order_tag=order_tag,
             )
             call_order_ids.append(call_order_id)
             put_order_ids.append(put_order_id)
         return call_order_ids, put_order_ids
 
 
 class SyntheticArbSystem:
@@ -820,18 +854,18 @@
         expiry,
         qty_in_lots,
         buy_strike,
         sell_strike,
         sleep_interval=1,
     ):
         ids_call_buy, ids_put_sell = place_synthetic_fut_order(
-            index, buy_strike, expiry, "BUY", qty_in_lots, 'MARKET'
+            index, buy_strike, expiry, "BUY", qty_in_lots, "MARKET"
         )
         ids_call_sell, ids_put_buy = place_synthetic_fut_order(
-            index, sell_strike, expiry, "SELL", qty_in_lots, 'MARKET'
+            index, sell_strike, expiry, "SELL", qty_in_lots, "MARKET"
         )
         ids = np.concatenate((ids_call_buy, ids_put_sell, ids_call_sell, ids_put_buy))
 
         sleep(sleep_interval)
         statuses = lookup_and_return("orderbook", "orderid", ids, "status")
 
         if any(statuses == "rejected"):
@@ -876,15 +910,18 @@
 
         if self.name == "BANKNIFTY":
             self.base = 100
             self.exchange_type = 1
         elif self.name == "NIFTY":
             self.base = 50
             self.exchange_type = 1
-        elif self.name in ["FINNIFTY", "MIDCPNIFTY"]:  # Finnifty and Midcpnifty temp fix
+        elif self.name in [
+            "FINNIFTY",
+            "MIDCPNIFTY",
+        ]:  # Finnifty and Midcpnifty temp fix
             self.base = 50
             self.exchange_type = 2
         else:
             self.base = get_base(self.name)
             self.exchange_type = 1
             logger.info(f"Base for {self.name} is {self.base}")
             # print(f"Base for {self.name} is {self.base}")
@@ -1067,23 +1104,24 @@
         return available_strikes
 
     def get_constituents(self, cutoff_pct=101):
         tickers, weights = get_index_constituents(self.name, cutoff_pct)
         return tickers, weights
 
     def log_combined_order(
-            self, strike=None,
-            call_strike=None,
-            put_strike=None,
-            expiry=None,
-            buy_or_sell=None,
-            call_price=None,
-            put_price=None,
-            order_tag=None):
-
+        self,
+        strike=None,
+        call_strike=None,
+        put_strike=None,
+        expiry=None,
+        buy_or_sell=None,
+        call_price=None,
+        put_price=None,
+        order_tag=None,
+    ):
         if strike is None and (call_strike is None or put_strike is None):
             raise Exception("Strike and call/put strike both not provided")
 
         if strike is not None and (call_strike is not None or put_strike is not None):
             raise Exception("Strike and call/put strike both provided")
 
         if strike is not None:
@@ -1255,18 +1293,32 @@
                 f"{order_prefix}ERROR. Order statuses uncertain for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s).",
                 self.webhook_url,
             )
             raise Exception("Order statuses uncertain")
 
     def place_synthetic_fut(
-            self, strike, expiry, buy_or_sell, quantity_in_lots, prices="LIMIT", stop_loss_order=False, order_tag=""
+        self,
+        strike,
+        expiry,
+        buy_or_sell,
+        quantity_in_lots,
+        prices="LIMIT",
+        stop_loss_order=False,
+        order_tag="",
     ):
         return place_synthetic_fut_order(
-            self.name, strike, expiry, buy_or_sell, quantity_in_lots, prices, stop_loss_order, order_tag
+            self.name,
+            strike,
+            expiry,
+            buy_or_sell,
+            quantity_in_lots,
+            prices,
+            stop_loss_order,
+            order_tag,
         )
 
     @time_the_function
     def find_equal_strike(
         self, exit_time, websocket, wait_for_equality, target_disparity, expiry=None
     ):
         expiry = expiry or self.current_expiry
@@ -1323,15 +1375,14 @@
 
         call_ltps, put_ltps = fetch_ltps(
             call_token_list, call_symbol_list, websocket
         ), fetch_ltps(put_token_list, put_symbol_list, websocket)
         disparities = compute_disparities(call_ltps, put_ltps)
 
         if wait_for_equality:
-
             last_print_time = currenttime()
             last_log_time = currenttime()
             last_notify_time = currenttime()
             print_interval = timedelta(seconds=0.05)
             log_interval = timedelta(minutes=1)
             notify_interval = timedelta(minutes=2)
 
@@ -1433,22 +1484,29 @@
             try:
                 with open(f"{obj.userId}_overnight_positions.json", "r") as f:
                     data = json.load(f)
                     return data
             except FileNotFoundError:
                 data = {}
                 notifier(
-                    "No positions found for overnight straddle. Creating new file.", self.webhook_url
+                    "No positions found for overnight straddle. Creating new file.",
+                    self.webhook_url,
                 )
                 with open(f"{obj.userId}_overnight_positions.json", "w") as f:
                     json.dump(data, f)
                 return data
             except Exception as e:
-                notifier(f"Error while reading overnight_positions.json: {e}", self.webhook_url)
-                logger.error(f"Error while reading positions.json", exc_info=(type(e), e, e.__traceback__))
+                notifier(
+                    f"Error while reading overnight_positions.json: {e}",
+                    self.webhook_url,
+                )
+                logger.error(
+                    f"Error while reading positions.json",
+                    exc_info=(type(e), e, e.__traceback__),
+                )
                 raise Exception("Error while reading positions.json")
 
         def save_data(data):
             with open(f"{obj.userId}_overnight_positions.json", "w") as f:
                 json.dump(data, f)
 
         avg_ltp = None
@@ -1472,15 +1530,17 @@
                 sleep(60)
             avg_ltp = np.mean(price_list)
 
         # Assigning vix
         vix = yf.Ticker("^INDIAVIX")
         vix = vix.fast_info["last_price"]
         if self.name in ["FINNIFTY", "BANKNIFTY"]:
-            beta = dm.get_summary_ratio(self.name, 'NIFTY')  # beta of the index vs nifty since vix is of nifty
+            beta = dm.get_summary_ratio(
+                self.name, "NIFTY"
+            )  # beta of the index vs nifty since vix is of nifty
             beta = 1.3 if beta is None else beta
             vix = vix * beta
 
         order_tag = "Overnight Short Straddle"
 
         weekend_in_expiry = check_for_weekend(self.current_expiry)
         ltp = avg_ltp if avg_ltp else self.fetch_ltp()
@@ -1491,33 +1551,37 @@
         call_iv, put_iv, iv = straddle_iv(
             call_ltp, put_ltp, ltp, sell_strike, timetoexpiry(self.current_expiry)
         )
         iv = iv * 100
 
         # This if-clause checks how far the expiry is
         if weekend_in_expiry:  # far from expiry
-
             if iv < vix * iv_threshold:
                 notifier(
                     f"{self.name} IV is too low compared to VIX - IV: {iv}, Vix: {vix}.",
                     self.webhook_url,
                 )
                 return
             else:
                 notifier(
-                    f"{self.name} IV is fine compared to VIX - IV: {iv}, Vix: {vix}.", self.webhook_url
+                    f"{self.name} IV is fine compared to VIX - IV: {iv}, Vix: {vix}.",
+                    self.webhook_url,
                 )
         elif (
             timetoexpiry(self.current_expiry, effective_time=True, in_days=True) < 2
         ):  # only exit
             sell_strike = None
-            notifier(f"{self.name} Only exiting current position. IV: {iv}, Vix: {vix}.", self.webhook_url)
+            notifier(
+                f"{self.name} Only exiting current position. IV: {iv}, Vix: {vix}.",
+                self.webhook_url,
+            )
         else:
             notifier(
-                f"{self.name} Rolling over overnight straddle - IV: {iv}, Vix: {vix}.", self.webhook_url
+                f"{self.name} Rolling over overnight straddle - IV: {iv}, Vix: {vix}.",
+                self.webhook_url,
             )
 
         trade_data = load_data()
         buy_strike = trade_data.get(self.name, None)
 
         # Checking if the buy strike is valid
         if (
@@ -1529,53 +1593,83 @@
             raise Exception(f"Invalid strike found for {self.name}.")
 
         # Placing orders
         if buy_strike is None and sell_strike is None:
             notifier(f"{self.name} No trade required.", self.webhook_url)
         elif sell_strike is None:  # only exiting current position
             notifier(
-                f"{self.name} Exiting current position on strike {buy_strike}.", self.webhook_url
+                f"{self.name} Exiting current position on strike {buy_strike}.",
+                self.webhook_url,
             )
             call_buy_avg, put_buy_avg = self.place_combined_order(
                 self.current_expiry,
                 "BUY",
                 quantity_in_lots,
                 strike=buy_strike,
                 return_avg_price=True,
                 order_tag=order_tag,
             )
-            self.log_combined_order(buy_strike, expiry=self.current_expiry, buy_or_sell="BUY", call_price=call_buy_avg,
-                                    put_price=put_buy_avg, order_tag=order_tag)
+            self.log_combined_order(
+                buy_strike,
+                expiry=self.current_expiry,
+                buy_or_sell="BUY",
+                call_price=call_buy_avg,
+                put_price=put_buy_avg,
+                order_tag=order_tag,
+            )
         elif buy_strike is None:  # only entering new position
             notifier(
-                f"{self.name} Entering new position on strike {sell_strike}.", self.webhook_url
+                f"{self.name} Entering new position on strike {sell_strike}.",
+                self.webhook_url,
             )
             call_sell_avg, put_sell_avg = self.place_combined_order(
                 self.current_expiry,
                 "SELL",
                 quantity_in_lots,
                 strike=sell_strike,
                 return_avg_price=True,
                 order_tag=order_tag,
             )
-            self.log_combined_order(sell_strike, expiry=self.current_expiry, buy_or_sell="SELL",
-                                    call_price=call_sell_avg, put_price=put_sell_avg, order_tag=order_tag)
+            self.log_combined_order(
+                sell_strike,
+                expiry=self.current_expiry,
+                buy_or_sell="SELL",
+                call_price=call_sell_avg,
+                put_price=put_sell_avg,
+                order_tag=order_tag,
+            )
         else:  # both entering and exiting positions
             if buy_strike == sell_strike:
-                notifier(f"{self.name} No trade required as strike is same.", self.webhook_url)
+                notifier(
+                    f"{self.name} No trade required as strike is same.",
+                    self.webhook_url,
+                )
                 call_ltp, put_ltp = fetch_straddle_price(
                     self.name, self.current_expiry, sell_strike
                 )
-                self.log_combined_order(buy_strike, expiry=self.current_expiry, buy_or_sell="BUY", call_price=call_ltp,
-                                        put_price=put_ltp, order_tag=order_tag)
-                self.log_combined_order(sell_strike, expiry=self.current_expiry, buy_or_sell="SELL",
-                                        call_price=call_ltp, put_price=put_ltp, order_tag=order_tag)
+                self.log_combined_order(
+                    buy_strike,
+                    expiry=self.current_expiry,
+                    buy_or_sell="BUY",
+                    call_price=call_ltp,
+                    put_price=put_ltp,
+                    order_tag=order_tag,
+                )
+                self.log_combined_order(
+                    sell_strike,
+                    expiry=self.current_expiry,
+                    buy_or_sell="SELL",
+                    call_price=call_ltp,
+                    put_price=put_ltp,
+                    order_tag=order_tag,
+                )
             else:
                 notifier(
-                    f"{self.name} Buying {buy_strike} and selling {sell_strike}.", self.webhook_url
+                    f"{self.name} Buying {buy_strike} and selling {sell_strike}.",
+                    self.webhook_url,
                 )
                 call_buy_avg, put_buy_avg = self.place_combined_order(
                     self.current_expiry,
                     "BUY",
                     quantity_in_lots,
                     strike=buy_strike,
                     return_avg_price=True,
@@ -1585,18 +1679,30 @@
                     self.current_expiry,
                     "SELL",
                     quantity_in_lots,
                     strike=sell_strike,
                     return_avg_price=True,
                     order_tag=order_tag,
                 )
-                self.log_combined_order(buy_strike, expiry=self.current_expiry, buy_or_sell="BUY",
-                                        call_price=call_buy_avg, put_price=put_buy_avg, order_tag=order_tag)
-                self.log_combined_order(sell_strike, expiry=self.current_expiry, buy_or_sell="SELL",
-                                        call_price=call_sell_avg, put_price=put_sell_avg, order_tag=order_tag)
+                self.log_combined_order(
+                    buy_strike,
+                    expiry=self.current_expiry,
+                    buy_or_sell="BUY",
+                    call_price=call_buy_avg,
+                    put_price=put_buy_avg,
+                    order_tag=order_tag,
+                )
+                self.log_combined_order(
+                    sell_strike,
+                    expiry=self.current_expiry,
+                    buy_or_sell="SELL",
+                    call_price=call_sell_avg,
+                    put_price=put_sell_avg,
+                    order_tag=order_tag,
+                )
 
         trade_data[self.name] = sell_strike
         save_data(trade_data)
 
     @log_errors
     def buy_weekly_hedge(
         self,
@@ -1625,17 +1731,24 @@
             strike=strike,
             call_strike=call_strike,
             put_strike=put_strike,
             order_tag="Weekly Hedge",
             return_avg_price=True,
         )
 
-        self.log_combined_order(strike=strike, call_strike=call_strike, put_strike=put_strike, expiry=self.next_expiry,
-                                buy_or_sell="BUY", call_price=call_buy_avg, put_price=put_buy_avg,
-                                order_tag="Weekly Hedge")
+        self.log_combined_order(
+            strike=strike,
+            call_strike=call_strike,
+            put_strike=put_strike,
+            expiry=self.next_expiry,
+            buy_or_sell="BUY",
+            call_price=call_buy_avg,
+            put_price=put_buy_avg,
+            order_tag="Weekly Hedge",
+        )
 
     @log_errors
     def intraday_straddle(
         self,
         quantity_in_lots,
         exit_time=(15, 28),
         websocket=None,
@@ -1745,24 +1858,24 @@
             call_sl_order_id = place_order(
                 call_symbol,
                 call_token,
                 quantity * self.lot_size,
                 "BUY",
                 call_avg_price * sl,
                 order_tag=stoploss_tag,
-                stop_loss_order=True
+                stop_loss_order=True,
             )
             put_sl_order_id = place_order(
                 put_symbol,
                 put_token,
                 quantity * self.lot_size,
                 "BUY",
                 put_avg_price * sl,
                 order_tag=stoploss_tag,
-                stop_loss_order=True
+                stop_loss_order=True,
             )
             call_stoploss_order_ids.append(call_sl_order_id)
             put_stoploss_order_ids.append(put_sl_order_id)
             sleep(0.3)
 
         orderbook = fetch_book("orderbook")
         call_sl_statuses = lookup_and_return(
@@ -1780,16 +1893,22 @@
             )
         else:
             notifier(
                 f"{self.name} stoploss orders not placed successfully", self.webhook_url
             )
             raise Exception("Stoploss orders not placed successfully")
 
-        self.log_combined_order(equal_strike, expiry=expiry, buy_or_sell="SELL", call_price=call_avg_price,
-                                put_price=put_avg_price, order_tag=order_tag)
+        self.log_combined_order(
+            equal_strike,
+            expiry=expiry,
+            buy_or_sell="SELL",
+            call_price=call_avg_price,
+            put_price=put_avg_price,
+            order_tag=order_tag,
+        )
         summary_message = "\n".join(
             f"{k}: {v}" for k, v in self.order_log[order_tag][0].items()
         )
 
         # Recording initial iv information
 
         traded_call_iv, traded_put_iv, traded_avg_iv = straddle_iv(
@@ -2017,18 +2136,15 @@
             """
 
             nonlocal orderbook, call_exit_price, put_exit_price, call_price, put_price, underlying_price
             nonlocal traded_call_iv, traded_put_iv, traded_avg_iv, call_iv, put_iv, avg_iv, entry_spot
 
             orderbook = fetch_orderbook_if_needed(data, refresh)
             triggered, complete = process_stop_loss_order_statuses(
-                orderbook,
-                order_ids,
-                context=f"SL: {side}",
-                notify_url=self.webhook_url
+                orderbook, order_ids, context=f"SL: {side}", notify_url=self.webhook_url
             )
 
             if not triggered and not complete:
                 return False, False
 
             # Checking if there has been an unjustified trigger of stoploss without much movement in the underlying
             # We will also use IV to check if the stoploss was justified or not
@@ -2202,16 +2318,15 @@
                     sl_order_id = place_order(
                         other_symbol,
                         other_token,
                         qty * self.lot_size,
                         "BUY",
                         other_avg_price,
                         order_tag=stoploss_tag,
-                        stop_loss_order=True
-
+                        stop_loss_order=True,
                     )
                     other_stoploss_order_ids.append(sl_order_id)
 
             # notifier(f'{self.name} {sl_type} stoploss triggered and completed.', self.webhook_url)
 
             refresh = True
             sleep(5)
@@ -2452,30 +2567,29 @@
 
     @log_errors
     def intraday_strangle(
         self,
         quantity_in_lots,
         call_strike_offset=0,
         put_strike_offset=0,
-        stop_loss='dynamic',
+        stop_loss="dynamic",
         call_stop_loss=None,
         put_stop_loss=None,
         exit_time=(15, 29),
         sleep_time=5,
         catch_trend=False,
         trend_qty_ratio=1,
         trend_strike_offset=0,
         trend_sl=0.003,
         disparity_threshold=np.inf,
         place_sl_orders=False,
         move_sl_to_cost=False,
         convert_to_butterfly=False,
-        shared_data=None
+        shared_data=None,
     ):
-
         """Intraday strangle strategy. Trades strangle with stop loss. All offsets are in percentage terms.
         Parameters
         ----------
         quantity_in_lots : int
             Quantity in lots
         call_strike_offset : float, optional
             Call strike offset in percentage terms, by default 0
@@ -2509,115 +2623,135 @@
             Convert to butterfly or not, by default False
         shared_data : SharedData class, optional
             shared data about client level orderbook and positions, by default None
         """
 
         @log_errors
         def position_monitor(info_dict):
-
             c_avg_price = info_dict["call_avg_price"]
             p_avg_price = info_dict["put_avg_price"]
             traded_strangle = info_dict["traded_strangle"]
 
             # Price deque
-            n_prices = max(int(30/sleep_time), 1)  # Hard coded 30-second price window for now
+            n_prices = max(
+                int(30 / sleep_time), 1
+            )  # Hard coded 30-second price window for now
             last_n_prices = {
-                "call": deque(maxlen=n_prices), "put": deque(maxlen=n_prices), "underlying": deque(maxlen=n_prices)
+                "call": deque(maxlen=n_prices),
+                "put": deque(maxlen=n_prices),
+                "underlying": deque(maxlen=n_prices),
             }
 
             # Conversion to butterfly
             ctb_notification_sent = False
             ctb_message = ""
             c_sl = call_stop_loss if call_stop_loss is not None else stop_loss
             p_sl = put_stop_loss if put_stop_loss is not None else stop_loss
             profit_if_call_sl = p_avg_price - (c_avg_price * (c_sl - 1))
             profit_if_put_sl = c_avg_price - (p_avg_price * (p_sl - 1))
             ctb_threshold = max(profit_if_call_sl, profit_if_put_sl)
 
             def process_ctb(profit_threshold):
-
                 hedge_call_strike = traded_strangle.call_strike + self.base
                 hedge_put_strike = traded_strangle.put_strike + self.base
-                h_strangle = Strangle(hedge_call_strike, hedge_put_strike, self.name, expiry)
+                h_strangle = Strangle(
+                    hedge_call_strike, hedge_put_strike, self.name, expiry
+                )
                 hedge_total_ltp = h_strangle.fetch_total_ltp()
 
-                hedge_profit = info_dict["total_avg_price"] - hedge_total_ltp - self.base
+                hedge_profit = (
+                    info_dict["total_avg_price"] - hedge_total_ltp - self.base
+                )
 
-                logging.info(f"{self.name} CTB threshold: {profit_threshold}, Hedge working: {hedge_profit}")
+                logging.info(
+                    f"{self.name} CTB threshold: {profit_threshold}, Hedge working: {hedge_profit}"
+                )
 
                 if hedge_profit >= profit_threshold:
                     return h_strangle
                 else:
                     return None
 
             last_print_time = currenttime()
             last_log_time = currenttime()
             last_notify_time = currenttime()
             print_interval = timedelta(seconds=5)
             log_interval = timedelta(minutes=60)
             notify_interval = timedelta(minutes=180)
 
             while not info_dict["trade_complete"]:
-
                 # Fetching prices
                 spot_price = self.fetch_ltp()
                 c_ltp, p_ltp = traded_strangle.fetch_ltp()
                 info_dict["underlying_ltp"] = spot_price
                 info_dict["call_ltp"] = c_ltp
                 info_dict["put_ltp"] = p_ltp
                 last_n_prices["call"].append(c_ltp)
                 last_n_prices["put"].append(p_ltp)
                 last_n_prices["underlying"].append(spot_price)
-                c_ltp_avg = sum(last_n_prices["call"])/len(last_n_prices["call"]) if last_n_prices["call"] else c_ltp
-                p_ltp_avg = sum(last_n_prices["put"])/len(last_n_prices["put"]) if last_n_prices["put"] else p_ltp
-                spot_price_avg = sum(last_n_prices["underlying"])/len(last_n_prices["underlying"]) \
-                    if last_n_prices["underlying"] else spot_price
+                c_ltp_avg = (
+                    sum(last_n_prices["call"]) / len(last_n_prices["call"])
+                    if last_n_prices["call"]
+                    else c_ltp
+                )
+                p_ltp_avg = (
+                    sum(last_n_prices["put"]) / len(last_n_prices["put"])
+                    if last_n_prices["put"]
+                    else p_ltp
+                )
+                spot_price_avg = (
+                    sum(last_n_prices["underlying"]) / len(last_n_prices["underlying"])
+                    if last_n_prices["underlying"]
+                    else spot_price
+                )
                 info_dict["call_ltp_avg"] = c_ltp_avg
                 info_dict["put_ltp_avg"] = p_ltp_avg
                 info_dict["underlying_ltp_avg"] = spot_price_avg
 
                 # Calculate IV
                 call_iv, put_iv, avg_iv = strangle_iv(
                     callprice=c_ltp,
                     putprice=p_ltp,
                     callstrike=traded_strangle.call_strike,
                     putstrike=traded_strangle.put_strike,
                     spot=spot_price,
-                    timeleft=timetoexpiry(expiry)
+                    timeleft=timetoexpiry(expiry),
                 )
                 info_dict["call_iv"] = call_iv
                 info_dict["put_iv"] = put_iv
                 info_dict["avg_iv"] = avg_iv
 
                 # Calculate mtm price
-                call_exit_price = info_dict.get('call_exit_price', c_ltp)
-                put_exit_price = info_dict.get('put_exit_price', p_ltp)
+                call_exit_price = info_dict.get("call_exit_price", c_ltp)
+                put_exit_price = info_dict.get("put_exit_price", p_ltp)
                 mtm_price = call_exit_price + put_exit_price
 
                 # Calculate profit
                 profit_in_pts = (c_avg_price + p_avg_price) - mtm_price
                 profit_in_rs = profit_in_pts * self.lot_size * quantity_in_lots
                 info_dict["profit_in_pts"] = profit_in_pts
                 info_dict["profit_in_rs"] = profit_in_rs
 
                 # Conversion to butterfly working
                 if (
-                        not (info_dict["call_sl"] or info_dict["put_sl"])
-                        and info_dict["time_left_day_start"] * 365 < 1
-                        and convert_to_butterfly
-                        and not ctb_notification_sent
+                    not (info_dict["call_sl"] or info_dict["put_sl"])
+                    and info_dict["time_left_day_start"] * 365 < 1
+                    and convert_to_butterfly
+                    and not ctb_notification_sent
                 ):
                     try:
                         ctb_hedge = process_ctb(ctb_threshold)
                         if ctb_hedge is not None:
                             notifier(
                                 f"{self.name} Convert to butterfly triggered\n",
                                 self.webhook_url,
                             )
-                            info_dict["exit_triggers"].update({"convert_to_butterfly": True})
+                            info_dict["exit_triggers"].update(
+                                {"convert_to_butterfly": True}
+                            )
                             ctb_message = f"Hedged with: {ctb_hedge}\n"
                             info_dict["ctb_hedge"] = ctb_hedge
                             ctb_notification_sent = True
                     except Exception as _e:
                         logging.info(f"Error in process_ctb: {_e}")
 
                 message = (
@@ -2631,16 +2765,15 @@
                     f"MTM Price: {mtm_price}\n"
                     f"Call last n avg: {c_ltp_avg}\n"
                     f"Put last n avg: {p_ltp_avg}\n"
                     f"IVs: {call_iv}, {put_iv}, {avg_iv}\n"
                     f"Call SL: {info_dict['call_sl']}\n"
                     f"Put SL: {info_dict['put_sl']}\n"
                     f"Profit Pts: {info_dict['profit_in_pts']:.2f}\n"
-                    f"Profit: {info_dict['profit_in_rs']:.2f}\n"
-                    + ctb_message
+                    f"Profit: {info_dict['profit_in_rs']:.2f}\n" + ctb_message
                 )
                 if currenttime() - last_print_time > print_interval:
                     print(message)
                     last_print_time = currenttime()
                 if currenttime() - last_log_time > log_interval:
                     logger.info(message)
                     last_log_time = currenttime()
@@ -2651,44 +2784,48 @@
 
         def get_range_of_strangles(c_strike, p_strike, exp, range_of_strikes=4):
             if range_of_strikes % 2 != 0:
                 range_of_strikes += 1
             c_strike_range = np.arange(
                 c_strike - (range_of_strikes / 2) * self.base,
                 c_strike + (range_of_strikes / 2) * self.base + self.base,
-                self.base
+                self.base,
             )
             if c_strike == p_strike:
                 return [Straddle(strike, self.name, exp) for strike in c_strike_range]
             else:
                 p_strike_ranges = np.arange(
-                        p_strike - (range_of_strikes/2)*self.base,
-                        p_strike + (range_of_strikes/2)*self.base + self.base,
-                        self.base
+                    p_strike - (range_of_strikes / 2) * self.base,
+                    p_strike + (range_of_strikes / 2) * self.base + self.base,
+                    self.base,
                 )
                 pairs = itertools.product(c_strike_range, p_strike_ranges)
                 return [Strangle(pair[0], pair[1], self.name, exp) for pair in pairs]
 
         @log_errors
         def trend_catcher(info_dict, sl_type, qty_ratio, sl, strike_offset):
-
-            offset = 1-strike_offset if sl_type == "call" else 1+strike_offset
+            offset = 1 - strike_offset if sl_type == "call" else 1 + strike_offset
 
             spot_price = info_dict["underlying_ltp"]
 
             # Setting up the trend option
             strike = spot_price * offset
             strike = findstrike(strike, self.base)
             opt_type = "PE" if sl_type == "call" else "CE"
             qty_in_lots = max(int(quantity_in_lots * qty_ratio), 1)
             trend_option = Option(strike, opt_type, self.name, expiry)
 
             # Placing the trend option order
             place_option_order_and_notify(
-                trend_option, "SELL", qty_in_lots, "LIMIT", "Intraday Strangle Trend Catcher", self.webhook_url
+                trend_option,
+                "SELL",
+                qty_in_lots,
+                "LIMIT",
+                "Intraday Strangle Trend Catcher",
+                self.webhook_url,
             )
 
             # Setting up the stop loss
             sl_multiplier = 1 - sl if sl_type == "call" else 1 + sl
             sl_price = spot_price * sl_multiplier
             trend_sl_hit = False
 
@@ -2697,178 +2834,247 @@
                 + f"Placed {qty_in_lots} lots of {strike} {opt_type} at {trend_option.fetch_ltp()}. "
                 + f"Stoploss price: {sl_price}, Underlying Price: {spot_price}",
                 self.webhook_url,
             )
 
             last_print_time = currenttime()
             print_interval = timedelta(seconds=10)
-            while all([currenttime().time() < time(*exit_time), not info_dict["trade_complete"]]):
+            while all(
+                [
+                    currenttime().time() < time(*exit_time),
+                    not info_dict["trade_complete"],
+                ]
+            ):
                 spot_price = info_dict["underlying_ltp"]
                 spot_price_avg = info_dict["underlying_ltp_avg"]
-                trend_sl_hit = spot_price_avg < sl_price if sl_type == "call" else spot_price_avg > sl_price
+                trend_sl_hit = (
+                    spot_price_avg < sl_price
+                    if sl_type == "call"
+                    else spot_price_avg > sl_price
+                )
                 if trend_sl_hit:
                     break
                 sleep(sleep_time)
                 if currenttime() - last_print_time > print_interval:
                     last_print_time = currenttime()
                     print(
                         f"{self.name} {sl_type} trend catcher running\n"
                         + f"Stoploss price: {sl_price}, Underlying price: {spot_price}\n"
                         + f"Underlying price avg: {spot_price_avg}, Stoploss hit: {trend_sl_hit}\n"
                     )
 
             if trend_sl_hit:
                 notifier(
-                    f"{self.name} strangle {sl_type} trend catcher stoploss hit.", self.webhook_url
+                    f"{self.name} strangle {sl_type} trend catcher stoploss hit.",
+                    self.webhook_url,
                 )
             else:
                 notifier(
-                    f"{self.name} strangle {sl_type} trend catcher exiting.", self.webhook_url
+                    f"{self.name} strangle {sl_type} trend catcher exiting.",
+                    self.webhook_url,
                 )
 
             # Buying the trend option back
             place_option_order_and_notify(
-                trend_option, "BUY", qty_in_lots, "LIMIT", "Intraday Strangle Trend Catcher", self.webhook_url
+                trend_option,
+                "BUY",
+                qty_in_lots,
+                "LIMIT",
+                "Intraday Strangle Trend Catcher",
+                self.webhook_url,
             )
 
         def justify_stop_loss(info_dict, side):
-
             entry_spot = info_dict.get("spot_at_entry")
             current_spot = info_dict.get("underlying_ltp")
 
             # If the spot has moved in the direction of stop loss
             time_left_day_start = info_dict.get("time_left_day_start")
             time_left_now = timetoexpiry(expiry)
-            time_delta = (time_left_day_start - time_left_now)*525600
+            time_delta = (time_left_day_start - time_left_now) * 525600
             time_delta = int(time_delta)
             estimated_movement = bs.target_movement(
                 side,
                 info_dict.get(f"{side}_avg_price"),
                 info_dict.get(f"{side}_stop_loss_price"),
                 entry_spot,
-                info_dict.get("traded_strangle").call_strike if side == "call" else info_dict.get("traded_strangle").put_strike,
+                info_dict.get("traded_strangle").call_strike
+                if side == "call"
+                else info_dict.get("traded_strangle").put_strike,
                 time_left_day_start,
-                time_delta
+                time_delta,
             )
             actual_movement = (current_spot - entry_spot) / entry_spot
             difference_in_sign = np.sign(estimated_movement) != np.sign(actual_movement)
             lack_of_movement = abs(actual_movement) < 0.8 * abs(estimated_movement)
             # 0.8 above is a magic number TODO: Remove magic number and find a better way to check for lack of movement
             if difference_in_sign or lack_of_movement:
                 if not info_dict.get(f"{side}_sl_check_notification_sent"):
-                    message = f'{self.name} strangle {side} stop loss appears to be unjustified. ' \
-                              f'Estimated movement: {estimated_movement}, Actual movement: {actual_movement}'
+                    message = (
+                        f"{self.name} strangle {side} stop loss appears to be unjustified. "
+                        f"Estimated movement: {estimated_movement}, Actual movement: {actual_movement}"
+                    )
                     notifier(message, self.webhook_url)
                     info_dict[f"{side}_sl_check_notification_sent"] = True
                 return False
             else:
-                message = f"{self.name} strangle {side} stop loss triggered. " \
-                          f"Estimated movement: {estimated_movement}, Actual movement: {actual_movement}"
+                message = (
+                    f"{self.name} strangle {side} stop loss triggered. "
+                    f"Estimated movement: {estimated_movement}, Actual movement: {actual_movement}"
+                )
                 notifier(message, self.webhook_url)
                 return True
 
         def check_for_stop_loss(info_dict, side, refresh_orderbook=False):
-
             """Check for stop loss."""
 
             stop_loss_order_ids = info_dict.get(f"{side}_stop_loss_order_ids")
 
             if stop_loss_order_ids is None:  # If stop loss order ids are not provided
                 avg_price = info_dict.get(f"{side}_ltp_avg")
                 stop_loss_price = info_dict.get(f"{side}_stop_loss_price")
                 stop_loss_triggered = avg_price > stop_loss_price
                 if stop_loss_triggered:
                     stop_loss_justified = justify_stop_loss(info_dict, side)
                     if stop_loss_justified:
                         info_dict[f"{side}_sl"] = True
 
             else:  # If stop loss order ids are provided
-                orderbook = fetch_orderbook_if_needed(shared_data, refresh_needed=refresh_orderbook)
+                orderbook = fetch_orderbook_if_needed(
+                    shared_data, refresh_needed=refresh_orderbook
+                )
                 orders_triggered, orders_complete = process_stop_loss_order_statuses(
-                    orderbook, stop_loss_order_ids, context=side, notify_url=self.webhook_url
+                    orderbook,
+                    stop_loss_order_ids,
+                    context=side,
+                    notify_url=self.webhook_url,
                 )
                 if orders_triggered:
                     justify_stop_loss(info_dict, side)
                     info_dict[f"{side}_sl"] = True
                 if not orders_complete:
                     info_dict[f"{side}_sl_order_ids"] = None
 
         def process_stop_loss(info_dict, sl_type):
-
-            if info_dict["call_sl"] and info_dict["put_sl"]:  # Check to avoid double processing
+            if (
+                info_dict["call_sl"] and info_dict["put_sl"]
+            ):  # Check to avoid double processing
                 return
 
             traded_strangle = info_dict["traded_strangle"]
             other_side = "call" if sl_type == "put" else "put"
 
             # Buying the stop loss option back if it is not already bought
             if info_dict[f"{sl_type}_sl_order_ids"] is None:
-                option_to_buy = traded_strangle.call_option if sl_type == "call" else traded_strangle.put_option
+                option_to_buy = (
+                    traded_strangle.call_option
+                    if sl_type == "call"
+                    else traded_strangle.put_option
+                )
                 exit_price = place_option_order_and_notify(
-                    option_to_buy, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
+                    option_to_buy,
+                    "BUY",
+                    quantity_in_lots,
+                    "LIMIT",
+                    order_tag,
+                    self.webhook_url,
                 )
             else:
-                orderbook = fetch_book('orderbook')
+                orderbook = fetch_book("orderbook")
                 exit_price = (
-                    lookup_and_return(orderbook, "orderid", info_dict[f"{sl_type}_sl_order_ids"], "averageprice")
+                    lookup_and_return(
+                        orderbook,
+                        "orderid",
+                        info_dict[f"{sl_type}_sl_order_ids"],
+                        "averageprice",
+                    )
                     .astype(float)
                     .mean()
                 )
-            info_dict[f'{sl_type}_exit_price'] = exit_price
+            info_dict[f"{sl_type}_exit_price"] = exit_price
 
             if move_sl_to_cost:
-                info_dict[f"{other_side}_stop_loss_price"] = info_dict[f"{other_side}_avg_price"]
+                info_dict[f"{other_side}_stop_loss_price"] = info_dict[
+                    f"{other_side}_avg_price"
+                ]
                 if info_dict[f"{other_side}_stop_loss_order_ids"] is not None:
-                    cancel_pending_orders(info_dict[f"{other_side}_stop_loss_order_ids"], "STOPLOSS")
+                    cancel_pending_orders(
+                        info_dict[f"{other_side}_stop_loss_order_ids"], "STOPLOSS"
+                    )
                     option_to_repair = (
-                        traded_strangle.call_option if other_side == "call" else traded_strangle.put_option
+                        traded_strangle.call_option
+                        if other_side == "call"
+                        else traded_strangle.put_option
                     )
-                    info_dict[f"{other_side}_stop_loss_order_ids"] = place_option_order_and_notify(
+                    info_dict[
+                        f"{other_side}_stop_loss_order_ids"
+                    ] = place_option_order_and_notify(
                         instrument=option_to_repair,
                         action="BUY",
                         qty_in_lots=quantity_in_lots,
                         prices=info_dict[f"{other_side}_stop_loss_price"],
                         order_tag=f"{other_side} SL Strangle",
                         webhook_url=self.webhook_url,
                         stop_loss_order=True,
                         target_status="trigger pending",
-                        return_avg_price=False
+                        return_avg_price=False,
                     )
 
             # Starting the trend catcher
             if catch_trend:
                 trend_thread = Thread(
                     target=trend_catcher,
-                    args=(info_dict, sl_type, trend_qty_ratio, trend_sl, trend_strike_offset),
+                    args=(
+                        info_dict,
+                        sl_type,
+                        trend_qty_ratio,
+                        trend_sl,
+                        trend_strike_offset,
+                    ),
                 )
                 trend_thread.start()
 
             refresh_orderbook = True
             # Wait for exit or other stop loss to hit
             while all([currenttime().time() < time(*exit_time)]):
-                check_for_stop_loss(info_dict, other_side, refresh_orderbook=refresh_orderbook)
+                check_for_stop_loss(
+                    info_dict, other_side, refresh_orderbook=refresh_orderbook
+                )
                 if info_dict[f"{other_side}_sl"]:
                     if info_dict[f"{other_side}_sl_order_ids"] is None:
                         other_sl_option = (
-                            traded_strangle.call_option if other_side == "call" else traded_strangle.put_option
+                            traded_strangle.call_option
+                            if other_side == "call"
+                            else traded_strangle.put_option
+                        )
+                        notifier(
+                            f"{self.name} strangle {other_side} stop loss hit.",
+                            self.webhook_url,
                         )
-                        notifier(f'{self.name} strangle {other_side} stop loss hit.', self.webhook_url)
                         other_exit_price = place_option_order_and_notify(
-                            other_sl_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
+                            other_sl_option,
+                            "BUY",
+                            quantity_in_lots,
+                            "LIMIT",
+                            order_tag,
+                            self.webhook_url,
                         )
                     else:
-                        orderbook = fetch_book('orderbook')
+                        orderbook = fetch_book("orderbook")
                         other_exit_price = (
                             lookup_and_return(
-                                orderbook, "orderid", info_dict[f"{other_side}_sl_order_ids"], "averageprice"
+                                orderbook,
+                                "orderid",
+                                info_dict[f"{other_side}_sl_order_ids"],
+                                "averageprice",
                             )
                             .astype(float)
                             .mean()
                         )
-                    info_dict[f'{other_side}_exit_price'] = other_exit_price
+                    info_dict[f"{other_side}_exit_price"] = other_exit_price
                     break
                 refresh_orderbook = False
                 sleep(1)
 
         # Entering the main function
 
         # Setting strikes and expiry
@@ -2876,102 +3082,126 @@
         underlying_ltp = self.fetch_ltp()
         temp_call_strike = underlying_ltp * (1 + call_strike_offset)
         temp_put_strike = underlying_ltp * (1 - put_strike_offset)
         temp_call_strike = findstrike(temp_call_strike, self.base)
         temp_put_strike = findstrike(temp_put_strike, self.base)
         expiry = self.current_expiry
 
-        prospective_strangles = get_range_of_strangles(temp_call_strike, temp_put_strike, expiry, range_of_strikes=4)
+        prospective_strangles = get_range_of_strangles(
+            temp_call_strike, temp_put_strike, expiry, range_of_strikes=4
+        )
         logger.info(f"{self.name} prospective strangles: {prospective_strangles}")
 
         # Placing the main order
         strangle = most_equal_strangle(
             *prospective_strangles,
             disparity_threshold=disparity_threshold,
-            exit_time=(datetime.combine(datetime.now().date(), time(*exit_time)) - timedelta(minutes=5)).time(),
+            exit_time=(
+                datetime.combine(datetime.now().date(), time(*exit_time))
+                - timedelta(minutes=5)
+            ).time(),
         )
         if strangle is None:
             notifier(
-                f"{self.name} no strangle found within disparity threshold {disparity_threshold}", self.webhook_url
+                f"{self.name} no strangle found within disparity threshold {disparity_threshold}",
+                self.webhook_url,
             )
             return
         call_ltp, put_ltp = strangle.fetch_ltp()
         call_avg_price, put_avg_price = place_option_order_and_notify(
-            strangle, "SELL", quantity_in_lots, "LIMIT", order_tag, self.webhook_url, return_avg_price=True
+            strangle,
+            "SELL",
+            quantity_in_lots,
+            "LIMIT",
+            order_tag,
+            self.webhook_url,
+            return_avg_price=True,
         )
         total_avg_price = call_avg_price + put_avg_price
 
         # Setting stop loss
         stop_loss_dict = {
             "fixed": {"BANKNIFTY": 1.7, "NIFTY": 1.5},
-            "dynamic": {"BANKNIFTY": 1.7, "NIFTY": 1.5}
+            "dynamic": {"BANKNIFTY": 1.7, "NIFTY": 1.5},
         }
 
         if isinstance(stop_loss, str):
             if stop_loss == "dynamic" and timetoexpiry(expiry, in_days=True) < 1:
                 stop_loss = 1.7
             else:
                 stop_loss = stop_loss_dict[stop_loss].get(self.name, 1.6)
         else:
             stop_loss = stop_loss
 
-        call_stop_loss_price = call_avg_price * call_stop_loss if call_stop_loss else call_avg_price * stop_loss
-        put_stop_loss_price = put_avg_price * put_stop_loss if put_stop_loss else put_avg_price * stop_loss
+        call_stop_loss_price = (
+            call_avg_price * call_stop_loss
+            if call_stop_loss
+            else call_avg_price * stop_loss
+        )
+        put_stop_loss_price = (
+            put_avg_price * put_stop_loss
+            if put_stop_loss
+            else put_avg_price * stop_loss
+        )
 
         # Logging information and sending notification
         self.log_combined_order(
             call_strike=strangle.call_strike,
             put_strike=strangle.put_strike,
             expiry=expiry,
             buy_or_sell="SELL",
             call_price=call_avg_price,
             put_price=put_avg_price,
-            order_tag=order_tag
+            order_tag=order_tag,
         )
 
         summary_message = "\n".join(
             f"{k}: {v}" for k, v in self.order_log[order_tag][-1].items()
         )
 
         traded_call_iv, traded_put_iv, traded_avg_iv = strangle_iv(
             callprice=call_avg_price,
             putprice=put_avg_price,
             callstrike=strangle.call_strike,
             putstrike=strangle.put_strike,
             spot=underlying_ltp,
-            timeleft=timetoexpiry(expiry)
+            timeleft=timetoexpiry(expiry),
         )
 
         time_left_at_trade = timetoexpiry(expiry)
-        summary_message += f"\nTraded IVs: {traded_call_iv}, {traded_put_iv}, {traded_avg_iv}"
-        summary_message += f"\nCall SL: {call_stop_loss_price}, Put SL: {put_stop_loss_price}"
+        summary_message += (
+            f"\nTraded IVs: {traded_call_iv}, {traded_put_iv}, {traded_avg_iv}"
+        )
+        summary_message += (
+            f"\nCall SL: {call_stop_loss_price}, Put SL: {put_stop_loss_price}"
+        )
         notifier(summary_message, self.webhook_url)
 
         if place_sl_orders:
             call_stop_loss_order_ids = place_option_order_and_notify(
                 instrument=strangle.call_option,
                 action="BUY",
                 qty_in_lots=quantity_in_lots,
                 prices=call_stop_loss_price,
                 order_tag="Call SL Strangle",
                 webhook_url=self.webhook_url,
                 stop_loss_order=True,
                 target_status="trigger pending",
-                return_avg_price=False
+                return_avg_price=False,
             )
             put_stop_loss_order_ids = place_option_order_and_notify(
                 instrument=strangle.put_option,
                 action="BUY",
                 qty_in_lots=quantity_in_lots,
                 prices=put_stop_loss_price,
                 order_tag="Put SL Strangle",
                 webhook_url=self.webhook_url,
                 stop_loss_order=True,
                 target_status="trigger pending",
-                return_avg_price=False
+                return_avg_price=False,
             )
         else:
             call_stop_loss_order_ids = None
             put_stop_loss_order_ids = None
 
         # Setting up shared info dict
         shared_info_dict = {
@@ -2998,80 +3228,110 @@
             "put_sl": False,
             "exit_triggers": {"convert_to_butterfly": False},
             "trade_complete": False,
             "call_sl_check_notification_sent": False,
             "put_sl_check_notification_sent": False,
         }
 
-        position_monitor_thread = Thread(target=position_monitor, args=(shared_info_dict,))
+        position_monitor_thread = Thread(
+            target=position_monitor, args=(shared_info_dict,)
+        )
         position_monitor_thread.start()
         sleep(3)  # To ensure that the position monitor thread has started
 
         refresh_book = True
 
         # Wait for exit time or both stop losses to hit (Main Loop)
         while all([currenttime().time() < time(*exit_time)]):
-            check_for_stop_loss(shared_info_dict, 'call', refresh_orderbook=refresh_book)
+            check_for_stop_loss(
+                shared_info_dict, "call", refresh_orderbook=refresh_book
+            )
             if shared_info_dict["call_sl"]:
                 process_stop_loss(shared_info_dict, "call")
                 break
-            check_for_stop_loss(shared_info_dict, 'put')
+            check_for_stop_loss(shared_info_dict, "put")
             if shared_info_dict["put_sl"]:
                 process_stop_loss(shared_info_dict, "put")
                 break
             refresh_book = False
             sleep(1)
 
         # Out of the while loop, so exit time reached or both stop losses hit
 
         # If we are hedged then wait till exit time
         # noinspection PyTypeChecker
         if shared_info_dict["exit_triggers"]["convert_to_butterfly"]:
             hedge_strangle = shared_info_dict["ctb_hedge"]
             place_option_order_and_notify(
-                hedge_strangle, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url, return_avg_price=False
+                hedge_strangle,
+                "BUY",
+                quantity_in_lots,
+                "LIMIT",
+                order_tag,
+                self.webhook_url,
+                return_avg_price=False,
             )
-            if shared_info_dict["call_stop_loss_order_ids"] and shared_info_dict["put_stop_loss_order_ids"]:
+            if (
+                shared_info_dict["call_stop_loss_order_ids"]
+                and shared_info_dict["put_stop_loss_order_ids"]
+            ):
                 cancel_pending_orders(
-                    shared_info_dict["call_stop_loss_order_ids"] + shared_info_dict["put_stop_loss_order_ids"]
+                    shared_info_dict["call_stop_loss_order_ids"]
+                    + shared_info_dict["put_stop_loss_order_ids"]
                 )
             notifier(f"{self.name}: Converted to butterfly", self.webhook_url)
             while currenttime().time() < time(*exit_time):
                 sleep(3)
 
         call_sl = shared_info_dict["call_sl"]
         put_sl = shared_info_dict["put_sl"]
 
         if not call_sl and not put_sl:
             # Both stop losses not hit
             if shared_info_dict["time_left_day_start"] * 365 < 1:  # expiry day
-                call_exit_avg_price, put_exit_avg_price = shared_info_dict["call_ltp"], shared_info_dict["put_ltp"]
+                call_exit_avg_price, put_exit_avg_price = (
+                    shared_info_dict["call_ltp"],
+                    shared_info_dict["put_ltp"],
+                )
             else:
                 call_exit_avg_price, put_exit_avg_price = place_option_order_and_notify(
-                    strangle, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url, return_avg_price=True
+                    strangle,
+                    "BUY",
+                    quantity_in_lots,
+                    "LIMIT",
+                    order_tag,
+                    self.webhook_url,
+                    return_avg_price=True,
                 )
-            shared_info_dict['call_exit_price'] = call_exit_avg_price
-            shared_info_dict['put_exit_price'] = put_exit_avg_price
+            shared_info_dict["call_exit_price"] = call_exit_avg_price
+            shared_info_dict["put_exit_price"] = put_exit_avg_price
 
         elif (call_sl or put_sl) and not (call_sl and put_sl):  # Only one stop loss hit
             exit_option = "put" if call_sl else "call"
             if shared_info_dict["time_left_day_start"] * 365 < 1:  # expiry day
                 non_sl_exit_price = shared_info_dict[f"{exit_option}_ltp"]
             else:
                 exit_option = strangle.put_option if call_sl else strangle.call_option
                 non_sl_exit_price = place_option_order_and_notify(
-                    exit_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
+                    exit_option,
+                    "BUY",
+                    quantity_in_lots,
+                    "LIMIT",
+                    order_tag,
+                    self.webhook_url,
                 )
             shared_info_dict[f"{exit_option}_exit_price"] = non_sl_exit_price
 
         else:  # Both stop losses hit
             pass
 
         # Calculate profit
-        total_exit_price = shared_info_dict["call_exit_price"] + shared_info_dict["put_exit_price"]
+        total_exit_price = (
+            shared_info_dict["call_exit_price"] + shared_info_dict["put_exit_price"]
+        )
         exit_message = (
             f"{self.name} strangle exited.\n"
             f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
             f"Underlying LTP: {shared_info_dict['underlying_ltp']}\n"
             f"Call Price: {shared_info_dict['call_ltp']}\n"
             f"Put Price: {shared_info_dict['put_ltp']}\n"
             f"Call SL: {shared_info_dict['call_sl']}\n"
@@ -3100,35 +3360,40 @@
         notifier(exit_message, self.webhook_url)
         shared_info_dict["trade_complete"] = True
         position_monitor_thread.join()
         return shared_info_dict
 
     @log_errors
     def intraday_trend(
-            self,
-            quantity_in_lots,
-            start_time=(9, 15, 58),
-            exit_time=(15, 27),
-            sleep_time=5,
-            threshold_movement=None,
-            minutes_to_avg=45,
-            beta=0.8,
-            max_entries=3
+        self,
+        quantity_in_lots,
+        start_time=(9, 15, 58),
+        exit_time=(15, 27),
+        sleep_time=5,
+        threshold_movement=None,
+        minutes_to_avg=45,
+        beta=0.8,
+        max_entries=3,
     ):
-
         while currenttime().time() < time(*start_time):
             print(f"{self.name} trender sleeping till {start_time}")
             sleep(1)
 
         open_price = self.fetch_ltp()
-        threshold_movement = threshold_movement or (get_current_vix() * (beta or 1)) / 48
+        threshold_movement = (
+            threshold_movement or (get_current_vix() * (beta or 1)) / 48
+        )
 
         exit_time = time(*exit_time)
-        scan_end_time = (datetime.combine(currenttime().date(), exit_time) - timedelta(minutes=10)).time()
-        price_boundaries = [open_price * (1 + ((-1) ** i) * threshold_movement / 100) for i in range(2)]
+        scan_end_time = (
+            datetime.combine(currenttime().date(), exit_time) - timedelta(minutes=10)
+        ).time()
+        price_boundaries = [
+            open_price * (1 + ((-1) ** i) * threshold_movement / 100) for i in range(2)
+        ]
 
         # Price deque
         n_prices = max(int(minutes_to_avg / sleep_time), 1)
         price_deque = deque(maxlen=n_prices)
 
         notifier(
             f"{self.name} trender starting with {threshold_movement:0.2f} threshold movement\n"
@@ -3137,57 +3402,76 @@
             self.webhook_url,
         )
 
         entries = 0
         last_print_time = currenttime()
         movement = 0
         while entries < max_entries and currenttime().time() < exit_time:
-
             # Scan for entry condition
-            while (abs(movement) < threshold_movement) and (currenttime().time() < scan_end_time):
-
+            notifier(
+                f"{self.name} trender {entries+1} scanning for entry condition.",
+                self.webhook_url,
+            )
+            while (abs(movement) < threshold_movement) and (
+                currenttime().time() < scan_end_time
+            ):
                 ltp = self.fetch_ltp()
                 price_deque.append(ltp)
-                avg_price = (sum(price_deque) / len(price_deque)) if price_deque else ltp
+                avg_price = (
+                    (sum(price_deque) / len(price_deque)) if price_deque else ltp
+                )
                 movement = (avg_price - open_price) / open_price * 100
 
                 if currenttime() > last_print_time + timedelta(minutes=1):
                     print(f"{self.name} trender: {movement:0.2f} movement.")
                     last_print_time = currenttime()
                 sleep(sleep_time)
 
             if currenttime().time() > scan_end_time:
-                notifier(f"{self.name} trender {entries+1} exiting due to time.", self.webhook_url)
+                notifier(
+                    f"{self.name} trender {entries+1} exiting due to time.",
+                    self.webhook_url,
+                )
                 return
 
             # Entry condition met taking position
             price = self.fetch_ltp()
             atm_strike = findstrike(price, self.base)
             position = "BUY" if movement > 0 else "SELL"
-            atm_synthetic_fut = SyntheticFuture(atm_strike, self.name, self.current_expiry)
+            atm_synthetic_fut = SyntheticFuture(
+                atm_strike, self.name, self.current_expiry
+            )
             stop_loss_price = price * (0.997 if position == "BUY" else 1.003)
             stop_loss_hit = False
             notifier(
                 f"{self.name} {position} trender triggered with {movement:0.2f} movement. {self.name} at {price}. "
                 f"Stop loss at {stop_loss_price}.",
                 self.webhook_url,
             )
             place_option_order_and_notify(
-                atm_synthetic_fut, position, quantity_in_lots, "LIMIT", f"{self.name} trender", self.webhook_url
+                atm_synthetic_fut,
+                position,
+                quantity_in_lots,
+                "LIMIT",
+                f"{self.name} trender",
+                self.webhook_url,
             )
 
             # Tracking position
             while currenttime().time() < exit_time and not stop_loss_hit:
-
                 ltp = self.fetch_ltp()
                 price_deque.append(ltp)
                 avg_price = sum(price_deque) / len(price_deque) if price_deque else ltp
                 movement = (avg_price - open_price) / open_price * 100
 
-                stop_loss_hit = (avg_price < stop_loss_price) if position == "BUY" else (avg_price > stop_loss_price)
+                stop_loss_hit = (
+                    (avg_price < stop_loss_price)
+                    if position == "BUY"
+                    else (avg_price > stop_loss_price)
+                )
                 sleep(sleep_time)
 
             # Exit condition met exiting position (stop loss or time)
             stop_loss_message = f"Trender stop loss hit. " if stop_loss_hit else ""
             notifier(
                 f"{stop_loss_message}{self.name} trender {entries+1} exiting. {self.name} at {self.fetch_ltp()}.",
                 self.webhook_url,
@@ -3411,36 +3695,62 @@
     # Write the updated data back to the JSON file with indentation
     with open(file_name, "w") as file:
         json.dump(data, file, indent=4, default=str)
 
 
 def word_to_num(s):
     word = {
-        'one': 1, 'two': 2, 'three': 3, 'four': 4, 'five': 5,
-        'six': 6, 'seven': 7, 'eight': 8, 'nine': 9, 'ten': 10,
-        'eleven': 11, 'twelve': 12, 'thirteen': 13, 'fourteen': 14,
-        'fifteen': 15, 'sixteen': 16, 'seventeen': 17, 'eighteen': 18, 'nineteen': 19,
-        'twenty': 20, 'thirty': 30, 'forty': 40, 'fifty': 50,
-        'sixty': 60, 'seventy': 70, 'eighty': 80, 'ninety': 90
+        "one": 1,
+        "two": 2,
+        "three": 3,
+        "four": 4,
+        "five": 5,
+        "six": 6,
+        "seven": 7,
+        "eight": 8,
+        "nine": 9,
+        "ten": 10,
+        "eleven": 11,
+        "twelve": 12,
+        "thirteen": 13,
+        "fourteen": 14,
+        "fifteen": 15,
+        "sixteen": 16,
+        "seventeen": 17,
+        "eighteen": 18,
+        "nineteen": 19,
+        "twenty": 20,
+        "thirty": 30,
+        "forty": 40,
+        "fifty": 50,
+        "sixty": 60,
+        "seventy": 70,
+        "eighty": 80,
+        "ninety": 90,
+    }
+    multiplier = {
+        "thousand": 1000,
+        "hundred": 100,
+        "million": 1000000,
+        "billion": 1000000000,
     }
-    multiplier = {'thousand': 1000, 'hundred': 100, 'million': 1000000, 'billion': 1000000000}
 
     words = s.lower().split()
-    if words[0] == 'a':
-        words[0] = 'one'
+    if words[0] == "a":
+        words[0] = "one"
     total = 0
     current = 0
     for w in words:
         if w in word:
             current += word[w]
         if w in multiplier:
             current *= multiplier[w]
-        if w == 'and':
+        if w == "and":
             continue
-        if w == 'thousand' or w == 'million' or w == 'billion':
+        if w == "thousand" or w == "million" or w == "billion":
             total += current
             current = 0
     total += current
     return total
 
 
 def login(user, pin, apikey, authkey, webhook_url=None):
@@ -3587,152 +3897,155 @@
                 headers={"Content-Type": "application/json"},
             )
             print(message)
         except requests.exceptions.SSLError as e:
             print(f"Error in sending notification: {e}")
 
 
-def check_and_notify_order_placement_statuses(statuses, target_status="complete", webhook_url=None, **kwargs):
-
+def check_and_notify_order_placement_statuses(
+    statuses, target_status="complete", webhook_url=None, **kwargs
+):
     order_prefix = f"{kwargs['order_tag']}: " if "order_tag" in kwargs else ""
     order_message = [f"{k}-{v}" for k, v in kwargs.items() if k != "order_tag"]
     order_message = ", ".join(order_message)
 
     if all(statuses == target_status):
         notifier(
             f"{order_prefix}Order(s) placed successfully for {order_message}",
-            webhook_url
+            webhook_url,
         )
     elif all(statuses == "rejected"):
-        notifier(
-            f"{order_prefix}All orders rejected for {order_message}",
-            webhook_url
-        )
+        notifier(f"{order_prefix}All orders rejected for {order_message}", webhook_url)
         raise Exception("Orders rejected")
     elif any(statuses == "open"):
         notifier(
             f"{order_prefix}Some orders pending for {order_message}. You can modify the orders.",
-            webhook_url
+            webhook_url,
         )
     elif any(statuses == "rejected"):
         notifier(
             f"{order_prefix}Some orders rejected for {order_message}.\nYou can place the rejected orders again.",
-            webhook_url
+            webhook_url,
         )
     else:
         notifier(
             f"{order_prefix}ERROR. Order statuses uncertain for {order_message}",
-            webhook_url
+            webhook_url,
         )
         raise Exception("Order statuses uncertain")
 
 
 def place_option_order_and_notify(
     instrument: Option | Strangle | Straddle | SyntheticFuture,
     action: str,
     qty_in_lots: int,
     prices: str | int | float | tuple | list | np.ndarray = "LIMIT",
     order_tag: str = "",
     webhook_url=None,
     stop_loss_order: bool = False,
     target_status: str = "complete",
     return_avg_price: bool = True,
-    **kwargs
+    **kwargs,
 ):
-
     notify_dict = {
         "order_tag": order_tag,
         "Underlying": instrument.underlying,
         "Action": action,
         "Expiry": instrument.expiry,
-        "Qty": qty_in_lots
+        "Qty": qty_in_lots,
     }
 
     order_params = {
         "transaction_type": action,
         "quantity_in_lots": qty_in_lots,
         "stop_loss_order": stop_loss_order,
-        "order_tag": order_tag
+        "order_tag": order_tag,
     }
 
     if isinstance(instrument, (Strangle, Straddle, SyntheticFuture)):
-        notify_dict.update({
-            "Strikes": [instrument.call_strike, instrument.put_strike]})
-        order_params.update({
-            "prices": prices
-        })
+        notify_dict.update({"Strikes": [instrument.call_strike, instrument.put_strike]})
+        order_params.update({"prices": prices})
     elif isinstance(instrument, Option):
-        notify_dict.update({
-            "Strike": instrument.strike,
-            "OptionType": instrument.option_type
-        })
-        order_params.update({
-            "price": prices
-        })
+        notify_dict.update(
+            {"Strike": instrument.strike, "OptionType": instrument.option_type}
+        )
+        order_params.update({"price": prices})
     else:
         raise ValueError("Invalid instrument type")
 
     notify_dict.update(kwargs)
 
     if stop_loss_order:
-        assert isinstance(prices, (int, float, tuple, list, np.ndarray)), "Stop loss order requires a price"
+        assert isinstance(
+            prices, (int, float, tuple, list, np.ndarray)
+        ), "Stop loss order requires a price"
         target_status = "trigger pending"
 
     # Placing the order
     order_ids = instrument.place_order(**order_params)
 
     if isinstance(order_ids, tuple):  # Strangle/Straddle/SyntheticFuture
         call_order_ids, put_order_ids = order_ids[0], order_ids[1]
         order_ids = list(itertools.chain(call_order_ids, put_order_ids))
     else:  # Option
         call_order_ids, put_order_ids = False, False
 
-    order_book = fetch_book('orderbook')
-    order_statuses_ = lookup_and_return(order_book, 'orderid', order_ids, 'status')
+    order_book = fetch_book("orderbook")
+    order_statuses_ = lookup_and_return(order_book, "orderid", order_ids, "status")
     check_and_notify_order_placement_statuses(
-        statuses=order_statuses_, target_status=target_status, webhook_url=webhook_url, **notify_dict
+        statuses=order_statuses_,
+        target_status=target_status,
+        webhook_url=webhook_url,
+        **notify_dict,
     )
 
     if return_avg_price:
         if call_order_ids and put_order_ids:
-            call_avg_price = lookup_and_return(
-                order_book, 'orderid', call_order_ids, 'averageprice'
-            ).astype(float).mean()
-            put_avg_price = lookup_and_return(
-                order_book, 'orderid', put_order_ids, 'averageprice'
-            ).astype(float).mean()
+            call_avg_price = (
+                lookup_and_return(order_book, "orderid", call_order_ids, "averageprice")
+                .astype(float)
+                .mean()
+            )
+            put_avg_price = (
+                lookup_and_return(order_book, "orderid", put_order_ids, "averageprice")
+                .astype(float)
+                .mean()
+            )
             return call_avg_price, put_avg_price
         else:
-            avg_price = lookup_and_return(order_book, 'orderid', order_ids, 'averageprice').astype(float).mean()
+            avg_price = (
+                lookup_and_return(order_book, "orderid", order_ids, "averageprice")
+                .astype(float)
+                .mean()
+            )
             return avg_price
 
     return order_ids
 
 
 def process_stop_loss_order_statuses(
-        order_book, order_ids, context="", notify_url=None,
+    order_book,
+    order_ids,
+    context="",
+    notify_url=None,
 ):
     pending_text = "trigger pending"
     context = f"{context} " if context else ""
 
     statuses = lookup_and_return(order_book, "orderid", order_ids, "status")
 
     if isinstance(statuses, (int, np.int32, np.int64)):
         logger.error(f"Statuses is {statuses} for orderid(s) {order_ids}")
 
     if all(statuses == pending_text):
         return False, False
 
     elif all(statuses == "rejected") or all(statuses == "cancelled"):
-        rejection_reasons = lookup_and_return(
-            order_book, "orderid", order_ids, "text"
-        )
-        if all(
-                rejection_reasons == "17070 : The Price is out of the LPP range"
-        ):
+        rejection_reasons = lookup_and_return(order_book, "orderid", order_ids, "text")
+        if all(rejection_reasons == "17070 : The Price is out of the LPP range"):
             return True, False
         else:
             notifier(
                 f"{context}Order rejected or cancelled. Reasons: {rejection_reasons[0]}",
                 notify_url,
             )
             raise Exception(f"Orders rejected or cancelled.")
@@ -3745,17 +4058,15 @@
         if all(statuses == "pending"):
             try:
                 cancel_pending_orders(order_ids, "NORMAL")
             except Exception as e:
                 try:
                     cancel_pending_orders(order_ids, "STOPLOSS")
                 except Exception as e:
-                    notifier(
-                        f"{context}Could not cancel orders: {e}", notify_url
-                    )
+                    notifier(f"{context}Could not cancel orders: {e}", notify_url)
                     raise Exception(f"Could not cancel orders: {e}")
             notifier(
                 f"{context}Orders pending and cancelled. Please check.",
                 notify_url,
             )
             return True, False
 
@@ -3772,17 +4083,15 @@
         notifier(
             f"{context}Orders in unknown state. Statuses: {statuses}",
             notify_url,
         )
         raise Exception(f"Orders in unknown state.")
 
 
-def fetch_orderbook_if_needed(
-    data_class=None, refresh_needed: bool = False
-):
+def fetch_orderbook_if_needed(data_class=None, refresh_needed: bool = False):
     if data_class is None or refresh_needed:
         return fetch_book("orderbook")
     if (
         currenttime() - data_class.updated_time < timedelta(seconds=15)
         and data_class.orderbook_data is not None
     ):
         return data_class.orderbook_data
@@ -3794,15 +4103,14 @@
     if time(9, 15) <= currenttime().time() <= time(15, 30):
         return True
     else:
         return False
 
 
 def last_market_close_time():
-
     if currenttime().time() < time(9, 15):
         wip_time = currenttime() - timedelta(days=1)
         wip_time = wip_time.replace(hour=15, minute=30, second=0, microsecond=0)
     elif currenttime().time() > time(15, 30):
         wip_time = currenttime().replace(hour=15, minute=30, second=0, microsecond=0)
     else:
         wip_time = currenttime()
@@ -3850,15 +4158,15 @@
     :param print_results:
     :return:
     """
 
     if price is None and vol is None:
         raise ValueError("Either price or vol must be specified.")
     flag = flag.lower()[0]
-    price_func = bs.put if flag == 'p' else bs.call
+    price_func = bs.put if flag == "p" else bs.call
 
     if direction == "away":
         if flag == "c":
             simulated_move = -simulated_move
         else:
             simulated_move = simulated_move
     elif direction == "towards" or direction == "toward":
@@ -3964,21 +4272,24 @@
         symbol_token_pairs = [
             (token_df.loc[token_df["token"] == token, "symbol"].values[0], token)
             for token in tokens
         ]
         return symbol_token_pairs
 
     if expiry is None and strike is None and option_type is None:  # Cash segment
-
         if name in ["NIFTY", "BANKNIFTY"]:  # Index scrips
             filtered_scrips = scrips.loc[
-                (scrips.name == name) & (scrips.exch_seg == "NSE") & (scrips.instrumenttype != "AMXIDX")
-            ]   # Temp fix for AMXIDX
+                (scrips.name == name)
+                & (scrips.exch_seg == "NSE")
+                & (scrips.instrumenttype != "AMXIDX")
+            ]  # Temp fix for AMXIDX
             # print(f'Length of filtered scrips: {len(filtered_scrips)}')
-            assert len(filtered_scrips) == 1, "More than one index scrip found for name."
+            assert (
+                len(filtered_scrips) == 1
+            ), "More than one index scrip found for name."
             symbol, token = filtered_scrips[["symbol", "token"]].values[0]
 
         elif name in ["FINNIFTY", "MIDCPNIFTY"]:  # Finnifty & Midcpnifty temp fix
             futures = scrips.loc[
                 (scrips.name == name) & (scrips.instrumenttype == "FUTIDX"),
                 ["expiry", "symbol", "token"],
             ]
@@ -3988,18 +4299,22 @@
 
         else:  # For all other equity scrips
             filtered_scrips = scrips.loc[
                 (scrips.name == name)
                 & (scrips.exch_seg == "NSE")
                 & (scrips.symbol.str.endswith("EQ"))
             ]
-            assert len(filtered_scrips) == 1, "More than one equity scrip found for name."
+            assert (
+                len(filtered_scrips) == 1
+            ), "More than one equity scrip found for name."
             symbol, token = filtered_scrips[["symbol", "token"]].values[0]
 
-    elif expiry is not None and strike is not None and option_type is not None:  # Options segment
+    elif (
+        expiry is not None and strike is not None and option_type is not None
+    ):  # Options segment
         strike = str(int(strike))  # Handle float strikes, convert to integer first
         symbol = name + expiry + strike + option_type
         token = scrips[scrips.symbol == symbol]["token"].tolist()[0]
 
     else:
         raise ValueError("Invalid arguments")
 
@@ -4074,37 +4389,36 @@
             else:
                 print(f"Error {attempt} in fetching LTP: {e}")
                 sleep(1)
                 continue
 
 
 def get_historical_prices(
-        interval,
-        last_n_intervals=None,
-        from_date=None,
-        to_date=None,
-        token=None,
-        name=None,
-        expiry=None,
-        strike=None,
-        option_type=None
+    interval,
+    last_n_intervals=None,
+    from_date=None,
+    to_date=None,
+    token=None,
+    name=None,
+    expiry=None,
+    strike=None,
+    option_type=None,
 ):
+    """Available intervals:
 
-    """ Available intervals:
+    ONE_MINUTE	1 Minute
+    THREE_MINUTE 3 Minute
+    FIVE_MINUTE	5 Minute
+    TEN_MINUTE	10 Minute
+    FIFTEEN_MINUTE	15 Minute
+    THIRTY_MINUTE	30 Minute
+    ONE_HOUR	1 Hour
+    ONE_DAY	1 Day
 
-        ONE_MINUTE	1 Minute
-        THREE_MINUTE 3 Minute
-        FIVE_MINUTE	5 Minute
-        TEN_MINUTE	10 Minute
-        FIFTEEN_MINUTE	15 Minute
-        THIRTY_MINUTE	30 Minute
-        ONE_HOUR	1 Hour
-        ONE_DAY	1 Day
-
-        """
+    """
 
     if token is None and name is None:
         raise ValueError("Either name or token must be specified.")
 
     if last_n_intervals is None and from_date is None:
         raise ValueError("Either last_n_intervals or from_date must be specified.")
 
@@ -4114,17 +4428,19 @@
     if to_date is None:
         to_date = last_market_close_time()
     else:
         to_date = pd.to_datetime(to_date)
 
     if from_date is None and last_n_intervals is not None:
         interval_digit, interval_unit = interval.lower().split("_")
-        interval_unit = interval_unit + "s" if interval_unit[-1] != "s" else interval_unit
+        interval_unit = (
+            interval_unit + "s" if interval_unit[-1] != "s" else interval_unit
+        )
         interval_digit = word_to_num(interval_digit)
-        time_delta = interval_digit*last_n_intervals
+        time_delta = interval_digit * last_n_intervals
         from_date = to_date - timedelta(**{interval_unit: time_delta})
     else:
         from_date = pd.to_datetime(from_date)
 
     to_date = to_date.strftime("%Y-%m-%d %H:%M")
     from_date = from_date.strftime("%Y-%m-%d %H:%M")
 
@@ -4138,15 +4454,15 @@
         "symboltoken": token,
         "interval": interval,
         "fromdate": from_date,
         "todate": to_date,
     }
     data = obj.getCandleData(historic_param)
     data = pd.DataFrame(data["data"])
-    data.set_index(pd.Series(data.iloc[:, 0], name='date'), inplace=True)
+    data.set_index(pd.Series(data.iloc[:, 0], name="date"), inplace=True)
     data.index = pd.to_datetime(data.index)
     data.index = data.index.tz_localize(None)
     data.drop(data.columns[0], axis=1, inplace=True)
     data.columns = ["open", "high", "low", "close", "volume"]
     return data
 
 
@@ -4200,15 +4516,14 @@
 # Finding ATM strike
 def findstrike(x, base):
     number = base * round(x / base)
     return int(number)
 
 
 def custom_round(x, base=0.05):
-
     if x == 0:
         return 0
 
     num = base * round(x / base)
     if num == 0:
         num = base
     return round(num, 2)
@@ -4235,38 +4550,53 @@
 def check_for_weekend(expiry):
     expiry = datetime.strptime(expiry, "%d%b%y")
     expiry = expiry + pd.DateOffset(minutes=930)
     date_range = pd.date_range(currenttime().date(), expiry - timedelta(days=1))
     return date_range.weekday.isin([5, 6]).any()
 
 
-def get_strangle_indices_to_trade(*indices, pre_weekend_indices=None):
-
-    if pre_weekend_indices is None:
-        pre_weekend_indices = ["NIFTY", "BANKNIFTY"]
-
-    times_to_expiries = [timetoexpiry(index.current_expiry, effective_time=True, in_days=True) for index in indices]
+def get_strangle_indices_to_trade(*indices, safe_indices=None):
+    if safe_indices is None:
+        safe_indices = ["NIFTY", "BANKNIFTY"]
+
+    times_to_expiries = [
+        timetoexpiry(index.current_expiry, effective_time=True, in_days=True)
+        for index in indices
+    ]
 
     # Check if any index has less than 1 day to expiry
-    indices_less_than_1_day = [index for index, time_to_expiry in zip(indices, times_to_expiries) if time_to_expiry < 1]
+    indices_less_than_1_day = [
+        index
+        for index, time_to_expiry in zip(indices, times_to_expiries)
+        if time_to_expiry < 1
+    ]
 
     if indices_less_than_1_day:
         return indices_less_than_1_day
 
     # If no index has less than 1 day to expiry
     min_expiry_time = min(times_to_expiries)
     indices_with_closest_expiries = [
-        index for index, time_to_expiry in zip(indices, times_to_expiries)
+        index
+        for index, time_to_expiry in zip(indices, times_to_expiries)
         if time_to_expiry == min_expiry_time
     ]
     closest_index_names = [index.name for index in indices_with_closest_expiries]
-    weekend_in_range = check_for_weekend(indices_with_closest_expiries[0].current_expiry)
+    weekend_in_range = check_for_weekend(
+        indices_with_closest_expiries[0].current_expiry
+    )
+
+    if "MIDCPNIFTY" in closest_index_names:
+        indices_without_midcp = [
+            index for index in indices if index.name != "MIDCPNIFTY"
+        ]
+        return get_strangle_indices_to_trade(*indices_without_midcp)
 
-    if (("FINNIFTY" in closest_index_names) and weekend_in_range) or ("MIDCPNIFTY" in closest_index_names):
-        return [index for index in indices if index.name in pre_weekend_indices]
+    if "FINNIFTY" in closest_index_names and weekend_in_range:
+        return [index for index in indices if index.name in safe_indices]
 
     return indices_with_closest_expiries
 
 
 def indices_to_trade(nifty, bnf, finnifty, multi_before_weekend=False):  # delete this
     fin_exp_closer = timetoexpiry(
         finnifty.current_expiry, effective_time=True, in_days=True
@@ -4375,48 +4705,54 @@
     gamma = bs.gamma(underlying_price, strike, time_left, 0.05, iv)
 
     return iv, delta, gamma
 
 
 @time_the_function
 def most_equal_strangle(*strangles, disparity_threshold=np.inf, exit_time=time(15, 25)):
-
     # Create a set of all distinct options
-    options = set(option for strangle in strangles for option in (strangle.call_option, strangle.put_option))
+    options = set(
+        option
+        for strangle in strangles
+        for option in (strangle.call_option, strangle.put_option)
+    )
 
     # Define the price disparity function
     def price_disparity(strangle):
         call_ltp = ltp_cache[strangle.call_option]
         put_ltp = ltp_cache[strangle.put_option]
         return abs(call_ltp - put_ltp) / min(call_ltp, put_ltp)
 
     tracked_strangle = None
 
     while currenttime().time() < exit_time:
-
         # If there's no tracked strangle update all prices and find the most equal strangle
         if tracked_strangle is None:
             ltp_cache = {option: option.fetch_ltp() for option in options}
-            most_equal, min_disparity = min(((s, price_disparity(s)) for s in strangles), key=lambda x: x[1])
+            most_equal, min_disparity = min(
+                ((s, price_disparity(s)) for s in strangles), key=lambda x: x[1]
+            )
             if min_disparity < 0.10:
                 tracked_strangle = most_equal
 
         # If there's a tracked strangle, check its disparity
         else:
             ltp_cache = {
                 tracked_strangle.call_option: tracked_strangle.call_option.fetch_ltp(),
-                tracked_strangle.put_option: tracked_strangle.put_option.fetch_ltp()
+                tracked_strangle.put_option: tracked_strangle.put_option.fetch_ltp(),
             }
             most_equal = tracked_strangle
             min_disparity = price_disparity(tracked_strangle)
             if min_disparity >= 0.10:
                 tracked_strangle = None
 
-        logger.info(f"Most equal strangle: {most_equal} with disparity {min_disparity} "
-                    f"and prices {ltp_cache[most_equal.call_option]} and {ltp_cache[most_equal.put_option]}")
+        logger.info(
+            f"Most equal strangle: {most_equal} with disparity {min_disparity} "
+            f"and prices {ltp_cache[most_equal.call_option]} and {ltp_cache[most_equal.put_option]}"
+        )
         logger.info(f"Most equal ltp cache: {ltp_cache}")
         # If the lowest disparity is below the threshold, return the most equal strangle
         if min_disparity < disparity_threshold:
             return most_equal
         else:
             pass
 
@@ -4444,46 +4780,57 @@
         constituents["Index weight"].to_list(),
     )
 
     return constituent_tickers, constituent_weights
 
 
 def convert_option_chains_to_df(option_chains, return_all=False, for_surface=False):
-
     def add_columns_for_surface(data_frame):
-
         data_frame = data_frame.copy()
-        data_frame['atm_strike'] = data_frame.apply(
-            lambda row: findstrike(row.spot, 50) if row.symbol == 'NIFTY' else findstrike(row.spot, 100),
-            axis=1)
-        data_frame['strike_iv'] = np.where(data_frame.strike > data_frame.atm_strike, data_frame.call_iv,
-                                           np.where(data_frame.strike < data_frame.atm_strike,
-                                                    data_frame.put_iv, data_frame.avg_iv))
-        data_frame['atm_iv'] = data_frame.apply(
-            lambda row: data_frame[(data_frame.strike == row.atm_strike)
-                                   & (data_frame.expiry == row.expiry)].strike_iv.values[0], axis=1)
-        data_frame.sort_values(['symbol', 'expiry', 'strike'], inplace=True)
-        data_frame['distance'] = (data_frame['strike'] / data_frame['spot'] - 1)
-        data_frame['iv_multiple'] = data_frame['strike_iv'] / data_frame['atm_iv']
-        data_frame['distance_squared'] = data_frame['distance'] ** 2
+        data_frame["atm_strike"] = data_frame.apply(
+            lambda row: findstrike(row.spot, 50)
+            if row.symbol == "NIFTY"
+            else findstrike(row.spot, 100),
+            axis=1,
+        )
+        data_frame["strike_iv"] = np.where(
+            data_frame.strike > data_frame.atm_strike,
+            data_frame.call_iv,
+            np.where(
+                data_frame.strike < data_frame.atm_strike,
+                data_frame.put_iv,
+                data_frame.avg_iv,
+            ),
+        )
+        data_frame["atm_iv"] = data_frame.apply(
+            lambda row: data_frame[
+                (data_frame.strike == row.atm_strike)
+                & (data_frame.expiry == row.expiry)
+            ].strike_iv.values[0],
+            axis=1,
+        )
+        data_frame.sort_values(["symbol", "expiry", "strike"], inplace=True)
+        data_frame["distance"] = data_frame["strike"] / data_frame["spot"] - 1
+        data_frame["iv_multiple"] = data_frame["strike_iv"] / data_frame["atm_iv"]
+        data_frame["distance_squared"] = data_frame["distance"] ** 2
 
         return data_frame
 
     symbol_dfs = []
     for symbol in option_chains:
         spot_price = option_chains[symbol].underlying_price
         expiry_dfs = []
         for expiry in option_chains[symbol]:
             df = pd.DataFrame(option_chains[symbol][expiry]).T
-            df.index = df.index.set_names('strike')
+            df.index = df.index.set_names("strike")
             df = df.reset_index()
-            df['spot'] = spot_price
-            df['expiry'] = expiry
-            df['symbol'] = symbol
-            df['time_to_expiry'] = timetoexpiry(expiry)
+            df["spot"] = spot_price
+            df["expiry"] = expiry
+            df["symbol"] = symbol
+            df["time_to_expiry"] = timetoexpiry(expiry)
             expiry_dfs.append(df)
         symbol_oc = pd.concat(expiry_dfs)
         if for_surface:
             symbol_oc = add_columns_for_surface(symbol_oc)
         symbol_dfs.append(symbol_oc)
 
     if return_all:
@@ -4527,16 +4874,16 @@
     charges_per_share = total_charges / (num_contracts * contract_size)
 
     return round(charges_per_share, 1)
 
 
 # ORDER FUNCTIONS BELOW #
 
-def place_order(symbol, token, qty, action, price, order_tag="", stop_loss_order=False):
 
+def place_order(symbol, token, qty, action, price, order_tag="", stop_loss_order=False):
     action = action.upper()
     if isinstance(price, str):
         price = price.upper()
 
     params = {
         "tradingsymbol": symbol,
         "symboltoken": token,
@@ -4546,39 +4893,49 @@
         "duration": "DAY",
         "quantity": int(qty),
         "ordertag": order_tag,
     }
 
     if stop_loss_order:
         execution_price = price * 1.1
-        params.update({
-            "variety": "STOPLOSS",
-            "ordertype": "STOPLOSS_LIMIT",
-            "triggerprice": round(price, 1),
-            "price": round(execution_price, 1),
-        })
+        params.update(
+            {
+                "variety": "STOPLOSS",
+                "ordertype": "STOPLOSS_LIMIT",
+                "triggerprice": round(price, 1),
+                "price": round(execution_price, 1),
+            }
+        )
     else:
-        order_type, execution_price = ("MARKET", 0) if price == "MARKET" else ("LIMIT", price)
+        order_type, execution_price = (
+            ("MARKET", 0) if price == "MARKET" else ("LIMIT", price)
+        )
         if order_type == "LIMIT":
             if execution_price < 10 and qty < 6000:
-                execution_price = np.ceil(price) if action == "BUY" else max(np.floor(price), 0.05)
+                execution_price = (
+                    np.ceil(price) if action == "BUY" else max(np.floor(price), 0.05)
+                )
 
-        params.update({
-            "variety": "NORMAL",
-            "ordertype": order_type,
-            "price": custom_round(execution_price)
-        })
+        params.update(
+            {
+                "variety": "NORMAL",
+                "ordertype": order_type,
+                "price": custom_round(execution_price),
+            }
+        )
 
     for attempt in range(1, 4):
         try:
             return obj.placeOrder(params)
         except Exception as e:
             if attempt == 3:
                 raise e
-            print(f"Error {attempt} in placing {'stop-loss ' if stop_loss_order else ''}order for {symbol}: {e}")
+            print(
+                f"Error {attempt} in placing {'stop-loss ' if stop_loss_order else ''}order for {symbol}: {e}"
+            )
             sleep(2)
 
 
 def place_synthetic_fut_order(
     name,
     strike,
     expiry,
```

### Comparing `volstreet-1.0.0/volstreet/discord_bot.py` & `volstreet-1.0.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.0/volstreet/nsefunctions.py` & `volstreet-1.0.1/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.0/volstreet/strategies.py` & `volstreet-1.0.1/volstreet/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,16 @@
     user=None,
     pin=None,
     apikey=None,
     authkey=None,
     webhook_url=None,
     shared_data=True,
     start_time=(9, 16),
-    special_parameters=None
+    special_parameters=None,
 ):
-
     """
     :param parameters: parameters for the strategy (refer to the strategy's docstring)
     :param strategy: 'straddle' or 'strangle' will invoke intraday_straddle or intraday_strangle of the index
     :param client:
     :param user:
     :param pin:
     :param apikey:
@@ -81,34 +80,36 @@
     nifty = vs.Index("NIFTY", webhook_url=discord_webhook_url)
     bnf = vs.Index("BANKNIFTY", webhook_url=discord_webhook_url)
     fin = vs.Index("FINNIFTY", webhook_url=discord_webhook_url)
     midcap = vs.Index("MIDCPNIFTY", webhook_url=discord_webhook_url)
 
     indices = vs.get_strangle_indices_to_trade(nifty, bnf, fin, midcap)
 
-    parameters["quantity_in_lots"] = (
-        parameters["quantity_in_lots"] // len(indices)
-    )
+    parameters["quantity_in_lots"] = parameters["quantity_in_lots"] // len(indices)
 
     # Setting the shared data
     if shared_data:
         shared_data = vs.SharedData()
         update_data_thread = threading.Thread(target=shared_data.update_data)
         parameters["shared_data"] = shared_data
     else:
         shared_data = None
         update_data_thread = None
 
     options_threads = []
     for index in indices:
         index_parameters = parameters.copy()
         index_parameters.update(special_parameters.get(index.name, {}))
-        vs.logger.info(f"Trading {index.name} {strategy} with parameters {index_parameters}")
+        vs.logger.info(
+            f"Trading {index.name} {strategy} with parameters {index_parameters}"
+        )
         vs.notifier(f"Trading {index.name} {strategy}.", discord_webhook_url)
-        thread = threading.Thread(target=getattr(index, f'intraday_{strategy}'), kwargs=index_parameters)
+        thread = threading.Thread(
+            target=getattr(index, f"intraday_{strategy}"), kwargs=index_parameters
+        )
         options_threads.append(thread)
 
     # Wait for the market to open
     while vs.currenttime().time() < time(*start_time):
         sleep(1)
 
     # Start the data updater thread
@@ -186,15 +187,14 @@
     client=None,
     user=None,
     pin=None,
     apikey=None,
     authkey=None,
     webhook_url=None,
 ):
-
     """
 
     :param parameters: parameters for the strategy (refer to the strategy's docstring)
                        summary of parameters:
                        quantity_in_lots,
                        start_time=(9, 15, 58),
                        exit_time=(15, 27),
@@ -228,17 +228,15 @@
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
 
     threads = []
     for index_symbol in indices:
         index = vs.Index(index_symbol, webhook_url=discord_webhook_url)
-        thread = threading.Thread(
-            target=index.intraday_trend, kwargs=parameters
-        )
+        thread = threading.Thread(target=index.intraday_trend, kwargs=parameters)
         threads.append(thread)
 
     for thread in threads:
         thread.start()
 
     for thread in threads:
         thread.join()
@@ -270,15 +268,19 @@
     index = vs.Index(index_symbol)
     index_info = index.fetch_otm_info(index_strike_offset, expiry=expirys[0])
     index_iv, index_shares = (
         index_info["avg_iv"],
         int(total_exposure / (index.fetch_ltp() * index.lot_size)) * index.lot_size,
     )
     index_premium_value = index_info["total_price"] * index_shares
-    index_break_even_points = (index_info["underlying_price"], index_info["call_strike"], index_info["put_strike"])
+    index_break_even_points = (
+        index_info["underlying_price"],
+        index_info["call_strike"],
+        index_info["put_strike"],
+    )
     index_break_even_points += (
         index_info["call_strike"] + index_info["total_price"],
         index_info["put_strike"] - index_info["total_price"],
     )
 
     # Calculate movements to break even
     def _return_abs_movement(current_price, threshold_price):
```

### Comparing `volstreet-1.0.0/volstreet.egg-info/requires.txt` & `volstreet-1.0.1/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

