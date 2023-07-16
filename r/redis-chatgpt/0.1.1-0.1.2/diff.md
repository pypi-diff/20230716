# Comparing `tmp/redis_chatgpt-0.1.1.tar.gz` & `tmp/redis_chatgpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_chatgpt-0.1.1.tar", last modified: Sun Jul 16 08:48:27 2023, max compression
+gzip compressed data, was "redis_chatgpt-0.1.2.tar", last modified: Sun Jul 16 09:05:46 2023, max compression
```

## Comparing `redis_chatgpt-0.1.1.tar` & `redis_chatgpt-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1072 2023-07-15 07:33:47.000000 redis_chatgpt-0.1.1/LICENSE
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1550 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/PKG-INFO
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1174 2023-07-16 08:37:54.000000 redis_chatgpt-0.1.1/README.md
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/redis_chatgpt/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       82 2023-07-15 07:41:51.000000 redis_chatgpt-0.1.1/redis_chatgpt/__init__.py
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/redis_chatgpt/manager/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       84 2023-07-15 08:36:59.000000 redis_chatgpt-0.1.1/redis_chatgpt/manager/__init__.py
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1537 2023-07-15 07:41:10.000000 redis_chatgpt-0.1.1/redis_chatgpt/manager/db_manager.py
-drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/
--rw-rw-r--   0 elmira    (1002) elmira    (1002)     1550 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/PKG-INFO
--rw-rw-r--   0 elmira    (1002) elmira    (1002)      306 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)        1 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       13 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/requires.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       14 2023-07-16 08:48:27.000000 redis_chatgpt-0.1.1/redis_chatgpt.egg-info/top_level.txt
--rw-rw-r--   0 elmira    (1002) elmira    (1002)       38 2023-07-16 08:48:27.213379 redis_chatgpt-0.1.1/setup.cfg
--rw-rw-r--   0 elmira    (1002) elmira    (1002)      756 2023-07-16 08:47:56.000000 redis_chatgpt-0.1.1/setup.py
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 09:05:46.107831 redis_chatgpt-0.1.2/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1072 2023-07-15 07:33:47.000000 redis_chatgpt-0.1.2/LICENSE
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     2274 2023-07-16 09:05:46.107831 redis_chatgpt-0.1.2/PKG-INFO
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1898 2023-07-16 09:04:26.000000 redis_chatgpt-0.1.2/README.md
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 09:05:46.107831 redis_chatgpt-0.1.2/redis_chatgpt/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       82 2023-07-15 07:41:51.000000 redis_chatgpt-0.1.2/redis_chatgpt/__init__.py
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 09:05:46.107831 redis_chatgpt-0.1.2/redis_chatgpt/manager/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       84 2023-07-15 08:36:59.000000 redis_chatgpt-0.1.2/redis_chatgpt/manager/__init__.py
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     1537 2023-07-15 07:41:10.000000 redis_chatgpt-0.1.2/redis_chatgpt/manager/db_manager.py
+drwxrwxr-x   0 elmira    (1002) elmira    (1002)        0 2023-07-16 09:05:46.107831 redis_chatgpt-0.1.2/redis_chatgpt.egg-info/
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)     2274 2023-07-16 09:05:46.000000 redis_chatgpt-0.1.2/redis_chatgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)      306 2023-07-16 09:05:46.000000 redis_chatgpt-0.1.2/redis_chatgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)        1 2023-07-16 09:05:46.000000 redis_chatgpt-0.1.2/redis_chatgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       13 2023-07-16 09:05:46.000000 redis_chatgpt-0.1.2/redis_chatgpt.egg-info/requires.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       14 2023-07-16 09:05:46.000000 redis_chatgpt-0.1.2/redis_chatgpt.egg-info/top_level.txt
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)       38 2023-07-16 09:05:46.107831 redis_chatgpt-0.1.2/setup.cfg
+-rw-rw-r--   0 elmira    (1002) elmira    (1002)      756 2023-07-16 09:05:08.000000 redis_chatgpt-0.1.2/setup.py
```

### Comparing `redis_chatgpt-0.1.1/LICENSE` & `redis_chatgpt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_chatgpt-0.1.1/PKG-INFO` & `redis_chatgpt-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: redis_chatgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A user-friendly package designed to save chat history conversation and truncate conversation if user exceeds max token when using OpenAI chat completion.
 Author: Elmira Ghorbani
 Project-URL: Github, https://github.com/ElmiraGhorbani/redis-chatgpt
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Redis Chatgpt
-Allows to save chat history of converation.
+This package is a useful tool specifically developed for effectively handling chat message history. This Python package's primary goal is to provide a reliable, efficient, and simple method to store chat logs in a Redis database.
 
+redis_chatgpt makes use of Redis, a fast, efficient, and highly scalable in-memory data structure store. By organizing and preserving the chat message history in Redis, users can retrieve message history promptly and easily with the best performance.
+
+This package is the perfect solution if you need to store and recover chat histories effortlessly from the Redis Database. With redis_chatgpt, you can streamline your chat log management tasks while becoming more productive and efficient with your resources.
 
 # Getting started
 ```
 pip install redis-chatgpt
 ```
 
 To build a simple data store:
 ```
 from redis_chatgpt.manager import RedisManager
 
 redis_db = RedisManager(host="localhost", port=6379)
+```
 
-# set data
+Set data
+```
 redis_key = "chat_key"
 chat_memory = [
     {
       "role": "system",
       "content": "Assistant is a large language model trained by OpenAI."
     },
     {
@@ -38,29 +43,30 @@
       "content": "hi"
     },
 ]
 redis_db.set_data(redis_key, chat_memory)
 
 ```
 
-```
-# get data
 
+Get data
+```
 chat_history = redis_db.get_data(redis_key)
 
 ```
 
+Truncate history(conversation)
 ```
-# truncate history(conversation)
+# You can choose whether to update the Redis database or 
+# not by specifying the 'overwrite' parameter (boolean).
 
-# You can choose whether to update the Redis database or not by specifying the 'overwrite' parameter (boolean)."
-redis_db.truncate_conversation(redis_key, overwrite=True)
+data = redis_db.truncate_conversation(redis_key, overwrite=True)
 
 ```
 
 ### Use with FastAPI Swagger
 `cd examples/chatbot`
 1. Get your `OpenAI` API key [here](https://platform.openai.com/overview).
 2. Copy env.example .env (set fastapi webserver workers and openai api key)
     `cp env.example .env`
-3. docker-compose up -d
-4. http://0.0.0.0:8012/docs
+3. `docker-compose up -d`
+4. check out : `http://0.0.0.0:8012/docs`
```

### Comparing `redis_chatgpt-0.1.1/redis_chatgpt/manager/db_manager.py` & `redis_chatgpt-0.1.2/redis_chatgpt/manager/db_manager.py`

 * *Files identical despite different names*

### Comparing `redis_chatgpt-0.1.1/redis_chatgpt.egg-info/PKG-INFO` & `redis_chatgpt-0.1.2/redis_chatgpt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: redis-chatgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A user-friendly package designed to save chat history conversation and truncate conversation if user exceeds max token when using OpenAI chat completion.
 Author: Elmira Ghorbani
 Project-URL: Github, https://github.com/ElmiraGhorbani/redis-chatgpt
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Redis Chatgpt
-Allows to save chat history of converation.
+This package is a useful tool specifically developed for effectively handling chat message history. This Python package's primary goal is to provide a reliable, efficient, and simple method to store chat logs in a Redis database.
 
+redis_chatgpt makes use of Redis, a fast, efficient, and highly scalable in-memory data structure store. By organizing and preserving the chat message history in Redis, users can retrieve message history promptly and easily with the best performance.
+
+This package is the perfect solution if you need to store and recover chat histories effortlessly from the Redis Database. With redis_chatgpt, you can streamline your chat log management tasks while becoming more productive and efficient with your resources.
 
 # Getting started
 ```
 pip install redis-chatgpt
 ```
 
 To build a simple data store:
 ```
 from redis_chatgpt.manager import RedisManager
 
 redis_db = RedisManager(host="localhost", port=6379)
+```
 
-# set data
+Set data
+```
 redis_key = "chat_key"
 chat_memory = [
     {
       "role": "system",
       "content": "Assistant is a large language model trained by OpenAI."
     },
     {
@@ -38,29 +43,30 @@
       "content": "hi"
     },
 ]
 redis_db.set_data(redis_key, chat_memory)
 
 ```
 
-```
-# get data
 
+Get data
+```
 chat_history = redis_db.get_data(redis_key)
 
 ```
 
+Truncate history(conversation)
 ```
-# truncate history(conversation)
+# You can choose whether to update the Redis database or 
+# not by specifying the 'overwrite' parameter (boolean).
 
-# You can choose whether to update the Redis database or not by specifying the 'overwrite' parameter (boolean)."
-redis_db.truncate_conversation(redis_key, overwrite=True)
+data = redis_db.truncate_conversation(redis_key, overwrite=True)
 
 ```
 
 ### Use with FastAPI Swagger
 `cd examples/chatbot`
 1. Get your `OpenAI` API key [here](https://platform.openai.com/overview).
 2. Copy env.example .env (set fastapi webserver workers and openai api key)
     `cp env.example .env`
-3. docker-compose up -d
-4. http://0.0.0.0:8012/docs
+3. `docker-compose up -d`
+4. check out : `http://0.0.0.0:8012/docs`
```

### Comparing `redis_chatgpt-0.1.1/setup.py` & `redis_chatgpt-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 project_urls = {
   'Github': 'https://github.com/ElmiraGhorbani/redis-chatgpt',
 }
 
 setup(
     name='redis_chatgpt',
-    version='0.1.1',
+    version='0.1.2',
     author='Elmira Ghorbani',
     description='A user-friendly package designed to save chat history conversation and truncate conversation if user exceeds max token when using OpenAI chat completion.',
     packages=find_packages(),
     install_requires=[
         'redis>=4.6.0'
     ],
     project_urls=project_urls,
```

