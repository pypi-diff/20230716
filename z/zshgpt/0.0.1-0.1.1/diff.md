# Comparing `tmp/zshgpt-0.0.1.tar.gz` & `tmp/zshgpt-0.1.1.tar.gz`

## Comparing `zshgpt-0.0.1.tar` & `zshgpt-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zshgpt-0.0.1/src/zshgpt/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.0.1/src/zshgpt/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.0.1/src/zshgpt/__main__.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 zshgpt-0.0.1/src/zshgpt/cli/__init__.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 zshgpt-0.0.1/src/zshgpt/cli/messages.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.0.1/zsh_plugin/zsh_plugin.zsh
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 zshgpt-0.0.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 zshgpt-0.0.1/README.md
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 zshgpt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 zshgpt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/__main__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/cli/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/cli/messages.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.1.1/zsh_plugin/zsh_plugin.zsh
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 zshgpt-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 zshgpt-0.1.1/README.md
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 zshgpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 zshgpt-0.1.1/PKG-INFO
```

### Comparing `zshgpt-0.0.1/src/zshgpt/cli/__init__.py` & `zshgpt-0.1.1/src/zshgpt/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,7 @@
 @click.version_option(version=__version__, prog_name='zshgpt')
 @click.argument('user_query')
 def zshgpt(user_query: str) -> str:
     response = openai.ChatCompletion.create(
         model='gpt-3.5-turbo', messages=[*messages, {'role': 'user', 'content': user_query}]
     )
     click.echo(response['choices'][0]['message']['content'], nl=False)
-
-
```

### Comparing `zshgpt-0.0.1/src/zshgpt/cli/messages.py` & `zshgpt-0.1.1/src/zshgpt/cli/messages.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 messages = [
     {
         'role': 'system',
-        'content': 'You are a zsh terminal assistant. '
-        'Complete the textual query of the '
-        'user with a valid zsh command or a textual reply as a comment.',
+        'content': """You are a zsh terminal assistant.
+- If the user wants a command give it to them.
+- If the user wants a textual answer, remember to put # in front of all lines in your answer.""",
     },
     {'role': 'user', 'content': '# Can you say hello?'},
     {'role': 'assistant', 'content': '# Hello!'},
     {'role': 'user', 'content': '# what processes are hogging the most cpu?'},
     {'role': 'assistant', 'content': 'ps aux | sort -nrk 3,3 | head -n 10.'},
     {'role': 'user', 'content': '# Who won the world series in 2020?'},
     {
@@ -32,15 +32,17 @@
     {'role': 'user', 'content': '# what other devices are on my network?'},
     {'role': 'assistant', 'content': 'arp -a'},
     {'role': 'user', 'content': '# how much storage is left?'},
     {'role': 'assistant', 'content': 'df -h'},
     {'role': 'user', 'content': '# Tell me a joke'},
     {
         'role': 'assistant',
-        'content': "# Sure, here's a joke for you: Why did the tomato turn red? Because it saw the salad dressing!",
+        'content': """# Sure, here's a joke for you: Why did the tomato turn red?
+
+Because it saw the salad dressing!""",
     },
     {'role': 'user', 'content': '# Another one, but multiple lines'},
     {
         'role': 'assistant',
         'content': """# Sure, here's a multiline joke for you:
 
 # Why don't skeletons fight each other?
@@ -48,11 +50,10 @@
 
 # Why did the scarecrow win an award?
 # Because he was outstanding in his field.
 
 # Why don't scientists trust atoms?
 # Because they make up everything.
 
-# I hope you enjoyed the jokes!
-""",
+# I hope you enjoyed the jokes!""",
     },
 ]
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-messages = [ { 'role': 'system', 'content': 'You are a zsh terminal assistant.
-' 'Complete the textual query of the ' 'user with a valid zsh command or a
-textual reply as a comment.', }, {'role': 'user', 'content': '# Can you say
-hello?'}, {'role': 'assistant', 'content': '# Hello!'}, {'role': 'user',
-'content': '# what processes are hogging the most cpu?'}, {'role': 'assistant',
-'content': 'ps aux | sort -nrk 3,3 | head -n 10.'}, {'role': 'user', 'content':
-'# Who won the world series in 2020?'}, { 'role': 'assistant', 'content': '#
-The Los Angeles Dodgers won the World Series in 2020.', }, {'role': 'user',
-'content': "# what's the weather in San Francisco?"}, {'role': 'assistant',
-'content': 'curl wttr.in/SanFrancisco'}, {'role': 'user', 'content': '# how big
-is pi, with accouracy of 10 decimals?'}, {'role': 'assistant', 'content': '# pi
-is 3.1415926535'}, {'role': 'user', 'content': '# add a hello world website to
-the index'}, { 'role': 'assistant', 'content': "echo '
+messages = [ { 'role': 'system', 'content': """You are a zsh terminal
+assistant. - If the user wants a command give it to them. - If the user wants a
+textual answer, remember to put # in front of all lines in your answer.""", },
+{'role': 'user', 'content': '# Can you say hello?'}, {'role': 'assistant',
+'content': '# Hello!'}, {'role': 'user', 'content': '# what processes are
+hogging the most cpu?'}, {'role': 'assistant', 'content': 'ps aux | sort -nrk
+3,3 | head -n 10.'}, {'role': 'user', 'content': '# Who won the world series in
+2020?'}, { 'role': 'assistant', 'content': '# The Los Angeles Dodgers won the
+World Series in 2020.', }, {'role': 'user', 'content': "# what's the weather in
+San Francisco?"}, {'role': 'assistant', 'content': 'curl wttr.in/
+SanFrancisco'}, {'role': 'user', 'content': '# how big is pi, with accouracy of
+10 decimals?'}, {'role': 'assistant', 'content': '# pi is 3.1415926535'},
+{'role': 'user', 'content': '# add a hello world website to the index'},
+{ 'role': 'assistant', 'content': "echo '
 ****** Hello World! ******
 ' > web-app/index.html", }, {'role': 'user', 'content': '# open it with vi'},
 {'role': 'assistant', 'content': 'vi web-app/index.html'}, {'role': 'user',
 'content': "# what's running on port 1018?"}, {'role': 'assistant', 'content':
 'lsof -i :1018'}, {'role': 'user', 'content': '# kill process 1584'}, {'role':
 'assistant', 'content': 'kill -9 1584'}, {'role': 'user', 'content': '# what
 other devices are on my network?'}, {'role': 'assistant', 'content': 'arp -a'},
 {'role': 'user', 'content': '# how much storage is left?'}, {'role':
 'assistant', 'content': 'df -h'}, {'role': 'user', 'content': '# Tell me a
-joke'}, { 'role': 'assistant', 'content': "# Sure, here's a joke for you: Why
-did the tomato turn red? Because it saw the salad dressing!", }, {'role':
+joke'}, { 'role': 'assistant', 'content': """# Sure, here's a joke for you: Why
+did the tomato turn red? Because it saw the salad dressing!""", }, {'role':
 'user', 'content': '# Another one, but multiple lines'}, { 'role': 'assistant',
 'content': """# Sure, here's a multiline joke for you: # Why don't skeletons
 fight each other? # They don't have the guts. # Why did the scarecrow win an
 award? # Because he was outstanding in his field. # Why don't scientists trust
-atoms? # Because they make up everything. # I hope you enjoyed the jokes! """,
+atoms? # Because they make up everything. # I hope you enjoyed the jokes!""",
 }, ]
```

### Comparing `zshgpt-0.0.1/zsh_plugin/zsh_plugin.zsh` & `zshgpt-0.1.1/zsh_plugin/zsh_plugin.zsh`

 * *Files identical despite different names*

### Comparing `zshgpt-0.0.1/.gitignore` & `zshgpt-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zshgpt-0.0.1/LICENSE.txt` & `zshgpt-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zshgpt-0.0.1/pyproject.toml` & `zshgpt-0.1.1/pyproject.toml`

 * *Files identical despite different names*

