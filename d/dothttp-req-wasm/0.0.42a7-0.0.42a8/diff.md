# Comparing `tmp/dothttp_req-wasm-0.0.42a7.tar.gz` & `tmp/dothttp_req-wasm-0.0.42a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dothttp_req-wasm-0.0.42a7.tar", last modified: Mon Dec 26 13:06:49 2022, max compression
+gzip compressed data, was "dothttp_req-wasm-0.0.42a8.tar", last modified: Tue Jan 31 11:47:05 2023, max compression
```

## Comparing `dothttp_req-wasm-0.0.42a7.tar` & `dothttp_req-wasm-0.0.42a8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.154391 dothttp_req-wasm-0.0.42a7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-26 13:06:49.154391 dothttp_req-wasm-0.0.42a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-26 13:06:43.000000 dothttp_req-wasm-0.0.42a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dotextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dotextensions/server/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/basic_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/gohandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/har2httphandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/http2har.py
--rw-r--r--   0 runner    (1001) docker     (123)    15379 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/http2postman.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/postman2http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dotextensions/server/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/models/har.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dotextensions/server/postman/
--rw-r--r--   0 runner    (1001) docker     (123)    55279 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/postman/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dotextensions/server/postman2_1/
--rw-r--r--   0 runner    (1001) docker     (123)    56959 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/postman2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dotextensions/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dotextensions/version/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/dothttp/
--rw-r--r--   0 runner    (1001) docker     (123)    38617 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/curl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/dsl_jsonparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/js3py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/parse_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/property_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/property_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    21940 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.154391 dothttp_req-wasm-0.0.42a7/dothttp_req/
--rw-r--r--   0 runner    (1001) docker     (123)    38617 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/curl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/dsl_jsonparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/js3py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/parse_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/property_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/property_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    21940 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/dothttp_req/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.154391 dothttp_req-wasm-0.0.42a7/dothttp_req_wasm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-26 13:06:49.000000 dothttp_req-wasm-0.0.42a7/dothttp_req_wasm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2022-12-26 13:06:49.000000 dothttp_req-wasm-0.0.42a7/dothttp_req_wasm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-26 13:06:49.000000 dothttp_req-wasm-0.0.42a7/dothttp_req_wasm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-26 13:06:49.000000 dothttp_req-wasm-0.0.42a7/dothttp_req_wasm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-26 13:06:49.000000 dothttp_req-wasm-0.0.42a7/dothttp_req_wasm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-26 13:06:49.154391 dothttp_req-wasm-0.0.42a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2022-12-26 13:06:43.000000 dothttp_req-wasm-0.0.42a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.150391 dothttp_req-wasm-0.0.42a7/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:49.154391 dothttp_req-wasm-0.0.42a7/test/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/test/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2022-12-26 13:06:10.000000 dothttp_req-wasm-0.0.42a7/test/server/ntlm_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.415902 dothttp_req-wasm-0.0.42a8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-31 11:47:05.415902 dothttp_req-wasm-0.0.42a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-31 11:46:57.000000 dothttp_req-wasm-0.0.42a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.403902 dothttp_req-wasm-0.0.42a8/dotextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.403902 dothttp_req-wasm-0.0.42a8/dotextensions/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.407902 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/basic_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/gohandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/har2httphandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/http2har.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/http2postman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/postman2http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.407902 dothttp_req-wasm-0.0.42a8/dotextensions/server/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/models/har.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.407902 dothttp_req-wasm-0.0.42a8/dotextensions/server/postman/
+-rw-r--r--   0 runner    (1001) docker     (123)    55279 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/postman/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.407902 dothttp_req-wasm-0.0.42a8/dotextensions/server/postman2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    56959 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/postman2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.407902 dothttp_req-wasm-0.0.42a8/dotextensions/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dotextensions/version/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.411903 dothttp_req-wasm-0.0.42a8/dothttp/
+-rw-r--r--   0 runner    (1001) docker     (123)    38617 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/curl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/dsl_jsonparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/js3py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/parse_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/property_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/property_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21940 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.411903 dothttp_req-wasm-0.0.42a8/dothttp_req/
+-rw-r--r--   0 runner    (1001) docker     (123)    38617 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/curl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/dsl_jsonparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/js3py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/parse_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/property_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/property_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21940 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/dothttp_req/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.415902 dothttp_req-wasm-0.0.42a8/dothttp_req_wasm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-31 11:47:05.000000 dothttp_req-wasm-0.0.42a8/dothttp_req_wasm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-31 11:47:05.000000 dothttp_req-wasm-0.0.42a8/dothttp_req_wasm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 11:47:05.000000 dothttp_req-wasm-0.0.42a8/dothttp_req_wasm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-31 11:47:05.000000 dothttp_req-wasm-0.0.42a8/dothttp_req_wasm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-31 11:47:05.000000 dothttp_req-wasm-0.0.42a8/dothttp_req_wasm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 11:47:05.415902 dothttp_req-wasm-0.0.42a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-31 11:46:57.000000 dothttp_req-wasm-0.0.42a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.403902 dothttp_req-wasm-0.0.42a8/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:47:05.415902 dothttp_req-wasm-0.0.42a8/test/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/test/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-31 11:46:14.000000 dothttp_req-wasm-0.0.42a8/test/server/ntlm_server.py
```

### Comparing `dothttp_req-wasm-0.0.42a7/LICENSE.txt` & `dothttp_req-wasm-0.0.42a8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/__main__.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/__main__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/basic_handlers.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/basic_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,22 +74,23 @@
         envs = params.get("env", [])
         target = params.get("target", '1')
         nocookie = params.get("nocookie", False)
         curl = params.get("curl", False)
         properties = [f"{i}={j}" for i, j in params.get('properties', {}).items()]
         content = params.get("content", None)
         contexts = params.get("contexts")
+        property_file = params.get("property-file", None)
         if contexts is None:
             contexts = []
         if content:
             try:
                 content = "\n".join(content.splitlines())
             except:
                 content = None
-        config = ContextConfig(file=filename, env=envs, properties=properties, curl=curl, property_file=None,
+        config = ContextConfig(file=filename, env=envs, properties=properties, curl=curl, property_file=property_file,
                                debug=True,
                                no_cookie=nocookie, format=False, info=False, target=target, content=content)
         config.contexts = contexts
         return config
 
     def get_request_result(self, command, comp: RequestCompiler):
         comp.load_def()
```

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/gohandler.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/gohandler.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/har2httphandler.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/har2httphandler.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/http2har.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/http2har.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/http2postman.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/http2postman.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/handlers/postman2http.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/handlers/postman2http.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/models/__init__.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/models/har.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/models/har.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/postman/__init__.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/postman/__init__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/postman2_1/__init__.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/postman2_1/__init__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/server.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/server.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dotextensions/server/utils.py` & `dothttp_req-wasm-0.0.42a8/dotextensions/server/utils.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/__init__.py` & `dothttp_req-wasm-0.0.42a8/dothttp/__init__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/__main__.py` & `dothttp_req-wasm-0.0.42a8/dothttp/__main__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/curl_utils.py` & `dothttp_req-wasm-0.0.42a8/dothttp/curl_utils.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/dsl_jsonparser.py` & `dothttp_req-wasm-0.0.42a8/dothttp/dsl_jsonparser.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/exceptions.py` & `dothttp_req-wasm-0.0.42a8/dothttp/exceptions.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/js3py.py` & `dothttp_req-wasm-0.0.42a8/dothttp/js3py.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/json_utils.py` & `dothttp_req-wasm-0.0.42a8/dothttp/json_utils.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/parse_models.py` & `dothttp_req-wasm-0.0.42a8/dothttp/parse_models.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/property_util.py` & `dothttp_req-wasm-0.0.42a8/dothttp/property_util.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/request_base.py` & `dothttp_req-wasm-0.0.42a8/dothttp/request_base.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp/utils.py` & `dothttp_req-wasm-0.0.42a8/dothttp/utils.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/__init__.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/__init__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/__main__.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/__main__.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/curl_utils.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/curl_utils.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/dsl_jsonparser.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/dsl_jsonparser.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/exceptions.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/exceptions.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/js3py.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/js3py.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/json_utils.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/json_utils.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/parse_models.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/parse_models.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/property_util.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/property_util.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/request_base.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/request_base.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req/utils.py` & `dothttp_req-wasm-0.0.42a8/dothttp_req/utils.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/dothttp_req_wasm.egg-info/SOURCES.txt` & `dothttp_req-wasm-0.0.42a8/dothttp_req_wasm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/setup.py` & `dothttp_req-wasm-0.0.42a8/setup.py`

 * *Files identical despite different names*

### Comparing `dothttp_req-wasm-0.0.42a7/test/server/ntlm_server.py` & `dothttp_req-wasm-0.0.42a8/test/server/ntlm_server.py`

 * *Files identical despite different names*

