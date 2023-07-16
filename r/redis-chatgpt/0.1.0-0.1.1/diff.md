# Comparing `tmp/redis_chatgpt-0.1.0.tar.gz` & `tmp/redis_chatgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_chatgpt-0.1.0.tar", last modified: Sun Jul 16 08:34:55 2023, max compression
+gzip compressed data, was "redis_chatgpt-0.1.1.tar", last modified: Sun Jul 16 08:48:27 2023, max compression
```

## Comparing `redis_chatgpt-0.1.0.tar` & `redis_chatgpt-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:34:55.676557 redis_chatgpt-0.1.0/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1072 2023-07-15 07:33:47.000000 redis_chatgpt-0.1.0/LICENSE
--rw-rw-r--   0 elmira    (1002) elmira    (1002)      335 2023-07-16 08:34:55.676557 redis_chatgpt-0.1.0/PKG-INFO
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1177 2023-07-16 08:33:43.000000 redis_chatgpt-0.1.0/README.md
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:34:55.676557 redis_chatgpt-0.1.0/redis_chatgpt/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       82 2023-07-15 07:41:51.000000 redis_chatgpt-0.1.0/redis_chatgpt/__init__.py
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:34:55.676557 redis_chatgpt-0.1.0/redis_chatgpt/manager/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       84 2023-07-15 08:36:59.000000 redis_chatgpt-0.1.0/redis_chatgpt/manager/__init__.py
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1537 2023-07-15 07:41:10.000000 redis_chatgpt-0.1.0/redis_chatgpt/manager/db_manager.py
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:34:55.676557 redis_chatgpt-0.1.0/redis_chatgpt.egg-info/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)      335 2023-07-16 08:34:55.000000 redis_chatgpt-0.1.0/redis_chatgpt.egg-info/PKG-INFO
--rw-rw-r--   0 elmira    (1002) elmira    (1002)      306 2023-07-16 08:34:55.000000 redis_chatgpt-0.1.0/redis_chatgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)        1 2023-07-16 08:34:55.000000 redis_chatgpt-0.1.0/redis_chatgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       13 2023-07-16 08:34:55.000000 redis_chatgpt-0.1.0/redis_chatgpt.egg-info/requires.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       14 2023-07-16 08:34:55.000000 redis_chatgpt-0.1.0/redis_chatgpt.egg-info/top_level.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       38 2023-07-16 08:34:55.676557 redis_chatgpt-0.1.0/setup.cfg
--rw-rw-r--   0 elmira    (1002) elmira    (1002)      500 2023-07-16 08:33:56.000000 redis_chatgpt-0.1.0/setup.py
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1072 2023-07-15 07:33:47.000000 redis_chatgpt-0.1.1/LICENSE
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1550 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/PKG-INFO
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1174 2023-07-16 08:37:54.000000 redis_chatgpt-0.1.1/README.md
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/redis_chatgpt/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       82 2023-07-15 07:41:51.000000 redis_chatgpt-0.1.1/redis_chatgpt/__init__.py
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/redis_chatgpt/manager/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       84 2023-07-15 08:36:59.000000 redis_chatgpt-0.1.1/redis_chatgpt/manager/__init__.py
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1537 2023-07-15 07:41:10.000000 redis_chatgpt-0.1.1/redis_chatgpt/manager/db_manager.py
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1550 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)      306 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)        1 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       13 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/requires.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       14 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/top_level.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       38 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/setup.cfg
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)      756 2023-07-16 08:47:56.000000 redis_chatgpt-0.1.1/setup.py
```

### Comparing `redis_chatgpt-0.1.0/LICENSE` & `redis_chatgpt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_chatgpt-0.1.0/README.md` & `redis_chatgpt-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Redis Chatgpt
 Allows to save chat history of converation.
 
 
 # Getting started
 ```
-pip install -i redis-chatgpt
+pip install redis-chatgpt
 ```
 
 To build a simple data store:
 ```
 from redis_chatgpt.manager import RedisManager
 
 redis_db = RedisManager(host="localhost", port=6379)
```

### Comparing `redis_chatgpt-0.1.0/redis_chatgpt/manager/db_manager.py` & `redis_chatgpt-0.1.1/redis_chatgpt/manager/db_manager.py`

 * *Files identical despite different names*

