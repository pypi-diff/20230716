# Comparing `tmp/llm_inference-0.0.5.dev0.tar.gz` & `tmp/llm_inference-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_inference-0.0.5.dev0.tar", last modified: Thu Jul  6 00:56:35 2023, max compression
+gzip compressed data, was "llm_inference-0.0.6.tar", last modified: Sun Jul 16 15:15:33 2023, max compression
```

## Comparing `llm_inference-0.0.5.dev0.tar` & `llm_inference-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   399922 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/assets/llama-inference-api-min.png
--rw-r--r--   0 runner    (1001) docker     (123)   395880 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/assets/llm-inference-min.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/llm_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.921806 llm_inference-0.0.5.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/src/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/src/chatbot/ui/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/ui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/ui/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/src/llm_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.325827 llm_inference-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-16 15:15:22.000000 llm_inference-0.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-16 15:15:22.000000 llm_inference-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-16 15:15:22.000000 llm_inference-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-16 15:15:22.000000 llm_inference-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-16 15:15:33.325827 llm_inference-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-16 15:15:22.000000 llm_inference-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.321827 llm_inference-0.0.6/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   399922 2023-07-16 15:15:22.000000 llm_inference-0.0.6/assets/llama-inference-api-min.png
+-rw-r--r--   0 runner    (1001) docker     (123)   395880 2023-07-16 15:15:22.000000 llm_inference-0.0.6/assets/llm-inference-min.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.325827 llm_inference-0.0.6/llm_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-16 15:15:33.000000 llm_inference-0.0.6/llm_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-16 15:15:33.000000 llm_inference-0.0.6/llm_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:15:33.000000 llm_inference-0.0.6/llm_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 15:15:33.000000 llm_inference-0.0.6/llm_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 15:15:33.000000 llm_inference-0.0.6/llm_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.325827 llm_inference-0.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 15:15:22.000000 llm_inference-0.0.6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 15:15:22.000000 llm_inference-0.0.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-16 15:15:33.325827 llm_inference-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 15:15:22.000000 llm_inference-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.321827 llm_inference-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.325827 llm_inference-0.0.6/src/llm_chain/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_chain/conversation_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_chain/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_chain/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.325827 llm_inference-0.0.6/src/llm_chain/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_chain/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_chain/ui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:15:33.325827 llm_inference-0.0.6/src/llm_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_inference/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_inference/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_inference/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-16 15:15:22.000000 llm_inference-0.0.6/src/llm_inference/token_manipulation.py
```

### Comparing `llm_inference-0.0.5.dev0/CODE_OF_CONDUCT.md` & `llm_inference-0.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.5.dev0/CONTRIBUTING.md` & `llm_inference-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.5.dev0/LICENSE` & `llm_inference-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.5.dev0/MANIFEST.in` & `llm_inference-0.0.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.5.dev0/PKG-INFO` & `llm_inference-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: llm_inference
-Version: 0.0.5.dev0
-Summary: Large Language Models Inference API and Applications
-Home-page: https://github.com/aniketmaurya/llm-inference
-Author: Aniket Maurya
-Author-email: theaniketmaurya@gmail.com
-License: Apache License 2.0
-Keywords: LLM,LLaMA,GPT,Falcon
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Large Language Model (LLM) Inference API and Chatbot 🦙
 
 ![project banner](https://github.com/aniketmaurya/llm-inference/raw/main/assets/llm-inference-min.png)
 
 Inference API for LLMs like LLaMA and Falcon powered by Lit-GPT from [Lightning AI](https://lightning.ai)
 
 ```
@@ -42,14 +28,49 @@
 path = prepare_weights("EleutherAI/pythia-70m")
 model = LLMInference(checkpoint_dir=path)
 
 print(model("New York is located in"))
 ```
 
 
+## How to use the Chatbot
+
+```python
+from llm_chain import LitGPTConversationChain, LitGPTLLM
+from llm_inference import prepare_weights
+from rich import print
+
+
+path = str(prepare_weights("lmsys/longchat-13b-16k"))
+llm = LitGPTLLM(checkpoint_dir=path, quantize="bnb.nf4")  # 8.4GB GPU memory
+bot = LitGPTConversationChain.from_llm(llm=llm, verbose=True)
+
+print(bot.send("hi, what is the capital of France?"))
+```
+
+## Launch Chatbot App
+
+<video width="320" height="240" controls>
+  <source src="/assets/chatbot-demo.mov" type="video/mp4">
+</video>
+
+**1. Download weights**
+```py
+from llm_inference import prepare_weights
+path = prepare_weights("lmsys/longchat-13b-16k")
+```
+
+**2. Launch Gradio App**
+
+```
+python examples/chatbot/gradio_demo.py
+```
+
+
+
 ## For deploying as a REST API
 
 Create a Python file `app.py` and initialize the `ServeLLaMA` App.
 
 ```python
 # app.py
 from llm_inference.serve import ServeLLaMA, Response, PromptRequest
@@ -59,20 +80,7 @@
 component = ServeLLaMA(input_type=PromptRequest, output_type=Response)
 app = L.LightningApp(component)
 ```
 
 ```bash
 lightning run app app.py
 ```
-
-## How to use the Chatbot
-
-```python
-from chatbot import LitGPTChatBot
-
-checkpoint_dir = "weights"
-
-bot = LitGPTChatBot(
-    checkpoint_dir=checkpoint_dir)
-
-print(bot.send("hi, what is the capital of France?"))
-```
```

### Comparing `llm_inference-0.0.5.dev0/assets/llama-inference-api-min.png` & `llm_inference-0.0.6/assets/llama-inference-api-min.png`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.5.dev0/assets/llm-inference-min.png` & `llm_inference-0.0.6/assets/llm-inference-min.png`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.5.dev0/llm_inference.egg-info/PKG-INFO` & `llm_inference-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: llm-inference
-Version: 0.0.5.dev0
+Name: llm_inference
+Version: 0.0.6
 Summary: Large Language Models Inference API and Applications
 Home-page: https://github.com/aniketmaurya/llm-inference
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT,Falcon
 Requires-Python: >=3.8
@@ -42,14 +42,49 @@
 path = prepare_weights("EleutherAI/pythia-70m")
 model = LLMInference(checkpoint_dir=path)
 
 print(model("New York is located in"))
 ```
 
 
+## How to use the Chatbot
+
+```python
+from llm_chain import LitGPTConversationChain, LitGPTLLM
+from llm_inference import prepare_weights
+from rich import print
+
+
+path = str(prepare_weights("lmsys/longchat-13b-16k"))
+llm = LitGPTLLM(checkpoint_dir=path, quantize="bnb.nf4")  # 8.4GB GPU memory
+bot = LitGPTConversationChain.from_llm(llm=llm, verbose=True)
+
+print(bot.send("hi, what is the capital of France?"))
+```
+
+## Launch Chatbot App
+
+<video width="320" height="240" controls>
+  <source src="/assets/chatbot-demo.mov" type="video/mp4">
+</video>
+
+**1. Download weights**
+```py
+from llm_inference import prepare_weights
+path = prepare_weights("lmsys/longchat-13b-16k")
+```
+
+**2. Launch Gradio App**
+
+```
+python examples/chatbot/gradio_demo.py
+```
+
+
+
 ## For deploying as a REST API
 
 Create a Python file `app.py` and initialize the `ServeLLaMA` App.
 
 ```python
 # app.py
 from llm_inference.serve import ServeLLaMA, Response, PromptRequest
@@ -59,20 +94,7 @@
 component = ServeLLaMA(input_type=PromptRequest, output_type=Response)
 app = L.LightningApp(component)
 ```
 
 ```bash
 lightning run app app.py
 ```
-
-## How to use the Chatbot
-
-```python
-from chatbot import LitGPTChatBot
-
-checkpoint_dir = "weights"
-
-bot = LitGPTChatBot(
-    checkpoint_dir=checkpoint_dir)
-
-print(bot.send("hi, what is the capital of France?"))
-```
```

### Comparing `llm_inference-0.0.5.dev0/llm_inference.egg-info/SOURCES.txt` & `llm_inference-0.0.6/llm_inference.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 llm_inference.egg-info/PKG-INFO
 llm_inference.egg-info/SOURCES.txt
 llm_inference.egg-info/dependency_links.txt
 llm_inference.egg-info/requires.txt
 llm_inference.egg-info/top_level.txt
 requirements/dev.txt
 requirements/requirements.txt
-src/chatbot/__init__.py
-src/chatbot/base.py
-src/chatbot/chain.py
-src/chatbot/ui/__init__.py
-src/chatbot/ui/main.py
-src/chatbot/ui/templates.py
+src/llm_chain/__init__.py
+src/llm_chain/conversation_chain.py
+src/llm_chain/llm.py
+src/llm_chain/templates.py
+src/llm_chain/ui/__init__.py
+src/llm_chain/ui/main.py
 src/llm_inference/__init__.py
 src/llm_inference/download.py
 src/llm_inference/model.py
-src/llm_inference/serve.py
+src/llm_inference/serve.py
+src/llm_inference/token_manipulation.py
```

### Comparing `llm_inference-0.0.5.dev0/src/chatbot/base.py` & `llm_inference-0.0.6/src/llm_chain/llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,47 +7,59 @@
 
 from llm_inference import LLMInference
 
 logger = logging.getLogger(__name__)
 
 
 class DummyLLM(LLM, BaseModel):
-    def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
-        return f"Bot: {prompt}"
+    def _call(self, prompt: str, stop: Optional[list] = None, **kwargs) -> str:
+        return f"Hi, I am a helpful chatbot!"
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "Dummy LLM"
 
 
 class LitGPTLLM(LLM, BaseModel):
     checkpoint_dir: str = ""
     model: Any = None
-
-    def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
+    quantize: Optional[str] = None
+    accelerator: Optional[str] = "auto"
+    model_configs: dict = {}
+
+    def _call(
+        self,
+        prompt: str,
+        stop: Optional[list] = None,
+        temperature=1e-5,
+        **kwargs: Any,
+    ) -> str:
         if not self.model:
+            print("Loading model for first time...")
             self.model = LLMInference(
                 checkpoint_dir=self.checkpoint_dir,
-                precision="bf16-mixed",
+                quantize=self.quantize,
+                accelerator=self.accelerator,
+                **self.model_configs,
             )
 
-        return self.model(prompt)
+        return self.model.chat(prompt, temperature=temperature, **kwargs)
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "Lit-GPT LLM"
 
 
 class ServerLLM(LLM, BaseModel):
     url: str = ""
     TIMEOUT: float = 60.0
 
-    def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
+    def _call(self, prompt: str, stop: Optional[list] = None) -> str:
         """Run the LLM on the given prompt and input."""
         if self.url == "":
             raise Exception("Server URL not set!")
 
         headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
```

### Comparing `llm_inference-0.0.5.dev0/src/chatbot/ui/main.py` & `llm_inference-0.0.6/src/llm_chain/ui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Python file to serve as the frontend"""
 import logging
 
 import rich
 import streamlit as st
 from streamlit_chat import message
 
-from chatbot import ServerChatBot
+from llm_chain import ServerChatBot
 
 logger = logging.getLogger(__name__)
 
 
 def run(lightning_app_state):
     if not lightning_app_state.llm_url:
         st.info("Waiting for server to get ready...")
```

### Comparing `llm_inference-0.0.5.dev0/src/llm_inference/model.py` & `llm_inference-0.0.6/src/llm_inference/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from lightning.fabric.strategies import FSDPStrategy
 from lit_gpt import GPT, Config, Tokenizer
 from lit_gpt.adapter_v2 import add_adapter_v2_parameters_to_linear_layers
 from lit_gpt.model import Block
 from lit_gpt.utils import check_valid_checkpoint_dir, lazy_load, quantization
 from torch.distributed.fsdp.wrap import transformer_auto_wrap_policy
 
+from .token_manipulation import get_stop_tokens
+
 load_dotenv()
 
 WEIGHTS_PATH = os.environ.get("WEIGHTS")
 
 
 def generate_prompt(example):
     """Generates a standardized message to prompt the model with an instruction, optional input and a
@@ -174,15 +176,15 @@
         temperature: float = 0.1,
         eos_id=None,
     ) -> str:
         tokenizer = self.tokenizer
         model = self.model
         fabric = self.fabric
 
-        encoded = tokenizer.encode(prompt, device=model.device)
+        encoded = tokenizer.encode(prompt, device=fabric.device)
         prompt_length = encoded.size(0)
         max_returned_tokens = prompt_length + max_new_tokens
 
         t0 = time.perf_counter()
         y = _generate(
             model,
             encoded,
@@ -191,15 +193,15 @@
             temperature=temperature,
             top_k=top_k,
             eos_id=eos_id,
         )
         t = time.perf_counter() - t0
 
         model.reset_cache()
-        output = tokenizer.decode(y)
+        output = tokenizer.decode(y[prompt_length:])
         tokens_generated = y.size(0) - prompt_length
         fabric.print(
             f"\n\nTime for inference: {t:.02f} sec total, {tokens_generated / t:.02f} tokens/sec",
             file=sys.stderr,
         )
         if fabric.device.type == "cuda":
             fabric.print(
@@ -224,14 +226,30 @@
             top_k=top_k,
             temperature=temperature,
             eos_id=self.tokenizer.eos_id,
         )
         output = output.split("### Response:")[1].strip()
         return output
 
+    def chat(
+        self,
+        prompt: str,
+        max_new_tokens: int = 100,
+        top_k: int = 200,
+        temperature: float = 0.1,
+    ) -> str:
+        output = self.__call__(
+            prompt=prompt,
+            max_new_tokens=max_new_tokens,
+            top_k=top_k,
+            temperature=temperature,
+            eos_id=self.tokenizer.eos_id,
+        )
+        return output
+
     def eval(self):
         self.model.eval()
 
     def load_model(self, checkpoint_path: Union[Path, str]):
         fabric = self.fabric
         quantize = self.quantize
         config = self.config
```

### Comparing `llm_inference-0.0.5.dev0/src/llm_inference/serve.py` & `llm_inference-0.0.6/src/llm_inference/serve.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,37 +11,34 @@
     prompt: str
 
 
 class Response(BaseModel):
     result: str
 
 
-class ServeLLaMA(PythonServer):
+class ServeLitGPT(PythonServer):
     def __init__(
         self,
         input_type,
         output_type,
-        checkpoint_path: str = None,
-        tokenizer_path: str = None,
+        checkpoint_dir: str = None,
     ):
         super().__init__(input_type, output_type)
-        self.checkpoint_path = checkpoint_path
-        self.tokenizer_path = tokenizer_path
+        self.checkpoint_dir = checkpoint_dir
 
     def setup(self, *args: Any, **kwargs: Any) -> None:
         self._model = LLMInference(
-            checkpoint_path=self.checkpoint_path,
-            tokenizer_path=self.tokenizer_path,
-            dtype="bfloat16",
+            checkpoint_dir=self.checkpoint_dir,
         )
 
     def predict(self, request: PromptRequest) -> Any:
-        result = self._model(request.prompt)
+        result = self._model.chat(request.prompt)
         return Response(result=result)
 
 
 if __name__ == "__main__":
-    component = ServeLLaMA(
+    component = ServeLitGPT(
         input_type=PromptRequest,
         output_type=Response,
+        checkpoint_dir="examples/chatbot/checkpoints/lmsys/longchat-7b-16k/",
     )
     app = L.LightningApp(component)
```

