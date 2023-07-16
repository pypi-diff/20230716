# Comparing `tmp/freeGPT-1.2.3.tar.gz` & `tmp/freeGPT-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.2.3.tar", last modified: Thu Jul 13 11:19:43 2023, max compression
+gzip compressed data, was "freeGPT-1.2.4.tar", last modified: Sun Jul 16 18:28:51 2023, max compression
```

## Comparing `freeGPT-1.2.3.tar` & `freeGPT-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:19:43.392366 freeGPT-1.2.3/
--rw-rw-rw-   0        0        0    18092 2023-07-13 11:17:19.000000 freeGPT-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     3637 2023-07-13 11:19:43.391366 freeGPT-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2356 2023-07-13 11:17:19.000000 freeGPT-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 11:19:43.345396 freeGPT-1.2.3/freeGPT/
--rw-rw-rw-   0        0        0      120 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/alpaca_7b.py
--rw-rw-rw-   0        0        0     2087 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/gpt3.py
--rw-rw-rw-   0        0        0     4647 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/gpt4.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:19:43.389368 freeGPT-1.2.3/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3637 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 11:19:43.393366 freeGPT-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1670 2023-07-13 11:17:19.000000 freeGPT-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:28:51.103456 freeGPT-1.2.4/
+-rw-rw-rw-   0        0        0    18092 2023-07-16 18:28:26.000000 freeGPT-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     4173 2023-07-16 18:28:51.102469 freeGPT-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2868 2023-07-16 18:28:26.000000 freeGPT-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 18:28:51.088457 freeGPT-1.2.4/freeGPT/
+-rw-rw-rw-   0        0        0      136 2023-07-16 18:28:26.000000 freeGPT-1.2.4/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     2087 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     4647 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/gpt4.py
+-rw-rw-rw-   0        0        0     3299 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/prodia.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:28:51.101466 freeGPT-1.2.4/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     4173 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 18:28:51.104456 freeGPT-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1670 2023-07-16 18:28:26.000000 freeGPT-1.2.4/setup.py
```

### Comparing `freeGPT-1.2.3/LICENSE` & `freeGPT-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.3/PKG-INFO` & `freeGPT-1.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.3
+Version: 1.2.4
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
@@ -31,28 +31,30 @@
 # freeGPT
 
 freeGPT provides free access to GPT3, GPT4 and more models.
 
 ## Get started:
 
 ```
-py -m pip install --upgrade freeGPT
+python -m pip install --upgrade freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
 | gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
+| prodia   | [<prodia.com>](https://prodia.com/)                     |
+
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
@@ -62,25 +64,26 @@
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
 - [x] Make the overall library easier to understand.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
 - [x] Make a ChatUI.
-- [ ] Add an image generation model.
+- [x] Add an image generation model.
 
 ## Discord bot:
 
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - This bot has all the models in this repository available.
 - It's interactive, overall fast, and easy to use.
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
+**Text Completion:**
 ```python
 import freeGPT
 import asyncio
 
 
 async def main():
     while True:
@@ -91,10 +94,31 @@
         except Exception as e:
             print(f"🤖: {e}")
 
 
 asyncio.run(main())
 ```
 
+**Image Generation:**
+```python
+import freeGPT
+import asyncio
+from PIL import Image
+
+
+async def main():
+    while True:
+        prompt = input("👦: ")
+        try:
+            resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
+            Image.open(resp).show()
+            print(f"🤖: Image shown.")
+        except Exception as e:
+            print(f"🤖: {e}")
+
+
+asyncio.run(main())
+```
+
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.3/README.md` & `freeGPT-1.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 # freeGPT
 
 freeGPT provides free access to GPT3, GPT4 and more models.
 
 ## Get started:
 
 ```
-py -m pip install --upgrade freeGPT
+python -m pip install --upgrade freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
 | gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
+| prodia   | [<prodia.com>](https://prodia.com/)                     |
+
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
@@ -36,25 +38,26 @@
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
 - [x] Make the overall library easier to understand.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
 - [x] Make a ChatUI.
-- [ ] Add an image generation model.
+- [x] Add an image generation model.
 
 ## Discord bot:
 
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - This bot has all the models in this repository available.
 - It's interactive, overall fast, and easy to use.
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
+**Text Completion:**
 ```python
 import freeGPT
 import asyncio
 
 
 async def main():
     while True:
@@ -65,10 +68,31 @@
         except Exception as e:
             print(f"🤖: {e}")
 
 
 asyncio.run(main())
 ```
 
+**Image Generation:**
+```python
+import freeGPT
+import asyncio
+from PIL import Image
+
+
+async def main():
+    while True:
+        prompt = input("👦: ")
+        try:
+            resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
+            Image.open(resp).show()
+            print(f"🤖: Image shown.")
+        except Exception as e:
+            print(f"🤖: {e}")
+
+
+asyncio.run(main())
+```
+
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.3/freeGPT/alpaca_7b.py` & `freeGPT-1.2.4/freeGPT/alpaca_7b.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.3/freeGPT/gpt3.py` & `freeGPT-1.2.4/freeGPT/gpt3.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.3/freeGPT/gpt4.py` & `freeGPT-1.2.4/freeGPT/gpt4.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.3/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.2.4/freeGPT.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.3
+Version: 1.2.4
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
@@ -31,28 +31,30 @@
 # freeGPT
 
 freeGPT provides free access to GPT3, GPT4 and more models.
 
 ## Get started:
 
 ```
-py -m pip install --upgrade freeGPT
+python -m pip install --upgrade freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
 | gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
+| prodia   | [<prodia.com>](https://prodia.com/)                     |
+
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
@@ -62,25 +64,26 @@
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
 - [x] Make the overall library easier to understand.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
 - [x] Make a ChatUI.
-- [ ] Add an image generation model.
+- [x] Add an image generation model.
 
 ## Discord bot:
 
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - This bot has all the models in this repository available.
 - It's interactive, overall fast, and easy to use.
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
+**Text Completion:**
 ```python
 import freeGPT
 import asyncio
 
 
 async def main():
     while True:
@@ -91,10 +94,31 @@
         except Exception as e:
             print(f"🤖: {e}")
 
 
 asyncio.run(main())
 ```
 
+**Image Generation:**
+```python
+import freeGPT
+import asyncio
+from PIL import Image
+
+
+async def main():
+    while True:
+        prompt = input("👦: ")
+        try:
+            resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
+            Image.open(resp).show()
+            print(f"🤖: Image shown.")
+        except Exception as e:
+            print(f"🤖: {e}")
+
+
+asyncio.run(main())
+```
+
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.3/setup.py` & `freeGPT-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.2.3",
+    version="1.2.4",
     description="freeGPT provides free access to GPT3, GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv2",
     keywords=[
```

