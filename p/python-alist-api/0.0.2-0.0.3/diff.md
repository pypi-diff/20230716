# Comparing `tmp/python-alist-api-0.0.2.tar.gz` & `tmp/python-alist-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-alist-api-0.0.2.tar", last modified: Sun Jul  9 09:06:05 2023, max compression
+gzip compressed data, was "python-alist-api-0.0.3.tar", last modified: Sun Jul 16 09:45:28 2023, max compression
```

## Comparing `python-alist-api-0.0.2.tar` & `python-alist-api-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/alist/
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/public.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/python_alist_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/alist/
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/python_alist_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/setup.cfg
```

### Comparing `python-alist-api-0.0.2/LICENSE` & `python-alist-api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.2/PKG-INFO` & `python-alist-api-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alist-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper for the Alist API
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
```

### Comparing `python-alist-api-0.0.2/README.md` & `python-alist-api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.2/alist/__init__.py` & `python-alist-api-0.0.3/alist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Kai Peng
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from requests import Session
 from requests import HTTPError
 import json
 from urllib.parse import urlparse
 from alist.public import AlistPublic
 from alist.admin import AlistAdmin
```

### Comparing `python-alist-api-0.0.2/alist/admin.py` & `python-alist-api-0.0.3/alist/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,33 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Kai Peng
 
 from alist.setting import AlistAaminSettings
+from alist.driver import AlistAdminDrivers
+from alist.account import AlistAdminAccount, AlistAdminAccounts
 
 class AlistAdmin(object):
     def __init__(self, alist):
         self.alist = alist
         self.endpoint = '/admin'
         self.settings = AlistAaminSettings(alist, self.endpoint)
+        self.drivers  = AlistAdminDrivers(alist, self.endpoint)
+        self.account  = AlistAdminAccount(alist, self.endpoint)
+        self.accounts = AlistAdminAccounts(alist, self.endpoint)
 
     def login(self):
         """ 登录
         :returns:
             登录成功返回Ture，登录失败触发异常。
         """
         endpoint = f'{self.endpoint}/login'
         # if login fail, will raise exception
         return self.alist.get(endpoint)
 
-    def accounts(self):
-        """ 获取账号列表。
-        :returns:
-            账号列表。
-        """
-        endpoint = f'{self.endpoint}/accounts'
-        return self.alist.get(endpoint)
-
-    def account_create(self):
-        pass
-
-    def account_save(self):
-        pass
-
-    def account_delete(self):
-        pass
-
-
-    def drivers(self):
-        """ 获取dricer列表，包含driver需要配置的字段列表
-        :returns:
-            driver列表
-        """
-        endpoint = f'{self.endpoint}/drivers'
-        return self.alist.get(endpoint)
-
     def clear_cache(self):
         """ 清理所有的缓存数据。
         :returns:
             清理成功返回True，清理失败触发异常。
         """
         endpoint = f'{self.endpoint}/clear_cache'
         return self.alist.get(endpoint)
```

### Comparing `python-alist-api-0.0.2/alist/public.py` & `python-alist-api-0.0.3/alist/public.py`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.2/alist/setting.py` & `python-alist-api-0.0.3/alist/setting.py`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.2/pyproject.toml` & `python-alist-api-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.2/python_alist_api.egg-info/PKG-INFO` & `python-alist-api-0.0.3/python_alist_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alist-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper for the Alist API
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
```

