# Comparing `tmp/qprom-0.5.1.tar.gz` & `tmp/qprom-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qprom-0.5.1.tar", last modified: Sun Jul 16 19:34:20 2023, max compression
+gzip compressed data, was "qprom-0.5.2.tar", last modified: Sun Jul 16 19:47:31 2023, max compression
```

## Comparing `qprom-0.5.1.tar` & `qprom-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.586210 qprom-0.5.1/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.5.1/LICENSE
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     4686 2023-07-16 19:34:20.586094 qprom-0.5.1/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     3945 2023-07-16 19:31:31.000000 qprom-0.5.1/README.md
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.583819 qprom-0.5.1/arguments/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1249 2023-07-16 19:12:09.000000 qprom-0.5.1/arguments/__init__.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.584017 qprom-0.5.1/config/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5.1/config/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1116 2023-07-16 19:13:45.000000 qprom-0.5.1/config/credentials.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.584440 qprom-0.5.1/gpt/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5.1/gpt/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1219 2023-07-15 23:11:02.000000 qprom-0.5.1/gpt/request.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.5.1/gpt/util.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.584859 qprom-0.5.1/qprom/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.5.1/qprom/__init__.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      759 2023-07-16 19:13:45.000000 qprom-0.5.1/qprom/main.py
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      250 2023-07-16 19:13:45.000000 qprom-0.5.1/qprom/utils.py
-drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:34:20.585907 qprom-0.5.1/qprom.egg-info/
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     4686 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/PKG-INFO
--rw-r--r--   0 martinwiechmann   (501) staff       (20)      383 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/SOURCES.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/dependency_links.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/entry_points.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.5.1/qprom.egg-info/not-zip-safe
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/requires.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-16 19:34:20.000000 qprom-0.5.1/qprom.egg-info/top_level.txt
--rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-16 19:34:20.586255 qprom-0.5.1/setup.cfg
--rw-r--r--   0 martinwiechmann   (501) staff       (20)     1282 2023-07-16 19:33:55.000000 qprom-0.5.1/setup.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:47:31.666518 qprom-0.5.2/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1066 2023-07-15 23:11:02.000000 qprom-0.5.2/LICENSE
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     4723 2023-07-16 19:47:31.666355 qprom-0.5.2/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     3982 2023-07-16 19:45:54.000000 qprom-0.5.2/README.md
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:47:31.663405 qprom-0.5.2/arguments/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1249 2023-07-16 19:12:09.000000 qprom-0.5.2/arguments/__init__.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:47:31.663724 qprom-0.5.2/config/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5.2/config/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1116 2023-07-16 19:13:45.000000 qprom-0.5.2/config/credentials.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:47:31.664262 qprom-0.5.2/gpt/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:11:02.000000 qprom-0.5.2/gpt/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     2266 2023-07-16 19:41:59.000000 qprom-0.5.2/gpt/request.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      201 2023-07-15 23:11:02.000000 qprom-0.5.2/gpt/util.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:47:31.664864 qprom-0.5.2/qprom/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        0 2023-07-15 23:34:49.000000 qprom-0.5.2/qprom/__init__.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      759 2023-07-16 19:13:45.000000 qprom-0.5.2/qprom/main.py
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      250 2023-07-16 19:13:45.000000 qprom-0.5.2/qprom/utils.py
+drwxr-xr-x   0 martinwiechmann   (501) staff       (20)        0 2023-07-16 19:47:31.666024 qprom-0.5.2/qprom.egg-info/
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     4723 2023-07-16 19:47:31.000000 qprom-0.5.2/qprom.egg-info/PKG-INFO
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)      383 2023-07-16 19:47:31.000000 qprom-0.5.2/qprom.egg-info/SOURCES.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-16 19:47:31.000000 qprom-0.5.2/qprom.egg-info/dependency_links.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       42 2023-07-16 19:47:31.000000 qprom-0.5.2/qprom.egg-info/entry_points.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)        1 2023-07-15 23:32:05.000000 qprom-0.5.2/qprom.egg-info/not-zip-safe
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       25 2023-07-16 19:47:31.000000 qprom-0.5.2/qprom.egg-info/requires.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       27 2023-07-16 19:47:31.000000 qprom-0.5.2/qprom.egg-info/top_level.txt
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)       38 2023-07-16 19:47:31.666568 qprom-0.5.2/setup.cfg
+-rw-r--r--   0 martinwiechmann   (501) staff       (20)     1282 2023-07-16 19:46:03.000000 qprom-0.5.2/setup.py
```

### Comparing `qprom-0.5.1/LICENSE` & `qprom-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qprom-0.5.1/PKG-INFO` & `qprom-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qprom
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.
 Home-page: https://github.com/MartinWie/qprom
 Download-URL: https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz
 Author: MartinWiechmann
 Author-email: donotsuspend@googlegroups.com
 License: MIT
 Keywords: GPT-4 CLI GPT-3 OpenAI
@@ -91,14 +91,15 @@
 This will run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask for the prompt during runtime.
 
 ## Todos
 
 * Testing
 * Add conversation mode
 * Add option to select default model in config
+* Add option to re-set the API token
 * Add option to set the token limit for the conversation modes history
 * Add option to disable streaming and only print the full response
 
 
 **Bug reports:**
```

### Comparing `qprom-0.5.1/README.md` & `qprom-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 This will run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask for the prompt during runtime.
 
 ## Todos
 
 * Testing
 * Add conversation mode
 * Add option to select default model in config
+* Add option to re-set the API token
 * Add option to set the token limit for the conversation modes history
 * Add option to disable streaming and only print the full response
 
 
 **Bug reports:**
```

#### html2text {}

```diff
@@ -33,13 +33,14 @@
 verbose mode enabled. ### Multi line prompting To facilitate multi-line input
 for the prompt, invoke qprom without utilizing the -p parameter. This will
 prompt you for your input at runtime, where you can provide multiple lines as
 needed. To signal the end of your input, simply enter the string 'END'. ```bash
 qprom ``` This will run qprom with default values model: `gpt-4`, a temperature
 of `0.7` and ask for the prompt during runtime. ## Todos * Testing * Add
 conversation mode * Add option to select default model in config * Add option
-to set the token limit for the conversation modes history * Add option to
-disable streaming and only print the full response **Bug reports:** ## License
-MIT [Link](https://github.com/MartinWie/qprom/blob/master/LICENSE) ## Support
-me :heart: :star: :money_with_wings: If this project provided value, and you
-want to give something back, you can give the repo a star or support by buying
-me a coffee. [Buy_Me_A_Coffee]
+to re-set the API token * Add option to set the token limit for the
+conversation modes history * Add option to disable streaming and only print the
+full response **Bug reports:** ## License MIT [Link](https://github.com/
+MartinWie/qprom/blob/master/LICENSE) ## Support me :heart: :star: :
+money_with_wings: If this project provided value, and you want to give
+something back, you can give the repo a star or support by buying me a coffee.
+[Buy_Me_A_Coffee]
```

### Comparing `qprom-0.5.1/arguments/__init__.py` & `qprom-0.5.2/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `qprom-0.5.1/config/credentials.py` & `qprom-0.5.2/config/credentials.py`

 * *Files identical despite different names*

### Comparing `qprom-0.5.1/qprom/main.py` & `qprom-0.5.2/qprom/main.py`

 * *Files identical despite different names*

### Comparing `qprom-0.5.1/qprom.egg-info/PKG-INFO` & `qprom-0.5.2/qprom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qprom
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.
 Home-page: https://github.com/MartinWie/qprom
 Download-URL: https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz
 Author: MartinWiechmann
 Author-email: donotsuspend@googlegroups.com
 License: MIT
 Keywords: GPT-4 CLI GPT-3 OpenAI
@@ -91,14 +91,15 @@
 This will run qprom with default values model: `gpt-4`, a temperature of `0.7` and ask for the prompt during runtime.
 
 ## Todos
 
 * Testing
 * Add conversation mode
 * Add option to select default model in config
+* Add option to re-set the API token
 * Add option to set the token limit for the conversation modes history
 * Add option to disable streaming and only print the full response
 
 
 **Bug reports:**
```

### Comparing `qprom-0.5.1/setup.py` & `qprom-0.5.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md', "r", encoding='utf-8') as f:
         return f.read()
 
 
 setup(name='qprom',
-      version='0.5.1',
+      version='0.5.2',
       description='A Python-based CLI tool to quickly interact with OpenAIs GPT models instead of relying on the web interface.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       download_url='https://github.com/MartinWie/AEnv/archive/2.0.2.tar.gz',
       entry_points={
           'console_scripts': [
               'qprom=qprom.main:main'
```

