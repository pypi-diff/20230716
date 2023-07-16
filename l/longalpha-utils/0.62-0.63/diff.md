# Comparing `tmp/longalpha_utils-0.62.tar.gz` & `tmp/longalpha_utils-0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.62.tar", last modified: Sat Jul 15 15:22:05 2023, max compression
+gzip compressed data, was "longalpha_utils-0.63.tar", last modified: Sun Jul 16 16:24:04 2023, max compression
```

## Comparing `longalpha_utils-0.62.tar` & `longalpha_utils-0.63.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:22:05.362236 longalpha_utils-0.62/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 15:22:05.362236 longalpha_utils-0.62/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:22:05.358236 longalpha_utils-0.62/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:22:05.362236 longalpha_utils-0.62/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:22:05.362236 longalpha_utils-0.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-15 15:21:54.000000 longalpha_utils-0.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:24:04.429872 longalpha_utils-0.63/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 16:24:04.429872 longalpha_utils-0.63/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:24:04.429872 longalpha_utils-0.63/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-16 16:23:53.000000 longalpha_utils-0.63/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:24:04.429872 longalpha_utils-0.63/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 16:24:04.000000 longalpha_utils-0.63/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:24:04.429872 longalpha_utils-0.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-16 16:23:53.000000 longalpha_utils-0.63/setup.py
```

### Comparing `longalpha_utils-0.62/longalpha_utils/messenger.py` & `longalpha_utils-0.63/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.62/longalpha_utils/transfers.py` & `longalpha_utils-0.63/longalpha_utils/transfers.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.62/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.63/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.62/longalpha_utils/utils.py` & `longalpha_utils-0.63/longalpha_utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,8 +63,12 @@
         return f"s3a://" + os.path.join(bucket, prefix)
 
 def get_date_range(star_date: date, end_date: date) -> List[date]:
     dates = []
     while star_date <= end_date:
         dates.append(star_date)
         star_date += timedelta(days=1)
-    return dates
+    return dates
+
+
+def get_features_objectname(s3_prefix: str, day:pd.Timestamp, file_type = "pkl") -> str:
+    return os.path.join(s3_prefix, str(day.year) , f"{day.date()}.{file_type}")
```

### Comparing `longalpha_utils-0.62/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.63/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.62/setup.py` & `longalpha_utils-0.63/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.62",
+    version="0.63",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

