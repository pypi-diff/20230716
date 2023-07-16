# Comparing `tmp/GPT4Readability-0.0.4.tar.gz` & `tmp/GPT4Readability-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPT4Readability-0.0.4.tar", last modified: Fri Jul 14 23:14:02 2023, max compression
+gzip compressed data, was "GPT4Readability-0.0.5.tar", last modified: Sun Jul 16 15:31:48 2023, max compression
```

## Comparing `GPT4Readability-0.0.4.tar` & `GPT4Readability-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.587057 GPT4Readability-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/GPT4Readability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/GPT4Readability/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/prompts/readme_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/prompts/refactor_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/readme_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/suggestions_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/GPT4Readability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:14:02.587057 GPT4Readability-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:31:48.608264 GPT4Readability-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:31:48.608264 GPT4Readability-0.0.5/GPT4Readability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/GPT4Readability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/GPT4Readability/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:31:48.608264 GPT4Readability-0.0.5/GPT4Readability/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/GPT4Readability/prompts/readme_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/GPT4Readability/prompts/refactor_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/GPT4Readability/readme_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/GPT4Readability/suggestions_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/GPT4Readability/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:31:48.608264 GPT4Readability-0.0.5/GPT4Readability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-16 15:31:48.000000 GPT4Readability-0.0.5/GPT4Readability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-16 15:31:48.000000 GPT4Readability-0.0.5/GPT4Readability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:31:48.000000 GPT4Readability-0.0.5/GPT4Readability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 15:31:48.000000 GPT4Readability-0.0.5/GPT4Readability.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-16 15:31:48.000000 GPT4Readability-0.0.5/GPT4Readability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 15:31:48.000000 GPT4Readability-0.0.5/GPT4Readability.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-16 15:31:48.608264 GPT4Readability-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:31:48.608264 GPT4Readability-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-16 15:31:36.000000 GPT4Readability-0.0.5/setup.py
```

### Comparing `GPT4Readability-0.0.4/GPT4Readability/__main__.py` & `GPT4Readability-0.0.5/GPT4Readability/__main__.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.4/GPT4Readability/prompts/readme_prompt.txt` & `GPT4Readability-0.0.5/GPT4Readability/prompts/readme_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.4/GPT4Readability/prompts/refactor_prompt.txt` & `GPT4Readability-0.0.5/GPT4Readability/prompts/refactor_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.4/GPT4Readability/readme_gen.py` & `GPT4Readability-0.0.5/GPT4Readability/readme_gen.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.4/GPT4Readability/suggestions_gen.py` & `GPT4Readability-0.0.5/GPT4Readability/suggestions_gen.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 
     # prompt_folder_name = os.path.join(os.path.dirname(__file__), "prompts")
     # prompt_path = os.path.join(prompt_folder_name, "refactor_prompt.txt")
 
     with open_text('GPT4Readability.prompts', 'refactor_prompt.txt') as f:
         inb_msg = f.read()
 
-    with open(prompt_path) as f:
-        lines = f.readlines()
-    inb_msg = "".join(lines)
 
     docs = get_docs(root_dir)
     python_files = find_python_files(root_dir)
     suggestions = []
     
     texts = split_docs(docs)
     chain = loadLLM(model)
```

### Comparing `GPT4Readability-0.0.4/GPT4Readability/utils.py` & `GPT4Readability-0.0.5/GPT4Readability/utils.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.4/GPT4Readability.egg-info/PKG-INFO` & `GPT4Readability-0.0.5/GPT4Readability.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,15 +26,15 @@
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
 > Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.  Any other changes made will be listed below:
 
 * I added the version (0.0.3) to the installation section.
-* UPDATE: Integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
+* UPDATE: README generation (suggestions coming soon!) is now integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
 
 ## Features
 
 - Automatic generation of a detailed README.md file for your Python codebase
 - Suggestions for code improvements to enhance readability and maintainability
 
 ## Installation
```

### Comparing `GPT4Readability-0.0.4/LICENSE` & `GPT4Readability-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.4/PKG-INFO` & `GPT4Readability-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,15 +26,15 @@
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
 > Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.  Any other changes made will be listed below:
 
 * I added the version (0.0.3) to the installation section.
-* UPDATE: Integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
+* UPDATE: README generation (suggestions coming soon!) is now integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
 
 ## Features
 
 - Automatic generation of a detailed README.md file for your Python codebase
 - Suggestions for code improvements to enhance readability and maintainability
 
 ## Installation
```

### Comparing `GPT4Readability-0.0.4/README.md` & `GPT4Readability-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
 > Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.  Any other changes made will be listed below:
 
 * I added the version (0.0.3) to the installation section.
-* UPDATE: Integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
+* UPDATE: README generation (suggestions coming soon!) is now integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
 
 ## Features
 
 - Automatic generation of a detailed README.md file for your Python codebase
 - Suggestions for code improvements to enhance readability and maintainability
 
 ## Installation
```

### Comparing `GPT4Readability-0.0.4/setup.py` & `GPT4Readability-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as readme:
     # ignore gifs
     description = ''.join([i for i in readme.readlines()
                            if not i.startswith('![')])
 
 setup(
     name='GPT4Readability',
-    version='0.0.4',
+    version='0.0.5',
     url='https://github.com/loevlie/GPT4Readability',
     author='Dennis Johan Loevlie',
     author_email='loevliedenny@gmail.com',
     description='A tool to automatically generate a README.md and suggest code improvements for any python code repository',
     long_description=description,
     long_description_content_type='text/markdown',
     packages=find_packages(),  # automatically discover all packages and subpackages
```

