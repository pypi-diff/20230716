# Comparing `tmp/FinQuant-0.3.0.tar.gz` & `tmp/FinQuant-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinQuant-0.3.0.tar", last modified: Fri Jul 14 13:23:40 2023, max compression
+gzip compressed data, was "FinQuant-0.3.1.tar", last modified: Sun Jul 16 10:15:15 2023, max compression
```

## Comparing `FinQuant-0.3.0.tar` & `FinQuant-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.721071 FinQuant-0.3.0/
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.482070 FinQuant-0.3.0/FinQuant.egg-info/
--rwxrwxrwx   0 frank     (1000) frank     (1000)    14821 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/PKG-INFO
--rwxrwxrwx   0 frank     (1000) frank     (1000)      801 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/SOURCES.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)        1 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/dependency_links.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)      176 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/requires.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)        9 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/top_level.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1059 2023-07-08 06:47:36.000000 FinQuant-0.3.0/LICENSE.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)    14821 2023-07-14 13:23:41.722070 FinQuant-0.3.0/PKG-INFO
--rwxrwxrwx   0 frank     (1000) frank     (1000)    13659 2023-07-14 13:20:17.000000 FinQuant-0.3.0/README.md
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.592070 FinQuant-0.3.0/finquant/
--rwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-08 06:47:36.000000 FinQuant-0.3.0/finquant/__init__.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2764 2023-07-14 10:30:56.000000 FinQuant-0.3.0/finquant/asset.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    16801 2023-07-10 17:36:45.000000 FinQuant-0.3.0/finquant/efficient_frontier.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     3180 2023-07-14 13:11:14.000000 FinQuant-0.3.0/finquant/market.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1993 2023-07-14 09:57:06.000000 FinQuant-0.3.0/finquant/minimise_fun.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    11159 2023-07-08 06:47:36.000000 FinQuant-0.3.0/finquant/monte_carlo.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     6685 2023-07-14 13:11:10.000000 FinQuant-0.3.0/finquant/moving_average.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    47239 2023-07-14 13:11:10.000000 FinQuant-0.3.0/finquant/portfolio.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     3936 2023-07-08 06:47:36.000000 FinQuant-0.3.0/finquant/quants.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2209 2023-07-14 09:57:06.000000 FinQuant-0.3.0/finquant/returns.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     4940 2023-07-14 13:11:14.000000 FinQuant-0.3.0/finquant/stock.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      106 2023-07-14 13:23:41.725073 FinQuant-0.3.0/setup.cfg
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2111 2023-07-12 07:35:01.000000 FinQuant-0.3.0/setup.py
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.711074 FinQuant-0.3.0/tests/
--rwxrwxrwx   0 frank     (1000) frank     (1000)     7949 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Analysis.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     3056 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Build-Portfolio-from-file.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     5368 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Build-Portfolio-from-web.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     6715 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Optimisation.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_efficient_frontier.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1006 2023-07-14 09:57:06.000000 FinQuant-0.3.0/tests/test_market.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     6288 2023-07-08 08:26:58.000000 FinQuant-0.3.0/tests/test_moving_average.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_optimisation.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    15918 2023-07-08 08:26:58.000000 FinQuant-0.3.0/tests/test_portfolio.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1283 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_quants.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2250 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_returns.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1926 2023-07-08 08:26:58.000000 FinQuant-0.3.0/tests/test_stock.py
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.333624 FinQuant-0.3.1/
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.088626 FinQuant-0.3.1/FinQuant.egg-info/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    14840 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/PKG-INFO
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      821 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/SOURCES.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        1 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/dependency_links.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      229 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/requires.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        9 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/top_level.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1059 2023-07-15 13:11:58.000000 FinQuant-0.3.1/LICENSE.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    14840 2023-07-16 10:15:16.334127 FinQuant-0.3.1/PKG-INFO
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    13659 2023-07-15 16:53:23.000000 FinQuant-0.3.1/README.md
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.194124 FinQuant-0.3.1/finquant/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-15 13:12:00.000000 FinQuant-0.3.1/finquant/__init__.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2766 2023-07-16 10:13:37.000000 FinQuant-0.3.1/finquant/asset_test.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    16730 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/efficient_frontier.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     3133 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/market.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1993 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/minimise_fun.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    11041 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/monte_carlo.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     7485 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/moving_average.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    46879 2023-07-16 10:12:50.000000 FinQuant-0.3.1/finquant/portfolio.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     3936 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/quants.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2219 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/returns.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     4840 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/stock.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      301 2023-07-15 16:53:23.000000 FinQuant-0.3.1/pyproject.toml
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      106 2023-07-16 10:15:16.337624 FinQuant-0.3.1/setup.cfg
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2200 2023-07-15 16:53:23.000000 FinQuant-0.3.1/setup.py
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.321626 FinQuant-0.3.1/tests/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     8254 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Analysis.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     3160 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Build-Portfolio-from-file.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     5489 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Build-Portfolio-from-web.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     6919 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Optimisation.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-15 13:12:01.000000 FinQuant-0.3.1/tests/test_efficient_frontier.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1007 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_market.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     6283 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_moving_average.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-15 13:12:01.000000 FinQuant-0.3.1/tests/test_optimisation.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    15920 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_portfolio.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1278 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_quants.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2244 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_returns.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1928 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_stock.py
```

### Comparing `FinQuant-0.3.0/FinQuant.egg-info/PKG-INFO` & `FinQuant-0.3.1/FinQuant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.3.0
+Version: 0.3.1
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.0.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.1.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -20,14 +20,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: cd
 License-File: LICENSE.txt
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.3.0 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.3.1 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.3.0.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.3.1.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: docs License-File:
-LICENSE.txt
+Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
+cd License-File: LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
 [pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
```

### Comparing `FinQuant-0.3.0/FinQuant.egg-info/SOURCES.txt` & `FinQuant-0.3.1/FinQuant.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 LICENSE.txt
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 FinQuant.egg-info/PKG-INFO
 FinQuant.egg-info/SOURCES.txt
 FinQuant.egg-info/dependency_links.txt
 FinQuant.egg-info/requires.txt
 FinQuant.egg-info/top_level.txt
 finquant/__init__.py
-finquant/asset.py
+finquant/asset_test.py
 finquant/efficient_frontier.py
 finquant/market.py
 finquant/minimise_fun.py
 finquant/monte_carlo.py
 finquant/moving_average.py
 finquant/portfolio.py
 finquant/quants.py
```

### Comparing `FinQuant-0.3.0/LICENSE.txt` & `FinQuant-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.0/PKG-INFO` & `FinQuant-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.3.0
+Version: 0.3.1
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.0.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.1.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -20,14 +20,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: cd
 License-File: LICENSE.txt
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.3.0 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.3.1 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.3.0.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.3.1.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: docs License-File:
-LICENSE.txt
+Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
+cd License-File: LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
 [pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
```

### Comparing `FinQuant-0.3.0/README.md` & `FinQuant-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.0/finquant/asset.py` & `FinQuant-0.3.1/finquant/asset_test.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ This module provides a public class ``Asset`` that holds and calculates quantities of a single asset.
 It is designed to be used for stocks and/or market indices.
 """
 
 import numpy as np
 import pandas as pd
+
 from finquant.returns import daily_returns, historical_mean_return
 
 
 class Asset:
     """Object that contains information about an asset.
     To initialise the object, it requires data, e.g. daily closing prices as a
     ``pandas.Series``, a name as string and a type as string.
@@ -29,15 +30,14 @@
         self.expected_return = self.comp_expected_return()
         self.volatility = self.comp_volatility()
         self.skew = self._comp_skew()
         self.kurtosis = self._comp_kurtosis()
         self.daily_returns = self.comp_daily_returns()
         self.asset_type = asset_type
 
-
     # functions to compute quantities
     def comp_daily_returns(self) -> pd.Series:
         """Computes the daily returns (percentage change) of the asset."""
         return daily_returns(self.data)
 
     def comp_expected_return(self, freq=252) -> float:
         """Computes the Expected Return of the asset."""
@@ -64,8 +64,8 @@
         string += "\nSkewness: {:0.5f}".format(self.skew)
         string += "\nKurtosis: {:0.5f}".format(self.kurtosis)
         string += "\n" + "-" * 50
         print(string)
 
     def __str__(self):
         string = "Contains information about {}".format(self.name)
-        return string
+        return string
```

### Comparing `FinQuant-0.3.0/finquant/efficient_frontier.py` & `FinQuant-0.3.1/finquant/efficient_frontier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """The module facilitates a class `EfficientFrontier` that can be used to
 optimise a portfolio by minimising a cost/objective function.
 """
 
 
+import matplotlib.pylab as plt
 import numpy as np
 import pandas as pd
 import scipy.optimize as sco
-import matplotlib.pylab as plt
+
 import finquant.minimise_fun as min_fun
 from finquant.quants import annualised_portfolio_quantities
 
 
-class EfficientFrontier(object):
+class EfficientFrontier:
     """An object designed to perform optimisations based on minimising a cost/objective function.
     It can find parameters for portfolios with
 
     - minimum volatility
     - maximum Sharpe ratio
     - minimum volatility for a given target return
     - maximum Sharpe ratio for a given target volatility
@@ -121,27 +122,31 @@
              of stocks within the optimised portfolio.
          :weights:
            - if "save_weights" is False: a ``numpy.ndarray`` of weights/allocation
              of stocks within the optimised portfolio.
         """
         if not isinstance(save_weights, bool):
             raise ValueError("save_weights is expected to be a boolean.")
+
         args = (self.mean_returns.values, self.cov_matrix.values)
-        # optimisation
+
+        # Optimization
         result = sco.minimize(
             min_fun.portfolio_volatility,
             args=args,
             x0=self.x0,
             method=self.method,
             bounds=self.bounds,
             constraints=self.constraints,
         )
-        # if successful, set self.last_optimisation
+
+        # Set the last optimization
         self.last_optimisation = "Minimum Volatility"
-        # set optimal weights
+
+        # Set optimal weights
         if save_weights:
             self.weights = result["x"]
             self.df_weights = self._dataframe_weights(self.weights)
             return self.df_weights
         else:
             # not setting instance variables, and returning array instead
             # of pandas.DataFrame
@@ -302,15 +307,15 @@
              range of target returns.
 
         :Output:
          :efrontier: ``numpy.ndarray`` of (volatility, return) values
         """
         if targets is not None and not isinstance(targets, (list, np.ndarray)):
             raise ValueError("targets is expected to be a list or numpy.ndarray")
-        elif targets is None:
+        if targets is None:
             # set range of target returns from the individual expected
             # returns of the stocks in the portfolio.
             min_return = self.mean_returns.min() * self.freq
             max_return = self.mean_returns.max() * self.freq
             targets = np.linspace(round(min_return, 3), round(max_return, 3), 100)
         # compute the efficient frontier
         efrontier = []
@@ -344,16 +349,16 @@
         plt.xlabel("Volatility")
         plt.ylabel("Expected Return")
         plt.legend()
 
     def plot_optimal_portfolios(self):
         """Plots markers of the optimised portfolios for
 
-         - minimum Volatility, and
-         - maximum Sharpe Ratio.
+        - minimum Volatility, and
+        - maximum Sharpe Ratio.
         """
         # compute optimal portfolios
         min_vol_weights = self.minimum_volatility(save_weights=False)
         max_sharpe_weights = self.maximum_sharpe_ratio(save_weights=False)
         # compute return and volatility for each portfolio
         min_vol_vals = list(
             annualised_portfolio_quantities(
@@ -415,19 +420,19 @@
             self.mean_returns,
             self.cov_matrix,
             risk_free_rate=self.risk_free_rate,
             freq=self.freq,
         )
         if verbose:
             string = "-" * 70
-            string += "\nOptimised portfolio for {}".format(self.last_optimisation)
-            string += "\n\nTime window/frequency: {}".format(self.freq)
-            string += "\nRisk free rate: {}".format(self.risk_free_rate)
-            string += "\nExpected annual Return: {:.3f}".format(expected_return)
-            string += "\nAnnual Volatility: {:.3f}".format(volatility)
-            string += "\nSharpe Ratio: {:.3f}".format(sharpe)
+            string += f"\nOptimised portfolio for {self.last_optimisation}"
+            string += f"\n\nTime window/frequency: {self.freq}"
+            string += f"\nRisk free rate: {self.risk_free_rate}"
+            string += f"\nExpected annual Return: {expected_return:.3f}"
+            string += f"\nAnnual Volatility: {volatility:.3f}"
+            string += f"\nSharpe Ratio: {sharpe:.3f}"
             string += "\n\nOptimal weights:"
-            string += "\n" + str(self.df_weights.transpose())
+            string += f"\n{str(self.df_weights.transpose())}"
             string += "\n"
             string += "-" * 70
             print(string)
         return (expected_return, volatility, sharpe)
```

### Comparing `FinQuant-0.3.0/finquant/market.py` & `FinQuant-0.3.1/finquant/market.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """This module provides a public class ``Market`` that holds and calculates quantities of a market index"""
 
 import numpy as np
 import pandas as pd
 
-from finquant.returns import historical_mean_return, daily_returns
+from finquant.returns import daily_returns, historical_mean_return
 
 
-class Market(object):
+class Market:
     """Object that contains information about a market index.
     To initialise the object, it requires a name and information about
     the index given as ``pandas.Series`` data structure.
     """
 
     def __init__(self, data: pd.Series) -> None:
         """
@@ -68,19 +68,19 @@
 
     def properties(self):
         """Nicely prints out the properties of the market index:
         Expected Return, Volatility, Skewness, and Kurtosis.
         """
         # nicely printing out information and quantities of market index
         string = "-" * 50
-        string += "\Market index: {}".format(self.name)
-        string += "\nExpected Return:{:0.3f}".format(self.expected_return)
-        string += "\nVolatility: {:0.3f}".format(self.volatility)
-        string += "\nSkewness: {:0.5f}".format(self.skew)
-        string += "\nKurtosis: {:0.5f}".format(self.kurtosis)
+        string += f"\nMarket index: {self.name}"
+        string += f"\nExpected Return:{self.expected_return:0.3f}"
+        string += f"\nVolatility: {self.volatility:0.3f}"
+        string += f"\nSkewness: {self.skew:0.5f}"
+        string += f"\nKurtosis: {self.kurtosis:0.5f}"
         string += "-" * 50
         print(string)
 
     def __str__(self):
         # print short description
         string = "Contains information about market index " + str(self.name) + "."
         return string
```

### Comparing `FinQuant-0.3.0/finquant/minimise_fun.py` & `FinQuant-0.3.1/finquant/minimise_fun.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.0/finquant/monte_carlo.py` & `FinQuant-0.3.1/finquant/monte_carlo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """The module provides a class ``MonteCarlo`` which is an implementation of the
 Monte Carlo method and a class ``MonteCarloOpt`` which allows the user to perform a
 Monte Carlo run to find optimised financial portfolios, given an intial portfolio.
 """
 
 
+import matplotlib.pylab as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pylab as plt
+
 from finquant.quants import annualised_portfolio_quantities
 
 
-class MonteCarlo(object):
+class MonteCarlo:
     """An object to perform a Monte Carlo run/simulation."""
 
     def __init__(self, num_trials=1000):
         """
         :Input:
          :num_trials: ``int`` (default: ``1000``), number of iterations of the
                  Monte Carlo run/simulation.
@@ -27,15 +28,15 @@
          :fun: Function to call at each iteration of the Monte Carlo run.
          :kwargs: (optional) Additional arguments that are passed to `fun`.
 
         :Output:
          :result: List of quantities returned from `fun` at each iteration.
         """
         result = []
-        for i in range(self.num_trials):
+        for _ in range(self.num_trials):
             res = fun(**kwargs)
             result.append(res)
         return np.asarray(result, dtype=object)
 
 
 class MonteCarloOpt(MonteCarlo):
     """An object to perform a Monte Carlo run/simulation for finding
@@ -88,15 +89,15 @@
             raise ValueError("freq is expected to be an integer.")
         self.returns = returns
         self.num_trials = num_trials
         self.risk_free_rate = risk_free_rate
         self.freq = freq
         self.initial_weights = initial_weights
         # initiate super class
-        super(MonteCarloOpt, self).__init__(num_trials=self.num_trials)
+        super().__init__(num_trials=self.num_trials)
         # setting additional variables
         self.num_stocks = len(self.returns.columns)
         self.return_means = self.returns.mean()
         self.cov_matrix = self.returns.cov()
         # setting up variables for results
         self.df_weights = None
         self.df_results = None
@@ -108,22 +109,22 @@
         corresponding Expected Return, Volatility and Sharpe Ratio.
 
         :Output:
          :(weights, quantities): Tuple of weights (np.ndarray) and a
              list of [expected return, volatility, sharpe ratio].
         """
         # select random weights for portfolio
-        w = np.array(np.random.random(self.num_stocks))
+        weights = np.array(np.random.random(self.num_stocks))
         # rebalance weights
-        w = w / np.sum(w)
+        weights = weights / np.sum(weights)
         # compute portfolio return and volatility
         portfolio_values = annualised_portfolio_quantities(
-            w, self.return_means, self.cov_matrix, self.risk_free_rate, self.freq
+            weights, self.return_means, self.cov_matrix, self.risk_free_rate, self.freq
         )
-        return (w, np.array(portfolio_values))
+        return (weights, np.array(portfolio_values))
 
     def _random_portfolios(self):
         """Performs a Monte Carlo run and gets a list of random portfolios
         and their corresponding quantities (Expected Return, Volatility,
         Sharpe Ratio). Returns ``pandas.DataFrame`` of weights and results.
 
         :Output:
@@ -181,15 +182,15 @@
         """
         if (
             self.df_results is None
             or self.df_weights is None
             or self.opt_weights is None
             or self.opt_results is None
         ):
-            raise Exception(
+            raise ValueError(
                 "Error: Cannot plot, run the Monte Carlo " + "optimisation first."
             )
         # create scatter plot coloured by Sharpe Ratio
         plt.scatter(
             self.df_results["Volatility"],
             self.df_results["Expected Return"],
             c=self.df_results["Sharpe Ratio"],
@@ -248,26 +249,20 @@
     def properties(self):
         """Prints out the properties of the Monte Carlo optimisation."""
         # print out results
         opt_vals = ["Min Volatility", "Max Sharpe Ratio"]
         string = ""
         for val in opt_vals:
             string += "-" * 70
-            string += "\nOptimised portfolio for {}".format(
-                val.replace("Min", "Minimum").replace("Max", "Maximum")
-            )
-            string += "\n\nTime period: {} days".format(self.freq)
-            string += "\nExpected return: {0:0.3f}".format(
-                self.opt_results.loc[val]["Expected Return"]
-            )
-            string += "\nVolatility: {:0.3f}".format(
-                self.opt_results.loc[val]["Volatility"]
-            )
-            string += "\nSharpe Ratio: {:0.3f}".format(
-                self.opt_results.loc[val]["Sharpe Ratio"]
+            string += f"\nOptimised portfolio for {val.replace('Min', 'Minimum').replace('Max', 'Maximum')}"
+            string += f"\n\nTime period: {self.freq} days"
+            string += f"\nExpected return: {self.opt_results.loc[val]['Expected Return']:0.3f}"
+            string += f"\nVolatility: {self.opt_results.loc[val]['Volatility']:0.3f}"
+            string += (
+                f"\nSharpe Ratio: {self.opt_results.loc[val]['Sharpe Ratio']:0.3f}"
             )
             string += "\n\nOptimal weights:"
             string += "\n" + str(
                 self.opt_weights.loc[val]
                 .to_frame()
                 .transpose()
                 .rename(index={val: "Allocation"})
```

### Comparing `FinQuant-0.3.0/finquant/moving_average.py` & `FinQuant-0.3.1/finquant/moving_average.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,41 +3,51 @@
 - *Simple Moving Averages*,
 - *Exponential Moving Averages*,
 - a *band* of *Moving Averages* (simple or exponential), and
 - *Bollinger Bands*.
 """
 
 
+from typing import Callable, List
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
 
 
-def compute_ma(data, fun, spans, plot=True):
+def compute_ma(
+    data, fun: Callable, spans: List[int], plot: bool = True
+) -> pd.DataFrame:
     """Computes a band of moving averages (sma or ema, depends on the input argument
     `fun`) for a number of different time windows. If `plot` is `True`, it also
     computes and sets markers for buy/sell signals based on crossovers of the Moving
     Averages with the shortest/longest spans.
 
     :Input:
-     :data: pandas.DataFrame with stock prices, only one column is expected.
+     :data: pandas.DataFrame, or pandas.Series, with stock prices
+         (if pandas.DataFrame: only one column is expected)
      :fun: function that computes a moving average, e.g. sma (simple) or
          ema (exponential).
      :spans: list of integers, time windows to compute the Moving Average on.
      :plot: boolean (default: True), whether to plot the moving averages
-         and buy/sell signales based on crossovers of shortest and longest
+         and buy/sell signals based on crossovers of shortest and longest
          moving average.
 
     :Output:
      :ma: pandas.DataFrame with moving averages of given data.
     """
-    if not isinstance(data, pd.DataFrame):
-        raise ValueError("data must be of type pandas.DataFrame")
-    # compute moving averages
+    if not isinstance(data, (pd.Series, pd.DataFrame)):
+        raise ValueError(
+            "data is expected to be of type pandas.Series or pandas.DataFrame"
+        )
     ma = data.copy(deep=True)
+    # converting data to pd.DataFrame if it is a pd.Series (for subsequent function calls):
+    if isinstance(ma, pd.Series):
+        ma = ma.to_frame()
+    # compute moving averages
     for span in spans:
         ma[str(span) + "d"] = fun(data, span=span)
     if plot:
         fig = plt.figure()
         ax = fig.add_subplot(111)
         # plot moving averages
         ma.plot(ax=ax)
@@ -78,94 +88,99 @@
         plt.legend(ncol=2)
         # axis labels
         plt.xlabel(data.index.name)
         plt.ylabel("Price")
     return ma
 
 
-def sma(data, span=100):
+def sma(data: pd.DataFrame, span: int = 100) -> pd.DataFrame:
     """Computes and returns the simple moving average.
 
     Note: the moving average is computed on all columns.
 
     :Input:
      :data: pandas.DataFrame with stock prices in columns
-     :span: int (defaul: 100), number of days/values over which
+     :span: int (default: 100), number of days/values over which
          the average is computed
 
     :Output:
      :sma: pandas.DataFrame of simple moving average
     """
     return data.rolling(window=span, center=False).mean()
 
 
-def ema(data, span=100):
+def ema(data: pd.DataFrame, span: int = 100) -> pd.DataFrame:
     """Computes and returns the exponential moving average.
 
     Note: the moving average is computed on all columns.
 
     :Input:
      :data: pandas.DataFrame with stock prices in columns
-     :span: int (defaul: 100), number of days/values over which
+     :span: int (default: 100), number of days/values over which
          the average is computed
 
     :Output:
      :ema: pandas.DataFrame of exponential moving average
     """
     return data.ewm(span=span, adjust=False, min_periods=span).mean()
 
 
-def sma_std(data, span=100):
+def sma_std(data: pd.DataFrame, span: int = 100) -> pd.DataFrame:
     """Computes and returns the standard deviation of the simple moving
     average.
 
     :Input:
      :data: pandas.DataFrame with stock prices in columns
-     :span: int (defaul: 100), number of days/values over which
+     :span: int (default: 100), number of days/values over which
          the average is computed
 
     :Output:
      :sma_std: pandas.DataFrame of standard deviation of
          simple moving average
     """
     return data.rolling(window=span, center=False).std()
 
 
-def ema_std(data, span=100):
+def ema_std(data: pd.DataFrame, span: int = 100) -> pd.DataFrame:
     """Computes and returns the standard deviation of the exponential
     moving average.
 
     :Input:
      :data: pandas.DataFrame with stock prices in columns
-     :span: int (defaul: 100), number of days/values over which
+     :span: int (default: 100), number of days/values over which
          the average is computed
 
     :Output:
      :ema_std: pandas.DataFrame of standard deviation of
          exponential moving average
     """
     return data.ewm(span=span, adjust=False, min_periods=span).std()
 
 
-def plot_bollinger_band(data, fun, span):
+def plot_bollinger_band(data, fun: Callable, span: int = 100) -> None:
     """Computes and visualises a Bolling Band.
 
     :Input:
-     :data: pandas.DataFrame with stock prices in columns
+     :data: pandas.Series or pandas.DataFrame with stock prices in columns
      :fun: function that computes a moving average, e.g. sma (simple) or
          ema (exponential).
-     :span: int (defaul: 100), number of days/values over which
+     :span: int (default: 100), number of days/values over which
          the average is computed
     """
-    if not isinstance(data, pd.DataFrame):
-        raise ValueError("data is expected to be a pandas.DataFrame")
-    if not len(data.columns.values) == 1:
+    if not isinstance(data, (pd.Series, pd.DataFrame)):
+        raise ValueError(
+            "data is expected to be of type pandas.Series or pandas.DataFrame"
+        )
+    if isinstance(data, pd.DataFrame) and not len(data.columns.values) == 1:
         raise ValueError("data is expected to have only one column.")
     if not isinstance(span, int):
         raise ValueError("span must be an integer.")
+    # converting data to pd.DataFrame if it is a pd.Series (for subsequent function calls):
+    if isinstance(data, pd.Series):
+        data = data.to_frame()
     # compute moving average
     ma = compute_ma(data, fun, [span], plot=False)
     # create dataframes for bollinger band object and standard
     # deviation
     bol = ma.copy(deep=True)
     std = ma.copy(deep=True)
     # get column label
```

### Comparing `FinQuant-0.3.0/finquant/portfolio.py` & `FinQuant-0.3.1/finquant/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 Furthermore, the constructed portfolio can be optimised for
 
 - minimum Volatility,
 - maximum Sharpe Ratio
 - minimum Volatility for a given Expected Return
 - maximum Sharpe Ratio for a given target Volatility
 
-by either performing a numerical computation to solve a minimisation problem, or by performing a Monte Carlo simulation of `n` trials.
+by either performing a numerical computation to solve a minimisation problem,
+or by performing a Monte Carlo simulation of `n` trials.
 The former should be the preferred method for reasons of computational effort
 and accuracy. The latter is only included for the sake of completeness.
 
 Finally, functions are implemented to generated the following plots:
 
 - Monte Carlo run to find optimal portfolio(s)
 - Efficient Frontier
@@ -43,29 +44,35 @@
 - Portfolio with the minimum Volatility for a given Expected Return based
   on a numerical optimisation
 - Portfolio with the maximum Sharpe Ratio for a given target Volatility
   based on a numerical optimisation
 - Individual stocks of the portfolio (Expected Return over Volatility)
 """
 
+from typing import List
+import datetime
 
+import matplotlib.pylab as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pylab as plt
-from finquant.quants import weighted_mean, weighted_std, sharpe_ratio
-from finquant.returns import historical_mean_return
-from finquant.returns import daily_returns, cumulative_returns
-from finquant.returns import daily_log_returns
-from finquant.stock import Stock
+
 from finquant.efficient_frontier import EfficientFrontier
-from finquant.monte_carlo import MonteCarloOpt
 from finquant.market import Market
+from finquant.monte_carlo import MonteCarloOpt
+from finquant.quants import sharpe_ratio, weighted_mean, weighted_std
+from finquant.returns import (
+    cumulative_returns,
+    daily_log_returns,
+    daily_returns,
+    historical_mean_return,
+)
+from finquant.stock import Stock
 
 
-class Portfolio(object):
+class Portfolio:
     """Object that contains information about an investment portfolio.
     To initialise the object, it does not require any input.
     To fill the portfolio with investment information, the
     function ``add_stock(stock)`` should be used, in which ``stock`` is
     an object of ``Stock``.
     """
 
@@ -99,62 +106,59 @@
 
     @totalinvestment.setter
     def totalinvestment(self, val):
         if val is not None:
             # treat "None" as initialisation
             if not isinstance(val, (float, int, np.floating, np.integer)):
                 raise ValueError("Total investment must be a float or integer.")
-            elif val <= 0:
+            if val <= 0:
                 raise ValueError(
                     "The money to be invested in the portfolio must be > 0."
                 )
-            else:
-                self.__totalinvestment = val
+            self.__totalinvestment = val
 
     @property
     def freq(self):
         return self.__freq
 
     @freq.setter
     def freq(self, val):
         if not isinstance(val, int):
             raise ValueError("Time window/frequency must be an integer.")
-        elif val <= 0:
+        if val <= 0:
             raise ValueError("freq must be > 0.")
-        else:
-            self.__freq = val
-            # now that this changed, update other quantities
-            self._update()
+        self.__freq = val
+        # now that this changed, update other quantities
+        self._update()
 
     @property
     def risk_free_rate(self):
         return self.__risk_free_rate
 
     @risk_free_rate.setter
     def risk_free_rate(self, val):
         if not isinstance(val, (float, int)):
             raise ValueError("Risk free rate must be a float or an integer.")
-        else:
-            self.__risk_free_rate = val
-            # now that this changed, update other quantities
-            self._update()
+        self.__risk_free_rate = val
+        # now that this changed, update other quantities
+        self._update()
 
     @property
     def market_index(self) -> Market:
         return self.__market_index
 
     @market_index.setter
     def market_index(self, index: Market) -> None:
         """Set the market index to the portfolio.
 
         :param index: An object of the ``Market`` class.
         """
         self.__market_index = index
 
-    def add_stock(self, stock):
+    def add_stock(self, stock: Stock) -> None:
         """Adds a stock of type ``Stock`` to the portfolio. Each time ``add_stock``
         is called, the following instance variables are updated:
 
         - ``portfolio``: ``pandas.DataFrame``, adds a column with information from ``stock``
         - ``stocks``: ``dictionary``, adds an entry for ``stock``
         - ``data``: ``pandas.DataFrame``, adds a column of stock prices from ``stock``
 
@@ -177,35 +181,35 @@
         )
         # setting an appropriate name for the portfolio
         self.portfolio.name = "Allocation of stocks"
         # also add stock data of stock to the dataframe
         self._add_stock_data(stock)
 
         # update quantities of portfolio
-        self._update()
+        # self._update() # the update will be done at the end of building portfolio
 
     def _add_stock_data(self, stock: Stock) -> None:
-        # loop over columns in given dataframe
-        for datacol in stock.data.columns:
-            cols = len(self.data.columns)
-            self.data.insert(loc=cols, column=datacol, value=stock.data[datacol].values)
+        # insert given data into portfolio stocks dataframe:
+        self.data.insert(
+            loc=len(self.data.columns), column=stock.name, value=stock.data
+        )
         # set index correctly
         self.data.set_index(stock.data.index.values, inplace=True)
         # set index name:
         self.data.index.rename("Date", inplace=True)
 
         if self.market_index is not None:
             # compute beta parameter of stock
             beta_stock = stock.comp_beta(self.market_index.daily_returns)
             # add beta of stock to portfolio's betas dataframe
             self.beta_stocks[stock.name] = [beta_stock]
 
     def _update(self):
         # sanity check (only update values if none of the below is empty):
-        if not (self.portfolio.empty or self.stocks == {} or self.data.empty):
+        if not (self.portfolio.empty or not self.stocks or self.data.empty):
             self.totalinvestment = self.portfolio.Allocation.sum()
             self.expected_return = self.comp_expected_return(freq=self.freq)
             self.volatility = self.comp_volatility(freq=self.freq)
             self.sharpe = self.comp_sharpe()
             self.skew = self._comp_skew()
             self.kurtosis = self._comp_kurtosis()
             if self.market_index is not None:
@@ -632,24 +636,24 @@
         - Kurtosis
 
         as well as the allocation of the stocks across the portfolio.
         """
         # nicely printing out information and quantities of the portfolio
         string = "-" * 70
         stocknames = self.portfolio.Name.values.tolist()
-        string += "\nStocks: {}".format(", ".join(stocknames))
+        string += f"\nStocks: {', '.join(stocknames)}"
         if self.market_index is not None:
-            string += "\nMarket Index: {}".format(self.market_index.name)
-        string += "\nTime window/frequency: {}".format(self.freq)
-        string += "\nRisk free rate: {}".format(self.risk_free_rate)
-        string += "\nPortfolio Expected Return: {:0.3f}".format(self.expected_return)
-        string += "\nPortfolio Volatility: {:0.3f}".format(self.volatility)
-        string += "\nPortfolio Sharpe Ratio: {:0.3f}".format(self.sharpe)
+            string += f"\nMarket Index: {self.market_index.name}"
+        string += f"\nTime window/frequency: {self.freq}"
+        string += f"\nRisk free rate: {self.risk_free_rate}"
+        string += f"\nPortfolio Expected Return: {self.expected_return:0.3f}"
+        string += f"\nPortfolio Volatility: {self.volatility:0.3f}"
+        string += f"\nPortfolio Sharpe Ratio: {self.sharpe:0.3f}"
         if self.beta is not None:
-            string += "\nPortfolio Beta: {:0.3f}".format(self.beta)
+            string += f"\nPortfolio Beta: {self.beta:0.3f}"
         string += "\n\nSkewness:"
         string += "\n" + str(self.skew.to_frame().transpose())
         string += "\n\nKurtosis:"
         string += "\n" + str(self.kurtosis.to_frame().transpose())
         string += "\n\nInformation:"
         string += "\n" + str(self.portfolio)
         string += "\n"
@@ -692,21 +696,21 @@
             + "Please make sure that it is installed."
         )
     # get correct stock names that quandl.get can request,
     # e.g. "WIKI/GOOG" for Google
     reqnames = _correct_quandl_request_stock_name(names)
     try:
         resp = quandl.get(reqnames, start_date=start_date, end_date=end_date)
-    except Exception:
+    except Exception as exc:
         errormsg = (
             "Error during download of stock data from Quandl.\n"
             + "Make sure all the requested stock names/tickers are "
             + "supported by Quandl."
         )
-        raise Exception(errormsg)
+        raise Exception(errormsg) from exc
     return resp
 
 
 def _yfinance_request(names, start_date=None, end_date=None):
     """This function performs a simple request from Yahoo Finance
     (using `yfinance`) and returns a ``pandas.DataFrame``
     containing stock data.
@@ -724,40 +728,40 @@
         print(
             "The following package is required:\n - `yfinance`\n"
             + "Please make sure that it is installed."
         )
     # yfinance does not exit safely if start/end date were not given correctly:
     # this step is not required for quandl as it handles this exception properly
     try:
-        import datetime
-
         if isinstance(start_date, str):
             start_date = datetime.datetime.strptime(start_date, "%Y-%m-%d")
         if isinstance(end_date, str):
             end_date = datetime.datetime.strptime(end_date, "%Y-%m-%d")
     except ImportError:
         print(
             "The following package is required:\n - `datetime`\n"
             + "Please make sure that it is installed."
         )
-    except Exception:
-        raise Exception("Please provide valid values for <start_date> and <end_date>")
+    except Exception as exc:
+        raise Exception(
+            "Please provide valid values for <start_date> and <end_date>"
+        ) from exc
 
     # unlike quandl, yfinance does not have a prefix in front of the ticker
     # thus we do not need to correct them
     try:
         resp = yf.download(names, start=start_date, end=end_date)
         if not isinstance(resp.columns, pd.MultiIndex) and len(names) > 0:
             # for single stock must make the dataframe multiindex
             stock_tuples = [(col, names[0]) for col in list(resp.columns)]
             resp.columns = pd.MultiIndex.from_tuples(stock_tuples)
-    except Exception:
+    except Exception as exc:
         raise Exception(
             "Error during download of stock data from Yahoo Finance with `yfinance`."
-        )
+        ) from exc
     return resp
 
 
 def _get_quandl_data_column_label(stock_name, data_label):
     """Given stock name and label of a data column, this function returns
     the string "<stock_name> - <data_label>" as it can be found in a
     ``pandas.DataFrame`` returned by `quandl`.
@@ -819,31 +823,29 @@
             else:
                 raise ValueError("Could not find column labels in given dataframe.")
             # append correct name to list of correct names
             reqcolnames.append(colname)
 
     # if data comes from yfinance, it is a multiindex dataframe:
     if isinstance(data.columns, pd.MultiIndex):
-        if not len(firstlevel_colnames) == 1:
+        if len(firstlevel_colnames) != 1:
             raise ValueError(
                 "Sorry, for now only one value/quantity per Stock is supported."
             )
         data = data[firstlevel_colnames[0]].loc[:, reqcolnames]
     else:
         # if it comes from quandl, it is not of type multiindex
         data = data.loc[:, reqcolnames]
 
     # if only one data column per stock exists, rename column labels
     # to the name of the corresponding stock
     newcolnames = {}
     if len(cols) == 1:
-        for i in range(len(names)):
-            newcolnames.update(
-                {_get_quandl_data_column_label(names[i], cols[0]): names[i]}
-            )
+        for i, name in enumerate(names):
+            newcolnames.update({_get_quandl_data_column_label(name, cols[0]): name})
         data.rename(columns=newcolnames, inplace=True)
     return data
 
 
 def _build_portfolio_from_api(
     names,
     pf_allocation=None,
@@ -877,27 +879,28 @@
     """
     # create an empty portfolio
     pf = Portfolio()
     # create empty dataframe for market data
     market_data = pd.DataFrame()
     # request data from service:
     if data_api == "yfinance":
-        data = _yfinance_request(names, start_date, end_date)
+        stock_data = _yfinance_request(names, start_date, end_date)
         if market_index is not None:
             market_data = _yfinance_request([market_index], start_date, end_date)
     elif data_api == "quandl":
-        data = _quandl_request(names, start_date, end_date)
+        stock_data = _quandl_request(names, start_date, end_date)
         if market_index is not None:
             # only generated if user explicitly requests market index with quandl
             raise Warning("Market index is not supported for quandl data.")
+
     # check pf_allocation:
     if pf_allocation is None:
         pf_allocation = _generate_pf_allocation(names=names)
     # build portfolio:
-    pf = _build_portfolio_from_df(data, pf_allocation, market_data=market_data)
+    pf = _build_portfolio_from_df(stock_data, pf_allocation, market_data=market_data)
     return pf
 
 
 def _stocknames_in_data_columns(names, df):
     """Returns True if at least one element of names was found as a column
     label in the dataframe df.
     """
@@ -938,55 +941,48 @@
     if data is not None and not isinstance(data, pd.DataFrame):
         raise ValueError("data is expected to be of type 'pandas.DataFrame'.")
     # if data is given:
     if data is not None:
         # this case is more complex, as we need to check for column labels in
         # data
         names = data.columns
+        # potential error message
+        errormsg = (
+            "'data' pandas.DataFrame contains conflicting column labels."
+            + "\nMultiple columns with a substring of\n {}\n"
+            + "were found. You have two options:"
+            + "\n 1. call 'build_portfolio' and pass a pandas.DataFrame "
+            + "'pf_allocation' that contains the weights/allocation of stocks "
+            + "within your portfolio. 'build_portfolio' will then extract the "
+            + "columns from 'data' that match the values of the column 'Name' in "
+            + "the pandas.DataFrame 'pf_allocation'."
+            + "\n 2. call 'build_portfolio' and pass a pandas.DataFrame 'data' "
+            + "that does not have conflicting column labels, e.g. 'GOOG' and "
+            + "'GOOG - Adj. Close' are considered conflicting column headers."
+        )
         # sanity check: split names at '-' and take the leading part of the
         # split string, and check if this occurs in any of the other names.
         # if so, we treat this as a duplication, and ask the user to provide
         # a DataFrame with one data column per stock.
         splitnames = [name.split("-")[0].strip() for name in names]
-        for i in range(len(splitnames)):
-            splitname = splitnames[i]
-            reducedlist = [elt for num, elt in enumerate(splitnames) if not num == i]
+        for i, splitname in enumerate(splitnames):
+            reducedlist = [elt for num, elt in enumerate(splitnames) if num != i]
             if splitname in reducedlist:
-                errormsg = (
-                    "'data' pandas.DataFrame contains conflicting "
-                    + "column labels."
-                    + "\nMultiple columns with a substring of "
-                    + "\n "
-                    + str(splitname)
-                    + "\n"
-                    + "were found. You have two options:"
-                    + "\n 1. call 'build_portfolio' and pass a "
-                    + "pandas.DataFrame 'pf_allocation' that contains the "
-                    + "weights/allocation of stocks within your "
-                    + "portfolio. 'build_portfolio' will then extract "
-                    + "the columns from 'data' that match the values "
-                    + "of the column 'Name' in the pandas.DataFrame "
-                    + "'pf_allocation'."
-                    + "\n 2. call 'build_portfolio' and pass a "
-                    + "pandas.DataFrame 'data' that does not have conflicting "
-                    + "column labels, e.g. 'GOOG' and "
-                    + "'GOOG - Adj. Close' are considered "
-                    + "conflicting column headers."
-                )
+                errormsg = errormsg.format(str(splitname))
                 raise ValueError(errormsg)
     # if names is given, we go directly to the below:
     # compute equal weights
     weights = [1.0 / len(names) for i in range(len(names))]
     return pd.DataFrame({"Allocation": weights, "Name": names})
 
 
 def _build_portfolio_from_df(
     data: pd.DataFrame,
     pf_allocation: pd.DataFrame = None,
-    datacolumns: list = ["Adj. Close"],
+    datacolumns: List[str] = None,
     market_data: pd.DataFrame = None,
 ) -> Portfolio:
     """Returns a portfolio based on input in form of ``pandas.DataFrame``.
 
     :Input:
      :data: A ``pandas.DataFrame`` which contains prices of the stocks listed in
          pf_allocation
@@ -1002,40 +998,42 @@
     :Output:
      :pf: Instance of Portfolio which contains all the information
          requested by the user.
     """
     # if pf_allocation is None, automatically generate it
     if pf_allocation is None:
         pf_allocation = _generate_pf_allocation(data=data)
+    if datacolumns is None:
+        datacolumns = ["Adj. Close"]
     # make sure stock names are in data dataframe
     if not _stocknames_in_data_columns(pf_allocation.Name.values, data):
         raise ValueError(
             "Error: None of the provided stock names were"
             + "found in the provided dataframe."
         )
     # extract only "Adjusted Close" price ("Adj. Close" in quandl, "Adj Close" in yfinance)
     # column from DataFrame:
     data = _get_stocks_data_columns(data, pf_allocation.Name.values, datacolumns)
+
     # building portfolio:
     pf = Portfolio()
     if market_data is not None and not market_data.empty:
         # extract only "Adjusted Close" price column from market data
         market_data = _get_index_adj_clos_pr(market_data)
         # set market index of portfolio
         pf.market_index = Market(data=market_data)
     for i in range(len(pf_allocation)):
         # get name of stock
-        name = pf_allocation.loc[i].Name
-        # extract data column(s) of said stock
-        stock_data = data.loc[:, [name]].copy(deep=True)
-        # if only one data column per stock exists, give dataframe a name
-        if len(datacolumns) == 1:
-            stock_data.name = datacolumns[0]
+        name = pf_allocation.iloc[i].Name
+        # extract data column of said stock
+        stock_data = data.loc[:, [name]].copy(deep=True).squeeze()
         # create Stock instance and add it to portfolio
-        pf.add_stock(Stock(pf_allocation.loc[i], data=stock_data))
+        pf.add_stock(Stock(pf_allocation.iloc[i], data=stock_data))
+    # update the portfolio
+    pf._update()
     return pf
 
 
 def _all_list_ele_in_other(l1, l2):
     """Returns True if all elements of list l1 are found in list l2."""
     return all(ele in l2 for ele in l1)
 
@@ -1087,16 +1085,16 @@
 
      The two different ways this function can be used are useful for:
 
      1. building a portfolio by pulling data from `quandl`/`yfinance`,
      2. building a portfolio by providing stock data which was obtained otherwise,
         e.g. from data files.
 
-     If used in an unsupported way, the function (or subsequently called function) raises appropriate Exceptions
-     with useful information what went wrong.
+     If used in an unsupported way, the function (or subsequently called function)
+     raises appropriate Exceptions with useful information what went wrong.
     """
     docstring_msg = (
         "Please read through the docstring, "
         "'build_portfolio.__doc__' and/or have a look at the "
         "examples in `examples/`."
     )
     input_error = (
@@ -1119,15 +1117,15 @@
         "end_date",
         "data",
         "data_api",
         "market_index",
     ]
 
     # check if no input argument was passed
-    if kwargs == {}:
+    if not kwargs:
         raise ValueError(
             "Error:\nbuild_portfolio() requires input " + "arguments.\n" + docstring_msg
         )
     # check for valid input arguments
     if not _all_list_ele_in_other(kwargs.keys(), all_input_args):
         unsupported_input = _list_complement(all_input_args, kwargs.keys())
         raise ValueError(
@@ -1167,18 +1165,19 @@
             raise ValueError(
                 input_comb_error.format(complement_input_args, allowed_mandatory_args)
             )
         # get portfolio:
         pf = _build_portfolio_from_df(**kwargs)
 
     # final check
+    # pylint: disable=R0916
     if (
         pf.portfolio.empty
         or pf.data.empty
-        or pf.stocks == {}
+        or not pf.stocks
         or pf.expected_return is None
         or pf.volatility is None
         or pf.sharpe is None
         or pf.skew is None
         or pf.kurtosis is None
     ):
         raise ValueError(
```

### Comparing `FinQuant-0.3.0/finquant/quants.py` & `FinQuant-0.3.1/finquant/quants.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.0/finquant/returns.py` & `FinQuant-0.3.1/finquant/returns.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import numpy as np
 import pandas as pd
 
 
 def cumulative_returns(data, dividend=0):
     """Returns DataFrame with cumulative returns
 
-    :math:`\\displaystyle R = \\dfrac{\\text{price}_{t_i} - \\text{price}_{t_0} + \\text{dividend}}{\\text{price}_{t_0}}`
+    :math:`\\displaystyle R = \\dfrac{\\text{price}_{t_i} - \\text{price}_{t_0} + \\text{dividend}}
+    {\\text{price}_{t_0}}`
 
     :Input:
      :data: ``pandas.DataFrame`` with daily stock prices
      :dividend: ``float`` (default= ``0``), paid dividend
 
     :Output:
      :ret: a ``pandas.DataFrame`` of cumulative Returns of given stock prices.
@@ -35,15 +36,16 @@
     return data.pct_change().dropna(how="all").replace([np.inf, -np.inf], np.nan)
 
 
 def daily_log_returns(data):
     """
     Returns DataFrame with daily log returns
 
-    :math:`R_{\\log} = \\log\\left(1 + \\dfrac{\\text{price}_{t_i} - \\text{price}_{t_{i-1}}}{\\text{price}_{t_{i-1}}}\\right)`
+    :math:`R_{\\log} = \\log\\left(1 + \\dfrac{\\text{price}_{t_i} - \\text{price}_{t_{i-1}}}
+    {\\text{price}_{t_{i-1}}}\\right)`
 
     :Input:
      :data: ``pandas.DataFrame`` with daily stock prices
 
     :Output:
      :ret: a ``pandas.DataFrame`` of
          log(1 + daily percentage change of Returns)
```

### Comparing `FinQuant-0.3.0/finquant/stock.py` & `FinQuant-0.3.1/finquant/stock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ This module provides a public class ``Stock`` that holds and calculates quantities of a single stock.
 Instances of this class are used in the ``Portfolio`` class (provided in ``finquant.portfolio``).   
 Every time a new instance of ``Stock`` is added to ``Portfolio``, the quantities of the portfolio are updated.  
 """
 
 import numpy as np
 import pandas as pd
-from finquant.returns import historical_mean_return
-from finquant.returns import daily_returns
 
+from finquant.returns import daily_returns, historical_mean_return
 
-class Stock(object):
+
+class Stock:
     """Object that contains information about a stock/fund.
     To initialise the object, it requires a name, information about
     the stock/fund given as one of the following data structures:
 
     - ``pandas.Series``
     - ``pandas.DataFrame``
 
@@ -31,15 +31,15 @@
     ``data`` must be given as a ``pandas.DataFrame``, and at least one data column
     is required to containing the closing price, hence it is required to
     contain one column label ``<stock_name> - Adj. Close`` which is used to
     compute the return of investment. However, ``data`` can contain more
     data in additional columns.
     """
 
-    def __init__(self, investmentinfo, data):
+    def __init__(self, investmentinfo: pd.DataFrame, data: pd.Series):
         """
         :Input:
          :investmentinfo: ``pandas.DataFrame`` of investment information
          :data: ``pandas.DataFrame`` of stock price
         """
         self.name = investmentinfo.Name
         self.investmentinfo = investmentinfo
@@ -81,50 +81,50 @@
         :Output:
          :volatility: Volatility of stock.
         """
         return self.comp_daily_returns().std() * np.sqrt(freq)
 
     def _comp_skew(self):
         """Computes and returns the skewness of the stock."""
-        return self.data.skew().values[0]
+        return self.data.skew()
 
     def _comp_kurtosis(self):
         """Computes and returns the Kurtosis of the stock."""
-        return self.data.kurt().values[0]
+        return self.data.kurt()
 
     def comp_beta(self, market_daily_returns: pd.Series) -> float:
         """Compute and return the Beta parameter of the stock.
 
         :Input:
          :market_daily_returns: ``pd.Series``, daily returns of the market
 
         :Output:
          :sharpe: ``float``, the Beta parameter of the stock
         """
         cov_mat = np.cov(
-            self.comp_daily_returns()[self.name],
+            self.comp_daily_returns(),
             market_daily_returns.to_frame()[market_daily_returns.name],
         )
 
         beta = cov_mat[0, 1] / cov_mat[1, 1]
         self.beta = beta
         return beta
 
     def properties(self):
         """Nicely prints out the properties of the stock: Expected Return,
         Volatility, Skewness, Kurtosis as well as the ``Allocation`` (and other
         information provided in investmentinfo.)
         """
         # nicely printing out information and quantities of the stock
         string = "-" * 50
-        string += "\nStock: {}".format(self.name)
-        string += "\nExpected Return:{:0.3f}".format(self.expected_return.values[0])
-        string += "\nVolatility: {:0.3f}".format(self.volatility.values[0])
-        string += "\nSkewness: {:0.5f}".format(self.skew)
-        string += "\nKurtosis: {:0.5f}".format(self.kurtosis)
+        string += f"\nStock: {self.name}"
+        string += f"\nExpected Return: {self.expected_return:0.3f}"
+        string += f"\nVolatility: {self.volatility:0.3f}"
+        string += f"\nSkewness: {self.skew:0.5f}"
+        string += f"\nKurtosis: {self.kurtosis:0.5f}"
         string += "\nInformation:"
         string += "\n" + str(self.investmentinfo.to_frame().transpose())
         string += "\n"
         string += "-" * 50
         print(string)
 
     def __str__(self):
```

### Comparing `FinQuant-0.3.0/setup.py` & `FinQuant-0.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import setuptools
 
+
+def read_file(file_path):
+    with open(file_path, "r") as f:
+        return f.read()
+
+
 # get version/release from file
-with open("version", "r") as f:
-    version = dict(x.rstrip().split("=") for x in f)
+version = dict(line.rstrip().split("=") for line in read_file("version").splitlines())
 
 # get long description from README
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+long_description = read_file("README.md")
+
 
 # get dependencies
 def read_requirements(file_path):
-    with open(file_path, "r") as f:
-        return [line.strip() for line in f if line.strip()]
+    return [line.strip() for line in read_file(file_path).splitlines() if line.strip()]
+
 
 install_requires = read_requirements("requirements.txt")
 
 extras_require = {
     "test": read_requirements("requirements_test.txt"),
     "dev": read_requirements("requirements_dev.txt"),
     "docs": read_requirements("requirements_docs.txt"),
+    "cd": read_requirements("requirements_cd.txt"),
 }
 
 setuptools.setup(
     name="FinQuant",
     version=version["version"],
     author="Frank Milthaler",
     author_email="f.milthaler@gmail.com",
     description="A program for financial portfolio management, analysis and optimisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fmilthaler/FinQuant",
-    download_url="https://github.com/fmilthaler/FinQuant/archive/v{}.tar.gz".format(
-        version["release"]
-    ),
+    download_url=f"https://github.com/fmilthaler/FinQuant/archive/v{version['release']}.tar.gz",
     license="MIT",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Other Audience",
```

### Comparing `FinQuant-0.3.0/tests/test_Example-Build-Portfolio-from-file.py` & `FinQuant-0.3.1/tests/test_Example-Build-Portfolio-from-file.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-# -*- coding: utf-8 -*-
-# <nbformat>4</nbformat>
-
-# <markdowncell>
-
-# # Building a portfolio with data from disk
-# ## Building a portfolio with `build_portfolio()` with data obtained from data files.
-# Note: The stock data is provided in two data files. The stock data was previously pulled from quandl.
-
-# <codecell>
-
-import pathlib
-import pandas as pd
-import datetime
-
-# importing FinQuant's function to automatically build the portfolio
-from finquant.portfolio import build_portfolio
-
-# <markdowncell>
-
-# ### Get data from disk/file
-# Here we use `pandas.read_cvs()` method to read in the data.
-
-# <codecell>
-
-# stock data was previously pulled from quandl and stored in ex1-stockdata.csv
-# commands used to save data:
-# pf.portfolio.to_csv("ex1-portfolio.csv", encoding='utf-8', index=False, header=True)
-# pf.data.to_csv("ex1-stockdata.csv", encoding='utf-8', index=True, index_label="Date")
-# read data from files:
-df_pf_path = pathlib.Path.cwd() / ".." / "data" / "ex1-portfolio.csv"
-df_data_path = pathlib.Path.cwd() / ".." / "data" / "ex1-stockdata.csv"
-df_pf = pd.read_csv(df_pf_path)
-df_data = pd.read_csv(df_data_path, index_col="Date", parse_dates=True)
-
-# <markdowncell>
-
-# ### Examining the DataFrames
-
-# <codecell>
-
-print(df_pf)
-
-# <codecell>
-
-print(df_data.head(3))
-
-# <markdowncell>
-
-# ## Building a portfolio with `build_portfolio()`
-# `build_portfolio()` is an interface that can be used in different ways. Two of which is shown below. For more information the docstring is shown below as well.
-# In this example `build_portfolio()` is being passed `df_data`, which was read in from file above.
-
-# <codecell>
-
-print(build_portfolio.__doc__)
-
-# <markdowncell>
-
-# ## Building a portfolio with data only
-# Below is an example of only passing a `DataFrame` containing data (e.g. stock prices) to `build_portfolio()` in order to build an instance of `Portfolio`. In this case, the allocation of stocks is automatically generated by equally distributing the weights across all stocks.
-
-# <codecell>
-
-# building a portfolio by providing stock data
-pf = build_portfolio(data=df_data)
-
-# <markdowncell>
-
-# ### Portfolio is successfully built
-# Below it is shown how the allocation of the stocks and the data (e.g. prices) of the stocks can be obtained from the object `pf`.
-
-# <codecell>
-
-# the portfolio information DataFrame
-print(pf.portfolio.name)
-print(pf.portfolio)
-
-# <codecell>
-
-# the portfolio stock data, prices DataFrame
-print(pf.data.head(3))
-
-# <markdowncell>
-
-# ## Building a portfolio with data and desired allocation
-# If a specific allocation of stocks in the portfolio is desired, a `DataFrame` such as `df_pf` (which was read from file above) can be passed to `build_portfolio()` as shown below.
-
-# <codecell>
-
-# building a portfolio by providing stock data
-# and a desired allocation
-pf2 = build_portfolio(data=df_data, pf_allocation=df_pf)
-
-# <codecell>
-
-# the portfolio information DataFrame
-print(pf2.portfolio.name)
-print(pf2.portfolio)
-
-# <codecell>
-
-# the portfolio stock data, prices DataFrame
-print(pf2.data.head(3))
+# -*- coding: utf-8 -*-
+# <nbformat>4</nbformat>
+
+# <markdowncell>
+
+# # Building a portfolio with data from disk
+# ## Building a portfolio with `build_portfolio()` with data obtained from data files.
+# Note: The stock data is provided in two data files. The stock data was previously pulled from quandl.
+
+# <codecell>
+
+import pathlib
+import pandas as pd
+import datetime
+
+# importing FinQuant's function to automatically build the portfolio
+from finquant.portfolio import build_portfolio
+
+# <markdowncell>
+
+# ### Get data from disk/file
+# Here we use `pandas.read_cvs()` method to read in the data.
+
+# <codecell>
+
+# stock data was previously pulled from quandl and stored in ex1-stockdata.csv
+# commands used to save data:
+# pf.portfolio.to_csv("ex1-portfolio.csv", encoding='utf-8', index=False, header=True)
+# pf.data.to_csv("ex1-stockdata.csv", encoding='utf-8', index=True, index_label="Date")
+# read data from files:
+df_pf_path = pathlib.Path.cwd() / ".." / "data" / "ex1-portfolio.csv"
+df_data_path = pathlib.Path.cwd() / ".." / "data" / "ex1-stockdata.csv"
+df_pf = pd.read_csv(df_pf_path)
+df_data = pd.read_csv(df_data_path, index_col="Date", parse_dates=True)
+
+# <markdowncell>
+
+# ### Examining the DataFrames
+
+# <codecell>
+
+print(df_pf)
+
+# <codecell>
+
+print(df_data.head(3))
+
+# <markdowncell>
+
+# ## Building a portfolio with `build_portfolio()`
+# `build_portfolio()` is an interface that can be used in different ways. Two of which is shown below. For more information the docstring is shown below as well.
+# In this example `build_portfolio()` is being passed `df_data`, which was read in from file above.
+
+# <codecell>
+
+print(build_portfolio.__doc__)
+
+# <markdowncell>
+
+# ## Building a portfolio with data only
+# Below is an example of only passing a `DataFrame` containing data (e.g. stock prices) to `build_portfolio()` in order to build an instance of `Portfolio`. In this case, the allocation of stocks is automatically generated by equally distributing the weights across all stocks.
+
+# <codecell>
+
+# building a portfolio by providing stock data
+pf = build_portfolio(data=df_data)
+
+# <markdowncell>
+
+# ### Portfolio is successfully built
+# Below it is shown how the allocation of the stocks and the data (e.g. prices) of the stocks can be obtained from the object `pf`.
+
+# <codecell>
+
+# the portfolio information DataFrame
+print(pf.portfolio.name)
+print(pf.portfolio)
+
+# <codecell>
+
+# the portfolio stock data, prices DataFrame
+print(pf.data.head(3))
+
+# <markdowncell>
+
+# ## Building a portfolio with data and desired allocation
+# If a specific allocation of stocks in the portfolio is desired, a `DataFrame` such as `df_pf` (which was read from file above) can be passed to `build_portfolio()` as shown below.
+
+# <codecell>
+
+# building a portfolio by providing stock data
+# and a desired allocation
+pf2 = build_portfolio(data=df_data, pf_allocation=df_pf)
+
+# <codecell>
+
+# the portfolio information DataFrame
+print(pf2.portfolio.name)
+print(pf2.portfolio)
+
+# <codecell>
+
+# the portfolio stock data, prices DataFrame
+print(pf2.data.head(3))
```

### Comparing `FinQuant-0.3.0/tests/test_Example-Build-Portfolio-from-web.py` & `FinQuant-0.3.1/tests/test_Example-Build-Portfolio-from-web.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-# -*- coding: utf-8 -*-
-# <nbformat>4</nbformat>
-
-# <markdowncell>
-
-# # Building a portfolio with data from `quandl`/`yfinance`
-# ## Building a portfolio with `build_portfolio()` by downloading relevant data through `quandl`/`yfinance` with stock names, start and end date and column labels
-# This example only focuses on how to use `build_portfolio()` to get an instance of `Portfolio` by providing a few items of information that is passed on to `quandl`/`yfinance`. For a more exhaustive description of this package and example, please try `Example-Analysis` and `Example-Optimisation`.
-
-# <codecell>
-
-import pandas as pd
-import datetime
-
-# importing some custom functions/objects
-from finquant.portfolio import build_portfolio
-import os;import quandl;quandl.ApiConfig.api_key = os.getenv("QUANDLAPIKEY")
-
-# <markdowncell>
-
-# ## Get data from `quandl`/`yfinance` and build portfolio
-# First we need to build a pandas.DataFrame that holds relevant data for our portfolio. The minimal information needed are stock names and the amount of money to be invested in them, e.g. Allocation.
-
-# <codecell>
-
-# To play around yourself with different stocks, here is a short list of companies and their tickers on Yahoo Finance:
-# d = {0: {'Name':'GOOG', 'Allocation':20},  # Google
-#      1: {'Name':'AMZN', 'Allocation':33},  # Amazon
-#      2: {'Name':'MSFT', 'Allocation':18},  # Microsoft
-#      3: {'Name':'AAPL', 'Allocation':10},  # Apple
-#      4: {'Name':'KO', 'Allocation':15},    # Coca-Cola
-#      5: {'Name':'XOM', 'Allocation':11},   # Exxon Mobil
-#      6: {'Name':'JPM', 'Allocation':21},   # JP Morgan
-#      7: {'Name':'DIS', 'Allocation':9},    # Disney
-#      8: {'Name':'MCD', 'Allocation':23},   # McDonald's
-#      9: {'Name':'WMT', 'Allocation':3},    # Walmart
-#     10: {'Name':'GS', 'Allocation':9},     # Goldman Sachs
-#     }
-
-# <codecell>
-
-d = {
-    0: {"Name": "GOOG", "Allocation": 20},
-    1: {"Name": "AMZN", "Allocation": 10},
-    2: {"Name": "MCD", "Allocation": 15},
-    3: {"Name": "DIS", "Allocation": 18},
-}
-# If you wish to use `quandl` as source, you must add "WIKI/" at the beginning of stock names/tickers, as "WIKI/GOOG".
-
-pf_allocation = pd.DataFrame.from_dict(d, orient="index")
-
-# <markdowncell>
-
-# ### User friendly interface to quandl/yfinance
-# As mentioned above, in this example `build_portfolio()` is used to build a portfolio by performing a query to `quandl`/`yfinance`. We mention that `quandl` will be removed in future versions of `FinQuant` as it is deprecated.
-#
-# To download Google's stock data, `quandl` requires the string `"WIKI/GOOG"` and `yfinance` the string `"GOOG"`.
-# For simplicity, `FinQuant` facilitates a set of functions under the hood to sort out lots of specific commands/required input for `quandl`/`yfinance`. When using `FinQuant`, the user simply needs to provide a list of stock names/tickers.
-# For example, if using `quandl` as a data source (currently the default option), a list of names/tickers as shown below is a valid input for `FinQuant`'s function `build_portfolio(names=names)`:
-#  * `names = ["WIKI/GOOG", "WIKI/AMZN"]`
-#
-# If using `yfinance` as a data source, `FinQuant`'s function `build_portfolio(names=names)` expects the stock names to be without any leading/trailing string (check Yahoo Finance for correct stock names):
-#  * `names = ["GOOG", "AMZN"]`
-#
-# By default, `FinQuant` currently uses `quandl` to obtain stock price data. The function `build_portfolio()` can be called with the optional argument `data_api` to use `yfinance` instead:
-#  * `build_portfolio(names=names, data_api="yfinance")`
-#
-# In the below example we are using `yfinance` to download stock data. We specify the start and end date of the stock prices to be downloaded.
-# We also provide the optional parameter `market_index` to download the historical data of a market index. `FinQuant` can use them to calculate the beta parameter, measuring the portfolio's daily volatility compared to the market.
-
-# <codecell>
-
-# here we set the list of names based on the names in
-# the DataFrame pf_allocation
-names = pf_allocation["Name"].values.tolist()
-
-# dates can be set as datetime or string, as shown below:
-start_date = datetime.datetime(2015, 1, 1)
-end_date = "2017-12-31"
-
-# the market index used to compare the portfolio to (in this case S&P 500).
-# If the parameter is omitted, no market comparison will be done
-market_index = "^GSPC"
-
-# While quandl/yfinance will download lots of different prices for each stock,
-# e.g. high, low, close, etc, FinQuant will extract the column "Adj. Close" ("Adj Close" if using yfinance).
-
-pf = build_portfolio(
-    names=names,
-    pf_allocation=pf_allocation,
-    start_date=start_date,
-    end_date=end_date,
-    data_api="yfinance",
-    market_index=market_index,
-)
-
-# <markdowncell>
-
-# ## Portfolio is successfully built
-# Getting data from the portfolio
-
-# <codecell>
-
-# the portfolio information DataFrame
-print(pf.portfolio)
-
-# <codecell>
-
-# the portfolio stock data, prices DataFrame
-print(pf.data.head(3))
-
-# <codecell>
-
-# print out information and quantities of given portfolio
-print(pf)
-pf.properties()
-
-# <markdowncell>
-
-# ## Please continue with `Example-Build-Portfolio-from-file.py`.
-# As mentioned above, this example only shows how to use `build_portfolio()` to get an instance of `Portfolio` by downloading data through `quandl`/`yfinance`.
+# -*- coding: utf-8 -*-
+# <nbformat>4</nbformat>
+
+# <markdowncell>
+
+# # Building a portfolio with data from `quandl`/`yfinance`
+# ## Building a portfolio with `build_portfolio()` by downloading relevant data through `quandl`/`yfinance` with stock names, start and end date and column labels
+# This example only focuses on how to use `build_portfolio()` to get an instance of `Portfolio` by providing a few items of information that is passed on to `quandl`/`yfinance`. For a more exhaustive description of this package and example, please try `Example-Analysis` and `Example-Optimisation`.
+
+# <codecell>
+
+import pandas as pd
+import datetime
+
+# importing some custom functions/objects
+from finquant.portfolio import build_portfolio
+import os;import quandl;quandl.ApiConfig.api_key = os.getenv("QUANDLAPIKEY")
+
+# <markdowncell>
+
+# ## Get data from `quandl`/`yfinance` and build portfolio
+# First we need to build a pandas.DataFrame that holds relevant data for our portfolio. The minimal information needed are stock names and the amount of money to be invested in them, e.g. Allocation.
+
+# <codecell>
+
+# To play around yourself with different stocks, here is a short list of companies and their tickers on Yahoo Finance:
+# d = {0: {'Name':'GOOG', 'Allocation':20},  # Google
+#      1: {'Name':'AMZN', 'Allocation':33},  # Amazon
+#      2: {'Name':'MSFT', 'Allocation':18},  # Microsoft
+#      3: {'Name':'AAPL', 'Allocation':10},  # Apple
+#      4: {'Name':'KO', 'Allocation':15},    # Coca-Cola
+#      5: {'Name':'XOM', 'Allocation':11},   # Exxon Mobil
+#      6: {'Name':'JPM', 'Allocation':21},   # JP Morgan
+#      7: {'Name':'DIS', 'Allocation':9},    # Disney
+#      8: {'Name':'MCD', 'Allocation':23},   # McDonald's
+#      9: {'Name':'WMT', 'Allocation':3},    # Walmart
+#     10: {'Name':'GS', 'Allocation':9},     # Goldman Sachs
+#     }
+
+# <codecell>
+
+d = {
+    0: {"Name": "GOOG", "Allocation": 20},
+    1: {"Name": "AMZN", "Allocation": 10},
+    2: {"Name": "MCD", "Allocation": 15},
+    3: {"Name": "DIS", "Allocation": 18},
+}
+# If you wish to use `quandl` as source, you must add "WIKI/" at the beginning of stock names/tickers, as "WIKI/GOOG".
+
+pf_allocation = pd.DataFrame.from_dict(d, orient="index")
+
+# <markdowncell>
+
+# ### User friendly interface to quandl/yfinance
+# As mentioned above, in this example `build_portfolio()` is used to build a portfolio by performing a query to `quandl`/`yfinance`. We mention that `quandl` will be removed in future versions of `FinQuant` as it is deprecated.
+#
+# To download Google's stock data, `quandl` requires the string `"WIKI/GOOG"` and `yfinance` the string `"GOOG"`.
+# For simplicity, `FinQuant` facilitates a set of functions under the hood to sort out lots of specific commands/required input for `quandl`/`yfinance`. When using `FinQuant`, the user simply needs to provide a list of stock names/tickers.
+# For example, if using `quandl` as a data source (currently the default option), a list of names/tickers as shown below is a valid input for `FinQuant`'s function `build_portfolio(names=names)`:
+#  * `names = ["WIKI/GOOG", "WIKI/AMZN"]`
+#
+# If using `yfinance` as a data source, `FinQuant`'s function `build_portfolio(names=names)` expects the stock names to be without any leading/trailing string (check Yahoo Finance for correct stock names):
+#  * `names = ["GOOG", "AMZN"]`
+#
+# By default, `FinQuant` currently uses `quandl` to obtain stock price data. The function `build_portfolio()` can be called with the optional argument `data_api` to use `yfinance` instead:
+#  * `build_portfolio(names=names, data_api="yfinance")`
+#
+# In the below example we are using `yfinance` to download stock data. We specify the start and end date of the stock prices to be downloaded.
+# We also provide the optional parameter `market_index` to download the historical data of a market index. `FinQuant` can use them to calculate the beta parameter, measuring the portfolio's daily volatility compared to the market.
+
+# <codecell>
+
+# here we set the list of names based on the names in
+# the DataFrame pf_allocation
+names = pf_allocation["Name"].values.tolist()
+
+# dates can be set as datetime or string, as shown below:
+start_date = datetime.datetime(2015, 1, 1)
+end_date = "2017-12-31"
+
+# the market index used to compare the portfolio to (in this case S&P 500).
+# If the parameter is omitted, no market comparison will be done
+market_index = "^GSPC"
+
+# While quandl/yfinance will download lots of different prices for each stock,
+# e.g. high, low, close, etc, FinQuant will extract the column "Adj. Close" ("Adj Close" if using yfinance).
+
+pf = build_portfolio(
+    names=names,
+    pf_allocation=pf_allocation,
+    start_date=start_date,
+    end_date=end_date,
+    data_api="yfinance",
+    market_index=market_index,
+)
+
+# <markdowncell>
+
+# ## Portfolio is successfully built
+# Getting data from the portfolio
+
+# <codecell>
+
+# the portfolio information DataFrame
+print(pf.portfolio)
+
+# <codecell>
+
+# the portfolio stock data, prices DataFrame
+print(pf.data.head(3))
+
+# <codecell>
+
+# print out information and quantities of given portfolio
+print(pf)
+pf.properties()
+
+# <markdowncell>
+
+# ## Please continue with `Example-Build-Portfolio-from-file.py`.
+# As mentioned above, this example only shows how to use `build_portfolio()` to get an instance of `Portfolio` by downloading data through `quandl`/`yfinance`.
```

### Comparing `FinQuant-0.3.0/tests/test_Example-Optimisation.py` & `FinQuant-0.3.1/tests/test_Example-Optimisation.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-# -*- coding: utf-8 -*-
-# <nbformat>4</nbformat>
-
-# <markdowncell>
-
-# # Example: Portfolio optimisation
-# This example shows how `FinQuant` can be used to optimise a portfolio.
-# Two different approaches are implemented in `FinQuant`:
-#  1. Efficient Frontier
-#  2. Monte Carlo run
-# With the *Efficient Frontier* approach, the portfolio can be optimised for
-#  - minimum volatility,
-#  - maximum Sharpe ratio
-#  - minimum volatility for a given expected return
-#  - maximum Sharpe ratio for a given target volatility
-# by performing a numerical solve to minimise/maximise an objective function.
-# Alternatively a *Monte Carlo* run of `n` trials can be performed to find the optimal portfolios for
-#  - minimum volatility,
-#  - maximum Sharpe ratio
-# The approach branded as *Efficient Frontier* should be the preferred method for reasons of computational effort and accuracy. The latter approach is only included for the sake of completeness, and creation of beautiful plots.
-#
-# ## Visualisation
-# Not only does `FinQuant` allow for the optimisation of a portfolio with the above mentioned methods and objectives, `FinQuant` also allows for the computation and visualisation of an *Efficient Frontier* and *Monte Carlo* run.
-# Let `pf` be an instance of `Portfolio`. The *Efficient Frontier* can be computed and visualised with `pf.ef_plot_efrontier()`. The optimal portfolios for *minimum volatility* and *maximum Sharpe ratio* can be visualised with `pf.ef_plot_optimal_portfolios()`. And if required, the individual stocks of the portfolio can be visualised with `pf.plot_stocks(show=False)`. An overlay of these three commands is shown below.
-# Finally, the entire result of a *Monte Carlo* run can also be visualised automatically by `FinQuant`. An example is shown below.
-
-# <codecell>
-
-import pathlib
-import matplotlib.pyplot as plt
-plt.switch_backend("Agg")
-import numpy as np
-import pandas as pd
-import datetime
-
-# importing FinQuant's function to automatically build the portfolio
-from finquant.portfolio import build_portfolio
-
-# <codecell>
-
-# plotting style:
-plt.style.use("seaborn-v0_8-darkgrid")
-# set line width
-plt.rcParams["lines.linewidth"] = 2
-# set font size for titles
-plt.rcParams["axes.titlesize"] = 14
-# set font size for labels on axes
-plt.rcParams["axes.labelsize"] = 12
-# set size of numbers on x-axis
-plt.rcParams["xtick.labelsize"] = 10
-# set size of numbers on y-axis
-plt.rcParams["ytick.labelsize"] = 10
-# set figure size
-plt.rcParams["figure.figsize"] = (10, 6)
-
-# <markdowncell>
-
-# ### Get data from disk/file
-# Here we use `pandas.read_cvs()` method to read in the data.
-
-# <codecell>
-
-# stock data was previously pulled from quandl and stored in ex1-stockdata.csv
-# read data from files:
-df_data_path = pathlib.Path.cwd() / ".." / "data" / "ex1-stockdata.csv"
-df_data = pd.read_csv(df_data_path, index_col="Date", parse_dates=True)
-# building a portfolio by providing stock data
-pf = build_portfolio(data=df_data)
-print(pf)
-pf.properties()
-
-# <markdowncell>
-
-# # Portfolio optimisation
-# ## Efficient Frontier
-# Based on the **Efficient Frontier**, the portfolio can be optimised for
-#  - minimum volatility
-#  - maximum Sharpe ratio
-#  - minimum volatility for a given target return
-#  - maximum Sharpe ratio for a given target volatility
-# See below for an example for each optimisation.
-
-# <codecell>
-
-# if needed, change risk free rate and frequency/time window of the portfolio
-print("pf.risk_free_rate = {}".format(pf.risk_free_rate))
-print("pf.freq = {}".format(pf.freq))
-
-# <codecell>
-
-pf.ef_minimum_volatility(verbose=True)
-
-# <codecell>
-
-# optimisation for maximum Sharpe ratio
-pf.ef_maximum_sharpe_ratio(verbose=True)
-
-# <codecell>
-
-# minimum volatility for a given target return of 0.26
-pf.ef_efficient_return(0.26, verbose=True)
-
-# <codecell>
-
-# maximum Sharpe ratio for a given target volatility of 0.22
-pf.ef_efficient_volatility(0.22, verbose=True)
-
-# <markdowncell>
-
-# ### Manually creating an instance of EfficientFrontier
-# If required, or preferred, the below code shows how the same is achieved by manually creating an instance of EfficientFrontier, passing it the mean returns and covariance matrix of the previously assembled portfolio.
-
-# <codecell>
-
-from finquant.efficient_frontier import EfficientFrontier
-
-# creating an instance of EfficientFrontier
-ef = EfficientFrontier(pf.comp_mean_returns(freq=1), pf.comp_cov())
-# optimisation for minimum volatility
-print(ef.minimum_volatility())
-
-# <codecell>
-
-# printing out relevant quantities of the optimised portfolio
-(expected_return, volatility, sharpe) = ef.properties(verbose=True)
-
-# <markdowncell>
-
-# ### Computing and visualising the Efficient Frontier
-# `FinQuant` offers several ways to compute the *Efficient Frontier*.
-#  1. Through the opject `pf`
-#   - with automatically setting limits of the *Efficient Frontier*
-#  2. By manually creating an instance of `EfficientFrontier` and providing the data from the portfolio
-#   - with automatically setting limits of the *Efficient Frontier*
-#   - by providing a range of target expected return values
-# As before, let `pf` and be an instance of `Portfolio`. The following code snippets compute and plot an *Efficient Frontier* of a portfolio, its optimised portfolios and individual stocks within the portfolio.
-#  - `pf.ef_plot_efrontier()`
-#  - `pf.ef_plot_optimal_portfolios()`
-#  - `pf.plot_stocks()`
-
-# <markdowncell>
-
-# #### Efficient Frontier of `pf`
-
-# <codecell>
-
-# computing and plotting efficient frontier of pf
-pf.ef_plot_efrontier()
-# adding markers to optimal solutions
-pf.ef_plot_optimal_portfolios()
-# and adding the individual stocks to the plot
-pf.plot_stocks()
-
-
-# <markdowncell>
-
-# #### Manually creating an Efficient Frontier with target return values
-
-# <codecell>
-
-targets = np.linspace(0.12, 0.45, 50)
-# computing efficient frontier
-efficient_frontier = ef.efficient_frontier(targets)
-# plotting efficient frontier
-ef.plot_efrontier()
-# adding markers to optimal solutions
-pf.ef.plot_optimal_portfolios()
-# and adding the individual stocks to the plot
-pf.plot_stocks()
-
-
-# <markdowncell>
-
-# ## Monte Carlo
-# Perform a Monte Carlo run to find the portfolio with the minimum volatility and maximum Sharpe Ratio.
-
-# <codecell>
-
-opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
-pf.mc_properties()
-pf.mc_plot_results()
-# again, the individual stocks can be added to the plot
-pf.plot_stocks()
-
-
-# <codecell>
-
-print(opt_res)
-print()
-print(opt_w)
-
-# <markdowncell>
-
-# # Optimisation overlay
-# ## Overlay of Monte Carlo portfolios and Efficient Frontier solutions
-
-# <codecell>
-
-opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
-pf.mc_plot_results()
-pf.ef_plot_efrontier()
-pf.ef.plot_optimal_portfolios()
-pf.plot_stocks()
-
+# -*- coding: utf-8 -*-
+# <nbformat>4</nbformat>
+
+# <markdowncell>
+
+# # Example: Portfolio optimisation
+# This example shows how `FinQuant` can be used to optimise a portfolio.
+# Two different approaches are implemented in `FinQuant`:
+#  1. Efficient Frontier
+#  2. Monte Carlo run
+# With the *Efficient Frontier* approach, the portfolio can be optimised for
+#  - minimum volatility,
+#  - maximum Sharpe ratio
+#  - minimum volatility for a given expected return
+#  - maximum Sharpe ratio for a given target volatility
+# by performing a numerical solve to minimise/maximise an objective function.
+# Alternatively a *Monte Carlo* run of `n` trials can be performed to find the optimal portfolios for
+#  - minimum volatility,
+#  - maximum Sharpe ratio
+# The approach branded as *Efficient Frontier* should be the preferred method for reasons of computational effort and accuracy. The latter approach is only included for the sake of completeness, and creation of beautiful plots.
+#
+# ## Visualisation
+# Not only does `FinQuant` allow for the optimisation of a portfolio with the above mentioned methods and objectives, `FinQuant` also allows for the computation and visualisation of an *Efficient Frontier* and *Monte Carlo* run.
+# Let `pf` be an instance of `Portfolio`. The *Efficient Frontier* can be computed and visualised with `pf.ef_plot_efrontier()`. The optimal portfolios for *minimum volatility* and *maximum Sharpe ratio* can be visualised with `pf.ef_plot_optimal_portfolios()`. And if required, the individual stocks of the portfolio can be visualised with `pf.plot_stocks(show=False)`. An overlay of these three commands is shown below.
+# Finally, the entire result of a *Monte Carlo* run can also be visualised automatically by `FinQuant`. An example is shown below.
+
+# <codecell>
+
+import pathlib
+import matplotlib.pyplot as plt
+plt.switch_backend("Agg")
+import numpy as np
+import pandas as pd
+import datetime
+
+# importing FinQuant's function to automatically build the portfolio
+from finquant.portfolio import build_portfolio
+
+# <codecell>
+
+# plotting style:
+plt.style.use("seaborn-v0_8-darkgrid")
+# set line width
+plt.rcParams["lines.linewidth"] = 2
+# set font size for titles
+plt.rcParams["axes.titlesize"] = 14
+# set font size for labels on axes
+plt.rcParams["axes.labelsize"] = 12
+# set size of numbers on x-axis
+plt.rcParams["xtick.labelsize"] = 10
+# set size of numbers on y-axis
+plt.rcParams["ytick.labelsize"] = 10
+# set figure size
+plt.rcParams["figure.figsize"] = (10, 6)
+
+# <markdowncell>
+
+# ### Get data from disk/file
+# Here we use `pandas.read_cvs()` method to read in the data.
+
+# <codecell>
+
+# stock data was previously pulled from quandl and stored in ex1-stockdata.csv
+# read data from files:
+df_data_path = pathlib.Path.cwd() / ".." / "data" / "ex1-stockdata.csv"
+df_data = pd.read_csv(df_data_path, index_col="Date", parse_dates=True)
+# building a portfolio by providing stock data
+pf = build_portfolio(data=df_data)
+print(pf)
+pf.properties()
+
+# <markdowncell>
+
+# # Portfolio optimisation
+# ## Efficient Frontier
+# Based on the **Efficient Frontier**, the portfolio can be optimised for
+#  - minimum volatility
+#  - maximum Sharpe ratio
+#  - minimum volatility for a given target return
+#  - maximum Sharpe ratio for a given target volatility
+# See below for an example for each optimisation.
+
+# <codecell>
+
+# if needed, change risk free rate and frequency/time window of the portfolio
+print("pf.risk_free_rate = {}".format(pf.risk_free_rate))
+print("pf.freq = {}".format(pf.freq))
+
+# <codecell>
+
+pf.ef_minimum_volatility(verbose=True)
+
+# <codecell>
+
+# optimisation for maximum Sharpe ratio
+pf.ef_maximum_sharpe_ratio(verbose=True)
+
+# <codecell>
+
+# minimum volatility for a given target return of 0.26
+pf.ef_efficient_return(0.26, verbose=True)
+
+# <codecell>
+
+# maximum Sharpe ratio for a given target volatility of 0.22
+pf.ef_efficient_volatility(0.22, verbose=True)
+
+# <markdowncell>
+
+# ### Manually creating an instance of EfficientFrontier
+# If required, or preferred, the below code shows how the same is achieved by manually creating an instance of EfficientFrontier, passing it the mean returns and covariance matrix of the previously assembled portfolio.
+
+# <codecell>
+
+from finquant.efficient_frontier import EfficientFrontier
+
+# creating an instance of EfficientFrontier
+ef = EfficientFrontier(pf.comp_mean_returns(freq=1), pf.comp_cov())
+# optimisation for minimum volatility
+print(ef.minimum_volatility())
+
+# <codecell>
+
+# printing out relevant quantities of the optimised portfolio
+(expected_return, volatility, sharpe) = ef.properties(verbose=True)
+
+# <markdowncell>
+
+# ### Computing and visualising the Efficient Frontier
+# `FinQuant` offers several ways to compute the *Efficient Frontier*.
+#  1. Through the opject `pf`
+#   - with automatically setting limits of the *Efficient Frontier*
+#  2. By manually creating an instance of `EfficientFrontier` and providing the data from the portfolio
+#   - with automatically setting limits of the *Efficient Frontier*
+#   - by providing a range of target expected return values
+# As before, let `pf` and be an instance of `Portfolio`. The following code snippets compute and plot an *Efficient Frontier* of a portfolio, its optimised portfolios and individual stocks within the portfolio.
+#  - `pf.ef_plot_efrontier()`
+#  - `pf.ef_plot_optimal_portfolios()`
+#  - `pf.plot_stocks()`
+
+# <markdowncell>
+
+# #### Efficient Frontier of `pf`
+
+# <codecell>
+
+# computing and plotting efficient frontier of pf
+pf.ef_plot_efrontier()
+# adding markers to optimal solutions
+pf.ef_plot_optimal_portfolios()
+# and adding the individual stocks to the plot
+pf.plot_stocks()
+
+
+# <markdowncell>
+
+# #### Manually creating an Efficient Frontier with target return values
+
+# <codecell>
+
+targets = np.linspace(0.12, 0.45, 50)
+# computing efficient frontier
+efficient_frontier = ef.efficient_frontier(targets)
+# plotting efficient frontier
+ef.plot_efrontier()
+# adding markers to optimal solutions
+pf.ef.plot_optimal_portfolios()
+# and adding the individual stocks to the plot
+pf.plot_stocks()
+
+
+# <markdowncell>
+
+# ## Monte Carlo
+# Perform a Monte Carlo run to find the portfolio with the minimum volatility and maximum Sharpe Ratio.
+
+# <codecell>
+
+opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
+pf.mc_properties()
+pf.mc_plot_results()
+# again, the individual stocks can be added to the plot
+pf.plot_stocks()
+
+
+# <codecell>
+
+print(opt_res)
+print()
+print(opt_w)
+
+# <markdowncell>
+
+# # Optimisation overlay
+# ## Overlay of Monte Carlo portfolios and Efficient Frontier solutions
+
+# <codecell>
+
+opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
+pf.mc_plot_results()
+pf.ef_plot_efrontier()
+pf.ef.plot_optimal_portfolios()
+pf.plot_stocks()
+
```

### Comparing `FinQuant-0.3.0/tests/test_market.py` & `FinQuant-0.3.1/tests/test_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ###################
 # tests for Market #
 ###################
 
 import numpy as np
 import pandas as pd
-import yfinance
 import pytest
-from finquant.portfolio import build_portfolio
+import yfinance
+
 from finquant.market import Market
+from finquant.portfolio import build_portfolio
 
 d = {
     0: {"Name": "GOOG", "Allocation": 20},
     1: {"Name": "AMZN", "Allocation": 10},
     2: {"Name": "MCD", "Allocation": 15},
     3: {"Name": "DIS", "Allocation": 18},
     4: {"Name": "TSLA", "Allocation": 48},
```

### Comparing `FinQuant-0.3.0/tests/test_moving_average.py` & `FinQuant-0.3.1/tests/test_moving_average.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-from finquant.moving_average import compute_ma, sma, ema, sma_std, ema_std
-from finquant.moving_average import plot_bollinger_band
+
+from finquant.moving_average import (
+    compute_ma,
+    ema,
+    ema_std,
+    plot_bollinger_band,
+    sma,
+    sma_std,
+)
 
 plt.switch_backend("Agg")
 
 
 def test_sma():
     orig = np.array(
         [
```

### Comparing `FinQuant-0.3.0/tests/test_portfolio.py` & `FinQuant-0.3.1/tests/test_portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 ###############################################################
 # testing modules portfolio, optimisation, efficient_frontier #
 # all through the interfaces in Portfolio                     #
 ###############################################################
+import datetime
 import os
 import pathlib
+
+import matplotlib.pylab as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pylab as plt
-import datetime
+import pytest
 import quandl
 import yfinance
-import pytest
-from finquant.portfolio import build_portfolio, Portfolio
-from finquant.stock import Stock
+
 from finquant.efficient_frontier import EfficientFrontier
+from finquant.portfolio import Portfolio, build_portfolio
+from finquant.stock import Stock
 
 # comparisons
 strong_abse = 1e-15
 weak_abse = 1e-8
 
 # setting quandl api key
 quandl.ApiConfig.api_key = os.getenv("QUANDLAPIKEY")
```

### Comparing `FinQuant-0.3.0/tests/test_quants.py` & `FinQuant-0.3.1/tests/test_quants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import numpy as np
-from finquant.quants import weighted_mean, weighted_std
-from finquant.quants import sharpe_ratio, annualised_portfolio_quantities
+
+from finquant.quants import (
+    annualised_portfolio_quantities,
+    sharpe_ratio,
+    weighted_mean,
+    weighted_std,
+)
 
 
 def test_weighted_mean():
     means = np.array([1])
     weights = np.array([1])
     assert weighted_mean(means, weights) == 1
     means = np.array(range(5))
```

### Comparing `FinQuant-0.3.0/tests/test_returns.py` & `FinQuant-0.3.1/tests/test_returns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import pandas as pd
-from finquant.returns import cumulative_returns, daily_returns
-from finquant.returns import daily_log_returns, historical_mean_return
+
+from finquant.returns import (
+    cumulative_returns,
+    daily_log_returns,
+    daily_returns,
+    historical_mean_return,
+)
 
 
 def test_cumulative_returns():
     orig = [
         list(range(10)),
         [0, -0.025, -0.05, -0.075, -0.1, -0.125, -0.15, -0.175, -0.2, -0.225],
     ]
```

### Comparing `FinQuant-0.3.0/tests/test_stock.py` & `FinQuant-0.3.1/tests/test_stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 ###################
 # tests for Stock #
 ###################
 
+import datetime
 import os
 import pathlib
+
 import numpy as np
 import pandas as pd
-import datetime
+import pytest
 import quandl
 import yfinance
-import pytest
+
 from finquant.portfolio import build_portfolio
 from finquant.stock import Stock
 
 # comparisons
 strong_abse = 1e-15
 weak_abse = 1e-8
```

