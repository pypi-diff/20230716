# Comparing `tmp/mad8-pandas-1.1.0.tar.gz` & `tmp/mad8-pandas-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mad8-pandas-1.1.0.tar", last modified: Sun Jul 16 13:06:15 2023, max compression
+gzip compressed data, was "mad8-pandas-1.1.1.tar", last modified: Sun Jul 16 13:12:32 2023, max compression
```

## Comparing `mad8-pandas-1.1.0.tar` & `mad8-pandas-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 stuartwalker   (502) staff       (20)        0 2023-07-16 13:06:15.837801 mad8-pandas-1.1.0/
--rw-r--r--   0 stuartwalker   (502) staff       (20)     1799 2021-04-15 11:46:39.000000 mad8-pandas-1.1.0/.gitignore
--rw-r--r--   0 stuartwalker   (502) staff       (20)     1077 2022-04-12 18:55:32.000000 mad8-pandas-1.1.0/LICENSE
--rw-r--r--   0 stuartwalker   (502) staff       (20)     1591 2023-07-16 13:06:15.837627 mad8-pandas-1.1.0/PKG-INFO
--rw-r--r--   0 stuartwalker   (502) staff       (20)      579 2023-07-16 13:05:43.000000 mad8-pandas-1.1.0/README.md
-drwxr-xr-x   0 stuartwalker   (502) staff       (20)        0 2023-07-16 13:06:15.835472 mad8-pandas-1.1.0/mad8_pandas.egg-info/
--rw-r--r--   0 stuartwalker   (502) staff       (20)     1591 2023-07-16 13:06:15.000000 mad8-pandas-1.1.0/mad8_pandas.egg-info/PKG-INFO
--rw-r--r--   0 stuartwalker   (502) staff       (20)      262 2023-07-16 13:06:15.000000 mad8-pandas-1.1.0/mad8_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 stuartwalker   (502) staff       (20)        1 2023-07-16 13:06:15.000000 mad8-pandas-1.1.0/mad8_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 stuartwalker   (502) staff       (20)       27 2023-07-16 13:06:15.000000 mad8-pandas-1.1.0/mad8_pandas.egg-info/requires.txt
--rw-r--r--   0 stuartwalker   (502) staff       (20)        6 2023-07-16 13:06:15.000000 mad8-pandas-1.1.0/mad8_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 stuartwalker   (502) staff       (20)        0 2023-07-16 13:06:15.837393 mad8-pandas-1.1.0/pand8/
--rw-r--r--   0 stuartwalker   (502) staff       (20)      132 2023-07-16 12:58:36.000000 mad8-pandas-1.1.0/pand8/__init__.py
--rw-r--r--   0 stuartwalker   (502) staff       (20)     1591 2023-07-16 12:35:34.000000 mad8-pandas-1.1.0/pand8/extras.py
--rw-r--r--   0 stuartwalker   (502) staff       (20)    11479 2023-07-16 13:04:32.000000 mad8-pandas-1.1.0/pand8/handler.py
--rw-r--r--   0 stuartwalker   (502) staff       (20)       38 2023-07-16 13:06:15.837849 mad8-pandas-1.1.0/setup.cfg
--rw-r--r--   0 stuartwalker   (502) staff       (20)     1361 2023-07-16 13:04:46.000000 mad8-pandas-1.1.0/setup.py
+drwxr-xr-x   0 stuartwalker   (502) staff       (20)        0 2023-07-16 13:12:32.568060 mad8-pandas-1.1.1/
+-rw-r--r--   0 stuartwalker   (502) staff       (20)     1799 2021-04-15 11:46:39.000000 mad8-pandas-1.1.1/.gitignore
+-rw-r--r--   0 stuartwalker   (502) staff       (20)     1077 2022-04-12 18:55:32.000000 mad8-pandas-1.1.1/LICENSE
+-rw-r--r--   0 stuartwalker   (502) staff       (20)     1591 2023-07-16 13:12:32.567736 mad8-pandas-1.1.1/PKG-INFO
+-rw-r--r--   0 stuartwalker   (502) staff       (20)      579 2023-07-16 13:05:43.000000 mad8-pandas-1.1.1/README.md
+drwxr-xr-x   0 stuartwalker   (502) staff       (20)        0 2023-07-16 13:12:32.566270 mad8-pandas-1.1.1/mad8_pandas.egg-info/
+-rw-r--r--   0 stuartwalker   (502) staff       (20)     1591 2023-07-16 13:12:32.000000 mad8-pandas-1.1.1/mad8_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 stuartwalker   (502) staff       (20)      262 2023-07-16 13:12:32.000000 mad8-pandas-1.1.1/mad8_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 stuartwalker   (502) staff       (20)        1 2023-07-16 13:12:32.000000 mad8-pandas-1.1.1/mad8_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 stuartwalker   (502) staff       (20)       27 2023-07-16 13:12:32.000000 mad8-pandas-1.1.1/mad8_pandas.egg-info/requires.txt
+-rw-r--r--   0 stuartwalker   (502) staff       (20)        6 2023-07-16 13:12:32.000000 mad8-pandas-1.1.1/mad8_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 stuartwalker   (502) staff       (20)        0 2023-07-16 13:12:32.567365 mad8-pandas-1.1.1/pand8/
+-rw-r--r--   0 stuartwalker   (502) staff       (20)      132 2023-07-16 12:58:36.000000 mad8-pandas-1.1.1/pand8/__init__.py
+-rw-r--r--   0 stuartwalker   (502) staff       (20)     1591 2023-07-16 12:35:34.000000 mad8-pandas-1.1.1/pand8/extras.py
+-rw-r--r--   0 stuartwalker   (502) staff       (20)    11486 2023-07-16 13:10:24.000000 mad8-pandas-1.1.1/pand8/handler.py
+-rw-r--r--   0 stuartwalker   (502) staff       (20)       38 2023-07-16 13:12:32.568229 mad8-pandas-1.1.1/setup.cfg
+-rw-r--r--   0 stuartwalker   (502) staff       (20)     1361 2023-07-16 13:11:40.000000 mad8-pandas-1.1.1/setup.py
```

### Comparing `mad8-pandas-1.1.0/.gitignore` & `mad8-pandas-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mad8-pandas-1.1.0/LICENSE` & `mad8-pandas-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mad8-pandas-1.1.0/PKG-INFO` & `mad8-pandas-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad8-pandas
-Version: 1.1.0
+Version: 1.1.1
 Summary: load mad8 output with pandas
 Home-page: https://github.com/st-walker/mad8-pandas
 Author: Stuart Walker
 Author-email: stuart.derek.walker@gmail.com
 License: MIT
 Keywords: mad8 pandas twiss
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mad8-pandas-1.1.0/README.md` & `mad8-pandas-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mad8-pandas-1.1.0/mad8_pandas.egg-info/PKG-INFO` & `mad8-pandas-1.1.1/mad8_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad8-pandas
-Version: 1.1.0
+Version: 1.1.1
 Summary: load mad8 output with pandas
 Home-page: https://github.com/st-walker/mad8-pandas
 Author: Stuart Walker
 Author-email: stuart.derek.walker@gmail.com
 License: MIT
 Keywords: mad8 pandas twiss
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mad8-pandas-1.1.0/pand8/extras.py` & `mad8-pandas-1.1.1/pand8/extras.py`

 * *Files identical despite different names*

### Comparing `mad8-pandas-1.1.0/pand8/handler.py` & `mad8-pandas-1.1.1/pand8/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import os
 import contextlib
-from typing import Optional, Union
+from typing import Optional, Any
 
 import pandas as pd
 import fortranformat as ff
 
 COMMON_COLUMNS: list[str] = [
     "KEYWORD",
     "NAME",
@@ -35,15 +36,15 @@
     "TILT",
     "VKICK",
     "VOLT",
     "XSIZE",
     "YSIZE",
 ]
 
-SURVEY_COLUMNS: str  = ["X", "Y", "Z", "SUML", "THETA", "PHI", "PSI"]
+SURVEY_COLUMNS: str = ["X", "Y", "Z", "SUML", "THETA", "PHI", "PSI"]
 
 
 COMMON_COLUMN_POSITIONS: dict[str, dict[str, int]] = {
     "DRIF": {"L": 0, "APER": 9, "NOTE": 10, "E": 11},
     "RBEN": {
         "L": 0,
         "ANGLE": 1,
```

### Comparing `mad8-pandas-1.1.0/setup.py` & `mad8-pandas-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="mad8-pandas",
-    version="1.1.0",
+    version="1.1.1",
     description="load mad8 output with pandas",
     packages=find_packages(include=["pand8"]),
     install_requires=["pandas", "fortranformat", "numpy"],
     url="https://github.com/st-walker/mad8-pandas",
     license="MIT",
     keywords="mad8 pandas twiss",
     author="Stuart Walker",
```

