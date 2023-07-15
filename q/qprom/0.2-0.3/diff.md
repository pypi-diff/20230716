# Comparing `tmp/qprom-0.2.tar.gz` & `tmp/qprom-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qprom-0.2.tar", last modified: Sat Jul 15 23:43:39 2023, max compression
+gzip compressed data, was "qprom-0.3.tar", last modified: Sat Jul 15 23:44:52 2023, max compression
```

## Comparing `qprom-0.2.tar` & `qprom-0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:43:39.329014 qprom-0.2/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.2/LICENSE
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     3239 2023-07-15 23:43:39.328882 qprom-0.2/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     2500 2023-07-15 23:11:02.000000 qprom-0.2/README.md
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:43:39.326746 qprom-0.2/arguments/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1434 2023-07-15 23:11:02.000000 qprom-0.2/arguments/__init__.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:43:39.327087 qprom-0.2/config/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.2/config/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1117 2023-07-15 23:11:02.000000 qprom-0.2/config/credentials.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:43:39.327430 qprom-0.2/gpt/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.2/gpt/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1219 2023-07-15 23:11:02.000000 qprom-0.2/gpt/request.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.2/gpt/util.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:43:39.327673 qprom-0.2/qprom/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.2/qprom/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      736 2023-07-15 23:41:44.000000 qprom-0.2/qprom/main.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:43:39.328670 qprom-0.2/qprom.egg-info/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     3239 2023-07-15 23:43:39.000000 qprom-0.2/qprom.egg-info/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      368 2023-07-15 23:43:39.000000 qprom-0.2/qprom.egg-info/SOURCES.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:43:39.000000 qprom-0.2/qprom.egg-info/dependency_links.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-15 23:43:39.000000 qprom-0.2/qprom.egg-info/entry_points.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.2/qprom.egg-info/not-zip-safe
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-15 23:43:39.000000 qprom-0.2/qprom.egg-info/requires.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-15 23:43:39.000000 qprom-0.2/qprom.egg-info/top_level.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-15 23:43:39.329067 qprom-0.2/setup.cfg
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1280 2023-07-15 23:40:38.000000 qprom-0.2/setup.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:44:52.071648 qprom-0.3/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.3/LICENSE
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     3258 2023-07-15 23:44:52.071551 qprom-0.3/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     2519 2023-07-15 23:44:30.000000 qprom-0.3/README.md
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:44:52.069897 qprom-0.3/arguments/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1434 2023-07-15 23:11:02.000000 qprom-0.3/arguments/__init__.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:44:52.070107 qprom-0.3/config/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.3/config/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1117 2023-07-15 23:11:02.000000 qprom-0.3/config/credentials.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:44:52.070424 qprom-0.3/gpt/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.3/gpt/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1219 2023-07-15 23:11:02.000000 qprom-0.3/gpt/request.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.3/gpt/util.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:44:52.070625 qprom-0.3/qprom/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.3/qprom/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      736 2023-07-15 23:41:44.000000 qprom-0.3/qprom/main.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:44:52.071376 qprom-0.3/qprom.egg-info/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     3258 2023-07-15 23:44:52.000000 qprom-0.3/qprom.egg-info/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      368 2023-07-15 23:44:52.000000 qprom-0.3/qprom.egg-info/SOURCES.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:44:52.000000 qprom-0.3/qprom.egg-info/dependency_links.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-15 23:44:52.000000 qprom-0.3/qprom.egg-info/entry_points.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.3/qprom.egg-info/not-zip-safe
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-15 23:44:52.000000 qprom-0.3/qprom.egg-info/requires.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-15 23:44:52.000000 qprom-0.3/qprom.egg-info/top_level.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-15 23:44:52.071689 qprom-0.3/setup.cfg
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1280 2023-07-15 23:44:30.000000 qprom-0.3/setup.py
```

### Comparing `qprom-0.2/LICENSE` & `qprom-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qprom-0.2/PKG-INFO` & `qprom-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qprom
-Version: 0.2
+Version: 0.3
 Summary: A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.
 Home-page: https://github.com/MartinWie/qprom
 Download-URL: https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz
 Author: MartinWiechmann
 Author-email: donotsuspend@googlegroups.com
 License: MIT
 Keywords: GPT-4 CLI GPT-3 OpenAI
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# qprom
+# qprom a.k.a Quick Prompt
 
 [![OS](https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [![RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)](https://github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 
 ![qprom](https://github.com/MartinWie/qprom/blob/master/qprom_logo.png)
 
 A Python-based CLI tool to quickly interact with OpenAI's GPT models instead of relying on the web interface.
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: qprom Version: 0.2 Summary: A Python-based CLI tool
+Metadata-Version: 2.1 Name: qprom Version: 0.3 Summary: A Python-based CLI tool
 to quickly interact with OpenAIs GPT models instead of relying on the web
 interface. Home-page: https://github.com/MartinWie/qprom Download-URL: https://
 github.com/MartinWie/AEnv/archive/2.0.2.tar.gz Author: MartinWiechmann Author-
 email: donotsuspend@googlegroups.com License: MIT Keywords: GPT-4 CLI GPT-
 3 OpenAI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE # qprom [![OS](https://
-img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [![RunsOn](https:
-//img.shields.io/github/license/MartinWie/AEnv)](https://github.com/MartinWie/
-AEnv/blob/master/LICENSE) [![Open Source](https://badges.frapsoft.com/os/v1/
-open-source.svg?v=103)](https://opensource.org/) ![qprom](https://github.com/
-MartinWie/qprom/blob/master/qprom_logo.png) A Python-based CLI tool to quickly
-interact with OpenAI's GPT models instead of relying on the web interface. ##
-Table of Contents 1. [Description](#description) 2. [Installation]
-(#installation) 3. [Usage](#Usage) 4. [Todos](#Todos) 5. [License](#License) ##
-Description qprom is a small project that lets you interact with OpenAI's GPT-
-4 and 3.5 chat API, quickly without having to use the web-ui. This enables
-quicker response times and better [data privacy](https://openai.com/policies/
-api-data-usage-policies) ## Installation ``` pip install qprom ``` ## Usage |
-Argument | Type | Default | Choices | Description | |---|---|---|---|---| | `-
-p` | String | None | None | Option to directly enter your prompt | | `-m` |
-String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model | | `-
-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature
-| | `-v` | Boolean | `False` | None | Enable verbose mode | ### Usage ```bash
-qprom -p  -m  -t  -v ``` - ``: Replace with your prompt - ``: Replace with
-either `gpt-3.5-turbo` or `gpt-4` - ``: Replace with a float value between `0`
-and `2` - `-v`: Add this flag to enable verbose mode For example: ```bash qprom
--p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -
-v ``` This will run the script with the provided prompt, using the `gpt-4`
-model, a temperature of `0.7`, and verbose mode enabled. ## Todos * Testing *
-Create and add logo * Update readme * Add conversation mode * Add option to
-select default model in config * Add option to disable streaming and only print
-the full response **Bug reports:** ## License MIT [Link](https://github.com/
-MartinWie/qprom/blob/master/LICENSE) ## Support me :heart: :star: :
-money_with_wings: If this project provided value, and you want to give
-something back, you can give the repo a star or support by buying me a coffee.
-[Buy_Me_A_Coffee]
+Type: text/markdown License-File: LICENSE # qprom a.k.a Quick Prompt [![OS]
+(https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [!
+[RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)](https://
+github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https://
+badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/) !
+[qprom](https://github.com/MartinWie/qprom/blob/master/qprom_logo.png) A
+Python-based CLI tool to quickly interact with OpenAI's GPT models instead of
+relying on the web interface. ## Table of Contents 1. [Description]
+(#description) 2. [Installation](#installation) 3. [Usage](#Usage) 4. [Todos]
+(#Todos) 5. [License](#License) ## Description qprom is a small project that
+lets you interact with OpenAI's GPT-4 and 3.5 chat API, quickly without having
+to use the web-ui. This enables quicker response times and better [data
+privacy](https://openai.com/policies/api-data-usage-policies) ## Installation
+``` pip install qprom ``` ## Usage | Argument | Type | Default | Choices |
+Description | |---|---|---|---|---| | `-p` | String | None | None | Option to
+directly enter your prompt | | `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-
+4` | Option to select the model | | `-t` | Float | `0.3` | Between `0` and `2`
+| Option to configure the temperature | | `-v` | Boolean | `False` | None |
+Enable verbose mode | ### Usage ```bash qprom -p  -m  -t  -v ``` - ``: Replace
+with your prompt - ``: Replace with either `gpt-3.5-turbo` or `gpt-4` - ``:
+Replace with a float value between `0` and `2` - `-v`: Add this flag to enable
+verbose mode For example: ```bash qprom -p "Translate the following English
+text to French: '{text}'" -m gpt-4 -t 0.7 -v ``` This will run the script with
+the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and
+verbose mode enabled. ## Todos * Testing * Create and add logo * Update readme
+* Add conversation mode * Add option to select default model in config * Add
+option to disable streaming and only print the full response **Bug reports:**
+## License MIT [Link](https://github.com/MartinWie/qprom/blob/master/LICENSE)
+## Support me :heart: :star: :money_with_wings: If this project provided value,
+and you want to give something back, you can give the repo a star or support by
+buying me a coffee. [Buy_Me_A_Coffee]
```

### Comparing `qprom-0.2/README.md` & `qprom-0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# qprom
+# qprom a.k.a Quick Prompt
 
 [![OS](https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [![RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)](https://github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 
 ![qprom](https://github.com/MartinWie/qprom/blob/master/qprom_logo.png)
 
 A Python-based CLI tool to quickly interact with OpenAI's GPT models instead of relying on the web interface.
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-# qprom [![OS](https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-
-green)]() [![RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)]
-(https://github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https:/
-/badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/) !
-[qprom](https://github.com/MartinWie/qprom/blob/master/qprom_logo.png) A
-Python-based CLI tool to quickly interact with OpenAI's GPT models instead of
-relying on the web interface. ## Table of Contents 1. [Description]
-(#description) 2. [Installation](#installation) 3. [Usage](#Usage) 4. [Todos]
-(#Todos) 5. [License](#License) ## Description qprom is a small project that
-lets you interact with OpenAI's GPT-4 and 3.5 chat API, quickly without having
-to use the web-ui. This enables quicker response times and better [data
-privacy](https://openai.com/policies/api-data-usage-policies) ## Installation
-``` pip install qprom ``` ## Usage | Argument | Type | Default | Choices |
-Description | |---|---|---|---|---| | `-p` | String | None | None | Option to
-directly enter your prompt | | `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-
-4` | Option to select the model | | `-t` | Float | `0.3` | Between `0` and `2`
-| Option to configure the temperature | | `-v` | Boolean | `False` | None |
-Enable verbose mode | ### Usage ```bash qprom -p  -m  -t  -v ``` - ``: Replace
-with your prompt - ``: Replace with either `gpt-3.5-turbo` or `gpt-4` - ``:
-Replace with a float value between `0` and `2` - `-v`: Add this flag to enable
-verbose mode For example: ```bash qprom -p "Translate the following English
-text to French: '{text}'" -m gpt-4 -t 0.7 -v ``` This will run the script with
-the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and
-verbose mode enabled. ## Todos * Testing * Create and add logo * Update readme
-* Add conversation mode * Add option to select default model in config * Add
-option to disable streaming and only print the full response **Bug reports:**
-## License MIT [Link](https://github.com/MartinWie/qprom/blob/master/LICENSE)
-## Support me :heart: :star: :money_with_wings: If this project provided value,
-and you want to give something back, you can give the repo a star or support by
-buying me a coffee. [Buy_Me_A_Coffee]
+# qprom a.k.a Quick Prompt [![OS](https://img.shields.io/badge/Runs%20on%3A-
+Linux%20%7C%20Mac-green)]() [![RunsOn](https://img.shields.io/github/license/
+MartinWie/AEnv)](https://github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open
+Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://
+opensource.org/) ![qprom](https://github.com/MartinWie/qprom/blob/master/
+qprom_logo.png) A Python-based CLI tool to quickly interact with OpenAI's GPT
+models instead of relying on the web interface. ## Table of Contents 1.
+[Description](#description) 2. [Installation](#installation) 3. [Usage](#Usage)
+4. [Todos](#Todos) 5. [License](#License) ## Description qprom is a small
+project that lets you interact with OpenAI's GPT-4 and 3.5 chat API, quickly
+without having to use the web-ui. This enables quicker response times and
+better [data privacy](https://openai.com/policies/api-data-usage-policies) ##
+Installation ``` pip install qprom ``` ## Usage | Argument | Type | Default |
+Choices | Description | |---|---|---|---|---| | `-p` | String | None | None |
+Option to directly enter your prompt | | `-m` | String | `gpt-4` | `gpt-3.5-
+turbo`, `gpt-4` | Option to select the model | | `-t` | Float | `0.3` | Between
+`0` and `2` | Option to configure the temperature | | `-v` | Boolean | `False`
+| None | Enable verbose mode | ### Usage ```bash qprom -p  -m  -t  -v ``` - ``:
+Replace with your prompt - ``: Replace with either `gpt-3.5-turbo` or `gpt-4` -
+``: Replace with a float value between `0` and `2` - `-v`: Add this flag to
+enable verbose mode For example: ```bash qprom -p "Translate the following
+English text to French: '{text}'" -m gpt-4 -t 0.7 -v ``` This will run the
+script with the provided prompt, using the `gpt-4` model, a temperature of
+`0.7`, and verbose mode enabled. ## Todos * Testing * Create and add logo *
+Update readme * Add conversation mode * Add option to select default model in
+config * Add option to disable streaming and only print the full response **Bug
+reports:** ## License MIT [Link](https://github.com/MartinWie/qprom/blob/
+master/LICENSE) ## Support me :heart: :star: :money_with_wings: If this project
+provided value, and you want to give something back, you can give the repo a
+star or support by buying me a coffee. [Buy_Me_A_Coffee]
```

### Comparing `qprom-0.2/arguments/__init__.py` & `qprom-0.3/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `qprom-0.2/config/credentials.py` & `qprom-0.3/config/credentials.py`

 * *Files identical despite different names*

### Comparing `qprom-0.2/gpt/request.py` & `qprom-0.3/gpt/request.py`

 * *Files identical despite different names*

### Comparing `qprom-0.2/qprom/main.py` & `qprom-0.3/qprom/main.py`

 * *Files identical despite different names*

### Comparing `qprom-0.2/qprom.egg-info/PKG-INFO` & `qprom-0.3/qprom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qprom
-Version: 0.2
+Version: 0.3
 Summary: A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.
 Home-page: https://github.com/MartinWie/qprom
 Download-URL: https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz
 Author: MartinWiechmann
 Author-email: donotsuspend@googlegroups.com
 License: MIT
 Keywords: GPT-4 CLI GPT-3 OpenAI
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# qprom
+# qprom a.k.a Quick Prompt
 
 [![OS](https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [![RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)](https://github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 
 ![qprom](https://github.com/MartinWie/qprom/blob/master/qprom_logo.png)
 
 A Python-based CLI tool to quickly interact with OpenAI's GPT models instead of relying on the web interface.
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: qprom Version: 0.2 Summary: A Python-based CLI tool
+Metadata-Version: 2.1 Name: qprom Version: 0.3 Summary: A Python-based CLI tool
 to quickly interact with OpenAIs GPT models instead of relying on the web
 interface. Home-page: https://github.com/MartinWie/qprom Download-URL: https://
 github.com/MartinWie/AEnv/archive/2.0.2.tar.gz Author: MartinWiechmann Author-
 email: donotsuspend@googlegroups.com License: MIT Keywords: GPT-4 CLI GPT-
 3 OpenAI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE # qprom [![OS](https://
-img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [![RunsOn](https:
-//img.shields.io/github/license/MartinWie/AEnv)](https://github.com/MartinWie/
-AEnv/blob/master/LICENSE) [![Open Source](https://badges.frapsoft.com/os/v1/
-open-source.svg?v=103)](https://opensource.org/) ![qprom](https://github.com/
-MartinWie/qprom/blob/master/qprom_logo.png) A Python-based CLI tool to quickly
-interact with OpenAI's GPT models instead of relying on the web interface. ##
-Table of Contents 1. [Description](#description) 2. [Installation]
-(#installation) 3. [Usage](#Usage) 4. [Todos](#Todos) 5. [License](#License) ##
-Description qprom is a small project that lets you interact with OpenAI's GPT-
-4 and 3.5 chat API, quickly without having to use the web-ui. This enables
-quicker response times and better [data privacy](https://openai.com/policies/
-api-data-usage-policies) ## Installation ``` pip install qprom ``` ## Usage |
-Argument | Type | Default | Choices | Description | |---|---|---|---|---| | `-
-p` | String | None | None | Option to directly enter your prompt | | `-m` |
-String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model | | `-
-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature
-| | `-v` | Boolean | `False` | None | Enable verbose mode | ### Usage ```bash
-qprom -p  -m  -t  -v ``` - ``: Replace with your prompt - ``: Replace with
-either `gpt-3.5-turbo` or `gpt-4` - ``: Replace with a float value between `0`
-and `2` - `-v`: Add this flag to enable verbose mode For example: ```bash qprom
--p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -
-v ``` This will run the script with the provided prompt, using the `gpt-4`
-model, a temperature of `0.7`, and verbose mode enabled. ## Todos * Testing *
-Create and add logo * Update readme * Add conversation mode * Add option to
-select default model in config * Add option to disable streaming and only print
-the full response **Bug reports:** ## License MIT [Link](https://github.com/
-MartinWie/qprom/blob/master/LICENSE) ## Support me :heart: :star: :
-money_with_wings: If this project provided value, and you want to give
-something back, you can give the repo a star or support by buying me a coffee.
-[Buy_Me_A_Coffee]
+Type: text/markdown License-File: LICENSE # qprom a.k.a Quick Prompt [![OS]
+(https://img.shields.io/badge/Runs%20on%3A-Linux%20%7C%20Mac-green)]() [!
+[RunsOn](https://img.shields.io/github/license/MartinWie/AEnv)](https://
+github.com/MartinWie/AEnv/blob/master/LICENSE) [![Open Source](https://
+badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/) !
+[qprom](https://github.com/MartinWie/qprom/blob/master/qprom_logo.png) A
+Python-based CLI tool to quickly interact with OpenAI's GPT models instead of
+relying on the web interface. ## Table of Contents 1. [Description]
+(#description) 2. [Installation](#installation) 3. [Usage](#Usage) 4. [Todos]
+(#Todos) 5. [License](#License) ## Description qprom is a small project that
+lets you interact with OpenAI's GPT-4 and 3.5 chat API, quickly without having
+to use the web-ui. This enables quicker response times and better [data
+privacy](https://openai.com/policies/api-data-usage-policies) ## Installation
+``` pip install qprom ``` ## Usage | Argument | Type | Default | Choices |
+Description | |---|---|---|---|---| | `-p` | String | None | None | Option to
+directly enter your prompt | | `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-
+4` | Option to select the model | | `-t` | Float | `0.3` | Between `0` and `2`
+| Option to configure the temperature | | `-v` | Boolean | `False` | None |
+Enable verbose mode | ### Usage ```bash qprom -p  -m  -t  -v ``` - ``: Replace
+with your prompt - ``: Replace with either `gpt-3.5-turbo` or `gpt-4` - ``:
+Replace with a float value between `0` and `2` - `-v`: Add this flag to enable
+verbose mode For example: ```bash qprom -p "Translate the following English
+text to French: '{text}'" -m gpt-4 -t 0.7 -v ``` This will run the script with
+the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and
+verbose mode enabled. ## Todos * Testing * Create and add logo * Update readme
+* Add conversation mode * Add option to select default model in config * Add
+option to disable streaming and only print the full response **Bug reports:**
+## License MIT [Link](https://github.com/MartinWie/qprom/blob/master/LICENSE)
+## Support me :heart: :star: :money_with_wings: If this project provided value,
+and you want to give something back, you can give the repo a star or support by
+buying me a coffee. [Buy_Me_A_Coffee]
```

### Comparing `qprom-0.2/setup.py` & `qprom-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md', "r", encoding='utf-8') as f:
         return f.read()
 
 
 setup(name='qprom',
-      version='0.2',
+      version='0.3',
       description='A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       download_url='https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz',
       entry_points={
           'console_scripts': [
               'qprom=qprom.main:main'
```

