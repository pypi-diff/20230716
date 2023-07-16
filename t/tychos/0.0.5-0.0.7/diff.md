# Comparing `tmp/tychos-0.0.5.tar.gz` & `tmp/tychos-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.5.tar", last modified: Mon Jul 10 19:51:46 2023, max compression
+gzip compressed data, was "tychos-0.0.7.tar", last modified: Sun Jul 16 14:20:40 2023, max compression
```

## Comparing `tychos-0.0.5.tar` & `tychos-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.500985 tychos-0.0.5/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.5/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)     2852 2023-07-10 19:51:46.500818 tychos-0.0.5/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)     2665 2023-07-10 19:50:29.000000 tychos-0.0.5/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-10 19:51:46.501026 tychos-0.0.5/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-10 19:49:15.000000 tychos-0.0.5/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.499350 tychos-0.0.5/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.5/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.5/tychos/cli.py
--rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.5/tychos/config.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.500662 tychos-0.0.5/tychos/helpers/
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.5/tychos/helpers/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1554 2023-07-10 19:48:44.000000 tychos-0.0.5/tychos/vector.py
--rw-r--r--   0 abe732     (501) staff       (20)     1734 2023-07-10 19:40:28.000000 tychos-0.0.5/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.500534 tychos-0.0.5/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)     2852 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      330 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/entry_points.txt
--rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/requires.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:20:40.174411 tychos-0.0.7/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.7/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)     2774 2023-07-16 14:20:40.174257 tychos-0.0.7/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)     2587 2023-07-16 14:16:28.000000 tychos-0.0.7/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-16 14:20:40.174448 tychos-0.0.7/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-16 14:16:28.000000 tychos-0.0.7/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:20:40.173125 tychos-0.0.7/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.7/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.7/tychos/cli.py
+-rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.7/tychos/config.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:20:40.174116 tychos-0.0.7/tychos/helpers/
+-rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.7/tychos/helpers/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1557 2023-07-16 14:16:28.000000 tychos-0.0.7/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1745 2023-07-16 14:16:28.000000 tychos-0.0.7/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:20:40.174000 tychos-0.0.7/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)     2774 2023-07-16 14:20:40.000000 tychos-0.0.7/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      330 2023-07-16 14:20:40.000000 tychos-0.0.7/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-16 14:20:40.000000 tychos-0.0.7/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-16 14:20:40.000000 tychos-0.0.7/tychos.egg-info/entry_points.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-16 14:20:40.000000 tychos-0.0.7/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-16 14:20:40.000000 tychos-0.0.7/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.5/LICENSE` & `tychos-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.0.5/PKG-INFO` & `tychos-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.5
+Version: 0.0.7
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
-You can find usage examples for the Tychos Python library in our [BioMed Demo App](https://demo.tychos.ai/) and the [/demo repo folder](https://github.com/tychos-ai/tychos).
-
+To see the Tychos API in action, you can test out our [PubMed Demo App](https://tychos.ai/demo).
 
 ## Installation
 
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
```

### Comparing `tychos-0.0.5/README.md` & `tychos-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
-You can find usage examples for the Tychos Python library in our [BioMed Demo App](https://demo.tychos.ai/) and the [/demo repo folder](https://github.com/tychos-ai/tychos).
-
+To see the Tychos API in action, you can test out our [PubMed Demo App](https://tychos.ai/demo).
 
 ## Installation
 
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
```

### Comparing `tychos-0.0.5/tychos/cli.py` & `tychos-0.0.7/tychos/cli.py`

 * *Files identical despite different names*

### Comparing `tychos-0.0.5/tychos/vector.py` & `tychos-0.0.7/tychos/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import requests
 
 class _Vector:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('TYCHOS_API_KEY')
-        self.base_url = 'https://www.tychos.ai/api/'
+        self.base_url = 'https://www.api.tychos.ai/api/'
         # self.base_url = 'http://localhost:3001/api/'
         
     def create(self, type, input_text, model, model_provider_key=None):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
         if type == "text_embedding":
             if model == "text-embedding-ada-002":
                 try:
-                    url = f'{self.base_url}/create-vector'
+                    url = f'{self.base_url}create-vector'
                     headers = {'api_key': self.api_key}
                     payload = {
                                 'model_provider_key': model_provider_key,
                                 'input': input_text,
                                 'model': model,
                             }
                     response = requests.post(url=url, headers=headers, json=payload)
```

### Comparing `tychos-0.0.5/tychos/vector_data_store.py` & `tychos-0.0.7/tychos/vector_data_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import os
 import requests
 from .vector import _Vector
 
 class VectorDataStore:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('TYCHOS_API_KEY')
-        self.base_url = 'https://www.tychos.ai/api/'
+        self.base_url = 'https://www.api.tychos.ai/api/'
         # self.base_url = 'http://localhost:3001/api/'
         self.vector = _Vector(api_key=self.api_key)
 
     def query(self, name, query_string, limit):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
         # vectorize query string
         query_vector = self.vector.create(
             type="text_embedding",
             input_text=query_string,
             model="text-embedding-ada-002"
         )
 
         # send query request to vector data store
-        url = f'{self.base_url}/query-vector-store'
+        url = f'{self.base_url}query-vector-store'
         headers = {'api_key': self.api_key}
         payload = {
                     'name': name,
                     'query_vector': query_vector,
                     'top': limit,
                 }
         response = requests.post(url=url, headers=headers, json=payload)
+        
 
         # error handling
         response.raise_for_status()
 
         return response.json()
     
     def list(self):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
-        url = f'{self.base_url}/datasets'
+        url = f'{self.base_url}datasets'
         headers = {'api_key': self.api_key}
         response = requests.get(url=url, headers=headers)
 
         # error handling
         response.raise_for_status()
 
         return response.json()
```

### Comparing `tychos-0.0.5/tychos.egg-info/PKG-INFO` & `tychos-0.0.7/tychos.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.5
+Version: 0.0.7
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
-You can find usage examples for the Tychos Python library in our [BioMed Demo App](https://demo.tychos.ai/) and the [/demo repo folder](https://github.com/tychos-ai/tychos).
-
+To see the Tychos API in action, you can test out our [PubMed Demo App](https://tychos.ai/demo).
 
 ## Installation
 
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
```

