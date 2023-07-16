# Comparing `tmp/loopgpt-0.0.9.tar.gz` & `tmp/loopgpt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopgpt-0.0.9.tar", last modified: Sat Apr 22 04:21:17 2023, max compression
+gzip compressed data, was "loopgpt-0.1.0.tar", last modified: Sun Jul 16 21:00:21 2023, max compression
```

## Comparing `loopgpt-0.0.9.tar` & `loopgpt-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.375331 loopgpt-0.0.9/
--rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      114 2023-04-22 04:21:17.375331 loopgpt-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    10253 2023-04-21 10:41:18.000000 loopgpt-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.343342 loopgpt-0.0.9/loopgpt/
--rw-rw-rw-   0        0        0      974 2023-04-22 04:20:47.000000 loopgpt-0.0.9/loopgpt/__init__.py
--rw-rw-rw-   0        0        0    16210 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/agent.py
--rw-rw-rw-   0        0        0     3962 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.359335 loopgpt-0.0.9/loopgpt/embeddings/
--rw-rw-rw-   0        0        0      775 2023-04-21 11:42:59.000000 loopgpt-0.0.9/loopgpt/embeddings/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/embeddings/openai_.py
--rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/embeddings/provider.py
--rw-rw-rw-   0        0        0       87 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.359335 loopgpt-0.0.9/loopgpt/loops/
--rw-rw-rw-   0        0        0       36 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/loops/__init__.py
--rw-rw-rw-   0        0        0     1711 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/loops/cli.py
--rw-rw-rw-   0        0        0     7371 2023-04-21 20:31:54.000000 loopgpt-0.0.9/loopgpt/loops/repl.py
--rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.9/loopgpt/loops/ui.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.359335 loopgpt-0.0.9/loopgpt/memory/
--rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/memory/__init__.py
--rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/memory/base_memory.py
--rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/memory/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.367330 loopgpt-0.0.9/loopgpt/models/
--rw-rw-rw-   0        0        0       38 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/models/__init__.py
--rw-rw-rw-   0        0        0     1950 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/models/openai_.py
--rw-rw-rw-   0        0        0     1984 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.375331 loopgpt-0.0.9/loopgpt/tools/
--rw-rw-rw-   0        0        0     1450 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/agent_manager.py
--rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/tools/base_tool.py
--rw-rw-rw-   0        0        0     5445 2023-04-22 04:20:27.000000 loopgpt-0.0.9/loopgpt/tools/browser.py
--rw-rw-rw-   0        0        0     3731 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/tools/code.py
--rw-rw-rw-   0        0        0     2645 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/filesystem.py
--rw-rw-rw-   0        0        0     2006 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/google_search.py
--rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/tools/memory_manager.py
--rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.9/loopgpt/tools/shell.py
--rw-rw-rw-   0        0        0     3136 2023-04-21 11:42:59.000000 loopgpt-0.0.9/loopgpt/tools/simple_browser.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.375331 loopgpt-0.0.9/loopgpt/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/utils/__init__.py
--rw-rw-rw-   0        0        0     4174 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/utils/spinner.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.351330 loopgpt-0.0.9/loopgpt.egg-info/
--rw-rw-rw-   0        0        0      114 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 04:21:17.375331 loopgpt-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-04-22 04:20:53.000000 loopgpt-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.350788 loopgpt-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      134 2023-07-16 21:00:21.350788 loopgpt-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11405 2023-07-16 20:56:28.000000 loopgpt-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.319153 loopgpt-0.1.0/loopgpt/
+-rw-rw-rw-   0        0        0     1265 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/__init__.py
+-rw-rw-rw-   0        0        0    28523 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/agent.py
+-rw-rw-rw-   0        0        0    13224 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/aifunc.py
+-rw-rw-rw-   0        0        0     4260 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.334778 loopgpt-0.1.0/loopgpt/embeddings/
+-rw-rw-rw-   0        0        0      909 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     1689 2023-05-09 22:51:58.000000 loopgpt-0.1.0/loopgpt/embeddings/azure_openai.py
+-rw-rw-rw-   0        0        0      479 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/embeddings/base.py
+-rw-rw-rw-   0        0        0      997 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/embeddings/hf.py
+-rw-rw-rw-   0        0        0      972 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/embeddings/openai_.py
+-rw-rw-rw-   0        0        0       87 2023-04-21 10:41:18.000000 loopgpt-0.1.0/loopgpt/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.334778 loopgpt-0.1.0/loopgpt/loops/
+-rw-rw-rw-   0        0        0       36 2023-04-21 10:41:18.000000 loopgpt-0.1.0/loopgpt/loops/__init__.py
+-rw-rw-rw-   0        0        0     1940 2023-05-05 11:15:05.000000 loopgpt-0.1.0/loopgpt/loops/cli.py
+-rw-rw-rw-   0        0        0     7259 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/loops/repl.py
+-rw-rw-rw-   0        0        0     3108 2023-04-23 21:23:37.000000 loopgpt-0.1.0/loopgpt/loops/ui.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.334778 loopgpt-0.1.0/loopgpt/memory/
+-rw-rw-rw-   0        0        0      698 2023-06-28 08:46:45.000000 loopgpt-0.1.0/loopgpt/memory/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-04-28 15:54:23.000000 loopgpt-0.1.0/loopgpt/memory/base_memory.py
+-rw-rw-rw-   0        0        0     2126 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/memory/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.334778 loopgpt-0.1.0/loopgpt/models/
+-rw-rw-rw-   0        0        0      904 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/models/__init__.py
+-rw-rw-rw-   0        0        0     3985 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/models/azure_openai.py
+-rw-rw-rw-   0        0        0      681 2023-05-09 22:51:58.000000 loopgpt-0.1.0/loopgpt/models/base.py
+-rw-rw-rw-   0        0        0     3580 2023-04-28 15:54:23.000000 loopgpt-0.1.0/loopgpt/models/hf.py
+-rw-rw-rw-   0        0        0     3674 2023-04-28 15:54:23.000000 loopgpt-0.1.0/loopgpt/models/llama_cpp.py
+-rw-rw-rw-   0        0        0     2440 2023-05-17 13:53:08.000000 loopgpt-0.1.0/loopgpt/models/openai_.py
+-rw-rw-rw-   0        0        0      102 2023-04-28 15:54:23.000000 loopgpt-0.1.0/loopgpt/models/stable_lm.py
+-rw-rw-rw-   0        0        0     4032 2023-07-16 20:56:31.000000 loopgpt-0.1.0/loopgpt/summarizer.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.350788 loopgpt-0.1.0/loopgpt/tools/
+-rw-rw-rw-   0        0        0     1629 2023-04-30 10:36:08.000000 loopgpt-0.1.0/loopgpt/tools/__init__.py
+-rw-rw-rw-   0        0        0     2245 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/agent_manager.py
+-rw-rw-rw-   0        0        0     1067 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/base_tool.py
+-rw-rw-rw-   0        0        0     5772 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/browser.py
+-rw-rw-rw-   0        0        0     3294 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/code.py
+-rw-rw-rw-   0        0        0     4985 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/filesystem.py
+-rw-rw-rw-   0        0        0     2834 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/google_search.py
+-rw-rw-rw-   0        0        0      372 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/math.py
+-rw-rw-rw-   0        0        0      479 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/memory_manager.py
+-rw-rw-rw-   0        0        0      543 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/shell.py
+-rw-rw-rw-   0        0        0     1321 2023-04-28 15:54:23.000000 loopgpt-0.1.0/loopgpt/tools/simple_browser.py
+-rw-rw-rw-   0        0        0      438 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/tools/user_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.350788 loopgpt-0.1.0/loopgpt/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 10:41:18.000000 loopgpt-0.1.0/loopgpt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1184 2023-05-09 22:51:58.000000 loopgpt-0.1.0/loopgpt/utils/openai_key.py
+-rw-rw-rw-   0        0        0     4461 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/utils/spinner.py
+-rw-rw-rw-   0        0        0     1341 2023-07-16 20:56:28.000000 loopgpt-0.1.0/loopgpt/utils/text.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.319153 loopgpt-0.1.0/loopgpt.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-07-16 21:00:21.000000 loopgpt-0.1.0/loopgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-07-16 21:00:21.000000 loopgpt-0.1.0/loopgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 21:00:21.000000 loopgpt-0.1.0/loopgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-16 21:00:21.000000 loopgpt-0.1.0/loopgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      224 2023-07-16 21:00:21.000000 loopgpt-0.1.0/loopgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 21:00:21.000000 loopgpt-0.1.0/loopgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 21:00:21.350788 loopgpt-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-07-16 20:56:54.000000 loopgpt-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:00:21.350788 loopgpt-0.1.0/tests/
+-rw-rw-rw-   0        0        0      527 2023-05-05 11:15:05.000000 loopgpt-0.1.0/tests/test_keys.py
+-rw-rw-rw-   0        0        0     1904 2023-07-16 20:56:28.000000 loopgpt-0.1.0/tests/test_serde.py
```

### Comparing `loopgpt-0.0.9/LICENSE` & `loopgpt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.9/README.md` & `loopgpt-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -28,38 +28,72 @@
 *  **Full state serialization** - Pick up where you left off; L♾️pGPT can save the complete state of an agent, including memory and the states of its tools to a file or python object. No external databases or vector stores required (but they are still supported)!
 
 
 ## 🧑‍💻 Installation
 
 ### Install from PyPI
 
+📗 **This installs the latest stable version of L♾️pGPT. This is recommended for most users:**
+
 ```bash
 pip install loopgpt
 ```
 
+📕 The below two methods install the latest development version of L♾️pGPT. Note that this version maybe unstable:
+
 ### Install from source
 
 ```bash
 pip install git+https://www.github.com/farizrahman4u/loopgpt.git@main
 ```
 
 ### Install from source (dev)
 
 ```bash
-git clone https://www.github.com/farizrahman4u/loopgpt.git@main
-cd loopgpt
-python setup.py develop
+git clone https://www.github.com/farizrahman4u/loopgpt.git
+cd  loopgpt
+pip install -e .
+```
+
+### Install from source (dev) using Docker
+```bash
+git clone https://www.github.com/farizrahman4u/loopgpt.git
+cd  loopgpt
+docker build -t loopgpt:local-dev .
 ```
 
 ## 🏎️ Getting Started
 
-**You must set your OpenAI API Key 🔑 in your environment variables for anything to work. See the [Requirements secion](#-requirements) below.**
+### Setup your OpenAI API Key 🔑
+
+#### Option 1️⃣: Via a `.env` file
+
+Create a `.env` file in your current working directory (wherever you are going to run L♾️pGPT from) and add the following line to it:
+
+```bash
+OPENAI_API_KEY="<your-openai-api-key>"
+```
+
+🛑 **IMPORTANT** 🛑
+
+Windows users, please make sure "show file extensions" is enabled in your file explorer. Otherwise, your file will be named `.env.txt` instead of `.env`.
+
+#### Option 2️⃣: Via environment variables
+
+Set an environment variable called `OPENAI_API_KEY` to your OpenAI API Key.
+
+How to set environment variables:
+- [Windows](https://www.architectryan.com/2018/08/31/how-to-change-environment-variables-on-windows-10/)
+- [Linux](https://www.freecodecamp.org/news/how-to-set-an-environment-variable-in-linux/)
+- [Mac](https://phoenixnap.com/kb/set-environment-variable-mac)
 
 ### Create a new L♾️pGPT Agent🕵️:
 
+Let's create an agent in a new [Python](https://python.org) script.
+
 ```python
 from loopgpt.agent import Agent
 
 agent = Agent()
 ```
 
 L♾️pGPT uses `gpt-3.5-turbo` by default and all outputs shown here are made using it. GPT-4 users can set `model="gpt-4"` instead:
@@ -84,18 +118,24 @@
 
 And we're off! Let's run the Agent🕵️'s CLI:
 
 ```python
 agent.cli()
 ```
 
-You can exit the CLI by typing "exit".
+Save your Python file as `research_gpt.py` and run it:
+
+```bash
+python research_gpt.py
+```
 
 <img src="/docs/assets/imgs/loopgpt_demo_pic.png?raw=true" height="350">
 
+You can exit the CLI by typing "exit".
+
 ### 🔁 Continuous Mode 🔁
 
 If `continuous` is set to `True`, the agent will not ask for the user's permission to execute commands. It may go into infinite loops, so use it at your own risk!
 
 ```python
 agent.cli(continuous=True)
 ```
@@ -106,106 +146,121 @@
 
 ```bash
 loopgpt run
 ```
 
 Run `loopgpt --help` to see all the available options.
 
+### 🐋 Docker Mode
+
+You can run L♾️pGPT in the previously mentioned modes, using Docker:
+
+```bash
+# CLI mode
+docker run -i --rm loopgpt:local-dev loopgpt run
+
+# Script mode example
+docker run -i --rm -v "$(pwd)/scripts:/scripts" loopgpt:local-dev python /scripts/myscript.py
+
+```
+
 ## ⚒️ Adding custom tools ⚒️
 
 L♾️pGPT agents come with a set of builtin tools which allows them to perform various basic tasks such as searching the web, filesystem operations, etc. You can view these tools with `print(agent.tools)`.
 
 In addition to these builtin tools, you can also add your own tools to the agent's toolbox.
 
 ### Example: WeatherGPT 🌦️
 
 Let's create WeatherGPT, an AI assistant for all things weather.
 
-A tool inherits from `BaseTool` and you only need to override 3 methods to get your tool up and running!
-
-- `args`: A dictionary describing the tool's arguments and their descriptions.
-- `resp`: A dictionary describing the tool's response and their descriptions.
-- `run`: The tool's main logic. It takes the tool's arguments as input and returns the tool's response.
+A tool inherits from `BaseTool` and you only need to write a docstring to get your tool up and running!
 
 ```python
 from loopgpt.tools import BaseTool
 
 class GetWeather(BaseTool):
-    @property
-    def args(self):
-        return {"city": "name of the city"}
+    """Quickly get the weather for a given city
+
+    Args:
+        city (str): name of the city
     
-    @property
-    def resp(self):
-        return {"report": "The weather report for the city"}
+    Returns:
+        dict: The weather report for the city
+    """
     
     def run(self, city):
         ...
 ```
 
-L♾️pGPT gives a default ID and description to your tool but you can override them if you'd like:
+L♾️pGPT gives a default ID to your tool but you can override them if you'd like:
 
 ```python
 class GetWeather(BaseTool):
-    ...
+    """Quickly get the weather for a given city
+
+    Args:
+        city (str): name of the city
+    
+    Returns:
+        dict: The weather report for the city
+    """
 
     @property
     def id(self):
         return "get_weather_command"
-    
-    @property
-    def desc(self):
-        """A description is recommended so that the agent knows more about what the tool does"""
-        return "Quickly get the weather for a given city"
 ```
 
 Now let's define what our tool will do in its `run` method:
 
 ```python
 import requests
 
 # Define your custom tool
 class GetWeather(BaseTool):
-    ...
+    """Quickly get the weather for a given city
+
+    Args:
+        city (str): name of the city
+    
+    Returns:
+        dict: The weather report for the city
+    """
     
     def run(self, city):
         try:
             url = "https://wttr.in/{}?format=%l+%C+%h+%t+%w+%p+%P".format(city)
             data = requests.get(url).text.split(" ")
             keys = ("location", "condition", "humidity", "temperature", "wind", "precipitation", "pressure")
-            data = {"report": dict(zip(keys, data))}
+            data = dict(zip(keys, data))
             return data
         except Exception as e:
-            return {"report": f"An error occured while getting the weather: {e}."}
+            return f"An error occurred while getting the weather: {e}."
 ```
 
 That's it! You've built your first custom tool. Let's register it with a new agent and run it:
 
 ```python
+from loopgpt.tools import WriteToFile
 import loopgpt
 
+# Register custom tool type
+# This is actually not required here, but is required when you load a saved agent with custom tools.
+loopgpt.tools.register_tool_type(GetWeather)
+
 # Create Agent
-agent = loopgpt.Agent()
+agent = loopgpt.Agent(tools=[GetWeather, WriteToFile])
 agent.name = "WeatherGPT"
 agent.description = "an AI assistant that tells you the weather"
 agent.goals = [
     "Get the weather for NewYork and Beijing",
     "Give the user tips on how to dress for the weather in NewYork and Beijing",
     "Write the tips to a file called 'dressing_tips.txt'"
 ]
 
-
-# Register custom tool type
-# This is actually not required here, but is required when you load a saved agent with custom tools.
-loopgpt.tools.register_tool_type(GetWeather)
-
-# Register Tool
-weather_tool = GetWeather()
-agent.tools[weather_tool.id] = weather_tool
-
 # Run the agent's CLI
 agent.cli()
 ```
 
 Let's take a look at the `dressing_tips.txt` file that WeatherGPT wrote for us:
 
 dressing_tips.txt
@@ -277,19 +332,14 @@
 agent = loopgpt.Agent.from_config(agent_config)
 ```
 
 ## 📋 Requirements
 
 - Python 3.8+
 - [An OpenAI API Key](https://platform.openai.com/account/api-keys)
-    - Set environment variable `OPENAI_API_KEY` to the API key
-    - How to set environment variables:
-        - [Windows](https://www.architectryan.com/2018/08/31/how-to-change-environment-variables-on-windows-10/)
-        - [Linux](https://www.freecodecamp.org/news/how-to-set-an-environment-variable-in-linux/)
-        - [Mac](https://phoenixnap.com/kb/set-environment-variable-mac)
 - Google Chrome
 
 ### Optional Requirements
 
 For official google search support you will need to setup two environment variable keys `GOOGLE_API_KEY` and `CUSTOM_SEARCH_ENGINE_ID`, here is how to get them:
 
 1. Create an application on the [Google Developers Console][google-console].
@@ -308,7 +358,11 @@
 
 ## 🌳 Community
 
 Need help? Join our [Discord](https://discord.gg/rqs26cqx7v).
 
 [google-console]: https://console.developers.google.com
 [google-custom-search]: https://programmablesearchengine.google.com/controlpanel/create
+
+
+## ⭐ Star History 📈
+<img src="https://api.star-history.com/svg?repos=farizrahman4u/loopgpt&type=Date" alt= "Star History Chart" height="350">
```

#### html2text {}

```diff
@@ -11,115 +11,128 @@
 yet! * **Minimal prompt overhead** - Every token counts. We are continuously
 working on getting the best results with the least possible number of tokens. *
 **Human in the Loop** - Ability to "course correct" agents who go astray via
 human feedback. * **Full state serialization** - Pick up where you left off;
 Lâ¾ï¸pGPT can save the complete state of an agent, including memory and the
 states of its tools to a file or python object. No external databases or vector
 stores required (but they are still supported)! ## ð§âð» Installation ###
-Install from PyPI ```bash pip install loopgpt ``` ### Install from source
+Install from PyPI ð **This installs the latest stable version of
+Lâ¾ï¸pGPT. This is recommended for most users:** ```bash pip install loopgpt
+``` ð The below two methods install the latest development version of
+Lâ¾ï¸pGPT. Note that this version maybe unstable: ### Install from source
 ```bash pip install git+https://www.github.com/farizrahman4u/loopgpt.git@main
 ``` ### Install from source (dev) ```bash git clone https://www.github.com/
-farizrahman4u/loopgpt.git@main cd loopgpt python setup.py develop ``` ##
-ðï¸ Getting Started **You must set your OpenAI API Key ð in your
-environment variables for anything to work. See the [Requirements secion](#-
-requirements) below.** ### Create a new Lâ¾ï¸pGPT Agentðµï¸: ```python
-from loopgpt.agent import Agent agent = Agent() ``` Lâ¾ï¸pGPT uses `gpt-3.5-
-turbo` by default and all outputs shown here are made using it. GPT-4 users can
-set `model="gpt-4"` instead: ```python agent = Agent(model="gpt-4") ``` ###
-Setup the Agentðµï¸'s attributes: ```python agent.name = "ResearchGPT"
+farizrahman4u/loopgpt.git cd loopgpt pip install -e . ``` ### Install from
+source (dev) using Docker ```bash git clone https://www.github.com/
+farizrahman4u/loopgpt.git cd loopgpt docker build -t loopgpt:local-dev . ``` ##
+ðï¸ Getting Started ### Setup your OpenAI API Key ð #### Option 1ï¸â£:
+Via a `.env` file Create a `.env` file in your current working directory
+(wherever you are going to run Lâ¾ï¸pGPT from) and add the following line to
+it: ```bash OPENAI_API_KEY="" ``` ð **IMPORTANT** ð Windows users, please
+make sure "show file extensions" is enabled in your file explorer. Otherwise,
+your file will be named `.env.txt` instead of `.env`. #### Option 2ï¸â£: Via
+environment variables Set an environment variable called `OPENAI_API_KEY` to
+your OpenAI API Key. How to set environment variables: - [Windows](https://
+www.architectryan.com/2018/08/31/how-to-change-environment-variables-on-
+windows-10/) - [Linux](https://www.freecodecamp.org/news/how-to-set-an-
+environment-variable-in-linux/) - [Mac](https://phoenixnap.com/kb/set-
+environment-variable-mac) ### Create a new Lâ¾ï¸pGPT Agentðµï¸: Let's
+create an agent in a new [Python](https://python.org) script. ```python from
+loopgpt.agent import Agent agent = Agent() ``` Lâ¾ï¸pGPT uses `gpt-3.5-turbo`
+by default and all outputs shown here are made using it. GPT-4 users can set
+`model="gpt-4"` instead: ```python agent = Agent(model="gpt-4") ``` ### Setup
+the Agentðµï¸'s attributes: ```python agent.name = "ResearchGPT"
 agent.description = "an AI assistant that researches and finds the best tech
 products" agent.goals = [ "Search for the best headphones on Google", "Analyze
 specs, prices and reviews to find the top 5 best headphones", "Write the list
 of the top 5 best headphones and their prices to a file", "Summarize the pros
 and cons of each headphone and write it to a different file called
 'summary.txt'", ] ``` And we're off! Let's run the Agentðµï¸'s CLI:
-```python agent.cli() ``` You can exit the CLI by typing "exit". [/docs/assets/
-imgs/loopgpt_demo_pic.png?raw=true] ### ð Continuous Mode ð If
-`continuous` is set to `True`, the agent will not ask for the user's permission
-to execute commands. It may go into infinite loops, so use it at your own risk!
-```python agent.cli(continuous=True) ``` ### ð» Command Line Only Mode You
-can run Lâ¾ï¸pGPT directly from the command line without having to write any
-python code as well: ```bash loopgpt run ``` Run `loopgpt --help` to see all
-the available options. ## âï¸ Adding custom tools âï¸ Lâ¾ï¸pGPT agents
+```python agent.cli() ``` Save your Python file as `research_gpt.py` and run
+it: ```bash python research_gpt.py ``` [/docs/assets/imgs/
+loopgpt_demo_pic.png?raw=true] You can exit the CLI by typing "exit". ### ð
+Continuous Mode ð If `continuous` is set to `True`, the agent will not ask
+for the user's permission to execute commands. It may go into infinite loops,
+so use it at your own risk! ```python agent.cli(continuous=True) ``` ### ð»
+Command Line Only Mode You can run Lâ¾ï¸pGPT directly from the command line
+without having to write any python code as well: ```bash loopgpt run ``` Run
+`loopgpt --help` to see all the available options. ### ð Docker Mode You can
+run Lâ¾ï¸pGPT in the previously mentioned modes, using Docker: ```bash # CLI
+mode docker run -i --rm loopgpt:local-dev loopgpt run # Script mode example
+docker run -i --rm -v "$(pwd)/scripts:/scripts" loopgpt:local-dev python /
+scripts/myscript.py ``` ## âï¸ Adding custom tools âï¸ Lâ¾ï¸pGPT agents
 come with a set of builtin tools which allows them to perform various basic
 tasks such as searching the web, filesystem operations, etc. You can view these
 tools with `print(agent.tools)`. In addition to these builtin tools, you can
 also add your own tools to the agent's toolbox. ### Example: WeatherGPT ð¦ï¸
 Let's create WeatherGPT, an AI assistant for all things weather. A tool
-inherits from `BaseTool` and you only need to override 3 methods to get your
-tool up and running! - `args`: A dictionary describing the tool's arguments and
-their descriptions. - `resp`: A dictionary describing the tool's response and
-their descriptions. - `run`: The tool's main logic. It takes the tool's
-arguments as input and returns the tool's response. ```python from
-loopgpt.tools import BaseTool class GetWeather(BaseTool): @property def args
-(self): return {"city": "name of the city"} @property def resp(self): return
-{"report": "The weather report for the city"} def run(self, city): ... ```
-Lâ¾ï¸pGPT gives a default ID and description to your tool but you can
-override them if you'd like: ```python class GetWeather(BaseTool): ...
-@property def id(self): return "get_weather_command" @property def desc(self):
-"""A description is recommended so that the agent knows more about what the
-tool does""" return "Quickly get the weather for a given city" ``` Now let's
-define what our tool will do in its `run` method: ```python import requests #
-Define your custom tool class GetWeather(BaseTool): ... def run(self, city):
-try: url = "https://wttr.in/{}?format=%l+%C+%h+%t+%w+%p+%P".format(city) data =
-requests.get(url).text.split(" ") keys = ("location", "condition", "humidity",
-"temperature", "wind", "precipitation", "pressure") data = {"report": dict(zip
-(keys, data))} return data except Exception as e: return {"report": f"An error
-occured while getting the weather: {e}."} ``` That's it! You've built your
-first custom tool. Let's register it with a new agent and run it: ```python
-import loopgpt # Create Agent agent = loopgpt.Agent() agent.name = "WeatherGPT"
+inherits from `BaseTool` and you only need to write a docstring to get your
+tool up and running! ```python from loopgpt.tools import BaseTool class
+GetWeather(BaseTool): """Quickly get the weather for a given city Args: city
+(str): name of the city Returns: dict: The weather report for the city """ def
+run(self, city): ... ``` Lâ¾ï¸pGPT gives a default ID to your tool but you
+can override them if you'd like: ```python class GetWeather(BaseTool):
+"""Quickly get the weather for a given city Args: city (str): name of the city
+Returns: dict: The weather report for the city """ @property def id(self):
+return "get_weather_command" ``` Now let's define what our tool will do in its
+`run` method: ```python import requests # Define your custom tool class
+GetWeather(BaseTool): """Quickly get the weather for a given city Args: city
+(str): name of the city Returns: dict: The weather report for the city """ def
+run(self, city): try: url = "https://wttr.in/
+{}?format=%l+%C+%h+%t+%w+%p+%P".format(city) data = requests.get
+(url).text.split(" ") keys = ("location", "condition", "humidity",
+"temperature", "wind", "precipitation", "pressure") data = dict(zip(keys,
+data)) return data except Exception as e: return f"An error occurred while
+getting the weather: {e}." ``` That's it! You've built your first custom tool.
+Let's register it with a new agent and run it: ```python from loopgpt.tools
+import WriteToFile import loopgpt # Register custom tool type # This is
+actually not required here, but is required when you load a saved agent with
+custom tools. loopgpt.tools.register_tool_type(GetWeather) # Create Agent agent
+= loopgpt.Agent(tools=[GetWeather, WriteToFile]) agent.name = "WeatherGPT"
 agent.description = "an AI assistant that tells you the weather" agent.goals =
 [ "Get the weather for NewYork and Beijing", "Give the user tips on how to
 dress for the weather in NewYork and Beijing", "Write the tips to a file called
-'dressing_tips.txt'" ] # Register custom tool type # This is actually not
-required here, but is required when you load a saved agent with custom tools.
-loopgpt.tools.register_tool_type(GetWeather) # Register Tool weather_tool =
-GetWeather() agent.tools[weather_tool.id] = weather_tool # Run the agent's CLI
-agent.cli() ``` Let's take a look at the `dressing_tips.txt` file that
-WeatherGPT wrote for us: dressing_tips.txt ``` - It's Clear outside with a
-temperature of +10Â°C in Beijing. Wearing a light jacket and pants is
-recommended. - It's Overcast outside with a temperature of +11Â°C in New York.
-Wearing a light jacket, pants, and an umbrella is recommended. ``` ## ð¢
-Course Correction Unlike Auto-GPT, the agent does not terminate when the user
-denies the execution of a command. Instead it asks the user for feedback to
-correct its course. To correct the agent's course, just deny execution and
-provide feedback: [/docs/assets/imgs/course_correction_1.png?raw=true] The
-agent has updated its course of action: [/docs/assets/imgs/
-course_correction_2.png?raw=true] ## ð¾ Saving and Loading Agent State ð¾
-You can save an agent's state to a json file with: ```python agent.save
-("ResearchGPT.json") ``` This saves the agent's configuration (model, name,
-description etc) as well as its internal state (conversation state, memory,
-tool states etc). You can also save just the confifguration by passing
+'dressing_tips.txt'" ] # Run the agent's CLI agent.cli() ``` Let's take a look
+at the `dressing_tips.txt` file that WeatherGPT wrote for us: dressing_tips.txt
+``` - It's Clear outside with a temperature of +10Â°C in Beijing. Wearing a
+light jacket and pants is recommended. - It's Overcast outside with a
+temperature of +11Â°C in New York. Wearing a light jacket, pants, and an
+umbrella is recommended. ``` ## ð¢ Course Correction Unlike Auto-GPT, the
+agent does not terminate when the user denies the execution of a command.
+Instead it asks the user for feedback to correct its course. To correct the
+agent's course, just deny execution and provide feedback: [/docs/assets/imgs/
+course_correction_1.png?raw=true] The agent has updated its course of action:
+[/docs/assets/imgs/course_correction_2.png?raw=true] ## ð¾ Saving and Loading
+Agent State ð¾ You can save an agent's state to a json file with: ```python
+agent.save("ResearchGPT.json") ``` This saves the agent's configuration (model,
+name, description etc) as well as its internal state (conversation state,
+memory, tool states etc). You can also save just the confifguration by passing
 `include_state=False` to `agent.save()`: ```python agent.save
 ("ResearchGPT.json", include_state=False) ``` Then pick up where you left off
 with: ```python import loopgpt agent = loopgpt.Agent.load("ResearchGPT.json")
 agent.cli() ``` or by running the saved agent from the command line: ```bash
 loopgpt run ResearchGPT.json ``` You can convert the agent state to a json
 compatible python dictionary instead of writing to a file: ```python
 agent_config = agent.config() ``` To get just the configuration without the
 internal state: ```python agent_config = agent.config(include_state=False) ```
 To reload the agent from the config, use: ```python import loopgpt agent =
 loopgpt.Agent.from_config(agent_config) ``` ## ð Requirements - Python 3.8+
-- [An OpenAI API Key](https://platform.openai.com/account/api-keys) - Set
-environment variable `OPENAI_API_KEY` to the API key - How to set environment
-variables: - [Windows](https://www.architectryan.com/2018/08/31/how-to-change-
-environment-variables-on-windows-10/) - [Linux](https://www.freecodecamp.org/
-news/how-to-set-an-environment-variable-in-linux/) - [Mac](https://
-phoenixnap.com/kb/set-environment-variable-mac) - Google Chrome ### Optional
-Requirements For official google search support you will need to setup two
-environment variable keys `GOOGLE_API_KEY` and `CUSTOM_SEARCH_ENGINE_ID`, here
-is how to get them: 1. Create an application on the [Google Developers Console]
-[google-console]. 2. Create your custom search engine using [Google Custom
-Search][google-custom-search]. 3. Once your custom search engine is created,
-select it and get into the details page of the search engine. - On the "Basic"
-section, you will find the "Search engine ID" field, that value is what you
-will use for the `CUSTOM_SEARCH_ENGINE_ID` environment variable. - Now go to
-the "Programmatic Access" section at the bottom of the page. - Create a "Custom
-Search JSON API" - Follow the dialog by selecting the application you created
-on step #1 and when you get your API key use it to populate the
-`GOOGLE_API_KEY` environment variable. â¹ï¸ In case these are absent,
-Lâ¾ï¸pGPT will fall back to using [DuckDuckGo Search](https://pypi.org/
-project/duckduckgo-search/). ## ð Contribute We need A LOT of Help! Please
-open an issue or a PR if you'd like to contribute. ## ð³ Community Need help?
-Join our [Discord](https://discord.gg/rqs26cqx7v). [google-console]: https://
-console.developers.google.com [google-custom-search]: https://
-programmablesearchengine.google.com/controlpanel/create
+- [An OpenAI API Key](https://platform.openai.com/account/api-keys) - Google
+Chrome ### Optional Requirements For official google search support you will
+need to setup two environment variable keys `GOOGLE_API_KEY` and
+`CUSTOM_SEARCH_ENGINE_ID`, here is how to get them: 1. Create an application on
+the [Google Developers Console][google-console]. 2. Create your custom search
+engine using [Google Custom Search][google-custom-search]. 3. Once your custom
+search engine is created, select it and get into the details page of the search
+engine. - On the "Basic" section, you will find the "Search engine ID" field,
+that value is what you will use for the `CUSTOM_SEARCH_ENGINE_ID` environment
+variable. - Now go to the "Programmatic Access" section at the bottom of the
+page. - Create a "Custom Search JSON API" - Follow the dialog by selecting the
+application you created on step #1 and when you get your API key use it to
+populate the `GOOGLE_API_KEY` environment variable. â¹ï¸ In case these are
+absent, Lâ¾ï¸pGPT will fall back to using [DuckDuckGo Search](https://
+pypi.org/project/duckduckgo-search/). ## ð Contribute We need A LOT of Help!
+Please open an issue or a PR if you'd like to contribute. ## ð³ Community
+Need help? Join our [Discord](https://discord.gg/rqs26cqx7v). [google-console]:
+https://console.developers.google.com [google-custom-search]: https://
+programmablesearchengine.google.com/controlpanel/create ## â­ Star History
+ð [Star History Chart]
```

### Comparing `loopgpt-0.0.9/loopgpt/__init__.py` & `loopgpt-0.1.0/loopgpt/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,44 @@
-__version__ = "0.0.9"
+"""LoopGPT is a modular Auto-GPT framework
+"""
 
+__version__ = "0.1.0"
 
-from loopgpt.agent import Agent
+
+from loopgpt.agent import Agent, empty_agent
 from loopgpt.tools import *
 from loopgpt.memory import *
 from loopgpt.embeddings import *
+from loopgpt.aifunc import aifunc
 
 agent_from_config = Agent.from_config
 from loopgpt.tools import from_config as tool_from_config
 from loopgpt.memory import from_config as memory_from_config
 from loopgpt.embeddings import from_config as embedding_provider_from_config
 
-from loopgpt.logger import logger
-from colorama import Fore, Style
+from loopgpt.utils.openai_key import check_openai_key
+from dotenv import load_dotenv
 
-import os
+import sys
 
 
-def check_openai_key():
-    if "OPENAI_API_KEY" not in os.environ:
-        logger.warn(
-            f"{Fore.RED}WARNING: OpenAI API Key not found. Please set the `OPENAI_API_KEY` environment variable. "
-            f"LoopGPT cannot work without it. "
-            f"See https://github.com/farizrahman4u/loopgpt#-requirements for more details{Style.RESET_ALL}"
-        )
+load_dotenv()
 
 
 def from_config(config):
     return globals()[config["type"] + "_from_config"](config)
 
 
-check_openai_key()
+def set_aifunc_args(model, embedding_provider):
+    """Set the model and embedding provider that will be used by :class:`~loopgpt.aifunc.aifunc` to create agents when needed.
+
+    :param model: The model to use.
+    :type model: ~loopgpt.models.base.BaseModel
+    :param embedding_provider: The embedding provider to use.
+    :type embedding_provider: ~loopgpt.embeddings.base.BaseEmbeddingProvider
+    """
+    aifunc.model = model
+    aifunc.embedding_provider = embedding_provider
+
+
+if "pytest" not in sys.modules:
+    check_openai_key()
```

### Comparing `loopgpt-0.0.9/loopgpt/agent.py` & `loopgpt-0.1.0/loopgpt/agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,328 @@
 from loopgpt.constants import (
     DEFAULT_RESPONSE_FORMAT_,
     INIT_PROMPT,
     DEFAULT_AGENT_NAME,
     DEFAULT_AGENT_DESCRIPTION,
     NEXT_PROMPT,
-    NEXT_PROMPT_SMALL,
+    DEFAULT_PROMPT_TEMPLATE,
+    AgentStates,
 )
 from loopgpt.memory import from_config as memory_from_config
-from loopgpt.models.openai_ import chat, count_tokens, get_token_limit
+from loopgpt.models import (
+    OpenAIModel,
+    AzureOpenAIModel,
+    from_config as model_from_config,
+)
 from loopgpt.tools import builtin_tools, from_config as tool_from_config
 from loopgpt.tools.code import ai_function
 from loopgpt.memory.local_memory import LocalMemory
-from loopgpt.embeddings.openai_ import OpenAIEmbeddingProvider
+from loopgpt.embeddings import OpenAIEmbeddingProvider, AzureOpenAIEmbeddingProvider
 from loopgpt.utils.spinner import spinner
 from loopgpt.loops import cli
 
 
 from typing import *
+from itertools import repeat
+from contextlib import contextmanager
 
+import openai
 import json
 import time
 import ast
+import re
+import os
+
+ACTIVE_AGENT = None
 
 
 class Agent:
+    """Creates a new LoopGPT agent.
+
+    :param name: The name of the agent. Defaults to AGENT_NAME.
+    :type name: str, optional
+    :param description: A description of the agent. Defaults to DEFAULT_AGENT_DESCRIPTION.
+    :type description: str, optional
+    :param goals: A list of goals for the agent. Defaults to None.
+    :type goals: list, optional
+    :param model: The model to use for the agent.
+        Strings are accepted only for OpenAI models. Specify a :class:`~loopgpt.models.base.BaseModel` object for other models.
+        Defaults to "gpt-3.5-turbo".
+    :type model: str, :class:`~loopgpt.models.base.BaseModel`, optional
+    :param embedding_provider: The embedding provider to use for the agent.
+        Defaults to :class:`~loopgpt.embeddings.OpenAIEmbeddingProvider`.
+        Specify a :class:`~loopgpt.embeddings.base.BaseEmbeddingProvider` object to use other embedding providers.
+    :type embedding_provider: :class:`~loopgpt.embeddings.base.BaseEmbeddingProvider`, optional
+    :param temperature: The temperature to use for agent's chat completion. Defaults to 0.8.
+    :type temperature: float, optional
+    """
+
     def __init__(
         self,
         name=DEFAULT_AGENT_NAME,
         description=DEFAULT_AGENT_DESCRIPTION,
         goals=None,
-        model="gpt-3.5-turbo",
+        model=None,
+        embedding_provider=None,
         temperature=0.8,
+        tools=None,
     ):
+        if openai.api_type == "azure":
+            if model is None:
+                raise ValueError(
+                    "You must provide an AzureOpenAIModel to the `model` argument when using the OpenAI Azure API"
+                )
+            if embedding_provider is None:
+                raise ValueError(
+                    "You must provide a deployed embedding provider to the `embedding_provider` argument when using the OpenAI Azure API"
+                )
+
+        if model is None:
+            model = OpenAIModel("gpt-3.5-turbo")
+        elif isinstance(model, str):
+            model = OpenAIModel(model)
+
+        if embedding_provider is None:
+            embedding_provider = OpenAIEmbeddingProvider()
+
         self.name = name
         self.description = description
         self.goals = goals or []
         self.model = model
+        self.embedding_provider = embedding_provider
         self.temperature = temperature
         self.sub_agents = {}
-        self.memory = LocalMemory(embedding_provider=OpenAIEmbeddingProvider())
+        self.memory = LocalMemory(embedding_provider=embedding_provider)
         self.history = []
-        tools = [tool_type() for tool_type in builtin_tools()]
+        if tools is None:
+            tools = [tool_type() for tool_type in builtin_tools()]
+        else:
+            tools = [tool_type() for tool_type in tools]
         self.tools = {tool.id: tool for tool in tools}
         self.staging_tool = None
         self.staging_response = None
         self.tool_response = None
-        self.init_prompt = INIT_PROMPT
-        self.next_prompt = NEXT_PROMPT
+        self.prompts = [INIT_PROMPT, NEXT_PROMPT]
+        self.prompt_gen = self.next_prompt()
+        self.prompt_template = DEFAULT_PROMPT_TEMPLATE
+        self.progress = []
+        self.plan = []
+        self.constraints = []
+        self.state = AgentStates.START
+        self.memory_query = None
+        self.additional_history = None
+
+    def next_prompt(self):
+        if self.prompts:
+            yield from self.prompts
+            yield from repeat(self.prompts[-1])
+        else:
+            yield from repeat("")
 
     def _get_non_user_messages(self, n):
         msgs = [
             msg
             for msg in self.history
             if msg["role"] != "user"
             and not (msg["role"] == "system" and "do_nothing" in msg["content"])
         ]
-        return msgs[-n - 1 : -1]
+        return msgs[-n - 1 :]
 
     def get_full_prompt(self, user_input: str = ""):
-        header = {"role": "system", "content": self.header_prompt()}
-        dtime = {
-            "role": "system",
-            "content": f"The current time and date is {time.strftime('%c')}",
-        }
-        prompt = [header, dtime]
-        msgs = self._get_non_user_messages(10)
-        relevant_memory = self.memory.get(str(msgs), 5) if len(msgs) > 5 else []
-        memory_added = False
-        if relevant_memory:
-            # Add as many documents from memory as possible while staying under the token limit
-            token_limit = 1500
-            while relevant_memory:
-                memstr = "\n".join(relevant_memory)
-                context = {
+        sections = re.findall(r"<(.*)>", self.prompt_template)
+        user_prompt = [{"role": "user", "content": user_input}]
+        # history = self.history[:]
+        history = self._get_compressed_history()
+        relevant_memory = []
+        for section in sections:
+            if section == "HEADER":
+                header = {"role": "system", "content": self.header_prompt()}
+                dtime = {
                     "role": "system",
-                    "content": f"This reminds you of these events from your past:\n{memstr}\n",
+                    "content": f"The current time and date is {time.strftime('%c')}",
                 }
-                token_count = count_tokens(prompt + [context], model=self.model)
-                if token_count < token_limit:
+            elif section.startswith("MEMORY"):
+                if self.memory_query:
+                    memory_query = self.memory_query
+                else:
+                    n = None
+                    if ":" in section:
+                        section, n = section.split(":")
+                        n = int(n)
+                    mem_source = self._get_non_user_messages(n) + user_prompt
+                    memory_query = "\n".join([hist["content"] for hist in mem_source])
+                relevant_memory = self.memory.get(memory_query, 10)
+
+        def _msgs():
+            updated_msgs = []
+            for section in sections:
+                if section == "HEADER":
+                    updated_msgs += [header, dtime]
+                if section.startswith("HISTORY"):
+                    updated_msgs += history[:]
+                elif section.startswith("MEMORY"):
+                    if relevant_memory:
+                        memstr = "\n".join(relevant_memory)
+                        context = {
+                            "role": "system",
+                            "content": (
+                                f"Remember the following things in your memory:"
+                                + "\n=============================MEMORY=============================\n"
+                                + f"\n{memstr}\n"
+                                + "================================================================\n"
+                            ),
+                        }
+                        updated_msgs.append(context)
+                elif section == "USER_INPUT":
+                    updated_msgs += user_prompt
+            return updated_msgs
+
+        maxtokens = self.model.get_token_limit() - 1000
+        while True:
+            msgs = _msgs()
+            ntokens = self.model.count_tokens(msgs)
+            if ntokens < maxtokens:
+                break
+            else:
+                if len(history) > 1:
+                    history = history[1:]
+                elif relevant_memory:
+                    relevant_memory = relevant_memory[1:]
+                else:
                     break
-                relevant_memory = relevant_memory[:-1]
-            if relevant_memory:
-                memory_added = True
-                prompt.append(context)
-        history = self._get_compressed_history()
-        user_prompt = [{"role": "user", "content": user_input}] if user_input else []
-        prompt = prompt[:2] + history + prompt[2:]
-        token_limit = get_token_limit(self.model) - 1000  # 1000 reserved for response
-        token_count = count_tokens(prompt + user_prompt, model=self.model)
-        while history[:-1] and token_count > token_limit:
-            history = history[1:]
-            prompt.pop(2)
-            token_count = count_tokens(prompt + user_prompt, model=self.model)
-        if memory_added and len(prompt) > 4:
-            sys_resp = prompt.pop(-2)
-            agent_resp = prompt.pop(-2)
-            prompt.append(agent_resp)
-            prompt.append(sys_resp)
-        prompt += user_prompt
-        return prompt, token_count
+        return msgs, ntokens
 
     def _get_compressed_history(self):
         hist = self.history[:]
         system_msgs = [i for i in range(len(hist)) if hist[i]["role"] == "system"]
-        for i in system_msgs[:-1]:
-            entry = hist[i].copy()
-            msg = entry["content"]
-            if msg.startswith("Response from "):
-                tool = msg[len("Response from ") :].split(":", 1)[0]
-                entry["content"] = f"<Response from {tool}>"
-                hist[i] = entry
         assist_msgs = [i for i in range(len(hist)) if hist[i]["role"] == "assistant"]
-        for i in assist_msgs[:-1]:
+        for i in assist_msgs:
             entry = hist[i].copy()
             try:
                 respd = json.loads(entry["content"])
                 thoughts = respd.get("thoughts")
                 if thoughts:
                     thoughts.pop("reasoning", None)
                     thoughts.pop("speak", None)
-                    thoughts.pop("criticism", None)
-                    # if False and i < len(assist_msgs) - 2:
                     thoughts.pop("text", None)
+                    thoughts.pop("plan", None)
                 entry["content"] = json.dumps(respd, indent=2)
                 hist[i] = entry
             except:
                 pass
         user_msgs = [i for i in range(len(hist)) if hist[i]["role"] == "user"]
-        for i in user_msgs:
-            entry = hist[i].copy()
-            msg = entry["content"]
-            if msg in [self.next_prompt, self.init_prompt]:
-                entry["content"] = NEXT_PROMPT_SMALL
-                hist[i] = entry
+        hist = [hist[i] for i in range(len(hist)) if i not in user_msgs]
         return hist
 
+    def _get_compressed_history(self):
+        history = self._get_non_user_messages(30)
+        maxtokens = self.model.get_token_limit()
+        while True:
+            message = [
+                {
+                    "role": "user",
+                    "content": (
+                        f"Please summarize this conversation for me:\n{history}\n\nImportant Details and Results:"
+                        + "\n- Include key findings from the research and data collection phases.\n- Highlight important commands"
+                        + "executed and their results.\n\nKey Highlights:\n- Summarize the main points of the conversation in bullet points."
+                        + "\n- Focus on relevant information and filter out redundant exchanges.\n\nAdditional Context:\n- Provide any relevant links"
+                        + " or references mentioned during the conversation.\n\nPlease ensure the summary accurately captures the essential aspects of"
+                        + " the task and includes details that are crucial for understanding the context and progress.\n\nThank you!"
+                    ),
+                }
+            ]
+            ntokens = self.model.count_tokens(message)
+            if ntokens < maxtokens:
+                break
+            else:
+                history.pop(0)
+
+        if len(history) == 0:
+            history = []
+        else:
+            history_summary = self.model.chat(message)
+            history = [{"role": "system", "content": history_summary}]
+        if self.additional_history:
+            history += [
+                {"role": role, "content": content}
+                for role, content in self.additional_history.items()
+            ]
+        return history
+
+    def get_full_message(self, message: Optional[str]):
+        return next(self.prompt_gen) + "\n\n" + (message or "")
+
+    def _default_response_callback(self, resp):
+        try:
+            resp = self._load_json(resp)
+            plan = resp.get("plan")
+            if plan and isinstance(plan, list):
+                if (
+                    len(plan) == 0
+                    or len(plan) == 1
+                    and len(plan[0].replace("-", "")) == 0
+                ):
+                    self.staging_tool = {"name": "task_complete", "args": {}}
+                    self.staging_response = resp
+                    self.state = AgentStates.STOP
+            else:
+                if isinstance(resp, dict):
+                    if "name" in resp:
+                        resp = {"command": resp}
+                    if "command" in resp:
+                        self.staging_tool = resp["command"]
+                        self.staging_response = resp
+                        self.state = AgentStates.TOOL_STAGED
+                    else:
+                        self.state = AgentStates.IDLE
+                else:
+                    self.state = AgentStates.IDLE
+
+            progress = resp.get("thoughts", {}).get("progress")
+            if progress:
+                if isinstance(plan, str):
+                    self.progress += [progress]
+                elif isinstance(progress, list):
+                    self.progress += progress
+            plan = resp.get("thoughts", {}).get("plan")
+            if plan:
+                if isinstance(plan, str):
+                    self.plan = [plan]
+                if isinstance(plan, list):
+                    self.plan = plan
+            return resp
+        except:
+            raise
+
     @spinner
-    def chat(self, message: Optional[str] = None, run_tool=False) -> Union[str, Dict]:
-        if message is None:
-            message = self.init_prompt
+    def chat(
+        self, message: Optional[str] = None, run_tool=False, response_callback=-1
+    ) -> Optional[Union[str, Dict]]:
+        if response_callback == -1:
+            response_callback = self._default_response_callback
+        if self.state == AgentStates.STOP:
+            raise ValueError(
+                "This agent has completed its tasks. It will not accept any more messages."
+                " You can do `agent.clear_state()` to start over with the same goals."
+            )
+        message = self.get_full_message(message)
         if self.staging_tool:
             tool = self.staging_tool
             if run_tool:
+                output = self.run_staging_tool()
+                self.tool_response = output
                 if tool.get("name") == "task_complete":
                     self.history.append(
                         {
                             "role": "system",
                             "content": "Completed all user specified tasks.",
                         }
                     )
-                    message = ""
-                output = self.run_staging_tool()
-                self.tool_response = output
+                    self.state = AgentStates.STOP
+                    return
                 if tool.get("name") != "do_nothing":
                     pass
                     # TODO We dont have enough space for this in gpt3
                     # self.memory.add(
                     #     f"Command \"{tool['name']}\" with args {tool['args']} returned :\n {output}"
                     # )
             else:
@@ -167,50 +334,47 @@
                 )
                 # self.memory.add(
                 #     f"User disapproved running command \"{tool['name']}\" with args {tool['args']} with following feedback\n: {message}"
                 # )
             self.staging_tool = None
             self.staging_response = None
         full_prompt, token_count = self.get_full_prompt(message)
-        token_limit = get_token_limit(self.model)
-        maxt_tokens = max(1000, token_limit - token_count)
-        resp = chat(
+        token_limit = self.model.get_token_limit()
+        max_tokens = min(1000, max(token_limit - token_count, 0))
+        assert max_tokens
+        # print("================================")
+        # print(full_prompt)
+        # print("================================")
+        resp = self.model.chat(
             full_prompt,
-            model=self.model,
-            max_tokens=maxt_tokens,
+            max_tokens=max_tokens,
             temperature=self.temperature,
         )
-        try:
-            resp = self._load_json(resp)
-            if "name" in resp:
-                resp = {"command": resp}
-            self.staging_tool = resp["command"]
-            self.staging_response = resp
-        except Exception as e:
-            pass
+        if response_callback:
+            resp = response_callback(resp)
+        if self.state == AgentStates.START:
+            self.state = AgentStates.IDLE
         self.history.append({"role": "user", "content": message})
         self.history.append(
             {
                 "role": "assistant",
-                "content": json.dumps(resp) if isinstance(resp, dict) else resp,
+                "content": json.dumps(resp) if isinstance(resp, dict) else str(resp),
             }
         )
         return resp
 
     def _extract_json_with_gpt(self, s):
         func = "def convert_to_json(response: str) -> str:"
         desc = f"""Convert the given string to a JSON string of the form \n{json.dumps(DEFAULT_RESPONSE_FORMAT_, indent=4)}\nEnsure the result can be parsed by Python json.loads."""
-        res = ai_function(func, desc, [s])
+        res = ai_function(func, desc, [s], self.model)
         return res
 
     def _load_json(self, s, try_gpt=True):
         if "Result: {" in s:
             s = s.split("Result: ", 1)[0]
-        if "{" not in s or "}" not in s:
-            raise Exception()
         try:
             return json.loads(s)
         except Exception:
             s = s[s.find("{") : s.rfind("}") + 1]
             try:
                 return json.loads(s)
             except Exception:
@@ -297,58 +461,83 @@
         )
         return resp
 
     def clear_state(self):
         self.staging_tool = None
         self.staging_response = None
         self.tool_response = None
+        self.progress = []
+        self.state = AgentStates.START
         self.history.clear()
         self.sub_agents.clear()
         self.memory.clear()
+        self.plan.clear()
 
     def header_prompt(self):
         prompt = []
         prompt.append(self.persona_prompt())
         if self.tools:
             prompt.append(self.tools_prompt())
         if self.goals:
             prompt.append(self.goals_prompt())
+        if self.constraints:
+            prompt.append(self.constraints_prompt())
+        if self.plan:
+            prompt.append(self.plan_prompt())
+        if self.progress:
+            prompt.append(self.progress_prompt())
         return "\n".join(prompt) + "\n"
 
     def persona_prompt(self):
         return f"You are {self.name}, {self.description}."
 
+    def progress_prompt(self):
+        prompt = []
+        prompt.append(f"PROGRESS SO FAR:")
+        for i, p in enumerate(self.progress):
+            prompt.append(f"{i + 1}. DONE - {p}")
+        return "\n".join(prompt) + "\n"
+
+    def plan_prompt(self):
+        plan = "\n".join(self.plan)
+        return f"CURRENT PLAN:\n{plan}\n"
+
     def goals_prompt(self):
         prompt = []
         prompt.append(f"GOALS:")
         for i, g in enumerate(self.goals):
             prompt.append(f"{i + 1}. {g}")
         return "\n".join(prompt) + "\n"
 
-    def tools_prompt(self):
+    def constraints_prompt(self):
+        prompt = []
+        prompt.append(f"CONSTRAINTS:")
+        for i, c in enumerate(self.constraints):
+            prompt.append(f"{i + 1}. {c}")
+        return "\n".join(prompt) + "\n"
+
+    def tools_prompt(self, extras=False):
         prompt = []
-        prompt.append("Commands:")
+        prompt.append("The following commands are already defined for you:")
         for i, tool in enumerate(self.tools.values()):
             tool.agent = self
-            prompt.append(f"{i + 1}. {tool.prompt()}")
-        task_complete_command = {
-            "name": "task_complete",
-            "description": "Execute when all tasks are completed.",
-            "args": {},
-            "response_format": {"success": "true"},
-        }
-        do_nothing_command = {
-            "name": "do_nothing",
-            "description": "Do nothing.",
-            "args": {},
-            "response_format": {"response": "Nothing Done."},
-        }
-        prompt.append(f"{i + 2}. {json.dumps(task_complete_command)}")
-        prompt.append(f"{i + 3}. {json.dumps(do_nothing_command)}")
-        return "\n".join(prompt) + "\n"
+            prompt.append(tool.prompt())
+
+        if extras:
+            task_complete_command = (
+                f'def task_complete():\n\t"""{task_complete.__doc__}\n\t"""'.expandtabs(
+                    4
+                )
+            )
+            do_nothing_command = (
+                f'def do_nothing():\n\t"""{do_nothing.__doc__}\n\t"""'.expandtabs(4)
+            )
+            prompt.append(task_complete_command)
+            prompt.append(do_nothing_command)
+        return "\n\n".join(prompt) + "\n"
 
     def resources_prompt(self):
         prompt = []
         prompt.append("Resources:")
         for i, res in enumerate(self.resources):
             prompt.append(f"{i + 1}. {res}")
         return "\n".join(prompt) + "\n"
@@ -356,22 +545,28 @@
     def config(self, include_state=True):
         cfg = {
             "class": self.__class__.__name__,
             "type": "agent",
             "name": self.name,
             "description": self.description,
             "goals": self.goals[:],
-            "model": self.model,
+            "constraints": self.constraints[:],
+            "state": self.state,
+            "model": self.model.config(),
             "temperature": self.temperature,
             "tools": [tool.config() for tool in self.tools.values()],
         }
         if include_state:
             cfg.update(
                 {
-                    "sub_agents": {k: (v[0].config(), v[1]) for k, v in self.sub_agents.items()},
+                    "progress": self.progress[:],
+                    "plan": self.plan[:],
+                    "sub_agents": {
+                        k: (v[0].config(), v[1]) for k, v in self.sub_agents.items()
+                    },
                     "history": self.history[:],
                     "memory": self.memory.config(),
                     "staging_tool": self.staging_tool,
                     "staging_response": self.staging_response,
                     "tool_response": self.tool_response,
                 }
             )
@@ -379,19 +574,24 @@
 
     @classmethod
     def from_config(cls, config):
         agent = cls()
         agent.name = config["name"]
         agent.description = config["description"]
         agent.goals = config["goals"][:]
+        agent.constraints = config["constraints"][:]
+        agent.state = config["state"]
         agent.temperature = config["temperature"]
-        agent.model = config["model"]
+        agent.model = model_from_config(config["model"])
         agent.tools = {tool.id: tool for tool in map(tool_from_config, config["tools"])}
+        agent.progress = config.get("progress", [])
+        agent.plan = config.get("plan", [])
         agent.sub_agents = {
-            k: (cls.from_config(v[0]), v[1]) for k, v in config.get("sub_agents", {}).items()
+            k: (cls.from_config(v[0]), v[1])
+            for k, v in config.get("sub_agents", {}).items()
         }
         agent.history = config.get("history", [])
         memory = config.get("memory")
         if memory:
             agent.memory = memory_from_config(memory)
         agent.staging_tool = config.get("staging_tool")
         agent.staging_response = config.get("staging_response")
@@ -399,14 +599,15 @@
         return agent
 
     def save(self, file, include_state=True):
         cfg = self.config(include_state=include_state)
         if hasattr(file, "write"):
             json.dump(cfg, file)
         elif isinstance(file, str):
+            os.makedirs(os.path.dirname(file), exist_ok=True)
             with open(file, "w") as f:
                 json.dump(cfg, f)
         else:
             raise TypeError(f"Expected str or file like object. Received {type(f)}.")
 
     @classmethod
     def load(cls, file):
@@ -417,7 +618,102 @@
                 cfg = json.load(f)
         else:
             raise TypeError(f"Expected str or file like object. Received {type(f)}.")
         return cls.from_config(cfg)
 
     def cli(self, continuous=False):
         cli(self, continuous=continuous)
+
+    def __enter__(self):
+        """Sets this agent as the active agent globally. This allows any tools to add data to this agent's memory
+        via a ``self.agent.memory.add`` call. In effect, the agent "watches" execution of tools in its with block.
+
+        Example:
+
+            >>> import loopgpt
+            >>> from loopgpt.tools import GoogleSearch
+            >>> agent = loopgpt.empty_agent()
+            >>> search = GoogleSearch()
+            >>> with agent:
+            ...     # the following line will add the search results to the agent's memory
+            ...     results, links = search("How to make a cake?")
+            ...
+            >>> print(agent.chat("Cake websites"))
+            Sure! Here are eight websites that offer cake recipes and inspiration:
+            1. Better Homes & Gardens - How to Make a Cake from Scratch That Looks Like It's From a Bakery: [Link](https://www.bhg.com/recipes/how-to/bake/how-to-make-a-cake/)
+            2. Food Network - Basic Vanilla Cake Recipe: [Link](https://www.foodnetwork.com/recipes/food-network-kitchen/basic-vanilla-cake-recipe-2043654)
+            3. ABCya! - Make a Cake: [Link](https://www.abcya.com/games/make-a-cake)
+            4. Allrecipes - Simple White Cake Recipe: [Link](https://www.allrecipes.com/recipe/17481/simple-white-cake/)
+            5. The Kitchn - How To Make a Cake from Scratch: [Link](https://www.thekitchn.com/how-to-make-a-cake-from-scratch-224370)
+            6. House & Garden - Vanilla Cake Recipe: [Link](https://www.houseandgarden.co.uk/recipe/simple-vanilla-cake-recipe)
+            7. RecipeTin Eats - My very best Vanilla Cake - stays moist 4 days!: [Link](https://www.recipetineats.com/my-very-best-vanilla-cake/)
+            8. Times of India - How to Make Cake at Home: Homemade Cake Recipe: [Link](https://recipes.timesofindia.com/us/recipes/homemade-cake/rs54404412.cms)
+        """
+        global ACTIVE_AGENT
+        ACTIVE_AGENT = self
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        """Resets the active agent to ``None``."""
+        global ACTIVE_AGENT
+        ACTIVE_AGENT = None
+
+    @contextmanager
+    def query(self, query):
+        """Set a query for the agent's memory. This gives more control over what the agent remembers while generating responses.
+
+        :param query: A query to filter the agent's memory by.
+        :type query: str
+        """
+        try:
+            self.memory_query = query
+            yield
+        finally:
+            self.memory_query = None
+
+    @contextmanager
+    def complete(self, history):
+        """Add additional history to the agent. This is useful for creating custom scenarios for the agent to respond to.
+
+        :param history: A list of dictionaries with a key ``"system"``,  ``"assistant"`` or ``"user"`` and a value of the text to add to the agent's history.
+        :type history: list
+        """
+        try:
+            self.additional_history = history
+            yield
+        finally:
+            self.additional_history = None
+
+
+def empty_agent(**agent_kwargs):
+    """Create an empty agent. Always use this function to create a new agent for use in conjunction with AI functions.
+    Creating agents with the :class:`Agent` class directly is reserved for CLI applications.
+
+    All parameters accepted by :class:`Agent` are accepted by this function.
+    """
+    agent = Agent(**agent_kwargs)
+    agent.prompts = []
+    agent.state = AgentStates.IDLE
+    agent.tools = agent.tools if agent_kwargs.get("tools") else {}
+    agent.goals = []
+    agent.constraints = []
+    agent.plan = []
+    agent.progress = []
+    agent.temperature = 0
+    agent._default_response_callback = lambda x: x
+    return agent
+
+
+def task_complete():
+    """Mark the current task as complete.
+
+    Returns:
+        None
+    """
+
+
+def do_nothing():
+    """No-op command.
+
+    Returns:
+        None
+    """
```

### Comparing `loopgpt-0.0.9/loopgpt/constants.py` & `loopgpt-0.1.0/loopgpt/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 """
 Credits: Auto-GPT (https://github.com/Significant-Gravitas/Auto-GPT)
 """
 
 
 DEFAULT_RESPONSE_FORMAT_ = {
     "thoughts": {
-        "text": "thought",
-        "reasoning": "reasoning",
+        "text": "What do you want to say to the user?",
+        "reasoning": "Why do you want to say this?",
+        "progress": "- A detailed list\n - of everything you have done so far",
         "plan": "- short bulleted\n- list that conveys\n- long-term plan",
-        "criticism": "constructive self-criticism",
         "speak": "thoughts summary to say to user",
     },
     "command": {"name": "next command in your plan", "args": {"arg name": "value"}},
 }
 
+
 DEFAULT_RESPONSE_FORMAT = f"You should only respond in JSON format as described below \nResponse Format: \n{json.dumps(DEFAULT_RESPONSE_FORMAT_, indent=4)}\nEnsure the response can be parsed by Python json.loads"
 
 
 NEXT_PROMPT_SMALL = "Next"
 
 
 EXPERIMENTAL_NEXT_PROMPT = (
@@ -43,46 +44,63 @@
     + "        points -= 1\n"
     + "    if (is_subset(current_plan, original_plan)):\n"
     + "        points += 100\n"
     + "    fill_response(json_format)\n"
     + "    return json_format\n"
 )
 
+
 NEXT_PROMPT = (
     "INSTRUCTIONS:\n"
-    + "1 - Use the command repsonses mentioned in previous system messages to plan your next command to work towards your goals.\n"
-    + "2 - exclusively use available commmands to work towards the goals.\n"
-    + "3 - Commands are expensive. Aim to complete tasks in the least number of steps.\n"
-    + "4 - A command is considered executed only if it is confirmed by a system message.\n"
-    + "5 - A command is not considered executed just becauses it was in your plan.\n"
-    + "6 - Rmember to use the output of previous command. If it contains useful information, save it to a file.\n"
-    + "7 - Do not use commands to retireve or analyze information you already have. Use your long term memory instead.\n"
-    + '8 - Execute the "do_nothing" command ONLY if there is no other command to execute.\n'
-    + '9 - Once all the planned commands are executed and ALL the goals are achieved, execute the "task_complete" command.\n'
-    + "10 - Explicitly associate a command with each step in your plan.\n"
-    + "11 - ONLY RESPOND IN THE FOLLOWING FORMAT: (MAKE SURE THAT IT CAN BE DECODED WITH PYTHON JSON.LOADS())\n"
+    + "1 - Check the progress of your goals.\n"
+    + '2 - If you have achieved all your goals, execute the "task_complete" command IMMEDIATELY. Otherwise,\n'
+    + "3 - Use the command responses in previous system messages to plan your next command to work towards your goals\n"
+    + "4 - Only use available commmands.\n"
+    + "5 - Commands are expensive. Aim to complete tasks in the least number of steps.\n"
+    + "6 - A command is considered executed only if it is confirmed by a system message.\n"
+    + "7 - A command is not considered executed just becauses it was in your plan.\n"
+    + "8 - Remember to use the output of previous command. If it contains useful information, save it to a file.\n"
+    + "9 - Do not use commands to retrieve or analyze information you already have. Use your long term memory instead.\n"
+    + '10 - Execute the "do_nothing" command ONLY if there is no other command to execute.\n'
+    + "11 - Make sure to execute commands only with supported arguments.\n"
+    + "12 - ONLY RESPOND IN THE FOLLOWING FORMAT: (MAKE SURE THAT IT CAN BE DECODED WITH PYTHON JSON.LOADS())\n"
     + json.dumps(DEFAULT_RESPONSE_FORMAT_, indent=4)
     + "\n"
 )
 
 
 INIT_PROMPT = (
     "Do the following:\n"
     + "1 - Execute the next best command to achieve the goals.\n"
     + '2 - Execute the "do_nothing" command if there is no other command to execute.\n'
     + "3 - ONLY RESPOND IN THE FOLLOWING FORMAT: (MAKE SURE THAT IT CAN BE DECODED WITH PYTHON JSON.LOADS())\n"
     + json.dumps(DEFAULT_RESPONSE_FORMAT_, indent=4)
     + "\n"
 )
 
+DEFAULT_PROMPT_TEMPLATE = """
+    <HEADER>
+    <HISTORY>
+    <MEMORY: 10>
+    <USER_INPUT>
+    """
+
 
 DEFAULT_AGENT_NAME = "LoopGPT"
 DEFAULT_AGENT_DESCRIPTION = "A personal assistant that responds exclusively in JSON"
 DEFAULT_GOALS = [
     "Respond exclusively in JSON format",
     "Give concise and useful responses",
     "Always execute plans to completion",
 ]
 
+
+class AgentStates:
+    START = "START"
+    IDLE = "IDLE"
+    TOOL_STAGED = "TOOL_STAGED"
+    STOP = "STOP"
+
+
 # SPINNER
 SPINNER_ENABLED = True
 SPINNER_START_DELAY = 2
```

### Comparing `loopgpt-0.0.9/loopgpt/embeddings/__init__.py` & `loopgpt-0.1.0/loopgpt/embeddings/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from loopgpt.embeddings.provider import BaseEmbeddingProvider
+from loopgpt.embeddings.base import BaseEmbeddingProvider
 from loopgpt.embeddings.openai_ import OpenAIEmbeddingProvider
+from loopgpt.embeddings.azure_openai import AzureOpenAIEmbeddingProvider
+from loopgpt.embeddings.hf import HuggingFaceEmbeddingProvider
 
 user_providers = {}
 
 
 def register_embedding_provider_type(provider):
     if isinstance(provider, BaseEmbeddingProvider):
         provider = provider.__class__
```

### Comparing `loopgpt-0.0.9/loopgpt/loops/cli.py` & `loopgpt-0.1.0/loopgpt/loops/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     parser.add_argument(
         "action",
         choices=["run"],
         help="Action to perform. If no file is specified, a new agent is created.",
     )
     parser.add_argument("filename", nargs="?", help="Agent state JSON.", default=None)
     parser.add_argument(
+        "--model", help="Model to use, uses gpt-3.5-turbo by default.", default=None
+    )
+    parser.add_argument(
         "--readonly",
         help="Read only mode. Does not write agent state to disk.",
         action="store_true",
     )
     parser.add_argument(
         "--reset",
         help="Reset agent state before use. Name, goals and description are not affected.",
@@ -42,19 +45,22 @@
             agent_state = json.load(f)
 
         agent = Agent.from_config(agent_state)
 
         if args.reset:
             agent.clear_state()
 
-        agent.cli()
-
-        if not args.readonly:
-            with open(filename, "w") as f:
-                json.dump(agent.config(), f)
+        try:
+            agent.cli()
+        finally:
+            if not args.readonly:
+                with open(filename, "w") as f:
+                    json.dump(agent.config(), f)
     else:
-        agent = Agent()
-        agent.cli(continuous=args.continuous)
+        agent = Agent(model=args.model)
 
-        if args.save:
-            with open(args.save, "w") as f:
-                json.dump(agent.config(), f)
+        try:
+            agent.cli(continuous=args.continuous)
+        finally:
+            if args.save:
+                with open(args.save, "w") as f:
+                    json.dump(agent.config(), f)
```

### Comparing `loopgpt-0.0.9/loopgpt/loops/repl.py` & `loopgpt-0.1.0/loopgpt/loops/repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 from colorama import Fore, Style
 
 import os
 
 LOOP_GPT = Fore.GREEN + "LoopGPT"
 REASONING = Fore.LIGHTBLUE_EX + "REASONING"
 PLAN = Fore.LIGHTYELLOW_EX + "PLAN"
-CRITICISM = Fore.LIGHTRED_EX + "CRITICISM"
+PROGRESS = Fore.LIGHTRED_EX + "PROGRESS"
 SPEAK = Fore.LIGHTGREEN_EX + "SPEAK"
 COMMAND = Fore.LIGHTMAGENTA_EX + "NEXT_COMMAND"
 SYSTEM = Fore.LIGHTYELLOW_EX + "SYSTEM"
 INPUT_PROMPT = Fore.LIGHTYELLOW_EX + "Enter message: " + Style.RESET_ALL
 
 profiles = {
     "loopgpt": LOOP_GPT,
     "reasoning": REASONING,
     "plan": PLAN,
-    "criticism": CRITICISM,
+    "progress": PROGRESS,
     "speak": SPEAK,
     "command": COMMAND,
     "system": SYSTEM,
 }
 
 
 def listed_prompt(speaker, message, item_kind):
@@ -84,14 +84,16 @@
 
 
 def check_agent_config(agent):
     if agent.name is None or agent.name == DEFAULT_AGENT_NAME:
         name = prompt("loopgpt", "Enter the name of your AI agent: ")
         if name.lower().strip() == "exit":
             return -1
+        if name.strip() == "":
+            name = "LoopGPT"
         agent.name = name
 
     if agent.description is None or agent.description == DEFAULT_AGENT_DESCRIPTION:
         description = prompt("loopgpt", "Enter a description for your AI agent: ")
         if description.lower().strip() == "exit":
             return -1
         agent.description = description
@@ -126,61 +128,57 @@
                     msgs["reasoning"] = thoughts["reasoning"]
                 if "plan" in thoughts:
                     msgs["plan"] = (
                         thoughts["plan"].split("\n")
                         if isinstance(thoughts["plan"], str)
                         else thoughts["plan"]
                     )
-                if "criticism" in thoughts:
-                    msgs["criticism"] = thoughts["criticism"]
+                if "progress" in thoughts:
+                    msgs["progress"] = thoughts["progress"]
                 if "speak" in thoughts:
                     msgs["speak"] = "(voice) " + thoughts["speak"]
                 for kind, msg in msgs.items():
                     print_line(kind, msg, end="\n\n")
             if "command" in resp:
                 command = resp["command"]
-                if (
-                    isinstance(command, dict)
-                    and "name" in command
-                    and "args" in command
-                ):
+                if isinstance(command, dict) and "name" in command:
                     if command["name"]:
                         print_line(
                             "command",
-                            f"{command['name']}, Args: {command['args']}",
+                            f"{command['name']}, Args: {command.get('args') or {}}",
                             end="\n\n",
                         )
                     while True:
                         if continuous or n > 1:
                             yn = "y"
                             n -= 1
                         else:
-                            inp = input(f"Execute? (Y/N/Y:n to execute n steps continuously): ")
+                            inp = input(
+                                f"Execute? (Y/N/Y:n to execute n steps continuously): "
+                            )
                             yn, n = inp.split(":") if ":" in inp else (inp, 1)
                             n = int(n)
                             yn = yn.lower().strip()
                             if yn == "exit":
                                 return
                         if yn in ("y", "n"):
                             break
                     if yn == "y":
                         cmd = agent.staging_tool.get("name", agent.staging_tool)
                         if cmd == "task_complete":
                             return
                         print_line("system", f"Executing command: {cmd}")
-                        resp = agent.chat(agent.next_prompt, True)
+                        resp = agent.chat(run_tool=True)
                         print_line("system", f"{cmd} output: {agent.tool_response}")
                     elif yn == "n":
                         feedback = input(
                             "Enter feedback (Why not execute the command?): "
                         )
                         if feedback.lower().strip() == "exit":
                             return
-                        next_prompt = agent.next_prompt
-                        feedback = next_prompt + "\n\n" + feedback
                         resp = agent.chat(feedback, False)
                     write_divider()
                     continue
         write_divider()
         inp = input(INPUT_PROMPT)
         if inp.lower().strip() == "exit":
             return
```

### Comparing `loopgpt-0.0.9/loopgpt/loops/ui.py` & `loopgpt-0.1.0/loopgpt/loops/ui.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.9/loopgpt/memory/__init__.py` & `loopgpt-0.1.0/loopgpt/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.9/loopgpt/memory/local_memory.py` & `loopgpt-0.1.0/loopgpt/memory/local_memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,21 @@
 class LocalMemory(BaseMemory):
     def __init__(self, embedding_provider: callable):
         super(BaseMemory, self).__init__()
         self.docs: List[str] = []
         self.embs: Optional[np.ndarray] = None
         self.embedding_provider = embedding_provider
 
-    def add(self, doc: str):
-        emb = self.embedding_provider(doc)
+    def __len__(self):
+        return len(self.docs)
+
+    def add(self, doc: str, key: Optional[str] = None):
+        if not key:
+            key = doc
+        emb = self.embedding_provider(key)
         if self.embs is None:
             self.embs = np.expand_dims(emb, 0)
         else:
             self.embs = np.concatenate([self.embs, [emb]], 0)
         self.docs.append(doc)
 
     def get(self, query: str, k: int):
```

### Comparing `loopgpt-0.0.9/loopgpt/models/openai_.py` & `loopgpt-0.1.0/loopgpt/models/openai_.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,79 @@
 from typing import *
 from loopgpt.logger import logger
+from loopgpt.models.base import BaseModel
+from loopgpt.utils.openai_key import get_openai_key
+
 import tiktoken
 import time
-import os
 
+from openai.error import RateLimitError
+import openai
 
-def _getkey(key: Optional[str] = None):
-    key = key or os.getenv("OPENAI_API_KEY")
-    if key is None:
-        raise ValueError(
-            "OpenAI API Key not found. Please set the `OPENAI_API_KEY` environment variable. "
-            "See https://github.com/farizrahman4u/loopgpt#-requirements for more details"
-        )
 
+class OpenAIModel(BaseModel):
+    def __init__(self, model: str = "gpt-3.5-turbo", api_key: Optional[str] = None):
+        self.model = model
+        self.api_key = api_key
+
+    def chat(
+        self,
+        messages: List[Dict[str, str]],
+        max_tokens: Optional[int] = None,
+        temperature: float = 0.8,
+    ) -> str:
+        api_key = get_openai_key(self.api_key)
+        num_retries = 3
+        for i in range(num_retries):
+            try:
+                resp = openai.ChatCompletion.create(
+                    model=self.model,
+                    messages=messages,
+                    api_key=api_key,
+                    max_tokens=max_tokens,
+                    temperature=temperature,
+                )["choices"][0]["message"]["content"]
+                return resp
+
+            except RateLimitError:
+                logger.warn("Rate limit exceeded. Retrying after 20 seconds.")
+                time.sleep(20)
+                if i == num_retries - 1:
+                    raise
+
+    def count_tokens(self, messages: List[Dict[str, str]]) -> int:
+        tokens_per_message, tokens_per_name = {
+            "gpt-3.5-turbo": (4, -1),
+            "gpt-4": (3, 1),
+            "gpt-4-32k": (3, 1),
+        }[self.model]
+        enc = tiktoken.encoding_for_model(self.model)
+        num_tokens = 0
+        for message in messages:
+            num_tokens += tokens_per_message
+            for key, value in message.items():
+                num_tokens += len(enc.encode(value))
+                if key == "name":
+                    num_tokens += tokens_per_name
+        num_tokens += 3
+        return num_tokens
+
+    def get_token_limit(self) -> int:
+        return {
+            "gpt-3.5-turbo": 4000,
+            "gpt-4": 8000,
+            "gpt-4-32k": 32000,
+        }[self.model]
+
+    def config(self):
+        cfg = super().config()
+        cfg.update(
+            {
+                "model": self.model,
+                "api_key": self.api_key,
+            }
+        )
+        return cfg
 
-def chat(
-    messages: List[Dict[str, str]],
-    model: str = "gpt-3.5-turbo",
-    api_key: Optional[str] = None,
-    max_tokens: Optional[int] = None,
-    temperature: float = 0.8,
-) -> str:
-    import openai
-    from openai.error import RateLimitError
-
-    api_key = _getkey(api_key)
-    num_retries = 3
-    for _ in range(num_retries):
-        try:
-            return openai.ChatCompletion.create(
-                model=model,
-                messages=messages,
-                api_key=api_key,
-                max_tokens=max_tokens,
-                temperature=temperature,
-            )["choices"][0]["message"]["content"]
-        except RateLimitError:
-            logger.warn("Rate limit exceeded. Retrying after 20 seconds.")
-            time.sleep(20)
-            continue
-
-
-def count_tokens(messages: List[Dict[str, str]], model: str = "gpt-3.5-turbo") -> int:
-    tokens_per_message, tokens_per_name = {"gpt-3.5-turbo": (4, -1), "gpt-4": (3, 1)}[
-        model
-    ]
-    enc = tiktoken.encoding_for_model(model)
-    num_tokens = 0
-    for message in messages:
-        num_tokens += tokens_per_message
-        for key, value in message.items():
-            num_tokens += len(enc.encode(value))
-            if key == "name":
-                num_tokens += tokens_per_name
-    num_tokens += 3
-    return num_tokens
-
-
-def get_token_limit(model: str = "gpt-3.5-turbo") -> int:
-    return {
-        "gpt-3.5-turbo": 4000,
-        "gpt-4": 8000,
-    }[model]
+    @classmethod
+    def from_config(cls, config):
+        return cls(config["model"], config.get("api_key"))
```

### Comparing `loopgpt-0.0.9/loopgpt/tools/__init__.py` & `loopgpt-0.1.0/loopgpt/tools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from loopgpt.tools.agent_manager import (
     CreateAgent,
     MessageAgent,
     DeleteAgent,
     ListAgents,
 )
+from loopgpt.tools.user_manager import AskUser
 from loopgpt.tools.base_tool import BaseTool
 from loopgpt.tools.browser import Browser
-from loopgpt.tools.code import ExecutePythonFile, EvaluateCode, ImproveCode, WriteTests
+from loopgpt.tools.code import ExecutePythonFile, ReviewCode, ImproveCode, WriteTests
+from loopgpt.tools.math import EvaluateMath
 from loopgpt.tools.google_search import GoogleSearch
 from loopgpt.tools.filesystem import (
     ReadFromFile,
     WriteToFile,
     AppendToFile,
     DeleteFile,
     CheckIfFileExists,
     ListFiles,
+    GetCWD,
+    MakeDirectory,
     FileSystemTools,
 )
 from loopgpt.tools.shell import Shell
 from loopgpt.tools.memory_manager import AddToMemory
 
 
 user_tools = {}
@@ -45,12 +49,15 @@
         GoogleSearch,
         Browser,
         CreateAgent,
         MessageAgent,
         ListAgents,
         DeleteAgent,
         *FileSystemTools,
-        EvaluateCode,
+        ReviewCode,
         ImproveCode,
         WriteTests,
         ExecutePythonFile,
+        EvaluateMath,
+        AskUser,
+        Shell,
     ]
```

### Comparing `loopgpt-0.0.9/loopgpt/tools/agent_manager.py` & `loopgpt-0.1.0/loopgpt/tools/agent_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,87 @@
 from loopgpt.tools.base_tool import BaseTool
 from typing import *
 from uuid import uuid4
 
 
-class _AgentMangerTool(BaseTool):
+class _AgentManagerTool(BaseTool):
     pass
 
 
-class CreateAgent(_AgentMangerTool):
-    @property
-    def args(self):
-        return {
-            "name": "Agent name",
-            "task": "Specific task for agent",
-            "prompt": "The prompt",
-        }
-
-    @property
-    def resp(self):
-        return {
-            "id": "Unique ID of new agent.",
-            "resp": "Response from new agent.",
-        }
+class CreateAgent(_AgentManagerTool):
+    """Create a new agent.
 
-    def run(self, name="", task="", prompt=""):
+    Args:
+        name (str): Agent name.
+        task (str): Specific task for agent.
+        prompt (str): The prompt.
+
+    Returns:
+        dict: A dict containing the id and response from the agent.
+    """
+
+    def run(self, name: str = "", task: str = "", prompt: str = ""):
         from loopgpt.agent import Agent
 
+        model = self.agent.model
+        emb = self.agent.embedding_provider
         agent = Agent(
-            name=name, description=f"An agent for performing this specific task: {task}"
+            name=name,
+            description=f"An agent for performing this specific task: {task}",
+            model=model,
+            embedding_provider=emb,
         )
         agent.tools.clear()
         id = uuid4().hex[:8]
-        self.agent.sub_agents[id] = (Agent(), task)
+        self.agent.sub_agents[id] = (agent, task)
         resp = agent.chat(prompt)
         return {"uuid": id, "resp": resp}
 
 
-class MessageAgent(_AgentMangerTool):
-    @property
-    def args(self):
-        return {
-            "id": "Agent id.",
-            "message": "The message",
-        }
-
-    @property
-    def resp(self):
-        return {"resp": "Response from the agent."}
+class MessageAgent(_AgentManagerTool):
+    """Send a message to an agent.
+
+    Args:
+        id (str): Agent id.
+        message (str): The message to send to the agent.
+
+    Returns:
+        str: The response from the agent.
+    """
 
-    def run(self, id, message):
+    def run(self, id: str, message: str):
         if id not in self.agent.sub_agents:
             return {"resp": "AGENT NOT FOUND!"}
         resp = self.agent.sub_agents[id][0].chat(message)
-        return {"resp": resp}
+        return resp
 
 
-class DeleteAgent(_AgentMangerTool):
-    @property
-    def args(self):
-        return {"id": "Agent id"}
+class DeleteAgent(_AgentManagerTool):
+    """Delete an agent.
 
-    @property
-    def resp(self):
-        return {"success": "true or false"}
+    Args:
+        id (str): Agent id.
 
-    def run(self, id):
+    Returns:
+        bool: True if the agent was deleted, False otherwise.
+    """
+
+    def run(self, id: str):
         try:
             self.agent.sub_agents.pop(id)
-            return {"resp": "Deleted."}
+            return True
         except KeyError:
-            return {f"resp": "Specified agent (id={id} not found.)"}
+            return f"Error: Specified agent {id} not found."
+
 
+class ListAgents(_AgentManagerTool):
+    """List all available agents.
 
-class ListAgents(_AgentMangerTool):
-    @property
-    def args(self):
-        return {}
-
-    @property
-    def resp(self):
-        return {
-            "agents": "List of available agents, where each item is of the form [agent id, task]"
-        }
+    Returns:
+        List: List of available agents, where each item is of the form [agent_id, task]
+    """
 
     def run(self):
         return [[k, v[1]] for k, v in self.agent.sub_agents.items()]
 
 
 AgentManagerTools = [CreateAgent, MessageAgent, DeleteAgent, ListAgents]
```

### Comparing `loopgpt-0.0.9/loopgpt/tools/base_tool.py` & `loopgpt-0.1.0/loopgpt/tools/base_tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 from typing import *
-import json
+import loopgpt.agent
+import inspect
 import re
 
 
 def camel_case_split(str):
     return re.findall(r"[A-Z](?:[a-z]+|[A-Z]*(?=[A-Z]|$))", str)
 
 
 class BaseTool:
-    @property
-    def id(self) -> str:
-        return "_".join(camel_case_split(self.__class__.__name__)).lower()
+    def __init__(self, *args, **kwargs):
+        self._agent = None
 
     @property
-    def desc(self) -> str:
-        return " ".join(camel_case_split(self.__class__.__name__))
+    def agent(self):
+        return loopgpt.agent.ACTIVE_AGENT or self._agent
 
-    @property
-    def args(self) -> Dict[str, str]:
-        raise NotImplementedError()
-
-    def run(**kwrags) -> str:
-        raise NotImplementedError()
+    @agent.setter
+    def agent(self, agent):
+        self._agent = agent
 
     @property
-    def resp(self) -> Dict[str, str]:
+    def id(self) -> str:
+        return "_".join(camel_case_split(self.__class__.__name__)).lower()
+
+    def run(**kwargs) -> str:
         raise NotImplementedError()
 
     def prompt(self):
-        return json.dumps(
-            {
-                "name": self.id,
-                "description": self.desc,
-                "args": self.args,
-                "response_format": self.resp,
-            }
-        )
+        sig = inspect.signature(self.run)
+        return f'def {self.id}{sig}:\n\t"""{self.__doc__}\n\t"""'.expandtabs(4)
 
     def config(self):
         return {
             "class": self.__class__.__name__,
             "type": "tool",
         }
 
+    def __call__(self, *args, **kwargs):
+        return self.run(*args, **kwargs)
+
     @classmethod
     def from_config(cls, config):
         return cls()
```

### Comparing `loopgpt-0.0.9/loopgpt/tools/browser.py` & `loopgpt-0.1.0/loopgpt/tools/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,48 +13,66 @@
 from loopgpt.summarizer import Summarizer
 from loopgpt.logger import logger
 import logging
 import atexit
 
 
 class Browser(BaseTool):
+    """This opens a browser. It opens the url and finds the answer for the query.
+    Provide an empty query if you want to summarize the page.
+
+    Args:
+        url (str): URL to open.
+        query (str): Query to search for.
+
+    Returns:
+        Dict: Relevant summary and a list of links extracted from the URL.
+
+    """
+
     def __init__(self, browser_type="chrome"):
         super(Browser, self).__init__()
         if browser_type not in ("chrome", "firefox"):
             browser_type = "chrome"
         self._set_browser_options(browser_type)
         self.driver = None
         self.summarizer = Summarizer()
         self.cache = {}
+        self.browsed = {}
         atexit.register(self.close)
-    
+
     def _set_browser_options(self, browser_type):
         self.browser_type = browser_type
         if self.browser_type == "chrome":
             from selenium.webdriver.chrome.options import Options
         elif self.browser_type == "firefox":
             from selenium.webdriver.firefox.options import Options
         options = Options()
         options.add_argument(
             "user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.5615.49 Safari/537.36"
         )
-        options.add_experimental_option("excludeSwitches", ["enable-logging"])
-        options.headless = True
+        if self.browser_type == "chrome":
+            options.add_experimental_option("excludeSwitches", ["enable-logging"])
+        elif self.browser_type == "firefox":
+            options.add_argument("TRACE")
+        options.add_argument("--headless")
         self.options = options
-    
+
     def _init_chrome_driver(self):
         try:
             self.driver = webdriver.Chrome(
                 executable_path=ChromeDriverManager().install(), options=self.options
             )
         except:
-            logger.log(logging.INFO, "Failed to initialize Chrome driver. Trying Firefox...")
+            logger.log(
+                logging.INFO, "Failed to initialize Chrome driver. Trying Firefox..."
+            )
             self._set_browser_options("firefox")
             self._init_driver()
-    
+
     def _init_firefox_driver(self):
         self.driver = webdriver.Firefox(options=self.options)
 
     def _init_driver(self):
         self.close()
         if self.browser_type == "chrome":
             self._init_chrome_driver()
@@ -91,56 +109,47 @@
         return [(link.text, link["href"]) for link in soup.find_all("a", href=True)]
 
     def _extract_text_from_soup(self, soup):
         lines = (line.strip() for line in soup.get_text().splitlines())
         chunks = (phrase.strip() for line in lines for phrase in line.split("  "))
         return "\n".join(chunk for chunk in chunks if chunk)
 
-    @property
-    def desc(self):
-        return "Scrape answers for a question in a given web page"
-
-    @property
-    def args(self):
-        return {"url": "URL of the website to scrape", "query": "The search query"}
-
-    @property
-    def resp(self):
-        return {
-            "text": "Summary of relevant text scraped from the website",
-            "links": "list of links from the website, where each item is in the form [link_text, link_url]",
-        }
-
     def close(self):
         try:
             self.driver.quit()
         except Exception:
             pass
 
-    def run(self, url: str, query: str):
+    def run(self, url: str, query: str = ""):
         if not isinstance(url, str):
             return "Scraping website failed. The URL must be a string."
+        if self.browsed.get(f"{url}_{query}"):
+            return self.browsed[f"{url}_{query}"]
         try:
             soup = BeautifulSoup(self._get(url), "html.parser")
             [script.extract() for script in soup(["script", "style"])]
             links = self._extract_links_from_soup(soup)[:5]
             text = self._extract_text_from_soup(soup)
-            self.summarizer.agent = getattr(self, "agent", None)
+            self.summarizer.agent = getattr(self, "agent")
             summary, chunks = self.summarizer.summarize(text, query)
-            if getattr(self, "agent", None):
+            if getattr(self, "agent"):
                 for chunk in chunks:
                     self.agent.memory.add(f"Snippet from {url}: {chunk}")
 
-            return {
-                "text": summary,
-                "links": links[:5],
-            }
+            result = (
+                summary
+                + "\n\n"
+                + "Links found on the page:\n"
+                + "\n".join([f"{link[1]}: {link[0]}" for link in links])
+            )
+            self.browsed[f"{url}_{query}"] = result
+            return result
         except Exception as e:
-            return f"An error occured while scraping the website: {e}. Make sure the URL is valid."
-    
+            return f"An error occurred while scraping the website: {e}. Make sure the URL is valid."
+
     def config(self):
         config = super().config()
         config["browser_type"] = self.browser_type
         return config
 
     @classmethod
     def from_config(cls, config):
```

### Comparing `loopgpt-0.0.9/loopgpt/tools/code.py` & `loopgpt-0.1.0/loopgpt/tools/code.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,107 @@
+from typing import List
 from loopgpt.tools.base_tool import BaseTool
-from loopgpt.models.openai_ import chat
+from loopgpt.models import BaseModel, OpenAIModel
 import subprocess
 import sys
 import os
 
 
-def ai_function(func, desc, args, model="gpt-3.5-turbo"):
+def ai_function(func, desc, args, model: BaseModel):
     """Credits: Auto-GPT (https://github.com/Significant-Gravitas/Auto-GPT)
     Also see: https://github.com/Torantulino/AI-Functions
     """
     msgs = [
         {
             "role": "system",
             "content": f"You are now the following python function: ```# {desc}\n{func}```\n\nOnly respond with your `return` value.",
         },
         {"role": "user", "content": ", ".join(map(str, args))},
     ]
-    return chat(messages=msgs, model=model, temperature=0.0)
+    return model.chat(messages=msgs, temperature=0.0)
 
 
 class _BaseCodeTool(BaseTool):
     @property
     def model(self):
-        if hasattr(self, "agent"):
+        if getattr(self, "agent"):
             return self.agent.model
-        return "gpt-3.5-turbo"
+        return OpenAIModel("gpt-3.5-turbo")
 
 
 class ExecutePythonFile(_BaseCodeTool):
-    @property
-    def args(self):
-        return {"file": "The Python file path as a string."}
+    """Execute a Python file and return the output.
 
-    @property
-    def resp(self):
-        return {
-            "output": "Value of stdout if the execution was successfull. Else error message."
-        }
+    Args:
+        file (str): Path to the Python file.
+
+    Returns:
+        str: Value of stdout if the execution was successful. Else error message.
+    """
 
-    def run(self, file):
+    def run(self, file: str):
         if not os.path.isfile(file):
-            return {"output": f"File {file} does not exist."}
+            return f"File {file} does not exist."
         if not file.lower().endswith(".py"):
-            return {"output": f"Only files with '.py' extension allowed."}
+            return f"Only files with '.py' extension are allowed."
         res = subprocess.run(
             f"{sys.executable} {file}",
             capture_output=True,
             encoding="utf-8",
             shell=True,
         )
         if res.returncode:
-            return {"output": f"Error: {res.stderr}"}
+            return f"Error: {res.stderr}"
         else:
-            return {"output": res.stdout}
+            return res.stdout
 
 
-class EvaluateCode(_BaseCodeTool):
-    @property
-    def description(self):
-        return "Returns a list of suggestions to improve a given piece of code."
+class ReviewCode(_BaseCodeTool):
+    """Review a piece of code and return a list of suggestions to improve it.
 
-    @property
-    def args(self):
-        return {
-            "code": "Code to evaluate",
-        }
+    Args:
+        code (str): Code to evaluate.
 
-    @property
-    def resp(self):
-        return {"suggestions": "List of suggestions to improve the code."}
+    Returns:
+        List[str]: List of suggestions to improve the code.
+    """
 
-    def run(self, code):
+    def run(self, code: str):
         func = "def analyze_code(code: str) -> List[str]:"
         desc = (
             "Analyzes the given code and returns a list of suggestions"
             " for improvements."
         )
-        return {"suggestions": ai_function(func, desc, [code], model=self.model)}
+        return ai_function(func, desc, [code], model=self.model)
 
 
 class ImproveCode(_BaseCodeTool):
-    @property
-    def description(self):
-        return "Improve a piece of code given a list of suggestions."
+    """Improve a piece of code given a list of suggestions.
 
-    @property
-    def args(self):
-        return {
-            "code": "The code to improve.",
-            "suggestions": "List of suggestions",
-        }
+    Args:
+        code (str): The code to improve.
+        suggestions (List[str]): List of suggestions
 
-    @property
-    def resp(self):
-        return {"improved_code": "Improved code."}
+    Returns:
+        str: Improved code.
+    """
 
-    def run(self, code, suggestions):
+    def run(self, code: str, suggestions: List[str]):
         func = "def generate_improved_code(suggestions: str, code: str) -> str:"
         desc = "Improves the provided code based on the suggestions provided, making no other changes."
-        return {
-            "improved_code": ai_function(
-                func, desc, [code, str(suggestions)], model=self.model
-            )
-        }
+        return ai_function(func, desc, [code, str(suggestions)], model=self.model)
 
 
 class WriteTests(_BaseCodeTool):
-    @property
-    def args(self):
-        return {
-            "code": "Code to write tests for.",
-        }
+    """Write tests for a piece of code.
 
-    @property
-    def resp(self):
-        return {"tests": "Tests."}
+    Args:
+        code (str): Code to write tests for.
+
+    Returns:
+        str: Tests.
+    """
 
-    def run(self, code):
+    def run(self, code: str):
         func = "def create_test_cases(code: str, focus: Optional[str] = None) -> str:"
         desc = "Generates test cases for the existing code, focusing on specific areas if required."
-        return {"tests": ai_function(func, desc, [code], model=self.model)}
+        return ai_function(func, desc, [code], model=self.model)
```

### Comparing `loopgpt-0.0.9/loopgpt/tools/google_search.py` & `loopgpt-0.1.0/loopgpt/tools/google_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,92 @@
 from loopgpt.tools.base_tool import BaseTool
+from itertools import islice
 
 import os
 
 
 class GoogleSearch(BaseTool):
+    """This tool searches google for the given query and returns the results.
+
+    Args:
+        query (str): The query to search for.
+
+    Returns:
+        str: Search results.
+    """
+
     def __init__(self):
         super(GoogleSearch, self).__init__()
         self.google_api_key = os.getenv("GOOGLE_API_KEY")
-        self.google_cx_id = os.getenv("CUSTOM_SEARCH_ENGINE_ID")
-
-    @property
-    def args(self):
-        return {"query": "The query to search for"}
-
-    @property
-    def resp(self):
-        return {
-            "results": "A list of results. Each result is a list of the form [title, link, description]"
-        }
+        self.google_cx_id = os.getenv("GOOGLE_CX_ID")
 
     def _duckduckgo_search(self, query, num_results=8):
-        from duckduckgo_search import ddg
+        from duckduckgo_search import DDGS
 
-        results = []
-        for result in ddg(query, max_results=num_results):
-            if getattr(self, "agent", None):
-                self.agent.memory.add(
-                    f"Search result for {query}: [{result['title']}]({result['href']})"
+        results_ = []
+        links_and_titles_ = []
+        links = []
+
+        with DDGS() as ddgs:
+            results = islice(ddgs.text(query), num_results)
+            for i, result in enumerate(results):
+                links_and_titles_.append(
+                    f"{i + 1}. {result['href']}: {result['title']}"
+                )
+                results_.append(
+                    f"{i + 1}. {result['href']}: {result['title']}\n{result['body']}\n"
                 )
-            results.append([result["title"], result["href"], result["body"]])
-        return {"results": results}
+                links.append(result["href"])
+
+        links_and_titles = "\n".join(links_and_titles_)
+        results = "\n".join(results_)
+
+        return results, links
 
     def _google_search(self, query, num_results=8):
         from googleapiclient.discovery import build
 
         service = build("customsearch", "v1", developerKey=self.google_api_key)
         results = (
             service.cse()
             .list(q=query, cx=self.google_cx_id, num=num_results)
             .execute()
             .get("items", [])
         )
-        for result in results:
-            if getattr(self, "agent", None):
-                self.agent.memory.add(
-                    f"Search result for {query}: [{result['title']}]({result['link']})"
+
+        results_ = []
+        links_and_titles_ = []
+        links = []
+
+        for i, result in enumerate(results):
+            try:
+                links_and_titles_.append(
+                    f"{i + 1}. {result['link']}: {result['title']}"
+                )
+                results_.append(
+                    f"{i + 1}. {result['link']}: {result['title']}\n{result['snippet'].strip('...')}\n"
                 )
-        results = [
-            [result["title"], result["link"], result["snippet"]] for result in results
-        ]
+                links.append(result["link"])
+            except:
+                continue
 
-        return {"results": results}
+        links_and_titles = "\n".join(links_and_titles_)
+        results = "\n".join(results_)
 
-    def run(self, query, num_results=8):
+        return results, links
+
+    def _add_to_memory(self, results):
+        if getattr(self, "agent"):
+            self.agent.memory.add(results)
+
+    def run(self, query: str):
         try:
-            return self._google_search(query, num_results)
+            results, links = self._google_search(query, 8)
         except:
-            return self._duckduckgo_search(query, num_results)
+            results, links = self._duckduckgo_search(query, 8)
+
+        assert len(results) > 0, "No results found."
+        if len(results) > 0:
+            self._add_to_memory(results)
+        else:
+            results = "No results found."
+        return results, links
```

### Comparing `loopgpt-0.0.9/loopgpt/utils/spinner.py` & `loopgpt-0.1.0/loopgpt/utils/spinner.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,14 @@
             with self._stderr_lock:
                 self._hide_event.clear()
                 self._clear_line()
                 self._hide_cursor()
 
     def stop(self):
         self._stop_event.set()
-        self.join()
         self._clear_line()
         self._show_cursor()
 
     def _clear_line(self):
         if self.file.isatty():
             # ANSI Control Sequence EL does not work in Jupyter
             self.file.write("\r\033[K")
@@ -133,7 +132,21 @@
     def inner(*args, **kwargs):
         spinner = Spinner()
 
         with run_spinner(spinner):
             return func(*args, **kwargs)
 
     return inner
+
+
+def hide_spinner(func):
+    @wraps(func)
+    def inner(*args, **kwargs):
+        if ACTIVE_SPINNER:
+            ACTIVE_SPINNER.hide()
+        try:
+            return func(*args, **kwargs)
+        finally:
+            if ACTIVE_SPINNER:
+                ACTIVE_SPINNER.show()
+
+    return inner
```

