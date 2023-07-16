# Comparing `tmp/aider-chat-0.8.3.tar.gz` & `tmp/aider-chat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.8.3.tar", last modified: Wed Jul 12 01:48:36 2023, max compression
+gzip compressed data, was "aider-chat-0.9.0.tar", last modified: Sun Jul 16 12:47:57 2023, max compression
```

## Comparing `aider-chat-0.8.3.tar` & `aider-chat-0.9.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-12 01:48:26.000000 aider-chat-0.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 01:48:26.000000 aider-chat-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-12 01:48:36.224317 aider-chat-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-12 01:48:26.000000 aider-chat-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.220317 aider-chat-0.8.3/aider/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/aider/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34993 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/base_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/base_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/editblock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/single_wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/single_wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/coders/wholefile_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-12 01:48:26.000000 aider-chat-0.8.3/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 01:48:36.000000 aider-chat-0.8.3/aider_chat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18449 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/prompts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/rungrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-12 01:48:26.000000 aider-chat-0.8.3/benchmark/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 01:48:26.000000 aider-chat-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:48:36.224317 aider-chat-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-12 01:48:26.000000 aider-chat-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:36.224317 aider-chat-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_editblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-12 01:48:26.000000 aider-chat-0.8.3/tests/test_wholefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:57.856482 aider-chat-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 12:47:47.000000 aider-chat-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 12:47:47.000000 aider-chat-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-16 12:47:57.856482 aider-chat-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-16 12:47:47.000000 aider-chat-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:57.852482 aider-chat-0.9.0/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:57.852482 aider-chat-0.9.0/aider/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35360 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/base_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/editblock_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/editblock_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/editblock_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/editblock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/single_wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/single_wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/wholefile_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/coders/wholefile_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-16 12:47:47.000000 aider-chat-0.9.0/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:57.852482 aider-chat-0.9.0/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-16 12:47:57.000000 aider-chat-0.9.0/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-16 12:47:57.000000 aider-chat-0.9.0/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:47:57.000000 aider-chat-0.9.0/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 12:47:57.000000 aider-chat-0.9.0/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-16 12:47:57.000000 aider-chat-0.9.0/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 12:47:57.000000 aider-chat-0.9.0/aider_chat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:57.852482 aider-chat-0.9.0/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:47.000000 aider-chat-0.9.0/benchmark/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18476 2023-07-16 12:47:47.000000 aider-chat-0.9.0/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-16 12:47:47.000000 aider-chat-0.9.0/benchmark/prompts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-16 12:47:47.000000 aider-chat-0.9.0/benchmark/rungrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-16 12:47:47.000000 aider-chat-0.9.0/benchmark/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-16 12:47:47.000000 aider-chat-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:47:57.856482 aider-chat-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-16 12:47:47.000000 aider-chat-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:57.856482 aider-chat-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_editblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/test_wholefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-16 12:47:47.000000 aider-chat-0.9.0/tests/utils.py
```

### Comparing `aider-chat-0.8.3/LICENSE.txt` & `aider-chat-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/PKG-INFO` & `aider-chat-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.8.3
+Version: 0.9.0
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
-Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting.
+Aider makes it easy to
+[git commit, diff & undo changes](https://aider.chat/docs/faq.html#how-does-aider-use-git)
+proposed by GPT without copy/pasting.
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
 
 
 ## Getting started
 
 See the
 [installation instructions](https://aider.chat/docs/install.html)
 for more details, but you can
 get started quickly like this:
 
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
-$ aider app.py
+$ aider hello.js
 
 Using git repo: .git
-Added app.py to the chat.
+Added hello.js to the chat.
 
-app.py> make a flask app that replies "hello world" on /hello
+hello.js> write a js app that prints hello world
 ```
 
 ## Example chat transcripts
 
 Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4.
 
 * [**Hello World Flask App**](https://aider.chat/examples/hello-world-flask.html): Start from scratch and have GPT create a simple Flask app with various endpoints, such as adding two numbers and calculating the Fibonacci sequence.
@@ -48,17 +50,18 @@
 [high level map of the repository based on ctags](https://aider.chat/docs/ctags.html).
 
 You can find more chat transcripts on the [examples page](https://aider.chat/examples/).
 
 ## Features
 
 * Chat with GPT about your code by launching `aider` from the command line with set of source files to discuss and edit together. Aider lets GPT see and edit the content of those files.
+* GPT can write and edit code in most popular languages: python, javascript, typescript, html, css, etc.
 * Request new features, changes, improvements, or bug fixes to your code. Ask for new test cases, updated documentation or code refactors.
 * Aider will apply the edits suggested by GPT directly to your source files.
-* Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
+* Aider will [automatically commit each changeset to your local git repo](https://aider.chat/docs/faq.html#how-does-aider-use-git) with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
 
 ## Usage
 
@@ -109,27 +112,19 @@
 Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
-* Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
+* [Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding](https://aider.chat/docs/faq.html#how-does-aider-use-git).
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
 
-## Kind words from users
-
-* "The best AI coding assistant so far." -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
-* "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
-* "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
-* "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
-* "Amazing project, definitely the best AI coding assistant I've used." -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
-
 ## GPT-4 vs GPT-3.5
 
 Aider supports all of OpenAI's chat models.
 You can choose a model with the `--model` command line argument.
 
 You should probably use GPT-4 if you can. For more details see the
 [FAQ entry that compares GPT-4 vs GPT-3.5](https://aider.chat/docs/faq.html#gpt-4-vs-gpt-35).
@@ -140,7 +135,17 @@
 ## Installation
 
 See the [installation instructions](https://aider.chat/docs/install.html).
 
 ## FAQ
 
 For more information, see the [FAQ](https://aider.chat/docs/faq.html).
+
+## Kind words from users
+
+* *The best AI coding assistant so far.* -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
+* *Hands down, this is the best AI coding assistant tool so far.* -- [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
+* *Aider ... has easily quadrupled my coding productivity.* -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
+* *What an amazing tool. It's incredible.* -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
+* *Aider is such an astounding thing!* -- [cgrothaus](https://github.com/paul-gauthier/aider/issues/82#issuecomment-1631876700)
+* *It was WAY faster than I would be getting off the ground and making the first few working versions.* -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
+* *Amazing project, definitely the best AI coding assistant I've used.* -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
```

### Comparing `aider-chat-0.8.3/README.md` & `aider-chat-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
-Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting.
+Aider makes it easy to
+[git commit, diff & undo changes](https://aider.chat/docs/faq.html#how-does-aider-use-git)
+proposed by GPT without copy/pasting.
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
 ![aider screencast](assets/screencast.svg)
 
 - [Getting started](#getting-started)
 - [Example chat transcripts](#example-chat-transcripts)
 - [Features](#features)
@@ -24,20 +26,20 @@
 [installation instructions](https://aider.chat/docs/install.html)
 for more details, but you can
 get started quickly like this:
 
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
-$ aider app.py
+$ aider hello.js
 
 Using git repo: .git
-Added app.py to the chat.
+Added hello.js to the chat.
 
-app.py> make a flask app that replies "hello world" on /hello
+hello.js> write a js app that prints hello world
 ```
 
 ## Example chat transcripts
 
 Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4.
 
 * [**Hello World Flask App**](https://aider.chat/examples/hello-world-flask.html): Start from scratch and have GPT create a simple Flask app with various endpoints, such as adding two numbers and calculating the Fibonacci sequence.
@@ -50,17 +52,18 @@
 [high level map of the repository based on ctags](https://aider.chat/docs/ctags.html).
 
 You can find more chat transcripts on the [examples page](https://aider.chat/examples/).
 
 ## Features
 
 * Chat with GPT about your code by launching `aider` from the command line with set of source files to discuss and edit together. Aider lets GPT see and edit the content of those files.
+* GPT can write and edit code in most popular languages: python, javascript, typescript, html, css, etc.
 * Request new features, changes, improvements, or bug fixes to your code. Ask for new test cases, updated documentation or code refactors.
 * Aider will apply the edits suggested by GPT directly to your source files.
-* Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
+* Aider will [automatically commit each changeset to your local git repo](https://aider.chat/docs/faq.html#how-does-aider-use-git) with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
 
 ## Usage
 
@@ -111,27 +114,19 @@
 Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
-* Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
+* [Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding](https://aider.chat/docs/faq.html#how-does-aider-use-git).
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
 
-## Kind words from users
-
-* "The best AI coding assistant so far." -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
-* "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
-* "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
-* "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
-* "Amazing project, definitely the best AI coding assistant I've used." -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
-
 ## GPT-4 vs GPT-3.5
 
 Aider supports all of OpenAI's chat models.
 You can choose a model with the `--model` command line argument.
 
 You should probably use GPT-4 if you can. For more details see the
 [FAQ entry that compares GPT-4 vs GPT-3.5](https://aider.chat/docs/faq.html#gpt-4-vs-gpt-35).
@@ -142,7 +137,17 @@
 ## Installation
 
 See the [installation instructions](https://aider.chat/docs/install.html).
 
 ## FAQ
 
 For more information, see the [FAQ](https://aider.chat/docs/faq.html).
+
+## Kind words from users
+
+* *The best AI coding assistant so far.* -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
+* *Hands down, this is the best AI coding assistant tool so far.* -- [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
+* *Aider ... has easily quadrupled my coding productivity.* -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
+* *What an amazing tool. It's incredible.* -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
+* *Aider is such an astounding thing!* -- [cgrothaus](https://github.com/paul-gauthier/aider/issues/82#issuecomment-1631876700)
+* *It was WAY faster than I would be getting off the ground and making the first few working versions.* -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
+* *Amazing project, definitely the best AI coding assistant I've used.* -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
```

### Comparing `aider-chat-0.8.3/aider/coders/base_coder.py` & `aider-chat-0.9.0/aider/coders/base_coder.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,24 @@
 
     @classmethod
     def create(
         self,
         main_model,
         edit_format,
         io,
-        openai_api_key,
-        openai_api_base="https://api.openai.com/v1",
         **kwargs,
     ):
         from . import (
             EditBlockCoder,
             EditBlockFunctionCoder,
             SingleWholeFileFunctionCoder,
             WholeFileCoder,
             WholeFileFunctionCoder,
         )
 
-        openai.api_key = openai_api_key
-        openai.api_base = openai_api_base
-
         if not main_model:
             main_model = models.GPT35_16k
 
         if not main_model.always_available:
             if not check_model_availability(main_model):
                 if main_model != models.GPT4:
                     io.tool_error(
@@ -345,31 +340,37 @@
             prompt += relative_fname
             prompt += f"\n{self.fence[0]}\n"
             prompt += content
             prompt += f"{self.fence[1]}\n"
 
         return prompt
 
+    def get_repo_map(self):
+        if not self.repo_map:
+            return
+
+        other_files = set(self.get_all_abs_files()) - set(self.abs_fnames)
+        repo_content = self.repo_map.get_repo_map(self.abs_fnames, other_files)
+        return repo_content
+
     def get_files_messages(self):
         all_content = ""
         if self.abs_fnames:
             files_content = self.gpt_prompts.files_content_prefix
             files_content += self.get_files_content()
         else:
             files_content = self.gpt_prompts.files_no_full_files
 
         all_content += files_content
 
-        other_files = set(self.get_all_abs_files()) - set(self.abs_fnames)
-        if self.repo_map:
-            repo_content = self.repo_map.get_repo_map(self.abs_fnames, other_files)
-            if repo_content:
-                if all_content:
-                    all_content += "\n"
-                all_content += repo_content
+        repo_content = self.get_repo_map()
+        if repo_content:
+            if all_content:
+                all_content += "\n"
+            all_content += repo_content
 
         files_messages = [
             dict(role="user", content=all_content),
             dict(role="assistant", content="Ok."),
         ]
         if self.abs_fnames:
             files_messages += [
@@ -561,15 +562,15 @@
 
             saved_message = self.gpt_prompts.files_content_gpt_edits.format(
                 hash=commit_hash,
                 message=commit_message,
             )
         else:
             if self.repo:
-                self.io.tool_error("Warning: no changes found in tracked files.")
+                self.io.tool_output("No changes made to git tracked files.")
             saved_message = self.gpt_prompts.files_content_gpt_no_edits
 
         return saved_message
 
     def check_for_file_mentions(self, content):
         words = set(word for word in content.split())
 
@@ -581,14 +582,17 @@
         words = set(word.strip(quotes) for word in words)
 
         addable_rel_fnames = self.get_addable_relative_files()
 
         mentioned_rel_fnames = set()
         fname_to_rel_fnames = {}
         for rel_fname in addable_rel_fnames:
+            if rel_fname in words:
+                mentioned_rel_fnames.add(str(rel_fname))
+
             fname = os.path.basename(rel_fname)
             if fname not in fname_to_rel_fnames:
                 fname_to_rel_fnames[fname] = []
             fname_to_rel_fnames[fname].append(rel_fname)
 
         for fname, rel_fnames in fname_to_rel_fnames.items():
             if len(rel_fnames) == 1 and fname in words:
@@ -614,26 +618,34 @@
             Timeout,
             APIError,
             ServiceUnavailableError,
             RateLimitError,
             requests.exceptions.ConnectionError,
         ),
         max_tries=10,
-        on_backoff=lambda details: print(f"Retry in {details['wait']} seconds."),
+        on_backoff=lambda details: print(
+            f"{details.get('exception','Exception')}\nRetry in {details['wait']:.1f} seconds."
+        ),
     )
     def send_with_retries(self, model, messages, functions):
         kwargs = dict(
             model=model,
             messages=messages,
             temperature=0,
             stream=self.stream,
         )
         if functions is not None:
             kwargs["functions"] = self.functions
 
+        # we are abusing the openai object to stash these values
+        if hasattr(openai, "api_deployment_id"):
+            kwargs["deployment_id"] = openai.api_deployment_id
+        if hasattr(openai, "api_engine"):
+            kwargs["engine"] = openai.api_engine
+
         # Generate SHA1 hash of kwargs and append it to chat_completion_call_hashes
         hash_object = hashlib.sha1(json.dumps(kwargs, sort_keys=True).encode())
         self.chat_completion_call_hashes.append(hash_object.hexdigest())
 
         res = openai.ChatCompletion.create(**kwargs)
         return res
```

### Comparing `aider-chat-0.8.3/aider/coders/editblock_coder.py` & `aider-chat-0.9.0/aider/coders/editblock_coder.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,46 +181,49 @@
 
     if whole.endswith("\n"):
         modified_whole += "\n"
 
     return modified_whole
 
 
-def strip_quoted_wrapping(res, fname=None):
+def strip_quoted_wrapping(res, fname=None, fence=None):
     """
     Given an input string which may have extra "wrapping" around it, remove the wrapping.
     For example:
 
     filename.ext
     ```
     We just want this content
     Not the filename and triple quotes
     ```
     """
     if not res:
         return res
 
+    if not fence:
+        fence = ("```", "```")
+
     res = res.splitlines()
 
     if fname and res[0].strip().endswith(Path(fname).name):
         res = res[1:]
 
-    if res[0].startswith("```") and res[-1].startswith("```"):
+    if res[0].startswith(fence[0]) and res[-1].startswith(fence[1]):
         res = res[1:-1]
 
     res = "\n".join(res)
     if res and res[-1] != "\n":
         res += "\n"
 
     return res
 
 
-def do_replace(fname, content, before_text, after_text):
-    before_text = strip_quoted_wrapping(before_text, fname)
-    after_text = strip_quoted_wrapping(after_text, fname)
+def do_replace(fname, content, before_text, after_text, fence=None):
+    before_text = strip_quoted_wrapping(before_text, fname, fence)
+    after_text = strip_quoted_wrapping(after_text, fname, fence)
     fname = Path(fname)
 
     # does it want to make a new file?
     if not fname.exists() and not before_text.strip():
         fname.touch()
         content = ""
```

### Comparing `aider-chat-0.8.3/aider/coders/editblock_func_coder.py` & `aider-chat-0.9.0/aider/coders/editblock_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/coders/editblock_func_prompts.py` & `aider-chat-0.9.0/aider/coders/editblock_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/coders/editblock_prompts.py` & `aider-chat-0.9.0/aider/coders/editblock_prompts.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 1. List the files you need to modify. *NEVER* suggest changes to *read-only* files. You *MUST* ask the user to make them *read-write* using the file's full path name. End your reply and wait for their approval.
 2. Think step-by-step and explain the needed changes.
 3. Describe each change with an *edit block* per the example below.
 """
 
     system_reminder = """You MUST format EVERY code change with an *edit block* like this:
 
-```python
+{fence[0]}python
 some/dir/example.py
 <<<<<<< ORIGINAL
     # some comment
     # Func to multiply
     def mul(a,b)
 =======
     # updated comment
     # Function to add
     def add(a,b):
 >>>>>>> UPDATED
-```
+{fence[1]}
 
-Every *edit block* must be fenced w/triple backticks with the correct code language.
+Every *edit block* must be fenced with {fence[0]}...{fence[1]} with the correct code language.
 Every *edit block* must start with the full path! *NEVER* propose edit blocks for *read-only* files.
 The ORIGINAL section must be an *exact* set of lines from the file:
 - NEVER SKIP LINES!
 - Include all original leading spaces and indentation!
 
 Edits to different parts of a file each need their own *edit block*.
```

### Comparing `aider-chat-0.8.3/aider/coders/single_wholefile_func_coder.py` & `aider-chat-0.9.0/aider/coders/single_wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/coders/single_wholefile_func_prompts.py` & `aider-chat-0.9.0/aider/coders/single_wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/coders/wholefile_coder.py` & `aider-chat-0.9.0/aider/coders/wholefile_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/coders/wholefile_func_coder.py` & `aider-chat-0.9.0/aider/coders/wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/coders/wholefile_func_prompts.py` & `aider-chat-0.9.0/aider/coders/wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/coders/wholefile_prompts.py` & `aider-chat-0.9.0/aider/coders/wholefile_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/commands.py` & `aider-chat-0.9.0/aider/commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/diffs.py` & `aider-chat-0.9.0/aider/diffs.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/dump.py` & `aider-chat-0.9.0/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/io.py` & `aider-chat-0.9.0/aider/io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/main.py` & `aider-chat-0.9.0/aider/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 from pathlib import Path
 
 import configargparse
 import git
+import openai
 
 from aider import __version__, models
 from aider.coders import Coder
 from aider.io import InputOutput
 
 
 def get_git_root():
@@ -71,16 +72,35 @@
     )
 
     ##########
     model_group = parser.add_argument_group("Advanced Model Settings")
     model_group.add_argument(
         "--openai-api-base",
         metavar="OPENAI_API_BASE",
-        default="https://api.openai.com/v1",
-        help="Specify the OpenAI API base endpoint (default: https://api.openai.com/v1)",
+        help="Specify the openai.api_base (default: https://api.openai.com/v1)",
+    )
+    model_group.add_argument(
+        "--openai-api-type",
+        metavar="OPENAI_API_TYPE",
+        help="Specify the openai.api_type",
+    )
+    model_group.add_argument(
+        "--openai-api-version",
+        metavar="OPENAI_API_VERSION",
+        help="Specify the openai.api_version",
+    )
+    model_group.add_argument(
+        "--openai-api-deployment-id",
+        metavar="OPENAI_API_DEPLOYMENT_ID",
+        help="Specify the deployment_id arg to be passed to openai.ChatCompletion.create()",
+    )
+    model_group.add_argument(
+        "--openai-api-engine",
+        metavar="OPENAI_API_ENGINE",
+        help="Specify the engine arg to be passed to openai.ChatCompletion.create()",
     )
     model_group.add_argument(
         "--edit-format",
         metavar="EDIT_FORMAT",
         default=None,
         help="Specify what edit format GPT should use (default depends on model)",
     )
@@ -245,14 +265,20 @@
         "-v",
         "--verbose",
         action="store_true",
         help="Enable verbose output",
         default=False,
     )
     other_group.add_argument(
+        "--show-repo-map",
+        action="store_true",
+        help="Print the repo map and exit (debug)",
+        default=False,
+    )
+    other_group.add_argument(
         "--message",
         "--msg",
         "-m",
         metavar="COMMAND",
         help="Specify a single message to send GPT, process reply then exit (disables chat mode)",
     )
     other_group.add_argument(
@@ -308,20 +334,24 @@
                 if not global_git_config.has_option("user", "email"):
                     git_config.set_value("user", "email", "you@example.com")
                     io.tool_error(
                         'Update git email with: git config --global user.email "you@example.com"'
                     )
             io.tool_output("Git repository created in the current working directory.")
 
+    def scrub_sensitive_info(text):
+        # Replace sensitive information with placeholder
+        return text.replace(args.openai_api_key, '***')
+
     if args.verbose:
-        show = parser.format_values()
+        show = scrub_sensitive_info(parser.format_values())
         io.tool_output(show)
         io.tool_output("Option settings:")
         for arg, val in sorted(vars(args).items()):
-            io.tool_output(f"  - {arg}: {val}")
+            io.tool_output(f"  - {arg}: {scrub_sensitive_info(str(val))}")
 
     io.tool_output(*sys.argv, log_only=True)
 
     if not args.openai_api_key:
         if os.name == "nt":
             io.tool_error(
                 "No OpenAI API key provided. Use --openai-api-key or setx OPENAI_API_KEY."
@@ -330,20 +360,27 @@
             io.tool_error(
                 "No OpenAI API key provided. Use --openai-api-key or export OPENAI_API_KEY."
             )
         return 1
 
     main_model = models.Model(args.model)
 
+    openai.api_key = args.openai_api_key
+    for attr in ("base", "type", "version", "deployment_id", "engine"):
+        arg_key = f"openai_api_{attr}"
+        val = getattr(args, arg_key)
+        if val is not None:
+            mod_key = f"api_{attr}"
+            setattr(openai, mod_key, val)
+            io.tool_output(f"Setting openai.{mod_key}={val}")
+
     coder = Coder.create(
         main_model,
         args.edit_format,
         io,
-        args.openai_api_key,
-        args.openai_api_base,
         ##
         fnames=args.files,
         pretty=args.pretty,
         show_diffs=args.show_diffs,
         auto_commits=args.auto_commits,
         dirty_commits=args.dirty_commits,
         dry_run=args.dry_run,
@@ -351,14 +388,20 @@
         verbose=args.verbose,
         assistant_output_color=args.assistant_output_color,
         code_theme=args.code_theme,
         stream=args.stream,
         use_git=args.git,
     )
 
+    if args.show_repo_map:
+        repo_map = coder.get_repo_map()
+        if repo_map:
+            io.tool_output(repo_map)
+        return
+
     if args.dirty_commits:
         coder.commit(ask=True, which="repo_files")
 
     if args.apply:
         content = io.read_text(args.apply)
         if content is None:
             return
```

### Comparing `aider-chat-0.8.3/aider/models.py` & `aider-chat-0.9.0/aider/models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/prompts.py` & `aider-chat-0.9.0/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider/repomap.py` & `aider-chat-0.9.0/aider/repomap.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 import random
 import subprocess
 import sys
 import tempfile
 from collections import Counter, defaultdict
+from pathlib import Path
 
 import networkx as nx
 import tiktoken
 from diskcache import Cache
 from pygments.lexers import guess_lexer_for_filename
 from pygments.token import Token
 from pygments.util import ClassNotFound
@@ -227,21 +228,21 @@
         except Exception as err:
             self.ctags_disabled_reason = f"error running universal-ctags: {err}"
             return
 
         return True
 
     def load_tags_cache(self):
-        self.TAGS_CACHE = Cache(self.TAGS_CACHE_DIR)
+        self.TAGS_CACHE = Cache(Path(self.root) / self.TAGS_CACHE_DIR)
 
     def save_tags_cache(self):
         pass
 
     def load_ident_cache(self):
-        self.IDENT_CACHE = Cache(self.IDENT_CACHE_DIR)
+        self.IDENT_CACHE = Cache(Path(self.root) / self.IDENT_CACHE_DIR)
 
     def save_ident_cache(self):
         pass
 
     def get_mtime(self, fname):
         try:
             return os.path.getmtime(fname)
```

### Comparing `aider-chat-0.8.3/aider/utils.py` & `aider-chat-0.9.0/aider/utils.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.9.0/aider_chat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.8.3
+Version: 0.9.0
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
-Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting.
+Aider makes it easy to
+[git commit, diff & undo changes](https://aider.chat/docs/faq.html#how-does-aider-use-git)
+proposed by GPT without copy/pasting.
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
 
 
 ## Getting started
 
 See the
 [installation instructions](https://aider.chat/docs/install.html)
 for more details, but you can
 get started quickly like this:
 
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
-$ aider app.py
+$ aider hello.js
 
 Using git repo: .git
-Added app.py to the chat.
+Added hello.js to the chat.
 
-app.py> make a flask app that replies "hello world" on /hello
+hello.js> write a js app that prints hello world
 ```
 
 ## Example chat transcripts
 
 Here are some example transcripts that show how you can chat with `aider` to write and edit code with GPT-4.
 
 * [**Hello World Flask App**](https://aider.chat/examples/hello-world-flask.html): Start from scratch and have GPT create a simple Flask app with various endpoints, such as adding two numbers and calculating the Fibonacci sequence.
@@ -48,17 +50,18 @@
 [high level map of the repository based on ctags](https://aider.chat/docs/ctags.html).
 
 You can find more chat transcripts on the [examples page](https://aider.chat/examples/).
 
 ## Features
 
 * Chat with GPT about your code by launching `aider` from the command line with set of source files to discuss and edit together. Aider lets GPT see and edit the content of those files.
+* GPT can write and edit code in most popular languages: python, javascript, typescript, html, css, etc.
 * Request new features, changes, improvements, or bug fixes to your code. Ask for new test cases, updated documentation or code refactors.
 * Aider will apply the edits suggested by GPT directly to your source files.
-* Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
+* Aider will [automatically commit each changeset to your local git repo](https://aider.chat/docs/faq.html#how-does-aider-use-git) with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
 
 ## Usage
 
@@ -109,27 +112,19 @@
 Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
-* Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
+* [Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding](https://aider.chat/docs/faq.html#how-does-aider-use-git).
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
 
-## Kind words from users
-
-* "The best AI coding assistant so far." -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
-* "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
-* "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
-* "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
-* "Amazing project, definitely the best AI coding assistant I've used." -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
-
 ## GPT-4 vs GPT-3.5
 
 Aider supports all of OpenAI's chat models.
 You can choose a model with the `--model` command line argument.
 
 You should probably use GPT-4 if you can. For more details see the
 [FAQ entry that compares GPT-4 vs GPT-3.5](https://aider.chat/docs/faq.html#gpt-4-vs-gpt-35).
@@ -140,7 +135,17 @@
 ## Installation
 
 See the [installation instructions](https://aider.chat/docs/install.html).
 
 ## FAQ
 
 For more information, see the [FAQ](https://aider.chat/docs/faq.html).
+
+## Kind words from users
+
+* *The best AI coding assistant so far.* -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
+* *Hands down, this is the best AI coding assistant tool so far.* -- [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
+* *Aider ... has easily quadrupled my coding productivity.* -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
+* *What an amazing tool. It's incredible.* -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
+* *Aider is such an astounding thing!* -- [cgrothaus](https://github.com/paul-gauthier/aider/issues/82#issuecomment-1631876700)
+* *It was WAY faster than I would be getting off the ground and making the first few working versions.* -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
+* *Amazing project, definitely the best AI coding assistant I've used.* -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
```

### Comparing `aider-chat-0.8.3/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.9.0/aider_chat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,9 @@
 tests/test_coder.py
 tests/test_commands.py
 tests/test_editblock.py
 tests/test_io.py
 tests/test_main.py
 tests/test_models.py
 tests/test_repomap.py
-tests/test_wholefile.py
+tests/test_wholefile.py
+tests/utils.py
```

### Comparing `aider-chat-0.8.3/aider_chat.egg-info/requires.txt` & `aider-chat-0.9.0/aider_chat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/benchmark/benchmark.py` & `aider-chat-0.9.0/benchmark/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from types import SimpleNamespace
 from typing import List
 
 import git
 import lox
 import matplotlib.pyplot as plt
 import numpy as np
+import openai
 import pandas as pd
 import prompts
 import typer
 from imgcat import imgcat
 from rich.console import Console
 
 from aider import models
@@ -503,19 +504,20 @@
     edit_format = edit_format or main_model.edit_format
 
     dump(main_model)
     dump(edit_format)
     show_fnames = ",".join(map(str, fnames))
     print("fnames:", show_fnames)
 
+    openai.api_key = os.environ["OPENAI_API_KEY"]
+
     coder = Coder.create(
         main_model,
         edit_format,
         io,
-        os.environ["OPENAI_API_KEY"],
         fnames=fnames,
         use_git=False,
         stream=False,
         pretty=False,
         verbose=verbose,
     )
```

### Comparing `aider-chat-0.8.3/benchmark/rungrid.py` & `aider-chat-0.9.0/benchmark/rungrid.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/benchmark/test_benchmark.py` & `aider-chat-0.9.0/benchmark/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/requirements.txt` & `aider-chat-0.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/setup.py` & `aider-chat-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/tests/test_coder.py` & `aider-chat-0.9.0/tests/test_coder.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import openai
 import requests
 
 from aider import models
 from aider.coders import Coder
 from aider.dump import dump  # noqa: F401
 from aider.io import InputOutput
+from tests.utils import GitTemporaryDirectory
 
 
 class TestCoder(unittest.TestCase):
     def setUp(self):
         self.patcher = patch("aider.coders.base_coder.check_model_availability")
         self.mock_check = self.patcher.start()
         self.mock_check.return_value = True
@@ -24,15 +25,15 @@
         self.patcher.stop()
 
     def test_check_for_file_mentions(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         # Mock the git repo
         mock = MagicMock()
         mock.return_value = set(["file1.txt", "file2.py"])
         coder.get_tracked_files = mock
 
         # Call the check_for_file_mentions method
@@ -58,28 +59,26 @@
 
         file1.touch()
         file2.touch()
 
         files = [file1, file2]
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(
-            models.GPT4, None, io=InputOutput(), openai_api_key="fake_key", fnames=files
-        )
+        coder = Coder.create(models.GPT4, None, io=InputOutput(), fnames=files)
 
         content = coder.get_files_content().splitlines()
         self.assertIn("file1.txt", content)
         self.assertIn("file2.txt", content)
 
     def test_check_for_filename_mentions_of_longer_paths(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         mock = MagicMock()
         mock.return_value = set(["file1.txt", "file2.py"])
         coder.get_tracked_files = mock
 
         # Call the check_for_file_mentions method
         coder.check_for_file_mentions("Please check file1.txt and file2.py")
@@ -93,35 +92,59 @@
                     Path(coder.root) / "file2.py",
                 ],
             )
         )
         self.assertEqual(coder.abs_fnames, expected_files)
 
     def test_check_for_ambiguous_filename_mentions_of_longer_paths(self):
-        # Mock the IO object
-        mock_io = MagicMock()
+        with GitTemporaryDirectory():
+            io = InputOutput(pretty=False, yes=True)
+            coder = Coder.create(models.GPT4, None, io)
 
-        # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+            fname = Path("file1.txt")
+            fname.touch()
 
-        mock = MagicMock()
-        mock.return_value = set(["file1.txt", "other/file1.txt"])
-        coder.get_tracked_files = mock
+            other_fname = Path("other") / "file1.txt"
+            other_fname.parent.mkdir(parents=True, exist_ok=True)
+            other_fname.touch()
 
-        # Call the check_for_file_mentions method
-        coder.check_for_file_mentions("Please check file1.txt!")
+            mock = MagicMock()
+            mock.return_value = set([str(fname), str(other_fname)])
+            coder.get_tracked_files = mock
+
+            # Call the check_for_file_mentions method
+            coder.check_for_file_mentions(f"Please check {fname}!")
+
+            self.assertEqual(coder.abs_fnames, set([str(fname.resolve())]))
 
-        self.assertEqual(coder.abs_fnames, set())
+    def test_check_for_subdir_mention(self):
+        with GitTemporaryDirectory():
+            io = InputOutput(pretty=False, yes=True)
+            coder = Coder.create(models.GPT4, None, io)
+
+            fname = Path("other") / "file1.txt"
+            fname.parent.mkdir(parents=True, exist_ok=True)
+            fname.touch()
+
+            mock = MagicMock()
+            mock.return_value = set([str(fname)])
+            coder.get_tracked_files = mock
+
+            dump(fname)
+            # Call the check_for_file_mentions method
+            coder.check_for_file_mentions(f"Please check `{fname}`")
+
+            self.assertEqual(coder.abs_fnames, set([str(fname.resolve())]))
 
     def test_get_commit_message(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         # Mock the send method to set partial_response_content and return False
         def mock_send(*args, **kwargs):
             coder.partial_response_content = "a good commit message"
             return False
 
         coder.send = MagicMock(side_effect=mock_send)
@@ -133,15 +156,15 @@
         self.assertEqual(result, "a good commit message")
 
     def test_get_commit_message_strip_quotes(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         # Mock the send method to set partial_response_content and return False
         def mock_send(*args, **kwargs):
             coder.partial_response_content = "a good commit message"
             return False
 
         coder.send = MagicMock(side_effect=mock_send)
@@ -153,15 +176,15 @@
         self.assertEqual(result, "a good commit message")
 
     def test_get_commit_message_no_strip_unmatched_quotes(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         # Mock the send method to set partial_response_content and return False
         def mock_send(*args, **kwargs):
             coder.partial_response_content = 'a good "commit message"'
             return False
 
         coder.send = MagicMock(side_effect=mock_send)
@@ -175,15 +198,15 @@
     @patch("aider.coders.base_coder.openai.ChatCompletion.create")
     @patch("builtins.print")
     def test_send_with_retries_rate_limit_error(self, mock_print, mock_chat_completion_create):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         # Set up the mock to raise RateLimitError on
         # the first call and return None on the second call
         mock_chat_completion_create.side_effect = [
             openai.error.RateLimitError("Rate limit exceeded"),
             None,
         ]
@@ -197,15 +220,15 @@
     @patch("aider.coders.base_coder.openai.ChatCompletion.create")
     @patch("builtins.print")
     def test_send_with_retries_connection_error(self, mock_print, mock_chat_completion_create):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         # Set up the mock to raise ConnectionError on the first call
         # and return None on the second call
         mock_chat_completion_create.side_effect = [
             requests.exceptions.ConnectionError("Connection error"),
             None,
         ]
@@ -226,17 +249,15 @@
 
         file1.touch()
         file2.touch()
 
         files = [file1, file2]
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(
-            models.GPT4, None, io=InputOutput(), openai_api_key="fake_key", fnames=files
-        )
+        coder = Coder.create(models.GPT4, None, io=InputOutput(), fnames=files)
 
         def mock_send(*args, **kwargs):
             coder.partial_response_content = "ok"
             coder.partial_response_function_call = dict()
 
         coder.send = MagicMock(side_effect=mock_send)
 
@@ -254,17 +275,15 @@
         # Create a few temporary files
         _, file1 = tempfile.mkstemp()
         _, file2 = tempfile.mkstemp()
 
         files = [file1, file2]
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(
-            models.GPT4, None, io=InputOutput(), openai_api_key="fake_key", fnames=files
-        )
+        coder = Coder.create(models.GPT4, None, io=InputOutput(), fnames=files)
 
         def mock_send(*args, **kwargs):
             coder.partial_response_content = "ok"
             coder.partial_response_function_call = dict()
 
         coder.send = MagicMock(side_effect=mock_send)
 
@@ -286,17 +305,15 @@
 
         with open(file1, "wb") as f:
             f.write(b"this contains ``` backticks")
 
         files = [file1]
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(
-            models.GPT4, None, io=InputOutput(), openai_api_key="fake_key", fnames=files
-        )
+        coder = Coder.create(models.GPT4, None, io=InputOutput(), fnames=files)
 
         def mock_send(*args, **kwargs):
             coder.partial_response_content = "ok"
             coder.partial_response_function_call = dict()
 
         coder.send = MagicMock(side_effect=mock_send)
 
@@ -316,15 +333,14 @@
         encoding = "utf-16"
 
         # Initialize the Coder object with the mocked IO and mocked repo
         coder = Coder.create(
             models.GPT4,
             None,
             io=InputOutput(encoding=encoding),
-            openai_api_key="fake_key",
             fnames=files,
         )
 
         def mock_send(*args, **kwargs):
             coder.partial_response_content = "ok"
             coder.partial_response_function_call = dict()
 
@@ -345,15 +361,15 @@
 
     @patch("aider.coders.base_coder.openai.ChatCompletion.create")
     def test_run_with_invalid_request_error(self, mock_chat_completion_create):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io)
 
         # Set up the mock to raise InvalidRequestError
         mock_chat_completion_create.side_effect = openai.error.InvalidRequestError(
             "Invalid request", "param"
         )
 
         # Call the run method and assert that InvalidRequestError is raised
@@ -389,15 +405,14 @@
         repo.git.commit("-m", "added")
 
         # Create a Coder object on the temporary directory
         coder = Coder.create(
             models.GPT4,
             None,
             io=InputOutput(),
-            openai_api_key="fake_key",
             fnames=[str(tempdir / filenames[0])],
         )
 
         tracked_files = coder.get_tracked_files()
 
         # On windows, paths will come back \like\this, so normalize them back to Paths
         tracked_files = [Path(fn) for fn in tracked_files]
```

### Comparing `aider-chat-0.8.3/tests/test_commands.py` & `aider-chat-0.9.0/tests/test_commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,30 +25,30 @@
         shutil.rmtree(self.tempdir)
 
     def test_cmd_add(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
         from aider.coders import Coder
 
-        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io)
         commands = Commands(io, coder)
 
         # Call the cmd_add method with 'foo.txt' and 'bar.txt' as a single string
         commands.cmd_add("foo.txt bar.txt")
 
         # Check if both files have been created in the temporary directory
         self.assertTrue(os.path.exists("foo.txt"))
         self.assertTrue(os.path.exists("bar.txt"))
 
     def test_cmd_add_with_glob_patterns(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
         from aider.coders import Coder
 
-        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io)
         commands = Commands(io, coder)
 
         # Create some test files
         with open("test1.py", "w") as f:
             f.write("print('test1')")
         with open("test2.py", "w") as f:
             f.write("print('test2')")
@@ -66,29 +66,29 @@
         self.assertNotIn(str(Path("test.txt").resolve()), coder.abs_fnames)
 
     def test_cmd_add_no_match(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
         from aider.coders import Coder
 
-        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io)
         commands = Commands(io, coder)
 
         # Call the cmd_add method with a non-existent file pattern
         commands.cmd_add("*.nonexistent")
 
         # Check if no files have been added to the chat session
         self.assertEqual(len(coder.abs_fnames), 0)
 
     def test_cmd_add_drop_directory(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
         from aider.coders import Coder
 
-        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io)
         commands = Commands(io, coder)
 
         # Create a directory and add files to it
         os.mkdir("test_dir")
         os.mkdir("test_dir/another_dir")
         with open("test_dir/test_file1.txt", "w") as f:
             f.write("Test file 1")
@@ -113,15 +113,15 @@
         )
 
     def test_cmd_drop_with_glob_patterns(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
         from aider.coders import Coder
 
-        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io)
         commands = Commands(io, coder)
 
         subdir = Path("subdir")
         subdir.mkdir()
         (subdir / "subtest1.py").touch()
         (subdir / "subtest2.py").touch()
 
@@ -140,30 +140,30 @@
         self.assertNotIn(str(Path("test2.py").resolve()), coder.abs_fnames)
 
     def test_cmd_add_bad_encoding(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
         from aider.coders import Coder
 
-        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io)
         commands = Commands(io, coder)
 
         # Create a new file foo.bad which will fail to decode as utf-8
         with codecs.open("foo.bad", "w", encoding="iso-8859-15") as f:
             f.write("ÆØÅ")  # Characters not present in utf-8
 
         commands.cmd_add("foo.bad")
 
         self.assertEqual(coder.abs_fnames, set())
 
     def test_cmd_tokens(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
 
-        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io)
         commands = Commands(io, coder)
 
         commands.cmd_add("foo.txt bar.txt")
 
         # Redirect the standard output to an instance of io.StringIO
         stdout = StringIO()
         sys.stdout = stdout
```

### Comparing `aider-chat-0.8.3/tests/test_editblock.py` & `aider-chat-0.9.0/tests/test_editblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,17 +244,15 @@
 
         with open(file1, "w", encoding="utf-8") as f:
             f.write("one\ntwo\nthree\n")
 
         files = [file1]
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(
-            models.GPT4, "diff", io=InputOutput(), openai_api_key="fake_key", fnames=files
-        )
+        coder = Coder.create(models.GPT4, "diff", io=InputOutput(), fnames=files)
 
         def mock_send(*args, **kwargs):
             coder.partial_response_content = f"""
 Do this:
 
 {Path(file1).name}
 <<<<<<< ORIGINAL
@@ -286,15 +284,14 @@
         files = [file1]
 
         # Initialize the Coder object with the mocked IO and mocked repo
         coder = Coder.create(
             models.GPT4,
             "diff",
             io=InputOutput(dry_run=True),
-            openai_api_key="fake_key",
             fnames=files,
             dry_run=True,
         )
 
         def mock_send(*args, **kwargs):
             coder.partial_response_content = f"""
 Do this:
```

### Comparing `aider-chat-0.8.3/tests/test_io.py` & `aider-chat-0.9.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/tests/test_main.py` & `aider-chat-0.9.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/tests/test_models.py` & `aider-chat-0.9.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.3/tests/test_repomap.py` & `aider-chat-0.9.0/tests/test_repomap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
-import tempfile
 import unittest
 from unittest.mock import patch
 
 from aider.io import InputOutput
 from aider.repomap import RepoMap
 
+from tests.utils import IgnorantTemporaryDirectory
+
 
 class TestRepoMap(unittest.TestCase):
     def test_get_repo_map(self):
         # Create a temporary directory with sample files for testing
         test_files = [
             "test_file1.py",
             "test_file2.py",
             "test_file3.md",
             "test_file4.json",
         ]
 
-        with tempfile.TemporaryDirectory() as temp_dir:
+        with IgnorantTemporaryDirectory() as temp_dir:
             for file in test_files:
                 with open(os.path.join(temp_dir, file), "w") as f:
                     f.write("")
 
             io = InputOutput()
             repo_map = RepoMap(root=temp_dir, io=io)
             other_files = [os.path.join(temp_dir, file) for file in test_files]
@@ -29,14 +30,17 @@
 
             # Check if the result contains the expected tags map
             self.assertIn("test_file1.py", result)
             self.assertIn("test_file2.py", result)
             self.assertIn("test_file3.md", result)
             self.assertIn("test_file4.json", result)
 
+            # close the open cache files, so Windows won't error
+            del repo_map
+
     def test_get_repo_map_with_identifiers(self):
         # Create a temporary directory with a sample Python file containing identifiers
         test_file1 = "test_file_with_identifiers.py"
         file_content1 = """\
 class MyClass:
     def my_method(self, arg1, arg2):
         return arg1 + arg2
@@ -53,15 +57,15 @@
 print(obj.my_method(1, 2))
 print(my_function(3, 4))
 """
 
         test_file3 = "test_file_pass.py"
         file_content3 = "pass"
 
-        with tempfile.TemporaryDirectory() as temp_dir:
+        with IgnorantTemporaryDirectory() as temp_dir:
             with open(os.path.join(temp_dir, test_file1), "w") as f:
                 f.write(file_content1)
 
             with open(os.path.join(temp_dir, test_file2), "w") as f:
                 f.write(file_content2)
 
             with open(os.path.join(temp_dir, test_file3), "w") as f:
@@ -79,14 +83,17 @@
             # Check if the result contains the expected tags map with identifiers
             self.assertIn("test_file_with_identifiers.py", result)
             self.assertIn("MyClass", result)
             self.assertIn("my_method", result)
             self.assertIn("my_function", result)
             self.assertIn("test_file_pass.py", result)
 
+            # close the open cache files, so Windows won't error
+            del repo_map
+
     def test_check_for_ctags_failure(self):
         with patch("subprocess.run") as mock_run:
             mock_run.side_effect = Exception("ctags not found")
             repo_map = RepoMap(io=InputOutput())
             self.assertFalse(repo_map.has_ctags)
 
     def test_check_for_ctags_success(self):
@@ -114,25 +121,28 @@
             "test_file2.md",
             "test_file3.json",
             "test_file4.html",
             "test_file5.css",
             "test_file6.js",
         ]
 
-        with tempfile.TemporaryDirectory() as temp_dir:
+        with IgnorantTemporaryDirectory() as temp_dir:
             for file in test_files:
                 with open(os.path.join(temp_dir, file), "w") as f:
                     f.write("")
 
             repo_map = RepoMap(root=temp_dir, io=InputOutput())
             repo_map.has_ctags = False  # force it off
 
             other_files = [os.path.join(temp_dir, file) for file in test_files]
             result = repo_map.get_repo_map([], other_files)
 
             # Check if the result contains each specific file in the expected tags map without ctags
             for file in test_files:
                 self.assertIn(file, result)
 
+            # close the open cache files, so Windows won't error
+            del repo_map
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aider-chat-0.8.3/tests/test_wholefile.py` & `aider-chat-0.9.0/tests/test_wholefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,17 +288,15 @@
 
         with open(file1, "w", encoding="utf-8") as f:
             f.write("one\ntwo\nthree\n")
 
         files = [file1]
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder.create(
-            models.GPT4, "whole", io=InputOutput(), openai_api_key="fake_key", fnames=files
-        )
+        coder = Coder.create(models.GPT4, "whole", io=InputOutput(), fnames=files)
 
         # no trailing newline so the response content below doesn't add ANOTHER newline
         new_content = "new\ntwo\nthree"
 
         def mock_send(*args, **kwargs):
             coder.partial_response_content = f"""
 Do this:
```

