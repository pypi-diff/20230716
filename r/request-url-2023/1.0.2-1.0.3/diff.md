# Comparing `tmp/request_url_2023-1.0.2.tar.gz` & `tmp/request_url_2023-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\request_url_2023-1.0.2.tar", last modified: Fri Jul 14 11:39:46 2023, max compression
+gzip compressed data, was "dist\request_url_2023-1.0.3.tar", last modified: Sun Jul 16 02:47:36 2023, max compression
```

## Comparing `request_url_2023-1.0.2.tar` & `request_url_2023-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/
--rw-rw-rw-   0        0        0     1089 2023-07-14 03:36:37.000000 request_url_2023-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1342 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-07-14 11:30:23.000000 request_url_2023-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/request_url_2023/
--rw-rw-rw-   0        0        0        0 2023-07-14 03:38:43.000000 request_url_2023-1.0.2/request_url_2023/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-07-14 11:12:33.000000 request_url_2023-1.0.2/request_url_2023/send_requests.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/request_url_2023.egg-info/
--rw-rw-rw-   0        0        0     1342 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/request_url_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/request_url_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/request_url_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/request_url_2023.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/request_url_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 11:39:46.000000 request_url_2023-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1188 2023-07-14 11:38:48.000000 request_url_2023-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-07-14 03:36:37.000000 request_url_2023-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1324 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-07-16 02:46:58.000000 request_url_2023-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/request_url_2023/
+-rw-rw-rw-   0        0        0        0 2023-07-14 03:38:43.000000 request_url_2023-1.0.3/request_url_2023/__init__.py
+-rw-rw-rw-   0        0        0     1885 2023-07-16 02:46:58.000000 request_url_2023-1.0.3/request_url_2023/send_requests.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/request_url_2023.egg-info/
+-rw-rw-rw-   0        0        0     1324 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/request_url_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/request_url_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/request_url_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/request_url_2023.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/request_url_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 02:47:36.000000 request_url_2023-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1188 2023-07-16 02:47:30.000000 request_url_2023-1.0.3/setup.py
```

### Comparing `request_url_2023-1.0.2/LICENSE` & `request_url_2023-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `request_url_2023-1.0.2/PKG-INFO` & `request_url_2023-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request_url_2023
-Version: 1.0.2
+Version: 1.0.3
 Summary: send bulk requests to a url
 Home-page: https://www.linkedin.com/in/chandlersong/
 Author: chandler song
 Author-email: 275737875@qq.com
 License: MIT
 Keywords: requests url
 Platform: all
@@ -25,29 +25,29 @@
 ```shell
 pip install request-url-2023
 ```
 ##  Example Usage:
 ```python
 from request_url_2023 import send_requests
 
-send_requests.run(url="https://www.hrtechchina.com/")
+send_requests.run(url="https://www.baidu.com/")
 ```
 
 ## Params
 
 ```python
 from request_url_2023 import send_requests
 
 # 总的请求数
 # TOTAL_COUNT = 10000
-# 线程池数目，
+# 线程池数目
 # THREAD_NUM = 20
 # 每个协程同时发送多少个请求
 # COROUTINE_REQUEST_COUNT = 50
 
 send_requests.run(
-    url="https://www.hrtechchina.com/",
+    url="https://www.baidu.com/",
     TOTAL_COUNT = 1000,
     THREAD_NUM = 20,
-    COROUTINE_REQUEST_COUNT = 50)
-```
+    COROUTINE_REQUEST_COUNT = 50
+)
 ```
```

### Comparing `request_url_2023-1.0.2/README.md` & `request_url_2023-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 ```shell
 pip install request-url-2023
 ```
 ##  Example Usage:
 ```python
 from request_url_2023 import send_requests
 
-send_requests.run(url="https://www.hrtechchina.com/")
+send_requests.run(url="https://www.baidu.com/")
 ```
 
 ## Params
 
 ```python
 from request_url_2023 import send_requests
 
 # 总的请求数
 # TOTAL_COUNT = 10000
-# 线程池数目，
+# 线程池数目
 # THREAD_NUM = 20
 # 每个协程同时发送多少个请求
 # COROUTINE_REQUEST_COUNT = 50
 
 send_requests.run(
-    url="https://www.hrtechchina.com/",
+    url="https://www.baidu.com/",
     TOTAL_COUNT = 1000,
     THREAD_NUM = 20,
-    COROUTINE_REQUEST_COUNT = 50)
-```
+    COROUTINE_REQUEST_COUNT = 50
+)
 ```
```

### Comparing `request_url_2023-1.0.2/request_url_2023/send_requests.py` & `request_url_2023-1.0.3/request_url_2023/send_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import random
-import sys
-
 import aiohttp
 import asyncio
-from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 from fake_headers import Headers
 
-# pip install fake-headers
-# pip install aiohttp
-
-
 def generate_header_list():
     header_list_len = 100
     header = Headers(
         # generate any browser & os headeers
         headers=False  # don`t generate misc headers
     )
     header_list = []
@@ -44,30 +38,36 @@
     ]
 
     await asyncio.wait(tasks)
 
 def task(url,request_count):
     asyncio.run(engine(url,request_count))
 
-def run(url, TOTAL_COUNT = 1000,THREAD_NUM = 20,COROUTINE_REQUEST_COUNT = 50):
+
+def run(url, TOTAL_COUNT=1000, THREAD_NUM=20, COROUTINE_REQUEST_COUNT=50):
     # 总的请求数
     # TOTAL_COUNT = 10000
+
     # url
     # url = "https://www.baidu.com"
-    # 线程池数目，
+
+    # 线程池数目
     # THREAD_NUM = 20
+
     # 每个协程同时发送多少个请求
     # COROUTINE_REQUEST_COUNT = 50
+
     # 初始化线程池
     pool = ThreadPoolExecutor(THREAD_NUM)
+
     #  1000/20=50，5
     loop_count, div = divmod(TOTAL_COUNT, COROUTINE_REQUEST_COUNT)
+
     # 循环50次 * 20 = 1000个请求
     for i in range(loop_count):
-        # print(COROUTINE_REQUEST_COUNT)
         pool.submit(task, url, COROUTINE_REQUEST_COUNT)
 
     pool.submit(task, url, div)
     # 等待所有任务执行完毕
     pool.shutdown()
```

### Comparing `request_url_2023-1.0.2/request_url_2023.egg-info/PKG-INFO` & `request_url_2023-1.0.3/request_url_2023.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-url-2023
-Version: 1.0.2
+Version: 1.0.3
 Summary: send bulk requests to a url
 Home-page: https://www.linkedin.com/in/chandlersong/
 Author: chandler song
 Author-email: 275737875@qq.com
 License: MIT
 Keywords: requests url
 Platform: all
@@ -25,29 +25,29 @@
 ```shell
 pip install request-url-2023
 ```
 ##  Example Usage:
 ```python
 from request_url_2023 import send_requests
 
-send_requests.run(url="https://www.hrtechchina.com/")
+send_requests.run(url="https://www.baidu.com/")
 ```
 
 ## Params
 
 ```python
 from request_url_2023 import send_requests
 
 # 总的请求数
 # TOTAL_COUNT = 10000
-# 线程池数目，
+# 线程池数目
 # THREAD_NUM = 20
 # 每个协程同时发送多少个请求
 # COROUTINE_REQUEST_COUNT = 50
 
 send_requests.run(
-    url="https://www.hrtechchina.com/",
+    url="https://www.baidu.com/",
     TOTAL_COUNT = 1000,
     THREAD_NUM = 20,
-    COROUTINE_REQUEST_COUNT = 50)
-```
+    COROUTINE_REQUEST_COUNT = 50
+)
 ```
```

### Comparing `request_url_2023-1.0.2/setup.py` & `request_url_2023-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.md", "r",encoding='utf-8') as f:
   long_description = f.read()
 setup(name='request_url_2023',  # 包名
-      version='1.0.2',  # 版本号
+      version='1.0.3',  # 版本号
       description='send bulk requests to a url',
       long_description_content_type = 'text/markdown',
       long_description=long_description,
       author='chandler song',
       author_email='275737875@qq.com',
       url='https://www.linkedin.com/in/chandlersong/',
       keywords = "requests url",
```

