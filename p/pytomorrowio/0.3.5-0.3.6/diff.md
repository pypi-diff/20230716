# Comparing `tmp/pytomorrowio-0.3.5.tar.gz` & `tmp/pytomorrowio-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytomorrowio-0.3.5.tar", last modified: Thu Sep 22 02:22:38 2022, max compression
+gzip compressed data, was "pytomorrowio-0.3.6.tar", last modified: Sun Jul 16 06:49:47 2023, max compression
```

## Comparing `pytomorrowio-0.3.5.tar` & `pytomorrowio-0.3.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:22:38.579934 pytomorrowio-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-09-22 02:22:38.579934 pytomorrowio-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:22:38.575934 pytomorrowio-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4870 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:22:38.575934 pytomorrowio-0.3.5/pytomorrowio/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/pytomorrowio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/pytomorrowio/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/pytomorrowio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/pytomorrowio/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/pytomorrowio/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    22036 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/pytomorrowio/pytomorrowio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:22:38.575934 pytomorrowio-0.3.5/pytomorrowio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-09-22 02:22:38.000000 pytomorrowio-0.3.5/pytomorrowio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-09-22 02:22:38.000000 pytomorrowio-0.3.5/pytomorrowio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 02:22:38.000000 pytomorrowio-0.3.5/pytomorrowio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 02:22:38.000000 pytomorrowio-0.3.5/pytomorrowio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-22 02:22:38.000000 pytomorrowio-0.3.5/pytomorrowio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-22 02:22:38.000000 pytomorrowio-0.3.5/pytomorrowio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-22 02:22:38.579934 pytomorrowio-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:22:38.575934 pytomorrowio-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:22:38.579934 pytomorrowio-0.3.5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/empty_response.json
--rw-r--r--   0 runner    (1001) docker     (121)    28840 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_1day.json
--rw-r--r--   0 runner    (1001) docker     (121)    50447 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_1day_greater_than_max_fields_1.json
--rw-r--r--   0 runner    (1001) docker     (121)    11633 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_1day_greater_than_max_fields_2.json
--rw-r--r--   0 runner    (1001) docker     (121)    99221 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_1hour.json
--rw-r--r--   0 runner    (1001) docker     (121)   328426 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_1min.json
--rw-r--r--   0 runner    (1001) docker     (121)    66743 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_5min.json
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_realtime.json
--rw-r--r--   0 runner    (1001) docker     (121)   958339 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_realtime_1min_1hour_1day.json
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_realtime_more_than_max_fields_1.json
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/fixtures/timelines_realtime_more_than_max_fields_2.json
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12872 2022-09-22 02:22:36.000000 pytomorrowio-0.3.5/tests/test_pytomorrowio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:49:47.942602 pytomorrowio-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-16 06:49:47.942602 pytomorrowio-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:49:47.938602 pytomorrowio-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4870 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:49:47.938602 pytomorrowio-0.3.6/pytomorrowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/pytomorrowio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/pytomorrowio/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/pytomorrowio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/pytomorrowio/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/pytomorrowio/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/pytomorrowio/pytomorrowio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:49:47.938602 pytomorrowio-0.3.6/pytomorrowio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-16 06:49:47.000000 pytomorrowio-0.3.6/pytomorrowio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-16 06:49:47.000000 pytomorrowio-0.3.6/pytomorrowio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 06:49:47.000000 pytomorrowio-0.3.6/pytomorrowio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 06:49:47.000000 pytomorrowio-0.3.6/pytomorrowio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 06:49:47.000000 pytomorrowio-0.3.6/pytomorrowio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-16 06:49:47.000000 pytomorrowio-0.3.6/pytomorrowio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-16 06:49:47.942602 pytomorrowio-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:49:47.938602 pytomorrowio-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:49:47.942602 pytomorrowio-0.3.6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/empty_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28840 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_1day.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50447 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_1day_greater_than_max_fields_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_1day_greater_than_max_fields_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    99221 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_1hour.json
+-rw-r--r--   0 runner    (1001) docker     (123)   328426 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_1min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    66743 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_5min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_realtime.json
+-rw-r--r--   0 runner    (1001) docker     (123)   958339 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_realtime_1min_1hour_1day.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_realtime_more_than_max_fields_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/fixtures/timelines_realtime_more_than_max_fields_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-07-16 06:49:44.000000 pytomorrowio-0.3.6/tests/test_pytomorrowio.py
```

### Comparing `pytomorrowio-0.3.5/CONTRIBUTING.rst` & `pytomorrowio-0.3.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/LICENSE` & `pytomorrowio-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/PKG-INFO` & `pytomorrowio-0.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pytomorrowio
-Version: 0.3.5
+Version: 0.3.6
 Summary: Async Python3.9+ package to access the Tomorrow.io API
 Home-page: https://github.com/raman325/pytomorrowio
 Author: raman325
 Author-email: 7243222+raman325@users.noreply.github.com
 License: MIT license
 Keywords: pytomorrowio
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -71,9 +70,7 @@
 History
 =======
 
 0.1.0 (2020-06-04)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `pytomorrowio-0.3.5/README.rst` & `pytomorrowio-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/docs/Makefile` & `pytomorrowio-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/docs/conf.py` & `pytomorrowio-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/docs/installation.rst` & `pytomorrowio-0.3.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/docs/make.bat` & `pytomorrowio-0.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/pytomorrowio/const.py` & `pytomorrowio-0.3.6/pytomorrowio/const.py`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/pytomorrowio/exceptions.py` & `pytomorrowio-0.3.6/pytomorrowio/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/pytomorrowio/fields.py` & `pytomorrowio-0.3.6/pytomorrowio/fields.py`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/pytomorrowio/pytomorrowio.py` & `pytomorrowio-0.3.6/pytomorrowio/pytomorrowio.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,39 +233,47 @@
                 json=payload,
                 compress=False,
             )
             resp_json = await resp.json(content_type=None)
         except ClientConnectionError as error:
             raise CantConnectException() from error
 
-        _LOGGER.debug(
-            "Received a response with status code %s and headers %s",
-            resp.status,
-            resp.headers,
-        )
-
         self._rate_limits = CIMultiDict(
             {k: int(v) for k, v in resp.headers.items() if "ratelimit" in k.lower()}
         )
 
         if resp.status in (HTTPStatus.OK, HTTPStatus.PARTIAL_CONTENT):
+            _LOGGER.debug(
+                "Received a response with status code %s and headers %s",
+                resp.status,
+                resp.headers,
+            )
+
             self._num_api_requests += 1
             for warning in set(
                 warning["message"] for warning in resp_json.get("warnings", [])
             ):
                 _LOGGER.info(
                     (
                         "While calling the API for the timesteps [%s], the following "
                         "warning was returned: %s"
                     ),
                     ", ".join(params["timesteps"]),
                     warning,
                 )
 
             return resp_json
+
+        _LOGGER.debug(
+            "Received a response with status code %s, headers %s, and body: %s",
+            resp.status,
+            resp.headers,
+            resp_json,
+        )
+
         if resp.status == HTTPStatus.BAD_REQUEST:
             raise MalformedRequestException(resp_json, resp.headers)
         if resp.status in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
             raise InvalidAPIKeyException(resp_json, resp.headers)
         if resp.status == HTTPStatus.TOO_MANY_REQUESTS:
             raise RateLimitedException(resp_json, resp.headers)
```

### Comparing `pytomorrowio-0.3.5/pytomorrowio.egg-info/PKG-INFO` & `pytomorrowio-0.3.6/pytomorrowio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pytomorrowio
-Version: 0.3.5
+Version: 0.3.6
 Summary: Async Python3.9+ package to access the Tomorrow.io API
 Home-page: https://github.com/raman325/pytomorrowio
 Author: raman325
 Author-email: 7243222+raman325@users.noreply.github.com
 License: MIT license
 Keywords: pytomorrowio
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -71,9 +70,7 @@
 History
 =======
 
 0.1.0 (2020-06-04)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `pytomorrowio-0.3.5/pytomorrowio.egg-info/SOURCES.txt` & `pytomorrowio-0.3.6/pytomorrowio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/setup.cfg` & `pytomorrowio-0.3.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.5
+current_version = 0.3.6
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pytomorrowio-0.3.5/setup.py` & `pytomorrowio-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     keywords="pytomorrowio",
     name="pytomorrowio",
     packages=find_packages(include=["pytomorrowio", "pytomorrowio.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/raman325/pytomorrowio",
-    version="0.3.5",
+    version="0.3.6",
     zip_safe=False,
 )
```

### Comparing `pytomorrowio-0.3.5/tests/const.py` & `pytomorrowio-0.3.6/tests/const.py`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_1day.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_1day.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_1day_greater_than_max_fields_1.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_1day_greater_than_max_fields_1.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_1day_greater_than_max_fields_2.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_1day_greater_than_max_fields_2.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_1hour.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_1hour.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_1min.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_1min.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_5min.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_5min.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_realtime.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_realtime.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_realtime_1min_1hour_1day.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_realtime_1min_1hour_1day.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_realtime_more_than_max_fields_1.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_realtime_more_than_max_fields_1.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/fixtures/timelines_realtime_more_than_max_fields_2.json` & `pytomorrowio-0.3.6/tests/fixtures/timelines_realtime_more_than_max_fields_2.json`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/helpers.py` & `pytomorrowio-0.3.6/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytomorrowio-0.3.5/tests/test_pytomorrowio.py` & `pytomorrowio-0.3.6/tests/test_pytomorrowio.py`

 * *Files identical despite different names*

