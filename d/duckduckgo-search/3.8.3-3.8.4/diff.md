# Comparing `tmp/duckduckgo_search-3.8.3.tar.gz` & `tmp/duckduckgo_search-3.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.8.3.tar", last modified: Fri Jun  9 13:20:52 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.8.4.tar", last modified: Sun Jul 16 00:15:34 2023, max compression
```

## Comparing `duckduckgo_search-3.8.3.tar` & `duckduckgo_search-3.8.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:34.381850 duckduckgo_search-3.8.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-16 00:15:34.381850 duckduckgo_search-3.8.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:34.377850 duckduckgo_search-3.8.4/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18751 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:34.381850 duckduckgo_search-3.8.4/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-16 00:15:34.000000 duckduckgo_search-3.8.4/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-16 00:15:34.000000 duckduckgo_search-3.8.4/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 00:15:34.000000 duckduckgo_search-3.8.4/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 00:15:34.000000 duckduckgo_search-3.8.4/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-16 00:15:34.000000 duckduckgo_search-3.8.4/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-16 00:15:34.000000 duckduckgo_search-3.8.4/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 00:15:34.381850 duckduckgo_search-3.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:34.381850 duckduckgo_search-3.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-16 00:15:14.000000 duckduckgo_search-3.8.4/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.8.3/LICENSE.md` & `duckduckgo_search-3.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.3/PKG-INFO` & `duckduckgo_search-3.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.8.3
+Version: 3.8.4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.8.3/README.md` & `duckduckgo_search-3.8.4/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.3/duckduckgo_search/__init__.py` & `duckduckgo_search-3.8.4/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.3/duckduckgo_search/cli.py` & `duckduckgo_search-3.8.4/duckduckgo_search/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,28 +97,27 @@
 
 
 async def download_file(url, dir_path, filename, sem, proxy):
     headers = {"User-Agent": choice(USERAGENTS)}
     for i in range(2):
         try:
             async with sem:
-                async with httpx.AsyncClient(headers=headers, proxies=proxy) as client:
+                async with httpx.AsyncClient(
+                    headers=headers, proxies=proxy, timeout=10
+                ) as client:
                     async with client.stream("GET", url) as resp:
-                        if resp.status_code == 200:
-                            async with aiofiles.open(
-                                os.path.join(dir_path, filename[:200]), "wb"
-                            ) as file:
-                                async for chunk in resp.aiter_bytes():
-                                    await file.write(chunk)
-                            break
+                        resp.raise_for_status()
+                        async with aiofiles.open(
+                            os.path.join(dir_path, filename[:200]), "wb"
+                        ) as file:
+                            async for chunk in resp.aiter_bytes():
+                                await file.write(chunk)
+                        break
         except (
-            httpx.ConnectTimeout,
-            httpx.ConnectError,
-            httpx.ProxyError,
-            httpx.ReadTimeout,
+            httpx.HTTPError,
             ssl.SSLCertVerificationError,
             ssl.SSLError,
         ) as ex:
             logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
         except ValueError as ex:
             raise ex
 
@@ -127,15 +126,15 @@
     if images:
         path = f"images_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     else:
         path = f"text_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     os.makedirs(path, exist_ok=True)
 
     tasks = []
-    threads = 20 if threads is None else threads
+    threads = 10 if threads is None else threads
     sem = asyncio.Semaphore(threads)
     for i, res in enumerate(results, start=1):
         if images:
             filename = unquote(res["image"].split("/")[-1].split("?")[0])
             task = asyncio.create_task(
                 download_file(res["image"], path, f"{i}_{filename}", sem, proxy)
             )
@@ -228,15 +227,15 @@
     "--threads",
     default=20,
     help="download threads, default=20",
 )
 @click.option(
     "-p",
     "--proxy",
-    help="proxy server for download, example: socks5://localhost:9150",
+    help="the proxy to send requests, example: socks5://localhost:9150",
 )
 def text(
     keywords,
     region,
     safesearch,
     timelimit,
     backend,
@@ -275,17 +274,22 @@
 )
 @click.option(
     "-o",
     "--output",
     default="print",
     help="csv, json (save the results to a csv or json file)",
 )
-def answers(keywords, output, *args, **kwargs):
+@click.option(
+    "-p",
+    "--proxy",
+    help="the proxy to send requests, example: socks5://localhost:9150",
+)
+def answers(keywords, output, proxy, *args, **kwargs):
     data = []
-    for r in DDGS().answers(keywords=keywords, *args, **kwargs):
+    for r in DDGS(proxies=proxy).answers(keywords=keywords, *args, **kwargs):
         data.append(r)
     filename = f"answers_{sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         print_data(data)
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
@@ -386,15 +390,15 @@
     "--threads",
     default=20,
     help="download threads, default=20",
 )
 @click.option(
     "-p",
     "--proxy",
-    help="proxy server for download, example: socks5://localhost:9150",
+    help="the proxy to send requests, example: socks5://localhost:9150",
 )
 def images(
     keywords,
     region,
     safesearch,
     timelimit,
     size,
@@ -480,17 +484,22 @@
 )
 @click.option(
     "-o",
     "--output",
     default="print",
     help="csv, json (save the results to a csv or json file)",
 )
-def videos(keywords, output, max_results, *args, **kwargs):
+@click.option(
+    "-p",
+    "--proxy",
+    help="the proxy to send requests, example: socks5://localhost:9150",
+)
+def videos(keywords, output, max_results, proxy, *args, **kwargs):
     data = []
-    for r in DDGS().videos(keywords=keywords, *args, **kwargs):
+    for r in DDGS(proxies=proxy).videos(keywords=keywords, *args, **kwargs):
         if len(data) >= max_results:
             break
         data.append(r)
     filename = f"videos_{sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         print_data(data)
     elif output == "csv":
@@ -529,17 +538,22 @@
 )
 @click.option(
     "-o",
     "--output",
     default="print",
     help="csv, json (save the results to a csv or json file)",
 )
-def news(keywords, output, max_results, *args, **kwargs):
+@click.option(
+    "-p",
+    "--proxy",
+    help="the proxy to send requests, example: socks5://localhost:9150",
+)
+def news(keywords, output, max_results, proxy, *args, **kwargs):
     data = []
-    for r in DDGS().news(keywords=keywords, *args, **kwargs):
+    for r in DDGS(proxies=proxy).news(keywords=keywords, *args, **kwargs):
         if len(data) >= max_results:
             break
         data.append(r)
     filename = f"news_{sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         print_data(data)
     elif output == "csv":
@@ -585,17 +599,24 @@
 @click.option("-m", "--max_results", default=50, help="number of results, default=50")
 @click.option(
     "-o",
     "--output",
     default="print",
     help="csv, json (save the results to a csv or json file)",
 )
-def maps(keywords, output, max_results, *args, **kwargs):
+@click.option(
+    "-proxy",
+    "--proxy",
+    help="the proxy to send requests, example: socks5://localhost:9150",
+)
+def maps(keywords, output, max_results, proxy, *args, **kwargs):
     data = []
-    for i, r in enumerate(DDGS().maps(keywords=keywords, *args, **kwargs), start=1):
+    for i, r in enumerate(
+        DDGS(proxies=proxy).maps(keywords=keywords, *args, **kwargs), start=1
+    ):
         if len(data) >= max_results:
             break
         data.append(r)
         if i % 100 == 0:
             print(i)
     filename = f"maps_{sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
@@ -621,16 +642,21 @@
 )
 @click.option(
     "-o",
     "--output",
     default="print",
     help="csv, json (save the results to a csv or json file)",
 )
-def translate(keywords, output, *args, **kwargs):
-    data = DDGS().translate(keywords=keywords, *args, **kwargs)
+@click.option(
+    "-p",
+    "--proxy",
+    help="the proxy to send requests, example: socks5://localhost:9150",
+)
+def translate(keywords, output, proxy, *args, **kwargs):
+    data = DDGS(proxies=proxy).translate(keywords=keywords, *args, **kwargs)
     data = [data]
     filename = f"translate_{sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         print_data(data)
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
@@ -647,17 +673,22 @@
 )
 @click.option(
     "-o",
     "--output",
     default="print",
     help="csv, json (save the results to a csv or json file)",
 )
-def suggestions(keywords, output, *args, **kwargs):
+@click.option(
+    "-p",
+    "--proxy",
+    help="the proxy to send requests, example: socks5://localhost:9150",
+)
+def suggestions(keywords, output, proxy, *args, **kwargs):
     data = []
-    for r in DDGS().suggestions(keywords=keywords, *args, **kwargs):
+    for r in DDGS(proxies=proxy).suggestions(keywords=keywords, *args, **kwargs):
         data.append(r)
     filename = (
         f"suggestions_{sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     )
     if output == "print":
         print_data(data)
     elif output == "csv":
```

### Comparing `duckduckgo_search-3.8.3/duckduckgo_search/compat.py` & `duckduckgo_search-3.8.4/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.3/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.8.4/duckduckgo_search/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.3/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.8.4/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.8.3
+Version: 3.8.4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.8.3/pyproject.toml` & `duckduckgo_search-3.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.3/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.8.4/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

