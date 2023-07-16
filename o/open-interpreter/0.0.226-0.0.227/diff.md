# Comparing `tmp/open_interpreter-0.0.226.tar.gz` & `tmp/open_interpreter-0.0.227.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.226.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.227.tar", max compression
```

## Comparing `open_interpreter-0.0.226.tar` & `open_interpreter-0.0.227.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.226/LICENSE
--rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.226/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.226/interpreter/__init__.py
--rw-r--r--   0        0        0     5462 2023-07-15 04:40:20.248931 open_interpreter-0.0.226/interpreter/exec.py
--rw-r--r--   0        0        0     5847 2023-07-15 17:55:30.625029 open_interpreter-0.0.226/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.226/interpreter/json_utils.py
--rw-r--r--   0        0        0     3857 2023-07-15 17:54:55.373624 open_interpreter-0.0.226/interpreter/openai_utils.py
--rw-r--r--   0        0        0     1283 2023-07-14 23:14:50.878970 open_interpreter-0.0.226/interpreter/system_message.txt
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.226/interpreter/view.py
--rw-r--r--   0        0        0      541 2023-07-15 17:56:37.307470 open_interpreter-0.0.226/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 open_interpreter-0.0.226/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.227/LICENSE
+-rw-r--r--   0        0        0     4090 2023-07-16 20:45:43.734678 open_interpreter-0.0.227/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.227/interpreter/__init__.py
+-rw-r--r--   0        0        0     5615 2023-07-16 08:28:36.435313 open_interpreter-0.0.227/interpreter/exec.py
+-rw-r--r--   0        0        0     5847 2023-07-15 17:55:30.625029 open_interpreter-0.0.227/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.227/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3850 2023-07-16 18:00:27.412921 open_interpreter-0.0.227/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     1379 2023-07-16 09:25:30.855857 open_interpreter-0.0.227/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.227/interpreter/view.py
+-rw-r--r--   0        0        0      542 2023-07-16 20:46:40.779010 open_interpreter-0.0.227/pyproject.toml
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 open_interpreter-0.0.227/PKG-INFO
```

### Comparing `open_interpreter-0.0.226/LICENSE` & `open_interpreter-0.0.227/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.226/interpreter/exec.py` & `open_interpreter-0.0.227/interpreter/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,19 @@
         else:
             panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
             self.live.update(panel, refresh=True)
 
     def flush(self):
         pass
 
+    # Some things (like youtube-dl) will check if this is "isatty()"
+    # then fail if it isn't present, so:
+    def isatty(self):
+        return True
+
 def exec_and_capture_output(code):
     # Store the original stdout and stderr
     old_stdout = sys.stdout
     old_stderr = sys.stderr
 
     # Create new instance of InteractiveShell
     shell = InteractiveShell.instance()
```

### Comparing `open_interpreter-0.0.226/interpreter/interpreter.py` & `open_interpreter-0.0.227/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.226/interpreter/json_utils.py` & `open_interpreter-0.0.227/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.226/interpreter/openai_utils.py` & `open_interpreter-0.0.227/interpreter/openai_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def openai_streaming_response(messages, functions, system_message, model, temperature, api_key):
 
     if api_key == None:
         if 'OPENAI_API_KEY' in os.environ:
             api_key = os.environ['OPENAI_API_KEY']
         else:
-            raise Exception("Please provide an OpenAI API key via interpreter.openai_api_key or as an environment variable ('OPENAI_API_KEY').")
+            raise Exception("Please provide an OpenAI API key via interpreter.api_key or as an environment variable ('OPENAI_API_KEY').")
     else:
         openai.api_key = api_key
 
     system_message_event = {"role": "system", "content": system_message}
 
     max_tokens = model_max_tokens[model]
     max_tokens -= num_tokens_from_messages([system_message_event], model)
```

### Comparing `open_interpreter-0.0.226/interpreter/system_message.txt` & `open_interpreter-0.0.227/interpreter/system_message.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 
 If you run_code and it fails, write a message to the user explaining what happened, theorizing why, and planning a new way forward.
 
 While you can generate and display static plots (like those from Matplotlib), you will not be able to see the output-- only the user will see it. Interactive and dynamic visualizations (like those from Plotly) won't be displayed correctly, so if you need to do something like that, save it as an image and display it.
 
 When a user refers to a filename, they're likely referring to an existing file in the directory you're currently in.
 
+If you're going to run a for loop, print something inside it so the user can see its progress.
+
 Write messages to the user in Markdown.
```

### Comparing `open_interpreter-0.0.226/interpreter/view.py` & `open_interpreter-0.0.227/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.226/pyproject.toml` & `open_interpreter-0.0.227/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.226"
-description = "Ask GPT-4 to run code locally"
+version = "0.0.227"
+description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
 rich = "^13.4.2"
```

