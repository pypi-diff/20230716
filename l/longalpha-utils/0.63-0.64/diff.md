# Comparing `tmp/longalpha_utils-0.63.tar.gz` & `tmp/longalpha_utils-0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.63.tar", last modified: Sun Jul 16 16:24:04 2023, max compression
+gzip compressed data, was "longalpha_utils-0.64.tar", last modified: Sun Jul 16 16:42:56 2023, max compression
```

## Comparing `longalpha_utils-0.63.tar` & `longalpha_utils-0.64.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:24:04.429872 longalpha_utils-0.63/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 16:24:04.429872 longalpha_utils-0.63/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:24:04.429872 longalpha_utils-0.63/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:24:04.429872 longalpha_utils-0.63/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:24:04.429872 longalpha_utils-0.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-16 16:23:53.000000 longalpha_utils-0.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:56.812733 longalpha_utils-0.64/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 16:42:56.808733 longalpha_utils-0.64/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:56.808733 longalpha_utils-0.64/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 16:42:43.000000 longalpha_utils-0.64/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 16:42:43.000000 longalpha_utils-0.64/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-16 16:42:43.000000 longalpha_utils-0.64/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-07-16 16:42:43.000000 longalpha_utils-0.64/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-16 16:42:43.000000 longalpha_utils-0.64/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-16 16:42:43.000000 longalpha_utils-0.64/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:42:56.808733 longalpha_utils-0.64/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 16:42:56.000000 longalpha_utils-0.64/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-16 16:42:56.000000 longalpha_utils-0.64/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:42:56.000000 longalpha_utils-0.64/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-16 16:42:56.000000 longalpha_utils-0.64/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 16:42:56.000000 longalpha_utils-0.64/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:42:56.812733 longalpha_utils-0.64/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-16 16:42:43.000000 longalpha_utils-0.64/setup.py
```

### Comparing `longalpha_utils-0.63/longalpha_utils/messenger.py` & `longalpha_utils-0.64/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.63/longalpha_utils/transfers.py` & `longalpha_utils-0.64/longalpha_utils/transfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from minio import Minio
 from minio.error import S3Error
 from pyspark.conf import SparkConf
 from pyspark.sql import SparkSession, DataFrame
 from pyspark.sql.utils import AnalysisException
 from tqdm import tqdm
 
-from longalpha_utils.utils import multi_union_by_name, get_s3_path
+from longalpha_utils.utils import multi_union_by_name, get_s3_path, get_features_objectname
 
 
 def init_spark(
     spark_executor_memory: str = "30g",
     spark_driver_memory: str = "90g",
     s3_endpoint: Optional[str] = None,
     s3_access_key: Optional[str] = None,
@@ -428,15 +428,15 @@
                 pass
 
     @staticmethod
     def get_pandas_data_one_day(
         mw: MinioWrapper, s3_bucket, s3_prefix, day: date, show_missing_date: bool = True
     ) -> Union[DataFrame, None]:
         try:
-            object_name = os.path.join(s3_prefix, f"{day}.pkl")
+            object_name = get_features_objectname(s3_prefix, day, "pkl")
             df = mw.get(bucket_name=s3_bucket, object_name=object_name, from_pickle=True)
             return df
         except minio.error.S3Error:
             if show_missing_date:
                 print(f"Data for {day} does not exist.")
             else:
                 pass
```

### Comparing `longalpha_utils-0.63/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.64/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.63/longalpha_utils/utils.py` & `longalpha_utils-0.64/longalpha_utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
-from typing import List, Optional
 from datetime import date, timedelta
 import os
 import pandas as pd
 from pyspark.sql import DataFrame
-
+from typing import List, Optional, Union
 
 def max_pandas_display(pd: pd, max_row: int = 100) -> None:
     """
     set pandas print format to print all
     Args:
         pd: pandas object
 
@@ -66,9 +65,10 @@
     dates = []
     while star_date <= end_date:
         dates.append(star_date)
         star_date += timedelta(days=1)
     return dates
 
 
-def get_features_objectname(s3_prefix: str, day:pd.Timestamp, file_type = "pkl") -> str:
-    return os.path.join(s3_prefix, str(day.year) , f"{day.date()}.{file_type}")
+def get_features_objectname(s3_prefix: str, day: Union[pd.Timestamp, date], file_type = "pkl") -> str:
+    ymd = str(day.date()) if isinstance(day, pd.Timestamp) else str(day)
+    return os.path.join(s3_prefix, str(day.year) , f"{ymd}.{file_type}")
```

### Comparing `longalpha_utils-0.63/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.64/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.63/setup.py` & `longalpha_utils-0.64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.63",
+    version="0.64",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

