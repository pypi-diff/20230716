# Comparing `tmp/qprom-0.4.tar.gz` & `tmp/qprom-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qprom-0.4.tar", last modified: Sun Jul 16 00:11:09 2023, max compression
+gzip compressed data, was "qprom-0.5.tar", last modified: Sun Jul 16 01:05:25 2023, max compression
```

## Comparing `qprom-0.4.tar` & `qprom-0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 00:11:09.689692 qprom-0.4/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.4/LICENSE
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     3256 2023-07-16 00:11:09.689587 qprom-0.4/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     2517 2023-07-16 00:10:21.000000 qprom-0.4/README.md
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 00:11:09.687479 qprom-0.4/arguments/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1434 2023-07-15 23:11:02.000000 qprom-0.4/arguments/__init__.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 00:11:09.687799 qprom-0.4/config/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.4/config/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1117 2023-07-15 23:11:02.000000 qprom-0.4/config/credentials.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 00:11:09.688205 qprom-0.4/gpt/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.4/gpt/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1219 2023-07-15 23:11:02.000000 qprom-0.4/gpt/request.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.4/gpt/util.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 00:11:09.688434 qprom-0.4/qprom/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.4/qprom/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      736 2023-07-15 23:41:44.000000 qprom-0.4/qprom/main.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 00:11:09.689418 qprom-0.4/qprom.egg-info/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     3256 2023-07-16 00:11:09.000000 qprom-0.4/qprom.egg-info/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      368 2023-07-16 00:11:09.000000 qprom-0.4/qprom.egg-info/SOURCES.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-16 00:11:09.000000 qprom-0.4/qprom.egg-info/dependency_links.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-16 00:11:09.000000 qprom-0.4/qprom.egg-info/entry_points.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.4/qprom.egg-info/not-zip-safe
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-16 00:11:09.000000 qprom-0.4/qprom.egg-info/requires.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-16 00:11:09.000000 qprom-0.4/qprom.egg-info/top_level.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-16 00:11:09.689731 qprom-0.4/setup.cfg
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1280 2023-07-16 00:09:18.000000 qprom-0.4/setup.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.029849 qprom-0.5/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.5/LICENSE
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     4160 2023-07-16 01:05:25.029742 qprom-0.5/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     3421 2023-07-16 01:02:26.000000 qprom-0.5/README.md
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028041 qprom-0.5/arguments/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1501 2023-07-16 01:02:26.000000 qprom-0.5/arguments/__init__.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028253 qprom-0.5/config/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5/config/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1117 2023-07-15 23:11:02.000000 qprom-0.5/config/credentials.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028581 qprom-0.5/gpt/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5/gpt/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1219 2023-07-15 23:11:02.000000 qprom-0.5/gpt/request.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.5/gpt/util.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.028796 qprom-0.5/qprom/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.5/qprom/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      736 2023-07-15 23:41:44.000000 qprom-0.5/qprom/main.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 01:05:25.029571 qprom-0.5/qprom.egg-info/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     4160 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      368 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/SOURCES.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/dependency_links.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/entry_points.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.5/qprom.egg-info/not-zip-safe
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/requires.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-16 01:05:25.000000 qprom-0.5/qprom.egg-info/top_level.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-16 01:05:25.029885 qprom-0.5/setup.cfg
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1280 2023-07-16 01:03:49.000000 qprom-0.5/setup.py
```

### Comparing `qprom-0.4/LICENSE` & `qprom-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qprom-0.4/PKG-INFO` & `qprom-0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qprom
-Version: 0.4
+Version: 0.5
 Summary: A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.
 Home-page: https://github.com/MartinWie/qprom
 Download-URL: https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz
 Author: MartinWiechmann
 Author-email: donotsuspend@googlegroups.com
 License: MIT
 Keywords: GPT-4 CLI GPT-3 OpenAI
@@ -44,20 +44,20 @@
 ```
 pip install qprom
 ```
 
 
 ## Usage
 
-| Argument | Type | Default | Choices | Description |
-|---|---|---|---|---|
-| `-p` | String | None | None | Option to directly enter your prompt |
-| `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model |
-| `-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature |
-| `-v` | Boolean | `False` | None | Enable verbose mode |
+| Argument | Type | Default | Choices | Description                                                                                            | Optional |
+|---|---|---|---|--------------------------------------------------------------------------------------------------------|---|
+| `-p` | String | None | None | Option to directly enter your prompt (Do not use this flag if you intend to have a multi-line prompt.) | yes |
+| `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model                                                                             | yes |
+| `-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature                                                                    | yes |
+| `-v` | Boolean | `False` | None | Enable verbose mode                                                                                    | yes |
 
 ### Usage
 
 ```bash
 qprom -p <prompt> -m <model> -t <temperature> -v
 ```
 
@@ -70,19 +70,26 @@
 
 ```bash
 qprom -p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -v
 ```
 
 This will run the script with the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and verbose mode enabled.
 
+### Multi line promting
+To facilitate multi-line input for the prompt, invoke qprom without utilizing the -p parameter. This will prompt you for your input at runtime, where you can provide multiple lines as needed. To signal the end of your input, simply enter the string 'END'.
+
+```bash
+qprom
+```
+
+This will run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask for the prompt during runtime.
+
 ## Todos
 
 * Testing
-* Create and add logo
-* Update readme
 * Add conversation mode
 * Add option to select default model in config
 * Add option to disable streaming and only print the full response
 
 
 **Bug reports:**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qprom Version: 0.4 Summary: A Python-based CLI tool
+Metadata-Version: 2.1 Name: qprom Version: 0.5 Summary: A Python-based CLI tool
 to quickly interact with OpenAIs GPT models instead of relying on the web
 interface. Home-page: https://github.com/MartinWie/qprom Download-URL: https://
 github.com/MartinWie/AEnv/archive/2.0.2.tar.gz Author: MartinWiechmann Author-
 email: donotsuspend@googlegroups.com License: MIT Keywords: GPT-4 CLI GPT-
 3 OpenAI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -17,24 +17,32 @@
 on the web interface. ## Table of Contents 1. [Description](#description) 2.
 [Installation](#installation) 3. [Usage](#Usage) 4. [Todos](#Todos) 5.
 [License](#License) ## Description qprom is a small project that lets you
 interact with OpenAI's GPT-4 and 3.5 chat API, quickly without having to use
 the web-ui. This enables quicker response times and better [data privacy]
 (https://openai.com/policies/api-data-usage-policies) ## Installation ``` pip
 install qprom ``` ## Usage | Argument | Type | Default | Choices | Description
-| |---|---|---|---|---| | `-p` | String | None | None | Option to directly
-enter your prompt | | `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` |
-Option to select the model | | `-t` | Float | `0.3` | Between `0` and `2` |
-Option to configure the temperature | | `-v` | Boolean | `False` | None |
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
+| Optional | |---|---|---|---|-------------------------------------------------
+-------------------------------------------------------|---| | `-p` | String |
+None | None | Option to directly enter your prompt (Do not use this flag if you
+intend to have a multi-line prompt.) | yes | | `-m` | String | `gpt-4` | `gpt-
+3.5-turbo`, `gpt-4` | Option to select the model | yes | | `-t` | Float | `0.3`
+| Between `0` and `2` | Option to configure the temperature | yes | | `-v` |
+Boolean | `False` | None | Enable verbose mode | yes | ### Usage ```bash qprom
+-p  -m  -t  -v ``` - ``: Replace with your prompt - ``: Replace with either
+`gpt-3.5-turbo` or `gpt-4` - ``: Replace with a float value between `0` and `2`
+- `-v`: Add this flag to enable verbose mode For example: ```bash qprom -
+p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -
+v ``` This will run the script with the provided prompt, using the `gpt-4`
+model, a temperature of `0.7`, and verbose mode enabled. ### Multi line
+promting To facilitate multi-line input for the prompt, invoke qprom without
+utilizing the -p parameter. This will prompt you for your input at runtime,
+where you can provide multiple lines as needed. To signal the end of your
+input, simply enter the string 'END'. ```bash qprom ``` This will run qprom
+with default values model: `gpt-4`, a temperature of `0.7` and ask for the
+prompt during runtime. ## Todos * Testing * Add conversation mode * Add option
+to select default model in config * Add option to disable streaming and only
+print the full response **Bug reports:** ## License MIT [Link](https://
+github.com/MartinWie/qprom/blob/master/LICENSE) ## Support me :heart: :star: :
+money_with_wings: If this project provided value, and you want to give
+something back, you can give the repo a star or support by buying me a coffee.
+[Buy_Me_A_Coffee]
```

### Comparing `qprom-0.4/README.md` & `qprom-0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 ```
 pip install qprom
 ```
 
 
 ## Usage
 
-| Argument | Type | Default | Choices | Description |
-|---|---|---|---|---|
-| `-p` | String | None | None | Option to directly enter your prompt |
-| `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model |
-| `-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature |
-| `-v` | Boolean | `False` | None | Enable verbose mode |
+| Argument | Type | Default | Choices | Description                                                                                            | Optional |
+|---|---|---|---|--------------------------------------------------------------------------------------------------------|---|
+| `-p` | String | None | None | Option to directly enter your prompt (Do not use this flag if you intend to have a multi-line prompt.) | yes |
+| `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model                                                                             | yes |
+| `-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature                                                                    | yes |
+| `-v` | Boolean | `False` | None | Enable verbose mode                                                                                    | yes |
 
 ### Usage
 
 ```bash
 qprom -p <prompt> -m <model> -t <temperature> -v
 ```
 
@@ -51,19 +51,26 @@
 
 ```bash
 qprom -p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -v
 ```
 
 This will run the script with the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and verbose mode enabled.
 
+### Multi line promting
+To facilitate multi-line input for the prompt, invoke qprom without utilizing the -p parameter. This will prompt you for your input at runtime, where you can provide multiple lines as needed. To signal the end of your input, simply enter the string 'END'.
+
+```bash
+qprom
+```
+
+This will run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask for the prompt during runtime.
+
 ## Todos
 
 * Testing
-* Create and add logo
-* Update readme
 * Add conversation mode
 * Add option to select default model in config
 * Add option to disable streaming and only print the full response
 
 
 **Bug reports:**
```

#### html2text {}

```diff
@@ -7,24 +7,32 @@
 models instead of relying on the web interface. ## Table of Contents 1.
 [Description](#description) 2. [Installation](#installation) 3. [Usage](#Usage)
 4. [Todos](#Todos) 5. [License](#License) ## Description qprom is a small
 project that lets you interact with OpenAI's GPT-4 and 3.5 chat API, quickly
 without having to use the web-ui. This enables quicker response times and
 better [data privacy](https://openai.com/policies/api-data-usage-policies) ##
 Installation ``` pip install qprom ``` ## Usage | Argument | Type | Default |
-Choices | Description | |---|---|---|---|---| | `-p` | String | None | None |
-Option to directly enter your prompt | | `-m` | String | `gpt-4` | `gpt-3.5-
-turbo`, `gpt-4` | Option to select the model | | `-t` | Float | `0.3` | Between
-`0` and `2` | Option to configure the temperature | | `-v` | Boolean | `False`
-| None | Enable verbose mode | ### Usage ```bash qprom -p  -m  -t  -v ``` - ``:
-Replace with your prompt - ``: Replace with either `gpt-3.5-turbo` or `gpt-4` -
-``: Replace with a float value between `0` and `2` - `-v`: Add this flag to
-enable verbose mode For example: ```bash qprom -p "Translate the following
-English text to French: '{text}'" -m gpt-4 -t 0.7 -v ``` This will run the
-script with the provided prompt, using the `gpt-4` model, a temperature of
-`0.7`, and verbose mode enabled. ## Todos * Testing * Create and add logo *
-Update readme * Add conversation mode * Add option to select default model in
-config * Add option to disable streaming and only print the full response **Bug
-reports:** ## License MIT [Link](https://github.com/MartinWie/qprom/blob/
-master/LICENSE) ## Support me :heart: :star: :money_with_wings: If this project
-provided value, and you want to give something back, you can give the repo a
-star or support by buying me a coffee. [Buy_Me_A_Coffee]
+Choices | Description | Optional | |---|---|---|---|---------------------------
+-----------------------------------------------------------------------------|-
+--| | `-p` | String | None | None | Option to directly enter your prompt (Do
+not use this flag if you intend to have a multi-line prompt.) | yes | | `-m` |
+String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model | yes
+| | `-t` | Float | `0.3` | Between `0` and `2` | Option to configure the
+temperature | yes | | `-v` | Boolean | `False` | None | Enable verbose mode |
+yes | ### Usage ```bash qprom -p  -m  -t  -v ``` - ``: Replace with your prompt
+- ``: Replace with either `gpt-3.5-turbo` or `gpt-4` - ``: Replace with a float
+value between `0` and `2` - `-v`: Add this flag to enable verbose mode For
+example: ```bash qprom -p "Translate the following English text to French: '
+{text}'" -m gpt-4 -t 0.7 -v ``` This will run the script with the provided
+prompt, using the `gpt-4` model, a temperature of `0.7`, and verbose mode
+enabled. ### Multi line promting To facilitate multi-line input for the prompt,
+invoke qprom without utilizing the -p parameter. This will prompt you for your
+input at runtime, where you can provide multiple lines as needed. To signal the
+end of your input, simply enter the string 'END'. ```bash qprom ``` This will
+run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask
+for the prompt during runtime. ## Todos * Testing * Add conversation mode * Add
+option to select default model in config * Add option to disable streaming and
+only print the full response **Bug reports:** ## License MIT [Link](https://
+github.com/MartinWie/qprom/blob/master/LICENSE) ## Support me :heart: :star: :
+money_with_wings: If this project provided value, and you want to give
+something back, you can give the repo a star or support by buying me a coffee.
+[Buy_Me_A_Coffee]
```

### Comparing `qprom-0.4/arguments/__init__.py` & `qprom-0.5/arguments/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def get_args():
     parser = argparse.ArgumentParser(
         prog='gptcli'
     )
 
-    parser.add_argument('-p', metavar='input', type=str, help='Option to directly enter your prompt')
+    parser.add_argument('-p', metavar='input', type=str, help='Option to directly enter your prompt.(Do not use this flag if you intend to have a multi-line prompt.)')
 
     parser.add_argument('-m', default='gpt-4', choices=['gpt-3.5-turbo', 'gpt-4'], help='Option to select the model. '
                                                                                         'Current default: GPT-4')
 
     parser.add_argument('-t', default=0.3, type=check_range, help='Option to configure the temperature:A number '
                                                                   'between 0 and 2. Current default: 0.3')
 
@@ -37,8 +37,8 @@
     print("Enter your prompt. Finish by typing 'END' on a new line:")
     lines = []
     while True:
         line = input()
         if line == 'END':
             break
         lines.append(line)
-    return '\n'.join(lines)
+    return '\n'.join(lines)
```

### Comparing `qprom-0.4/config/credentials.py` & `qprom-0.5/config/credentials.py`

 * *Files identical despite different names*

### Comparing `qprom-0.4/gpt/request.py` & `qprom-0.5/gpt/request.py`

 * *Files identical despite different names*

### Comparing `qprom-0.4/qprom/main.py` & `qprom-0.5/qprom/main.py`

 * *Files identical despite different names*

### Comparing `qprom-0.4/qprom.egg-info/PKG-INFO` & `qprom-0.5/qprom.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qprom
-Version: 0.4
+Version: 0.5
 Summary: A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.
 Home-page: https://github.com/MartinWie/qprom
 Download-URL: https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz
 Author: MartinWiechmann
 Author-email: donotsuspend@googlegroups.com
 License: MIT
 Keywords: GPT-4 CLI GPT-3 OpenAI
@@ -44,20 +44,20 @@
 ```
 pip install qprom
 ```
 
 
 ## Usage
 
-| Argument | Type | Default | Choices | Description |
-|---|---|---|---|---|
-| `-p` | String | None | None | Option to directly enter your prompt |
-| `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model |
-| `-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature |
-| `-v` | Boolean | `False` | None | Enable verbose mode |
+| Argument | Type | Default | Choices | Description                                                                                            | Optional |
+|---|---|---|---|--------------------------------------------------------------------------------------------------------|---|
+| `-p` | String | None | None | Option to directly enter your prompt (Do not use this flag if you intend to have a multi-line prompt.) | yes |
+| `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` | Option to select the model                                                                             | yes |
+| `-t` | Float | `0.3` | Between `0` and `2` | Option to configure the temperature                                                                    | yes |
+| `-v` | Boolean | `False` | None | Enable verbose mode                                                                                    | yes |
 
 ### Usage
 
 ```bash
 qprom -p <prompt> -m <model> -t <temperature> -v
 ```
 
@@ -70,19 +70,26 @@
 
 ```bash
 qprom -p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -v
 ```
 
 This will run the script with the provided prompt, using the `gpt-4` model, a temperature of `0.7`, and verbose mode enabled.
 
+### Multi line promting
+To facilitate multi-line input for the prompt, invoke qprom without utilizing the -p parameter. This will prompt you for your input at runtime, where you can provide multiple lines as needed. To signal the end of your input, simply enter the string 'END'.
+
+```bash
+qprom
+```
+
+This will run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask for the prompt during runtime.
+
 ## Todos
 
 * Testing
-* Create and add logo
-* Update readme
 * Add conversation mode
 * Add option to select default model in config
 * Add option to disable streaming and only print the full response
 
 
 **Bug reports:**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qprom Version: 0.4 Summary: A Python-based CLI tool
+Metadata-Version: 2.1 Name: qprom Version: 0.5 Summary: A Python-based CLI tool
 to quickly interact with OpenAIs GPT models instead of relying on the web
 interface. Home-page: https://github.com/MartinWie/qprom Download-URL: https://
 github.com/MartinWie/AEnv/archive/2.0.2.tar.gz Author: MartinWiechmann Author-
 email: donotsuspend@googlegroups.com License: MIT Keywords: GPT-4 CLI GPT-
 3 OpenAI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -17,24 +17,32 @@
 on the web interface. ## Table of Contents 1. [Description](#description) 2.
 [Installation](#installation) 3. [Usage](#Usage) 4. [Todos](#Todos) 5.
 [License](#License) ## Description qprom is a small project that lets you
 interact with OpenAI's GPT-4 and 3.5 chat API, quickly without having to use
 the web-ui. This enables quicker response times and better [data privacy]
 (https://openai.com/policies/api-data-usage-policies) ## Installation ``` pip
 install qprom ``` ## Usage | Argument | Type | Default | Choices | Description
-| |---|---|---|---|---| | `-p` | String | None | None | Option to directly
-enter your prompt | | `-m` | String | `gpt-4` | `gpt-3.5-turbo`, `gpt-4` |
-Option to select the model | | `-t` | Float | `0.3` | Between `0` and `2` |
-Option to configure the temperature | | `-v` | Boolean | `False` | None |
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
+| Optional | |---|---|---|---|-------------------------------------------------
+-------------------------------------------------------|---| | `-p` | String |
+None | None | Option to directly enter your prompt (Do not use this flag if you
+intend to have a multi-line prompt.) | yes | | `-m` | String | `gpt-4` | `gpt-
+3.5-turbo`, `gpt-4` | Option to select the model | yes | | `-t` | Float | `0.3`
+| Between `0` and `2` | Option to configure the temperature | yes | | `-v` |
+Boolean | `False` | None | Enable verbose mode | yes | ### Usage ```bash qprom
+-p  -m  -t  -v ``` - ``: Replace with your prompt - ``: Replace with either
+`gpt-3.5-turbo` or `gpt-4` - ``: Replace with a float value between `0` and `2`
+- `-v`: Add this flag to enable verbose mode For example: ```bash qprom -
+p "Translate the following English text to French: '{text}'" -m gpt-4 -t 0.7 -
+v ``` This will run the script with the provided prompt, using the `gpt-4`
+model, a temperature of `0.7`, and verbose mode enabled. ### Multi line
+promting To facilitate multi-line input for the prompt, invoke qprom without
+utilizing the -p parameter. This will prompt you for your input at runtime,
+where you can provide multiple lines as needed. To signal the end of your
+input, simply enter the string 'END'. ```bash qprom ``` This will run qprom
+with default values model: `gpt-4`, a temperature of `0.7` and ask for the
+prompt during runtime. ## Todos * Testing * Add conversation mode * Add option
+to select default model in config * Add option to disable streaming and only
+print the full response **Bug reports:** ## License MIT [Link](https://
+github.com/MartinWie/qprom/blob/master/LICENSE) ## Support me :heart: :star: :
+money_with_wings: If this project provided value, and you want to give
+something back, you can give the repo a star or support by buying me a coffee.
+[Buy_Me_A_Coffee]
```

### Comparing `qprom-0.4/setup.py` & `qprom-0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md', "r", encoding='utf-8') as f:
         return f.read()
 
 
 setup(name='qprom',
-      version='0.4',
+      version='0.5',
       description='A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       download_url='https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz',
       entry_points={
           'console_scripts': [
               'qprom=qprom.main:main'
```

