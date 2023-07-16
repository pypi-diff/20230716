# Comparing `tmp/volstreet-0.9.9.tar.gz` & `tmp/volstreet-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-0.9.9.tar", last modified: Wed Jun 14 06:56:50 2023, max compression
+gzip compressed data, was "volstreet-1.0.0.tar", last modified: Sun Jul 16 12:55:25 2023, max compression
```

## Comparing `volstreet-0.9.9.tar` & `volstreet-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:56:50.886340 volstreet-0.9.9/
--rw-rw-rw-   0        0        0      497 2023-06-14 06:56:50.887338 volstreet-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.9/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.9/pyproject.toml
--rw-rw-rw-   0        0        0     1375 2023-06-14 06:56:50.888334 volstreet-0.9.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 06:56:50.879365 volstreet-0.9.9/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.9/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.9/volstreet/__init__.py
--rw-rw-rw-   0        0        0     8765 2023-06-13 13:36:04.000000 volstreet-0.9.9/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.9/volstreet/constants.py
--rw-rw-rw-   0        0        0    25475 2023-06-12 13:04:14.000000 volstreet-0.9.9/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   168512 2023-06-14 04:51:09.000000 volstreet-0.9.9/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.9/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.9/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.9/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.9/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:56:50.885343 volstreet-0.9.9/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      787 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 12:55:25.771697 volstreet-1.0.0/
+-rw-rw-rw-   0        0        0      497 2023-07-16 12:55:25.771697 volstreet-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.0/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-07-16 12:55:25.774111 volstreet-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 12:55:25.765208 volstreet-1.0.0/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.0/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.0/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     8889 2023-07-08 15:26:12.000000 volstreet-1.0.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.0/volstreet/constants.py
+-rw-rw-rw-   0        0        0    41203 2023-07-14 15:07:17.000000 volstreet-1.0.0/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   185952 2023-07-16 12:37:53.000000 volstreet-1.0.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-1.0.0/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.0/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    13073 2023-07-15 16:36:10.000000 volstreet-1.0.0/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:55:25.771697 volstreet-1.0.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 12:55:25.000000 volstreet-1.0.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-0.9.9/setup.cfg` & `volstreet-1.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 302e 392e 390d 0a61  rsion = 0.9.9..a
+00000020: 7273 696f 6e20 3d20 312e 302e 300d 0a61  rsion = 1.0.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
@@ -36,51 +36,52 @@
 00000230: 6469 7363 6f72 642e 7079 3e3d 322e 322e  discord.py>=2.2.
 00000240: 320d 0a09 656e 7472 7970 6f69 6e74 733d  2...entrypoints=
 00000250: 3d30 2e34 0d0a 0965 7865 6375 7469 6e67  =0.4...executing
 00000260: 3d3d 312e 322e 300d 0a09 656f 643d 3d30  ==1.2.0...eod==0
 00000270: 2e32 2e31 0d0a 0966 757a 7a79 7775 7a7a  .2.1...fuzzywuzz
 00000280: 793d 3d30 2e31 382e 300d 0a09 6964 6e61  y==0.18.0...idna
 00000290: 3d3d 332e 340d 0a09 6a65 6469 3d3d 302e  ==3.4...jedi==0.
-000002a0: 3138 2e32 0d0a 096c 786d 6c3d 3d34 2e39  18.2...lxml==4.9
-000002b0: 2e32 0d0a 096d 6174 706c 6f74 6c69 622d  .2...matplotlib-
-000002c0: 696e 6c69 6e65 3d3d 302e 312e 360d 0a09  inline==0.1.6...
-000002d0: 6e65 7374 2d61 7379 6e63 696f 3d3d 312e  nest-asyncio==1.
-000002e0: 352e 360d 0a09 6e75 6d70 793d 3d31 2e32  5.6...numpy==1.2
-000002f0: 342e 320d 0a09 7061 636b 6167 696e 673d  4.2...packaging=
-00000300: 3d32 332e 300d 0a09 7061 6e64 6173 3d3d  =23.0...pandas==
-00000310: 312e 352e 330d 0a09 7061 7273 6f3d 3d30  1.5.3...parso==0
-00000320: 2e38 2e33 0d0a 0970 6963 6b6c 6573 6861  .8.3...picklesha
-00000330: 7265 3d3d 302e 372e 350d 0a09 706c 6174  re==0.7.5...plat
-00000340: 666f 726d 6469 7273 3d3d 322e 362e 320d  formdirs==2.6.2.
-00000350: 0a09 706c 6f74 6c79 3d3d 352e 3134 2e31  ..plotly==5.14.1
-00000360: 0d0a 0970 726f 6d70 742d 746f 6f6c 6b69  ...prompt-toolki
-00000370: 743d 3d33 2e30 2e33 360d 0a09 7073 7574  t==3.0.36...psut
-00000380: 696c 3d3d 352e 392e 340d 0a09 7075 7265  il==5.9.4...pure
-00000390: 2d65 7661 6c3d 3d30 2e32 2e32 0d0a 0950  -eval==0.2.2...P
-000003a0: 7967 6d65 6e74 733d 3d32 2e31 342e 300d  ygments==2.14.0.
-000003b0: 0a09 7079 6f74 703d 3d32 2e38 2e30 0d0a  ..pyotp==2.8.0..
-000003c0: 0970 7974 686f 6e2d 6461 7465 7574 696c  .python-dateutil
-000003d0: 3d3d 322e 382e 320d 0a09 7079 7468 6f6e  ==2.8.2...python
-000003e0: 2d4c 6576 656e 7368 7465 696e 3d3d 302e  -Levenshtein==0.
-000003f0: 3231 2e30 0d0a 0970 7974 7a3d 3d32 3032  21.0...pytz==202
-00000400: 322e 372e 310d 0a09 7079 7769 6e33 323d  2.7.1...pywin32=
-00000410: 3d33 3035 0d0a 0970 797a 6d71 3d3d 3235  =305...pyzmq==25
-00000420: 2e30 2e30 0d0a 0972 6571 7565 7374 733d  .0.0...requests=
-00000430: 3d32 2e32 382e 320d 0a09 7363 696b 6974  =2.28.2...scikit
-00000440: 2d6c 6561 726e 3d3d 312e 322e 320d 0a09  -learn==1.2.2...
-00000450: 7363 6970 793d 3d31 2e31 302e 310d 0a09  scipy==1.10.1...
-00000460: 7369 783d 3d31 2e31 362e 300d 0a09 736d  six==1.16.0...sm
-00000470: 6172 7461 7069 2d70 7974 686f 6e3d 3d31  artapi-python==1
-00000480: 2e33 2e30 0d0a 0973 7079 6465 722d 6b65  .3.0...spyder-ke
-00000490: 726e 656c 733e 3d32 2e32 2e31 0d0a 0973  rnels>=2.2.1...s
-000004a0: 7461 636b 2d64 6174 613d 3d30 2e36 2e32  tack-data==0.6.2
-000004b0: 0d0a 0974 6f72 6e61 646f 3d3d 362e 320d  ...tornado==6.2.
-000004c0: 0a09 7472 6169 746c 6574 733d 3d35 2e38  ..traitlets==5.8
-000004d0: 2e31 0d0a 0975 726c 6c69 6233 3d3d 312e  .1...urllib3==1.
-000004e0: 3236 2e31 340d 0a09 7763 7769 6474 683d  26.14...wcwidth=
-000004f0: 3d30 2e32 2e36 0d0a 0977 6562 736f 636b  =0.2.6...websock
-00000500: 6574 2d63 6c69 656e 743d 3d31 2e35 2e31  et-client==1.5.1
-00000510: 0d0a 0978 6c72 643d 3d32 2e30 2e31 0d0a  ...xlrd==2.0.1..
-00000520: 0979 6669 6e61 6e63 653d 3d30 2e32 2e31  .yfinance==0.2.1
-00000530: 340d 0a0d 0a5b 6567 675f 696e 666f 5d0d  4....[egg_info].
-00000540: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000550: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000002a0: 3138 2e32 0d0a 096b 6974 6563 6f6e 6e65  18.2...kiteconne
+000002b0: 6374 3d3d 342e 322e 300d 0a09 6c78 6d6c  ct==4.2.0...lxml
+000002c0: 3d3d 342e 392e 320d 0a09 6d61 7470 6c6f  ==4.9.2...matplo
+000002d0: 746c 6962 2d69 6e6c 696e 653d 3d30 2e31  tlib-inline==0.1
+000002e0: 2e36 0d0a 096e 6573 742d 6173 796e 6369  .6...nest-asynci
+000002f0: 6f3d 3d31 2e35 2e36 0d0a 096e 756d 7079  o==1.5.6...numpy
+00000300: 3d3d 312e 3234 2e32 0d0a 0970 6163 6b61  ==1.24.2...packa
+00000310: 6769 6e67 3d3d 3233 2e30 0d0a 0970 616e  ging==23.0...pan
+00000320: 6461 733d 3d31 2e35 2e33 0d0a 0970 6172  das==1.5.3...par
+00000330: 736f 3d3d 302e 382e 330d 0a09 7069 636b  so==0.8.3...pick
+00000340: 6c65 7368 6172 653d 3d30 2e37 2e35 0d0a  leshare==0.7.5..
+00000350: 0970 6c61 7466 6f72 6d64 6972 733d 3d32  .platformdirs==2
+00000360: 2e36 2e32 0d0a 0970 6c6f 746c 793d 3d35  .6.2...plotly==5
+00000370: 2e31 342e 310d 0a09 7072 6f6d 7074 2d74  .14.1...prompt-t
+00000380: 6f6f 6c6b 6974 3d3d 332e 302e 3336 0d0a  oolkit==3.0.36..
+00000390: 0970 7375 7469 6c3d 3d35 2e39 2e34 0d0a  .psutil==5.9.4..
+000003a0: 0970 7572 652d 6576 616c 3d3d 302e 322e  .pure-eval==0.2.
+000003b0: 320d 0a09 5079 676d 656e 7473 3d3d 322e  2...Pygments==2.
+000003c0: 3134 2e30 0d0a 0970 796f 7470 3d3d 322e  14.0...pyotp==2.
+000003d0: 382e 300d 0a09 7079 7468 6f6e 2d64 6174  8.0...python-dat
+000003e0: 6575 7469 6c3d 3d32 2e38 2e32 0d0a 0970  eutil==2.8.2...p
+000003f0: 7974 686f 6e2d 4c65 7665 6e73 6874 6569  ython-Levenshtei
+00000400: 6e3d 3d30 2e32 312e 300d 0a09 7079 747a  n==0.21.0...pytz
+00000410: 3d3d 3230 3232 2e37 2e31 0d0a 0970 7977  ==2022.7.1...pyw
+00000420: 696e 3332 3d3d 3330 350d 0a09 7079 7a6d  in32==305...pyzm
+00000430: 713d 3d32 352e 302e 300d 0a09 7265 7175  q==25.0.0...requ
+00000440: 6573 7473 3d3d 322e 3238 2e32 0d0a 0973  ests==2.28.2...s
+00000450: 6369 6b69 742d 6c65 6172 6e3d 3d31 2e32  cikit-learn==1.2
+00000460: 2e32 0d0a 0973 6369 7079 3d3d 312e 3130  .2...scipy==1.10
+00000470: 2e31 0d0a 0973 656c 656e 6975 6d3d 3d34  .1...selenium==4
+00000480: 2e31 302e 300d 0a09 7369 783d 3d31 2e31  .10.0...six==1.1
+00000490: 362e 300d 0a09 736d 6172 7461 7069 2d70  6.0...smartapi-p
+000004a0: 7974 686f 6e3d 3d31 2e33 2e30 0d0a 0973  ython==1.3.0...s
+000004b0: 7461 636b 2d64 6174 613d 3d30 2e36 2e32  tack-data==0.6.2
+000004c0: 0d0a 0974 6f72 6e61 646f 3d3d 362e 320d  ...tornado==6.2.
+000004d0: 0a09 7472 6169 746c 6574 733d 3d35 2e38  ..traitlets==5.8
+000004e0: 2e31 0d0a 0975 726c 6c69 6233 3d3d 312e  .1...urllib3==1.
+000004f0: 3236 2e31 340d 0a09 7763 7769 6474 683d  26.14...wcwidth=
+00000500: 3d30 2e32 2e36 0d0a 0977 6562 736f 636b  =0.2.6...websock
+00000510: 6574 2d63 6c69 656e 743d 3d31 2e35 2e31  et-client==1.5.1
+00000520: 0d0a 0978 6c72 643d 3d32 2e30 2e31 0d0a  ...xlrd==2.0.1..
+00000530: 0979 6669 6e61 6e63 653d 3d30 2e32 2e31  .yfinance==0.2.1
+00000540: 340d 0a0d 0a5b 6567 675f 696e 666f 5d0d  4....[egg_info].
+00000550: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000560: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `volstreet-0.9.9/volstreet/SmartWebSocketV2.py` & `volstreet-1.0.0/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.9/volstreet/blackscholes.py` & `volstreet-1.0.0/volstreet/blackscholes.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,18 +254,22 @@
     flag = flag.lower()[0]
     price_func = call if flag == 'c' else put
     vol = implied_volatility(current_price, current_spot, strike, timeleft, 0.06, flag)
     delta_ = delta(current_spot, strike, timeleft, 0.06, vol, flag)
     estimated_movement_points = (target_price - current_price) / delta_
     estimated_movement = estimated_movement_points / current_spot
     timeleft = timeleft - (time_delta / 525600) if time_delta else timeleft
-    if timeleft < 0.0008:  # On expiry day
+
+    if timeleft < 0.0008:  # On expiry day we need to adjust the vol as iv increases steadily as we approach expiry
         vol_multiple = 2 - (1401.74 * timeleft)
         vol = vol * vol_multiple
-    modified_vol = iv_curve_adjustor(estimated_movement, timeleft, iv=vol, spot=current_spot, strike=strike)
+
+    modified_vol = iv_curve_adjustor(
+        estimated_movement, timeleft, iv=vol, spot=current_spot, strike=strike, _print_details=_print_details
+    )
 
     if _print_details:
         print(f'estimated movement: {estimated_movement}, vol: {vol}, modified vol: {modified_vol}')
 
     f = lambda s1: price_func(s1, strike, timeleft, 0.06, modified_vol) - target_price
 
     if target_price > current_price:
```

### Comparing `volstreet-0.9.9/volstreet/constants.py` & `volstreet-1.0.0/volstreet/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         response = requests.get(freeze_qty_url, timeout=10)  # Set the timeout value
         response.raise_for_status()  # Raise an exception if the response contains an HTTP error status
         df = pd.read_excel(response.content)
         df.columns = df.columns.str.strip()
         df["SYMBOL"] = df["SYMBOL"].str.strip()
     except Exception as e:
         print(f"Error in fetching qtyfreeze.xls: {e}")
-        df = pd.read_csv("autotrader/info/qtyfreeze.csv")
+        df = pd.read_csv("data/qtyfreeze.csv")
         df.columns = df.columns.str.strip()
         df["SYMBOL"] = df["SYMBOL"].str.strip()
     return df
 
 
 def create_logger(name):
     logger = logging.getLogger(name)
@@ -69,8 +69,8 @@
 
 scrips["expiry_dt"] = pd.to_datetime(
     scrips[scrips.expiry != ""]["expiry"], format="%d%b%Y"
 )
 scrips["expiry_formatted"] = scrips["expiry_dt"].dt.strftime("%d%b%y")
 scrips["expiry_formatted"] = scrips["expiry_formatted"].str.upper()
 
-logger = create_logger("volstreet")
+logger = create_logger("volstreet")
```

### Comparing `volstreet-0.9.9/volstreet/dealingroom.py` & `volstreet-1.0.0/volstreet/dealingroom.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,45 @@
 import logging
 import functools
 import itertools
 import traceback
 
 global login_data, obj
 
-large_order_threshold = 10
+LARGE_ORDER_THRESHOLD = 10
+ERROR_NOTIFICATION_SETTINGS = {'url': None}
+
+
+def set_error_notification_settings(key, value):
+    global ERROR_NOTIFICATION_SETTINGS
+    ERROR_NOTIFICATION_SETTINGS[key] = value
+
+
+def time_the_function(func):
+    def wrapper(*args, **kwargs):
+        start = datetime.now()
+        result = func(*args, **kwargs)
+        end = (datetime.now() - start).total_seconds()
+        logger.info(f"Time taken for {func.__name__}: {end:.2f} seconds")
+        return result
+    return wrapper
 
 
 def log_errors(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
-            logger.error(f"Error in function {func.__name__}: {e}\nTraceback:{traceback.format_exc()}")
+            user_prefix = ERROR_NOTIFICATION_SETTINGS.get('user', '')
+            logger.error(f"{user_prefix}Error in function {func.__name__}: {e}\nTraceback:{traceback.format_exc()}")
+            notifier(
+                f"{user_prefix}Error in function {func.__name__}: {e}\nTraceback:{traceback.format_exc()}",
+                ERROR_NOTIFICATION_SETTINGS['url']
+            )
             raise e
     return wrapper
 
 
 class OptionChains(defaultdict):
     """An object for having option chains for multiple expiries.
     Each expiry is a dictionary with integer default values"""
@@ -56,15 +77,15 @@
         self.price_dict = {}
         self.symbol_option_chains = {}
         self.last_update_time = None
         self.iv_log = defaultdict(lambda: defaultdict(dict))
         self.webhook_url = webhook_url
         self.index_option_chains_subscribed = []
         self.correlation_id = correlation_id
-        self.finnifty_index = Index("FINNIFTY")
+        self.finnifty_index = Index("FINNIFTY")  # Finnifty temp fix
 
     def start_websocket(self):
         def on_open(wsapp):
             self.subscribe_tokens()
 
         # Assign the callbacks.
         self.on_open = on_open
@@ -103,15 +124,15 @@
         self.last_update_time = currenttime()
 
     def parse_price_dict(self):
         new_price_dict = {
             scrips.loc[scrips.token == token]["symbol"].values[0]: value
             for token, value in self.price_dict.items()
         }
-        new_price_dict.update({"FINNIFTY": {"ltp": self.finnifty_index.fetch_ltp()}})
+        new_price_dict.update({"FINNIFTY": {"ltp": self.finnifty_index.fetch_ltp()}})  # Finnifty temp fix
         return new_price_dict
 
     def add_options(self, *underlyings, range_of_strikes=10, expiries=None, mode=1):
         """Adds options for the given underlyings to the symbol_option_chains dictionary.
         Params:
         underlyings is a list of underlying objects not strings
         If expiries is None, then the current, next and month expiry are added.
@@ -512,15 +533,15 @@
 class Strangle:
     def __init__(self, call_strike, put_strike, underlying, expiry):
         self.call_option = Option(call_strike, "CE", underlying, expiry)
         self.put_option = Option(put_strike, "PE", underlying, expiry)
         self.call_strike = self.call_option.strike
         self.put_strike = self.put_option.strike
         self.underlying = underlying
-        self.underlying_exchange = "NFO" if self.underlying == "FINNIFTY" else "NSE"
+        self.underlying_exchange = "NFO" if self.underlying in ["FINNIFTY", "MIDCPNIFTY"] else "NSE"  # Fin/Mid temp fix
         self.expiry = expiry
         self.call_symbol, self.call_token = self.call_option.fetch_symbol_token()
         self.put_symbol, self.put_token = self.put_option.fetch_symbol_token()
         self.freeze_qty_in_shares = self.call_option.freeze_qty_in_shares
         self.freeze_qty_in_lots = self.call_option.freeze_qty_in_lots
         self.lot_size = self.call_option.lot_size
 
@@ -553,54 +574,117 @@
 
     def fetch_total_ltp(self):
         call_ltp, put_ltp = fetchltp(
             "NFO", self.call_symbol, self.call_token
         ), fetchltp("NFO", self.put_symbol, self.put_token)
         return call_ltp + put_ltp
 
+    def price_disparity(self):
+        call_ltp, put_ltp = self.fetch_ltp()
+        disparity = abs(call_ltp - put_ltp)/min(call_ltp, put_ltp)
+        return disparity
+
     def fetch_symbol_token(self):
         return self.call_symbol, self.call_token, self.put_symbol, self.put_token
 
-    def place_order(self, transaction_type, quantity_in_lots, prices="LIMIT", order_tag=""):
-        if isinstance(prices, (tuple, list, np.ndarray)):
+    def place_order(self, transaction_type, quantity_in_lots, prices="LIMIT", stop_loss_order=False, order_tag=""):
+
+        if stop_loss_order:
+            assert isinstance(prices, (tuple, list, np.ndarray)), "Prices must be a tuple of prices for stop loss order"
             call_price, put_price = prices
-        elif prices.upper() == "LIMIT":
-            call_price, put_price = self.fetch_ltp()
-            modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
-            call_price, put_price = call_price * modifier, put_price * modifier
-        elif prices.upper() == "MARKET":
-            call_price = put_price = prices
         else:
-            raise ValueError("Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices")
+            if isinstance(prices, (tuple, list, np.ndarray)):
+                call_price, put_price = prices
+            elif prices.upper() == "LIMIT":
+                call_price, put_price = self.fetch_ltp()
+                modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
+                call_price, put_price = call_price * modifier, put_price * modifier
+            elif prices.upper() == "MARKET":
+                call_price = put_price = prices
+            else:
+                raise ValueError("Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices")
 
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
+                stop_loss_order=stop_loss_order,
                 order_tag=order_tag
             )
             put_order_id = place_order(
-                self.put_symbol, self.put_token, qty * self.lot_size, transaction_type, put_price, order_tag=order_tag
+                self.put_symbol,
+                self.put_token,
+                qty * self.lot_size,
+                transaction_type,
+                put_price,
+                stop_loss_order=stop_loss_order,
+                order_tag=order_tag
             )
             call_order_ids.append(call_order_id)
             put_order_ids.append(put_order_id)
         return call_order_ids, put_order_ids
 
 
 class Straddle(Strangle):
     def __init__(self, strike, underlying, expiry):
         super().__init__(strike, strike, underlying, expiry)
 
 
+class SyntheticFuture(Strangle):
+    def __init__(self, strike, underlying, expiry):
+        super().__init__(strike, strike, underlying, expiry)
+
+    def place_order(
+            self, transaction_type, quantity_in_lots, prices: str | tuple = "LIMIT", stop_loss_order=False, order_tag=""
+    ):
+        if isinstance(prices, (tuple, list, np.ndarray)):
+            call_price, put_price = prices
+        elif prices.upper() == "LIMIT":
+            call_price, put_price = self.fetch_ltp()
+            c_modifier, p_modifier = (1.05, 0.95) if transaction_type.upper() == "BUY" else (0.95, 1.05)
+            call_price, put_price = call_price * c_modifier, put_price * p_modifier
+        elif prices.upper() == "MARKET":
+            call_price = put_price = prices
+        else:
+            raise ValueError("Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices")
+
+        call_transaction_type = "BUY" if transaction_type.upper() == "BUY" else "SELL"
+        put_transaction_type = "SELL" if transaction_type.upper() == "BUY" else "BUY"
+
+        spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
+        call_order_ids = []
+        put_order_ids = []
+        for qty in spliced_orders:
+            call_order_id = place_order(
+                self.call_symbol,
+                self.call_token,
+                qty * self.lot_size,
+                call_transaction_type,
+                call_price,
+                order_tag=order_tag
+            )
+            put_order_id = place_order(
+                self.put_symbol,
+                self.put_token,
+                qty * self.lot_size,
+                put_transaction_type,
+                put_price,
+                order_tag=order_tag
+            )
+            call_order_ids.append(call_order_id)
+            put_order_ids.append(put_order_id)
+        return call_order_ids, put_order_ids
+
+
 class SyntheticArbSystem:
     def __init__(self, symbol_option_chains):
         self.symbol_option_chains = symbol_option_chains
         self.index_expiry_pairs = {}
         self.successful_trades = 0
         self.unsuccessful_trades = 0
 
@@ -632,18 +716,17 @@
             np.array(put_ask_qty),
         )
 
     def find_arbitrage_opportunities(
         self,
         index: str,
         expiry: str,
-        qty: int,
+        qty_in_lots: int,
         exit_time=(15, 28),
         threshold=3,
-        at_market=False,
     ):
         (
             strikes,
             call_prices,
             put_prices,
             call_bids,
             call_asks,
@@ -675,36 +758,25 @@
 
             if max_price - min_price > threshold:
                 print(
                     f"**********Trade Identified at {currenttime()} on strike: Min {strikes[min_price_index]} "
                     f"and Max {strikes[max_price_index]}**********\n"
                     f"Minimum price: {min_price} at strike: {strikes[min_price_index]} Call Ask: {call_asks[min_price_index]} Put Bid: {put_bids[min_price_index]}\n"
                     f"Maximum price: {max_price} at strike: {strikes[max_price_index]} Call Bid: {call_bids[max_price_index]} Put Ask: {put_asks[max_price_index]}\n"
-                    f"Price difference: {max_price - min_price}\nExpected Profit: {(max_price - min_price) * qty}\n"
+                    f"Price difference: {max_price - min_price}\n"
                 )
                 min_strike = strikes[min_price_index]
                 max_strike = strikes[max_price_index]
-                min_strike_call_ask = call_asks[min_price_index]
-                min_strike_put_bid = put_bids[min_price_index]
-                max_strike_call_bid = call_bids[max_price_index]
-                max_strike_put_ask = put_asks[max_price_index]
-                if at_market:
-                    buy_prices = "MARKET"
-                    sell_prices = "MARKET"
-                else:
-                    buy_prices = (min_strike_call_ask, min_strike_put_bid)
-                    sell_prices = (max_strike_call_bid, max_strike_put_ask)
+
                 self.execute_synthetic_trade(
                     index,
                     expiry,
-                    qty,
+                    qty_in_lots,
                     min_strike,
-                    buy_prices,
                     max_strike,
-                    sell_prices,
                     sleep_interval=5,
                 )
 
             for i, strike in enumerate(strikes):
                 call_prices[i] = self.symbol_option_chains[index][expiry][strike][
                     "call_price"
                 ]
@@ -738,82 +810,37 @@
             synthetic_buy_prices = strikes + call_asks - put_bids
             synthetic_sell_prices = strikes + call_bids - put_asks
             min_price_index = np.argmin(synthetic_buy_prices)
             max_price_index = np.argmax(synthetic_sell_prices)
             min_price = synthetic_buy_prices[min_price_index]
             max_price = synthetic_sell_prices[max_price_index]
 
+    @staticmethod
     def execute_synthetic_trade(
-        self,
         index,
         expiry,
-        qty,
+        qty_in_lots,
         buy_strike,
-        buy_strike_prices,
         sell_strike,
-        sell_strike_prices,
         sleep_interval=1,
     ):
-        id_call_buy, id_put_sell = place_synthetic_fut_order(
-            index, buy_strike, expiry, "BUY", qty, buy_strike_prices
-        )
-        id_call_sell, id_put_buy = place_synthetic_fut_order(
-            index, sell_strike, expiry, "SELL", qty, sell_strike_prices
-        )
-        ids = [id_call_buy, id_put_sell, id_call_sell, id_put_buy]
-        call_buy_token, call_buy_symbol = fetch_symbol_token(
-            index, expiry, buy_strike, "CE"
-        )
-        put_sell_token, put_sell_symbol = fetch_symbol_token(
-            index, expiry, buy_strike, "PE"
-        )
-        call_sell_token, call_sell_symbol = fetch_symbol_token(
-            index, expiry, sell_strike, "CE"
+        ids_call_buy, ids_put_sell = place_synthetic_fut_order(
+            index, buy_strike, expiry, "BUY", qty_in_lots, 'MARKET'
         )
-        put_buy_token, put_buy_symbol = fetch_symbol_token(
-            index, expiry, sell_strike, "PE"
+        ids_call_sell, ids_put_buy = place_synthetic_fut_order(
+            index, sell_strike, expiry, "SELL", qty_in_lots, 'MARKET'
         )
+        ids = np.concatenate((ids_call_buy, ids_put_sell, ids_call_sell, ids_put_buy))
+
         sleep(sleep_interval)
         statuses = lookup_and_return("orderbook", "orderid", ids, "status")
-        if any(statuses == "open"):
-            # Finding the open order ids using statues and ids and cancelling them in the fastest way possible
-            open_order_ids = [
-                ids[i] for i, status in enumerate(statuses) if status == "open"
-            ]
-            cancel_pending_orders(open_order_ids)
 
-            # Reversing the trade which got executed
-            for i, status in enumerate(statuses):
-                if status == "complete":
-                    if i == 0:
-                        place_order(
-                            call_buy_symbol, call_buy_token, qty, "SELL", "MARKET"
-                        )
-                    elif i == 1:
-                        place_order(
-                            put_sell_symbol, put_sell_token, qty, "BUY", "MARKET"
-                        )
-                    elif i == 2:
-                        place_order(
-                            call_sell_symbol, call_sell_token, qty, "BUY", "MARKET"
-                        )
-                    elif i == 3:
-                        place_order(put_buy_symbol, put_buy_token, qty, "SELL", "MARKET")
-            logger.info(
-                f"Order cancelled and reversed for {index} {expiry} {qty} Buy {buy_strike} Sell {sell_strike}"
-            )
-            self.unsuccessful_trades += 1
-        elif all(statuses == "complete"):
-            self.successful_trades += 1
-            logger.info(
-                f"Order executed for {index} {expiry} {qty} Buy {buy_strike} Sell {sell_strike}"
-            )
-        elif any(statuses == "rejected"):
+        if any(statuses == "rejected"):
             logger.error(
-                f"Order rejected for {index} {expiry} {qty} Buy {buy_strike} Sell {sell_strike}"
+                f"Order rejected for {index} {expiry} {qty_in_lots} Buy {buy_strike} Sell {sell_strike}"
             )
 
 
 class Index:
     """Initialize an index with the name of the index in uppercase"""
 
     def __init__(self, name, webhook_url=None, websocket=None, spot_future_rate=0.06):
@@ -849,15 +876,15 @@
 
         if self.name == "BANKNIFTY":
             self.base = 100
             self.exchange_type = 1
         elif self.name == "NIFTY":
             self.base = 50
             self.exchange_type = 1
-        elif self.name == "FINNIFTY":
+        elif self.name in ["FINNIFTY", "MIDCPNIFTY"]:  # Finnifty and Midcpnifty temp fix
             self.base = 50
             self.exchange_type = 2
         else:
             self.base = get_base(self.name)
             self.exchange_type = 1
             logger.info(f"Base for {self.name} is {self.base}")
             # print(f"Base for {self.name} is {self.base}")
@@ -957,16 +984,16 @@
 
         self.current_expiry = currentexpiry
         self.next_expiry = nextexpiry
         self.month_expiry = monthexpiry
         self.fut_expiry = futexpiry
 
     def fetch_ltp(self):
-        """Fetch LTP of the index. Uses futures for FINNIFTY"""
-        if self.name == "FINNIFTY":
+        """Fetch LTP of the index. Uses futures for FINNIFTY and MIDCPNIFTY"""
+        if self.name in ["FINNIFTY", "MIDCPNIFTY"]:  # Finnifty & Midcpnifty temp fix
             ltp = fetchltp("NFO", self.symbol, self.token)
             self.ltp = spot_price_from_future(
                 ltp, self.spot_future_rate, timetoexpiry(self.fut_expiry)
             )
         else:
             self.ltp = fetchltp("NSE", self.symbol, self.token)
         return self.ltp
@@ -1076,15 +1103,15 @@
             "Tag": order_tag,
         }
         self.order_log[order_tag].append(dict_format)
 
     def splice_orders(self, quantity_in_lots):
         if quantity_in_lots > self.freeze_qty:
             loops = int(quantity_in_lots / self.freeze_qty)
-            if loops > large_order_threshold:
+            if loops > LARGE_ORDER_THRESHOLD:
                 raise Exception(
                     "Order too big. This error was raised to prevent accidental large order placement."
                 )
 
             remainder = quantity_in_lots % self.freeze_qty
             if remainder == 0:
                 spliced_orders = [self.freeze_qty] * loops
@@ -1227,124 +1254,34 @@
             notifier(
                 f"{order_prefix}ERROR. Order statuses uncertain for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s).",
                 self.webhook_url,
             )
             raise Exception("Order statuses uncertain")
 
-    def place_synthetic_fut_order(
-        self,
-        strike,
-        expiry,
-        buy_or_sell,
-        quantity_in_lots,
-        prices="LIMIT",
-        check_status=True,
+    def place_synthetic_fut(
+            self, strike, expiry, buy_or_sell, quantity_in_lots, prices="LIMIT", stop_loss_order=False, order_tag=""
     ):
-        """Places a synthetic future order. Quantity is in number of shares."""
-        name = self.name
-        strike = int(strike)
-        expiry = expiry
-        buy_or_sell = buy_or_sell
-        spliced_orders = self.splice_orders(quantity_in_lots)
-        straddle = Straddle(strike, name, expiry)
-        call_symbol, call_token, put_symbol, put_token = straddle.fetch_symbol_token()
-        if prices == "LIMIT":
-            call_price, put_price = straddle.fetch_ltp()
-            if buy_or_sell == "BUY":
-                call_price = call_price * 1.05
-                put_price = put_price * 0.95
-            else:
-                call_price = call_price * 0.95
-                put_price = put_price * 1.05
-        elif prices == "MARKET":
-            call_price = "MARKET"
-            put_price = "MARKET"
-        else:
-            call_price, put_price = prices
-
-        call_action = "BUY" if buy_or_sell == "BUY" else "SELL"
-        put_action = "SELL" if buy_or_sell == "BUY" else "BUY"
-
-        order_ids_call = []
-        order_ids_put = []
-        for quantity in spliced_orders:
-            quantity_in_shares = quantity * self.lot_size
-
-            order_id_call = place_order(
-                call_symbol, call_token, quantity_in_shares, call_action, call_price
-            )
-            order_id_put = place_order(
-                put_symbol, put_token, quantity_in_shares, put_action, put_price
-            )
-            if check_status:
-                order_ids_call.append(order_id_call)
-                order_ids_put.append(order_id_put)
-
-        if check_status:
-            orderbook = fetch_book("orderbook")
-
-            call_order_statuses = lookup_and_return(
-                orderbook, "orderid", order_ids_call, "status"
-            )
-            put_order_statuses = lookup_and_return(
-                orderbook, "orderid", order_ids_put, "status"
-            )
-
-            if all(call_order_statuses == "complete") and all(
-                put_order_statuses == "complete"
-            ):
-                logger.info(
-                    f"Synthetic Order(s) placed successfully for {buy_or_sell} {name} {strike} {expiry} "
-                    f"{quantity_in_lots} lot(s)."
-                )
-                print(
-                    f"Synthetic Order(s) placed successfully for {buy_or_sell} {name} {strike} {expiry} "
-                    f"{quantity_in_lots} lot(s)."
-                )
-            elif all(call_order_statuses == "rejected") and all(
-                put_order_statuses == "rejected"
-            ):
-                logger.info(
-                    f"All synthetic orders rejected for {buy_or_sell} {name} {strike} "
-                    f"{expiry} {quantity_in_lots} lot(s)."
-                )
-                print(
-                    f"All synthetic orders rejected for {buy_or_sell} {name} {strike} "
-                    f"{expiry} {quantity_in_lots} lot(s)."
-                )
-            elif any(call_order_statuses == "pending") and any(
-                put_order_statuses == "pending"
-            ):
-                logger.info(
-                    f"Some synthetic orders pending for {buy_or_sell} {name} {strike} "
-                    f"{expiry} {quantity_in_lots} lot(s)."
-                )
-                print(
-                    f"Some synthetic orders pending for {buy_or_sell} {name} {strike} "
-                    f"{expiry} {quantity_in_lots} lot(s)."
-                )
-            else:
-                logger.error(
-                    f"ERROR. Synthetic order statuses uncertain for {buy_or_sell} {name} {strike} "
-                    f"{expiry} {quantity_in_lots} lot(s)."
-                )
+        return place_synthetic_fut_order(
+            self.name, strike, expiry, buy_or_sell, quantity_in_lots, prices, stop_loss_order, order_tag
+        )
 
+    @time_the_function
     def find_equal_strike(
         self, exit_time, websocket, wait_for_equality, target_disparity, expiry=None
     ):
         expiry = expiry or self.current_expiry
         ltp = (
             self.fetch_ltp()
             if not websocket
             else websocket.price_dict.get(self.token, 0)["ltp"]
         )
         current_strike = findstrike(ltp, self.base)
         strike_range = np.arange(
-            current_strike - self.base * 2, current_strike + self.base * 2, self.base
+            current_strike - self.base * 2, current_strike + self.base * 3, self.base
         )
 
         def fetch_data(strike, exp):
             c_symbol, c_token = fetch_symbol_token(self.name, exp, strike, "CE")
             p_symbol, p_token = fetch_symbol_token(self.name, exp, strike, "PE")
             return c_symbol, c_token, p_symbol, p_token
 
@@ -1386,16 +1323,22 @@
 
         call_ltps, put_ltps = fetch_ltps(
             call_token_list, call_symbol_list, websocket
         ), fetch_ltps(put_token_list, put_symbol_list, websocket)
         disparities = compute_disparities(call_ltps, put_ltps)
 
         if wait_for_equality:
+
             last_print_time = currenttime()
-            print_interval = timedelta(seconds=0.0005)
+            last_log_time = currenttime()
+            last_notify_time = currenttime()
+            print_interval = timedelta(seconds=0.05)
+            log_interval = timedelta(minutes=1)
+            notify_interval = timedelta(minutes=2)
+
             min_disparity_idx = np.argmin(disparities)
             min_disparity = disparities[min_disparity_idx]
 
             while min_disparity > target_disparity:
                 if min_disparity < 10:
                     # Update only the minimum disparity strike data
                     call_ltp, put_ltp = fetch_ltps(
@@ -1417,24 +1360,30 @@
                         call_token_list, call_symbol_list, websocket
                     ), fetch_ltps(put_token_list, put_symbol_list, websocket)
                     disparities = compute_disparities(call_ltps, put_ltps)
                     single_check = False
 
                 min_disparity_idx = np.argmin(disparities)
                 min_disparity = disparities[min_disparity_idx]
-
-                if (currenttime() - last_print_time) > print_interval:
-                    print(
-                        f'Time: {currenttime().strftime("%H:%M:%S")}\n'
-                        + f"Index: {self.name}\n"
-                        + f"Current lowest disparity: {min_disparity:.2f}\n"
-                        + f"Strike: {strike_range[min_disparity_idx]}\n"
-                        + f"Single Strike: {single_check}\n"
-                    )
+                message = (
+                    f'Time: {currenttime().strftime("%H:%M:%S")}\n'
+                    + f"Index: {self.name}\n"
+                    + f"Current lowest disparity: {min_disparity:.2f}\n"
+                    + f"Strike: {strike_range[min_disparity_idx]}\n"
+                    + f"Single Strike: {single_check}\n"
+                )
+                if currenttime() - last_print_time > print_interval:
+                    print(message)
                     last_print_time = currenttime()
+                if currenttime() - last_log_time > log_interval:
+                    logger.info(message)
+                    last_log_time = currenttime()
+                if currenttime() - last_notify_time > notify_interval:
+                    notifier(message, self.webhook_url)
+                    last_notify_time = currenttime()
 
                 if (currenttime() + timedelta(minutes=5)).time() > time(*exit_time):
                     notifier(
                         "Equal strike tracker exited due to time limit.",
                         self.webhook_url,
                     )
                     raise Exception("Equal strike tracker exited due to time limit.")
@@ -1644,14 +1593,15 @@
                                         call_price=call_buy_avg, put_price=put_buy_avg, order_tag=order_tag)
                 self.log_combined_order(sell_strike, expiry=self.current_expiry, buy_or_sell="SELL",
                                         call_price=call_sell_avg, put_price=put_sell_avg, order_tag=order_tag)
 
         trade_data[self.name] = sell_strike
         save_data(trade_data)
 
+    @log_errors
     def buy_weekly_hedge(
         self,
         quantity_in_lots,
         type_of_hedge="strangle",
         strike_offset=1,
         call_offset=1,
         put_offset=1,
@@ -1978,16 +1928,16 @@
                             notifier(
                                 f"{self.name} Convert to butterfly triggered\n",
                                 self.webhook_url,
                             )
                             ctb_trg = True
                             ctb_message = f"Hedged with: {ctb_hedge}\n"
                             ctb_notification_sent = True
-                    except Exception as e:
-                        print(f"Error in process_ctb: {e}")
+                    except Exception as _e:
+                        print(f"Error in process_ctb: {_e}")
 
                 # Continuously calculate IV
                 call_iv, put_iv, avg_iv = straddle_iv(
                     call_price,
                     put_price,
                     underlying_price,
                     equal_strike,
@@ -2057,110 +2007,28 @@
                         + f"Profit in points: {profit_in_pts:0.2f}\n"
                         + f"Profit Value: {profit_in_rs:0.2f}\n"
                         + f"IV: {print_iv * 100:0.2f}\nSmart Exit: {smart_exit_trg}\n"
                         + ctb_message
                     )
                     last_print_time = currenttime()
 
-        def process_order_statuses(
-            order_book, order_ids, stop_loss=False, notify_url=None, context=""
-        ):
-            nonlocal orderbook
-
-            pending_text = "trigger pending" if stop_loss else "open"
-            context = f"{context} " if context else ""
-
-            statuses = lookup_and_return(order_book, "orderid", order_ids, "status")
-
-            if isinstance(statuses, (int, np.int32, np.int64)):
-                logger.error(f"Statuses is {statuses} for orderid(s) {order_ids}")
-
-            if all(statuses == pending_text):
-                return False, False
-
-            elif all(statuses == "rejected") or all(statuses == "cancelled"):
-                rejection_reasons = lookup_and_return(
-                    order_book, "orderid", order_ids, "text"
-                )
-                if all(
-                    rejection_reasons == "17070 : The Price is out of the LPP range"
-                ):
-                    return True, False
-                else:
-                    notifier(
-                        f"{context}Order rejected or cancelled. Reasons: {rejection_reasons[0]}",
-                        notify_url,
-                    )
-                    raise Exception(f"Orders rejected or cancelled.")
-
-            elif stop_loss and all(statuses == "pending"):
-                sleep(1)
-                orderbook = fetch_book("orderbook")
-                statuses = lookup_and_return(orderbook, "orderid", order_ids, "status")
-
-                if all(statuses == "pending"):
-                    try:
-                        cancel_pending_orders(order_ids, "NORMAL")
-                    except Exception as e:
-                        try:
-                            cancel_pending_orders(order_ids, "STOPLOSS")
-                        except Exception as e:
-                            notifier(
-                                f"{context}Could not cancel orders: {e}", notify_url
-                            )
-                            raise Exception(f"Could not cancel orders: {e}")
-                    notifier(
-                        f"{context}Orders pending and cancelled. Please check.",
-                        notify_url,
-                    )
-                    return True, False
-
-                elif all(statuses == "complete"):
-                    return True, True
-
-                else:
-                    raise Exception(f"Orders in unknown state.")
-
-            elif all(statuses == "complete"):
-                return True, True
-
-            else:
-                notifier(
-                    f"{context}Orders in unknown state. Statuses: {statuses}",
-                    notify_url,
-                )
-                raise Exception(f"Orders in unknown state.")
-
-        def fetch_orderbook_if_needed(
-            data_class=shared_data, refresh_needed: bool = False
-        ):
-            if data_class is None or refresh_needed:
-                return fetch_book("orderbook")
-            if (
-                currenttime() - data_class.updated_time < timedelta(seconds=15)
-                and data_class.orderbook_data is not None
-            ):
-                return data_class.orderbook_data
-            return fetch_book("orderbook")
-
         def check_sl_orders(order_ids, side: str, data=shared_data, refresh=False):
             """This function checks if the stop loss orders have been triggered or not. It also updates the order book
             in the nonlocal scope. This function is responsible for setting the exit prices.
             """
 
             nonlocal orderbook, call_exit_price, put_exit_price, call_price, put_price, underlying_price
             nonlocal traded_call_iv, traded_put_iv, traded_avg_iv, call_iv, put_iv, avg_iv, entry_spot
 
             orderbook = fetch_orderbook_if_needed(data, refresh)
-            triggered, complete = process_order_statuses(
+            triggered, complete = process_stop_loss_order_statuses(
                 orderbook,
                 order_ids,
-                stop_loss=True,
-                notify_url=self.webhook_url,
                 context=f"SL: {side}",
+                notify_url=self.webhook_url
             )
 
             if not triggered and not complete:
                 return False, False
 
             # Checking if there has been an unjustified trigger of stoploss without much movement in the underlying
             # We will also use IV to check if the stoploss was justified or not
@@ -2584,37 +2452,41 @@
 
     @log_errors
     def intraday_strangle(
         self,
         quantity_in_lots,
         call_strike_offset=0,
         put_strike_offset=0,
-        stop_loss=1.6,
+        stop_loss='dynamic',
         call_stop_loss=None,
         put_stop_loss=None,
         exit_time=(15, 29),
         sleep_time=5,
         catch_trend=False,
         trend_qty_ratio=1,
         trend_strike_offset=0,
         trend_sl=0.003,
-        place_sl_orders=False
+        disparity_threshold=np.inf,
+        place_sl_orders=False,
+        move_sl_to_cost=False,
+        convert_to_butterfly=False,
+        shared_data=None
     ):
 
-        """Intraday strangle strategy. Trades strangle with  stop loss. All offsets are in percentage terms.
+        """Intraday strangle strategy. Trades strangle with stop loss. All offsets are in percentage terms.
         Parameters
         ----------
         quantity_in_lots : int
             Quantity in lots
         call_strike_offset : float, optional
             Call strike offset in percentage terms, by default 0
         put_strike_offset : float, optional
             Put strike offset in percentage terms, by default 0
-        stop_loss : float, optional
-            Stop loss percentage, by default 1.6
+        stop_loss : float or string, optional
+            Stop loss percentage, by default 'dynamic'
         call_stop_loss : float, optional
             Call stop loss percentage, by default None. If None then stop loss is same as stop_loss.
         put_stop_loss : float, optional
             Put stop loss percentage, by default None. If None then stop loss is same as stop_loss.
         exit_time : tuple, optional
             Exit time, by default (15, 29)
         sleep_time : int, optional
@@ -2623,57 +2495,96 @@
             Catch trend or not, by default False
         trend_qty_ratio : int, optional
             Ratio of trend quantity to strangle quantity, by default 1
         trend_strike_offset : float, optional
             Strike offset for trend order in percentage terms, by default 0
         trend_sl : float, optional
             Stop loss for trend order, by default 0.003
+        disparity_threshold : float, optional
+            Disparity threshold for equality of strikes, by default np.inf
         place_sl_orders : bool, optional
             Place stop loss orders or not, by default False
+        move_sl_to_cost : bool, optional
+            Move other stop loss to cost or not, by default False
+        convert_to_butterfly : bool, optional
+            Convert to butterfly or not, by default False
+        shared_data : SharedData class, optional
+            shared data about client level orderbook and positions, by default None
         """
 
         @log_errors
         def position_monitor(info_dict):
 
             c_avg_price = info_dict["call_avg_price"]
             p_avg_price = info_dict["put_avg_price"]
             traded_strangle = info_dict["traded_strangle"]
 
             # Price deque
             n_prices = max(int(30/sleep_time), 1)  # Hard coded 30-second price window for now
-            last_n_prices = {"call": deque(maxlen=n_prices), "put": deque(maxlen=n_prices)}
+            last_n_prices = {
+                "call": deque(maxlen=n_prices), "put": deque(maxlen=n_prices), "underlying": deque(maxlen=n_prices)
+            }
+
+            # Conversion to butterfly
+            ctb_notification_sent = False
+            ctb_message = ""
+            c_sl = call_stop_loss if call_stop_loss is not None else stop_loss
+            p_sl = put_stop_loss if put_stop_loss is not None else stop_loss
+            profit_if_call_sl = p_avg_price - (c_avg_price * (c_sl - 1))
+            profit_if_put_sl = c_avg_price - (p_avg_price * (p_sl - 1))
+            ctb_threshold = max(profit_if_call_sl, profit_if_put_sl)
+
+            def process_ctb(profit_threshold):
+
+                hedge_call_strike = traded_strangle.call_strike + self.base
+                hedge_put_strike = traded_strangle.put_strike + self.base
+                h_strangle = Strangle(hedge_call_strike, hedge_put_strike, self.name, expiry)
+                hedge_total_ltp = h_strangle.fetch_total_ltp()
+
+                hedge_profit = info_dict["total_avg_price"] - hedge_total_ltp - self.base
+
+                logging.info(f"{self.name} CTB threshold: {profit_threshold}, Hedge working: {hedge_profit}")
+
+                if hedge_profit >= profit_threshold:
+                    return h_strangle
+                else:
+                    return None
 
             last_print_time = currenttime()
             last_log_time = currenttime()
             last_notify_time = currenttime()
             print_interval = timedelta(seconds=5)
             log_interval = timedelta(minutes=60)
             notify_interval = timedelta(minutes=180)
 
-            while not info_dict["exit_triggers"]["trade_complete"]:
+            while not info_dict["trade_complete"]:
 
                 # Fetching prices
                 spot_price = self.fetch_ltp()
                 c_ltp, p_ltp = traded_strangle.fetch_ltp()
                 info_dict["underlying_ltp"] = spot_price
                 info_dict["call_ltp"] = c_ltp
                 info_dict["put_ltp"] = p_ltp
                 last_n_prices["call"].append(c_ltp)
                 last_n_prices["put"].append(p_ltp)
+                last_n_prices["underlying"].append(spot_price)
                 c_ltp_avg = sum(last_n_prices["call"])/len(last_n_prices["call"]) if last_n_prices["call"] else c_ltp
                 p_ltp_avg = sum(last_n_prices["put"])/len(last_n_prices["put"]) if last_n_prices["put"] else p_ltp
+                spot_price_avg = sum(last_n_prices["underlying"])/len(last_n_prices["underlying"]) \
+                    if last_n_prices["underlying"] else spot_price
                 info_dict["call_ltp_avg"] = c_ltp_avg
                 info_dict["put_ltp_avg"] = p_ltp_avg
+                info_dict["underlying_ltp_avg"] = spot_price_avg
 
                 # Calculate IV
                 call_iv, put_iv, avg_iv = strangle_iv(
                     callprice=c_ltp,
                     putprice=p_ltp,
-                    callstrike=call_strike,
-                    putstrike=put_strike,
+                    callstrike=traded_strangle.call_strike,
+                    putstrike=traded_strangle.put_strike,
                     spot=spot_price,
                     timeleft=timetoexpiry(expiry)
                 )
                 info_dict["call_iv"] = call_iv
                 info_dict["put_iv"] = put_iv
                 info_dict["avg_iv"] = avg_iv
 
@@ -2684,42 +2595,83 @@
 
                 # Calculate profit
                 profit_in_pts = (c_avg_price + p_avg_price) - mtm_price
                 profit_in_rs = profit_in_pts * self.lot_size * quantity_in_lots
                 info_dict["profit_in_pts"] = profit_in_pts
                 info_dict["profit_in_rs"] = profit_in_rs
 
+                # Conversion to butterfly working
+                if (
+                        not (info_dict["call_sl"] or info_dict["put_sl"])
+                        and info_dict["time_left_day_start"] * 365 < 1
+                        and convert_to_butterfly
+                        and not ctb_notification_sent
+                ):
+                    try:
+                        ctb_hedge = process_ctb(ctb_threshold)
+                        if ctb_hedge is not None:
+                            notifier(
+                                f"{self.name} Convert to butterfly triggered\n",
+                                self.webhook_url,
+                            )
+                            info_dict["exit_triggers"].update({"convert_to_butterfly": True})
+                            ctb_message = f"Hedged with: {ctb_hedge}\n"
+                            info_dict["ctb_hedge"] = ctb_hedge
+                            ctb_notification_sent = True
+                    except Exception as _e:
+                        logging.info(f"Error in process_ctb: {_e}")
+
                 message = (
                     f"\nUnderlying: {self.name}\n"
                     f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
                     f"Underlying LTP: {spot_price}\n"
-                    f"Call Strike: {call_strike}\n"
-                    f"Put Strike: {put_strike}\n"
+                    f"Call Strike: {traded_strangle.call_strike}\n"
+                    f"Put Strike: {traded_strangle.put_strike}\n"
                     f"Call Price: {c_ltp}\n"
                     f"Put Price: {p_ltp}\n"
                     f"MTM Price: {mtm_price}\n"
                     f"Call last n avg: {c_ltp_avg}\n"
                     f"Put last n avg: {p_ltp_avg}\n"
                     f"IVs: {call_iv}, {put_iv}, {avg_iv}\n"
                     f"Call SL: {info_dict['call_sl']}\n"
                     f"Put SL: {info_dict['put_sl']}\n"
                     f"Profit Pts: {info_dict['profit_in_pts']:.2f}\n"
                     f"Profit: {info_dict['profit_in_rs']:.2f}\n"
+                    + ctb_message
                 )
                 if currenttime() - last_print_time > print_interval:
                     print(message)
                     last_print_time = currenttime()
                 if currenttime() - last_log_time > log_interval:
                     logger.info(message)
                     last_log_time = currenttime()
                 if currenttime() - last_notify_time > notify_interval:
                     notifier(message, self.webhook_url)
                     last_notify_time = currenttime()
                 sleep(sleep_time)
 
+        def get_range_of_strangles(c_strike, p_strike, exp, range_of_strikes=4):
+            if range_of_strikes % 2 != 0:
+                range_of_strikes += 1
+            c_strike_range = np.arange(
+                c_strike - (range_of_strikes / 2) * self.base,
+                c_strike + (range_of_strikes / 2) * self.base + self.base,
+                self.base
+            )
+            if c_strike == p_strike:
+                return [Straddle(strike, self.name, exp) for strike in c_strike_range]
+            else:
+                p_strike_ranges = np.arange(
+                        p_strike - (range_of_strikes/2)*self.base,
+                        p_strike + (range_of_strikes/2)*self.base + self.base,
+                        self.base
+                )
+                pairs = itertools.product(c_strike_range, p_strike_ranges)
+                return [Strangle(pair[0], pair[1], self.name, exp) for pair in pairs]
+
         @log_errors
         def trend_catcher(info_dict, sl_type, qty_ratio, sl, strike_offset):
 
             offset = 1-strike_offset if sl_type == "call" else 1+strike_offset
 
             spot_price = info_dict["underlying_ltp"]
 
@@ -2745,26 +2697,27 @@
                 + f"Placed {qty_in_lots} lots of {strike} {opt_type} at {trend_option.fetch_ltp()}. "
                 + f"Stoploss price: {sl_price}, Underlying Price: {spot_price}",
                 self.webhook_url,
             )
 
             last_print_time = currenttime()
             print_interval = timedelta(seconds=10)
-            while all([currenttime().time() < time(*exit_time), not info_dict["exit_triggers"]["trade_complete"]]):
+            while all([currenttime().time() < time(*exit_time), not info_dict["trade_complete"]]):
                 spot_price = info_dict["underlying_ltp"]
-                trend_sl_hit = spot_price < sl_price if sl_type == "call" else spot_price > sl_price
+                spot_price_avg = info_dict["underlying_ltp_avg"]
+                trend_sl_hit = spot_price_avg < sl_price if sl_type == "call" else spot_price_avg > sl_price
                 if trend_sl_hit:
                     break
-                sleep(1)
+                sleep(sleep_time)
                 if currenttime() - last_print_time > print_interval:
                     last_print_time = currenttime()
                     print(
                         f"{self.name} {sl_type} trend catcher running\n"
-                        + f"Stoploss price: {sl_price}, Underlying Price: {spot_price}\n"
-                        + f"Stoploss hit: {trend_sl_hit}\n"
+                        + f"Stoploss price: {sl_price}, Underlying price: {spot_price}\n"
+                        + f"Underlying price avg: {spot_price_avg}, Stoploss hit: {trend_sl_hit}\n"
                     )
 
             if trend_sl_hit:
                 notifier(
                     f"{self.name} strangle {sl_type} trend catcher stoploss hit.", self.webhook_url
                 )
             else:
@@ -2773,224 +2726,345 @@
                 )
 
             # Buying the trend option back
             place_option_order_and_notify(
                 trend_option, "BUY", qty_in_lots, "LIMIT", "Intraday Strangle Trend Catcher", self.webhook_url
             )
 
-        def check_for_stop_loss(info_dict, side, sl_order_ids=None):
-
-            if sl_order_ids is None:  # Not using SL orders
-                sl = info_dict[f"{side}_ltp_avg"] > info_dict[f"{side}_stop_loss_price"]
+        def justify_stop_loss(info_dict, side):
 
-            else:  # Using SL orders
-                sl = False
-                pass  # TODO: Implement fetching order status and checking for SL
+            entry_spot = info_dict.get("spot_at_entry")
+            current_spot = info_dict.get("underlying_ltp")
 
-            info_dict[f"{side}_sl"] = sl
+            # If the spot has moved in the direction of stop loss
+            time_left_day_start = info_dict.get("time_left_day_start")
+            time_left_now = timetoexpiry(expiry)
+            time_delta = (time_left_day_start - time_left_now)*525600
+            time_delta = int(time_delta)
+            estimated_movement = bs.target_movement(
+                side,
+                info_dict.get(f"{side}_avg_price"),
+                info_dict.get(f"{side}_stop_loss_price"),
+                entry_spot,
+                info_dict.get("traded_strangle").call_strike if side == "call" else info_dict.get("traded_strangle").put_strike,
+                time_left_day_start,
+                time_delta
+            )
+            actual_movement = (current_spot - entry_spot) / entry_spot
+            difference_in_sign = np.sign(estimated_movement) != np.sign(actual_movement)
+            lack_of_movement = abs(actual_movement) < 0.8 * abs(estimated_movement)
+            # 0.8 above is a magic number TODO: Remove magic number and find a better way to check for lack of movement
+            if difference_in_sign or lack_of_movement:
+                if not info_dict.get(f"{side}_sl_check_notification_sent"):
+                    message = f'{self.name} strangle {side} stop loss appears to be unjustified. ' \
+                              f'Estimated movement: {estimated_movement}, Actual movement: {actual_movement}'
+                    notifier(message, self.webhook_url)
+                    info_dict[f"{side}_sl_check_notification_sent"] = True
+                return False
+            else:
+                message = f"{self.name} strangle {side} stop loss triggered. " \
+                          f"Estimated movement: {estimated_movement}, Actual movement: {actual_movement}"
+                notifier(message, self.webhook_url)
+                return True
+
+        def check_for_stop_loss(info_dict, side, refresh_orderbook=False):
+
+            """Check for stop loss."""
+
+            stop_loss_order_ids = info_dict.get(f"{side}_stop_loss_order_ids")
+
+            if stop_loss_order_ids is None:  # If stop loss order ids are not provided
+                avg_price = info_dict.get(f"{side}_ltp_avg")
+                stop_loss_price = info_dict.get(f"{side}_stop_loss_price")
+                stop_loss_triggered = avg_price > stop_loss_price
+                if stop_loss_triggered:
+                    stop_loss_justified = justify_stop_loss(info_dict, side)
+                    if stop_loss_justified:
+                        info_dict[f"{side}_sl"] = True
+
+            else:  # If stop loss order ids are provided
+                orderbook = fetch_orderbook_if_needed(shared_data, refresh_needed=refresh_orderbook)
+                orders_triggered, orders_complete = process_stop_loss_order_statuses(
+                    orderbook, stop_loss_order_ids, context=side, notify_url=self.webhook_url
+                )
+                if orders_triggered:
+                    justify_stop_loss(info_dict, side)
+                    info_dict[f"{side}_sl"] = True
+                if not orders_complete:
+                    info_dict[f"{side}_sl_order_ids"] = None
 
         def process_stop_loss(info_dict, sl_type):
 
             if info_dict["call_sl"] and info_dict["put_sl"]:  # Check to avoid double processing
                 return
 
             traded_strangle = info_dict["traded_strangle"]
-            # Buying the stop loss option back
-            notifier(f'{self.name} strangle {sl_type} stop loss hit.', self.webhook_url)
-            option_to_buy = traded_strangle.call_option if sl_type == "call" else traded_strangle.put_option
-            exit_price = place_option_order_and_notify(
-                option_to_buy, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
-            )
+            other_side = "call" if sl_type == "put" else "put"
+
+            # Buying the stop loss option back if it is not already bought
+            if info_dict[f"{sl_type}_sl_order_ids"] is None:
+                option_to_buy = traded_strangle.call_option if sl_type == "call" else traded_strangle.put_option
+                exit_price = place_option_order_and_notify(
+                    option_to_buy, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
+                )
+            else:
+                orderbook = fetch_book('orderbook')
+                exit_price = (
+                    lookup_and_return(orderbook, "orderid", info_dict[f"{sl_type}_sl_order_ids"], "averageprice")
+                    .astype(float)
+                    .mean()
+                )
             info_dict[f'{sl_type}_exit_price'] = exit_price
 
+            if move_sl_to_cost:
+                info_dict[f"{other_side}_stop_loss_price"] = info_dict[f"{other_side}_avg_price"]
+                if info_dict[f"{other_side}_stop_loss_order_ids"] is not None:
+                    cancel_pending_orders(info_dict[f"{other_side}_stop_loss_order_ids"], "STOPLOSS")
+                    option_to_repair = (
+                        traded_strangle.call_option if other_side == "call" else traded_strangle.put_option
+                    )
+                    info_dict[f"{other_side}_stop_loss_order_ids"] = place_option_order_and_notify(
+                        instrument=option_to_repair,
+                        action="BUY",
+                        qty_in_lots=quantity_in_lots,
+                        prices=info_dict[f"{other_side}_stop_loss_price"],
+                        order_tag=f"{other_side} SL Strangle",
+                        webhook_url=self.webhook_url,
+                        stop_loss_order=True,
+                        target_status="trigger pending",
+                        return_avg_price=False
+                    )
+
             # Starting the trend catcher
             if catch_trend:
                 trend_thread = Thread(
                     target=trend_catcher,
                     args=(info_dict, sl_type, trend_qty_ratio, trend_sl, trend_strike_offset),
                 )
                 trend_thread.start()
 
+            refresh_orderbook = True
             # Wait for exit or other stop loss to hit
-            other_sl_type = "put" if sl_type == "call" else "call"
             while all([currenttime().time() < time(*exit_time)]):
-                check_for_stop_loss(info_dict, other_sl_type)
-                if info_dict[f"{other_sl_type}_sl"]:
-                    other_sl_option = traded_strangle.put_option if sl_type == "call" else traded_strangle.call_option
-                    notifier(f'{self.name} strangle {other_sl_type} stop loss hit.', self.webhook_url)
-                    other_exit_price = place_option_order_and_notify(
-                        other_sl_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
-                    )
-                    info_dict[f'{other_sl_type}_exit_price'] = other_exit_price
+                check_for_stop_loss(info_dict, other_side, refresh_orderbook=refresh_orderbook)
+                if info_dict[f"{other_side}_sl"]:
+                    if info_dict[f"{other_side}_sl_order_ids"] is None:
+                        other_sl_option = (
+                            traded_strangle.call_option if other_side == "call" else traded_strangle.put_option
+                        )
+                        notifier(f'{self.name} strangle {other_side} stop loss hit.', self.webhook_url)
+                        other_exit_price = place_option_order_and_notify(
+                            other_sl_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
+                        )
+                    else:
+                        orderbook = fetch_book('orderbook')
+                        other_exit_price = (
+                            lookup_and_return(
+                                orderbook, "orderid", info_dict[f"{other_side}_sl_order_ids"], "averageprice"
+                            )
+                            .astype(float)
+                            .mean()
+                        )
+                    info_dict[f'{other_side}_exit_price'] = other_exit_price
                     break
+                refresh_orderbook = False
                 sleep(1)
 
+        # Entering the main function
+
         # Setting strikes and expiry
         order_tag = "Intraday Strangle"
         underlying_ltp = self.fetch_ltp()
-        call_strike = underlying_ltp * (1 + call_strike_offset)
-        put_strike = underlying_ltp * (1 - put_strike_offset)
-        call_strike = findstrike(call_strike, self.base)
-        put_strike = findstrike(put_strike, self.base)
+        temp_call_strike = underlying_ltp * (1 + call_strike_offset)
+        temp_put_strike = underlying_ltp * (1 - put_strike_offset)
+        temp_call_strike = findstrike(temp_call_strike, self.base)
+        temp_put_strike = findstrike(temp_put_strike, self.base)
         expiry = self.current_expiry
 
+        prospective_strangles = get_range_of_strangles(temp_call_strike, temp_put_strike, expiry, range_of_strikes=4)
+        logger.info(f"{self.name} prospective strangles: {prospective_strangles}")
+
         # Placing the main order
-        strangle = Strangle(call_strike=call_strike, put_strike=put_strike, underlying=self.name, expiry=expiry)
-        call_ltp, put_ltp = strangle.fetch_ltp()
-        call_order_ids, put_order_ids = strangle.place_order(
-            "SELL", quantity_in_lots, prices="LIMIT", order_tag=order_tag
+        strangle = most_equal_strangle(
+            *prospective_strangles,
+            disparity_threshold=disparity_threshold,
+            exit_time=(datetime.combine(datetime.now().date(), time(*exit_time)) - timedelta(minutes=5)).time(),
         )
-        orderbook = fetch_book('orderbook')
-        order_statuses = lookup_and_return(orderbook, 'orderid', call_order_ids+put_order_ids, 'status')
-        check_and_notify_order_statuses(
-            order_statuses,
-            self.webhook_url,
-            target_status="complete",
-            order_tag=order_tag,
-            Underlying=self.name,
-            Action="SELL",
-            Strikes=[call_strike, put_strike],
-            Expiry=expiry,
-            Quantity=quantity_in_lots
+        if strangle is None:
+            notifier(
+                f"{self.name} no strangle found within disparity threshold {disparity_threshold}", self.webhook_url
+            )
+            return
+        call_ltp, put_ltp = strangle.fetch_ltp()
+        call_avg_price, put_avg_price = place_option_order_and_notify(
+            strangle, "SELL", quantity_in_lots, "LIMIT", order_tag, self.webhook_url, return_avg_price=True
         )
+        total_avg_price = call_avg_price + put_avg_price
 
-        # Calculating average prices
-        def get_avg_price(book, order_ids, ltp):
-            prices = lookup_and_return(book, ['orderid', 'status'], [order_ids, 'complete'], 'averageprice')
-            return ltp if not isinstance(prices, np.ndarray) else prices.astype(float).mean()
+        # Setting stop loss
+        stop_loss_dict = {
+            "fixed": {"BANKNIFTY": 1.7, "NIFTY": 1.5},
+            "dynamic": {"BANKNIFTY": 1.7, "NIFTY": 1.5}
+        }
 
-        call_avg_price = get_avg_price(orderbook, call_order_ids, call_ltp)
-        put_avg_price = get_avg_price(orderbook, put_order_ids, put_ltp)
-        total_avg_price = call_avg_price + put_avg_price
+        if isinstance(stop_loss, str):
+            if stop_loss == "dynamic" and timetoexpiry(expiry, in_days=True) < 1:
+                stop_loss = 1.7
+            else:
+                stop_loss = stop_loss_dict[stop_loss].get(self.name, 1.6)
+        else:
+            stop_loss = stop_loss
 
         call_stop_loss_price = call_avg_price * call_stop_loss if call_stop_loss else call_avg_price * stop_loss
         put_stop_loss_price = put_avg_price * put_stop_loss if put_stop_loss else put_avg_price * stop_loss
 
         # Logging information and sending notification
         self.log_combined_order(
-            call_strike=call_strike,
-            put_strike=put_strike,
+            call_strike=strangle.call_strike,
+            put_strike=strangle.put_strike,
             expiry=expiry,
             buy_or_sell="SELL",
             call_price=call_avg_price,
             put_price=put_avg_price,
             order_tag=order_tag
         )
 
         summary_message = "\n".join(
             f"{k}: {v}" for k, v in self.order_log[order_tag][-1].items()
         )
 
         traded_call_iv, traded_put_iv, traded_avg_iv = strangle_iv(
             callprice=call_avg_price,
             putprice=put_avg_price,
-            callstrike=call_strike,
-            putstrike=put_strike,
+            callstrike=strangle.call_strike,
+            putstrike=strangle.put_strike,
             spot=underlying_ltp,
             timeleft=timetoexpiry(expiry)
         )
 
+        time_left_at_trade = timetoexpiry(expiry)
         summary_message += f"\nTraded IVs: {traded_call_iv}, {traded_put_iv}, {traded_avg_iv}"
         summary_message += f"\nCall SL: {call_stop_loss_price}, Put SL: {put_stop_loss_price}"
         notifier(summary_message, self.webhook_url)
 
         if place_sl_orders:
             call_stop_loss_order_ids = place_option_order_and_notify(
-                option=strangle.call_option,
+                instrument=strangle.call_option,
                 action="BUY",
                 qty_in_lots=quantity_in_lots,
-                price=call_stop_loss_price,
+                prices=call_stop_loss_price,
                 order_tag="Call SL Strangle",
                 webhook_url=self.webhook_url,
                 stop_loss_order=True,
                 target_status="trigger pending",
                 return_avg_price=False
             )
             put_stop_loss_order_ids = place_option_order_and_notify(
-                option=strangle.put_option,
+                instrument=strangle.put_option,
                 action="BUY",
                 qty_in_lots=quantity_in_lots,
-                price=put_stop_loss_price,
+                prices=put_stop_loss_price,
                 order_tag="Put SL Strangle",
                 webhook_url=self.webhook_url,
                 stop_loss_order=True,
                 target_status="trigger pending",
                 return_avg_price=False
             )
         else:
             call_stop_loss_order_ids = None
             put_stop_loss_order_ids = None
 
         # Setting up shared info dict
         shared_info_dict = {
             "traded_strangle": strangle,
+            "spot_at_entry": underlying_ltp,
             "call_avg_price": call_avg_price,
             "put_avg_price": put_avg_price,
+            "total_avg_price": total_avg_price,
+            "call_iv_at_entry": traded_call_iv,
+            "put_iv_at_entry": traded_put_iv,
+            "avg_iv_at_entry": traded_avg_iv,
             "call_stop_loss_price": call_stop_loss_price,
             "put_stop_loss_price": put_stop_loss_price,
             "call_stop_loss_order_ids": call_stop_loss_order_ids,
             "put_stop_loss_order_ids": put_stop_loss_order_ids,
+            "time_left_day_start": time_left_at_trade,
             "call_ltp": call_ltp,
             "put_ltp": put_ltp,
             "underlying_ltp": underlying_ltp,
+            "call_iv": traded_call_iv,
+            "put_iv": traded_put_iv,
+            "avg_iv": traded_avg_iv,
             "call_sl": False,
             "put_sl": False,
-            "exit_triggers": {"trade_complete": False}
+            "exit_triggers": {"convert_to_butterfly": False},
+            "trade_complete": False,
+            "call_sl_check_notification_sent": False,
+            "put_sl_check_notification_sent": False,
         }
 
         position_monitor_thread = Thread(target=position_monitor, args=(shared_info_dict,))
         position_monitor_thread.start()
         sleep(3)  # To ensure that the position monitor thread has started
 
+        refresh_book = True
+
         # Wait for exit time or both stop losses to hit (Main Loop)
         while all([currenttime().time() < time(*exit_time)]):
-            check_for_stop_loss(shared_info_dict, 'call')
+            check_for_stop_loss(shared_info_dict, 'call', refresh_orderbook=refresh_book)
             if shared_info_dict["call_sl"]:
                 process_stop_loss(shared_info_dict, "call")
                 break
             check_for_stop_loss(shared_info_dict, 'put')
             if shared_info_dict["put_sl"]:
                 process_stop_loss(shared_info_dict, "put")
                 break
+            refresh_book = False
             sleep(1)
 
         # Out of the while loop, so exit time reached or both stop losses hit
 
+        # If we are hedged then wait till exit time
+        # noinspection PyTypeChecker
+        if shared_info_dict["exit_triggers"]["convert_to_butterfly"]:
+            hedge_strangle = shared_info_dict["ctb_hedge"]
+            place_option_order_and_notify(
+                hedge_strangle, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url, return_avg_price=False
+            )
+            if shared_info_dict["call_stop_loss_order_ids"] and shared_info_dict["put_stop_loss_order_ids"]:
+                cancel_pending_orders(
+                    shared_info_dict["call_stop_loss_order_ids"] + shared_info_dict["put_stop_loss_order_ids"]
+                )
+            notifier(f"{self.name}: Converted to butterfly", self.webhook_url)
+            while currenttime().time() < time(*exit_time):
+                sleep(3)
+
         call_sl = shared_info_dict["call_sl"]
         put_sl = shared_info_dict["put_sl"]
 
         if not call_sl and not put_sl:
-            call_order_ids, put_order_ids = strangle.place_order("BUY", quantity_in_lots, "LIMIT", order_tag)
-            order_book = fetch_book('orderbook')
-            order_statuses_ = lookup_and_return(order_book, 'orderid', call_order_ids + put_order_ids, 'status')
-            check_and_notify_order_statuses(
-                order_statuses_,
-                self.webhook_url,
-                target_status="complete",
-                order_tag='Strangle Exit',
-                Underlying=self.name,
-                Action='BUY',
-                Strikes=[strangle.call_option.strike, strangle.put_option.strike],
-                Expiry=strangle.call_option.expiry,
-                Qty=quantity_in_lots,
-            )
-
-            shared_info_dict['call_exit_price'] = lookup_and_return(
-                order_book, 'orderid', call_order_ids, 'averageprice'
-            ).astype(float).mean()
-            shared_info_dict['put_exit_price'] = lookup_and_return(
-                order_book, 'orderid', put_order_ids, 'averageprice'
-            ).astype(float).mean()
+            # Both stop losses not hit
+            if shared_info_dict["time_left_day_start"] * 365 < 1:  # expiry day
+                call_exit_avg_price, put_exit_avg_price = shared_info_dict["call_ltp"], shared_info_dict["put_ltp"]
+            else:
+                call_exit_avg_price, put_exit_avg_price = place_option_order_and_notify(
+                    strangle, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url, return_avg_price=True
+                )
+            shared_info_dict['call_exit_price'] = call_exit_avg_price
+            shared_info_dict['put_exit_price'] = put_exit_avg_price
 
         elif (call_sl or put_sl) and not (call_sl and put_sl):  # Only one stop loss hit
-            exit_option = strangle.put_option if call_sl else strangle.call_option
-            non_sl_exit_price = place_option_order_and_notify(
-                exit_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
-            )
             exit_option = "put" if call_sl else "call"
+            if shared_info_dict["time_left_day_start"] * 365 < 1:  # expiry day
+                non_sl_exit_price = shared_info_dict[f"{exit_option}_ltp"]
+            else:
+                exit_option = strangle.put_option if call_sl else strangle.call_option
+                non_sl_exit_price = place_option_order_and_notify(
+                    exit_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
+                )
             shared_info_dict[f"{exit_option}_exit_price"] = non_sl_exit_price
 
         else:  # Both stop losses hit
             pass
 
         # Calculate profit
         total_exit_price = shared_info_dict["call_exit_price"] + shared_info_dict["put_exit_price"]
@@ -3020,18 +3094,118 @@
             self.order_log[order_tag][0].update(exit_dict)
         except Exception as e:
             notifier(
                 f"{self.name}: Error updating order list with exit details. {e}",
                 self.webhook_url,
             )
         notifier(exit_message, self.webhook_url)
-        shared_info_dict["exit_triggers"] = {"trade_complete": True}
+        shared_info_dict["trade_complete"] = True
         position_monitor_thread.join()
         return shared_info_dict
 
+    @log_errors
+    def intraday_trend(
+            self,
+            quantity_in_lots,
+            start_time=(9, 15, 58),
+            exit_time=(15, 27),
+            sleep_time=5,
+            threshold_movement=None,
+            minutes_to_avg=45,
+            beta=0.8,
+            max_entries=3
+    ):
+
+        while currenttime().time() < time(*start_time):
+            print(f"{self.name} trender sleeping till {start_time}")
+            sleep(1)
+
+        open_price = self.fetch_ltp()
+        threshold_movement = threshold_movement or (get_current_vix() * (beta or 1)) / 48
+
+        exit_time = time(*exit_time)
+        scan_end_time = (datetime.combine(currenttime().date(), exit_time) - timedelta(minutes=10)).time()
+        price_boundaries = [open_price * (1 + ((-1) ** i) * threshold_movement / 100) for i in range(2)]
+
+        # Price deque
+        n_prices = max(int(minutes_to_avg / sleep_time), 1)
+        price_deque = deque(maxlen=n_prices)
+
+        notifier(
+            f"{self.name} trender starting with {threshold_movement:0.2f} threshold movement\n"
+            f"Current Price: {open_price}\nUpper limit: {price_boundaries[1]:0.2f}\n"
+            f"Lower limit: {price_boundaries[0]:0.2f}.",
+            self.webhook_url,
+        )
+
+        entries = 0
+        last_print_time = currenttime()
+        movement = 0
+        while entries < max_entries and currenttime().time() < exit_time:
+
+            # Scan for entry condition
+            while (abs(movement) < threshold_movement) and (currenttime().time() < scan_end_time):
+
+                ltp = self.fetch_ltp()
+                price_deque.append(ltp)
+                avg_price = (sum(price_deque) / len(price_deque)) if price_deque else ltp
+                movement = (avg_price - open_price) / open_price * 100
+
+                if currenttime() > last_print_time + timedelta(minutes=1):
+                    print(f"{self.name} trender: {movement:0.2f} movement.")
+                    last_print_time = currenttime()
+                sleep(sleep_time)
+
+            if currenttime().time() > scan_end_time:
+                notifier(f"{self.name} trender {entries+1} exiting due to time.", self.webhook_url)
+                return
+
+            # Entry condition met taking position
+            price = self.fetch_ltp()
+            atm_strike = findstrike(price, self.base)
+            position = "BUY" if movement > 0 else "SELL"
+            atm_synthetic_fut = SyntheticFuture(atm_strike, self.name, self.current_expiry)
+            stop_loss_price = price * (0.997 if position == "BUY" else 1.003)
+            stop_loss_hit = False
+            notifier(
+                f"{self.name} {position} trender triggered with {movement:0.2f} movement. {self.name} at {price}. "
+                f"Stop loss at {stop_loss_price}.",
+                self.webhook_url,
+            )
+            place_option_order_and_notify(
+                atm_synthetic_fut, position, quantity_in_lots, "LIMIT", f"{self.name} trender", self.webhook_url
+            )
+
+            # Tracking position
+            while currenttime().time() < exit_time and not stop_loss_hit:
+
+                ltp = self.fetch_ltp()
+                price_deque.append(ltp)
+                avg_price = sum(price_deque) / len(price_deque) if price_deque else ltp
+                movement = (avg_price - open_price) / open_price * 100
+
+                stop_loss_hit = (avg_price < stop_loss_price) if position == "BUY" else (avg_price > stop_loss_price)
+                sleep(sleep_time)
+
+            # Exit condition met exiting position (stop loss or time)
+            stop_loss_message = f"Trender stop loss hit. " if stop_loss_hit else ""
+            notifier(
+                f"{stop_loss_message}{self.name} trender {entries+1} exiting. {self.name} at {self.fetch_ltp()}.",
+                self.webhook_url,
+            )
+            place_option_order_and_notify(
+                atm_synthetic_fut,
+                "BUY" if position == "SELL" else "SELL",
+                quantity_in_lots,
+                "LIMIT",
+                f"{self.name} trender",
+                self.webhook_url,
+            )
+            entries += 1
+
     def intraday_straddle_delta_hedged(
         self,
         quantity_in_lots,
         exit_time=(15, 30),
         websocket=None,
         wait_for_equality=False,
         delta_threshold=1,
@@ -3125,15 +3299,15 @@
                         self.webhook_url,
                     )
                     place_synthetic_fut_order(
                         self.name,
                         equal_strike,
                         expiry,
                         "SELL",
-                        lots_to_sell * self.lot_size,
+                        lots_to_sell,
                     )
                     positions[synthetic_fut_call]["delta_quantity"] -= (
                         lots_to_sell * self.lot_size
                     )
                     positions[synthetic_fut_put]["delta_quantity"] += (
                         lots_to_sell * self.lot_size
                     )
@@ -3146,15 +3320,15 @@
                         self.webhook_url,
                     )
                     place_synthetic_fut_order(
                         self.name,
                         equal_strike,
                         expiry,
                         "BUY",
-                        lots_to_buy * self.lot_size,
+                        lots_to_buy,
                     )
                     positions[synthetic_fut_call]["delta_quantity"] += (
                         lots_to_buy * self.lot_size
                     )
                     positions[synthetic_fut_put]["delta_quantity"] -= (
                         lots_to_buy * self.lot_size
                     )
@@ -3174,22 +3348,23 @@
         # Squaring off the delta positions
         call_delta_quantity = positions[synthetic_fut_call]["delta_quantity"]
         put_delta_quantity = positions[synthetic_fut_put]["delta_quantity"]
 
         if call_delta_quantity != 0 and put_delta_quantity != 0:
             assert call_delta_quantity == -1 * put_delta_quantity
             quantity_to_square_up = abs(call_delta_quantity)
+            quantity_to_square_up_in_lots = quantity_to_square_up / self.lot_size
 
             if call_delta_quantity > 0:
                 action = "SELL"
             else:
                 action = "BUY"
 
-            self.place_synthetic_fut_order(
-                equal_strike, expiry, action, quantity_to_square_up
+            self.place_synthetic_fut(
+                equal_strike, expiry, action, quantity_to_square_up_in_lots
             )
             notifier(
                 f"Intraday Straddle with delta: Squared off delta positions. "
                 + f"{action} {quantity_to_square_up} synthetic futures.",
                 self.webhook_url,
             )
         elif call_delta_quantity == 0 and put_delta_quantity == 0:
@@ -3301,14 +3476,15 @@
         error_handler = logging.FileHandler(error_log_filename)
         error_handler.setLevel(logging.ERROR)
         error_handler.setFormatter(formatter)
         logger.addHandler(error_handler)
 
         logger.info("Logged in successfully.")
 
+        set_error_notification_settings("user", f"{obj.userId} - ")
         notifier(
             f'Date: {currenttime().strftime("%d %b %Y %H:%M:%S")}\nLogged in successfully.',
             webhook_url,
         )
 
 
 def parse_symbol(symbol):
@@ -3371,16 +3547,16 @@
 
         if len(bucket) == 0:
             return 0
         else:
             return np.array(bucket)
 
     if not (
-        isinstance(field_to_lookup, (str, list))
-        and isinstance(value_to_lookup, (str, list))
+        isinstance(field_to_lookup, (str, list, tuple, np.ndarray))
+        and isinstance(value_to_lookup, (str, list, tuple, np.ndarray))
     ):
         raise ValueError(
             "Both 'field_to_lookup' and 'value_to_lookup' must be strings or lists."
         )
 
     if isinstance(field_to_lookup, list) and isinstance(value_to_lookup, str):
         raise ValueError(
@@ -3394,30 +3570,32 @@
         return filter_and_return(book_data)
     else:
         raise ValueError("Invalid input")
 
 
 # Discord messenger
 def notifier(message, webhook_url=None):
-    if webhook_url is None:
+    if webhook_url is None or webhook_url is False:
         print(message)
         return
     else:
         notification_url = webhook_url
         data = {"content": message}
-        requests.post(
-            notification_url,
-            data=json.dumps(data),
-            headers={"Content-Type": "application/json"},
-        )
-        print(message)
-    return
+        try:
+            requests.post(
+                notification_url,
+                data=json.dumps(data),
+                headers={"Content-Type": "application/json"},
+            )
+            print(message)
+        except requests.exceptions.SSLError as e:
+            print(f"Error in sending notification: {e}")
 
 
-def check_and_notify_order_statuses(statuses, webhook_url=None, target_status="complete", **kwargs):
+def check_and_notify_order_placement_statuses(statuses, target_status="complete", webhook_url=None, **kwargs):
 
     order_prefix = f"{kwargs['order_tag']}: " if "order_tag" in kwargs else ""
     order_message = [f"{k}-{v}" for k, v in kwargs.items() if k != "order_tag"]
     order_message = ", ".join(order_message)
 
     if all(statuses == target_status):
         notifier(
@@ -3445,57 +3623,176 @@
             f"{order_prefix}ERROR. Order statuses uncertain for {order_message}",
             webhook_url
         )
         raise Exception("Order statuses uncertain")
 
 
 def place_option_order_and_notify(
-        option: Option,
-        action: str,
-        qty_in_lots,
-        price="LIMIT",
-        order_tag="",
-        webhook_url=None,
-        stop_loss_order=False,
-        target_status="complete",
-        return_avg_price=True
+    instrument: Option | Strangle | Straddle | SyntheticFuture,
+    action: str,
+    qty_in_lots: int,
+    prices: str | int | float | tuple | list | np.ndarray = "LIMIT",
+    order_tag: str = "",
+    webhook_url=None,
+    stop_loss_order: bool = False,
+    target_status: str = "complete",
+    return_avg_price: bool = True,
+    **kwargs
 ):
 
+    notify_dict = {
+        "order_tag": order_tag,
+        "Underlying": instrument.underlying,
+        "Action": action,
+        "Expiry": instrument.expiry,
+        "Qty": qty_in_lots
+    }
+
+    order_params = {
+        "transaction_type": action,
+        "quantity_in_lots": qty_in_lots,
+        "stop_loss_order": stop_loss_order,
+        "order_tag": order_tag
+    }
+
+    if isinstance(instrument, (Strangle, Straddle, SyntheticFuture)):
+        notify_dict.update({
+            "Strikes": [instrument.call_strike, instrument.put_strike]})
+        order_params.update({
+            "prices": prices
+        })
+    elif isinstance(instrument, Option):
+        notify_dict.update({
+            "Strike": instrument.strike,
+            "OptionType": instrument.option_type
+        })
+        order_params.update({
+            "price": prices
+        })
+    else:
+        raise ValueError("Invalid instrument type")
+
+    notify_dict.update(kwargs)
+
     if stop_loss_order:
-        assert isinstance(price, (int, float)), "Stop loss order requires a price"
+        assert isinstance(prices, (int, float, tuple, list, np.ndarray)), "Stop loss order requires a price"
+        target_status = "trigger pending"
+
+    # Placing the order
+    order_ids = instrument.place_order(**order_params)
+
+    if isinstance(order_ids, tuple):  # Strangle/Straddle/SyntheticFuture
+        call_order_ids, put_order_ids = order_ids[0], order_ids[1]
+        order_ids = list(itertools.chain(call_order_ids, put_order_ids))
+    else:  # Option
+        call_order_ids, put_order_ids = False, False
 
-    order_ids = option.place_order(
-        transaction_type=action,
-        quantity_in_lots=qty_in_lots,
-        price=price,
-        stop_loss_order=stop_loss_order,
-        order_tag=order_tag
-    )
     order_book = fetch_book('orderbook')
     order_statuses_ = lookup_and_return(order_book, 'orderid', order_ids, 'status')
-    check_and_notify_order_statuses(
-        order_statuses_,
-        webhook_url,
-        target_status=target_status,
-        order_tag=order_tag,
-        Underlying=option.underlying,
-        Action=action,
-        Strike=option.strike,
-        OptionType=option.option_type,
-        Expiry=option.expiry,
-        Qty=qty_in_lots
+    check_and_notify_order_placement_statuses(
+        statuses=order_statuses_, target_status=target_status, webhook_url=webhook_url, **notify_dict
     )
 
     if return_avg_price:
-        avg_price = lookup_and_return(order_book, 'orderid', order_ids, 'averageprice').astype(float).mean()
-        return avg_price
+        if call_order_ids and put_order_ids:
+            call_avg_price = lookup_and_return(
+                order_book, 'orderid', call_order_ids, 'averageprice'
+            ).astype(float).mean()
+            put_avg_price = lookup_and_return(
+                order_book, 'orderid', put_order_ids, 'averageprice'
+            ).astype(float).mean()
+            return call_avg_price, put_avg_price
+        else:
+            avg_price = lookup_and_return(order_book, 'orderid', order_ids, 'averageprice').astype(float).mean()
+            return avg_price
 
     return order_ids
 
 
+def process_stop_loss_order_statuses(
+        order_book, order_ids, context="", notify_url=None,
+):
+    pending_text = "trigger pending"
+    context = f"{context} " if context else ""
+
+    statuses = lookup_and_return(order_book, "orderid", order_ids, "status")
+
+    if isinstance(statuses, (int, np.int32, np.int64)):
+        logger.error(f"Statuses is {statuses} for orderid(s) {order_ids}")
+
+    if all(statuses == pending_text):
+        return False, False
+
+    elif all(statuses == "rejected") or all(statuses == "cancelled"):
+        rejection_reasons = lookup_and_return(
+            order_book, "orderid", order_ids, "text"
+        )
+        if all(
+                rejection_reasons == "17070 : The Price is out of the LPP range"
+        ):
+            return True, False
+        else:
+            notifier(
+                f"{context}Order rejected or cancelled. Reasons: {rejection_reasons[0]}",
+                notify_url,
+            )
+            raise Exception(f"Orders rejected or cancelled.")
+
+    elif all(statuses == "pending"):
+        sleep(5)
+        order_book = fetch_book("orderbook")
+        statuses = lookup_and_return(order_book, "orderid", order_ids, "status")
+
+        if all(statuses == "pending"):
+            try:
+                cancel_pending_orders(order_ids, "NORMAL")
+            except Exception as e:
+                try:
+                    cancel_pending_orders(order_ids, "STOPLOSS")
+                except Exception as e:
+                    notifier(
+                        f"{context}Could not cancel orders: {e}", notify_url
+                    )
+                    raise Exception(f"Could not cancel orders: {e}")
+            notifier(
+                f"{context}Orders pending and cancelled. Please check.",
+                notify_url,
+            )
+            return True, False
+
+        elif all(statuses == "complete"):
+            return True, True
+
+        else:
+            raise Exception(f"Orders in unknown state.")
+
+    elif all(statuses == "complete"):
+        return True, True
+
+    else:
+        notifier(
+            f"{context}Orders in unknown state. Statuses: {statuses}",
+            notify_url,
+        )
+        raise Exception(f"Orders in unknown state.")
+
+
+def fetch_orderbook_if_needed(
+    data_class=None, refresh_needed: bool = False
+):
+    if data_class is None or refresh_needed:
+        return fetch_book("orderbook")
+    if (
+        currenttime() - data_class.updated_time < timedelta(seconds=15)
+        and data_class.orderbook_data is not None
+    ):
+        return data_class.orderbook_data
+    return fetch_book("orderbook")
+
+
 # Market Hours
 def markethours():
     if time(9, 15) <= currenttime().time() <= time(15, 30):
         return True
     else:
         return False
 
@@ -3667,37 +3964,46 @@
         symbol_token_pairs = [
             (token_df.loc[token_df["token"] == token, "symbol"].values[0], token)
             for token in tokens
         ]
         return symbol_token_pairs
 
     if expiry is None and strike is None and option_type is None:  # Cash segment
-        if name in ["BANKNIFTY", "NIFTY", "NIFTY FIN SERVICE"]:  # Index scrips
-            symbol, token = scrips.loc[
-                (scrips.name == name) & (scrips.exch_seg == "NSE"), ["symbol", "token"]
-            ].values[0]
-        elif name == "FINNIFTY":  # Specific additional case for finnifty since cash segment price is not available
+
+        if name in ["NIFTY", "BANKNIFTY"]:  # Index scrips
+            filtered_scrips = scrips.loc[
+                (scrips.name == name) & (scrips.exch_seg == "NSE") & (scrips.instrumenttype != "AMXIDX")
+            ]   # Temp fix for AMXIDX
+            # print(f'Length of filtered scrips: {len(filtered_scrips)}')
+            assert len(filtered_scrips) == 1, "More than one index scrip found for name."
+            symbol, token = filtered_scrips[["symbol", "token"]].values[0]
+
+        elif name in ["FINNIFTY", "MIDCPNIFTY"]:  # Finnifty & Midcpnifty temp fix
             futures = scrips.loc[
                 (scrips.name == name) & (scrips.instrumenttype == "FUTIDX"),
                 ["expiry", "symbol", "token"],
             ]
             futures["expiry"] = pd.to_datetime(futures["expiry"], format="%d%b%Y")
             futures = futures.sort_values(by="expiry")
             symbol, token = futures.iloc[0][["symbol", "token"]].values
+
         else:  # For all other equity scrips
-            symbol, token = scrips.loc[
+            filtered_scrips = scrips.loc[
                 (scrips.name == name)
                 & (scrips.exch_seg == "NSE")
-                & (scrips.symbol.str.endswith("EQ")),
-                ["symbol", "token"],
-            ].values[0]
+                & (scrips.symbol.str.endswith("EQ"))
+            ]
+            assert len(filtered_scrips) == 1, "More than one equity scrip found for name."
+            symbol, token = filtered_scrips[["symbol", "token"]].values[0]
+
     elif expiry is not None and strike is not None and option_type is not None:  # Options segment
         strike = str(int(strike))  # Handle float strikes, convert to integer first
         symbol = name + expiry + strike + option_type
         token = scrips[scrips.symbol == symbol]["token"].tolist()[0]
+
     else:
         raise ValueError("Invalid arguments")
 
     return symbol, token
 
 
 def get_straddle_symbol_tokens(name, strike, expiry):
@@ -3907,15 +4213,15 @@
         num = base
     return round(num, 2)
 
 
 def splice_orders(quantity_in_lots, freeze_qty):
     if quantity_in_lots > freeze_qty:
         loops = int(quantity_in_lots / freeze_qty)
-        if loops > large_order_threshold:
+        if loops > LARGE_ORDER_THRESHOLD:
             raise Exception(
                 "Order too big. This error was raised to prevent accidental large order placement."
             )
 
         remainder = quantity_in_lots % freeze_qty
         if remainder == 0:
             spliced_orders = [freeze_qty] * loops
@@ -3929,15 +4235,43 @@
 def check_for_weekend(expiry):
     expiry = datetime.strptime(expiry, "%d%b%y")
     expiry = expiry + pd.DateOffset(minutes=930)
     date_range = pd.date_range(currenttime().date(), expiry - timedelta(days=1))
     return date_range.weekday.isin([5, 6]).any()
 
 
-def indices_to_trade(nifty, bnf, finnifty, multi_before_weekend=False):
+def get_strangle_indices_to_trade(*indices, pre_weekend_indices=None):
+
+    if pre_weekend_indices is None:
+        pre_weekend_indices = ["NIFTY", "BANKNIFTY"]
+
+    times_to_expiries = [timetoexpiry(index.current_expiry, effective_time=True, in_days=True) for index in indices]
+
+    # Check if any index has less than 1 day to expiry
+    indices_less_than_1_day = [index for index, time_to_expiry in zip(indices, times_to_expiries) if time_to_expiry < 1]
+
+    if indices_less_than_1_day:
+        return indices_less_than_1_day
+
+    # If no index has less than 1 day to expiry
+    min_expiry_time = min(times_to_expiries)
+    indices_with_closest_expiries = [
+        index for index, time_to_expiry in zip(indices, times_to_expiries)
+        if time_to_expiry == min_expiry_time
+    ]
+    closest_index_names = [index.name for index in indices_with_closest_expiries]
+    weekend_in_range = check_for_weekend(indices_with_closest_expiries[0].current_expiry)
+
+    if (("FINNIFTY" in closest_index_names) and weekend_in_range) or ("MIDCPNIFTY" in closest_index_names):
+        return [index for index in indices if index.name in pre_weekend_indices]
+
+    return indices_with_closest_expiries
+
+
+def indices_to_trade(nifty, bnf, finnifty, multi_before_weekend=False):  # delete this
     fin_exp_closer = timetoexpiry(
         finnifty.current_expiry, effective_time=True, in_days=True
     ) < timetoexpiry(nifty.current_expiry, effective_time=True, in_days=True)
     weekend_in_range = check_for_weekend(finnifty.current_expiry)
     if fin_exp_closer:
         if weekend_in_range and multi_before_weekend:
             return [nifty, finnifty]
@@ -3961,15 +4295,15 @@
     # Subtracting holidays and weekends
     if effective_time:
         date_range = pd.date_range(currenttime().date(), expiry - timedelta(days=1))
         numer_of_weekdays = sum(date_range.dayofweek > 4)
         number_of_holidays = sum(date_range.isin(holidays))
         time_to_expiry -= (numer_of_weekdays + number_of_holidays) / 365
         # print(f'Number of weekdays: {numer_of_weekdays} and number of holidays: {number_of_holidays}')
-    return time_to_expiry * multiplier
+    return round(time_to_expiry, 3) * multiplier
 
 
 def calculate_iv(opt_price, spot, strike, tte, opt_type):
     try:
         return bs.implied_volatility(opt_price, spot, strike, tte, 0.06, opt_type)
     except ValueError:
         return None
@@ -4039,24 +4373,71 @@
     )
     delta = bs.delta(underlying_price, strike, time_left, 0.05, iv, option_type)
     gamma = bs.gamma(underlying_price, strike, time_left, 0.05, iv)
 
     return iv, delta, gamma
 
 
+@time_the_function
+def most_equal_strangle(*strangles, disparity_threshold=np.inf, exit_time=time(15, 25)):
+
+    # Create a set of all distinct options
+    options = set(option for strangle in strangles for option in (strangle.call_option, strangle.put_option))
+
+    # Define the price disparity function
+    def price_disparity(strangle):
+        call_ltp = ltp_cache[strangle.call_option]
+        put_ltp = ltp_cache[strangle.put_option]
+        return abs(call_ltp - put_ltp) / min(call_ltp, put_ltp)
+
+    tracked_strangle = None
+
+    while currenttime().time() < exit_time:
+
+        # If there's no tracked strangle update all prices and find the most equal strangle
+        if tracked_strangle is None:
+            ltp_cache = {option: option.fetch_ltp() for option in options}
+            most_equal, min_disparity = min(((s, price_disparity(s)) for s in strangles), key=lambda x: x[1])
+            if min_disparity < 0.10:
+                tracked_strangle = most_equal
+
+        # If there's a tracked strangle, check its disparity
+        else:
+            ltp_cache = {
+                tracked_strangle.call_option: tracked_strangle.call_option.fetch_ltp(),
+                tracked_strangle.put_option: tracked_strangle.put_option.fetch_ltp()
+            }
+            most_equal = tracked_strangle
+            min_disparity = price_disparity(tracked_strangle)
+            if min_disparity >= 0.10:
+                tracked_strangle = None
+
+        logger.info(f"Most equal strangle: {most_equal} with disparity {min_disparity} "
+                    f"and prices {ltp_cache[most_equal.call_option]} and {ltp_cache[most_equal.put_option]}")
+        logger.info(f"Most equal ltp cache: {ltp_cache}")
+        # If the lowest disparity is below the threshold, return the most equal strangle
+        if min_disparity < disparity_threshold:
+            return most_equal
+        else:
+            pass
+
+    else:
+        return None
+
+
 def get_current_vix():
     vix = yf.Ticker("^INDIAVIX")
     vix = vix.fast_info["last_price"]
     return vix
 
 
 def get_index_constituents(index_symbol, cutoff_pct=101):
     # Fetch and filter constituents
     constituents = (
-        pd.read_csv(f"autotrader/info/{index_symbol}_constituents.csv")
+        pd.read_csv(f"data/{index_symbol}_constituents.csv")
         .sort_values("Index weight", ascending=False)
         .assign(cum_weight=lambda df: df["Index weight"].cumsum())
         .loc[lambda df: df.cum_weight < cutoff_pct]
     )
 
     constituent_tickers, constituent_weights = (
         constituents.Ticker.to_list(),
@@ -4174,15 +4555,15 @@
             "ordertype": "STOPLOSS_LIMIT",
             "triggerprice": round(price, 1),
             "price": round(execution_price, 1),
         })
     else:
         order_type, execution_price = ("MARKET", 0) if price == "MARKET" else ("LIMIT", price)
         if order_type == "LIMIT":
-            if execution_price < 10 and qty < 4000:
+            if execution_price < 10 and qty < 6000:
                 execution_price = np.ceil(price) if action == "BUY" else max(np.floor(price), 0.05)
 
         params.update({
             "variety": "NORMAL",
             "ordertype": order_type,
             "price": custom_round(execution_price)
         })
@@ -4198,38 +4579,26 @@
 
 
 def place_synthetic_fut_order(
     name,
     strike,
     expiry,
     buy_or_sell,
-    quantity_in_shares,
+    quantity_in_lots,
     prices: str | tuple = "MARKET",
+    stop_loss_order=False,
+    order_tag="",
 ):
     """Places a synthetic future order. Quantity is in number of shares."""
 
-    strike = int(strike)
-    call_symbol, call_token = fetch_symbol_token(name, expiry, strike, "CE")
-    put_symbol, put_token = fetch_symbol_token(name, expiry, strike, "PE")
-
-    if prices == "MARKET":
-        call_price = "MARKET"
-        put_price = "MARKET"
-    else:
-        call_price, put_price = prices
-
-    call_action = "BUY" if buy_or_sell == "BUY" else "SELL"
-    put_action = "SELL" if buy_or_sell == "BUY" else "BUY"
-    order_id_call = place_order(
-        call_symbol, call_token, quantity_in_shares, call_action, call_price
-    )
-    order_id_put = place_order(
-        put_symbol, put_token, quantity_in_shares, put_action, put_price
+    syn_fut = SyntheticFuture(strike, name, expiry)
+    call_order_ids, put_order_ids = syn_fut.place_order(
+        buy_or_sell, quantity_in_lots, prices, stop_loss_order, order_tag
     )
-    return order_id_call, order_id_put
+    return call_order_ids, put_order_ids
 
 
 def cancel_pending_orders(order_ids, variety="STOPLOSS"):
     if isinstance(order_ids, (list, np.ndarray)):
         for order_id in order_ids:
             obj.cancelOrder(order_id, variety)
     else:
```

### Comparing `volstreet-0.9.9/volstreet/discord_bot.py` & `volstreet-1.0.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.9/volstreet/nsefunctions.py` & `volstreet-1.0.0/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.9/volstreet/strategies.py` & `volstreet-1.0.0/volstreet/strategies.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,32 +37,35 @@
     user=None,
     pin=None,
     apikey=None,
     authkey=None,
     webhook_url=None,
     shared_data=True,
     start_time=(9, 16),
-    multi_before_weekend=True,
+    special_parameters=None
 ):
 
     """
     :param parameters: parameters for the strategy (refer to the strategy's docstring)
     :param strategy: 'straddle' or 'strangle' will invoke intraday_straddle or intraday_strangle of the index
     :param client:
     :param user:
     :param pin:
     :param apikey:
     :param authkey:
     :param webhook_url:
     :param shared_data:
     :param start_time:
-    :param multi_before_weekend:
+    :param special_parameters: special parameters for a particular index
     :return:
     """
 
+    if special_parameters is None:
+        special_parameters = {}
+
     user, pin, apikey, authkey, discord_webhook_url = get_user_data(
         client, user, pin, apikey, authkey, webhook_url
     )
 
     # If today is a holiday, the script will exit
     if vs.currenttime().date() in vs.holidays:
         vs.notifier("Today is a holiday. Exiting.", discord_webhook_url)
@@ -74,41 +77,43 @@
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
     nifty = vs.Index("NIFTY", webhook_url=discord_webhook_url)
     bnf = vs.Index("BANKNIFTY", webhook_url=discord_webhook_url)
     fin = vs.Index("FINNIFTY", webhook_url=discord_webhook_url)
+    midcap = vs.Index("MIDCPNIFTY", webhook_url=discord_webhook_url)
+
+    indices = vs.get_strangle_indices_to_trade(nifty, bnf, fin, midcap)
 
-    indices = vs.indices_to_trade(
-        nifty, bnf, fin, multi_before_weekend=multi_before_weekend
-    )
-    quantity_multiplier = 2 if len(indices) == 1 else 1
     parameters["quantity_in_lots"] = (
-        parameters["quantity_in_lots"] * quantity_multiplier
+        parameters["quantity_in_lots"] // len(indices)
     )
 
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
+        index_parameters = parameters.copy()
+        index_parameters.update(special_parameters.get(index.name, {}))
+        vs.logger.info(f"Trading {index.name} {strategy} with parameters {index_parameters}")
         vs.notifier(f"Trading {index.name} {strategy}.", discord_webhook_url)
-        thread = threading.Thread(target=getattr(index, f'intraday_{strategy}'), kwargs=parameters)
+        thread = threading.Thread(target=getattr(index, f'intraday_{strategy}'), kwargs=index_parameters)
         options_threads.append(thread)
 
     # Wait for the market to open
     while vs.currenttime().time() < time(*start_time):
-        pass
+        sleep(1)
 
     # Start the data updater thread
     if shared_data and update_data_thread is not None:
         update_data_thread.start()
 
     # Start the options threads
     for thread in options_threads:
@@ -171,116 +176,76 @@
 
     try:
         vs.append_data_to_json(nifty.order_log, f"{user}_NIFTY_ON_straddle_log.json")
     except Exception as e:
         vs.notifier(f"Appending data failed: {e}", discord_webhook_url)
 
 
-@vs.log_errors
-def intraday_trend_on_nifty(
-    quantity_in_lots,
+def intraday_trend_on_indices(
+    parameters,
+    indices,
     client=None,
     user=None,
     pin=None,
     apikey=None,
     authkey=None,
     webhook_url=None,
-    start_time=(9, 15, 55),
-    exit_time=(15, 27),
 ):
+
+    """
+
+    :param parameters: parameters for the strategy (refer to the strategy's docstring)
+                       summary of parameters:
+                       quantity_in_lots,
+                       start_time=(9, 15, 58),
+                       exit_time=(15, 27),
+                       sleep_time=5,
+                       threshold_movement=None,
+                       minutes_to_avg=45,
+                       beta=0.8,
+                       max_entries=3
+    :param indices: list of indices to trade
+    :param client: client's name
+    :param user: username
+    :param pin: user's pin
+    :param apikey: user apikey
+    :param authkey: user authkey
+    :param webhook_url: discord webhook url
+
+    """
+
     user, pin, apikey, authkey, discord_webhook_url = get_user_data(
         client, user, pin, apikey, authkey, webhook_url
     )
 
     if vs.currenttime().date() in vs.holidays:
-        vs.notifier("Today is a holiday. Exiting.")
+        vs.notifier("Today is a holiday hence exiting.", discord_webhook_url)
         exit()
 
     vs.login(
         user=user,
         pin=pin,
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
 
-    nifty = vs.Index("NIFTY", webhook_url=discord_webhook_url)
-
-    while vs.currenttime().time() < time(*start_time):
-        pass
+    threads = []
+    for index_symbol in indices:
+        index = vs.Index(index_symbol, webhook_url=discord_webhook_url)
+        thread = threading.Thread(
+            target=index.intraday_trend, kwargs=parameters
+        )
+        threads.append(thread)
 
-    nifty_open_price = nifty.fetch_ltp()
-    movement = 0
-    vix = vs.get_current_vix()
-    threshold_movement = vix / 48
-    exit_time = time(*exit_time)
-    scan_end_time = vs.datetime.combine(vs.currenttime().date(), exit_time)
-    scan_end_time = scan_end_time - vs.timedelta(minutes=10)
-    scan_end_time = scan_end_time.time()
-    upper_limit = nifty_open_price * (1 + threshold_movement / 100)
-    lower_limit = nifty_open_price * (1 - threshold_movement / 100)
-
-    vs.notifier(
-        f"Nifty trender starting with {threshold_movement:0.2f} threshold movement\n"
-        f"Current Price: {nifty_open_price}\nUpper limit: {upper_limit:0.2f}\n"
-        f"Lower limit: {lower_limit:0.2f}.",
-        discord_webhook_url,
-    )
-    last_printed_time = vs.currenttime()
-    while (
-        abs(movement) < threshold_movement and vs.currenttime().time() < scan_end_time
-    ):
-        movement = ((nifty.fetch_ltp() / nifty_open_price) - 1) * 100
-        if vs.currenttime() > last_printed_time + vs.timedelta(minutes=1):
-            print(f"Nifty trender: {movement:0.2f} movement.")
-            last_printed_time = vs.currenttime()
-        sleep(1)
+    for thread in threads:
+        thread.start()
 
-    if vs.currenttime().time() > scan_end_time:
-        vs.notifier("Nifty trender exiting due to time.", discord_webhook_url)
-        return
-
-    price = nifty.fetch_ltp()
-    atm_strike = vs.findstrike(price, nifty.base)
-    position = "BUY" if movement > 0 else "SELL"
-    nifty.place_synthetic_fut_order(
-        atm_strike,
-        nifty.current_expiry,
-        position,
-        quantity_in_lots,
-        prices="LIMIT",
-        check_status=True,
-    )
-    stop_loss_multiplier = 1.0032 if position == "SELL" else 0.9968
-    stop_loss_price = price * stop_loss_multiplier
-    stop_loss_hit = False
-    vs.notifier(
-        f"Nifty {position} trender triggered with {movement:0.2f} movement. Nifty at {price}. "
-        f"Stop loss at {stop_loss_price}.",
-        discord_webhook_url,
-    )
-    while vs.currenttime().time() < exit_time and not stop_loss_hit:
-        if position == "BUY":
-            stop_loss_hit = nifty.fetch_ltp() < stop_loss_price
-        else:
-            stop_loss_hit = nifty.fetch_ltp() > stop_loss_price
-        sleep(3)
-    nifty.place_synthetic_fut_order(
-        atm_strike,
-        nifty.current_expiry,
-        "SELL" if position == "BUY" else "BUY",
-        quantity_in_lots,
-        prices="LIMIT",
-        check_status=True,
-    )
-    stop_loss_message = "Trender stop loss hit. " if stop_loss_hit else ""
-    vs.notifier(
-        f"{stop_loss_message}Nifty trender exited. Nifty at {nifty.fetch_ltp()}.",
-        discord_webhook_url,
-    )
+    for thread in threads:
+        thread.join()
 
 
 def index_vs_constituents(
     index_symbol,
     strike_offset=0,
     index_strike_offset=None,
     cutoff_pct=90,
```

### Comparing `volstreet-0.9.9/volstreet.egg-info/requires.txt` & `volstreet-1.0.0/volstreet.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 discord.py>=2.2.2
 entrypoints==0.4
 executing==1.2.0
 eod==0.2.1
 fuzzywuzzy==0.18.0
 idna==3.4
 jedi==0.18.2
+kiteconnect==4.2.0
 lxml==4.9.2
 matplotlib-inline==0.1.6
 nest-asyncio==1.5.6
 numpy==1.24.2
 packaging==23.0
 pandas==1.5.3
 parso==0.8.3
@@ -30,17 +31,17 @@
 python-Levenshtein==0.21.0
 pytz==2022.7.1
 pywin32==305
 pyzmq==25.0.0
 requests==2.28.2
 scikit-learn==1.2.2
 scipy==1.10.1
+selenium==4.10.0
 six==1.16.0
 smartapi-python==1.3.0
-spyder-kernels>=2.2.1
 stack-data==0.6.2
 tornado==6.2
 traitlets==5.8.1
 urllib3==1.26.14
 wcwidth==0.2.6
 websocket-client==1.5.1
 xlrd==2.0.1
```

