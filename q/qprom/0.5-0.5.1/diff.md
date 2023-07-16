# Comparing `tmp/qprom-0.5.tar.gz` & `tmp/qprom-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qprom-0.5.tar", last modified: Sun Jul 16 01:05:25 2023, max compression
+gzip compressed data, was "qprom-0.5.1.tar", last modified: Sun Jul 16 19:34:20 2023, max compression
```

## Comparing `qprom-0.5.tar` & `qprom-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.029849 qprom-0.5/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.5/LICENSE
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     4160 2023-07-16 01:05:25.029742 qprom-0.5/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     3421 2023-07-16 01:02:26.000000 qprom-0.5/README.md
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028041 qprom-0.5/arguments/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1501 2023-07-16 01:02:26.000000 qprom-0.5/arguments/__init__.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028253 qprom-0.5/config/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5/config/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1117 2023-07-15 23:11:02.000000 qprom-0.5/config/credentials.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028581 qprom-0.5/gpt/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5/gpt/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1219 2023-07-15 23:11:02.000000 qprom-0.5/gpt/request.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.5/gpt/util.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028796 qprom-0.5/qprom/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.5/qprom/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      736 2023-07-15 23:41:44.000000 qprom-0.5/qprom/main.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.029571 qprom-0.5/qprom.egg-info/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     4160 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      368 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/SOURCES.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/dependency_links.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/entry_points.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.5/qprom.egg-info/not-zip-safe
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/requires.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/top_level.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-16 01:05:25.029885 qprom-0.5/setup.cfg
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1280 2023-07-16 01:03:49.000000 qprom-0.5/setup.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.586210 qprom-0.5.1/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.5.1/LICENSE
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     4686 2023-07-16 19:34:20.586094 qprom-0.5.1/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     3945 2023-07-16 19:31:31.000000 qprom-0.5.1/README.md
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.583819 qprom-0.5.1/arguments/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1249 2023-07-16 19:12:09.000000 qprom-0.5.1/arguments/__init__.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.584017 qprom-0.5.1/config/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5.1/config/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1116 2023-07-16 19:13:45.000000 qprom-0.5.1/config/credentials.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.584440 qprom-0.5.1/gpt/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5.1/gpt/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1219 2023-07-15 23:11:02.000000 qprom-0.5.1/gpt/request.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.5.1/gpt/util.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.584859 qprom-0.5.1/qprom/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.5.1/qprom/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      759 2023-07-16 19:13:45.000000 qprom-0.5.1/qprom/main.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      250 2023-07-16 19:13:45.000000 qprom-0.5.1/qprom/utils.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.585907 qprom-0.5.1/qprom.egg-info/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     4686 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      383 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/SOURCES.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/dependency_links.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/entry_points.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.5.1/qprom.egg-info/not-zip-safe
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/requires.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/top_level.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-16 19:34:20.586255 qprom-0.5.1/setup.cfg
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1282 2023-07-16 19:33:55.000000 qprom-0.5.1/setup.py
```

### Comparing `qprom-0.5/LICENSE` & `qprom-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qprom-0.5/PKG-INFO` & `qprom-0.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-Metadata-Version: 2.1
-Name: qprom
-Version: 0.5
-Summary: A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.
-Home-page: https://github.com/MartinWie/qprom
-Download-URL: https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz
-Author: MartinWiechmann
-Author-email: donotsuspend@googlegroups.com
-License: MIT
-Keywords: GPT-4 CLI GPT-3 OpenAI
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # qprom a.k.a Quick Prompt
 
 [![OS](https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [![RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)](https://github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 
 ![qprom](https://github.com/MartinWie/qprom/blob/main/qprom_logo.png)
 
 A Python-based CLI tool to quickly interact with OpenAI's GPT models instead of relying on the web interface.
 
 ## Table of Contents
 
 1. [Description](#description)
 2. [Installation](#installation)
+3. [Setup](#Setup)
 3. [Usage](#Usage)
 4. [Todos](#Todos)
 5. [License](#License)
 
 ## Description
 
 qprom is a small project that lets you interact with OpenAI's GPT-4 and 3.5 chat API, quickly without having to use the web-ui.
@@ -41,14 +23,20 @@
 ## Installation
 
 
 ```
 pip install qprom
 ```
 
+## Setup
+
+Make sure you have your [OpenAI API key](https://platform.openai.com/account/api-keys).
+
+When running qprom the script tries to fetch the OpenAI API key from a credentials file located in the `.qprom` folder within the user's home directory. 
+If the API key is not found in the credentials file, the user is prompted to provide it, and the provided key is then stored in the aforementioned credentials file for future use.
 
 ## Usage
 
 | Argument | Type | Default | Choices | Description                                                                                            | Optional |
 |---|---|---|---|--------------------------------------------------------------------------------------------------------|---|
 | `-p` | String | None | None | Option to directly enter your prompt (Do not use this flag if you intend to have a multi-line prompt.) | yes |
 | `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model                                                                             | yes |
@@ -70,35 +58,36 @@
 
 ```bash
 qprom -p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -v
 ```
 
 This will run the script with the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and verbose mode enabled.
 
-### Multi line promting
+### Multi line prompting
 To facilitate multi-line input for the prompt, invoke qprom without utilizing the -p parameter. This will prompt you for your input at runtime, where you can provide multiple lines as needed. To signal the end of your input, simply enter the string 'END'.
 
 ```bash
 qprom
 ```
 
 This will run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask for the prompt during runtime.
 
 ## Todos
 
 * Testing
 * Add conversation mode
 * Add option to select default model in config
+* Add option to set the token limit for the conversation modes history
 * Add option to disable streaming and only print the full response
 
 
 **Bug reports:**
 
 
 ## License
 
 MIT [Link](https://github.com/MartinWie/qprom/blob/master/LICENSE)
 
 ## Support me :heart: :star: :money_with_wings:
 If this project provided value, and you want to give something back, you can give the repo a star or support by buying me a coffee.
 
-<a href="https://buymeacoffee.com/MartinWie" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" width="170"></a>
+<a href="https://buymeacoffee.com/MartinWie" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" width="170"></a>
```

#### html2text {}

```diff
@@ -1,48 +1,45 @@
-Metadata-Version: 2.1 Name: qprom Version: 0.5 Summary: A Python-based CLI tool
-to quickly interact with OpenAIs GPT models instead of relying on the web
-interface. Home-page: https://github.com/MartinWie/qprom Download-URL: https://
-github.com/MartinWie/AEnv/archive/2.0.2.tar.gz Author: MartinWiechmann Author-
-email: donotsuspend@googlegroups.com License: MIT Keywords: GPT-4 CLI GPT-
-3 OpenAI Classifier: Development Status :: 5 - Production/Stable Classifier:
-Environment :: Console Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE # qprom a.k.a Quick Prompt [![OS]
-(https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [!
-[RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)](https://
-github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https://
-badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/) !
-[qprom](https://github.com/MartinWie/qprom/blob/main/qprom_logo.png) A Python-
-based CLI tool to quickly interact with OpenAI's GPT models instead of relying
-on the web interface. ## Table of Contents 1. [Description](#description) 2.
-[Installation](#installation) 3. [Usage](#Usage) 4. [Todos](#Todos) 5.
-[License](#License) ## Description qprom is a small project that lets you
-interact with OpenAI's GPT-4 and 3.5 chat API, quickly without having to use
-the web-ui. This enables quicker response times and better [data privacy]
-(https://openai.com/policies/api-data-usage-policies) ## Installation ``` pip
-install qprom ``` ## Usage | Argument | Type | Default | Choices | Description
-| Optional | |---|---|---|---|-------------------------------------------------
--------------------------------------------------------|---| | `-p` | String |
-None | None | Option to directly enter your prompt (Do not use this flag if you
-intend to have a multi-line prompt.) | yes | | `-m` | String | `gpt-4` | `gpt-
-3.5-turbo`, `gpt-4` | Option to select the model | yes | | `-t` | Float | `0.3`
-| Between `0` and `2` | Option to configure the temperature | yes | | `-v` |
-Boolean | `False` | None | Enable verbose mode | yes | ### Usage ```bash qprom
--p  -m  -t  -v ``` - ``: Replace with your prompt - ``: Replace with either
-`gpt-3.5-turbo` or `gpt-4` - ``: Replace with a float value between `0` and `2`
-- `-v`: Add this flag to enable verbose mode For example: ```bash qprom -
-p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -
-v ``` This will run the script with the provided prompt, using the `gpt-4`
-model, a temperature of `0.7`, and verbose mode enabled. ### Multi line
-promting To facilitate multi-line input for the prompt, invoke qprom without
-utilizing the -p parameter. This will prompt you for your input at runtime,
-where you can provide multiple lines as needed. To signal the end of your
-input, simply enter the string 'END'. ```bash qprom ``` This will run qprom
-with default values model: `gpt-4`, a temperature of `0.7` and ask for the
-prompt during runtime. ## Todos * Testing * Add conversation mode * Add option
-to select default model in config * Add option to disable streaming and only
-print the full response **Bug reports:** ## License MIT [Link](https://
-github.com/MartinWie/qprom/blob/master/LICENSE) ## Support me :heart: :star: :
-money_with_wings: If this project provided value, and you want to give
-something back, you can give the repo a star or support by buying me a coffee.
-[Buy_Me_A_Coffee]
+# qprom a.k.a Quick Prompt [![OS](https://img.shields.io/badge/Runs%20on%3A-
+Linux%20%7C%20Mac-green)]() [![RunsOn](https://img.shields.io/github/license/
+MartinWie/AEnv)](https://github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open
+Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://
+opensource.org/) ![qprom](https://github.com/MartinWie/qprom/blob/main/
+qprom_logo.png) A Python-based CLI tool to quickly interact with OpenAI's GPT
+models instead of relying on the web interface. ## Table of Contents 1.
+[Description](#description) 2. [Installation](#installation) 3. [Setup](#Setup)
+3. [Usage](#Usage) 4. [Todos](#Todos) 5. [License](#License) ## Description
+qprom is a small project that lets you interact with OpenAI's GPT-4 and 3.5
+chat API, quickly without having to use the web-ui. This enables quicker
+response times and better [data privacy](https://openai.com/policies/api-data-
+usage-policies) ## Installation ``` pip install qprom ``` ## Setup Make sure
+you have your [OpenAI API key](https://platform.openai.com/account/api-keys).
+When running qprom the script tries to fetch the OpenAI API key from a
+credentials file located in the `.qprom` folder within the user's home
+directory. If the API key is not found in the credentials file, the user is
+prompted to provide it, and the provided key is then stored in the
+aforementioned credentials file for future use. ## Usage | Argument | Type |
+Default | Choices | Description | Optional | |---|---|---|---|-----------------
+-------------------------------------------------------------------------------
+--------|---| | `-p` | String | None | None | Option to directly enter your
+prompt (Do not use this flag if you intend to have a multi-line prompt.) | yes
+| | `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the
+model | yes | | `-t` | Float | `0.3` | Between `0` and `2` | Option to
+configure the temperature | yes | | `-v` | Boolean | `False` | None | Enable
+verbose mode | yes | ### Usage ```bash qprom -p  -m  -t  -v ``` - ``: Replace
+with your prompt - ``: Replace with either `gpt-3.5-turbo` or `gpt-4` - ``:
+Replace with a float value between `0` and `2` - `-v`: Add this flag to enable
+verbose mode For example: ```bash qprom -p "Translate the following English
+text to French: '{text}'" -m gpt-4 -t 0.7 -v ``` This will run the script with
+the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and
+verbose mode enabled. ### Multi line prompting To facilitate multi-line input
+for the prompt, invoke qprom without utilizing the -p parameter. This will
+prompt you for your input at runtime, where you can provide multiple lines as
+needed. To signal the end of your input, simply enter the string 'END'. ```bash
+qprom ``` This will run qprom with default values model: `gpt-4`, a temperature
+of `0.7` and ask for the prompt during runtime. ## Todos * Testing * Add
+conversation mode * Add option to select default model in config * Add option
+to set the token limit for the conversation modes history * Add option to
+disable streaming and only print the full response **Bug reports:** ## License
+MIT [Link](https://github.com/MartinWie/qprom/blob/master/LICENSE) ## Support
+me :heart: :star: :money_with_wings: If this project provided value, and you
+want to give something back, you can give the repo a star or support by buying
+me a coffee. [Buy_Me_A_Coffee]
```

### Comparing `qprom-0.5/README.md` & `qprom-0.5.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,293 @@
-00000000: 2320 7170 726f 6d20 612e 6b2e 6120 5175  # qprom a.k.a Qu
-00000010: 6963 6b20 5072 6f6d 7074 0a0a 5b21 5b4f  ick Prompt..[![O
-00000020: 535d 2868 7474 7073 3a2f 2f69 6d67 2e73  S](https://img.s
-00000030: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000040: 5275 6e73 2532 306f 6e25 3341 2d4c 696e  Runs%20on%3A-Lin
-00000050: 7578 2532 3025 3743 2532 304d 6163 2d67  ux%20%7C%20Mac-g
-00000060: 7265 656e 295d 2829 205b 215b 5275 6e73  reen)]() [![Runs
-00000070: 4f6e 5d28 6874 7470 733a 2f2f 696d 672e  On](https://img.
-00000080: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000090: 622f 6c69 6365 6e73 652f 4d61 7274 696e  b/license/Martin
-000000a0: 5769 652f 4145 6e76 295d 2868 7474 7073  Wie/AEnv)](https
-000000b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d61  ://github.com/Ma
-000000c0: 7274 696e 5769 652f 4145 6e76 2f62 6c6f  rtinWie/AEnv/blo
-000000d0: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-000000e0: 2920 5b21 5b4f 7065 6e20 536f 7572 6365  ) [![Open Source
-000000f0: 5d28 6874 7470 733a 2f2f 6261 6467 6573  ](https://badges
-00000100: 2e66 7261 7073 6f66 742e 636f 6d2f 6f73  .frapsoft.com/os
-00000110: 2f76 312f 6f70 656e 2d73 6f75 7263 652e  /v1/open-source.
-00000120: 7376 673f 763d 3130 3329 5d28 6874 7470  svg?v=103)](http
-00000130: 733a 2f2f 6f70 656e 736f 7572 6365 2e6f  s://opensource.o
-00000140: 7267 2f29 0a0a 215b 7170 726f 6d5d 2868  rg/)..![qprom](h
-00000150: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000160: 6d2f 4d61 7274 696e 5769 652f 7170 726f  m/MartinWie/qpro
-00000170: 6d2f 626c 6f62 2f6d 6169 6e2f 7170 726f  m/blob/main/qpro
-00000180: 6d5f 6c6f 676f 2e70 6e67 290a 0a41 2050  m_logo.png)..A P
-00000190: 7974 686f 6e2d 6261 7365 6420 434c 4920  ython-based CLI 
-000001a0: 746f 6f6c 2074 6f20 7175 6963 6b6c 7920  tool to quickly 
-000001b0: 696e 7465 7261 6374 2077 6974 6820 4f70  interact with Op
-000001c0: 656e 4149 2773 2047 5054 206d 6f64 656c  enAI's GPT model
-000001d0: 7320 696e 7374 6561 6420 6f66 2072 656c  s instead of rel
-000001e0: 7969 6e67 206f 6e20 7468 6520 7765 6220  ying on the web 
-000001f0: 696e 7465 7266 6163 652e 0a0a 2323 2054  interface...## T
-00000200: 6162 6c65 206f 6620 436f 6e74 656e 7473  able of Contents
-00000210: 0a0a 312e 205b 4465 7363 7269 7074 696f  ..1. [Descriptio
-00000220: 6e5d 2823 6465 7363 7269 7074 696f 6e29  n](#description)
-00000230: 0a32 2e20 5b49 6e73 7461 6c6c 6174 696f  .2. [Installatio
-00000240: 6e5d 2823 696e 7374 616c 6c61 7469 6f6e  n](#installation
-00000250: 290a 332e 205b 5573 6167 655d 2823 5573  ).3. [Usage](#Us
-00000260: 6167 6529 0a34 2e20 5b54 6f64 6f73 5d28  age).4. [Todos](
-00000270: 2354 6f64 6f73 290a 352e 205b 4c69 6365  #Todos).5. [Lice
-00000280: 6e73 655d 2823 4c69 6365 6e73 6529 0a0a  nse](#License)..
-00000290: 2323 2044 6573 6372 6970 7469 6f6e 0a0a  ## Description..
-000002a0: 7170 726f 6d20 6973 2061 2073 6d61 6c6c  qprom is a small
-000002b0: 2070 726f 6a65 6374 2074 6861 7420 6c65   project that le
-000002c0: 7473 2079 6f75 2069 6e74 6572 6163 7420  ts you interact 
-000002d0: 7769 7468 204f 7065 6e41 4927 7320 4750  with OpenAI's GP
-000002e0: 542d 3420 616e 6420 332e 3520 6368 6174  T-4 and 3.5 chat
-000002f0: 2041 5049 2c20 7175 6963 6b6c 7920 7769   API, quickly wi
-00000300: 7468 6f75 7420 6861 7669 6e67 2074 6f20  thout having to 
-00000310: 7573 6520 7468 6520 7765 622d 7569 2e0a  use the web-ui..
-00000320: 5468 6973 2065 6e61 626c 6573 2071 7569  This enables qui
-00000330: 636b 6572 2072 6573 706f 6e73 6520 7469  cker response ti
-00000340: 6d65 7320 616e 6420 6265 7474 6572 205b  mes and better [
-00000350: 6461 7461 2070 7269 7661 6379 5d28 6874  data privacy](ht
-00000360: 7470 733a 2f2f 6f70 656e 6169 2e63 6f6d  tps://openai.com
-00000370: 2f70 6f6c 6963 6965 732f 6170 692d 6461  /policies/api-da
-00000380: 7461 2d75 7361 6765 2d70 6f6c 6963 6965  ta-usage-policie
-00000390: 7329 0a0a 2323 2049 6e73 7461 6c6c 6174  s)..## Installat
-000003a0: 696f 6e0a 0a0a 6060 600a 7069 7020 696e  ion...```.pip in
-000003b0: 7374 616c 6c20 7170 726f 6d0a 6060 600a  stall qprom.```.
-000003c0: 0a0a 2323 2055 7361 6765 0a0a 7c20 4172  ..## Usage..| Ar
-000003d0: 6775 6d65 6e74 207c 2054 7970 6520 7c20  gument | Type | 
-000003e0: 4465 6661 756c 7420 7c20 4368 6f69 6365  Default | Choice
-000003f0: 7320 7c20 4465 7363 7269 7074 696f 6e20  s | Description 
-00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 2020 2020 2020 2020 2020 207c 204f 7074             | Opt
-00000460: 696f 6e61 6c20 7c0a 7c2d 2d2d 7c2d 2d2d  ional |.|---|---
-00000470: 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 2d2d 2d2d  |---|---|-------
-00000480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004e0: 2d7c 2d2d 2d7c 0a7c 2060 2d70 6020 7c20  -|---|.| `-p` | 
-000004f0: 5374 7269 6e67 207c 204e 6f6e 6520 7c20  String | None | 
-00000500: 4e6f 6e65 207c 204f 7074 696f 6e20 746f  None | Option to
-00000510: 2064 6972 6563 746c 7920 656e 7465 7220   directly enter 
-00000520: 796f 7572 2070 726f 6d70 7420 2844 6f20  your prompt (Do 
-00000530: 6e6f 7420 7573 6520 7468 6973 2066 6c61  not use this fla
-00000540: 6720 6966 2079 6f75 2069 6e74 656e 6420  g if you intend 
-00000550: 746f 2068 6176 6520 6120 6d75 6c74 692d  to have a multi-
-00000560: 6c69 6e65 2070 726f 6d70 742e 2920 7c20  line prompt.) | 
-00000570: 7965 7320 7c0a 7c20 602d 6d60 207c 2053  yes |.| `-m` | S
-00000580: 7472 696e 6720 7c20 6067 7074 2d34 6020  tring | `gpt-4` 
-00000590: 7c20 6067 7074 2d33 2e35 2d74 7572 626f  | `gpt-3.5-turbo
-000005a0: 602c 2060 6770 742d 3460 207c 204f 7074  `, `gpt-4` | Opt
-000005b0: 696f 6e20 746f 2073 656c 6563 7420 7468  ion to select th
-000005c0: 6520 6d6f 6465 6c20 2020 2020 2020 2020  e model         
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 2020 7c20 7965 7320 7c0a 7c20 602d      | yes |.| `-
-00000620: 7460 207c 2046 6c6f 6174 207c 2060 302e  t` | Float | `0.
-00000630: 3360 207c 2042 6574 7765 656e 2060 3060  3` | Between `0`
-00000640: 2061 6e64 2060 3260 207c 204f 7074 696f   and `2` | Optio
-00000650: 6e20 746f 2063 6f6e 6669 6775 7265 2074  n to configure t
-00000660: 6865 2074 656d 7065 7261 7475 7265 2020  he temperature  
-00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006b0: 2020 7c20 7965 7320 7c0a 7c20 602d 7660    | yes |.| `-v`
-000006c0: 207c 2042 6f6f 6c65 616e 207c 2060 4661   | Boolean | `Fa
-000006d0: 6c73 6560 207c 204e 6f6e 6520 7c20 456e  lse` | None | En
-000006e0: 6162 6c65 2076 6572 626f 7365 206d 6f64  able verbose mod
-000006f0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2020 2020 207c 2079 6573 207c 0a0a 2323       | yes |..##
-00000750: 2320 5573 6167 650a 0a60 6060 6261 7368  # Usage..```bash
-00000760: 0a71 7072 6f6d 202d 7020 3c70 726f 6d70  .qprom -p <promp
-00000770: 743e 202d 6d20 3c6d 6f64 656c 3e20 2d74  t> -m <model> -t
-00000780: 203c 7465 6d70 6572 6174 7572 653e 202d   <temperature> -
-00000790: 760a 6060 600a 0a2d 2060 3c70 726f 6d70  v.```..- `<promp
-000007a0: 743e 603a 2052 6570 6c61 6365 2077 6974  t>`: Replace wit
-000007b0: 6820 796f 7572 2070 726f 6d70 740a 2d20  h your prompt.- 
-000007c0: 603c 6d6f 6465 6c3e 603a 2052 6570 6c61  `<model>`: Repla
-000007d0: 6365 2077 6974 6820 6569 7468 6572 2060  ce with either `
-000007e0: 6770 742d 332e 352d 7475 7262 6f60 206f  gpt-3.5-turbo` o
-000007f0: 7220 6067 7074 2d34 600a 2d20 603c 7465  r `gpt-4`.- `<te
-00000800: 6d70 6572 6174 7572 653e 603a 2052 6570  mperature>`: Rep
-00000810: 6c61 6365 2077 6974 6820 6120 666c 6f61  lace with a floa
-00000820: 7420 7661 6c75 6520 6265 7477 6565 6e20  t value between 
-00000830: 6030 6020 616e 6420 6032 600a 2d20 602d  `0` and `2`.- `-
-00000840: 7660 3a20 4164 6420 7468 6973 2066 6c61  v`: Add this fla
-00000850: 6720 746f 2065 6e61 626c 6520 7665 7262  g to enable verb
-00000860: 6f73 6520 6d6f 6465 0a0a 466f 7220 6578  ose mode..For ex
-00000870: 616d 706c 653a 0a0a 6060 6062 6173 680a  ample:..```bash.
-00000880: 7170 726f 6d20 2d70 2022 5472 616e 736c  qprom -p "Transl
-00000890: 6174 6520 7468 6520 666f 6c6c 6f77 696e  ate the followin
-000008a0: 6720 456e 676c 6973 6820 7465 7874 2074  g English text t
-000008b0: 6f20 4672 656e 6368 3a20 277b 7465 7874  o French: '{text
-000008c0: 7d27 2220 2d6d 2067 7074 2d34 202d 7420  }'" -m gpt-4 -t 
-000008d0: 302e 3720 2d76 0a60 6060 0a0a 5468 6973  0.7 -v.```..This
-000008e0: 2077 696c 6c20 7275 6e20 7468 6520 7363   will run the sc
-000008f0: 7269 7074 2077 6974 6820 7468 6520 7072  ript with the pr
-00000900: 6f76 6964 6564 2070 726f 6d70 742c 2075  ovided prompt, u
-00000910: 7369 6e67 2074 6865 2060 6770 742d 3460  sing the `gpt-4`
-00000920: 206d 6f64 656c 2c20 6120 7465 6d70 6572   model, a temper
-00000930: 6174 7572 6520 6f66 2060 302e 3760 2c20  ature of `0.7`, 
-00000940: 616e 6420 7665 7262 6f73 6520 6d6f 6465  and verbose mode
-00000950: 2065 6e61 626c 6564 2e0a 0a23 2323 204d   enabled...### M
-00000960: 756c 7469 206c 696e 6520 7072 6f6d 7469  ulti line promti
-00000970: 6e67 0a54 6f20 6661 6369 6c69 7461 7465  ng.To facilitate
-00000980: 206d 756c 7469 2d6c 696e 6520 696e 7075   multi-line inpu
-00000990: 7420 666f 7220 7468 6520 7072 6f6d 7074  t for the prompt
-000009a0: 2c20 696e 766f 6b65 2071 7072 6f6d 2077  , invoke qprom w
-000009b0: 6974 686f 7574 2075 7469 6c69 7a69 6e67  ithout utilizing
-000009c0: 2074 6865 202d 7020 7061 7261 6d65 7465   the -p paramete
-000009d0: 722e 2054 6869 7320 7769 6c6c 2070 726f  r. This will pro
-000009e0: 6d70 7420 796f 7520 666f 7220 796f 7572  mpt you for your
-000009f0: 2069 6e70 7574 2061 7420 7275 6e74 696d   input at runtim
-00000a00: 652c 2077 6865 7265 2079 6f75 2063 616e  e, where you can
-00000a10: 2070 726f 7669 6465 206d 756c 7469 706c   provide multipl
-00000a20: 6520 6c69 6e65 7320 6173 206e 6565 6465  e lines as neede
-00000a30: 642e 2054 6f20 7369 676e 616c 2074 6865  d. To signal the
-00000a40: 2065 6e64 206f 6620 796f 7572 2069 6e70   end of your inp
-00000a50: 7574 2c20 7369 6d70 6c79 2065 6e74 6572  ut, simply enter
-00000a60: 2074 6865 2073 7472 696e 6720 2745 4e44   the string 'END
-00000a70: 272e 0a0a 6060 6062 6173 680a 7170 726f  '...```bash.qpro
-00000a80: 6d0a 6060 600a 0a54 6869 7320 7769 6c6c  m.```..This will
-00000a90: 2072 756e 2071 7072 6f6d 2077 6974 6820   run qprom with 
-00000aa0: 6465 6661 756c 7420 7661 6c75 6573 206d  default values m
-00000ab0: 6f64 656c 3a20 6067 7074 2d34 602c 2061  odel: `gpt-4`, a
-00000ac0: 2074 656d 7065 7261 7475 7265 206f 6620   temperature of 
-00000ad0: 6030 2e37 6020 616e 6420 6173 6b20 666f  `0.7` and ask fo
-00000ae0: 7220 7468 6520 7072 6f6d 7074 2064 7572  r the prompt dur
-00000af0: 696e 6720 7275 6e74 696d 652e 0a0a 2323  ing runtime...##
-00000b00: 2054 6f64 6f73 0a0a 2a20 5465 7374 696e   Todos..* Testin
-00000b10: 670a 2a20 4164 6420 636f 6e76 6572 7361  g.* Add conversa
-00000b20: 7469 6f6e 206d 6f64 650a 2a20 4164 6420  tion mode.* Add 
-00000b30: 6f70 7469 6f6e 2074 6f20 7365 6c65 6374  option to select
-00000b40: 2064 6566 6175 6c74 206d 6f64 656c 2069   default model i
-00000b50: 6e20 636f 6e66 6967 0a2a 2041 6464 206f  n config.* Add o
-00000b60: 7074 696f 6e20 746f 2064 6973 6162 6c65  ption to disable
-00000b70: 2073 7472 6561 6d69 6e67 2061 6e64 206f   streaming and o
-00000b80: 6e6c 7920 7072 696e 7420 7468 6520 6675  nly print the fu
-00000b90: 6c6c 2072 6573 706f 6e73 650a 0a0a 2a2a  ll response...**
-00000ba0: 4275 6720 7265 706f 7274 733a 2a2a 0a0a  Bug reports:**..
-00000bb0: 0a23 2320 4c69 6365 6e73 650a 0a4d 4954  .## License..MIT
-00000bc0: 205b 4c69 6e6b 5d28 6874 7470 733a 2f2f   [Link](https://
-00000bd0: 6769 7468 7562 2e63 6f6d 2f4d 6172 7469  github.com/Marti
-00000be0: 6e57 6965 2f71 7072 6f6d 2f62 6c6f 622f  nWie/qprom/blob/
-00000bf0: 6d61 7374 6572 2f4c 4943 454e 5345 290a  master/LICENSE).
-00000c00: 0a23 2320 5375 7070 6f72 7420 6d65 203a  .## Support me :
-00000c10: 6865 6172 743a 203a 7374 6172 3a20 3a6d  heart: :star: :m
-00000c20: 6f6e 6579 5f77 6974 685f 7769 6e67 733a  oney_with_wings:
-00000c30: 0a49 6620 7468 6973 2070 726f 6a65 6374  .If this project
-00000c40: 2070 726f 7669 6465 6420 7661 6c75 652c   provided value,
-00000c50: 2061 6e64 2079 6f75 2077 616e 7420 746f   and you want to
-00000c60: 2067 6976 6520 736f 6d65 7468 696e 6720   give something 
-00000c70: 6261 636b 2c20 796f 7520 6361 6e20 6769  back, you can gi
-00000c80: 7665 2074 6865 2072 6570 6f20 6120 7374  ve the repo a st
-00000c90: 6172 206f 7220 7375 7070 6f72 7420 6279  ar or support by
-00000ca0: 2062 7579 696e 6720 6d65 2061 2063 6f66   buying me a cof
-00000cb0: 6665 652e 0a0a 3c61 2068 7265 663d 2268  fee...<a href="h
-00000cc0: 7474 7073 3a2f 2f62 7579 6d65 6163 6f66  ttps://buymeacof
-00000cd0: 6665 652e 636f 6d2f 4d61 7274 696e 5769  fee.com/MartinWi
-00000ce0: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
-00000cf0: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
-00000d00: 7073 3a2f 2f63 646e 2e62 7579 6d65 6163  ps://cdn.buymeac
-00000d10: 6f66 6665 652e 636f 6d2f 6275 7474 6f6e  offee.com/button
-00000d20: 732f 7632 2f64 6566 6175 6c74 2d62 6c75  s/v2/default-blu
-00000d30: 652e 706e 6722 2061 6c74 3d22 4275 7920  e.png" alt="Buy 
-00000d40: 4d65 2041 2043 6f66 6665 6522 2077 6964  Me A Coffee" wid
-00000d50: 7468 3d22 3137 3022 3e3c 2f61 3e         th="170"></a>
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7170 726f  : 2.1.Name: qpro
+00000020: 6d0a 5665 7273 696f 6e3a 2030 2e35 2e31  m.Version: 0.5.1
+00000030: 0a53 756d 6d61 7279 3a20 4120 5079 7468  .Summary: A Pyth
+00000040: 6f6e 2d62 6173 6564 2043 4c49 2074 6f6f  on-based CLI too
+00000050: 6c20 746f 2071 7569 636b 6c79 2069 6e74  l to quickly int
+00000060: 6572 6163 7420 7769 7468 204f 7065 6e41  eract with OpenA
+00000070: 4973 2047 5054 206d 6f64 656c 7320 696e  Is GPT models in
+00000080: 7374 6561 6420 6f66 2072 656c 7969 6e67  stead of relying
+00000090: 206f 6e20 7468 6520 7765 6220 696e 7465   on the web inte
+000000a0: 7266 6163 652e 0a48 6f6d 652d 7061 6765  rface..Home-page
+000000b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000000c0: 2e63 6f6d 2f4d 6172 7469 6e57 6965 2f71  .com/MartinWie/q
+000000d0: 7072 6f6d 0a44 6f77 6e6c 6f61 642d 5552  prom.Download-UR
+000000e0: 4c3a 2068 7474 7073 3a2f 2f67 6974 6875  L: https://githu
+000000f0: 622e 636f 6d2f 4d61 7274 696e 5769 652f  b.com/MartinWie/
+00000100: 4145 6e76 2f61 7263 6869 7665 2f32 2e30  AEnv/archive/2.0
+00000110: 2e32 2e74 6172 2e67 7a0a 4175 7468 6f72  .2.tar.gz.Author
+00000120: 3a20 4d61 7274 696e 5769 6563 686d 616e  : MartinWiechman
+00000130: 6e0a 4175 7468 6f72 2d65 6d61 696c 3a20  n.Author-email: 
+00000140: 646f 6e6f 7473 7573 7065 6e64 4067 6f6f  donotsuspend@goo
+00000150: 676c 6567 726f 7570 732e 636f 6d0a 4c69  glegroups.com.Li
+00000160: 6365 6e73 653a 204d 4954 0a4b 6579 776f  cense: MIT.Keywo
+00000170: 7264 733a 2047 5054 2d34 2043 4c49 2047  rds: GPT-4 CLI G
+00000180: 5054 2d33 204f 7065 6e41 490a 436c 6173  PT-3 OpenAI.Clas
+00000190: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
+000001a0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
+000001b0: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
+000001c0: 626c 650a 436c 6173 7369 6669 6572 3a20  ble.Classifier: 
+000001d0: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
+000001e0: 6f6e 736f 6c65 0a43 6c61 7373 6966 6965  onsole.Classifie
+000001f0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000200: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+00000210: 7273 0a43 6c61 7373 6966 6965 723a 204c  rs.Classifier: L
+00000220: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000230: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000240: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
+00000250: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000260: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000270: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+00000280: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000290: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000002a0: 6465 6e74 0a44 6573 6372 6970 7469 6f6e  dent.Description
+000002b0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002c0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+000002d0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000002e0: 5345 0a0a 2320 7170 726f 6d20 612e 6b2e  SE..# qprom a.k.
+000002f0: 6120 5175 6963 6b20 5072 6f6d 7074 0a0a  a Quick Prompt..
+00000300: 5b21 5b4f 535d 2868 7474 7073 3a2f 2f69  [![OS](https://i
+00000310: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000320: 6467 652f 5275 6e73 2532 306f 6e25 3341  dge/Runs%20on%3A
+00000330: 2d4c 696e 7578 2532 3025 3743 2532 304d  -Linux%20%7C%20M
+00000340: 6163 2d67 7265 656e 295d 2829 205b 215b  ac-green)]() [![
+00000350: 5275 6e73 4f6e 5d28 6874 7470 733a 2f2f  RunsOn](https://
+00000360: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000370: 6974 6875 622f 6c69 6365 6e73 652f 4d61  ithub/license/Ma
+00000380: 7274 696e 5769 652f 4145 6e76 295d 2868  rtinWie/AEnv)](h
+00000390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003a0: 6d2f 4d61 7274 696e 5769 652f 4145 6e76  m/MartinWie/AEnv
+000003b0: 2f62 6c6f 622f 6d61 7374 6572 2f4c 4943  /blob/master/LIC
+000003c0: 454e 5345 2920 5b21 5b4f 7065 6e20 536f  ENSE) [![Open So
+000003d0: 7572 6365 5d28 6874 7470 733a 2f2f 6261  urce](https://ba
+000003e0: 6467 6573 2e66 7261 7073 6f66 742e 636f  dges.frapsoft.co
+000003f0: 6d2f 6f73 2f76 312f 6f70 656e 2d73 6f75  m/os/v1/open-sou
+00000400: 7263 652e 7376 673f 763d 3130 3329 5d28  rce.svg?v=103)](
+00000410: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00000420: 6365 2e6f 7267 2f29 0a0a 215b 7170 726f  ce.org/)..![qpro
+00000430: 6d5d 2868 7474 7073 3a2f 2f67 6974 6875  m](https://githu
+00000440: 622e 636f 6d2f 4d61 7274 696e 5769 652f  b.com/MartinWie/
+00000450: 7170 726f 6d2f 626c 6f62 2f6d 6169 6e2f  qprom/blob/main/
+00000460: 7170 726f 6d5f 6c6f 676f 2e70 6e67 290a  qprom_logo.png).
+00000470: 0a41 2050 7974 686f 6e2d 6261 7365 6420  .A Python-based 
+00000480: 434c 4920 746f 6f6c 2074 6f20 7175 6963  CLI tool to quic
+00000490: 6b6c 7920 696e 7465 7261 6374 2077 6974  kly interact wit
+000004a0: 6820 4f70 656e 4149 2773 2047 5054 206d  h OpenAI's GPT m
+000004b0: 6f64 656c 7320 696e 7374 6561 6420 6f66  odels instead of
+000004c0: 2072 656c 7969 6e67 206f 6e20 7468 6520   relying on the 
+000004d0: 7765 6220 696e 7465 7266 6163 652e 0a0a  web interface...
+000004e0: 2323 2054 6162 6c65 206f 6620 436f 6e74  ## Table of Cont
+000004f0: 656e 7473 0a0a 312e 205b 4465 7363 7269  ents..1. [Descri
+00000500: 7074 696f 6e5d 2823 6465 7363 7269 7074  ption](#descript
+00000510: 696f 6e29 0a32 2e20 5b49 6e73 7461 6c6c  ion).2. [Install
+00000520: 6174 696f 6e5d 2823 696e 7374 616c 6c61  ation](#installa
+00000530: 7469 6f6e 290a 332e 205b 5365 7475 705d  tion).3. [Setup]
+00000540: 2823 5365 7475 7029 0a33 2e20 5b55 7361  (#Setup).3. [Usa
+00000550: 6765 5d28 2355 7361 6765 290a 342e 205b  ge](#Usage).4. [
+00000560: 546f 646f 735d 2823 546f 646f 7329 0a35  Todos](#Todos).5
+00000570: 2e20 5b4c 6963 656e 7365 5d28 234c 6963  . [License](#Lic
+00000580: 656e 7365 290a 0a23 2320 4465 7363 7269  ense)..## Descri
+00000590: 7074 696f 6e0a 0a71 7072 6f6d 2069 7320  ption..qprom is 
+000005a0: 6120 736d 616c 6c20 7072 6f6a 6563 7420  a small project 
+000005b0: 7468 6174 206c 6574 7320 796f 7520 696e  that lets you in
+000005c0: 7465 7261 6374 2077 6974 6820 4f70 656e  teract with Open
+000005d0: 4149 2773 2047 5054 2d34 2061 6e64 2033  AI's GPT-4 and 3
+000005e0: 2e35 2063 6861 7420 4150 492c 2071 7569  .5 chat API, qui
+000005f0: 636b 6c79 2077 6974 686f 7574 2068 6176  ckly without hav
+00000600: 696e 6720 746f 2075 7365 2074 6865 2077  ing to use the w
+00000610: 6562 2d75 692e 0a54 6869 7320 656e 6162  eb-ui..This enab
+00000620: 6c65 7320 7175 6963 6b65 7220 7265 7370  les quicker resp
+00000630: 6f6e 7365 2074 696d 6573 2061 6e64 2062  onse times and b
+00000640: 6574 7465 7220 5b64 6174 6120 7072 6976  etter [data priv
+00000650: 6163 795d 2868 7474 7073 3a2f 2f6f 7065  acy](https://ope
+00000660: 6e61 692e 636f 6d2f 706f 6c69 6369 6573  nai.com/policies
+00000670: 2f61 7069 2d64 6174 612d 7573 6167 652d  /api-data-usage-
+00000680: 706f 6c69 6369 6573 290a 0a23 2320 496e  policies)..## In
+00000690: 7374 616c 6c61 7469 6f6e 0a0a 0a60 6060  stallation...```
+000006a0: 0a70 6970 2069 6e73 7461 6c6c 2071 7072  .pip install qpr
+000006b0: 6f6d 0a60 6060 0a0a 2323 2053 6574 7570  om.```..## Setup
+000006c0: 0a0a 4d61 6b65 2073 7572 6520 796f 7520  ..Make sure you 
+000006d0: 6861 7665 2079 6f75 7220 5b4f 7065 6e41  have your [OpenA
+000006e0: 4920 4150 4920 6b65 795d 2868 7474 7073  I API key](https
+000006f0: 3a2f 2f70 6c61 7466 6f72 6d2e 6f70 656e  ://platform.open
+00000700: 6169 2e63 6f6d 2f61 6363 6f75 6e74 2f61  ai.com/account/a
+00000710: 7069 2d6b 6579 7329 2e0a 0a57 6865 6e20  pi-keys)...When 
+00000720: 7275 6e6e 696e 6720 7170 726f 6d20 7468  running qprom th
+00000730: 6520 7363 7269 7074 2074 7269 6573 2074  e script tries t
+00000740: 6f20 6665 7463 6820 7468 6520 4f70 656e  o fetch the Open
+00000750: 4149 2041 5049 206b 6579 2066 726f 6d20  AI API key from 
+00000760: 6120 6372 6564 656e 7469 616c 7320 6669  a credentials fi
+00000770: 6c65 206c 6f63 6174 6564 2069 6e20 7468  le located in th
+00000780: 6520 602e 7170 726f 6d60 2066 6f6c 6465  e `.qprom` folde
+00000790: 7220 7769 7468 696e 2074 6865 2075 7365  r within the use
+000007a0: 7227 7320 686f 6d65 2064 6972 6563 746f  r's home directo
+000007b0: 7279 2e20 0a49 6620 7468 6520 4150 4920  ry. .If the API 
+000007c0: 6b65 7920 6973 206e 6f74 2066 6f75 6e64  key is not found
+000007d0: 2069 6e20 7468 6520 6372 6564 656e 7469   in the credenti
+000007e0: 616c 7320 6669 6c65 2c20 7468 6520 7573  als file, the us
+000007f0: 6572 2069 7320 7072 6f6d 7074 6564 2074  er is prompted t
+00000800: 6f20 7072 6f76 6964 6520 6974 2c20 616e  o provide it, an
+00000810: 6420 7468 6520 7072 6f76 6964 6564 206b  d the provided k
+00000820: 6579 2069 7320 7468 656e 2073 746f 7265  ey is then store
+00000830: 6420 696e 2074 6865 2061 666f 7265 6d65  d in the aforeme
+00000840: 6e74 696f 6e65 6420 6372 6564 656e 7469  ntioned credenti
+00000850: 616c 7320 6669 6c65 2066 6f72 2066 7574  als file for fut
+00000860: 7572 6520 7573 652e 0a0a 2323 2055 7361  ure use...## Usa
+00000870: 6765 0a0a 7c20 4172 6775 6d65 6e74 207c  ge..| Argument |
+00000880: 2054 7970 6520 7c20 4465 6661 756c 7420   Type | Default 
+00000890: 7c20 4368 6f69 6365 7320 7c20 4465 7363  | Choices | Desc
+000008a0: 7269 7074 696f 6e20 2020 2020 2020 2020  ription         
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2020 207c 204f 7074 696f 6e61 6c20 7c0a     | Optional |.
+00000910: 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d  |---|---|---|---
+00000920: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00000930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000980: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d7c 0a7c  ---------|---|.|
+00000990: 2060 2d70 6020 7c20 5374 7269 6e67 207c   `-p` | String |
+000009a0: 204e 6f6e 6520 7c20 4e6f 6e65 207c 204f   None | None | O
+000009b0: 7074 696f 6e20 746f 2064 6972 6563 746c  ption to directl
+000009c0: 7920 656e 7465 7220 796f 7572 2070 726f  y enter your pro
+000009d0: 6d70 7420 2844 6f20 6e6f 7420 7573 6520  mpt (Do not use 
+000009e0: 7468 6973 2066 6c61 6720 6966 2079 6f75  this flag if you
+000009f0: 2069 6e74 656e 6420 746f 2068 6176 6520   intend to have 
+00000a00: 6120 6d75 6c74 692d 6c69 6e65 2070 726f  a multi-line pro
+00000a10: 6d70 742e 2920 7c20 7965 7320 7c0a 7c20  mpt.) | yes |.| 
+00000a20: 602d 6d60 207c 2053 7472 696e 6720 7c20  `-m` | String | 
+00000a30: 6067 7074 2d34 6020 7c20 6067 7074 2d33  `gpt-4` | `gpt-3
+00000a40: 2e35 2d74 7572 626f 602c 2060 6770 742d  .5-turbo`, `gpt-
+00000a50: 3460 207c 204f 7074 696f 6e20 746f 2073  4` | Option to s
+00000a60: 656c 6563 7420 7468 6520 6d6f 6465 6c20  elect the model 
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 7c20 7965              | ye
+00000ac0: 7320 7c0a 7c20 602d 7460 207c 2046 6c6f  s |.| `-t` | Flo
+00000ad0: 6174 207c 2060 302e 3360 207c 2042 6574  at | `0.3` | Bet
+00000ae0: 7765 656e 2060 3060 2061 6e64 2060 3260  ween `0` and `2`
+00000af0: 207c 204f 7074 696f 6e20 746f 2063 6f6e   | Option to con
+00000b00: 6669 6775 7265 2074 6865 2074 656d 7065  figure the tempe
+00000b10: 7261 7475 7265 2020 2020 2020 2020 2020  rature          
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 2020 2020 2020 7c20 7965 7320            | yes 
+00000b60: 7c0a 7c20 602d 7660 207c 2042 6f6f 6c65  |.| `-v` | Boole
+00000b70: 616e 207c 2060 4661 6c73 6560 207c 204e  an | `False` | N
+00000b80: 6f6e 6520 7c20 456e 6162 6c65 2076 6572  one | Enable ver
+00000b90: 626f 7365 206d 6f64 6520 2020 2020 2020  bose mode       
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 2020 2020 2020 2020 2020 2020 207c 2079               | y
+00000bf0: 6573 207c 0a0a 2323 2320 5573 6167 650a  es |..### Usage.
+00000c00: 0a60 6060 6261 7368 0a71 7072 6f6d 202d  .```bash.qprom -
+00000c10: 7020 3c70 726f 6d70 743e 202d 6d20 3c6d  p <prompt> -m <m
+00000c20: 6f64 656c 3e20 2d74 203c 7465 6d70 6572  odel> -t <temper
+00000c30: 6174 7572 653e 202d 760a 6060 600a 0a2d  ature> -v.```..-
+00000c40: 2060 3c70 726f 6d70 743e 603a 2052 6570   `<prompt>`: Rep
+00000c50: 6c61 6365 2077 6974 6820 796f 7572 2070  lace with your p
+00000c60: 726f 6d70 740a 2d20 603c 6d6f 6465 6c3e  rompt.- `<model>
+00000c70: 603a 2052 6570 6c61 6365 2077 6974 6820  `: Replace with 
+00000c80: 6569 7468 6572 2060 6770 742d 332e 352d  either `gpt-3.5-
+00000c90: 7475 7262 6f60 206f 7220 6067 7074 2d34  turbo` or `gpt-4
+00000ca0: 600a 2d20 603c 7465 6d70 6572 6174 7572  `.- `<temperatur
+00000cb0: 653e 603a 2052 6570 6c61 6365 2077 6974  e>`: Replace wit
+00000cc0: 6820 6120 666c 6f61 7420 7661 6c75 6520  h a float value 
+00000cd0: 6265 7477 6565 6e20 6030 6020 616e 6420  between `0` and 
+00000ce0: 6032 600a 2d20 602d 7660 3a20 4164 6420  `2`.- `-v`: Add 
+00000cf0: 7468 6973 2066 6c61 6720 746f 2065 6e61  this flag to ena
+00000d00: 626c 6520 7665 7262 6f73 6520 6d6f 6465  ble verbose mode
+00000d10: 0a0a 466f 7220 6578 616d 706c 653a 0a0a  ..For example:..
+00000d20: 6060 6062 6173 680a 7170 726f 6d20 2d70  ```bash.qprom -p
+00000d30: 2022 5472 616e 736c 6174 6520 7468 6520   "Translate the 
+00000d40: 666f 6c6c 6f77 696e 6720 456e 676c 6973  following Englis
+00000d50: 6820 7465 7874 2074 6f20 4672 656e 6368  h text to French
+00000d60: 3a20 277b 7465 7874 7d27 2220 2d6d 2067  : '{text}'" -m g
+00000d70: 7074 2d34 202d 7420 302e 3720 2d76 0a60  pt-4 -t 0.7 -v.`
+00000d80: 6060 0a0a 5468 6973 2077 696c 6c20 7275  ``..This will ru
+00000d90: 6e20 7468 6520 7363 7269 7074 2077 6974  n the script wit
+00000da0: 6820 7468 6520 7072 6f76 6964 6564 2070  h the provided p
+00000db0: 726f 6d70 742c 2075 7369 6e67 2074 6865  rompt, using the
+00000dc0: 2060 6770 742d 3460 206d 6f64 656c 2c20   `gpt-4` model, 
+00000dd0: 6120 7465 6d70 6572 6174 7572 6520 6f66  a temperature of
+00000de0: 2060 302e 3760 2c20 616e 6420 7665 7262   `0.7`, and verb
+00000df0: 6f73 6520 6d6f 6465 2065 6e61 626c 6564  ose mode enabled
+00000e00: 2e0a 0a23 2323 204d 756c 7469 206c 696e  ...### Multi lin
+00000e10: 6520 7072 6f6d 7074 696e 670a 546f 2066  e prompting.To f
+00000e20: 6163 696c 6974 6174 6520 6d75 6c74 692d  acilitate multi-
+00000e30: 6c69 6e65 2069 6e70 7574 2066 6f72 2074  line input for t
+00000e40: 6865 2070 726f 6d70 742c 2069 6e76 6f6b  he prompt, invok
+00000e50: 6520 7170 726f 6d20 7769 7468 6f75 7420  e qprom without 
+00000e60: 7574 696c 697a 696e 6720 7468 6520 2d70  utilizing the -p
+00000e70: 2070 6172 616d 6574 6572 2e20 5468 6973   parameter. This
+00000e80: 2077 696c 6c20 7072 6f6d 7074 2079 6f75   will prompt you
+00000e90: 2066 6f72 2079 6f75 7220 696e 7075 7420   for your input 
+00000ea0: 6174 2072 756e 7469 6d65 2c20 7768 6572  at runtime, wher
+00000eb0: 6520 796f 7520 6361 6e20 7072 6f76 6964  e you can provid
+00000ec0: 6520 6d75 6c74 6970 6c65 206c 696e 6573  e multiple lines
+00000ed0: 2061 7320 6e65 6564 6564 2e20 546f 2073   as needed. To s
+00000ee0: 6967 6e61 6c20 7468 6520 656e 6420 6f66  ignal the end of
+00000ef0: 2079 6f75 7220 696e 7075 742c 2073 696d   your input, sim
+00000f00: 706c 7920 656e 7465 7220 7468 6520 7374  ply enter the st
+00000f10: 7269 6e67 2027 454e 4427 2e0a 0a60 6060  ring 'END'...```
+00000f20: 6261 7368 0a71 7072 6f6d 0a60 6060 0a0a  bash.qprom.```..
+00000f30: 5468 6973 2077 696c 6c20 7275 6e20 7170  This will run qp
+00000f40: 726f 6d20 7769 7468 2064 6566 6175 6c74  rom with default
+00000f50: 2076 616c 7565 7320 6d6f 6465 6c3a 2060   values model: `
+00000f60: 6770 742d 3460 2c20 6120 7465 6d70 6572  gpt-4`, a temper
+00000f70: 6174 7572 6520 6f66 2060 302e 3760 2061  ature of `0.7` a
+00000f80: 6e64 2061 736b 2066 6f72 2074 6865 2070  nd ask for the p
+00000f90: 726f 6d70 7420 6475 7269 6e67 2072 756e  rompt during run
+00000fa0: 7469 6d65 2e0a 0a23 2320 546f 646f 730a  time...## Todos.
+00000fb0: 0a2a 2054 6573 7469 6e67 0a2a 2041 6464  .* Testing.* Add
+00000fc0: 2063 6f6e 7665 7273 6174 696f 6e20 6d6f   conversation mo
+00000fd0: 6465 0a2a 2041 6464 206f 7074 696f 6e20  de.* Add option 
+00000fe0: 746f 2073 656c 6563 7420 6465 6661 756c  to select defaul
+00000ff0: 7420 6d6f 6465 6c20 696e 2063 6f6e 6669  t model in confi
+00001000: 670a 2a20 4164 6420 6f70 7469 6f6e 2074  g.* Add option t
+00001010: 6f20 7365 7420 7468 6520 746f 6b65 6e20  o set the token 
+00001020: 6c69 6d69 7420 666f 7220 7468 6520 636f  limit for the co
+00001030: 6e76 6572 7361 7469 6f6e 206d 6f64 6573  nversation modes
+00001040: 2068 6973 746f 7279 0a2a 2041 6464 206f   history.* Add o
+00001050: 7074 696f 6e20 746f 2064 6973 6162 6c65  ption to disable
+00001060: 2073 7472 6561 6d69 6e67 2061 6e64 206f   streaming and o
+00001070: 6e6c 7920 7072 696e 7420 7468 6520 6675  nly print the fu
+00001080: 6c6c 2072 6573 706f 6e73 650a 0a0a 2a2a  ll response...**
+00001090: 4275 6720 7265 706f 7274 733a 2a2a 0a0a  Bug reports:**..
+000010a0: 0a23 2320 4c69 6365 6e73 650a 0a4d 4954  .## License..MIT
+000010b0: 205b 4c69 6e6b 5d28 6874 7470 733a 2f2f   [Link](https://
+000010c0: 6769 7468 7562 2e63 6f6d 2f4d 6172 7469  github.com/Marti
+000010d0: 6e57 6965 2f71 7072 6f6d 2f62 6c6f 622f  nWie/qprom/blob/
+000010e0: 6d61 7374 6572 2f4c 4943 454e 5345 290a  master/LICENSE).
+000010f0: 0a23 2320 5375 7070 6f72 7420 6d65 203a  .## Support me :
+00001100: 6865 6172 743a 203a 7374 6172 3a20 3a6d  heart: :star: :m
+00001110: 6f6e 6579 5f77 6974 685f 7769 6e67 733a  oney_with_wings:
+00001120: 0a49 6620 7468 6973 2070 726f 6a65 6374  .If this project
+00001130: 2070 726f 7669 6465 6420 7661 6c75 652c   provided value,
+00001140: 2061 6e64 2079 6f75 2077 616e 7420 746f   and you want to
+00001150: 2067 6976 6520 736f 6d65 7468 696e 6720   give something 
+00001160: 6261 636b 2c20 796f 7520 6361 6e20 6769  back, you can gi
+00001170: 7665 2074 6865 2072 6570 6f20 6120 7374  ve the repo a st
+00001180: 6172 206f 7220 7375 7070 6f72 7420 6279  ar or support by
+00001190: 2062 7579 696e 6720 6d65 2061 2063 6f66   buying me a cof
+000011a0: 6665 652e 0a0a 3c61 2068 7265 663d 2268  fee...<a href="h
+000011b0: 7474 7073 3a2f 2f62 7579 6d65 6163 6f66  ttps://buymeacof
+000011c0: 6665 652e 636f 6d2f 4d61 7274 696e 5769  fee.com/MartinWi
+000011d0: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
+000011e0: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
+000011f0: 7073 3a2f 2f63 646e 2e62 7579 6d65 6163  ps://cdn.buymeac
+00001200: 6f66 6665 652e 636f 6d2f 6275 7474 6f6e  offee.com/button
+00001210: 732f 7632 2f64 6566 6175 6c74 2d62 6c75  s/v2/default-blu
+00001220: 652e 706e 6722 2061 6c74 3d22 4275 7920  e.png" alt="Buy 
+00001230: 4d65 2041 2043 6f66 6665 6522 2077 6964  Me A Coffee" wid
+00001240: 7468 3d22 3137 3022 3e3c 2f61 3e0a       th="170"></a>.
```

### Comparing `qprom-0.5/arguments/__init__.py` & `qprom-0.5.1/arguments/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,18 +27,7 @@
     args = parser.parse_args()
 
     # Replace the newline character representation with an actual newline
     if args.p is not None:
         args.p = args.p.replace('\\n', '\n')
 
     return args
-
-
-def get_multiline_input():
-    print("Enter your prompt. Finish by typing 'END' on a new line:")
-    lines = []
-    while True:
-        line = input()
-        if line == 'END':
-            break
-        lines.append(line)
-    return '\n'.join(lines)
```

### Comparing `qprom-0.5/config/credentials.py` & `qprom-0.5.1/config/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def get_api_key():
     # Create a config parser
     config = configparser.ConfigParser()
 
     # Get the path to the credentials file
-    credential_path = os.path.join(os.path.expanduser('~'), '.gptcli', 'credentials.ini')
+    credential_path = os.path.join(os.path.expanduser('~'), '.qprom', 'credentials.ini')
 
     # Read the credentials file
     config.read(credential_path)
 
     # Check if the API key exists
     if config.has_option('default', 'openai_api_key'):
         api_key = config.get('default', 'openai_api_key')
```

### Comparing `qprom-0.5/gpt/request.py` & `qprom-0.5.1/gpt/request.py`

 * *Files identical despite different names*

### Comparing `qprom-0.5/qprom/main.py` & `qprom-0.5.1/qprom/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import openai
-from arguments import get_args, get_multiline_input
+from arguments import get_args
 from config.credentials import get_api_key
 from gpt.request import openai_request, print_streamed_response
+from qprom.utils import get_multiline_input
 
 
 def main():
     openai.api_key = get_api_key()
 
     args = get_args()
```

### Comparing `qprom-0.5/qprom.egg-info/PKG-INFO` & `qprom-0.5.1/qprom.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,260 +1,293 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7170 726f  : 2.1.Name: qpro
-00000020: 6d0a 5665 7273 696f 6e3a 2030 2e35 0a53  m.Version: 0.5.S
-00000030: 756d 6d61 7279 3a20 4120 5079 7468 6f6e  ummary: A Python
-00000040: 2d62 6173 6564 2043 4c49 2074 6f6f 6c20  -based CLI tool 
-00000050: 746f 2071 7569 636b 6c79 2069 6e74 6572  to quickly inter
-00000060: 6163 7420 7769 7468 204f 7065 6e41 4973  act with OpenAIs
-00000070: 2047 5054 206d 6f64 656c 7320 696e 7374   GPT models inst
-00000080: 6561 6420 6f66 2072 656c 7969 6e67 206f  ead of relying o
-00000090: 6e20 7468 6520 7765 6220 696e 7465 7266  n the web interf
-000000a0: 6163 652e 0a48 6f6d 652d 7061 6765 3a20  ace..Home-page: 
-000000b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000c0: 6f6d 2f4d 6172 7469 6e57 6965 2f71 7072  om/MartinWie/qpr
-000000d0: 6f6d 0a44 6f77 6e6c 6f61 642d 5552 4c3a  om.Download-URL:
-000000e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000f0: 636f 6d2f 4d61 7274 696e 5769 652f 4145  com/MartinWie/AE
-00000100: 6e76 2f61 7263 6869 7665 2f32 2e30 2e32  nv/archive/2.0.2
-00000110: 2e74 6172 2e67 7a0a 4175 7468 6f72 3a20  .tar.gz.Author: 
-00000120: 4d61 7274 696e 5769 6563 686d 616e 6e0a  MartinWiechmann.
-00000130: 4175 7468 6f72 2d65 6d61 696c 3a20 646f  Author-email: do
-00000140: 6e6f 7473 7573 7065 6e64 4067 6f6f 676c  notsuspend@googl
-00000150: 6567 726f 7570 732e 636f 6d0a 4c69 6365  egroups.com.Lice
-00000160: 6e73 653a 204d 4954 0a4b 6579 776f 7264  nse: MIT.Keyword
-00000170: 733a 2047 5054 2d34 2043 4c49 2047 5054  s: GPT-4 CLI GPT
-00000180: 2d33 204f 7065 6e41 490a 436c 6173 7369  -3 OpenAI.Classi
-00000190: 6669 6572 3a20 4465 7665 6c6f 706d 656e  fier: Developmen
-000001a0: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
-000001b0: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
-000001c0: 650a 436c 6173 7369 6669 6572 3a20 456e  e.Classifier: En
-000001d0: 7669 726f 6e6d 656e 7420 3a3a 2043 6f6e  vironment :: Con
-000001e0: 736f 6c65 0a43 6c61 7373 6966 6965 723a  sole.Classifier:
-000001f0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-00000200: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-00000210: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-00000220: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000230: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000240: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
-00000250: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000260: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000270: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-00000280: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000290: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000002a0: 6e74 0a44 6573 6372 6970 7469 6f6e 2d43  nt.Description-C
-000002b0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000002c0: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
-000002d0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000002e0: 0a0a 2320 7170 726f 6d20 612e 6b2e 6120  ..# qprom a.k.a 
-000002f0: 5175 6963 6b20 5072 6f6d 7074 0a0a 5b21  Quick Prompt..[!
-00000300: 5b4f 535d 2868 7474 7073 3a2f 2f69 6d67  [OS](https://img
-00000310: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000320: 652f 5275 6e73 2532 306f 6e25 3341 2d4c  e/Runs%20on%3A-L
-00000330: 696e 7578 2532 3025 3743 2532 304d 6163  inux%20%7C%20Mac
-00000340: 2d67 7265 656e 295d 2829 205b 215b 5275  -green)]() [![Ru
-00000350: 6e73 4f6e 5d28 6874 7470 733a 2f2f 696d  nsOn](https://im
-00000360: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00000370: 6875 622f 6c69 6365 6e73 652f 4d61 7274  hub/license/Mart
-00000380: 696e 5769 652f 4145 6e76 295d 2868 7474  inWie/AEnv)](htt
-00000390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000003a0: 4d61 7274 696e 5769 652f 4145 6e76 2f62  MartinWie/AEnv/b
-000003b0: 6c6f 622f 6d61 7374 6572 2f4c 4943 454e  lob/master/LICEN
-000003c0: 5345 2920 5b21 5b4f 7065 6e20 536f 7572  SE) [![Open Sour
-000003d0: 6365 5d28 6874 7470 733a 2f2f 6261 6467  ce](https://badg
-000003e0: 6573 2e66 7261 7073 6f66 742e 636f 6d2f  es.frapsoft.com/
-000003f0: 6f73 2f76 312f 6f70 656e 2d73 6f75 7263  os/v1/open-sourc
-00000400: 652e 7376 673f 763d 3130 3329 5d28 6874  e.svg?v=103)](ht
-00000410: 7470 733a 2f2f 6f70 656e 736f 7572 6365  tps://opensource
-00000420: 2e6f 7267 2f29 0a0a 215b 7170 726f 6d5d  .org/)..![qprom]
-00000430: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000440: 636f 6d2f 4d61 7274 696e 5769 652f 7170  com/MartinWie/qp
-00000450: 726f 6d2f 626c 6f62 2f6d 6169 6e2f 7170  rom/blob/main/qp
-00000460: 726f 6d5f 6c6f 676f 2e70 6e67 290a 0a41  rom_logo.png)..A
-00000470: 2050 7974 686f 6e2d 6261 7365 6420 434c   Python-based CL
-00000480: 4920 746f 6f6c 2074 6f20 7175 6963 6b6c  I tool to quickl
-00000490: 7920 696e 7465 7261 6374 2077 6974 6820  y interact with 
-000004a0: 4f70 656e 4149 2773 2047 5054 206d 6f64  OpenAI's GPT mod
-000004b0: 656c 7320 696e 7374 6561 6420 6f66 2072  els instead of r
-000004c0: 656c 7969 6e67 206f 6e20 7468 6520 7765  elying on the we
-000004d0: 6220 696e 7465 7266 6163 652e 0a0a 2323  b interface...##
-000004e0: 2054 6162 6c65 206f 6620 436f 6e74 656e   Table of Conten
-000004f0: 7473 0a0a 312e 205b 4465 7363 7269 7074  ts..1. [Descript
-00000500: 696f 6e5d 2823 6465 7363 7269 7074 696f  ion](#descriptio
-00000510: 6e29 0a32 2e20 5b49 6e73 7461 6c6c 6174  n).2. [Installat
-00000520: 696f 6e5d 2823 696e 7374 616c 6c61 7469  ion](#installati
-00000530: 6f6e 290a 332e 205b 5573 6167 655d 2823  on).3. [Usage](#
-00000540: 5573 6167 6529 0a34 2e20 5b54 6f64 6f73  Usage).4. [Todos
-00000550: 5d28 2354 6f64 6f73 290a 352e 205b 4c69  ](#Todos).5. [Li
-00000560: 6365 6e73 655d 2823 4c69 6365 6e73 6529  cense](#License)
-00000570: 0a0a 2323 2044 6573 6372 6970 7469 6f6e  ..## Description
-00000580: 0a0a 7170 726f 6d20 6973 2061 2073 6d61  ..qprom is a sma
-00000590: 6c6c 2070 726f 6a65 6374 2074 6861 7420  ll project that 
-000005a0: 6c65 7473 2079 6f75 2069 6e74 6572 6163  lets you interac
-000005b0: 7420 7769 7468 204f 7065 6e41 4927 7320  t with OpenAI's 
-000005c0: 4750 542d 3420 616e 6420 332e 3520 6368  GPT-4 and 3.5 ch
-000005d0: 6174 2041 5049 2c20 7175 6963 6b6c 7920  at API, quickly 
-000005e0: 7769 7468 6f75 7420 6861 7669 6e67 2074  without having t
-000005f0: 6f20 7573 6520 7468 6520 7765 622d 7569  o use the web-ui
-00000600: 2e0a 5468 6973 2065 6e61 626c 6573 2071  ..This enables q
-00000610: 7569 636b 6572 2072 6573 706f 6e73 6520  uicker response 
-00000620: 7469 6d65 7320 616e 6420 6265 7474 6572  times and better
-00000630: 205b 6461 7461 2070 7269 7661 6379 5d28   [data privacy](
-00000640: 6874 7470 733a 2f2f 6f70 656e 6169 2e63  https://openai.c
-00000650: 6f6d 2f70 6f6c 6963 6965 732f 6170 692d  om/policies/api-
-00000660: 6461 7461 2d75 7361 6765 2d70 6f6c 6963  data-usage-polic
-00000670: 6965 7329 0a0a 2323 2049 6e73 7461 6c6c  ies)..## Install
-00000680: 6174 696f 6e0a 0a0a 6060 600a 7069 7020  ation...```.pip 
-00000690: 696e 7374 616c 6c20 7170 726f 6d0a 6060  install qprom.``
-000006a0: 600a 0a0a 2323 2055 7361 6765 0a0a 7c20  `...## Usage..| 
-000006b0: 4172 6775 6d65 6e74 207c 2054 7970 6520  Argument | Type 
-000006c0: 7c20 4465 6661 756c 7420 7c20 4368 6f69  | Default | Choi
-000006d0: 6365 7320 7c20 4465 7363 7269 7074 696f  ces | Descriptio
-000006e0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000730: 2020 2020 2020 2020 2020 2020 207c 204f               | O
-00000740: 7074 696f 6e61 6c20 7c0a 7c2d 2d2d 7c2d  ptional |.|---|-
-00000750: 2d2d 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 2d2d  --|---|---|-----
-00000760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000007a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000007b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000007c0: 2d2d 2d7c 2d2d 2d7c 0a7c 2060 2d70 6020  ---|---|.| `-p` 
-000007d0: 7c20 5374 7269 6e67 207c 204e 6f6e 6520  | String | None 
-000007e0: 7c20 4e6f 6e65 207c 204f 7074 696f 6e20  | None | Option 
-000007f0: 746f 2064 6972 6563 746c 7920 656e 7465  to directly ente
-00000800: 7220 796f 7572 2070 726f 6d70 7420 2844  r your prompt (D
-00000810: 6f20 6e6f 7420 7573 6520 7468 6973 2066  o not use this f
-00000820: 6c61 6720 6966 2079 6f75 2069 6e74 656e  lag if you inten
-00000830: 6420 746f 2068 6176 6520 6120 6d75 6c74  d to have a mult
-00000840: 692d 6c69 6e65 2070 726f 6d70 742e 2920  i-line prompt.) 
-00000850: 7c20 7965 7320 7c0a 7c20 602d 6d60 207c  | yes |.| `-m` |
-00000860: 2053 7472 696e 6720 7c20 6067 7074 2d34   String | `gpt-4
-00000870: 6020 7c20 6067 7074 2d33 2e35 2d74 7572  ` | `gpt-3.5-tur
-00000880: 626f 602c 2060 6770 742d 3460 207c 204f  bo`, `gpt-4` | O
-00000890: 7074 696f 6e20 746f 2073 656c 6563 7420  ption to select 
-000008a0: 7468 6520 6d6f 6465 6c20 2020 2020 2020  the model       
+00000020: 6d0a 5665 7273 696f 6e3a 2030 2e35 2e31  m.Version: 0.5.1
+00000030: 0a53 756d 6d61 7279 3a20 4120 5079 7468  .Summary: A Pyth
+00000040: 6f6e 2d62 6173 6564 2043 4c49 2074 6f6f  on-based CLI too
+00000050: 6c20 746f 2071 7569 636b 6c79 2069 6e74  l to quickly int
+00000060: 6572 6163 7420 7769 7468 204f 7065 6e41  eract with OpenA
+00000070: 4973 2047 5054 206d 6f64 656c 7320 696e  Is GPT models in
+00000080: 7374 6561 6420 6f66 2072 656c 7969 6e67  stead of relying
+00000090: 206f 6e20 7468 6520 7765 6220 696e 7465   on the web inte
+000000a0: 7266 6163 652e 0a48 6f6d 652d 7061 6765  rface..Home-page
+000000b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000000c0: 2e63 6f6d 2f4d 6172 7469 6e57 6965 2f71  .com/MartinWie/q
+000000d0: 7072 6f6d 0a44 6f77 6e6c 6f61 642d 5552  prom.Download-UR
+000000e0: 4c3a 2068 7474 7073 3a2f 2f67 6974 6875  L: https://githu
+000000f0: 622e 636f 6d2f 4d61 7274 696e 5769 652f  b.com/MartinWie/
+00000100: 4145 6e76 2f61 7263 6869 7665 2f32 2e30  AEnv/archive/2.0
+00000110: 2e32 2e74 6172 2e67 7a0a 4175 7468 6f72  .2.tar.gz.Author
+00000120: 3a20 4d61 7274 696e 5769 6563 686d 616e  : MartinWiechman
+00000130: 6e0a 4175 7468 6f72 2d65 6d61 696c 3a20  n.Author-email: 
+00000140: 646f 6e6f 7473 7573 7065 6e64 4067 6f6f  donotsuspend@goo
+00000150: 676c 6567 726f 7570 732e 636f 6d0a 4c69  glegroups.com.Li
+00000160: 6365 6e73 653a 204d 4954 0a4b 6579 776f  cense: MIT.Keywo
+00000170: 7264 733a 2047 5054 2d34 2043 4c49 2047  rds: GPT-4 CLI G
+00000180: 5054 2d33 204f 7065 6e41 490a 436c 6173  PT-3 OpenAI.Clas
+00000190: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
+000001a0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
+000001b0: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
+000001c0: 626c 650a 436c 6173 7369 6669 6572 3a20  ble.Classifier: 
+000001d0: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
+000001e0: 6f6e 736f 6c65 0a43 6c61 7373 6966 6965  onsole.Classifie
+000001f0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000200: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+00000210: 7273 0a43 6c61 7373 6966 6965 723a 204c  rs.Classifier: L
+00000220: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000230: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000240: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
+00000250: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000260: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000270: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+00000280: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000290: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000002a0: 6465 6e74 0a44 6573 6372 6970 7469 6f6e  dent.Description
+000002b0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002c0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+000002d0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000002e0: 5345 0a0a 2320 7170 726f 6d20 612e 6b2e  SE..# qprom a.k.
+000002f0: 6120 5175 6963 6b20 5072 6f6d 7074 0a0a  a Quick Prompt..
+00000300: 5b21 5b4f 535d 2868 7474 7073 3a2f 2f69  [![OS](https://i
+00000310: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000320: 6467 652f 5275 6e73 2532 306f 6e25 3341  dge/Runs%20on%3A
+00000330: 2d4c 696e 7578 2532 3025 3743 2532 304d  -Linux%20%7C%20M
+00000340: 6163 2d67 7265 656e 295d 2829 205b 215b  ac-green)]() [![
+00000350: 5275 6e73 4f6e 5d28 6874 7470 733a 2f2f  RunsOn](https://
+00000360: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000370: 6974 6875 622f 6c69 6365 6e73 652f 4d61  ithub/license/Ma
+00000380: 7274 696e 5769 652f 4145 6e76 295d 2868  rtinWie/AEnv)](h
+00000390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003a0: 6d2f 4d61 7274 696e 5769 652f 4145 6e76  m/MartinWie/AEnv
+000003b0: 2f62 6c6f 622f 6d61 7374 6572 2f4c 4943  /blob/master/LIC
+000003c0: 454e 5345 2920 5b21 5b4f 7065 6e20 536f  ENSE) [![Open So
+000003d0: 7572 6365 5d28 6874 7470 733a 2f2f 6261  urce](https://ba
+000003e0: 6467 6573 2e66 7261 7073 6f66 742e 636f  dges.frapsoft.co
+000003f0: 6d2f 6f73 2f76 312f 6f70 656e 2d73 6f75  m/os/v1/open-sou
+00000400: 7263 652e 7376 673f 763d 3130 3329 5d28  rce.svg?v=103)](
+00000410: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00000420: 6365 2e6f 7267 2f29 0a0a 215b 7170 726f  ce.org/)..![qpro
+00000430: 6d5d 2868 7474 7073 3a2f 2f67 6974 6875  m](https://githu
+00000440: 622e 636f 6d2f 4d61 7274 696e 5769 652f  b.com/MartinWie/
+00000450: 7170 726f 6d2f 626c 6f62 2f6d 6169 6e2f  qprom/blob/main/
+00000460: 7170 726f 6d5f 6c6f 676f 2e70 6e67 290a  qprom_logo.png).
+00000470: 0a41 2050 7974 686f 6e2d 6261 7365 6420  .A Python-based 
+00000480: 434c 4920 746f 6f6c 2074 6f20 7175 6963  CLI tool to quic
+00000490: 6b6c 7920 696e 7465 7261 6374 2077 6974  kly interact wit
+000004a0: 6820 4f70 656e 4149 2773 2047 5054 206d  h OpenAI's GPT m
+000004b0: 6f64 656c 7320 696e 7374 6561 6420 6f66  odels instead of
+000004c0: 2072 656c 7969 6e67 206f 6e20 7468 6520   relying on the 
+000004d0: 7765 6220 696e 7465 7266 6163 652e 0a0a  web interface...
+000004e0: 2323 2054 6162 6c65 206f 6620 436f 6e74  ## Table of Cont
+000004f0: 656e 7473 0a0a 312e 205b 4465 7363 7269  ents..1. [Descri
+00000500: 7074 696f 6e5d 2823 6465 7363 7269 7074  ption](#descript
+00000510: 696f 6e29 0a32 2e20 5b49 6e73 7461 6c6c  ion).2. [Install
+00000520: 6174 696f 6e5d 2823 696e 7374 616c 6c61  ation](#installa
+00000530: 7469 6f6e 290a 332e 205b 5365 7475 705d  tion).3. [Setup]
+00000540: 2823 5365 7475 7029 0a33 2e20 5b55 7361  (#Setup).3. [Usa
+00000550: 6765 5d28 2355 7361 6765 290a 342e 205b  ge](#Usage).4. [
+00000560: 546f 646f 735d 2823 546f 646f 7329 0a35  Todos](#Todos).5
+00000570: 2e20 5b4c 6963 656e 7365 5d28 234c 6963  . [License](#Lic
+00000580: 656e 7365 290a 0a23 2320 4465 7363 7269  ense)..## Descri
+00000590: 7074 696f 6e0a 0a71 7072 6f6d 2069 7320  ption..qprom is 
+000005a0: 6120 736d 616c 6c20 7072 6f6a 6563 7420  a small project 
+000005b0: 7468 6174 206c 6574 7320 796f 7520 696e  that lets you in
+000005c0: 7465 7261 6374 2077 6974 6820 4f70 656e  teract with Open
+000005d0: 4149 2773 2047 5054 2d34 2061 6e64 2033  AI's GPT-4 and 3
+000005e0: 2e35 2063 6861 7420 4150 492c 2071 7569  .5 chat API, qui
+000005f0: 636b 6c79 2077 6974 686f 7574 2068 6176  ckly without hav
+00000600: 696e 6720 746f 2075 7365 2074 6865 2077  ing to use the w
+00000610: 6562 2d75 692e 0a54 6869 7320 656e 6162  eb-ui..This enab
+00000620: 6c65 7320 7175 6963 6b65 7220 7265 7370  les quicker resp
+00000630: 6f6e 7365 2074 696d 6573 2061 6e64 2062  onse times and b
+00000640: 6574 7465 7220 5b64 6174 6120 7072 6976  etter [data priv
+00000650: 6163 795d 2868 7474 7073 3a2f 2f6f 7065  acy](https://ope
+00000660: 6e61 692e 636f 6d2f 706f 6c69 6369 6573  nai.com/policies
+00000670: 2f61 7069 2d64 6174 612d 7573 6167 652d  /api-data-usage-
+00000680: 706f 6c69 6369 6573 290a 0a23 2320 496e  policies)..## In
+00000690: 7374 616c 6c61 7469 6f6e 0a0a 0a60 6060  stallation...```
+000006a0: 0a70 6970 2069 6e73 7461 6c6c 2071 7072  .pip install qpr
+000006b0: 6f6d 0a60 6060 0a0a 2323 2053 6574 7570  om.```..## Setup
+000006c0: 0a0a 4d61 6b65 2073 7572 6520 796f 7520  ..Make sure you 
+000006d0: 6861 7665 2079 6f75 7220 5b4f 7065 6e41  have your [OpenA
+000006e0: 4920 4150 4920 6b65 795d 2868 7474 7073  I API key](https
+000006f0: 3a2f 2f70 6c61 7466 6f72 6d2e 6f70 656e  ://platform.open
+00000700: 6169 2e63 6f6d 2f61 6363 6f75 6e74 2f61  ai.com/account/a
+00000710: 7069 2d6b 6579 7329 2e0a 0a57 6865 6e20  pi-keys)...When 
+00000720: 7275 6e6e 696e 6720 7170 726f 6d20 7468  running qprom th
+00000730: 6520 7363 7269 7074 2074 7269 6573 2074  e script tries t
+00000740: 6f20 6665 7463 6820 7468 6520 4f70 656e  o fetch the Open
+00000750: 4149 2041 5049 206b 6579 2066 726f 6d20  AI API key from 
+00000760: 6120 6372 6564 656e 7469 616c 7320 6669  a credentials fi
+00000770: 6c65 206c 6f63 6174 6564 2069 6e20 7468  le located in th
+00000780: 6520 602e 7170 726f 6d60 2066 6f6c 6465  e `.qprom` folde
+00000790: 7220 7769 7468 696e 2074 6865 2075 7365  r within the use
+000007a0: 7227 7320 686f 6d65 2064 6972 6563 746f  r's home directo
+000007b0: 7279 2e20 0a49 6620 7468 6520 4150 4920  ry. .If the API 
+000007c0: 6b65 7920 6973 206e 6f74 2066 6f75 6e64  key is not found
+000007d0: 2069 6e20 7468 6520 6372 6564 656e 7469   in the credenti
+000007e0: 616c 7320 6669 6c65 2c20 7468 6520 7573  als file, the us
+000007f0: 6572 2069 7320 7072 6f6d 7074 6564 2074  er is prompted t
+00000800: 6f20 7072 6f76 6964 6520 6974 2c20 616e  o provide it, an
+00000810: 6420 7468 6520 7072 6f76 6964 6564 206b  d the provided k
+00000820: 6579 2069 7320 7468 656e 2073 746f 7265  ey is then store
+00000830: 6420 696e 2074 6865 2061 666f 7265 6d65  d in the aforeme
+00000840: 6e74 696f 6e65 6420 6372 6564 656e 7469  ntioned credenti
+00000850: 616c 7320 6669 6c65 2066 6f72 2066 7574  als file for fut
+00000860: 7572 6520 7573 652e 0a0a 2323 2055 7361  ure use...## Usa
+00000870: 6765 0a0a 7c20 4172 6775 6d65 6e74 207c  ge..| Argument |
+00000880: 2054 7970 6520 7c20 4465 6661 756c 7420   Type | Default 
+00000890: 7c20 4368 6f69 6365 7320 7c20 4465 7363  | Choices | Desc
+000008a0: 7269 7074 696f 6e20 2020 2020 2020 2020  ription         
 000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 2020 7c20 7965 7320 7c0a 7c20        | yes |.| 
-00000900: 602d 7460 207c 2046 6c6f 6174 207c 2060  `-t` | Float | `
-00000910: 302e 3360 207c 2042 6574 7765 656e 2060  0.3` | Between `
-00000920: 3060 2061 6e64 2060 3260 207c 204f 7074  0` and `2` | Opt
-00000930: 696f 6e20 746f 2063 6f6e 6669 6775 7265  ion to configure
-00000940: 2074 6865 2074 656d 7065 7261 7475 7265   the temperature
-00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000990: 2020 2020 7c20 7965 7320 7c0a 7c20 602d      | yes |.| `-
-000009a0: 7660 207c 2042 6f6f 6c65 616e 207c 2060  v` | Boolean | `
-000009b0: 4661 6c73 6560 207c 204e 6f6e 6520 7c20  False` | None | 
-000009c0: 456e 6162 6c65 2076 6572 626f 7365 206d  Enable verbose m
-000009d0: 6f64 6520 2020 2020 2020 2020 2020 2020  ode             
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2020 2020 207c 2079 6573 207c 0a0a         | yes |..
-00000a30: 2323 2320 5573 6167 650a 0a60 6060 6261  ### Usage..```ba
-00000a40: 7368 0a71 7072 6f6d 202d 7020 3c70 726f  sh.qprom -p <pro
-00000a50: 6d70 743e 202d 6d20 3c6d 6f64 656c 3e20  mpt> -m <model> 
-00000a60: 2d74 203c 7465 6d70 6572 6174 7572 653e  -t <temperature>
-00000a70: 202d 760a 6060 600a 0a2d 2060 3c70 726f   -v.```..- `<pro
-00000a80: 6d70 743e 603a 2052 6570 6c61 6365 2077  mpt>`: Replace w
-00000a90: 6974 6820 796f 7572 2070 726f 6d70 740a  ith your prompt.
-00000aa0: 2d20 603c 6d6f 6465 6c3e 603a 2052 6570  - `<model>`: Rep
-00000ab0: 6c61 6365 2077 6974 6820 6569 7468 6572  lace with either
-00000ac0: 2060 6770 742d 332e 352d 7475 7262 6f60   `gpt-3.5-turbo`
-00000ad0: 206f 7220 6067 7074 2d34 600a 2d20 603c   or `gpt-4`.- `<
-00000ae0: 7465 6d70 6572 6174 7572 653e 603a 2052  temperature>`: R
-00000af0: 6570 6c61 6365 2077 6974 6820 6120 666c  eplace with a fl
-00000b00: 6f61 7420 7661 6c75 6520 6265 7477 6565  oat value betwee
-00000b10: 6e20 6030 6020 616e 6420 6032 600a 2d20  n `0` and `2`.- 
-00000b20: 602d 7660 3a20 4164 6420 7468 6973 2066  `-v`: Add this f
-00000b30: 6c61 6720 746f 2065 6e61 626c 6520 7665  lag to enable ve
-00000b40: 7262 6f73 6520 6d6f 6465 0a0a 466f 7220  rbose mode..For 
-00000b50: 6578 616d 706c 653a 0a0a 6060 6062 6173  example:..```bas
-00000b60: 680a 7170 726f 6d20 2d70 2022 5472 616e  h.qprom -p "Tran
-00000b70: 736c 6174 6520 7468 6520 666f 6c6c 6f77  slate the follow
-00000b80: 696e 6720 456e 676c 6973 6820 7465 7874  ing English text
-00000b90: 2074 6f20 4672 656e 6368 3a20 277b 7465   to French: '{te
-00000ba0: 7874 7d27 2220 2d6d 2067 7074 2d34 202d  xt}'" -m gpt-4 -
-00000bb0: 7420 302e 3720 2d76 0a60 6060 0a0a 5468  t 0.7 -v.```..Th
-00000bc0: 6973 2077 696c 6c20 7275 6e20 7468 6520  is will run the 
-00000bd0: 7363 7269 7074 2077 6974 6820 7468 6520  script with the 
-00000be0: 7072 6f76 6964 6564 2070 726f 6d70 742c  provided prompt,
-00000bf0: 2075 7369 6e67 2074 6865 2060 6770 742d   using the `gpt-
-00000c00: 3460 206d 6f64 656c 2c20 6120 7465 6d70  4` model, a temp
-00000c10: 6572 6174 7572 6520 6f66 2060 302e 3760  erature of `0.7`
-00000c20: 2c20 616e 6420 7665 7262 6f73 6520 6d6f  , and verbose mo
-00000c30: 6465 2065 6e61 626c 6564 2e0a 0a23 2323  de enabled...###
-00000c40: 204d 756c 7469 206c 696e 6520 7072 6f6d   Multi line prom
-00000c50: 7469 6e67 0a54 6f20 6661 6369 6c69 7461  ting.To facilita
-00000c60: 7465 206d 756c 7469 2d6c 696e 6520 696e  te multi-line in
-00000c70: 7075 7420 666f 7220 7468 6520 7072 6f6d  put for the prom
-00000c80: 7074 2c20 696e 766f 6b65 2071 7072 6f6d  pt, invoke qprom
-00000c90: 2077 6974 686f 7574 2075 7469 6c69 7a69   without utilizi
-00000ca0: 6e67 2074 6865 202d 7020 7061 7261 6d65  ng the -p parame
-00000cb0: 7465 722e 2054 6869 7320 7769 6c6c 2070  ter. This will p
-00000cc0: 726f 6d70 7420 796f 7520 666f 7220 796f  rompt you for yo
-00000cd0: 7572 2069 6e70 7574 2061 7420 7275 6e74  ur input at runt
-00000ce0: 696d 652c 2077 6865 7265 2079 6f75 2063  ime, where you c
-00000cf0: 616e 2070 726f 7669 6465 206d 756c 7469  an provide multi
-00000d00: 706c 6520 6c69 6e65 7320 6173 206e 6565  ple lines as nee
-00000d10: 6465 642e 2054 6f20 7369 676e 616c 2074  ded. To signal t
-00000d20: 6865 2065 6e64 206f 6620 796f 7572 2069  he end of your i
-00000d30: 6e70 7574 2c20 7369 6d70 6c79 2065 6e74  nput, simply ent
-00000d40: 6572 2074 6865 2073 7472 696e 6720 2745  er the string 'E
-00000d50: 4e44 272e 0a0a 6060 6062 6173 680a 7170  ND'...```bash.qp
-00000d60: 726f 6d0a 6060 600a 0a54 6869 7320 7769  rom.```..This wi
-00000d70: 6c6c 2072 756e 2071 7072 6f6d 2077 6974  ll run qprom wit
-00000d80: 6820 6465 6661 756c 7420 7661 6c75 6573  h default values
-00000d90: 206d 6f64 656c 3a20 6067 7074 2d34 602c   model: `gpt-4`,
-00000da0: 2061 2074 656d 7065 7261 7475 7265 206f   a temperature o
-00000db0: 6620 6030 2e37 6020 616e 6420 6173 6b20  f `0.7` and ask 
-00000dc0: 666f 7220 7468 6520 7072 6f6d 7074 2064  for the prompt d
-00000dd0: 7572 696e 6720 7275 6e74 696d 652e 0a0a  uring runtime...
-00000de0: 2323 2054 6f64 6f73 0a0a 2a20 5465 7374  ## Todos..* Test
-00000df0: 696e 670a 2a20 4164 6420 636f 6e76 6572  ing.* Add conver
-00000e00: 7361 7469 6f6e 206d 6f64 650a 2a20 4164  sation mode.* Ad
-00000e10: 6420 6f70 7469 6f6e 2074 6f20 7365 6c65  d option to sele
-00000e20: 6374 2064 6566 6175 6c74 206d 6f64 656c  ct default model
-00000e30: 2069 6e20 636f 6e66 6967 0a2a 2041 6464   in config.* Add
-00000e40: 206f 7074 696f 6e20 746f 2064 6973 6162   option to disab
-00000e50: 6c65 2073 7472 6561 6d69 6e67 2061 6e64  le streaming and
-00000e60: 206f 6e6c 7920 7072 696e 7420 7468 6520   only print the 
-00000e70: 6675 6c6c 2072 6573 706f 6e73 650a 0a0a  full response...
-00000e80: 2a2a 4275 6720 7265 706f 7274 733a 2a2a  **Bug reports:**
-00000e90: 0a0a 0a23 2320 4c69 6365 6e73 650a 0a4d  ...## License..M
-00000ea0: 4954 205b 4c69 6e6b 5d28 6874 7470 733a  IT [Link](https:
-00000eb0: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 6172  //github.com/Mar
-00000ec0: 7469 6e57 6965 2f71 7072 6f6d 2f62 6c6f  tinWie/qprom/blo
-00000ed0: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-00000ee0: 290a 0a23 2320 5375 7070 6f72 7420 6d65  )..## Support me
-00000ef0: 203a 6865 6172 743a 203a 7374 6172 3a20   :heart: :star: 
-00000f00: 3a6d 6f6e 6579 5f77 6974 685f 7769 6e67  :money_with_wing
-00000f10: 733a 0a49 6620 7468 6973 2070 726f 6a65  s:.If this proje
-00000f20: 6374 2070 726f 7669 6465 6420 7661 6c75  ct provided valu
-00000f30: 652c 2061 6e64 2079 6f75 2077 616e 7420  e, and you want 
-00000f40: 746f 2067 6976 6520 736f 6d65 7468 696e  to give somethin
-00000f50: 6720 6261 636b 2c20 796f 7520 6361 6e20  g back, you can 
-00000f60: 6769 7665 2074 6865 2072 6570 6f20 6120  give the repo a 
-00000f70: 7374 6172 206f 7220 7375 7070 6f72 7420  star or support 
-00000f80: 6279 2062 7579 696e 6720 6d65 2061 2063  by buying me a c
-00000f90: 6f66 6665 652e 0a0a 3c61 2068 7265 663d  offee...<a href=
-00000fa0: 2268 7474 7073 3a2f 2f62 7579 6d65 6163  "https://buymeac
-00000fb0: 6f66 6665 652e 636f 6d2f 4d61 7274 696e  offee.com/Martin
-00000fc0: 5769 6522 2074 6172 6765 743d 225f 626c  Wie" target="_bl
-00000fd0: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
-00000fe0: 7474 7073 3a2f 2f63 646e 2e62 7579 6d65  ttps://cdn.buyme
-00000ff0: 6163 6f66 6665 652e 636f 6d2f 6275 7474  acoffee.com/butt
-00001000: 6f6e 732f 7632 2f64 6566 6175 6c74 2d62  ons/v2/default-b
-00001010: 6c75 652e 706e 6722 2061 6c74 3d22 4275  lue.png" alt="Bu
-00001020: 7920 4d65 2041 2043 6f66 6665 6522 2077  y Me A Coffee" w
-00001030: 6964 7468 3d22 3137 3022 3e3c 2f61 3e0a  idth="170"></a>.
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2020 207c 204f 7074 696f 6e61 6c20 7c0a     | Optional |.
+00000910: 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d  |---|---|---|---
+00000920: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00000930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000980: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d7c 0a7c  ---------|---|.|
+00000990: 2060 2d70 6020 7c20 5374 7269 6e67 207c   `-p` | String |
+000009a0: 204e 6f6e 6520 7c20 4e6f 6e65 207c 204f   None | None | O
+000009b0: 7074 696f 6e20 746f 2064 6972 6563 746c  ption to directl
+000009c0: 7920 656e 7465 7220 796f 7572 2070 726f  y enter your pro
+000009d0: 6d70 7420 2844 6f20 6e6f 7420 7573 6520  mpt (Do not use 
+000009e0: 7468 6973 2066 6c61 6720 6966 2079 6f75  this flag if you
+000009f0: 2069 6e74 656e 6420 746f 2068 6176 6520   intend to have 
+00000a00: 6120 6d75 6c74 692d 6c69 6e65 2070 726f  a multi-line pro
+00000a10: 6d70 742e 2920 7c20 7965 7320 7c0a 7c20  mpt.) | yes |.| 
+00000a20: 602d 6d60 207c 2053 7472 696e 6720 7c20  `-m` | String | 
+00000a30: 6067 7074 2d34 6020 7c20 6067 7074 2d33  `gpt-4` | `gpt-3
+00000a40: 2e35 2d74 7572 626f 602c 2060 6770 742d  .5-turbo`, `gpt-
+00000a50: 3460 207c 204f 7074 696f 6e20 746f 2073  4` | Option to s
+00000a60: 656c 6563 7420 7468 6520 6d6f 6465 6c20  elect the model 
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 7c20 7965              | ye
+00000ac0: 7320 7c0a 7c20 602d 7460 207c 2046 6c6f  s |.| `-t` | Flo
+00000ad0: 6174 207c 2060 302e 3360 207c 2042 6574  at | `0.3` | Bet
+00000ae0: 7765 656e 2060 3060 2061 6e64 2060 3260  ween `0` and `2`
+00000af0: 207c 204f 7074 696f 6e20 746f 2063 6f6e   | Option to con
+00000b00: 6669 6775 7265 2074 6865 2074 656d 7065  figure the tempe
+00000b10: 7261 7475 7265 2020 2020 2020 2020 2020  rature          
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 2020 2020 2020 7c20 7965 7320            | yes 
+00000b60: 7c0a 7c20 602d 7660 207c 2042 6f6f 6c65  |.| `-v` | Boole
+00000b70: 616e 207c 2060 4661 6c73 6560 207c 204e  an | `False` | N
+00000b80: 6f6e 6520 7c20 456e 6162 6c65 2076 6572  one | Enable ver
+00000b90: 626f 7365 206d 6f64 6520 2020 2020 2020  bose mode       
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 2020 2020 2020 2020 2020 2020 207c 2079               | y
+00000bf0: 6573 207c 0a0a 2323 2320 5573 6167 650a  es |..### Usage.
+00000c00: 0a60 6060 6261 7368 0a71 7072 6f6d 202d  .```bash.qprom -
+00000c10: 7020 3c70 726f 6d70 743e 202d 6d20 3c6d  p <prompt> -m <m
+00000c20: 6f64 656c 3e20 2d74 203c 7465 6d70 6572  odel> -t <temper
+00000c30: 6174 7572 653e 202d 760a 6060 600a 0a2d  ature> -v.```..-
+00000c40: 2060 3c70 726f 6d70 743e 603a 2052 6570   `<prompt>`: Rep
+00000c50: 6c61 6365 2077 6974 6820 796f 7572 2070  lace with your p
+00000c60: 726f 6d70 740a 2d20 603c 6d6f 6465 6c3e  rompt.- `<model>
+00000c70: 603a 2052 6570 6c61 6365 2077 6974 6820  `: Replace with 
+00000c80: 6569 7468 6572 2060 6770 742d 332e 352d  either `gpt-3.5-
+00000c90: 7475 7262 6f60 206f 7220 6067 7074 2d34  turbo` or `gpt-4
+00000ca0: 600a 2d20 603c 7465 6d70 6572 6174 7572  `.- `<temperatur
+00000cb0: 653e 603a 2052 6570 6c61 6365 2077 6974  e>`: Replace wit
+00000cc0: 6820 6120 666c 6f61 7420 7661 6c75 6520  h a float value 
+00000cd0: 6265 7477 6565 6e20 6030 6020 616e 6420  between `0` and 
+00000ce0: 6032 600a 2d20 602d 7660 3a20 4164 6420  `2`.- `-v`: Add 
+00000cf0: 7468 6973 2066 6c61 6720 746f 2065 6e61  this flag to ena
+00000d00: 626c 6520 7665 7262 6f73 6520 6d6f 6465  ble verbose mode
+00000d10: 0a0a 466f 7220 6578 616d 706c 653a 0a0a  ..For example:..
+00000d20: 6060 6062 6173 680a 7170 726f 6d20 2d70  ```bash.qprom -p
+00000d30: 2022 5472 616e 736c 6174 6520 7468 6520   "Translate the 
+00000d40: 666f 6c6c 6f77 696e 6720 456e 676c 6973  following Englis
+00000d50: 6820 7465 7874 2074 6f20 4672 656e 6368  h text to French
+00000d60: 3a20 277b 7465 7874 7d27 2220 2d6d 2067  : '{text}'" -m g
+00000d70: 7074 2d34 202d 7420 302e 3720 2d76 0a60  pt-4 -t 0.7 -v.`
+00000d80: 6060 0a0a 5468 6973 2077 696c 6c20 7275  ``..This will ru
+00000d90: 6e20 7468 6520 7363 7269 7074 2077 6974  n the script wit
+00000da0: 6820 7468 6520 7072 6f76 6964 6564 2070  h the provided p
+00000db0: 726f 6d70 742c 2075 7369 6e67 2074 6865  rompt, using the
+00000dc0: 2060 6770 742d 3460 206d 6f64 656c 2c20   `gpt-4` model, 
+00000dd0: 6120 7465 6d70 6572 6174 7572 6520 6f66  a temperature of
+00000de0: 2060 302e 3760 2c20 616e 6420 7665 7262   `0.7`, and verb
+00000df0: 6f73 6520 6d6f 6465 2065 6e61 626c 6564  ose mode enabled
+00000e00: 2e0a 0a23 2323 204d 756c 7469 206c 696e  ...### Multi lin
+00000e10: 6520 7072 6f6d 7074 696e 670a 546f 2066  e prompting.To f
+00000e20: 6163 696c 6974 6174 6520 6d75 6c74 692d  acilitate multi-
+00000e30: 6c69 6e65 2069 6e70 7574 2066 6f72 2074  line input for t
+00000e40: 6865 2070 726f 6d70 742c 2069 6e76 6f6b  he prompt, invok
+00000e50: 6520 7170 726f 6d20 7769 7468 6f75 7420  e qprom without 
+00000e60: 7574 696c 697a 696e 6720 7468 6520 2d70  utilizing the -p
+00000e70: 2070 6172 616d 6574 6572 2e20 5468 6973   parameter. This
+00000e80: 2077 696c 6c20 7072 6f6d 7074 2079 6f75   will prompt you
+00000e90: 2066 6f72 2079 6f75 7220 696e 7075 7420   for your input 
+00000ea0: 6174 2072 756e 7469 6d65 2c20 7768 6572  at runtime, wher
+00000eb0: 6520 796f 7520 6361 6e20 7072 6f76 6964  e you can provid
+00000ec0: 6520 6d75 6c74 6970 6c65 206c 696e 6573  e multiple lines
+00000ed0: 2061 7320 6e65 6564 6564 2e20 546f 2073   as needed. To s
+00000ee0: 6967 6e61 6c20 7468 6520 656e 6420 6f66  ignal the end of
+00000ef0: 2079 6f75 7220 696e 7075 742c 2073 696d   your input, sim
+00000f00: 706c 7920 656e 7465 7220 7468 6520 7374  ply enter the st
+00000f10: 7269 6e67 2027 454e 4427 2e0a 0a60 6060  ring 'END'...```
+00000f20: 6261 7368 0a71 7072 6f6d 0a60 6060 0a0a  bash.qprom.```..
+00000f30: 5468 6973 2077 696c 6c20 7275 6e20 7170  This will run qp
+00000f40: 726f 6d20 7769 7468 2064 6566 6175 6c74  rom with default
+00000f50: 2076 616c 7565 7320 6d6f 6465 6c3a 2060   values model: `
+00000f60: 6770 742d 3460 2c20 6120 7465 6d70 6572  gpt-4`, a temper
+00000f70: 6174 7572 6520 6f66 2060 302e 3760 2061  ature of `0.7` a
+00000f80: 6e64 2061 736b 2066 6f72 2074 6865 2070  nd ask for the p
+00000f90: 726f 6d70 7420 6475 7269 6e67 2072 756e  rompt during run
+00000fa0: 7469 6d65 2e0a 0a23 2320 546f 646f 730a  time...## Todos.
+00000fb0: 0a2a 2054 6573 7469 6e67 0a2a 2041 6464  .* Testing.* Add
+00000fc0: 2063 6f6e 7665 7273 6174 696f 6e20 6d6f   conversation mo
+00000fd0: 6465 0a2a 2041 6464 206f 7074 696f 6e20  de.* Add option 
+00000fe0: 746f 2073 656c 6563 7420 6465 6661 756c  to select defaul
+00000ff0: 7420 6d6f 6465 6c20 696e 2063 6f6e 6669  t model in confi
+00001000: 670a 2a20 4164 6420 6f70 7469 6f6e 2074  g.* Add option t
+00001010: 6f20 7365 7420 7468 6520 746f 6b65 6e20  o set the token 
+00001020: 6c69 6d69 7420 666f 7220 7468 6520 636f  limit for the co
+00001030: 6e76 6572 7361 7469 6f6e 206d 6f64 6573  nversation modes
+00001040: 2068 6973 746f 7279 0a2a 2041 6464 206f   history.* Add o
+00001050: 7074 696f 6e20 746f 2064 6973 6162 6c65  ption to disable
+00001060: 2073 7472 6561 6d69 6e67 2061 6e64 206f   streaming and o
+00001070: 6e6c 7920 7072 696e 7420 7468 6520 6675  nly print the fu
+00001080: 6c6c 2072 6573 706f 6e73 650a 0a0a 2a2a  ll response...**
+00001090: 4275 6720 7265 706f 7274 733a 2a2a 0a0a  Bug reports:**..
+000010a0: 0a23 2320 4c69 6365 6e73 650a 0a4d 4954  .## License..MIT
+000010b0: 205b 4c69 6e6b 5d28 6874 7470 733a 2f2f   [Link](https://
+000010c0: 6769 7468 7562 2e63 6f6d 2f4d 6172 7469  github.com/Marti
+000010d0: 6e57 6965 2f71 7072 6f6d 2f62 6c6f 622f  nWie/qprom/blob/
+000010e0: 6d61 7374 6572 2f4c 4943 454e 5345 290a  master/LICENSE).
+000010f0: 0a23 2320 5375 7070 6f72 7420 6d65 203a  .## Support me :
+00001100: 6865 6172 743a 203a 7374 6172 3a20 3a6d  heart: :star: :m
+00001110: 6f6e 6579 5f77 6974 685f 7769 6e67 733a  oney_with_wings:
+00001120: 0a49 6620 7468 6973 2070 726f 6a65 6374  .If this project
+00001130: 2070 726f 7669 6465 6420 7661 6c75 652c   provided value,
+00001140: 2061 6e64 2079 6f75 2077 616e 7420 746f   and you want to
+00001150: 2067 6976 6520 736f 6d65 7468 696e 6720   give something 
+00001160: 6261 636b 2c20 796f 7520 6361 6e20 6769  back, you can gi
+00001170: 7665 2074 6865 2072 6570 6f20 6120 7374  ve the repo a st
+00001180: 6172 206f 7220 7375 7070 6f72 7420 6279  ar or support by
+00001190: 2062 7579 696e 6720 6d65 2061 2063 6f66   buying me a cof
+000011a0: 6665 652e 0a0a 3c61 2068 7265 663d 2268  fee...<a href="h
+000011b0: 7474 7073 3a2f 2f62 7579 6d65 6163 6f66  ttps://buymeacof
+000011c0: 6665 652e 636f 6d2f 4d61 7274 696e 5769  fee.com/MartinWi
+000011d0: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
+000011e0: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
+000011f0: 7073 3a2f 2f63 646e 2e62 7579 6d65 6163  ps://cdn.buymeac
+00001200: 6f66 6665 652e 636f 6d2f 6275 7474 6f6e  offee.com/button
+00001210: 732f 7632 2f64 6566 6175 6c74 2d62 6c75  s/v2/default-blu
+00001220: 652e 706e 6722 2061 6c74 3d22 4275 7920  e.png" alt="Buy 
+00001230: 4d65 2041 2043 6f66 6665 6522 2077 6964  Me A Coffee" wid
+00001240: 7468 3d22 3137 3022 3e3c 2f61 3e0a       th="170"></a>.
```

### Comparing `qprom-0.5/setup.py` & `qprom-0.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md', "r", encoding='utf-8') as f:
         return f.read()
 
 
 setup(name='qprom',
-      version='0.5',
+      version='0.5.1',
       description='A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       download_url='https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz',
       entry_points={
           'console_scripts': [
               'qprom=qprom.main:main'
```

