# Comparing `tmp/volworld_aws_api_common-0.1.98.tar.gz` & `tmp/volworld_aws_api_common-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volworld_aws_api_common-0.1.98.tar", last modified: Fri May  5 13:00:21 2023, max compression
+gzip compressed data, was "volworld_aws_api_common-0.1.99.tar", last modified: Thu May 18 00:48:28 2023, max compression
```

## Comparing `volworld_aws_api_common-0.1.98.tar` & `volworld_aws_api_common-0.1.99.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/LICENSE.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/README.rst
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/setup.cfg
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-05 13:00:19.000000 volworld_aws_api_common-0.1.98/setup.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.497691 volworld_aws_api_common-0.1.98/src/
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.497691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.501691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/AA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/Aws.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/Url.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.501691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/enum/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-05 12:58:42.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/enum/ErrorCode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/enum/HttpStatus.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/enum/ProjectModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/enum/QueryModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/enum/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.501691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/url/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/url/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      809 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/url/authUrl.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/ProjectMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/QueryMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/UserPool.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/api/OAPI.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/api/OpenApiValidation.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/api/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3260 2023-05-05 13:00:15.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/api/request_open_api_validation.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/ATestRequest.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/get__current_user.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/post__login.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/post__signup.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/request_util.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-05 03:26:25.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/url.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.505691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/behave/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/behave/ACotA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/behave/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/request.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 13:00:21.501691 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common.egg-info/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 13:00:21.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common.egg-info/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1840 2023-05-05 13:00:21.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common.egg-info/SOURCES.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-05 13:00:21.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common.egg-info/dependency_links.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-05 13:00:21.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common.egg-info/requires.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-05 13:00:21.000000 volworld_aws_api_common-0.1.98/src/volworld_aws_api_common.egg-info/top_level.txt
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.591691 volworld_aws_api_common-0.1.99/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/LICENSE.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      251 2023-05-18 00:48:28.591691 volworld_aws_api_common-0.1.99/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/README.rst
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-18 00:48:28.591691 volworld_aws_api_common-0.1.99/setup.cfg
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-18 00:48:21.000000 volworld_aws_api_common-0.1.99/setup.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.575692 volworld_aws_api_common-0.1.99/src/
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.575692 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.575692 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/AA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/Aws.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/Url.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      167 2023-05-17 02:29:05.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/dom_id.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.579692 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/enum/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/enum/ErrorCode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/enum/HttpStatus.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/enum/ProjectModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/enum/QueryModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/enum/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.579692 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/url/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/url/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      809 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/url/authUrl.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.587691 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/ProjectMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/QueryMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/UserPool.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.587691 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/api/OAPI.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/api/OpenApiValidation.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/api/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3260 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/api/request_open_api_validation.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.587691 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/ATestRequest.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.587691 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/get__current_user.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/post__login.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/post__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/request_util.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/url.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.591691 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/behave/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/behave/ACotA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/behave/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-18 00:45:33.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/request.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-18 00:48:28.575692 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common.egg-info/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      251 2023-05-18 00:48:28.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common.egg-info/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1882 2023-05-18 00:48:28.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-18 00:48:28.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-18 00:48:28.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common.egg-info/requires.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-18 00:48:28.000000 volworld_aws_api_common-0.1.99/src/volworld_aws_api_common.egg-info/top_level.txt
```

### Comparing `volworld_aws_api_common-0.1.98/LICENSE.txt` & `volworld_aws_api_common-0.1.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/enum/HttpStatus.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/enum/HttpStatus.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/api/url/authUrl.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/api/url/authUrl.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/UserPool.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/UserPool.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/api/OpenApiValidation.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/api/OpenApiValidation.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/api/request_open_api_validation.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/api/request_open_api_validation.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/get__current_user.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/get__current_user.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/post__login.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/post__login.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/post__signup.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/post__signup.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/request/request_util.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/request/request_util.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/aws/url.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/aws/url.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common/test/request.py` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common/test/request.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.98/src/volworld_aws_api_common.egg-info/SOURCES.txt` & `volworld_aws_api_common-0.1.99/src/volworld_aws_api_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/volworld_aws_api_common.egg-info/dependency_links.txt
 src/volworld_aws_api_common.egg-info/requires.txt
 src/volworld_aws_api_common.egg-info/top_level.txt
 src/volworld_aws_api_common/api/AA.py
 src/volworld_aws_api_common/api/Aws.py
 src/volworld_aws_api_common/api/Url.py
 src/volworld_aws_api_common/api/__init__.py
+src/volworld_aws_api_common/api/dom_id.py
 src/volworld_aws_api_common/api/enum/ErrorCode.py
 src/volworld_aws_api_common/api/enum/HttpStatus.py
 src/volworld_aws_api_common/api/enum/ProjectModeType.py
 src/volworld_aws_api_common/api/enum/QueryModeType.py
 src/volworld_aws_api_common/api/enum/__init__.py
 src/volworld_aws_api_common/api/url/__init__.py
 src/volworld_aws_api_common/api/url/authUrl.py
```

