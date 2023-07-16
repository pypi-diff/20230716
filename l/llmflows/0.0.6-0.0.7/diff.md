# Comparing `tmp/llmflows-0.0.6.tar.gz` & `tmp/llmflows-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflows-0.0.6.tar", last modified: Sun Jul  9 17:56:16 2023, max compression
+gzip compressed data, was "llmflows-0.0.7.tar", last modified: Sun Jul 16 16:29:28 2023, max compression
```

## Comparing `llmflows-0.0.6.tar` & `llmflows-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-09 17:56:06.000000 llmflows-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-09 17:56:16.303363 llmflows-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-09 17:56:06.000000 llmflows-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/async_base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/async_functional_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/functional_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/functional_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/vectorstore_flowstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/llmflows/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/openai_embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/llmflows/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/prompts/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/llmflows/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/vector_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-09 17:56:06.000000 llmflows-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:56:16.303363 llmflows-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.838099 llmflows-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 16:29:16.000000 llmflows-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-16 16:29:28.838099 llmflows-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-07-16 16:29:16.000000 llmflows-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.834099 llmflows-0.0.7/llmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.834099 llmflows-0.0.7/llmflows/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/callbacks/async_base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/callbacks/async_functional_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/callbacks/base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/callbacks/functional_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.838099 llmflows-0.0.7/llmflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/async_base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/async_base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/async_chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/async_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/async_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/functional_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/flows/vectorstore_flowstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.838099 llmflows-0.0.7/llmflows/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/llms/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/llms/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/llms/message_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/llms/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/llms/openai_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.838099 llmflows-0.0.7/llmflows/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/prompts/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.838099 llmflows-0.0.7/llmflows/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/vectorstores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/vectorstores/vector_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-16 16:29:16.000000 llmflows-0.0.7/llmflows/vectorstores/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:28.834099 llmflows-0.0.7/llmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-16 16:29:28.000000 llmflows-0.0.7/llmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-16 16:29:28.000000 llmflows-0.0.7/llmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:29:28.000000 llmflows-0.0.7/llmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 16:29:28.000000 llmflows-0.0.7/llmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 16:29:28.000000 llmflows-0.0.7/llmflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-16 16:29:16.000000 llmflows-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:29:28.838099 llmflows-0.0.7/setup.cfg
```

### Comparing `llmflows-0.0.6/LICENSE` & `llmflows-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/PKG-INFO` & `llmflows-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: llmflows
-Version: 0.0.6
-Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
-Author: Stoyan Stoyanov
-Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
-Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LLMFlows - Simple, Explicit, and Transparent LLM Apps
 
 <p align="center">
   <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
@@ -36,23 +22,23 @@
 ## Installation
 ```
 pip install llmflows
 ```
 
 ## Philosophy
 
-### Simple
+### **Simple**
 Our goal is to build a simple, well-documented framework with minimal abstractions that 
 allow users to build flexible LLM-powered apps without compromising on capabilities.
 
-### Explicit
+### **Explicit**
 We want to create an explicit API enabling users to write clean and readable code while 
 easily creating complex flows of LLMs interacting with each other.
 
-### Transparent
+### **Transparent**
 We aim to help users have full transparency on their LLM-powered apps by providing 
 traceable flows and complete information for each app component, making it easy to 
 monitor, maintain, and debug.
 
 
 ## Usage
 You can quickly build a simple application with LLMFlows' `LLM` and `PrompTemplate` 
@@ -69,14 +55,28 @@
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
 
 ```
 
+You can also create a simple chat application with a few lines of code:
+```python
+from llmflows.llms import OpenAIChat
+
+
+llm = OpenAIChat(system_prompt="You are a useful assistant")
+
+while True:
+    user_message = input("You:")
+    llm.add_message(user_message)
+    llm_response, call_data, model_config = llm.generate()
+    print(f"LLM: {llm_response}")
+```
+
 However, real-world applications are often more complex and have dependencies between 
 prompts and LLM calls. For example:
 
 ![Complex flow](docs/complex_flow.png)
 
 You can build such flow using the `Flow` and `Flowstep` classes. LLMFlows will figure 
 out the dependencies and make sure each flowstep runs only when all its dependencies 
@@ -140,36 +140,83 @@
 ```
 
 In addition, LLMFlows provides async classes to improve the runtime of any complex flow 
 by running flow steps that already have all their required inputs in parallel.
 Check our documentation for more examples, such as creating question-answering apps and 
 web applications with Flask and FastAPI.
 
+## Features
+
+### **LLMs**
+- Utilize LLMs such as OpenAI's ChatGPT to generate natural language text.
+- Configure LLM classes easily, choosing specific models, parameters, and settings.
+- Benefit from automatic retries when model calls fail, ensuring reliable LLM 
+  interactions.
+
+### **Prompt Templates**
+- Create dynamic prompts using Prompt Templates, providing flexible and customizable 
+  text generation.
+- Define variables within prompts to generate prompt strings tailored to specific 
+  inputs.
+
+### **Flows and FlowSteps**
+- Structure LLM applications using Flows and FlowSteps, providing a clear and organized framework for executing LLM interactions.
+- Connect flow steps to pass outputs as inputs, facilitating seamless data flow and
+    maintaining a transparent LLM pipeline.
+- Leverage Async Flows to run LLMs in parallel when all their inputs are available, 
+  optimizing performance and efficiency.
+- Incorporate custom string manipulation functions directly into flows, allowing 
+  specialized text transformations without relying solely on LLM calls.
+
+### **VectorStore Integrations**
+- Integrate with vector databases like Pinecone using the VectorStoreFlowStep, 
+  empowering efficient and scalable storage and retrieval of vector embeddings.
+- Leverage vector databases for seamless storage and querying of vectors, enabling straightforward integration with LLM-powered applications.
+
+### **Callbacks**
+- Execute callback functions at different stages within flow steps, enabling enhanced customization, logging, tracing, or other specific integrations.
+- Utilize callbacks to comprehensively control and monitor LLM-powered apps, ensuring 
+  clear visibility into the execution process.
+
+### **Complete Transparency**
+After executing a Flow you can answer questions such as:
+
+- When was a particular flowstep run?
+- How much time did it take?
+- What were the input variables?
+- What was the prompt template?
+- What did the prompt look like?
+- What was the exact configuration of the model?
+- How many times did we retry the request?
+- What was the raw data the API returned?
+- How many tokens were used?
+- What was the final result?
+
 ## FAQ
 
-### How is this different than langchain?
+### **How is this different than langchain?**
 Langchain is a great library, and LLMFlows has undoubtedly been inspired by it. 
 However, our philosophy is a bit different. Langchian has a "chain for everything" 
 philosophy and provides many classes with multiple LLM calls, logic, and built-in 
 default prompts. While this is great for beginners and default use cases, we feel this 
 can be overwhelming if users want to do anything "out of the ordinary." In contrast, 
 we are focusing on providing as few building blocks as possible and having an 
 easy-to-understand API while matching (and in some cases exceeding) the capabilities 
 of langchain.
 
-### You only have OpenAI wrappers, but I want to use AcmeLLM.
+### **You only have OpenAI wrappers, but I want to use AcmeLLM.**
 We decided to release the library initially supporting only OpenAI LLMs, but we have a 
 roadmap and will slowly add new wrappers around the most popular models. If you are 
 willing to spend some time, we are looking for contributors and maintainers.
 
-### You only support Pinecone. Do you have plans to extend the list?
+### **You only support Pinecone. Do you have plans to extend the list?**
 Yes! Over time, we will also add Chroma, Weaviate, Redis, Elastic Search, and other 
 popular solutions. If you want to help us out, check out our contribution section.
 
-### Why can't I find any info related to document loaders?
+### **Why can't I find any info related to document loaders?**
 For the time being, we have decided not to implement document loaders for a few reasons:
 
 1. plenty of capable libraries like Llama-index and langchain have tons of loaders.
 2. We think mixing document loaders with LLM and prompt management libraries is awkward 
 3. since document loading usually happens in separate pipelines and is not part of the 
 4. LLM-powered app.
 5. Real-life documents are messy. In our experience, no matter how many loaders are out
```

### Comparing `llmflows-0.0.6/llmflows/callbacks/async_base_callback.py` & `llmflows-0.0.7/llmflows/callbacks/async_base_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/callbacks/async_functional_callback.py` & `llmflows-0.0.7/llmflows/callbacks/async_functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/callbacks/base_callback.py` & `llmflows-0.0.7/llmflows/callbacks/base_callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module provides the BaseCallback class.
 
 The Callback class is designed to be subclassed by users who want to create their
 own custom callbacks for different stages of a FlowStep execution.
 """
 
-from typing import Callable, Optional, Any
+from typing import Any
 
 
 class BaseCallback:
     """
     Represents a callback to be invoked at different stages of a FlowStep execution.
 
     The user can subclass this and override the methods corresponding to
```

### Comparing `llmflows-0.0.6/llmflows/callbacks/functional_callback.py` & `llmflows-0.0.7/llmflows/callbacks/functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/flows/async_base_flow.py` & `llmflows-0.0.7/llmflows/flows/async_base_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,19 @@
             self.output_keys.add(step.output_key)
             self.names.add(step.name)
 
             flowstep_class = step.__class__.__name__
             if flowstep_class == "AsyncFlowStep":
                 self.input_keys.update(step.prompt_template.variables)
             elif flowstep_class == "AsyncChatFlowStep":
-                self.input_keys.update(
-                    step.system_prompt_template.variables,
-                    step.message_prompt_template.variables,
-                    {step.message_key},
-                )
+                self.input_keys.update({step.message_key})
+
+                if step.message_prompt_template:
+                    self.input_keys.update(step.message_prompt_template.variables)
+
 
     def _check_all_input_keys_available(self, user_inputs):
         """
         Checks that all required input keys for all steps in the flow are available.
 
         Args:
             user_inputs (dict): The set of input keys provided by the user.
```

### Comparing `llmflows-0.0.6/llmflows/flows/async_base_flowstep.py` & `llmflows-0.0.7/llmflows/flows/async_base_flowstep.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
         Args:
             inputs (dict[str, Any]): The inputs to the flow step.
 
         Returns:
             tuple: result, call data and model configuration.
         """
-        pass
 
     async def run(
         self, inputs: dict[str, str], verbose: bool = False
     ) -> dict[str, str]:
         """
         Runs the flow step with the provided inputs and returns a dictionary with
         runtime details.
```

### Comparing `llmflows-0.0.6/llmflows/flows/async_chat_flowstep.py` & `llmflows-0.0.7/llmflows/flows/async_chat_flowstep.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 """
 This file contains the AsyncChatFlowStep class, which represents a step in an AsyncFlow
 that is using a chat LLM. The async implementation allows async flowsteps to be 
 run in parallel if multiple flowsteps have all the required inputs available.
 """
 
-import logging
 from typing import Any, Union
-from llmflows.llms.llm import BaseLLM
+from llmflows.llms import OpenAIChat, MessageHistory
 from llmflows.prompts.prompt_template import PromptTemplate
 from llmflows.callbacks.async_base_callback import AsyncBaseCallback
 from llmflows.flows.async_base_flowstep import AsyncBaseFlowStep
 
 
 class AsyncChatFlowStep(AsyncBaseFlowStep):
     """
@@ -20,87 +19,79 @@
 
     An AsyncChatFlowStep calls a language model using two prompt templates, namely
     a system prompt and a message prompt, records the run time, and optionally
     invokes callback functions on the results.
 
     Args:
         name (str): The name of the flow step.
-        llm (BaseLLM): The language model to be used in the flow step.
+        llm (OpenAIChat): The language model to be used in the flow step.
         output_key (str): The key for the output of the flow step.
-        system_prompt_template (PromptTemplate): Prompt tempalte for the system prompt
-            to be used with the language model.
+        message_history (Union[MessageHistory, None]): predefined conversation history
         message_key (str): Key used to extract message from inputs.
         message_prompt_template (PromptTemplate): Prompt template for the message used
             with the language model.
         callbacks (Union[list[AsyncBaseCallback], None]): Callbacks to be invoked
-            during the flowstep run.
+            within the flowstep
 
     Attributes:
         llm (BaseLLM): The language model to be used in the flow step.
         message_key (str): Key used to extract message from inputs.
         system_prompt_template (PromptTemplate): Prompt tempalte for the system prompt
             to be used with the language model.
         message_prompt_template (PromptTemplate): Prompt template for the message used
             with the language model.
         required_keys (set[str]): The keys required for the flow step to run.
     """
 
     def __init__(
         self,
         name: str,
-        llm: BaseLLM,
+        llm: OpenAIChat,
         output_key: str,
-        system_prompt_template: PromptTemplate,
         message_key: str,
+        message_history: Union[MessageHistory, None] = None,
         message_prompt_template: Union[PromptTemplate, None] = None,
-        callbacks:  Union[list[AsyncBaseCallback], None] = None,
+        callbacks: Union[list[AsyncBaseCallback], None] = None,
     ):
         super().__init__(name, output_key, callbacks)
         self.llm = llm
         self.message_key = message_key
-        self.system_prompt_template = system_prompt_template
+        self.message_history = message_history if message_history else MessageHistory()
         self.message_prompt_template = message_prompt_template
         self.required_keys = self._add_required_keys()
         self._validate_message_key()
 
     def _add_required_keys(self):
+        required_keys = {}
         if self.message_prompt_template:
             required_keys = {self.message_key}.union(
-                self.system_prompt_template.variables,
                 self.message_prompt_template.variables,
             )
-        else:
-            required_keys = {self.message_key}.union(
-                self.system_prompt_template.variables
-            )
 
         return required_keys
 
     def _validate_message_key(self):
-        if self.message_key in self.system_prompt_template.variables:
-            logging.warning(
-                "The message_key matches a variable in the system"
-                " prompt.\nmessage_key: %s\nsystem_prompt_template"
-                " variables: %s. Ignore this warning"
-                " if you intended to include the message in the system prompt.",
-                self.message_key,
-                self.system_prompt_template.variables
-            )
-
         if self.message_prompt_template:
             if self.message_key not in self.message_prompt_template.variables:
                 raise ValueError(
                     "You've provided a message prompt template that doesn't contain "
                     "the message key variable."
                 )
 
     async def generate(self, inputs: dict[str, Any]) -> tuple[Any, Any, Any]:
-        system_prompt = self.system_prompt_template.get_prompt(**inputs)
-        self.llm.update_system_prompt(system_prompt)
-
         if self.message_prompt_template:
             message = self.message_prompt_template.get_prompt(**inputs)
         else:
             message = inputs[self.message_key]
-        self.llm.add_message(message)
 
-        return await self.llm.generate_async()
+        self.message_history.add_user_message(message)
+        results = await self.llm.generate_async(self.message_history)
+
+        results[1]["message_prompt_template"] = (
+            self.message_prompt_template.prompt
+            if self.message_prompt_template
+            else None
+        )
+        results[1]["message_prompt"] = message
+        results[1]["message_history"] = self.message_history.messages
+
+        return results
```

### Comparing `llmflows-0.0.6/llmflows/flows/async_flow.py` & `llmflows-0.0.7/llmflows/flows/async_flow.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/flows/async_flowstep.py` & `llmflows-0.0.7/llmflows/flows/async_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/flows/base_flow.py` & `llmflows-0.0.7/llmflows/flows/base_flow.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,19 +84,19 @@
             self.output_keys.add(step.output_key)
             self.names.add(step.name)
 
             flowstep_class = step.__class__.__name__
             if flowstep_class == "FlowStep":
                 self.input_keys.update(step.prompt_template.variables)
             elif flowstep_class == "ChatFlowStep":
-                self.input_keys.update(
-                    step.system_prompt_template.variables,
-                    step.message_prompt_template.variables,
-                    {step.message_key},
-                )
+                self.input_keys.update({step.message_key})
+
+                if step.message_prompt_template:
+                    self.input_keys.update(step.message_prompt_template.variables)
+
             elif flowstep_class == "FunctionalFlowStep":
                 self.input_keys.update(step.required_keys)
 
     def _check_all_input_keys_available(self, user_inputs):
         """
         Checks that all required input keys are available.
```

### Comparing `llmflows-0.0.6/llmflows/flows/base_flowstep.py` & `llmflows-0.0.7/llmflows/flows/base_flowstep.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 
         Args:
             inputs (dict[str, Any]): The inputs to the flow step.
 
         Returns:
             tuple: result, call data and model configuration.
         """
-        pass
 
     def run(self, inputs: dict[str, str], verbose: bool = False) -> dict[str, str]:
         """
         Executes the flow step with the provided inputs and returns a dictionary with
         execution details.
 
         This includes the start and end times, the prompts and the input to the
```

### Comparing `llmflows-0.0.6/llmflows/flows/flow.py` & `llmflows-0.0.7/llmflows/flows/flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,21 @@
     """
 
     def __init__(self, first_step: BaseFlowStep):
         super().__init__(first_step)
         self.results = {}
         self.completed_steps = set()
 
+    def _reset_flow(self):
+        """
+        Resets the flow by clearing the results and completed steps.
+        """
+        self.results = {}
+        self.completed_steps = set()
+
     def start(self, verbose=False, **inputs) -> dict:
         """
         Executes the flow with the provided inputs.
 
         Args:
             verbose (bool): Specifies if the flow step should print their output.
             **inputs (dict): The inputs to the flow.
@@ -40,15 +47,19 @@
             A dictionary of the results from each flow step.
 
         Raises:
             ValueError: If any required inputs are missing.
         """
         self._check_all_input_keys_available(inputs)
         self._run_step(self._first_step, inputs, verbose)
-        return self.results
+
+        final_result = self.results
+        self._reset_flow()
+
+        return final_result
 
     def _run_step(self, step, inputs, verbose):
         """
         Executes the given step and its next steps in a DFS-like manner.
 
         Args:
             step (FlowStep): The step to run.
@@ -58,17 +69,15 @@
         Returns:
             Any: The output of the step.
         """
 
         if not step or any(parent.output_key not in inputs for parent in step.parents):
             return
 
-        required_inputs = {
-            key: inputs[key] for key in step.required_keys
-        }
+        required_inputs = {key: inputs[key] for key in step.required_keys}
 
         if step not in self.completed_steps:
             flow_data = step.run(required_inputs, verbose)
             self.completed_steps.add(step)
 
             if flow_data:
                 self.results[step.name] = flow_data
```

### Comparing `llmflows-0.0.6/llmflows/flows/flowstep.py` & `llmflows-0.0.7/llmflows/flows/flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/flows/functional_flowstep.py` & `llmflows-0.0.7/llmflows/flows/functional_flowstep.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 LLMFlow module for the `FunctionalFlowstep` class that can be used to run a given
 function within a flow.
 """
 
 import inspect
+from typing import Callable, Any, Union
 from llmflows.flows.flowstep import BaseFlowStep
 from llmflows.callbacks.base_callback import BaseCallback
-from typing import Callable, Any, Union
 
 
 class FunctionalFlowStep(BaseFlowStep):
     """
     Represents a functional flow step that runs a function. The function must take
         a dictionary of strings as input and return a string(like regular flow steps)
 
@@ -55,8 +55,15 @@
         fn_args = inspect.getfullargspec(self.flowstep_fn).args
 
         # Create a new dictionary from inputs containing only the keys that fn requires
         filtered_inputs = {
             key: value for key, value in inputs.items() if key in fn_args
         }
 
-        return self.flowstep_fn(**filtered_inputs), None, None
+        result = self.flowstep_fn(**filtered_inputs)
+
+        if not isinstance(result, str):
+            raise TypeError(
+                f"Return value must be of type str, but got {type(result).__name__}"
+            )
+
+        return result, None, None
```

### Comparing `llmflows-0.0.6/llmflows/flows/vectorstore_flowstep.py` & `llmflows-0.0.7/llmflows/flows/vectorstore_flowstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+# pylint: disable=R0913
 """
 This module provides the `VectorStoreFlowStep` class which extends the `BaseFlowStep` 
 class.
 
 This class represents a flow step that uses its prompt to search for a vector store.
 Each instance of this class will be initialized with a specific vector store, 
 embeddings model, prompt template, and other attributes.
 """
 
+from typing import Any, Union
 from llmflows.prompts.prompt_template import PromptTemplate
 from llmflows.llms.llm import BaseLLM
 from llmflows.flows.flowstep import BaseFlowStep
 from llmflows.callbacks.base_callback import BaseCallback
 from llmflows.vectorstores.vector_store import VectorStore
 from llmflows.vectorstores.vector_doc import VectorDoc
-from typing import Any, Union
 
 
 class VectorStoreFlowStep(BaseFlowStep):
     """
     Represents a flowstep that uses a prompt to search for a vector store.
 
     The VectorStoreFlowstep uses the prompt template and the inputs to create a prompt,
```

### Comparing `llmflows-0.0.6/llmflows/llms/llm_utils.py` & `llmflows-0.0.7/llmflows/llms/llm_utils.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/llms/openai.py` & `llmflows-0.0.7/llmflows/llms/openai.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# pylint: disable=too-few-public-methods
+# pylint: disable=too-few-public-methods, R0913, W0221
 
 """
 This module implements a wrapper for OpenAI completion models, using BaseLLM as a 
 base class.
 """
 
-import os
 import openai
 from .llm import BaseLLM
 from .llm_utils import call_with_retry, async_call_with_retry
 
 
 class OpenAI(BaseLLM):
     """
@@ -20,44 +19,51 @@
     Uses the specified OpenAI model and parameters for interacting with the OpenAI API.
 
     Args:
         model (str): The name of the OpenAI model to use.
         temperature (float): The temperature to use for text generation.
         max_tokens (int): The maximum number of tokens to generate.
         max_retries (int): The maximum number of retries for generating tokens.
+        api_key (str): The API key to use for interacting with the OpenAI API.
 
     Attributes:
         temperature (float): The temperature to use for text generation.
         max_tokens (int): The maximum number of tokens to generate.
         max_retries (int): The maximum number of retries for generating tokens.
     """
 
     def __init__(
         self,
+        api_key: str,
         model: str = "text-davinci-003",
         temperature: float = 0.7,
         max_tokens: int = 500,
-        max_retries: int = 3,
+        max_retries: int = 3
     ):
         super().__init__(model)
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.max_retries = max_retries
-        self._api_key = os.environ["OPENAI_API_KEY"]
+        self._api_key = api_key
+        if not self._api_key:
+            raise ValueError(
+                "API Key must be provided or set in the OPENAI_API_KEY environment"
+                " variable"
+            )
 
-    def perepare_results(self, model_outputs, retries) -> tuple[str, dict, dict]:
+    def prepare_results(self, model_outputs, retries) -> tuple[str, dict, dict]:
         """
         Formats results after generation.
 
         Args:
             model_outputs: Raw output after model generation.
             retries (int): Number of retries taken for successful generation.
 
         Returns:
-            A tuple containing the generated text, the raw response data, and the 
+            A tuple containing the generated text, the raw response data, and the
                 model configuration.
         """
         text_result = model_outputs.choices[0]["text"]
 
         call_data = {
             "raw_outputs": model_outputs,
             "retries": retries,
@@ -67,50 +73,58 @@
             "model_name": self.model,
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
         }
 
         return text_result, call_data, model_config
 
-    def generate(self, prompt) -> tuple[str, dict, dict]:
+    def generate(self, prompt: str) -> tuple[str, dict, dict]:
         """
         Generates text from a given prompt using OpenAI API.
 
         Args:
             prompt (str): Text prompt for generation.
 
         Returns:
-            A tuple containing the generated text, the raw response data, and the 
+            A tuple containing the generated text, the raw response data, and the
                 model configuration.
         """
+
+        if not isinstance(prompt, str):
+            raise TypeError("Prompt must be a string")
+
         completion, retries = call_with_retry(
             api_obj=openai.Completion,
             max_retries=self.max_retries,
             model=self.model,
             prompt=prompt,
             max_tokens=self.max_tokens,
             temperature=self.temperature,
         )
 
-        return self.perepare_results(completion, retries)
+        return self.prepare_results(completion, retries)
 
-    async def generate_async(self, prompt) -> tuple[str, dict, dict]:
+    async def generate_async(self, prompt: str) -> tuple[str, dict, dict]:
         """
         Generates text from a given prompt using OpenAI API asynchronously.
 
         Args:
             prompt (str): Text prompt for generation.
 
         Returns:
-            A tuple containing the generated text, the raw response data, and the 
+            A tuple containing the generated text, the raw response data, and the
                 model configuration.
         """
+
+        if not isinstance(prompt, str):
+            raise TypeError("Prompt must be a string")
+
         completion, retries = await async_call_with_retry(
             api_obj=openai.Completion,
             max_retries=self.max_retries,
             model=self.model,
             prompt=prompt,
             max_tokens=self.max_tokens,
             temperature=self.temperature,
         )
 
-        return self.perepare_results(completion, retries)
+        return self.prepare_results(completion, retries)
```

### Comparing `llmflows-0.0.6/llmflows/llms/openai_embeddings.py` & `llmflows-0.0.7/llmflows/llms/openai_embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,82 @@
-# pylint: disable=too-few-public-methods
+# pylint: disable=too-few-public-methods, W0221, R0801
 
 """
 This module helps with creating embeddings form OpenAIs API.
 """
 
-import os
 from typing import Union
 import openai
 from llmflows.vectorstores.vector_doc import VectorDoc
 from llmflows.llms.llm_utils import call_with_retry, async_call_with_retry
 from .llm import BaseLLM
 
 
 class OpenAIEmbeddings(BaseLLM):
     """
     A class for interacting with the OpenAI embeddings API.
 
     Inherits from BaseLLM.
 
-    Uses the specified OpenAI model and parameters for interacting with the OpenAI 
-    embeddings API. Adds embeddings to a single VectorDoc or a list of VectorDoc 
+    Uses the specified OpenAI model and parameters for interacting with the OpenAI
+    embeddings API. Adds embeddings to a single VectorDoc or a list of VectorDoc
     classes, based on the text in the VectorDoc.
 
     Args:
         model (str): The name of the OpenAI model to use.
+        api_key (str): The API key to use for authentication.
+        max_retries (int): The maximum number of retries for generating embeddings.
 
     Attributes:
         _api_key (str): The API key to use for authentication.
         max_retries (int): The maximum number of retries for generating embeddings.
     """
 
-    def __init__(self, model: str = "text-embedding-ada-002", max_retries: int = 3):
+    def __init__(
+        self,
+        api_key: str,
+        model: str = "text-embedding-ada-002",
+        max_retries: int = 3,
+    ):
         super().__init__(model)
-        self._api_key = os.getenv("OPENAI_API_KEY")
         self.max_retries = max_retries
+        self._api_key = api_key
+        if not self._api_key:
+            raise ValueError(
+                "API Key must be provided or set in the OPENAI_API_KEY environment"
+                " variable"
+            )
 
     def generate(
         self, docs: Union[VectorDoc, list[VectorDoc]]
     ) -> Union[VectorDoc, list[VectorDoc]]:
         """
         Adds embeddings to a single or list of VectorDocs using OpenAI's service.
 
         Args:
             docs: A single VectorDoc or a list of VectorDocs to embed.
 
         Returns:
             If a single VectorDoc was passed, returns it with its embedding field
-                updated. If a list of VectorDocs was passed, returns the list with the 
+                updated. If a list of VectorDocs was passed, returns the list with the
                 embedding field of each VectorDoc updated.
         """
         single_item = False
 
         if not isinstance(docs, list):
             docs = [docs]
             single_item = True
 
         texts = [doc.doc for doc in docs]
 
         result, _ = call_with_retry(
             api_obj=openai.Embedding,
             engine=self.model,
             input=texts,
-            max_retries=self.max_retries
+            max_retries=self.max_retries,
         )
 
         for i, doc in enumerate(docs):
             doc.embedding = result["data"][i]["embedding"]
 
         return docs[0] if single_item else docs
 
@@ -76,29 +87,29 @@
         Async Method that adds embeddings to a single or list of VectorDocs using OpenAI's service.
 
         Args:
             docs: A single VectorDoc or a list of VectorDocs to embed.
 
         Returns:
             If a single VectorDoc was passed, returns it with its embedding field
-                updated. If a list of VectorDocs was passed, returns the list with the 
+                updated. If a list of VectorDocs was passed, returns the list with the
                 embedding field of each VectorDoc updated.
         """
         single_item = False
 
         if not isinstance(docs, list):  # if a single item was passed
             docs = [docs]
             single_item = True
 
         texts = [doc.doc for doc in docs]
 
         result, _ = await async_call_with_retry(
             api_obj=openai.Embedding,
             engine=self.model,
             input=texts,
-            max_retries=self.max_retries
+            max_retries=self.max_retries,
         )
 
         for i, doc in enumerate(docs):
             doc.embedding = result["data"][i]["embedding"]
 
         return docs[0] if single_item else docs
```

### Comparing `llmflows-0.0.6/llmflows/prompts/prompt_template.py` & `llmflows-0.0.7/llmflows/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/vectorstores/pinecone.py` & `llmflows-0.0.7/llmflows/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/vectorstores/vector_doc.py` & `llmflows-0.0.7/llmflows/vectorstores/vector_doc.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.6/llmflows/vectorstores/vector_store.py` & `llmflows-0.0.7/llmflows/vectorstores/vector_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 Classes that represent specific vector store services (like Pinecone, for example)
 should inherit from VectorStore and provide their own implementations for
 each of the methods defined in VectorStore.
 """
 
 from abc import ABC, abstractmethod
-from llmflows.vectorstores.vector_doc import VectorDoc
 from typing import List
+from llmflows.vectorstores.vector_doc import VectorDoc
 
 
 class VectorStore(ABC):
     """
     Abstract base class for vector store services.
 
     This class defines the interface that all vector store services must provide.
@@ -25,31 +25,28 @@
         self.storage_entity = storage_entity
         self._api_key = api_key
         self.region = region
 
     @abstractmethod
     def describe(self) -> None:
         """Describe the index."""
-        pass
 
     @abstractmethod
     def search(self, query: VectorDoc, top_k: int) -> List[dict]:
         """
         Search the index for similar vectors.
 
         Args:
             query (VectorDoc): The query vector to search for.
             top_k (int): The number of results to return.
 
         Returns:
             list[dict]: A list of dictionaries representing the search results.
         """
-        pass
 
     @abstractmethod
     def upsert(self, docs: List[VectorDoc]) -> None:
         """Insert or update vectors in the index.
 
         Args:
             docs (list[VectorDoc]): VectorDoc objects to insert or update.
         """
-        pass
```

### Comparing `llmflows-0.0.6/llmflows.egg-info/SOURCES.txt` & `llmflows-0.0.7/llmflows.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 llmflows/flows/flow.py
 llmflows/flows/flowstep.py
 llmflows/flows/functional_flowstep.py
 llmflows/flows/vectorstore_flowstep.py
 llmflows/llms/__init__.py
 llmflows/llms/llm.py
 llmflows/llms/llm_utils.py
+llmflows/llms/message_history.py
 llmflows/llms/openai.py
 llmflows/llms/openai_chat.py
 llmflows/llms/openai_embeddings.py
 llmflows/prompts/__init__.py
 llmflows/prompts/prompt_template.py
 llmflows/vectorstores/__init__.py
 llmflows/vectorstores/pinecone.py
```

### Comparing `llmflows-0.0.6/pyproject.toml` & `llmflows-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llmflows"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Stoyan Stoyanov"},
 ]
 description = "LLMFlows - Simple, Explicit and Transparent LLM Apps"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

