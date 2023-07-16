# Comparing `tmp/afkode-0.4.3.tar.gz` & `tmp/afkode-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afkode-0.4.3.tar", max compression
+gzip compressed data, was "afkode-0.4.4.tar", max compression
```

## Comparing `afkode-0.4.3.tar` & `afkode-0.4.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       55 2023-07-15 22:05:21.061208 afkode-0.4.3/LICENSE
--rw-r--r--   0        0        0     6407 2023-07-15 22:05:21.061208 afkode-0.4.3/README.md
--rw-r--r--   0        0        0      446 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/__init__.py
--rw-r--r--   0        0        0     2896 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/action.py
--rw-r--r--   0        0        0     5747 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/api.py
--rw-r--r--   0        0        0      834 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/0_template.py
--rw-r--r--   0        0        0       81 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/__init__.py
--rw-r--r--   0        0        0      851 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/keyword_search.py
--rw-r--r--   0        0        0      787 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/list_actions.py
--rw-r--r--   0        0        0      852 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/send_latest_agent_response_to_notes.py
--rw-r--r--   0        0        0      743 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/send_latest_transcription_to_chat.py
--rw-r--r--   0        0        0      815 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/send_latest_transcription_to_notes.py
--rw-r--r--   0        0        0      860 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_actions.py
--rw-r--r--   0        0        0      994 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_functionality.py
--rw-r--r--   0        0        0      987 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_improvements.py
--rw-r--r--   0        0        0      984 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_tests.py
--rw-r--r--   0        0        0      995 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/summarize_filename.py
--rw-r--r--   0        0        0     1195 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/summarize_today.py
--rw-r--r--   0        0        0      148 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/config.json
--rw-r--r--   0        0        0      306 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/globals.py
--rw-r--r--   0        0        0       81 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/ios/__init__.py
--rw-r--r--   0        0        0     2263 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/ios/listen.py
--rw-r--r--   0        0        0      938 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/ios/speech.py
--rw-r--r--   0        0        0       81 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/__init__.py
--rw-r--r--   0        0        0     3586 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/blip.wav
--rw-r--r--   0        0        0     2980 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/listen.py
--rw-r--r--   0        0        0     3409 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/speech.py
--rw-r--r--   0        0        0     3286 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/meta.py
--rw-r--r--   0        0        0     1545 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/nox_tests.txt
--rw-r--r--   0        0        0      662 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_actions.txt
--rw-r--r--   0        0        0      608 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_functionality.txt
--rw-r--r--   0        0        0     1191 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_improvements.txt
--rw-r--r--   0        0        0      634 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_tests.txt
--rw-r--r--   0        0        0      326 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/whisper_hallucinations.txt
--rw-r--r--   0        0        0     1404 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/choose_command.txt
--rw-r--r--   0        0        0      916 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/harmonize_transcripts.txt
--rw-r--r--   0        0        0      777 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/proposed_filename.txt
--rw-r--r--   0        0        0     1738 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/user_input_assist.txt
--rw-r--r--   0        0        0     2231 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/run.py
--rw-r--r--   0        0        0      639 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/set_env.py
--rw-r--r--   0        0        0     8574 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/utils.py
--rw-r--r--   0        0        0     8186 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/voice_interface.py
--rw-r--r--   0        0        0     3320 2023-07-15 22:05:21.065209 afkode-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8414 2023-07-15 22:07:34.093763 afkode-0.4.3/setup.py
--rw-r--r--   0        0        0     9024 2023-07-15 22:07:34.095024 afkode-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-07-16 00:24:21.053440 afkode-0.4.4/LICENSE
+-rw-r--r--   0        0        0     6448 2023-07-16 00:24:21.053440 afkode-0.4.4/README.md
+-rw-r--r--   0        0        0      446 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/__init__.py
+-rw-r--r--   0        0        0     2934 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/action.py
+-rw-r--r--   0        0        0     5763 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/api.py
+-rw-r--r--   0        0        0      834 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/commands/0_template.py
+-rw-r--r--   0        0        0       81 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/commands/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/commands/keyword_search.py
+-rw-r--r--   0        0        0      604 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/commands/list_actions.py
+-rw-r--r--   0        0        0      852 2023-07-16 00:24:21.053440 afkode-0.4.4/afkode/commands/send_latest_agent_response_to_notes.py
+-rw-r--r--   0        0        0      743 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/send_latest_transcription_to_chat.py
+-rw-r--r--   0        0        0      815 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/send_latest_transcription_to_notes.py
+-rw-r--r--   0        0        0      876 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/suggest_program_actions.py
+-rw-r--r--   0        0        0     1024 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/suggest_program_functionality.py
+-rw-r--r--   0        0        0     1017 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/suggest_program_improvements.py
+-rw-r--r--   0        0        0     1000 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/suggest_program_tests.py
+-rw-r--r--   0        0        0     1011 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/summarize_filename.py
+-rw-r--r--   0        0        0     1195 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/commands/summarize_today.py
+-rw-r--r--   0        0        0      148 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/config.json
+-rw-r--r--   0        0        0      306 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/globals.py
+-rw-r--r--   0        0        0       81 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/ios/__init__.py
+-rw-r--r--   0        0        0     2263 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/ios/listen.py
+-rw-r--r--   0        0        0      938 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/ios/speech.py
+-rw-r--r--   0        0        0       81 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/macos/__init__.py
+-rw-r--r--   0        0        0     3586 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/macos/blip.wav
+-rw-r--r--   0        0        0     2980 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/macos/listen.py
+-rw-r--r--   0        0        0     3409 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/macos/speech.py
+-rw-r--r--   0        0        0     3286 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/meta.py
+-rw-r--r--   0        0        0     1545 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/debug/nox_tests.txt
+-rw-r--r--   0        0        0      662 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/debug/program_actions.txt
+-rw-r--r--   0        0        0      608 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/debug/program_functionality.txt
+-rw-r--r--   0        0        0     1191 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/debug/program_improvements.txt
+-rw-r--r--   0        0        0      634 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/debug/program_tests.txt
+-rw-r--r--   0        0        0      358 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/debug/whisper_hallucinations.txt
+-rw-r--r--   0        0        0     1404 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/programflow/choose_command.txt
+-rw-r--r--   0        0        0      916 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/programflow/harmonize_transcripts.txt
+-rw-r--r--   0        0        0      777 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/programflow/proposed_filename.txt
+-rw-r--r--   0        0        0     1738 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/prompts/programflow/user_input_assist.txt
+-rw-r--r--   0        0        0     2231 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/run.py
+-rw-r--r--   0        0        0      639 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/set_env.py
+-rw-r--r--   0        0        0     8574 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/utils.py
+-rw-r--r--   0        0        0     8186 2023-07-16 00:24:21.057440 afkode-0.4.4/afkode/voice_interface.py
+-rw-r--r--   0        0        0     3357 2023-07-16 00:24:21.057440 afkode-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     8483 2023-07-16 00:26:15.592821 afkode-0.4.4/setup.py
+-rw-r--r--   0        0        0     9103 2023-07-16 00:26:15.594154 afkode-0.4.4/PKG-INFO
```

### Comparing `afkode-0.4.3/README.md` & `afkode-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,20 @@
 Follow the [Instructions for developers](#instructions-for-developers) to set up the virtual environment and dependency management.
 
 ### Installation
 
 MacOS requirements:
 
 - Python 3.8
+- pyaudio
 - ffmpeg for mp3 text-to-speech, `brew install ffmpeg`
 
+```
+brew install portaudio
+```
 
 Note: Instructions marked with %% are not functioning and are for demo purposes only.
 
 Install the project using pip %%:
 
 ```bash
 pip install afkode
```

### Comparing `afkode-0.4.3/afkode/action.py` & `afkode-0.4.4/afkode/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 
         Args:
             command_candidate (str): The potential command name to look for.
         """
         options = utils.get_formatted_command_list()
 
         # Get our command prompt
-        choose_command_prompt = Path(utils.get_prompt_path(), "programflow", "choose_command.txt").read_text()
+        choose_command_prompt = Path(utils.get_prompt_path(), "programflow", "choose_command.txt").read_text(
+            encoding="utf-8"
+        )
 
         choose_command_request = (
             choose_command_prompt + "\nUser input:" + command_candidate + f"\n{'-'*20}Options:\n" + options
         )
         choose_command_response = api.chatgpt(choose_command_request)
         logging.debug(f"Request: {choose_command_request}")
         logging.info(f"Command: {choose_command_response}")
```

### Comparing `afkode-0.4.3/afkode/api.py` & `afkode-0.4.4/afkode/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         logging.error("Whisper API connection error")
         # speak("Connection error")
         transcript = "exit"
 
     # Whisper is prone to hallucinations, so we suppress known hallucination outputs
     # They aren't really a problem at least in the longer transcripts, but they mess up the logging
     hallucinations_path = Path(utils.get_base_path(), "afkode", "prompts", "debug", "whisper_hallucinations.txt")
-    hallucinations = hallucinations_path.read_text().split("\n")
+    hallucinations = hallucinations_path.read_text(encoding="utf-8").split("\n")
     if transcript in hallucinations:
         logging.debug("Hallucination detected")
         transcript = ""
 
     return transcript
```

### Comparing `afkode-0.4.3/afkode/commands/0_template.py` & `afkode-0.4.4/afkode/commands/0_template.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/commands/keyword_search.py` & `afkode-0.4.4/afkode/commands/keyword_search.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/commands/list_actions.py` & `afkode-0.4.4/afkode/commands/list_actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 by Nick Jenkins. All rights reserved
 """Custom command."""
-
-from pathlib import Path
-
 from afkode import utils
 
 
 def execute(all_additional_instructions_provided_after_command: str) -> str:
     """The user wants information from a file system about what command names are available.
 
     Args:
         all_additional_instructions_provided_after_command: all_additional_instructions_provided_after_command
 
     Returns:
         list of commands
     """
-    command_dir = Path(utils.get_base_path(), "afkode", "commands")
-    ignore = ["__init__"]
-    command_files = sorted([f.stem.replace("_", " ") for f in command_dir.glob("*.py") if f.stem not in ignore])
-
+    command_files = utils.get_spoken_command_list()
     response = "List of commands: " + "\n".join(command_files)
     return response
```

### Comparing `afkode-0.4.3/afkode/commands/send_latest_agent_response_to_notes.py` & `afkode-0.4.4/afkode/commands/send_latest_agent_response_to_notes.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/commands/send_latest_transcription_to_chat.py` & `afkode-0.4.4/afkode/commands/send_latest_transcription_to_chat.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/commands/send_latest_transcription_to_notes.py` & `afkode-0.4.4/afkode/commands/send_latest_transcription_to_notes.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/commands/suggest_program_actions.py` & `afkode-0.4.4/afkode/commands/suggest_program_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     Args:
         not_used: not_used
 
     Returns:
         Chatgpt reponse
     """
-    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_actions.txt").read_text()
+    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_actions.txt").read_text(encoding="utf-8")
 
     readme = meta.get_formatted_readme()
     run = meta.clean_py(Path(utils.get_base_path(), "afkode", "run.py").read_text(encoding="utf-8"))
     commands = utils.get_formatted_command_list()
 
     request = program_commands_prompt + "\n\n" + readme + "\n\n" + run + "\n\n" + commands
     response = api.chatgpt(request)
```

### Comparing `afkode-0.4.3/afkode/commands/suggest_program_functionality.py` & `afkode-0.4.4/afkode/commands/suggest_program_functionality.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
     Args:
         not_used: not_used
 
     Returns:
         Chatgpt reponse
     """
-    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_functionality.txt").read_text()
+    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_functionality.txt").read_text(
+        encoding="utf-8"
+    )
 
     readme = meta.get_formatted_readme()
 
     file_data = ""
     input_files = utils.resolve_input_paths(["/**/*.py"], exclude=["__init__.py"])
     for input_file in input_files:
         clean = meta.clean_py(input_file.read_text(encoding="utf-8"))
```

### Comparing `afkode-0.4.3/afkode/commands/suggest_program_improvements.py` & `afkode-0.4.4/afkode/commands/suggest_program_improvements.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
     Args:
         not_used: not_used
 
     Returns:
         Chatgpt reponse
     """
-    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_improvements.txt").read_text()
+    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_improvements.txt").read_text(
+        encoding="utf-8"
+    )
 
     readme = meta.get_formatted_readme()
 
     file_data = ""
     input_files = utils.resolve_input_paths(["/**/*.py"], exclude=["__init__.py"])
     for input_file in input_files:
         clean = meta.clean_py(input_file.read_text(encoding="utf-8"))
```

### Comparing `afkode-0.4.3/afkode/commands/suggest_program_tests.py` & `afkode-0.4.4/afkode/commands/suggest_program_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     Args:
         not_used: not_used
 
     Returns:
         Chatgpt reponse
     """
-    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_tests.txt").read_text()
+    program_commands_prompt = Path(utils.get_prompt_path(), "debug", "program_tests.txt").read_text(encoding="utf-8")
 
     readme = meta.get_formatted_readme()
 
     file_data = ""
     input_files = utils.resolve_input_paths(["../tests/*.py", "/**/*.py"], exclude=["__init__.py"])
     for input_file in input_files:
         clean = meta.clean_py(input_file.read_text(encoding="utf-8"))
```

### Comparing `afkode-0.4.3/afkode/commands/summarize_filename.py` & `afkode-0.4.4/afkode/commands/summarize_filename.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Args:
         transcript: transcription input from user
 
     Returns:
         Chatgpt response, limited to four words
     """
-    prompt = Path(utils.get_prompt_path(), "programflow", "proposed_filename.txt").read_text()
+    prompt = Path(utils.get_prompt_path(), "programflow", "proposed_filename.txt").read_text(encoding="utf-8")
     request = prompt + "\n\n--------- Here is the user input:\n" + transcript
 
     logging.debug(request)
     response = api.chatgpt(request)
 
     proposed_filename = " ".join(f"{response}    ".split(" ")[:4]).strip()
     output_path = Path(utils.get_user_prompt_directory(), f"{dt.now()} - {proposed_filename}.txt")
```

### Comparing `afkode-0.4.3/afkode/commands/summarize_today.py` & `afkode-0.4.4/afkode/commands/summarize_today.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/ios/listen.py` & `afkode-0.4.4/afkode/ios/listen.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/ios/speech.py` & `afkode-0.4.4/afkode/ios/speech.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/macos/blip.wav` & `afkode-0.4.4/afkode/macos/blip.wav`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/macos/listen.py` & `afkode-0.4.4/afkode/macos/listen.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/macos/speech.py` & `afkode-0.4.4/afkode/macos/speech.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/meta.py` & `afkode-0.4.4/afkode/meta.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/debug/nox_tests.txt` & `afkode-0.4.4/afkode/prompts/debug/nox_tests.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/debug/program_actions.txt` & `afkode-0.4.4/afkode/prompts/debug/program_actions.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/debug/program_functionality.txt` & `afkode-0.4.4/afkode/prompts/debug/program_functionality.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/debug/program_improvements.txt` & `afkode-0.4.4/afkode/prompts/debug/program_improvements.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/debug/program_tests.txt` & `afkode-0.4.4/afkode/prompts/debug/program_tests.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/programflow/choose_command.txt` & `afkode-0.4.4/afkode/prompts/programflow/choose_command.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/programflow/harmonize_transcripts.txt` & `afkode-0.4.4/afkode/prompts/programflow/harmonize_transcripts.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/programflow/proposed_filename.txt` & `afkode-0.4.4/afkode/prompts/programflow/proposed_filename.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/prompts/programflow/user_input_assist.txt` & `afkode-0.4.4/afkode/prompts/programflow/user_input_assist.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/run.py` & `afkode-0.4.4/afkode/run.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/set_env.py` & `afkode-0.4.4/afkode/set_env.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/utils.py` & `afkode-0.4.4/afkode/utils.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/afkode/voice_interface.py` & `afkode-0.4.4/afkode/voice_interface.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.3/pyproject.toml` & `afkode-0.4.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "afkode"
-version = "0.4.3"
+version = "0.4.4"
 description = "Personal voice command interface for iPhone on pythonista powered by Whisper and ChatGPT."
 license = "MIT"
 authors = ["Nick Jenkins"]
 readme = "README.md"
 homepage = "https://www.ndjenkins.com/"
 repository = "https://github.com/ndjenkins85/afkode/"
 documentation = "https://ndjenkins85.github.io/afkode/"
@@ -35,15 +35,15 @@
 python = ">=3.8.1,<3.9"
 
 openai = "^0.27.5"
 PyAudio = "^0.2.13"
 PyYAML = "^6.0"
 pydub = "^0.25.1"
 gTTS = "^2.3.2"
-
+google-auth = "2.22.0"
 requests = "^2.23.0"
 requests_toolbelt = "^1.0.0"
 urllib3 = "1.26.16"
 types-requests = "^2.31.0"
 
 black = { version = "^23.3", optional = true }
 darglint = { version = "^1.8", optional = true }
@@ -68,14 +68,15 @@
 sphinx_rtd_theme = { version = "^1.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.23.1"
 ipython = "7.23.1"
 traitlets = "^5.9.0"
 jupyter = "^1.0.0"
+lxml = "4.9.2"
 nox = "^2023.04.22"
 pre-commit = "^2.15"
 MarkupSafe = "^2.0.1"
 
 [tool.poetry.extras]
 lint = ["black", "darglint", "flake8", "mypy", "safety", "xdoctest", "flake8-annotations", "flake8-bandit", "flake8-bugbear", "flake8-builtins", "flake8-docstrings", "types-PyYAML"]
 tests = ["pytest", "pytest-cases", "pytest-cov"]
```

### Comparing `afkode-0.4.3/setup.py` & `afkode-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 package_data = \
 {'': ['*'], 'afkode': ['prompts/debug/*', 'prompts/programflow/*']}
 
 install_requires = \
 ['PyAudio>=0.2.13,<0.3.0',
  'PyYAML>=6.0,<7.0',
  'gTTS>=2.3.2,<3.0.0',
+ 'google-auth==2.22.0',
  'openai>=0.27.5,<0.28.0',
  'pydub>=0.25.1,<0.26.0',
  'requests>=2.23.0,<3.0.0',
  'requests_toolbelt>=1.0.0,<2.0.0',
  'types-requests>=2.31.0,<3.0.0',
  'urllib3==1.26.16']
 
@@ -40,17 +41,17 @@
            'pytest-cov>=3.0,<4.0']}
 
 entry_points = \
 {'console_scripts': ['afkode = afkode.run:start']}
 
 setup_kwargs = {
     'name': 'afkode',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'Personal voice command interface for iPhone on pythonista powered by Whisper and ChatGPT.',
-    'long_description': '# AFKode - Speak it, Save it, AFKode it!\n\nAFKode allows users to interact with AI and file system using only voice, allowing you to work away from keyboard.\nWorks on iPhone with pythonista, or on MacOS.\nPowered by Whisper and ChatGPT.\n\nThis project was inspired by long walks on the beach while ruminating and organizing ones thoughts.\n\nUsers of this program should be comfortable using pythonista/python.\nYou are required to BYO OpenAI secret key in variable `OPENAI_KEY` using environment variables or within `afkcode/secrets.py`.\n\nKey features:\n\n- Detection of start/stop dictation for transcription\n- Uses ChatGPT create smart file naming for your notes\n\nInterfaces:\n\n* At home: Supports MacOS with base speakers/microphone or AirPods. May not work with other bluetooth headsets like Bose headphones.\n* Out and about: Supports Pythonista iOS with base speakers/microphones, or plugged in lightning wired heaphones. Bluetooth headsets like AirPods and Bose headphones currently not working.\n\n## Contents\n\n* [Instructions for users](#instructions-for-users)\n  * [Installation](#installation)\n  * [Usage documentation](#usage-documentation)\n  * [Bug reports](#bug-reports)\n* [Instructions for developers](#instructions-for-developers)\n  * [Poetry](#environment-1-poetry)\n  * [Testing with Nox](#testing-with-nox)\n  * [Code formatting with Pre-commit](#code-formatting-with-pre-commit)\n* [Contributors](#contributors)\n\n## Instructions for users\n\nThe following are the quick start instructions for using the project as an end-user.\n\nFollow the [Instructions for developers](#instructions-for-developers) to set up the virtual environment and dependency management.\n\n### Installation\n\nMacOS requirements:\n\n- Python 3.8\n- ffmpeg for mp3 text-to-speech, `brew install ffmpeg`\n\n\nNote: Instructions marked with %% are not functioning and are for demo purposes only.\n\nInstall the project using pip %%:\n\n```bash\npip install afkode\n```\n\nTo replicate the data transformations and model results, run the following commands from the project root.\nThese should be run from the `poetry shell`, or `conda` environment, or with the `poetry run` prefix.\n```bash\npython -m afkode.run\n```\n\n### Usage documentation\n\nThe user guides can be found on [github pages](https://ndjenkins85.github.io/afkode).\nThis includes overview of features, discussion of `afkode` framework, and API reference.\n\n### Bug reports\n\nPlease raise an [issue](https://github.com/ndjenkins85/afkode/issues) with `bug` label and I will look into it!\n\n## Instructions for developers\n\nThe following are the setup instructions for developers looking to improve this project.\nFor information on current contributors and guidelines see the [contributors](#contributors) section.\nFollow each step here and ensure tests are working.\n\n### Poetry\n\n[Poetry](https://python-poetry.org/docs/) handles virtual environment management, dev and optional extra libraries, library development, builds and publishing.\n\nCheck the poetry website for the latest instructions on how to install poetry.\nYou can use the following command on OS/linux to install poetry 1.1.9 used in this project.\n\n```bash\ncurl -sSL https://install.python-poetry.org | python - --version 1.1.9\n```\n\nIt is recommended to set virtual environment creation to within project using the following command.\nThis adds a `.venv` directory to project to handle cache and virtual environment.\n```bash\npoetry config virtualenvs.in-project true\n```\n\nYou can set up the virtual environment in the repo using the following command.\nMake sure that any other virtual environments (i.e. `conda deactivate`) are deactivated before running.\n\n```bash\npoetry install\n```\n\nTroubleshooting: You may need to point poetry to the correct python interpreter using the following command.\nIn another terminal and in conda, run `which python`.\n```bash\npoetry env use /path/to/python3\n```\n\nWhen the environment is correctly installed, you can enter the virtual environment using `poetry shell`. Library can be built using `poetry build`.\n\n### Testing with Nox\n\n[Nox](https://nox.thea.codes/en/stable/index.html) is a command-line tool that automates testing in multiple Python environments, similar to tox, Makefiles or scripts. Unlike tox, Nox uses a standard Python file for configuration.\n\nHere it is used for code quality, testing, and generating documentation.\n\nThe following command can be used to run mypy, lint, and tests.\nIt is recommended to run these before pushing code, as this is run with Github Actions.\nSome checks such as black are run more frequently with [pre-commit](#code-formatting-with-pre-commit).\n\n```bash\npoetry run nox\n```\n\nLocal Sphinx documentation can be generated with the following command.\nDocumentation publishing using Github Actions to Github pages is enabled by default.\n\n```bash\npoetry run nox -s docs\n```\n\nOther available commands include:\n\n```bash\npoetry run nox -rs coverage\n```\n\n### Code formatting with Pre-commit\n\n[Pre-commit](https://pre-commit.com/) is a framework for managing and maintaining multi-language pre-commit hooks.\n\nIt intercepts the `git commit` command to run checks of staged code before the commit is finalized.\nThe checks are specified in `.pre-commit-config.yaml`.\nChecks in use are quick, pragmatic, and apply automatic formatting checks.\nIf checks fail, it is usually only a matter of re-staging the files (`git add`) and attempting to commit again.\n\nThe aim is to provide a lightweight way to keep some code standards automatically in line with standards.\nThis does not replace the need to run nox tests, although pre-commits will satisfy some of the nox test checks.\n\nOn first time use of the repository, pre-commit will need to be installed locally.\nYou will need to be in the `poetry shell` or `conda` environment.\nRun the following command to perform a first time install.\n\n```bash\npre-commit install\n```\n\nThis will cache several code assets used in the checks.\n\nWhen you have new code to commit, pre-commit will kick in and check the code.\nAlternatively, you can run the following command to run for all files in repo.\n\n``` bash\npre-commit run --all-files\n```\n\n## Contributors\n\n* [Nick Jenkins](https://www.ndjenkins.com) - Data Scientist, API & Web dev, Team lead, Writer\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) in Github repo for specific instructions on contributing to project.\n\nUsage rights governed by [LICENSE](LICENSE)  in Github repo or page footer.\n',
+    'long_description': '# AFKode - Speak it, Save it, AFKode it!\n\nAFKode allows users to interact with AI and file system using only voice, allowing you to work away from keyboard.\nWorks on iPhone with pythonista, or on MacOS.\nPowered by Whisper and ChatGPT.\n\nThis project was inspired by long walks on the beach while ruminating and organizing ones thoughts.\n\nUsers of this program should be comfortable using pythonista/python.\nYou are required to BYO OpenAI secret key in variable `OPENAI_KEY` using environment variables or within `afkcode/secrets.py`.\n\nKey features:\n\n- Detection of start/stop dictation for transcription\n- Uses ChatGPT create smart file naming for your notes\n\nInterfaces:\n\n* At home: Supports MacOS with base speakers/microphone or AirPods. May not work with other bluetooth headsets like Bose headphones.\n* Out and about: Supports Pythonista iOS with base speakers/microphones, or plugged in lightning wired heaphones. Bluetooth headsets like AirPods and Bose headphones currently not working.\n\n## Contents\n\n* [Instructions for users](#instructions-for-users)\n  * [Installation](#installation)\n  * [Usage documentation](#usage-documentation)\n  * [Bug reports](#bug-reports)\n* [Instructions for developers](#instructions-for-developers)\n  * [Poetry](#environment-1-poetry)\n  * [Testing with Nox](#testing-with-nox)\n  * [Code formatting with Pre-commit](#code-formatting-with-pre-commit)\n* [Contributors](#contributors)\n\n## Instructions for users\n\nThe following are the quick start instructions for using the project as an end-user.\n\nFollow the [Instructions for developers](#instructions-for-developers) to set up the virtual environment and dependency management.\n\n### Installation\n\nMacOS requirements:\n\n- Python 3.8\n- pyaudio\n- ffmpeg for mp3 text-to-speech, `brew install ffmpeg`\n\n```\nbrew install portaudio\n```\n\nNote: Instructions marked with %% are not functioning and are for demo purposes only.\n\nInstall the project using pip %%:\n\n```bash\npip install afkode\n```\n\nTo replicate the data transformations and model results, run the following commands from the project root.\nThese should be run from the `poetry shell`, or `conda` environment, or with the `poetry run` prefix.\n```bash\npython -m afkode.run\n```\n\n### Usage documentation\n\nThe user guides can be found on [github pages](https://ndjenkins85.github.io/afkode).\nThis includes overview of features, discussion of `afkode` framework, and API reference.\n\n### Bug reports\n\nPlease raise an [issue](https://github.com/ndjenkins85/afkode/issues) with `bug` label and I will look into it!\n\n## Instructions for developers\n\nThe following are the setup instructions for developers looking to improve this project.\nFor information on current contributors and guidelines see the [contributors](#contributors) section.\nFollow each step here and ensure tests are working.\n\n### Poetry\n\n[Poetry](https://python-poetry.org/docs/) handles virtual environment management, dev and optional extra libraries, library development, builds and publishing.\n\nCheck the poetry website for the latest instructions on how to install poetry.\nYou can use the following command on OS/linux to install poetry 1.1.9 used in this project.\n\n```bash\ncurl -sSL https://install.python-poetry.org | python - --version 1.1.9\n```\n\nIt is recommended to set virtual environment creation to within project using the following command.\nThis adds a `.venv` directory to project to handle cache and virtual environment.\n```bash\npoetry config virtualenvs.in-project true\n```\n\nYou can set up the virtual environment in the repo using the following command.\nMake sure that any other virtual environments (i.e. `conda deactivate`) are deactivated before running.\n\n```bash\npoetry install\n```\n\nTroubleshooting: You may need to point poetry to the correct python interpreter using the following command.\nIn another terminal and in conda, run `which python`.\n```bash\npoetry env use /path/to/python3\n```\n\nWhen the environment is correctly installed, you can enter the virtual environment using `poetry shell`. Library can be built using `poetry build`.\n\n### Testing with Nox\n\n[Nox](https://nox.thea.codes/en/stable/index.html) is a command-line tool that automates testing in multiple Python environments, similar to tox, Makefiles or scripts. Unlike tox, Nox uses a standard Python file for configuration.\n\nHere it is used for code quality, testing, and generating documentation.\n\nThe following command can be used to run mypy, lint, and tests.\nIt is recommended to run these before pushing code, as this is run with Github Actions.\nSome checks such as black are run more frequently with [pre-commit](#code-formatting-with-pre-commit).\n\n```bash\npoetry run nox\n```\n\nLocal Sphinx documentation can be generated with the following command.\nDocumentation publishing using Github Actions to Github pages is enabled by default.\n\n```bash\npoetry run nox -s docs\n```\n\nOther available commands include:\n\n```bash\npoetry run nox -rs coverage\n```\n\n### Code formatting with Pre-commit\n\n[Pre-commit](https://pre-commit.com/) is a framework for managing and maintaining multi-language pre-commit hooks.\n\nIt intercepts the `git commit` command to run checks of staged code before the commit is finalized.\nThe checks are specified in `.pre-commit-config.yaml`.\nChecks in use are quick, pragmatic, and apply automatic formatting checks.\nIf checks fail, it is usually only a matter of re-staging the files (`git add`) and attempting to commit again.\n\nThe aim is to provide a lightweight way to keep some code standards automatically in line with standards.\nThis does not replace the need to run nox tests, although pre-commits will satisfy some of the nox test checks.\n\nOn first time use of the repository, pre-commit will need to be installed locally.\nYou will need to be in the `poetry shell` or `conda` environment.\nRun the following command to perform a first time install.\n\n```bash\npre-commit install\n```\n\nThis will cache several code assets used in the checks.\n\nWhen you have new code to commit, pre-commit will kick in and check the code.\nAlternatively, you can run the following command to run for all files in repo.\n\n``` bash\npre-commit run --all-files\n```\n\n## Contributors\n\n* [Nick Jenkins](https://www.ndjenkins.com) - Data Scientist, API & Web dev, Team lead, Writer\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) in Github repo for specific instructions on contributing to project.\n\nUsage rights governed by [LICENSE](LICENSE)  in Github repo or page footer.\n',
     'author': 'Nick Jenkins',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.ndjenkins.com/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `afkode-0.4.3/PKG-INFO` & `afkode-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afkode
-Version: 0.4.3
+Version: 0.4.4
 Summary: Personal voice command interface for iPhone on pythonista powered by Whisper and ChatGPT.
 Home-page: https://www.ndjenkins.com/
 License: MIT
 Keywords: quick_start,python_packaging,whisper,chatgpt,openai
 Author: Nick Jenkins
 Requires-Python: >=3.8.1,<3.9
 Classifier: Development Status :: 4 - Beta
@@ -30,14 +30,15 @@
 Requires-Dist: flake8 (>=6.0,<7.0); extra == "lint"
 Requires-Dist: flake8-annotations (>=3.0,<4.0); extra == "lint"
 Requires-Dist: flake8-bandit (>=4.1,<5.0); extra == "lint"
 Requires-Dist: flake8-bugbear (>=23.6,<24.0); extra == "lint"
 Requires-Dist: flake8-builtins (>=2.1,<3.0); extra == "lint"
 Requires-Dist: flake8-docstrings (>=1.7,<2.0); extra == "lint"
 Requires-Dist: gTTS (>=2.3.2,<3.0.0)
+Requires-Dist: google-auth (==2.22.0)
 Requires-Dist: m2r2 (>=0.3,<0.4); extra == "docs"
 Requires-Dist: mypy (>=0.910,<0.911); extra == "lint"
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytest (>=6.2,<7.0); extra == "tests"
 Requires-Dist: pytest-cases (>=3.6,<4.0); extra == "tests"
 Requires-Dist: pytest-cov (>=3.0,<4.0); extra == "tests"
@@ -95,16 +96,20 @@
 Follow the [Instructions for developers](#instructions-for-developers) to set up the virtual environment and dependency management.
 
 ### Installation
 
 MacOS requirements:
 
 - Python 3.8
+- pyaudio
 - ffmpeg for mp3 text-to-speech, `brew install ffmpeg`
 
+```
+brew install portaudio
+```
 
 Note: Instructions marked with %% are not functioning and are for demo purposes only.
 
 Install the project using pip %%:
 
 ```bash
 pip install afkode
```

