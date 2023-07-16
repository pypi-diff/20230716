# Comparing `tmp/deepchecks-llm-client-0.0.3.tar.gz` & `tmp/deepchecks-llm-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchecks-llm-client-0.0.3.tar", last modified: Thu Jul 13 07:06:24 2023, max compression
+gzip compressed data, was "deepchecks-llm-client-0.0.4.tar", last modified: Sun Jul 16 11:08:51 2023, max compression
```

## Comparing `deepchecks-llm-client-0.0.3.tar` & `deepchecks-llm-client-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.998999 deepchecks-llm-client-0.0.3/
--rw-r--r--   0 shay       (501) staff       (20)       18 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.3/MANIFEST.in
--rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-13 07:06:23.998882 deepchecks-llm-client-0.0.3/PKG-INFO
--rw-r--r--   0 shay       (501) staff       (20)      142 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/README.md
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.997882 deepchecks-llm-client-0.0.3/deepchecks_llm_client/
--rw-r--r--   0 shay       (501) staff       (20)       88 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/__init__.py
--rw-r--r--   0 shay       (501) staff       (20)     3847 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/api.py
--rw-r--r--   0 shay       (501) staff       (20)     3214 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/client.py
--rw-r--r--   0 shay       (501) staff       (20)     3682 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/openai_instrumentor.py
--rw-r--r--   0 shay       (501) staff       (20)     2887 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/utils.py
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.998444 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/
--rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/PKG-INFO
--rw-r--r--   0 shay       (501) staff       (20)      481 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/SOURCES.txt
--rw-r--r--   0 shay       (501) staff       (20)        1 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/dependency_links.txt
--rw-r--r--   0 shay       (501) staff       (20)       29 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/requires.txt
--rw-r--r--   0 shay       (501) staff       (20)       22 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/top_level.txt
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.998620 deepchecks-llm-client-0.0.3/examples/
--rw-r--r--   0 shay       (501) staff       (20)        0 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/examples/__init__.py
--rw-r--r--   0 shay       (501) staff       (20)     2327 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/examples/usage.py
--rw-r--r--   0 shay       (501) staff       (20)       29 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.3/requirements.txt
--rw-r--r--   0 shay       (501) staff       (20)       38 2023-07-13 07:06:23.999039 deepchecks-llm-client-0.0.3/setup.cfg
--rw-r--r--   0 shay       (501) staff       (20)     3069 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.3/setup.py
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.661552 deepchecks-llm-client-0.0.4/
+-rw-r--r--   0 shay       (501) staff       (20)       18 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.4/MANIFEST.in
+-rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-16 11:08:51.661449 deepchecks-llm-client-0.0.4/PKG-INFO
+-rw-r--r--   0 shay       (501) staff       (20)      142 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/README.md
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.660498 deepchecks-llm-client-0.0.4/deepchecks_llm_client/
+-rw-r--r--   0 shay       (501) staff       (20)       88 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/__init__.py
+-rw-r--r--   0 shay       (501) staff       (20)     3847 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/api.py
+-rw-r--r--   0 shay       (501) staff       (20)     3214 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/client.py
+-rw-r--r--   0 shay       (501) staff       (20)     3682 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/openai_instrumentor.py
+-rw-r--r--   0 shay       (501) staff       (20)     2887 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/utils.py
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.661007 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/
+-rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/PKG-INFO
+-rw-r--r--   0 shay       (501) staff       (20)      481 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shay       (501) staff       (20)        1 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shay       (501) staff       (20)       13 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/requires.txt
+-rw-r--r--   0 shay       (501) staff       (20)       22 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/top_level.txt
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.661189 deepchecks-llm-client-0.0.4/examples/
+-rw-r--r--   0 shay       (501) staff       (20)        0 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/examples/__init__.py
+-rw-r--r--   0 shay       (501) staff       (20)     2327 2023-07-16 10:23:12.000000 deepchecks-llm-client-0.0.4/examples/usage.py
+-rw-r--r--   0 shay       (501) staff       (20)       13 2023-07-16 11:07:56.000000 deepchecks-llm-client-0.0.4/requirements.txt
+-rw-r--r--   0 shay       (501) staff       (20)       38 2023-07-16 11:08:51.661582 deepchecks-llm-client-0.0.4/setup.cfg
+-rw-r--r--   0 shay       (501) staff       (20)     3069 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.4/setup.py
```

### Comparing `deepchecks-llm-client-0.0.3/deepchecks_llm_client/api.py` & `deepchecks-llm-client-0.0.4/deepchecks_llm_client/api.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.0.3/deepchecks_llm_client/client.py` & `deepchecks-llm-client-0.0.4/deepchecks_llm_client/client.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.0.3/deepchecks_llm_client/openai_instrumentor.py` & `deepchecks-llm-client-0.0.4/deepchecks_llm_client/openai_instrumentor.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.0.3/deepchecks_llm_client/utils.py` & `deepchecks-llm-client-0.0.4/deepchecks_llm_client/utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.0.3/examples/usage.py` & `deepchecks-llm-client-0.0.4/examples/usage.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.0.3/setup.py` & `deepchecks-llm-client-0.0.4/setup.py`

 * *Files identical despite different names*

