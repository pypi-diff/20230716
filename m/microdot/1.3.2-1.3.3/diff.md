# Comparing `tmp/microdot-1.3.2.tar.gz` & `tmp/microdot-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdot-1.3.2.tar", last modified: Tue Jun 13 13:45:09 2023, max compression
+gzip compressed data, was "microdot-1.3.3.tar", last modified: Sun Jul 16 10:41:02 2023, max compression
```

## Comparing `microdot-1.3.2.tar` & `microdot-1.3.3.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.783913 microdot-1.3.2/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2020-02-18 23:41:59.000000 microdot-1.3.2/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-06-13 13:45:09.784158 microdot-1.3.2/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      847 2022-08-07 14:45:44.000000 microdot-1.3.2/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-05 23:20:28.000000 microdot-1.3.2/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1035 2023-06-13 13:45:09.785465 microdot-1.3.2/setup.cfg
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-05 23:12:41.000000 microdot-1.3.2/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.759444 microdot-1.3.2/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.763285 microdot-1.3.2/src/microdot.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1018 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-06 10:08:26.000000 microdot-1.3.2/src/microdot.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)      248 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/top_level.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)    46254 2023-06-07 23:27:49.000000 microdot-1.3.2/src/microdot.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4952 2023-06-07 22:50:44.000000 microdot-1.3.2/src/microdot_asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2855 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_asgi_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    17370 2023-06-07 23:27:49.000000 microdot-1.3.2/src/microdot_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     7828 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_asyncio_test_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3780 2023-06-06 22:21:28.000000 microdot-1.3.2/src/microdot_asyncio_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1128 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_jinja.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2966 2023-06-06 22:20:32.000000 microdot-1.3.2/src/microdot_session.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10818 2023-06-06 22:21:28.000000 microdot-1.3.2/src/microdot_test_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1331 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_utemplate.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5935 2023-06-06 22:21:28.000000 microdot-1.3.2/src/microdot_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3486 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_websocket_alt.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2364 2023-06-06 22:20:32.000000 microdot-1.3.2/src/microdot_wsgi.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.783067 microdot-1.3.2/tests/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6572 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_cors.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1818 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_jinja.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    24051 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_microdot.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5088 2023-06-07 22:50:44.000000 microdot-1.3.2/tests/test_microdot_asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    24173 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_microdot_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2087 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_microdot_asyncio_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2670 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_microdot_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3449 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_microdot_wsgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2367 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_multidict.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5785 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_request.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5272 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_request_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    12042 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_response.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5784 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_response_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3855 2023-06-06 22:20:36.000000 microdot-1.3.2/tests/test_session.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4188 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_url_pattern.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      403 2023-06-06 22:20:32.000000 microdot-1.3.2/tests/test_urlencode.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1752 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_utemplate.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-16 10:41:02.570682 microdot-1.3.3/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1072 2023-06-16 15:35:30.000000 microdot-1.3.3/LICENSE
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1546 2023-07-16 10:41:02.574682 microdot-1.3.3/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      847 2023-06-16 15:35:30.000000 microdot-1.3.3/README.md
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      104 2023-06-16 15:35:30.000000 microdot-1.3.3/pyproject.toml
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1092 2023-07-16 10:41:02.574682 microdot-1.3.3/setup.cfg
+-rwxrwxr-x   0 miguel    (1000) miguel    (1000)       38 2023-06-16 15:35:30.000000 microdot-1.3.3/setup.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-16 10:41:02.570682 microdot-1.3.3/src/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-16 10:41:02.570682 microdot-1.3.3/src/microdot.egg-info/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1546 2023-07-16 10:41:02.000000 microdot-1.3.3/src/microdot.egg-info/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1074 2023-07-16 10:41:02.000000 microdot-1.3.3/src/microdot.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-07-16 10:41:02.000000 microdot-1.3.3/src/microdot.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-06-16 15:52:27.000000 microdot-1.3.3/src/microdot.egg-info/not-zip-safe
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       15 2023-07-16 10:41:02.000000 microdot-1.3.3/src/microdot.egg-info/requires.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      262 2023-07-16 10:41:02.000000 microdot-1.3.3/src/microdot.egg-info/top_level.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    46361 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     4991 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_asgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2855 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_asgi_websocket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    17370 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_asyncio.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     7828 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_asyncio_test_client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3780 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_asyncio_websocket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5270 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_cors.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1128 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_jinja.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2966 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_session.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10818 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_test_client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1331 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_utemplate.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5935 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_websocket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3486 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_websocket_alt.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2364 2023-07-16 10:39:46.000000 microdot-1.3.3/src/microdot_wsgi.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-16 10:41:02.570682 microdot-1.3.3/tests/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     6572 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_cors.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1818 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_jinja.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    24051 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_microdot.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5088 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_microdot_asgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    24173 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_microdot_asyncio.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2087 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_microdot_asyncio_websocket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2670 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_microdot_websocket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3449 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_microdot_wsgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2367 2023-06-16 15:35:30.000000 microdot-1.3.3/tests/test_multidict.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5819 2023-06-21 19:21:22.000000 microdot-1.3.3/tests/test_request.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5306 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_request_asyncio.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    12042 2023-06-16 15:35:30.000000 microdot-1.3.3/tests/test_response.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5784 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_response_asyncio.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3855 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_session.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     4188 2023-06-16 15:35:30.000000 microdot-1.3.3/tests/test_url_pattern.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      403 2023-06-16 15:35:30.000000 microdot-1.3.3/tests/test_urlencode.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1752 2023-07-16 10:39:46.000000 microdot-1.3.3/tests/test_utemplate.py
```

### Comparing `microdot-1.3.2/LICENSE` & `microdot-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/PKG-INFO` & `microdot-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.3.2
+Version: 1.3.3
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 # microdot
 [![Build status](https://github.com/miguelgrinberg/microdot/workflows/build/badge.svg)](https://github.com/miguelgrinberg/microdot/actions) [![codecov](https://codecov.io/gh/miguelgrinberg/microdot/branch/main/graph/badge.svg)](https://codecov.io/gh/miguelgrinberg/microdot)
 
 *“The impossibly small web framework for Python and MicroPython”*
```

### Comparing `microdot-1.3.2/README.md` & `microdot-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/setup.cfg` & `microdot-1.3.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = microdot
-version = 1.3.2
+version = 1.3.3
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = The impossibly small web framework for MicroPython
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/microdot
 project_urls = 
@@ -24,20 +24,25 @@
 	= src
 py_modules = 
 	microdot
 	microdot_asyncio
 	microdot_utemplate
 	microdot_jinja
 	microdot_session
+	microdot_cors
 	microdot_websocket
 	microdot_websocket_alt
 	microdot_asyncio_websocket
 	microdot_test_client
 	microdot_asyncio_test_client
 	microdot_wsgi
 	microdot_asgi
 	microdot_asgi_websocket
 
+[options.extras_require]
+docs = 
+	sphinx
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `microdot-1.3.2/src/microdot.egg-info/PKG-INFO` & `microdot-1.3.3/src/microdot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.3.2
+Version: 1.3.3
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 # microdot
 [![Build status](https://github.com/miguelgrinberg/microdot/workflows/build/badge.svg)](https://github.com/miguelgrinberg/microdot/actions) [![codecov](https://codecov.io/gh/miguelgrinberg/microdot/branch/main/graph/badge.svg)](https://codecov.io/gh/miguelgrinberg/microdot)
 
 *“The impossibly small web framework for Python and MicroPython”*
```

### Comparing `microdot-1.3.2/src/microdot.egg-info/SOURCES.txt` & `microdot-1.3.3/src/microdot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 setup.py
 src/microdot.py
 src/microdot_asgi.py
 src/microdot_asgi_websocket.py
 src/microdot_asyncio.py
 src/microdot_asyncio_test_client.py
 src/microdot_asyncio_websocket.py
+src/microdot_cors.py
 src/microdot_jinja.py
 src/microdot_session.py
 src/microdot_test_client.py
 src/microdot_utemplate.py
 src/microdot_websocket.py
 src/microdot_websocket_alt.py
 src/microdot_wsgi.py
 src/microdot.egg-info/PKG-INFO
 src/microdot.egg-info/SOURCES.txt
 src/microdot.egg-info/dependency_links.txt
 src/microdot.egg-info/not-zip-safe
+src/microdot.egg-info/requires.txt
 src/microdot.egg-info/top_level.txt
 tests/test_cors.py
 tests/test_jinja.py
 tests/test_microdot.py
 tests/test_microdot_asgi.py
 tests/test_microdot_asyncio.py
 tests/test_microdot_asyncio_websocket.py
```

### Comparing `microdot-1.3.2/src/microdot.py` & `microdot-1.3.3/src/microdot.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,21 +400,23 @@
         return Request(app, client_addr, method, url, http_version, headers,
                        stream=client_stream, sock=client_sock)
 
     def _parse_urlencoded(self, urlencoded):
         data = MultiDict()
         if len(urlencoded) > 0:
             if isinstance(urlencoded, str):
-                for k, v in [pair.split('=', 1)
-                             for pair in urlencoded.split('&') if pair]:
-                    data[urldecode_str(k)] = urldecode_str(v)
+                for kv in [pair.split('=', 1)
+                           for pair in urlencoded.split('&') if pair]:
+                    data[urldecode_str(kv[0])] = urldecode_str(kv[1]) \
+                        if len(kv) > 1 else ''
             elif isinstance(urlencoded, bytes):  # pragma: no branch
-                for k, v in [pair.split(b'=', 1)
-                             for pair in urlencoded.split(b'&') if pair]:
-                    data[urldecode_bytes(k)] = urldecode_bytes(v)
+                for kv in [pair.split(b'=', 1)
+                           for pair in urlencoded.split(b'&') if pair]:
+                    data[urldecode_bytes(kv[0])] = urldecode_bytes(kv[1]) \
+                        if len(kv) > 1 else b''
         return data
 
     @property
     def body(self):
         """The body of the request, as bytes."""
         if self.stream_used:
             raise RuntimeError('Cannot use both stream and body')
```

### Comparing `microdot-1.3.2/src/microdot_asgi.py` & `microdot-1.3.3/src/microdot_asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,25 +116,26 @@
                 if event['type'] == 'http.disconnect':  # pragma: no branch
                     cancelled = True
                     break
 
         asyncio.ensure_future(cancel_monitor())
 
         body_iter = res.body_iter().__aiter__()
+        res_body = b''
         try:
-            body = await body_iter.__anext__()
+            res_body = await body_iter.__anext__()
             while not cancelled:  # pragma: no branch
                 next_body = await body_iter.__anext__()
                 await send({'type': 'http.response.body',
-                            'body': body,
+                            'body': res_body,
                             'more_body': True})
-                body = next_body
+                res_body = next_body
         except StopAsyncIteration:
             await send({'type': 'http.response.body',
-                        'body': body,
+                        'body': res_body,
                         'more_body': False})
 
     async def __call__(self, scope, receive, send):
         return await self.asgi_app(scope, receive, send)
 
     def shutdown(self):
         if self.embedded_server:  # pragma: no cover
```

### Comparing `microdot-1.3.2/src/microdot_asgi_websocket.py` & `microdot-1.3.3/src/microdot_asgi_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_asyncio.py` & `microdot-1.3.3/src/microdot_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_asyncio_test_client.py` & `microdot-1.3.3/src/microdot_asyncio_test_client.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_asyncio_websocket.py` & `microdot-1.3.3/src/microdot_asyncio_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_jinja.py` & `microdot-1.3.3/src/microdot_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_session.py` & `microdot-1.3.3/src/microdot_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_test_client.py` & `microdot-1.3.3/src/microdot_test_client.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_utemplate.py` & `microdot-1.3.3/src/microdot_utemplate.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_websocket.py` & `microdot-1.3.3/src/microdot_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_websocket_alt.py` & `microdot-1.3.3/src/microdot_websocket_alt.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/src/microdot_wsgi.py` & `microdot-1.3.3/src/microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_cors.py` & `microdot-1.3.3/tests/test_cors.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_jinja.py` & `microdot-1.3.3/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_microdot.py` & `microdot-1.3.3/tests/test_microdot.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_microdot_asgi.py` & `microdot-1.3.3/tests/test_microdot_asgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_microdot_asyncio.py` & `microdot-1.3.3/tests/test_microdot_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_microdot_asyncio_websocket.py` & `microdot-1.3.3/tests/test_microdot_asyncio_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_microdot_websocket.py` & `microdot-1.3.3/tests/test_microdot_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_microdot_wsgi.py` & `microdot-1.3.3/tests/test_microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_multidict.py` & `microdot-1.3.3/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_request.py` & `microdot-1.3.3/tests/test_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,20 @@
             'Content-Length': '3'})
         self.assertEqual(req.content_type, 'application/json')
         self.assertEqual(req.cookies, {'foo': 'bar', 'abc': 'def'})
         self.assertEqual(req.content_length, 3)
         self.assertEqual(req.body, b'aaa')
 
     def test_args(self):
-        fd = get_request_fd('GET', '/?foo=bar&abc=def&x=%2f%%')
+        fd = get_request_fd('GET', '/?foo=bar&abc=def&foo&x=%2f%%')
         req = Request.create('app', fd, 'addr')
-        self.assertEqual(req.query_string, 'foo=bar&abc=def&x=%2f%%')
-        self.assertEqual(req.args, MultiDict(
-            {'foo': 'bar', 'abc': 'def', 'x': '/%%'}))
+        self.assertEqual(req.query_string, 'foo=bar&abc=def&foo&x=%2f%%')
+        md = MultiDict({'foo': 'bar', 'abc': 'def', 'x': '/%%'})
+        md['foo'] = ''
+        self.assertEqual(req.args, md)
 
     def test_badly_formatted_args(self):
         fd = get_request_fd('GET', '/?&foo=bar&abc=def&&&x=%2f%%')
         req = Request.create('app', fd, 'addr')
         self.assertEqual(req.query_string, '&foo=bar&abc=def&&&x=%2f%%')
         self.assertEqual(req.args, MultiDict(
             {'foo': 'bar', 'abc': 'def', 'x': '/%%'}))
```

### Comparing `microdot-1.3.2/tests/test_request_asyncio.py` & `microdot-1.3.3/tests/test_request_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,20 @@
             'Content-Length': '3'})
         self.assertEqual(req.content_type, 'application/json')
         self.assertEqual(req.cookies, {'foo': 'bar', 'abc': 'def'})
         self.assertEqual(req.content_length, 3)
         self.assertEqual(req.body, b'aaa')
 
     def test_args(self):
-        fd = get_async_request_fd('GET', '/?foo=bar&abc=def&x=%2f%%')
+        fd = get_async_request_fd('GET', '/?foo=bar&abc=def&foo&x=%2f%%')
         req = _run(Request.create('app', fd, 'writer', 'addr'))
-        self.assertEqual(req.query_string, 'foo=bar&abc=def&x=%2f%%')
-        self.assertEqual(req.args, MultiDict(
-            {'foo': 'bar', 'abc': 'def', 'x': '/%%'}))
+        self.assertEqual(req.query_string, 'foo=bar&abc=def&foo&x=%2f%%')
+        md = MultiDict({'foo': 'bar', 'abc': 'def', 'x': '/%%'})
+        md['foo'] = ''
+        self.assertEqual(req.args, md)
 
     def test_json(self):
         fd = get_async_request_fd('GET', '/foo', headers={
             'Content-Type': 'application/json'}, body='{"foo":"bar"}')
         req = _run(Request.create('app', fd, 'writer', 'addr'))
         json = req.json
         self.assertEqual(json, {'foo': 'bar'})
```

### Comparing `microdot-1.3.2/tests/test_response.py` & `microdot-1.3.3/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_response_asyncio.py` & `microdot-1.3.3/tests/test_response_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_session.py` & `microdot-1.3.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_url_pattern.py` & `microdot-1.3.3/tests/test_url_pattern.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.2/tests/test_utemplate.py` & `microdot-1.3.3/tests/test_utemplate.py`

 * *Files identical despite different names*

