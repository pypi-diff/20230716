# Comparing `tmp/vector_vault-2.0.7.tar.gz` & `tmp/vector_vault-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.7.tar", last modified: Sat Jun 10 04:18:06 2023, max compression
+gzip compressed data, was "vector_vault-2.1.0.tar", last modified: Sun Jul 16 05:53:47 2023, max compression
```

## Comparing `vector_vault-2.0.7.tar` & `vector_vault-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-10 04:18:06.337669 vector_vault-2.0.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    19254 2023-06-10 04:18:06.337479 vector_vault-2.0.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    18529 2023-06-10 00:06:46.000000 vector_vault-2.0.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-10 04:18:06.337707 vector_vault-2.0.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-10 04:17:45.000000 vector_vault-2.0.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-10 04:18:06.333311 vector_vault-2.0.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    19254 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-10 04:18:06.000000 vector_vault-2.0.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-10 04:18:06.337080 vector_vault-2.0.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.0.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1954 2023-06-09 19:11:10.000000 vector_vault-2.0.7/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2398 2023-06-08 04:57:38.000000 vector_vault-2.0.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.7/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    30807 2023-06-09 19:58:53.000000 vector_vault-2.0.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.7/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-16 05:53:47.459117 vector_vault-2.1.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    27260 2023-07-16 05:53:47.458940 vector_vault-2.1.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    26535 2023-07-16 05:51:39.000000 vector_vault-2.1.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-07-16 05:53:47.459203 vector_vault-2.1.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-07-16 05:52:24.000000 vector_vault-2.1.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-16 05:53:47.454665 vector_vault-2.1.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    27260 2023-07-16 05:53:47.000000 vector_vault-2.1.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-07-16 05:53:47.000000 vector_vault-2.1.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-07-16 05:53:47.000000 vector_vault-2.1.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-07-16 05:53:47.000000 vector_vault-2.1.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-07-16 05:53:47.000000 vector_vault-2.1.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-16 05:53:47.458407 vector_vault-2.1.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.0/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3145 2023-06-10 21:41:11.000000 vector_vault-2.1.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2599 2023-07-16 05:00:05.000000 vector_vault-2.1.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16189 2023-06-10 21:42:18.000000 vector_vault-2.1.0/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    36519 2023-07-16 05:13:46.000000 vector_vault-2.1.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.0/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.7/LICENSE` & `vector_vault-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.7/setup.py` & `vector_vault-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.7",
+    version="2.1.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.7/vectorvault/ai.py` & `vector_vault-2.1.0/vectorvault/ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         Use the following Context to answer the Question at the end. 
         Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
         Additional Context: {context}
 
-        Question: {question}
+        Question: {content}
 
         (Answer the question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
         Answer:""" 
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
@@ -101,15 +101,15 @@
                     char_to_take_away = overby * 5
                     context_length = len(context)
                     remove_from_context = int(context_length - char_to_take_away)
                     context = context[-remove_from_context:] 
 
         # Format the prompt
         user_input = history + user_input
-        prompt = prompt_template.format(context=context, history=history, question=user_input)
+        prompt = prompt_template.format(context=context, history=history, content=user_input)
         response = openai.ChatCompletion.create(
             model=model,
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
         )
         return response['choices'][0]['message']['content']
 
@@ -166,15 +166,15 @@
         Use the following Context to answer the Question at the end. 
         Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
         Additional Context: {context}
 
-        Question: {question}
+        Question: {content}
 
         (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
         Answer:""" 
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
@@ -204,15 +204,15 @@
                 if double_check > max_tokens:
                     overby = double_check - max_tokens
                     char_to_take_away = overby * 5
                     context_length = len(context)
                     remove_from_context = int(context_length - char_to_take_away)
                     context = context[-remove_from_context:] 
 
-        prompt = prompt_template.format(context=context, history=history, question=user_input)
+        prompt = prompt_template.format(context=context, history=history, content=user_input)
         user_input = history + user_input
         response = openai.ChatCompletion.create(
             model=model,
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
             stream=True
         )
```

### Comparing `vector_vault-2.0.7/vectorvault/cloud_api.py` & `vector_vault-2.1.0/vectorvault/cloud_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import requests
+from typing import List, Dict
 
 base_url = 'https://register.vectorvault.io'
 
-def register(first_name: str, last_name: str, email: str, password: str) -> dict:
+def register(first_name: str, last_name: str, email: str, password: str, tags: List[Dict[str, str]]) -> dict:
     '''
         Registers a new user:
         
         response = register('John', 'Smith', 'johnsmith@gmail.com', 'password')
         print(response)
     '''
-
     headers = {
         'Authorization': 'expected_authorization_code'  # replace with your actual authorization code
     }
     data = {
         'first': first_name,
         'last': last_name,
         'email': email,
-        'password': password
+        'password': password,
+        'tags': tags  # include the tags as part of the request data
     }
-    response = requests.post(f'{base_url}/register', headers=headers, data=data)
+    response = requests.post(f'{base_url}/register', headers=headers, json=data)  # use json=data instead of data=data
 
     if response.status_code != 200:
         return {'error': response.text}
 
     return response.json()
```

### Comparing `vector_vault-2.0.7/vectorvault/cloudmanager.py` & `vector_vault-2.1.0/vectorvault/cloudmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault. See license for consent.
 
 import tempfile
 import os
 import json
-from .creds import CustomCredentials
-from .vecreq import call_proj
-from .itemize import cloud_name
+from creds import CustomCredentials
+from vecreq import call_proj
+from itemize import cloud_name
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = user
         self.api = api_key
```

### Comparing `vector_vault-2.0.7/vectorvault/creds.py` & `vector_vault-2.1.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.7/vectorvault/download.py` & `vector_vault-2.1.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.7/vectorvault/itemize.py` & `vector_vault-2.1.0/vectorvault/itemize.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 # herein are proprietary to Vector Vault
 # and its suppliers and may be covered by U.S. and Foreign Patents,
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault. See license for consent.import datetime 
 
-from .vecreq import call_name_vecs, call_buildpath
+from vecreq import call_name_vecs, call_buildpath
 from annoy import AnnoyIndex
 import threading
 from copy import deepcopy
+import datetime
 
 def itemize(vault, x, meta=None, text=None, name=None):
     meta = deepcopy(meta) if meta else {}
     if 'name' not in meta and name is not None:
         meta['name'] = name
     elif name is None:
         meta['name'] = f'{vault}-{x}'
@@ -66,13 +67,20 @@
 
 def get_item(item):
     item_id = item["meta"]["item_id"]
     item_text = item["text"]
     item_meta = item["meta"]
     return item_text, item_id, item_meta
 
-def build_return(results, item_data, meta):
-    result = {
-        "data": item_data,
-        "metadata": meta
-    }
-    results.append(result)
+def build_return(results, item_data, meta, distance=None):
+    if not distance:
+        result = {
+            "data": item_data,
+            "metadata": meta
+        }
+    else:
+        result = {
+            "data": item_data,
+            "metadata": meta,
+            "distance": distance
+        }
+    results.append(result)
```

### Comparing `vector_vault-2.0.7/vectorvault/tools_gpt.py` & `vector_vault-2.1.0/vectorvault/tools_gpt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .ai import AI
+from ai import AI
+import time
 
 '''
     ToolsGPT is a set of tools special to large language models. 
     Every tool turns subjectivity into objectivity.
     
     Objectivity is needed for code. 
     Subjectivity is the primary human input.
@@ -32,27 +33,32 @@
 '''
 
 class ToolsGPT():
     def __init__(self, verbose=False):
         self.verbose = verbose
         self.llm = AI().llm
 
-    def get_rating(self, text: str, concept_to_rate_for: str = 'Quality', model='gpt-3.5-turbo', custom_prompt=False, loop_limit=20) -> int:
+    def get_rating(self, text: str = None, concept_to_rate_for: str = None, model='gpt-3.5-turbo', loop_limit=20) -> int:
         '''
-            Get a numeric rating out of 10. Input plain text, and optionally include a concept to rate for
-            Concept can be a comparison, or skill, or anything 
-            Output is integer
-        '''
-        prompt_template = custom_prompt if custom_prompt else """Rate the following content 1 - 10. Respond only with a number in integer format.
-        Concept to rate out of ten for: {concept_to_rate_for}
-        User: Content to classify out of 10: "{content}" \n\n Reponse: Since I am not allowed to give any explination before or after my rating, I'd like to say
-        that this number has been carefully considered given your content. My rating out of 10 integer is: """
-        prompt = prompt_template.format(concept_to_rate_for=concept_to_rate_for, content=text)
-
-        answer = self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
+            Get a numeric rating out of 10. Input plain text, and concept to rate for. Defualts to 'quality'
+            Output is integer. Leave no text and pass concept only to format custom
+        '''
+        if text:
+            prompt_template = """Rate the following content 1 - 10. Respond only with a number in integer format.
+            Concept to rate out of ten for: {concept_to_rate_for}
+            User: Content to classify out of 10: "{content}" \n\n Reponse: Since I am not allowed to give any explination before or after my rating, I'd like to say
+            that this number has been carefully considered given your content. My rating out of 10 integer is: """
+            prompt = prompt_template.format(concept_to_rate_for=concept_to_rate_for, content=text)
+        else:
+            prompt_template = """Rate the following content 1 - 10. Respond only with a number in integer format.
+            Concept to rate out of ten for: {concept_to_rate_for} \n\n Reponse: Since I am not allowed to give any explination before or after my rating, I'd like to say
+            that this number has been carefully considered given your concept. My rating out of 10 integer is: """
+            prompt = prompt_template.format(concept_to_rate_for=concept_to_rate_for)
+        
+        answer = self.retry_llm(custom_prompt=prompt, model=model)
         if self.verbose == True:
             print(f"'Rating Initial Answer: {answer}")
 
         try:
             answer = int(answer)
         except:
             loops = 0
@@ -65,116 +71,115 @@
                 loops += 1
                 try:
                     answer = int(answer)
                     break
                 except:
                     pass
 
-        # internal function to objectify
-        def get_number(self, text: str, model='gpt-3.5-turbo', custom_prompt=False):
-            prompt_template = custom_prompt if custom_prompt else """Respond only with a number in integer format... 
-            Example content: 'The number I would give to this is a 7 out of 10.' Example answer: '7' 
-            Example content 2: 'This is level 5 of sales quality' Example answer 2: '5' 
-            Example content 3: 'This s good, but could be better. I would rate this as an 8 out of 10.' Example answer 3: '8'\n
-            User: The following content should be a number between 1 & 10 - Content: "{content}" 
-            \n\nResponse: The number is: """
-            prompt = prompt_template.format(content=text)
-
-            return self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
+            # internal function to get integer 
+            def get_number(self, text: str, model='gpt-3.5-turbo', loop_limit=5):
+                prompt_template = """Respond only with a number in integer format... 
+                Example content: 'The number I would give to this is a 7 out of 10.' Example answer: '7' 
+                Example content 2: 'This is level 5 of sales quality' Example answer 2: '5' 
+                Example content 3: 'This s good, but could be better. I would rate this as an 8 out of 10.' Example answer 3: '8'\n
+                User: The following content should be a number between 1 & 10 - Content: "{content}" 
+                \n\nResponse: The number is: """
+                prompt = prompt_template.format(content=text)
+
+                response = self.retry_llm(custom_prompt=prompt, model=model, loop_limit=loop_limit)
+                if self.verbose: 
+                    print("Extracted Number: ", response)
+                return response
             
         return answer
         
 
-    def get_yes_no(self, text: str, question: str, model='gpt-3.5-turbo', custom_prompt=False, loop_limit=20) -> str:
+    def get_yes_no(self, text: str, question: str, model='gpt-3.5-turbo', loop_limit=20) -> str:
         '''
             Get an exact "yes" or "no" to any question, given an input. 
             Be sure to input text to get a yes or no to, then ask the question to answer
         '''
-        answer = self.yay_or_nay(text, question, model=model, custom_prompt=custom_prompt)
+        answer = self.yay_or_nay(text, question, model=model)
         if self.verbose == True:
             print(f"Y/N Initial Answer: {answer}")
 
-        if answer == 'yes' or answer == 'no':
-            pass
-        else:
-            loops = 0
-            while True:
-                if loops >= loop_limit:
-                    break
-                answer = self.isolate_yes_no(answer)
-                if self.verbose == True:
-                    print(f"Y/N Answer {loops}: {answer}")
-                loops += 1
-                if answer == 'yes' or answer == 'no':
-                    break
-            
+        loops = 0
+        while loops < loop_limit and answer not in ['yes', 'no']:
+            answer = self.isolate_yes_no(answer)
+            if self.verbose:
+                print(f"Y/N Answer {loops}: {answer}")
+            loops += 1
+
         return answer
 
+    def get_binary(self, text: str, zero_if: str, one_if: str, model='gpt-3.5-turbo', loop_limit=20) -> str:
+        '''
+            Get an exact "0" or "1" to any question, given an input. 
+            Input text to get a decision on, then tell why to pick 0 and why to pick 1. 
+            Prompt starts with "Repond '0' if"...
+        '''
+        answer = self.zero_or_one(text, zero_if, one_if, model=model)
+        if self.verbose == True:
+            print(f"0/1 Initial Answer: {answer}")
+
+        loops = 0
+        while loops < loop_limit and int(answer) not in [0, 1]:
+            answer = self.isolate_zero_one(answer)
+            if self.verbose:
+                print(f"0/1 Answer {loops}: {answer}")
+            loops += 1
+            
+        return answer
 
-    def get_match(self, text: str, list_of_options: list, model='gpt-3.5-turbo', custom_prompt=False, loop_limit=20) -> str:
+    def get_match(self, text: str, list_of_options: list, model='gpt-3.5-turbo', loop_limit=4) -> str:
         '''
-            This function could be used in a variety of Natural Language Processing (NLP) tasks, 
-            such as text classification or intent recognition.
+        This function could be used in a variety of Natural Language Processing (NLP) tasks, 
+        such as text classification or intent recognition.
 
-            Classify any text input to a single option contained in a list of options. - Returns exact match to one of items on list.
-            Input text, and list of answers: ["list of answers", "is a list of strings", "do not forget"]
+        Classify any text input to a single option contained in a list of options. - Returns exact match to one of items on list.
+        Input text, and list of answers: ["list of answers", "is a list of strings", "do not forget"]
         '''
+
         list_copy = []
         for option in list_of_options:
             list_copy.append(option.strip().replace('.', '').lower().strip('"').strip("'"))
-        prompt_template = custom_prompt if custom_prompt else """Respond with one of the options on this list: {list_of_options} 
+        prompt_template = """Respond with one of the options on this list: {list_of_options} 
         Content to classify: "{content}"  \n\n Classifiy the content above into one of the following options: {list_of_options}"""
-
         prompt = prompt_template.format(content=text, list_of_options=list_copy)
 
-        answer = self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
-        if self.verbose == True:
-            print(f"Get Answer Initial Answer: {answer}")
+        answer = self.retry_llm_in_list(prompt, list_copy, model, loop_limit)
 
-        loops = 0
-        while answer not in list_copy:
-            loops += 1
-            answer = self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
-            if self.verbose == True:
-                print(f"Answer {loops}: {answer}")
-            if loops >= loop_limit:
-                break
+        if self.verbose:
+            print(f"Get Answer: {answer}")
 
-        answer = list_of_options[list_copy.index(answer)] # return original answer
-        
-        return answer
+        if answer is not None:
+            answer = list_of_options[list_copy.index(answer)]  # return original answer
 
+        return answer
 
-    def get_topic(self, text: str, list_of_options: list, model='gpt-3.5-turbo', custom_prompt=False, loop_limit=20) -> str:
+    def get_topic(self, text: str, list_of_options: list, model='gpt-3.5-turbo', loop_limit=4) -> str:
         '''
-            Like get_match, default optimized for topic recognition
+        Like get_match, default optimized for topic recognition
         '''
+
         list_copy = []
         for option in list_of_options:
             list_copy.append(option.strip().replace('.', '').lower().strip('"').strip("'"))
-        prompt_template = custom_prompt if custom_prompt else """Respond with one of the options on this list: {list_of_options} 
+        prompt_template = """Respond with one of the options on this list: {list_of_options} 
         Content to classify: "{content}"  \n\nClassifiy the content above based on which topic it is mostly related to one topic: {list_of_options}"""
-
         prompt = prompt_template.format(content=text, list_of_options=list_copy)
 
-        topic = self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
-        if self.verbose == True:
-            print(f"Topic Initial Answer: {topic}")
+        topic = self.retry_llm_in_list(prompt, list_copy, model, loop_limit)
+
+        if self.verbose:
+            print(f"Topic Answer: {topic}")
+
+        if topic is not None:
+            topic = list_of_options[list_copy.index(topic)]  # return original topic
 
-        loops = 0
-        while topic not in list_copy:
-            loops += 1
-            topic = self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
-            if self.verbose == True:
-                print(f"Topic Answer {loops}: {topic}")
-            if loops >= loop_limit:
-                break
-        
-        topic = list_of_options[list_copy.index(topic)] # return original topic
-        
         return topic
 
 
     def match_or_make(self, text, list_of_options: list = [], model='gpt-3.5-turbo', loop_limit=20) -> str:
         ''' 
             "M&M" Returns exact match or new option. Input text and list_of_options. 
             If no list is input, then one will be made and be output
@@ -219,57 +224,95 @@
     # internal function 
     def make_option(self, text, list_of_options: list, model='gpt-3.5-turbo') -> str:
         prompt_template = """Content to classify: "{content}"  \n\n
         Create a new category for the content based on these other categories in this list: {list_of_options}"""
 
         prompt = prompt_template.format(content=text, list_of_options=list_of_options)
 
-        return self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
+        return self.retry_llm(custom_prompt=prompt, model=model)
 
     # internal function 
     def make_option_from_zero(self, text, model='gpt-3.5-turbo'):
         '''
             Option without anything to go off of but the text input
         '''
         prompt_template = """Given the following content: {content} 
         Make a simple and general category to classify content like this. Respond only with the category, and 
         no explination before or after, just the name of the catagory. \n\nThe name of the category is: """
         
         prompt = prompt_template.format(content=text)
 
-        return self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
+        return self.retry_llm(custom_prompt=prompt, model=model)
     
     # internal function 
     def finalize_category(self, text, prev_answer):
         prompt_template = """Given the following category suggestion: "{prev_answer}"
         \nand this text: "{text}" The final and simple one or two word category name I created for it is: """
         
         prompt = prompt_template.format(prev_answer=prev_answer, text=text)
 
-        return self.llm(custom_prompt=prompt).strip().replace('.', '').lower().strip('"').strip("'")
+        return self.retry_llm(custom_prompt=prompt)
 
     # internal function 
-    def isolate_yes_no(self, content, question: str, model='gpt-3.5-turbo', custom_prompt=False):
+    def isolate_yes_no(self, content, question: str, model='gpt-3.5-turbo'):
         '''Not recommended for external use. Internal function'''
-        prompt_template = custom_prompt if custom_prompt else """Do not respond with anything before the yes or no. Do not add anything after the "yes" or "no". 
+        prompt_template = """Do not respond with anything before the yes or no. Do not add anything after the "yes" or "no". 
         Example question 1: 'Is the Eiffel tower located in Paris?' Example answer 1: 'Yes' Example question 2: 'Do you think I am fat?' 
         Example answer 2: 'No' Example question 3: 'Should I use Matplotlib in Python to draw a graph of csv information I have' Example answer 3: 'Yes'
         Example question 4: 'As an ai language model, I can't tell you yes or no, but I it does have a tendency to work sometimes.' Example answer 4: 'Yes'
         Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: 'No'
         \n\nRespond with a "yes" or "no" to following: "{question}"  """
 
         prompt = prompt_template.format(content=content, question=question)
 
-        return self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
+        return self.retry_llm(custom_prompt=prompt, model=model)
     
-    def yay_or_nay(self, content, question: str, model='gpt-3.5-turbo', custom_prompt=False):
+    def yay_or_nay(self, content, question: str, model='gpt-3.5-turbo'):
         '''Not recommended for external use. Internal function'''
-        prompt_template = custom_prompt if custom_prompt else """Do not respond with anything before the yes or no. Do not add anything after the "yes" or "no". 
+        prompt_template = """Do not respond with anything before the yes or no. Do not add anything after the "yes" or "no". 
         Example question 1: 'Is the Eiffel tower located in Paris?' Example answer 1: 'Yes' Example question 2: 'Do you think I am fat?' 
         Example answer 2: 'No' Example question 3: 'Should I use Matplotlib in Python to draw a graph of csv information I have' Example answer 3: 'Yes'
         Example question 4: 'As an ai language model, I can't tell you yes or no, but I it does have a tendency to work sometimes.' Example answer 4: 'Yes'
         Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: 'No'
         \n\nGiven this content: "{content}", Respond with a "yes" or "no" to following question: "{question}"  """
 
         prompt = prompt_template.format(content=content, question=question)
 
-        return self.llm(custom_prompt=prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
+        return self.retry_llm(custom_prompt=prompt, model=model)
+    
+    def zero_or_one(self, content, zero_if: str, one_if: str, model='gpt-3.5-turbo'):
+        '''Not recommended for external use. Internal function'''
+        prompt_template = """Do not respond with anything before the 1 or 0. Do not add anything after the "1" or "0". 
+        Example question 1: 'Is the Eiffel tower located in Paris?' Example answer 1: '1' Example question 2: 'Do you think I am fat?' 
+        Example answer 2: '0' Example question 3: 'Should I use Matplotlib in Python to draw a graph of csv information I have' Example answer 3: '1'
+        Example question 4: 'As an ai language model, I can't tell you yes or no, but I it does have a tendency to work sometimes.' Example answer 4: '1'
+        Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: '0'
+        \n\nGiven this content: "{content}", Respond with a "0" if {zero_if} \n... or "1" if: "{one_if}"  """
+
+        prompt = prompt_template.format(content=content, zero_if=zero_if, one_if=one_if)
+
+        return self.retry_llm(custom_prompt=prompt, model=model)
+    
+    def isolate_zero_one(self, content, model='gpt-3.5-turbo'):
+        '''Not recommended for external use. Internal function'''
+        prompt_template = """Do not respond with anything before the 1 or 0. Do not add anything after the "1" or "0". 
+        Example question 1: 'Is the Eiffel tower located in Paris?' Example answer 1: '1' Example question 2: 'Do you think I am fat?' 
+        Example answer 2: '0' Example question 3: 'Should I use Matplotlib in Python to draw a graph of csv information I have' Example answer 3: '1'
+        Example question 4: 'As an ai language model, I can't tell you yes or no, but I it does have a tendency to work sometimes.' Example answer 4: '1'
+        Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: '0'
+        \n\nGiven this content: "{content}", Respond with a "0" or "1": """
+
+        prompt = prompt_template.format(content=content)
+
+        return self.retry_llm(custom_prompt=prompt, model=model)
+
+    # This function is called by the others to handle retries:
+    def retry_llm(self, custom_prompt, model='gpt-3.5-turbo', loop_limit=5):
+        for i in range(loop_limit):
+            try:
+                return self.llm(custom_prompt=custom_prompt, model=model).strip().replace('.', '').lower().strip('"').strip("'")
+            except Exception as e:
+                if i < loop_limit - 1:  # i is zero indexed
+                    time.sleep(5)  # wait 5 seconds before trying again
+                    print(f"Attempt {i+1} failed with error: {str(e)}. Retrying...")
+                else:
+                    raise f"Attempt {i+1} failed with error: {str(e)}. No more retries."
```

### Comparing `vector_vault-2.0.7/vectorvault/vault.py` & `vector_vault-2.1.0/vectorvault/vault.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 import os
 import time
 import re
 import openai
 import json
 import traceback
 from concurrent.futures import ThreadPoolExecutor
-from .cloudmanager import CloudManager
-from .ai import AI
-from .itemize import itemize, name_vecs, get_item, get_vectors, build_return, cloud_name
-from .vecreq import call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
-from .tools_gpt import ToolsGPT
+from cloudmanager import CloudManager
+from ai import AI
+from itemize import itemize, name_vecs, get_item, get_vectors, build_return, cloud_name
+from vecreq import call_get_total_vectors, call_get_vaults, call_get_similar
+from tools_gpt import ToolsGPT
 
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
@@ -54,21 +54,39 @@
         self.first_run = True
         self.needed_sleep_time = None
         self.saved_already = False
         self.ai = AI()
         self.tools = ToolsGPT(verbose=verbose)
 
     def get_vaults(self, vault: str = None):
+        '''
+            Returns a list of vaults within the current vault directory 
+        '''
         vault = self.vault if vault is None else vault
         return call_get_vaults(self.user, self.api, vault)
 
-    def get_total_vectors(self):
+    def get_total_items(self):
+        '''
+            Returns the total number of vectored items in the Vault
+        '''
         return call_get_total_vectors(self.user, self.vault, self.api)
     
+    def get_distance(self, id1, id2):
+        self.check_index()
+        return self.vectors.get_distance(id1, id2)
+    
+    def get_item_vector(self, item_id):
+        self.check_index()
+        return self.vectors.get_item_vector(item_id)
+    
     def save(self, trees=16):
+        '''
+            Saves all the data added locally to the Cloud Vault. All Vault references are Cloud Vault references, so
+            to add data to the Vault and access it later, you must call add(), then get_vectors(), then save().
+        '''
         if self.saved_already == True:
             self.clear_cache()
             print("The last save was aborted before build finished. Clearing cache to start again...")
         self.saved_already = True
         start_time = time.time()
         self.vectors.build(trees)
 
@@ -90,30 +108,39 @@
         self.vecs_loaded = False
         self.saved_already = False
 
         if self.verbose:
             print(f"upload time --- {(time.time() - start_time)} seconds --- {total_saved_items} items saved")
             
     def clear_cache(self):
+        '''
+            Clears the cache for all the loaded items 
+        '''
         self.reload_vectors()
         self.x_checked = True
         self.vecs_loaded = True
         self.saved_already = False
 
     def delete(self):
+        '''
+            Deletes the entire Vault and all contents
+        '''
         if self.verbose == True:
             print('Deleting started. Note: this can take a while for large datasets')
         # Clear the local vector data
         self.vectors = get_vectors(self.dims)
         self.items.clear()
         self.x = 0
         self.cloud_manager.delete()
         print('Vault deleted')
 
     def check_index(self):
+        '''
+            Internal function use only
+        '''
         start_time = time.time()
         if self.cloud_manager.vault_exists(name_vecs(self.vault, self.user, self.api)):
             if self.vecs_loaded == False:
                 self.load_vectors()
             num_existing_items = self.vectors.get_n_items()
             new_index = get_vectors(self.dims)
             for i in range(num_existing_items):
@@ -125,32 +152,41 @@
             pass
         
         self.x_checked = True
         if self.verbose == True:
             print("initialize index --- %s seconds ---" % (time.time() - start_time))
     
     def reload_vectors(self):
-            num_existing_items = self.vectors.get_n_items()
-            new_index = get_vectors(self.dims)
-            for i in range(num_existing_items):
-                vector = self.vectors.get_item_vector(i)
-                new_index.add_item(i, vector)
-            self.x = i + 1
-            self.vectors = new_index
+        '''
+            Internal function 
+        '''
+        num_existing_items = self.vectors.get_n_items()
+        new_index = get_vectors(self.dims)
+        for i in range(num_existing_items):
+            vector = self.vectors.get_item_vector(i)
+            new_index.add_item(i, vector)
+        self.x = i + 1
+        self.vectors = new_index
 
     def load_vectors(self):
+        '''
+            Internal function 
+        '''
         start_time = time.time()
         temp_file_path = self.cloud_manager.download_to_temp_file(name_vecs(self.vault, self.user, self.api))
         self.vectors.load(temp_file_path)
         os.remove(temp_file_path)
         self.vecs_loaded = True
         if self.verbose:
             print("get load vectors --- %s seconds ---" % (time.time() - start_time))
 
     def split_text(self, text, min_threshold=1000, max_threshold=16000):
+        '''
+            Internal function 
+        '''
         segments = []
         sentence_spans = list(re.finditer(r"(?<=[.!?])\s+", text))
 
         current_segment = []
         current_length = 0
 
         sentence_start = 0
@@ -180,72 +216,137 @@
             segments.append(" ".join(current_segment))
 
         if self.verbose == True:
             print(f'New text chunk of size: {len(current_segment)}') 
 
         return segments
     
-    def get_items_by_vector(self, vector, n: int = 4):
+    def get_items(self, ids: list = []) -> list:
+        '''
+            Get any items from the Vault. Input the item id(s) in a list. 
+            - Example Single Item Usage:
+                item = vault.get_items([132])
+
+            - Example Multi-Item Usage:
+                items = vault.get_items([132, 128, 393, 74, 644, 71])
+        '''
         self.load_vectors()
         start_time = time.time()
 
-        results = []
-        vecs = self.vectors.get_nns_by_vector(vector, n)
-        for vec in vecs:
+        for i in ids:
+            results = []
             # Retrieve the item
-            item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, vec, item=True))
+            item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, i, self.user, self.api, item=True))
             # Retrieve the metadata
-            meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, vec, meta=True))
+            meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, i, self.user, self.api, meta=True))
             meta = json.loads(meta_data)
             build_return(results, item_data, meta)
-
-        if self.verbose == True:
-            print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
+            if self.verbose == True:
+                print(f"get {len(ids)} items back --- %s seconds ---" % (time.time() - start_time))
 
         return results
     
-    def get_similar_local(self, text, n: int = 4):
+    def get_items_by_vector(self, vector, n: int = 4, include_distances=False):
+        '''
+            Internal function that returns vector similar items. Requires input vector, returns similar items
+        '''
+        self.load_vectors()
+        start_time = time.time()
+
+        if not include_distances:
+            results = []
+            vecs = self.vectors.get_nns_by_vector(vector, n)
+            for vec in vecs:
+                # Retrieve the item
+                item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, vec, self.user, self.api, item=True))
+                # Retrieve the metadata
+                meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, vec, self.user, self.api, meta=True))
+                meta = json.loads(meta_data)
+                build_return(results, item_data, meta)
+                if self.verbose == True:
+                    print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
+
+            return results
+        else:
+            results = []
+            vecs, distances = self.vectors.get_nns_by_vector(vector, n, include_distances=include_distances)
+            counter = 0
+            for vec in vecs:
+                # Retrieve the item
+                item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, vec, self.user, self.api, item=True))
+                # Retrieve the metadata
+                meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, vec, self.user, self.api, meta=True))
+                meta = json.loads(meta_data)
+                build_return(results, item_data, meta, distances[counter])
+                counter+=1
+                if self.verbose == True:
+                    print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
+
+            return results
+
+    def get_similar_local(self, text, n: int = 4, include_distances=False):
+        '''
+            Returns similar items from the Vault as the one you entered, but locally
+        '''
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
-        return self.get_items_by_vector(self.user, self.vault, self.api, vector, n)
+        return self.get_items_by_vector(vector, n, include_distances=include_distances)
     
-    def get_similar(self, text, n: int = 4):
-        return call_get_similar(self.user, self.vault, self.api, text, n)
+    def get_similar(self, text, n: int = 4, include_distances=False):
+        '''
+            Returns similar items from the Vault as the text you enter.
+            Sample print out when called:
+            `[{'data': 'Using Cloud Storage
+            with Cloud Run requires some techniques...', 
+            'metadata': {'name': '', 'item_id': 1, 'created_at':
+            '2023-07-16T04:29:00.730754', 'updated_at': '2023-07-16T04:29:00.730758'},
+            'distance': 0.7101698517799377}]`
+
+            (Usually there are four items, but in this sample print out, we have removed the other 3 
+            and shortened this one's data for brevity)
+
+            This sample was called with "include_distances=True", which adds the "distance" field to the return.
+            The distance can be useful for assessing similarity differences in the items returned. 
+            Each item has its' own distance number.
+
+
+        '''
+        return call_get_similar(self.user, self.vault, self.api, text, n, include_distances=include_distances)
 
     def add_item(self, text: str, meta: dict = None, name: str = ''):
         """
-            If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
+            If your text length is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         if self.x_checked == False:
             self.check_index()
         else: 
             pass
         
         new_item = itemize(self.vault, self.x, meta, text, name)
         self.items.append(new_item)
         self.x += 1
 
     def add(self, text: str, meta: dict = None, name: str = '', split=False, split_size=1000):
         """
-            If your text length lenght is greater than 4000 tokens, Vault.split_text(your_text)  
+            If your text length is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
 
         if len(text) > 15000 or split == True:
             if self.verbose == True:
                 print('Using the built-in "split_text()" function to get a list of texts') 
             texts = self.split_text(text, min_threshold=split_size) # returns list of text segments
         else:
             texts = [text]
         for text in texts:
             self.add_item(text, meta, name)
 
     def add_item_with_vector(self, text: str, vector: list, meta: dict = None, name: str = None):
         """
-            If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
+            If your text length is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         if self.x_checked == False:
             self.check_index()
         else: 
             pass
         start_time = time.time()
@@ -259,14 +360,17 @@
 
         self.x += 1
 
         if self.verbose == True:
             print("add item time --- %s seconds ---" % (time.time() - start_time))
 
     def process_batch(self, batch_text_chunks, never_stop, loop_timeout):
+        '''
+            Internal function
+        '''
         loop_start_time = time.time()
         exceptions = 0
         while True:
             try:
                 res = openai.Embedding.create(input=batch_text_chunks, engine="text-embedding-ada-002")
                 break
             except Exception as e:
@@ -280,14 +384,17 @@
                         if exceptions >= 5:
                             print(f"API Failed too many times, exiting loop: {e}.")
                             break
                         raise TimeoutError("Loop timed out")
         return [record['embedding'] for record in res['data']]
 
     def get_vectors(self, batch_size: int = 32, never_stop: bool = False, loop_timeout: int = 180):
+        '''
+            Takes text data added to the vault, and gets vectors for them
+        '''
         start_time = time.time()
         if not self.last_time:
             self.last_time = start_time - 1
         
         if not self.needed_sleep_time:
             self.needed_sleep_time = 0
         
@@ -345,70 +452,79 @@
 
     def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, custom_prompt=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
-            Example Signle Usage: 
+            - Example Signle Usage: 
             `response = vault.get_chat(text)`
 
-            Example Chat: 
+            - Example Chat: 
             `response = vault.get_chat(text, chat_history)`
             
-            Example Summary: 
+            - Example Summary: 
             `summary = vault.get_chat(text, summary=True)`
 
-            Example Context-Based Response:
+            - Example Context-Based Response:
             `response = vault.get_chat(text, get_context = True)`
 
-            Example Context-Based Response w/ Chat History:
+            - Example Context-Based Response w/ Chat History:
             `response = vault.get_chat(text, chat_history, get_context = True)`
 
-            Example Context-Response with Context Samples Returned:
+            - Example Context-Response with Context Samples Returned:
             `vault_response = vault.get_chat(text, get_context = True, return_context = True)`
             
             Response is a string, unless return_context == True, then response will be a dictionary 
 
-            Example to print dictionary results:
+            - Example to print dictionary results:
             # print response:
             `print(vault_response['response'])` 
 
             # print context:
             for item in vault_response['context']['results']:
                 print("\n\n", f"item {item['metadata']['item_index']}")
                 print(item['data'])
 
-            Default `expansion = False` can be set to True to create additional context from user input for vector retrieval. Allowing for greater search accuracy if
-            user input is too short or lacks the specificity needed for a quality retrieval search. ('expansion' is not context-aware). Default is good.
-
             history_search is False by default skip adding the history of the conversation to the text input for similarity search (useful if history contains subject infomation useful for answering the new text input and the text input doesn't contain that info)
-        
-            custom_prompt overrides the stock prompt. Check out the prompts in ai.py to see more. 
-            `llm` and `llm_stream` models manage history internally, so the input is the only part that needs formatting. 
-            example for generic chat: 
-            custom_prompt = """
-                Answer this question as if you were a financial advisor: "{content}". 
-            """
+            
+            - Example Custom Prompt:
+            `response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)`
+
+            `custom_prompt` overrides the stock prompt we provide. Check ai.py to see the originals we provide. 
+            `llm` and `llm_stream` models manage history internally, so the `content` is the only variable to be included and formattable in the prompt. 
+
+            *Example WIHTOUT Vault Context:*
+
+            ```python
+            my_prompt = """Answer this question as if you were a financial advisor: "{content}". """
+            response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)
+            ```
 
-            The `llm_w_context` and `llm__w_context_stream` models for retrieval inject the history, context, and user input all in one prompt.
-            example for Vault chat - 
+            Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
+            `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
+
+            *Example WITH Vault Context:*  
+            ```python
             custom_prompt = """
                 Use the following Context to answer the Question at the end. 
                 Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
                 Chat History (if any): {history}
 
                 Additional Context: {context}
 
                 Question: {question}
 
                 (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
                 Answer:
             """ 
+            response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)
+            ```
+
         '''
 
         start_time = time.time()
         if not self.last_chat_time:
             self.last_chat_time = start_time - 20
         
         if not self.needed_sleep_time:
@@ -489,65 +605,76 @@
         if return_context == False:
             return response
         elif return_context == True:
             return {'response': response, 'context': context}
         
     def get_chat_stream(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False, custom_prompt=False):
         '''
-            This streams. Example: vault.print_stream(vault.get_chat_stream(text))
             Always use this get_chat_stream() wrapped by either print_stream(), or cloud_stream().
-            cloud_stream() is for cloud functions, like a flask app, serving a front end elsewhere
+            cloud_stream() is for cloud functions, like a flask app serving a front end elsewhere.
             print_stream() is for local console printing
 
-            Example Signle Usage: 
+            - Example Signle Usage: 
             `response = vault.print_stream(vault.get_chat_stream(text))`
 
-            Example Chat: 
+            - Example Chat: 
             `response = vault.print_stream(vault.get_chat_stream(text, chat_history))`
             
-            Example Summary: 
+            - Example Summary: 
             `summary = vault.print_stream(vault.get_chat_stream(text, summary=True))`
 
-            Example Context-Based Response:
+            - Example Context-Based Response:
             `response = vault.print_stream(vault.get_chat_stream(text, get_context = True))`
 
-            Example Context-Based Response w/ Chat History:
+            - Example Context-Based Response w/ Chat History:
             `response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True))`
 
-            Example Context-Response with Context Samples Returned:
+            - Example Context-Response with Context Samples Returned:
             `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True))`
 
-            Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
+            - Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
             `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
             
-            Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
+            - Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
             `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
             
-            custom_prompt overrides the stock prompt. Check out the prompts in ai.py to see more. 
-            `llm` and `llm_stream` models manage history internally, so the input is the only part that needs formatting. 
-            example for generic chat: 
-            custom_prompt = """
-                Answer this question as if you were a financial advisor: "{content}". 
-            """
 
-            The `llm_w_context` and `llm__w_context_stream` models for retrieval inject the history, context, and user input all in one prompt.
-            example for Vault chat - 
+            - Example Custom Prompt:
+            `response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)`
+
+            `custom_prompt` overrides the stock prompt we provide. Check ai.py to see the originals we provide. 
+            `llm` and `llm_stream` models manage history internally, so the `content` is the only variable to be included and formattable in the prompt. 
+
+            *Example WIHTOUT Vault Context:*
+
+            ```python
+            my_prompt = """Answer this question as if you were a financial advisor: "{content}". """
+            response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True, custom_prompt=my_prompt))
+            ```
+
+            Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
+            `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
+
+            *Example WITH Vault Context:*  
+            ```python
             custom_prompt = """
                 Use the following Context to answer the Question at the end. 
                 Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
                 Chat History (if any): {history}
 
                 Additional Context: {context}
 
                 Question: {question}
 
                 (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
                 Answer:
             """ 
+            response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True, custom_prompt=my_prompt))
+            ```
         '''
 
         start_time = time.time()
         if not self.last_chat_time:
             self.last_chat_time = start_time - 20
         
         if not self.needed_sleep_time:
@@ -646,14 +773,17 @@
                      
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
     def print_stream(self, function, printing=True):
+        '''
+            For local use printing the chat stream. Call 'printing=False' for no pretty printing to be applied
+        '''
         full_text= ''
         newlinetime=1
         for word in function:
             if word != '!END':
                 full_text += word
                 if printing == True:
                     if len(full_text) / 80 > newlinetime:
@@ -661,9 +791,12 @@
                         print(f'\n{word}', end='', flush=True)
                     else:
                         print(word, end='', flush=True) 
             else:
                 return full_text
     
     def cloud_stream(self, function):
+        '''
+            For cloud application yielding the chat stream, like a flask app
+        '''
         for word in function:
             yield f"data: {json.dumps({'data': word})} \n\n"
```

### Comparing `vector_vault-2.0.7/vectorvault/vecreq.py` & `vector_vault-2.1.0/vectorvault/vecreq.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,32 +68,34 @@
         'user': user,
         'vault': vault,
         'api_key': api_key
     }
     response = requests.get(url, params=params)
     return response.json()['total_vectors']
 
-def call_items_by_vector(user, vault, api_key, vector, num_items=4):
+def call_items_by_vector(user, vault, api_key, vector, num_items=4, include_distances=False):
     url = f"https://api.vectorvault.io/items_by_vector"
     payload = {
         'user': user,
         'vault': vault,
         'vector': vector,
+        'include_distances': include_distances,
         'num_items': num_items,
         'api_key': api_key
     }
     response = requests.post(url, json=payload)
     return response.json()['results']
 
-def call_get_similar(user, vault, api_key, text, num_items=4):
+def call_get_similar(user, vault, api_key, text, num_items=4, include_distances=False):
     url = f"https://api.vectorvault.io/get_similar"
     payload = {
         'user': user,
         'vault': vault,
         'api_key': api_key,
+        'include_distances': include_distances,
         'text': text,
         'num_items': num_items
     }
     response = requests.post(url, json=payload)
     return response.json()['results']
```

