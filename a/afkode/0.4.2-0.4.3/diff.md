# Comparing `tmp/afkode-0.4.2.tar.gz` & `tmp/afkode-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afkode-0.4.2.tar", max compression
+gzip compressed data, was "afkode-0.4.3.tar", max compression
```

## Comparing `afkode-0.4.2.tar` & `afkode-0.4.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       55 2023-06-11 20:56:43.959118 afkode-0.4.2/LICENSE
--rw-r--r--   0        0        0     6407 2023-06-18 18:46:50.646174 afkode-0.4.2/README.md
--rw-r--r--   0        0        0      446 2023-07-15 21:45:23.741292 afkode-0.4.2/afkode/__init__.py
--rw-r--r--   0        0        0     2896 2023-07-15 20:48:15.586405 afkode-0.4.2/afkode/action.py
--rw-r--r--   0        0        0     5747 2023-07-15 20:48:15.587406 afkode-0.4.2/afkode/api.py
--rw-r--r--   0        0        0      834 2023-06-21 12:33:57.674451 afkode-0.4.2/afkode/commands/0_template.py
--rw-r--r--   0        0        0       81 2023-06-16 03:57:46.426173 afkode-0.4.2/afkode/commands/__init__.py
--rw-r--r--   0        0        0      851 2023-06-21 03:21:27.774808 afkode-0.4.2/afkode/commands/keyword_search.py
--rw-r--r--   0        0        0      787 2023-07-15 18:02:04.861498 afkode-0.4.2/afkode/commands/list_actions.py
--rw-r--r--   0        0        0      852 2023-06-25 23:33:27.163337 afkode-0.4.2/afkode/commands/send_latest_agent_response_to_notes.py
--rw-r--r--   0        0        0      743 2023-06-25 23:13:10.479208 afkode-0.4.2/afkode/commands/send_latest_transcription_to_chat.py
--rw-r--r--   0        0        0      815 2023-06-25 23:33:27.165415 afkode-0.4.2/afkode/commands/send_latest_transcription_to_notes.py
--rw-r--r--   0        0        0      860 2023-06-21 13:07:35.314109 afkode-0.4.2/afkode/commands/suggest_program_actions.py
--rw-r--r--   0        0        0      994 2023-06-21 13:07:42.728505 afkode-0.4.2/afkode/commands/suggest_program_functionality.py
--rw-r--r--   0        0        0      987 2023-06-21 13:07:49.312156 afkode-0.4.2/afkode/commands/suggest_program_improvements.py
--rw-r--r--   0        0        0      984 2023-06-21 13:07:55.363573 afkode-0.4.2/afkode/commands/suggest_program_tests.py
--rw-r--r--   0        0        0      995 2023-07-15 20:48:15.588393 afkode-0.4.2/afkode/commands/summarize_filename.py
--rw-r--r--   0        0        0     1195 2023-06-21 03:21:24.718527 afkode-0.4.2/afkode/commands/summarize_today.py
--rw-r--r--   0        0        0      148 2023-07-15 20:48:15.589670 afkode-0.4.2/afkode/config.json
--rw-r--r--   0        0        0      306 2023-07-15 20:48:15.590843 afkode-0.4.2/afkode/globals.py
--rw-r--r--   0        0        0       81 2023-06-16 03:57:46.432139 afkode-0.4.2/afkode/ios/__init__.py
--rw-r--r--   0        0        0     2263 2023-06-21 02:39:58.258537 afkode-0.4.2/afkode/ios/listen.py
--rw-r--r--   0        0        0      938 2023-07-15 18:02:04.862367 afkode-0.4.2/afkode/ios/speech.py
--rw-r--r--   0        0        0       81 2023-06-16 03:57:46.435013 afkode-0.4.2/afkode/macos/__init__.py
--rw-r--r--   0        0        0     3586 2023-06-16 03:57:46.435646 afkode-0.4.2/afkode/macos/blip.wav
--rw-r--r--   0        0        0     2980 2023-06-21 02:39:58.268584 afkode-0.4.2/afkode/macos/listen.py
--rw-r--r--   0        0        0     3409 2023-07-15 18:02:04.862884 afkode-0.4.2/afkode/macos/speech.py
--rw-r--r--   0        0        0     3286 2023-06-21 12:47:08.277479 afkode-0.4.2/afkode/meta.py
--rw-r--r--   0        0        0     1545 2023-06-21 02:50:43.079156 afkode-0.4.2/afkode/prompts/debug/nox_tests.txt
--rw-r--r--   0        0        0      662 2023-06-16 22:59:22.394673 afkode-0.4.2/afkode/prompts/debug/program_actions.txt
--rw-r--r--   0        0        0      608 2023-06-21 12:36:52.717280 afkode-0.4.2/afkode/prompts/debug/program_functionality.txt
--rw-r--r--   0        0        0     1191 2023-06-21 12:35:20.610391 afkode-0.4.2/afkode/prompts/debug/program_improvements.txt
--rw-r--r--   0        0        0      634 2023-06-21 12:37:35.441216 afkode-0.4.2/afkode/prompts/debug/program_tests.txt
--rw-r--r--   0        0        0      326 2023-07-15 20:48:15.591524 afkode-0.4.2/afkode/prompts/debug/whisper_hallucinations.txt
--rw-r--r--   0        0        0     1404 2023-06-21 12:33:00.785694 afkode-0.4.2/afkode/prompts/programflow/choose_command.txt
--rw-r--r--   0        0        0      916 2023-06-20 00:21:10.454010 afkode-0.4.2/afkode/prompts/programflow/harmonize_transcripts.txt
--rw-r--r--   0        0        0      777 2023-06-11 19:45:59.626257 afkode-0.4.2/afkode/prompts/programflow/proposed_filename.txt
--rw-r--r--   0        0        0     1738 2023-06-20 00:21:10.457910 afkode-0.4.2/afkode/prompts/programflow/user_input_assist.txt
--rw-r--r--   0        0        0     2231 2023-07-15 20:48:15.592550 afkode-0.4.2/afkode/run.py
--rw-r--r--   0        0        0      639 2023-07-15 20:48:15.593284 afkode-0.4.2/afkode/set_env.py
--rw-r--r--   0        0        0     8574 2023-07-15 20:48:15.594326 afkode-0.4.2/afkode/utils.py
--rw-r--r--   0        0        0     8186 2023-07-15 20:48:15.595431 afkode-0.4.2/afkode/voice_interface.py
--rw-r--r--   0        0        0     3320 2023-07-15 21:45:22.167330 afkode-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8414 2023-07-15 21:53:03.751136 afkode-0.4.2/setup.py
--rw-r--r--   0        0        0     9024 2023-07-15 21:53:03.752068 afkode-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-07-15 22:05:21.061208 afkode-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6407 2023-07-15 22:05:21.061208 afkode-0.4.3/README.md
+-rw-r--r--   0        0        0      446 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/__init__.py
+-rw-r--r--   0        0        0     2896 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/action.py
+-rw-r--r--   0        0        0     5747 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/api.py
+-rw-r--r--   0        0        0      834 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/0_template.py
+-rw-r--r--   0        0        0       81 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/keyword_search.py
+-rw-r--r--   0        0        0      787 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/list_actions.py
+-rw-r--r--   0        0        0      852 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/send_latest_agent_response_to_notes.py
+-rw-r--r--   0        0        0      743 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/send_latest_transcription_to_chat.py
+-rw-r--r--   0        0        0      815 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/send_latest_transcription_to_notes.py
+-rw-r--r--   0        0        0      860 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_actions.py
+-rw-r--r--   0        0        0      994 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_functionality.py
+-rw-r--r--   0        0        0      987 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_improvements.py
+-rw-r--r--   0        0        0      984 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/suggest_program_tests.py
+-rw-r--r--   0        0        0      995 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/summarize_filename.py
+-rw-r--r--   0        0        0     1195 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/commands/summarize_today.py
+-rw-r--r--   0        0        0      148 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/config.json
+-rw-r--r--   0        0        0      306 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/globals.py
+-rw-r--r--   0        0        0       81 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/ios/__init__.py
+-rw-r--r--   0        0        0     2263 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/ios/listen.py
+-rw-r--r--   0        0        0      938 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/ios/speech.py
+-rw-r--r--   0        0        0       81 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/__init__.py
+-rw-r--r--   0        0        0     3586 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/blip.wav
+-rw-r--r--   0        0        0     2980 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/listen.py
+-rw-r--r--   0        0        0     3409 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/macos/speech.py
+-rw-r--r--   0        0        0     3286 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/meta.py
+-rw-r--r--   0        0        0     1545 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/nox_tests.txt
+-rw-r--r--   0        0        0      662 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_actions.txt
+-rw-r--r--   0        0        0      608 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_functionality.txt
+-rw-r--r--   0        0        0     1191 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_improvements.txt
+-rw-r--r--   0        0        0      634 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/program_tests.txt
+-rw-r--r--   0        0        0      326 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/debug/whisper_hallucinations.txt
+-rw-r--r--   0        0        0     1404 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/choose_command.txt
+-rw-r--r--   0        0        0      916 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/harmonize_transcripts.txt
+-rw-r--r--   0        0        0      777 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/proposed_filename.txt
+-rw-r--r--   0        0        0     1738 2023-07-15 22:05:21.061208 afkode-0.4.3/afkode/prompts/programflow/user_input_assist.txt
+-rw-r--r--   0        0        0     2231 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/run.py
+-rw-r--r--   0        0        0      639 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/set_env.py
+-rw-r--r--   0        0        0     8574 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/utils.py
+-rw-r--r--   0        0        0     8186 2023-07-15 22:05:21.065209 afkode-0.4.3/afkode/voice_interface.py
+-rw-r--r--   0        0        0     3320 2023-07-15 22:05:21.065209 afkode-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8414 2023-07-15 22:07:34.093763 afkode-0.4.3/setup.py
+-rw-r--r--   0        0        0     9024 2023-07-15 22:07:34.095024 afkode-0.4.3/PKG-INFO
```

### Comparing `afkode-0.4.2/README.md` & `afkode-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/action.py` & `afkode-0.4.3/afkode/action.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/api.py` & `afkode-0.4.3/afkode/api.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/0_template.py` & `afkode-0.4.3/afkode/commands/0_template.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/keyword_search.py` & `afkode-0.4.3/afkode/commands/keyword_search.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/list_actions.py` & `afkode-0.4.3/afkode/commands/list_actions.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/send_latest_agent_response_to_notes.py` & `afkode-0.4.3/afkode/commands/send_latest_agent_response_to_notes.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/send_latest_transcription_to_chat.py` & `afkode-0.4.3/afkode/commands/send_latest_transcription_to_chat.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/send_latest_transcription_to_notes.py` & `afkode-0.4.3/afkode/commands/send_latest_transcription_to_notes.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/suggest_program_actions.py` & `afkode-0.4.3/afkode/commands/suggest_program_actions.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/suggest_program_functionality.py` & `afkode-0.4.3/afkode/commands/suggest_program_functionality.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/suggest_program_improvements.py` & `afkode-0.4.3/afkode/commands/suggest_program_improvements.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/suggest_program_tests.py` & `afkode-0.4.3/afkode/commands/suggest_program_tests.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/summarize_filename.py` & `afkode-0.4.3/afkode/commands/summarize_filename.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/commands/summarize_today.py` & `afkode-0.4.3/afkode/commands/summarize_today.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/ios/listen.py` & `afkode-0.4.3/afkode/ios/listen.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/ios/speech.py` & `afkode-0.4.3/afkode/ios/speech.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/macos/blip.wav` & `afkode-0.4.3/afkode/macos/blip.wav`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/macos/listen.py` & `afkode-0.4.3/afkode/macos/listen.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/macos/speech.py` & `afkode-0.4.3/afkode/macos/speech.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/meta.py` & `afkode-0.4.3/afkode/meta.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/debug/nox_tests.txt` & `afkode-0.4.3/afkode/prompts/debug/nox_tests.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/debug/program_actions.txt` & `afkode-0.4.3/afkode/prompts/debug/program_actions.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/debug/program_functionality.txt` & `afkode-0.4.3/afkode/prompts/debug/program_functionality.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/debug/program_improvements.txt` & `afkode-0.4.3/afkode/prompts/debug/program_improvements.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/debug/program_tests.txt` & `afkode-0.4.3/afkode/prompts/debug/program_tests.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/programflow/choose_command.txt` & `afkode-0.4.3/afkode/prompts/programflow/choose_command.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/programflow/harmonize_transcripts.txt` & `afkode-0.4.3/afkode/prompts/programflow/harmonize_transcripts.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/programflow/proposed_filename.txt` & `afkode-0.4.3/afkode/prompts/programflow/proposed_filename.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/prompts/programflow/user_input_assist.txt` & `afkode-0.4.3/afkode/prompts/programflow/user_input_assist.txt`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/run.py` & `afkode-0.4.3/afkode/run.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/set_env.py` & `afkode-0.4.3/afkode/set_env.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/utils.py` & `afkode-0.4.3/afkode/utils.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/afkode/voice_interface.py` & `afkode-0.4.3/afkode/voice_interface.py`

 * *Files identical despite different names*

### Comparing `afkode-0.4.2/pyproject.toml` & `afkode-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "afkode"
-version = "0.4.2"
+version = "0.4.3"
 description = "Personal voice command interface for iPhone on pythonista powered by Whisper and ChatGPT."
 license = "MIT"
 authors = ["Nick Jenkins"]
 readme = "README.md"
 homepage = "https://www.ndjenkins.com/"
 repository = "https://github.com/ndjenkins85/afkode/"
 documentation = "https://ndjenkins85.github.io/afkode/"
```

### Comparing `afkode-0.4.2/setup.py` & `afkode-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
            'pytest-cov>=3.0,<4.0']}
 
 entry_points = \
 {'console_scripts': ['afkode = afkode.run:start']}
 
 setup_kwargs = {
     'name': 'afkode',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'Personal voice command interface for iPhone on pythonista powered by Whisper and ChatGPT.',
     'long_description': '# AFKode - Speak it, Save it, AFKode it!\n\nAFKode allows users to interact with AI and file system using only voice, allowing you to work away from keyboard.\nWorks on iPhone with pythonista, or on MacOS.\nPowered by Whisper and ChatGPT.\n\nThis project was inspired by long walks on the beach while ruminating and organizing ones thoughts.\n\nUsers of this program should be comfortable using pythonista/python.\nYou are required to BYO OpenAI secret key in variable `OPENAI_KEY` using environment variables or within `afkcode/secrets.py`.\n\nKey features:\n\n- Detection of start/stop dictation for transcription\n- Uses ChatGPT create smart file naming for your notes\n\nInterfaces:\n\n* At home: Supports MacOS with base speakers/microphone or AirPods. May not work with other bluetooth headsets like Bose headphones.\n* Out and about: Supports Pythonista iOS with base speakers/microphones, or plugged in lightning wired heaphones. Bluetooth headsets like AirPods and Bose headphones currently not working.\n\n## Contents\n\n* [Instructions for users](#instructions-for-users)\n  * [Installation](#installation)\n  * [Usage documentation](#usage-documentation)\n  * [Bug reports](#bug-reports)\n* [Instructions for developers](#instructions-for-developers)\n  * [Poetry](#environment-1-poetry)\n  * [Testing with Nox](#testing-with-nox)\n  * [Code formatting with Pre-commit](#code-formatting-with-pre-commit)\n* [Contributors](#contributors)\n\n## Instructions for users\n\nThe following are the quick start instructions for using the project as an end-user.\n\nFollow the [Instructions for developers](#instructions-for-developers) to set up the virtual environment and dependency management.\n\n### Installation\n\nMacOS requirements:\n\n- Python 3.8\n- ffmpeg for mp3 text-to-speech, `brew install ffmpeg`\n\n\nNote: Instructions marked with %% are not functioning and are for demo purposes only.\n\nInstall the project using pip %%:\n\n```bash\npip install afkode\n```\n\nTo replicate the data transformations and model results, run the following commands from the project root.\nThese should be run from the `poetry shell`, or `conda` environment, or with the `poetry run` prefix.\n```bash\npython -m afkode.run\n```\n\n### Usage documentation\n\nThe user guides can be found on [github pages](https://ndjenkins85.github.io/afkode).\nThis includes overview of features, discussion of `afkode` framework, and API reference.\n\n### Bug reports\n\nPlease raise an [issue](https://github.com/ndjenkins85/afkode/issues) with `bug` label and I will look into it!\n\n## Instructions for developers\n\nThe following are the setup instructions for developers looking to improve this project.\nFor information on current contributors and guidelines see the [contributors](#contributors) section.\nFollow each step here and ensure tests are working.\n\n### Poetry\n\n[Poetry](https://python-poetry.org/docs/) handles virtual environment management, dev and optional extra libraries, library development, builds and publishing.\n\nCheck the poetry website for the latest instructions on how to install poetry.\nYou can use the following command on OS/linux to install poetry 1.1.9 used in this project.\n\n```bash\ncurl -sSL https://install.python-poetry.org | python - --version 1.1.9\n```\n\nIt is recommended to set virtual environment creation to within project using the following command.\nThis adds a `.venv` directory to project to handle cache and virtual environment.\n```bash\npoetry config virtualenvs.in-project true\n```\n\nYou can set up the virtual environment in the repo using the following command.\nMake sure that any other virtual environments (i.e. `conda deactivate`) are deactivated before running.\n\n```bash\npoetry install\n```\n\nTroubleshooting: You may need to point poetry to the correct python interpreter using the following command.\nIn another terminal and in conda, run `which python`.\n```bash\npoetry env use /path/to/python3\n```\n\nWhen the environment is correctly installed, you can enter the virtual environment using `poetry shell`. Library can be built using `poetry build`.\n\n### Testing with Nox\n\n[Nox](https://nox.thea.codes/en/stable/index.html) is a command-line tool that automates testing in multiple Python environments, similar to tox, Makefiles or scripts. Unlike tox, Nox uses a standard Python file for configuration.\n\nHere it is used for code quality, testing, and generating documentation.\n\nThe following command can be used to run mypy, lint, and tests.\nIt is recommended to run these before pushing code, as this is run with Github Actions.\nSome checks such as black are run more frequently with [pre-commit](#code-formatting-with-pre-commit).\n\n```bash\npoetry run nox\n```\n\nLocal Sphinx documentation can be generated with the following command.\nDocumentation publishing using Github Actions to Github pages is enabled by default.\n\n```bash\npoetry run nox -s docs\n```\n\nOther available commands include:\n\n```bash\npoetry run nox -rs coverage\n```\n\n### Code formatting with Pre-commit\n\n[Pre-commit](https://pre-commit.com/) is a framework for managing and maintaining multi-language pre-commit hooks.\n\nIt intercepts the `git commit` command to run checks of staged code before the commit is finalized.\nThe checks are specified in `.pre-commit-config.yaml`.\nChecks in use are quick, pragmatic, and apply automatic formatting checks.\nIf checks fail, it is usually only a matter of re-staging the files (`git add`) and attempting to commit again.\n\nThe aim is to provide a lightweight way to keep some code standards automatically in line with standards.\nThis does not replace the need to run nox tests, although pre-commits will satisfy some of the nox test checks.\n\nOn first time use of the repository, pre-commit will need to be installed locally.\nYou will need to be in the `poetry shell` or `conda` environment.\nRun the following command to perform a first time install.\n\n```bash\npre-commit install\n```\n\nThis will cache several code assets used in the checks.\n\nWhen you have new code to commit, pre-commit will kick in and check the code.\nAlternatively, you can run the following command to run for all files in repo.\n\n``` bash\npre-commit run --all-files\n```\n\n## Contributors\n\n* [Nick Jenkins](https://www.ndjenkins.com) - Data Scientist, API & Web dev, Team lead, Writer\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) in Github repo for specific instructions on contributing to project.\n\nUsage rights governed by [LICENSE](LICENSE)  in Github repo or page footer.\n',
     'author': 'Nick Jenkins',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.ndjenkins.com/',
```

### Comparing `afkode-0.4.2/PKG-INFO` & `afkode-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afkode
-Version: 0.4.2
+Version: 0.4.3
 Summary: Personal voice command interface for iPhone on pythonista powered by Whisper and ChatGPT.
 Home-page: https://www.ndjenkins.com/
 License: MIT
 Keywords: quick_start,python_packaging,whisper,chatgpt,openai
 Author: Nick Jenkins
 Requires-Python: >=3.8.1,<3.9
 Classifier: Development Status :: 4 - Beta
```

