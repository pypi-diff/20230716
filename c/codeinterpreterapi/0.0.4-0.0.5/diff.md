# Comparing `tmp/codeinterpreterapi-0.0.4.tar.gz` & `tmp/codeinterpreterapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinterpreterapi-0.0.4.tar", max compression
+gzip compressed data, was "codeinterpreterapi-0.0.5.tar", max compression
```

## Comparing `codeinterpreterapi-0.0.4.tar` & `codeinterpreterapi-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.4/LICENSE
--rw-r--r--   0        0        0     2142 2023-07-15 08:38:12.853808 codeinterpreterapi-0.0.4/README.md
--rw-r--r--   0        0        0       62 2023-07-14 11:46:56.280365 codeinterpreterapi-0.0.4/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.4/codeinterpreterapi/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/functions_agent.py
--rw-r--r--   0        0        0     3054 2023-07-14 17:11:05.973711 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0     1836 2023-07-14 17:11:05.948871 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/remove_download_link.py
--rw-r--r--   0        0        0      336 2023-07-14 17:11:05.942603 codeinterpreterapi-0.0.4/codeinterpreterapi/config.py
--rw-r--r--   0        0        0       78 2023-07-14 17:11:05.936317 codeinterpreterapi-0.0.4/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.4/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-15 11:55:28.309715 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/file.py
--rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/input.py
--rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/response.py
--rw-r--r--   0        0        0     7960 2023-07-14 17:36:03.828238 codeinterpreterapi-0.0.4/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      629 2023-07-15 12:04:32.328557 codeinterpreterapi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2917 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2476 2023-07-16 09:17:02.062499 codeinterpreterapi-0.0.5/README.md
+-rw-r--r--   0        0        0       62 2023-07-14 11:46:56.280365 codeinterpreterapi-0.0.5/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.5/codeinterpreterapi/callbacks.py
+-rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/functions_agent.py
+-rw-r--r--   0        0        0     3054 2023-07-14 17:11:05.973711 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0     1836 2023-07-14 17:11:05.948871 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/remove_download_link.py
+-rw-r--r--   0        0        0      336 2023-07-14 17:11:05.942603 codeinterpreterapi-0.0.5/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0       78 2023-07-14 17:11:05.936317 codeinterpreterapi-0.0.5/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.5/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/__init__.py
+-rw-r--r--   0        0        0     2301 2023-07-15 13:40:20.463191 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/file.py
+-rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/input.py
+-rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/response.py
+-rw-r--r--   0        0        0     7979 2023-07-16 08:46:08.541001 codeinterpreterapi-0.0.5/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      629 2023-07-16 09:23:19.074950 codeinterpreterapi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.5/PKG-INFO
```

### Comparing `codeinterpreterapi-0.0.4/LICENSE` & `codeinterpreterapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.4/README.md` & `codeinterpreterapi-0.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # Code Interpreter API
 
 A LangChain implementation of the ChatGPT Code Interpreter.
 Using CodeBoxes as backend for sandboxed python code execution.
 [CodeBox](https://github.com/shroominic/codebox-api/tree/main) is the simplest cloud infrastructure for your LLM Apps.
-You can run everything local using your own OpenAI API Key.
+You can run everything local except the LLM using your own OpenAI API Key.
+
+## Features
+
+- Dataset Analysis, Stock Charting, Image Manipulation, ....
+- Internet access and auto Python package installation
+- Input `text + files` -> Receive `text + files`
+- Run everything local except the OpenAI API (OpenOrca or others coming soon)
+- Use CodeBox API for easy scaling in production (coming soon)
 
 ## Installation
 
+Get your OpenAI API Key [here](https://platform.openai.com/account/api-keys) and install the package.
+
 ```bash
 pip install codeinterpreterapi
 ```
 
 ## Usage
 
 ```python
@@ -34,29 +44,30 @@
     print("AI: ", output.content)
 
     # terminate the session
     await session.astop()
     
 
 if __name__ == "__main__":
-    import asyncio
+    import asyncio, os
+    os.environ["OPENAI_API_KEY"] = "sk-*********"  # or .env file
 
     asyncio.run(main())
 
 ```
 
 ## Output
 
 ![Bitcoin YTD](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/bitcoin_chart.png?raw=true)
 
 ## Production
 
 In case you want to deploy to production you can use the CodeBox API for easy scaling.
-Please contact me if you want to use the CodeBox API in production.
-Its currently in early development and not everything is automated yet.
+
+Please contact me if you interested in this, because it's still in early development.
 
 ## Contributing
 
 There are some TODOs left in the code
 so if you want to contribute feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
 Just open an issue pull request and I will review it.
@@ -69,10 +80,9 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
-You can contact me at [pleurae-berets.0u@icloud.com](mailto:pleurae-berets.0u@icloud.com)
-Sorry for the weird email address but I don't want to get spammed so I can deactivate it if necessary.
-But you can also contact me on [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community).
+You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
+But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community) DMs.
```

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/callbacks.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/callbacks.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/chains/functions_agent.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/chains/functions_agent.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/chains/modifications_check.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/chains/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/chains/remove_download_link.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/chains/remove_download_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/schema/file.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/schema/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         # Convert image to RGB if it's not
         if img.mode not in ('RGB', 'L'):  # L is for greyscale images
             img = img.convert('RGB')
 
         # Display the image
         try:
             # Try to get the IPython shell if available.
-            shell = get_ipython().__class__.__name__
+            shell = get_ipython().__class__.__name__  # type: ignore
 
             # If the shell is ZMQInteractiveShell, it means we're in a Jupyter notebook or similar.
             if shell == 'ZMQInteractiveShell':
                 from IPython.display import display
                 display(img)
             else:
                 # We're not in a Jupyter notebook.
```

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/schema/response.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/schema/response.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.4/codeinterpreterapi/session.py` & `codeinterpreterapi-0.0.5/codeinterpreterapi/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from langchain.tools import StructuredTool
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.prompts.chat import MessagesPlaceholder
 from langchain.agents import AgentExecutor, BaseSingleActionAgent
 from langchain.memory import ConversationBufferMemory
 
-from codeinterpreterapi.schema import CodeInterpreterResponse, CodeInput, File, UserRequest  # type: ignore
+from codeinterpreterapi.schema import CodeInterpreterResponse, CodeInput, File, UserRequest
 from codeinterpreterapi.config import settings
 from codeinterpreterapi.chains.functions_agent import OpenAIFunctionsAgent
 from codeinterpreterapi.prompts import code_interpreter_system_message
 from codeinterpreterapi.callbacks import CodeCallbackHandler
 from codeinterpreterapi.chains.modifications_check import get_file_modifications
 from codeinterpreterapi.chains.remove_download_link import remove_download_link
 
@@ -35,15 +35,15 @@
             StructuredTool(
                 name="python",
                 description=
                 # TODO: variables as context to the agent
                 # TODO: current files as context to the agent
                 "Input a string of code to a python interpreter (jupyter kernel). "
                 "Variables are preserved between runs. ",
-                func=self.codebox.run,
+                func=self.run_handler,
                 coroutine=self.arun_handler,
                 args_schema=CodeInput,
             ),
         ]
 
     def _llm(self, model: str | None, openai_api_key: str | None) -> BaseChatModel:
         if model is None:
@@ -87,15 +87,14 @@
             print(code)
 
     def run_handler(self, code: str):
         raise NotImplementedError("Use arun_handler for now.")
 
     async def arun_handler(self, code: str):
         """Run code in container and send the output to the user"""
-        # TODO: upload files
         output: CodeBoxOutput = await self.codebox.arun(code)
 
         if not isinstance(output.content, str):
             raise TypeError("Expected output.content to be a string.")
 
         if output.type == "image/png":
             filename = f"image-{uuid.uuid4()}.png"
@@ -107,16 +106,18 @@
         elif output.type == "error":
             if "ModuleNotFoundError" in output.content:
                 if package := re.search(
                     r"ModuleNotFoundError: No module named '(.*)'", output.content
                 ):
                     await self.codebox.ainstall(package.group(1))
                     return f"{package.group(1)} was missing but got installed now. Please try again."
-            # TODO: preanalyze error to optimize next code generation
-            print("Error:", output.content)
+            else: pass
+                # TODO: preanalyze error to optimize next code generation
+            if settings.VERBOSE:
+                print("Error:", output.content)
 
         elif modifications := await get_file_modifications(code, self.llm):
             for filename in modifications:
                 if filename in [file.name for file in self.input_files]:
                     continue
                 fileb = await self.codebox.adownload(filename)
                 if not fileb.content:
```

### Comparing `codeinterpreterapi-0.0.4/pyproject.toml` & `codeinterpreterapi-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeinterpreterapi"
-version = "0.0.4"
+version = "0.0.5"
 description = "CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter."
 authors = ["Shroominic <pleurae-berets.0u@icloud.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `codeinterpreterapi-0.0.4/PKG-INFO` & `codeinterpreterapi-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeinterpreterapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,18 +19,28 @@
 Description-Content-Type: text/markdown
 
 # Code Interpreter API
 
 A LangChain implementation of the ChatGPT Code Interpreter.
 Using CodeBoxes as backend for sandboxed python code execution.
 [CodeBox](https://github.com/shroominic/codebox-api/tree/main) is the simplest cloud infrastructure for your LLM Apps.
-You can run everything local using your own OpenAI API Key.
+You can run everything local except the LLM using your own OpenAI API Key.
+
+## Features
+
+- Dataset Analysis, Stock Charting, Image Manipulation, ....
+- Internet access and auto Python package installation
+- Input `text + files` -> Receive `text + files`
+- Run everything local except the OpenAI API (OpenOrca or others coming soon)
+- Use CodeBox API for easy scaling in production (coming soon)
 
 ## Installation
 
+Get your OpenAI API Key [here](https://platform.openai.com/account/api-keys) and install the package.
+
 ```bash
 pip install codeinterpreterapi
 ```
 
 ## Usage
 
 ```python
@@ -54,29 +64,30 @@
     print("AI: ", output.content)
 
     # terminate the session
     await session.astop()
     
 
 if __name__ == "__main__":
-    import asyncio
+    import asyncio, os
+    os.environ["OPENAI_API_KEY"] = "sk-*********"  # or .env file
 
     asyncio.run(main())
 
 ```
 
 ## Output
 
 ![Bitcoin YTD](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/bitcoin_chart.png?raw=true)
 
 ## Production
 
 In case you want to deploy to production you can use the CodeBox API for easy scaling.
-Please contact me if you want to use the CodeBox API in production.
-Its currently in early development and not everything is automated yet.
+
+Please contact me if you interested in this, because it's still in early development.
 
 ## Contributing
 
 There are some TODOs left in the code
 so if you want to contribute feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
 Just open an issue pull request and I will review it.
@@ -89,11 +100,10 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
-You can contact me at [pleurae-berets.0u@icloud.com](mailto:pleurae-berets.0u@icloud.com)
-Sorry for the weird email address but I don't want to get spammed so I can deactivate it if necessary.
-But you can also contact me on [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community).
+You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
+But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community) DMs.
```

