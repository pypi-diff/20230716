# Comparing `tmp/chai-guanaco-1.0.4.tar.gz` & `tmp/chai-guanaco-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.0.4.tar", last modified: Thu Jul  6 23:24:57 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.0.5.tar", last modified: Sun Jul 16 03:02:49 2023, max compression
```

## Comparing `chai-guanaco-1.0.4.tar` & `chai-guanaco-1.0.5.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/
--rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-06 21:45:32.000000 chai-guanaco-1.0.4/MANIFEST.in
--rw-rw-r--   0 tom       (1002) tom       (1002)    10662 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     8968 2023-07-06 23:24:38.000000 chai-guanaco-1.0.4/README.md
--rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/requirements.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-07-06 23:24:48.000000 chai-guanaco-1.0.4/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)      224 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-06 19:37:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/formatters.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/src/chai_guanaco/login_cli.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/
--rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/blade.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/captain_wyatt.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/filbert.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/leo.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/levi.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/mr_wilson.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/nerd_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/scaramouche.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/story_teller.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/vampire_queen.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/wednesday_addams.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/src/chai_guanaco/submit.py
--rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/src/chai_guanaco/utils.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)    10662 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     1254 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/tests/
--rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-06 21:05:17.000000 chai-guanaco-1.0.4/tests/test_chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.4/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/tests/test_login.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/tests/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/
+-rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/MANIFEST.in
+-rw-rw-r--   0 tom       (1002) tom       (1002)    11015 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     9305 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/README.md
+-rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/requirements.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/setup.cfg
+-rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-07-16 03:02:45.000000 chai-guanaco-1.0.5/setup.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco/
+-rw-rw-r--   0 tom       (1002) tom       (1002)      270 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3259 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/formatters.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/login_cli.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     5249 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/src/chai_guanaco/metrics.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-15 21:49:57.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/blade.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-15 21:49:57.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/captain_wyatt.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/filbert.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-15 21:49:57.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/leo.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/levi.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/mr_wilson.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/nerd_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/scaramouche.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/story_teller.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/vampire_queen.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/wednesday_addams.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     5426 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/src/chai_guanaco/submit.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1894 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/src/chai_guanaco/utils.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/
+-rw-rw-r--   0 tom       (1002) tom       (1002)    11015 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1430 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/tests/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/tests/resources/
+-rw-rw-r--   0 tom       (1002) tom       (1002) 10541478 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/tests/resources/test_get_leaderboard.yaml
+-rw-rw-r--   0 tom       (1002) tom       (1002)  9300316 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/tests/resources/test_get_submission_metrics.yaml
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/tests/test_chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.5/tests/test_feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1629 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/tests/test_guanaco_python_utils.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/tests/test_login.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3716 2023-07-16 02:17:04.000000 chai-guanaco-1.0.5/tests/test_metrics.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     5607 2023-07-16 02:17:04.000000 chai-guanaco-1.0.5/tests/test_submit.py
```

### Comparing `chai-guanaco-1.0.4/PKG-INFO` & `chai-guanaco-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.4
+Version: 1.0.5
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -73,15 +73,15 @@
         To submit model simply run:
         
         ```python
         import chai_guanaco as chai
         
         model_url = "EleutherAI/gpt-j-6b" # Your model URL
         
-        generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0, "top_k": 0}
+        generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0.2, "top_k": 40, "stopping_words": ['\n']}
         submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
         
         submitter = chai.ModelSubmitter()
         submission_id = submitter.submit(submission_parameters)
         ````
         
         This will display an animation while your model is being deployed, a typical
@@ -131,17 +131,17 @@
         
         This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
         
         **Getting Live Leaderboard**
         
         To see how your model performs against other models, run:
         ```python
-        chai.display_leaderboard()
+        df = chai.display_leaderboard()
         ```
-        which prints out the current leaderboard, with your models positions highlighted
+        which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
         
         **Re-Submitting Models**
         
         Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
         
         ```python
         chai.deactivate_model(submission_id)
@@ -161,14 +161,16 @@
         **Advanced Usage**
         - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
         - You can also access the raw feedback data by running
         	```python
         	model_feedback = chai.get_feedback(submission_id)
         	raw_data = model_feedback.raw_data
         	```
+        - To submit your model with custom formatting, you can create your own
+          `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
         
         
         
         ## Resources
         |                                                                        |                                                                                                 |
         | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
         | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
```

### Comparing `chai-guanaco-1.0.4/README.md` & `chai-guanaco-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 To submit model simply run:
 
 ```python
 import chai_guanaco as chai
 
 model_url = "EleutherAI/gpt-j-6b" # Your model URL
 
-generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0, "top_k": 0}
+generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0.2, "top_k": 40, "stopping_words": ['\n']}
 submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
 
 submitter = chai.ModelSubmitter()
 submission_id = submitter.submit(submission_parameters)
 ````
 
 This will display an animation while your model is being deployed, a typical
@@ -123,17 +123,17 @@
 
 This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
 
 **Getting Live Leaderboard**
 
 To see how your model performs against other models, run:
 ```python
-chai.display_leaderboard()
+df = chai.display_leaderboard()
 ```
-which prints out the current leaderboard, with your models positions highlighted
+which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
 
 **Re-Submitting Models**
 
 Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
 
 ```python
 chai.deactivate_model(submission_id)
@@ -153,14 +153,16 @@
 **Advanced Usage**
 - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
 - You can also access the raw feedback data by running
 	```python
 	model_feedback = chai.get_feedback(submission_id)
 	raw_data = model_feedback.raw_data
 	```
+- To submit your model with custom formatting, you can create your own
+  `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
 
 
 
 ## Resources
 |                                                                        |                                                                                                 |
 | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
 | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
```

### Comparing `chai-guanaco-1.0.4/setup.py` & `chai-guanaco-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.0.4"
+    version = "1.0.5"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
```

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/chat.py` & `chai-guanaco-1.0.5/src/chai_guanaco/chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/feedback.py` & `chai-guanaco-1.0.5/src/chai_guanaco/feedback.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from chai_guanaco.utils import print_color
 from chai_guanaco.login_cli import auto_authenticate
 
 
 BASE_URL = "https://guanaco-feedback.chai-research.com"
 FEEDBACK_ENDPOINT = "/feedback/{submission_id}"
 
-FEEDBACK_URL = BASE_URL + FEEDBACK_ENDPOINT
+
+def get_url(endpoint):
+    return BASE_URL + endpoint
 
 
 class Feedback():
     def __init__(self, raw_data):
         self.raw_data = raw_data
 
     @property
@@ -84,12 +86,13 @@
 
 
 @auto_authenticate
 def get_feedback(submission_id: str, developer_key=None):
     headers = {
         "developer_key": developer_key,
     }
-    url = FEEDBACK_URL.format(submission_id=submission_id)
+    url = get_url(FEEDBACK_ENDPOINT)
+    url = url.format(submission_id=submission_id)
     resp = requests.get(url, headers=headers)
     assert resp.status_code == 200, resp.json()
     feedback = Feedback(resp.json())
     return feedback
```

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/formatters.py` & `chai-guanaco-1.0.5/src/chai_guanaco/formatters.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/login_cli.py` & `chai-guanaco-1.0.5/src/chai_guanaco/login_cli.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/blade.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/blade.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/captain_wyatt.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/captain_wyatt.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/filbert.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/filbert.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/leo.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/leo.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/levi.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/levi.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/mr_wilson.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/mr_wilson.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/nerd_girl.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/nerd_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/scaramouche.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/scaramouche.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/story_teller.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/story_teller.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/vampire_queen.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/vampire_queen.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/wednesday_addams.json` & `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/wednesday_addams.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.0.5/src/chai_guanaco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.4
+Version: 1.0.5
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -73,15 +73,15 @@
         To submit model simply run:
         
         ```python
         import chai_guanaco as chai
         
         model_url = "EleutherAI/gpt-j-6b" # Your model URL
         
-        generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0, "top_k": 0}
+        generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0.2, "top_k": 40, "stopping_words": ['\n']}
         submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
         
         submitter = chai.ModelSubmitter()
         submission_id = submitter.submit(submission_parameters)
         ````
         
         This will display an animation while your model is being deployed, a typical
@@ -131,17 +131,17 @@
         
         This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
         
         **Getting Live Leaderboard**
         
         To see how your model performs against other models, run:
         ```python
-        chai.display_leaderboard()
+        df = chai.display_leaderboard()
         ```
-        which prints out the current leaderboard, with your models positions highlighted
+        which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
         
         **Re-Submitting Models**
         
         Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
         
         ```python
         chai.deactivate_model(submission_id)
@@ -161,14 +161,16 @@
         **Advanced Usage**
         - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
         - You can also access the raw feedback data by running
         	```python
         	model_feedback = chai.get_feedback(submission_id)
         	raw_data = model_feedback.raw_data
         	```
+        - To submit your model with custom formatting, you can create your own
+          `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
         
         
         
         ## Resources
         |                                                                        |                                                                                                 |
         | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
         | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
```

### Comparing `chai-guanaco-1.0.4/src/chai_guanaco.egg-info/SOURCES.txt` & `chai-guanaco-1.0.5/src/chai_guanaco.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 requirements.txt
 setup.py
 src/chai_guanaco/__init__.py
 src/chai_guanaco/chat.py
 src/chai_guanaco/feedback.py
 src/chai_guanaco/formatters.py
 src/chai_guanaco/login_cli.py
+src/chai_guanaco/metrics.py
 src/chai_guanaco/submit.py
 src/chai_guanaco/utils.py
 src/chai_guanaco.egg-info/PKG-INFO
 src/chai_guanaco.egg-info/SOURCES.txt
 src/chai_guanaco.egg-info/dependency_links.txt
 src/chai_guanaco.egg-info/entry_points.txt
 src/chai_guanaco.egg-info/not-zip-safe
@@ -26,9 +27,13 @@
 src/chai_guanaco/resources/bot_config/nerd_girl.json
 src/chai_guanaco/resources/bot_config/scaramouche.json
 src/chai_guanaco/resources/bot_config/story_teller.json
 src/chai_guanaco/resources/bot_config/vampire_queen.json
 src/chai_guanaco/resources/bot_config/wednesday_addams.json
 tests/test_chat.py
 tests/test_feedback.py
+tests/test_guanaco_python_utils.py
 tests/test_login.py
-tests/test_submit.py
+tests/test_metrics.py
+tests/test_submit.py
+tests/resources/test_get_leaderboard.yaml
+tests/resources/test_get_submission_metrics.yaml
```

### Comparing `chai-guanaco-1.0.4/tests/test_chat.py` & `chai-guanaco-1.0.5/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/tests/test_feedback.py` & `chai-guanaco-1.0.5/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/tests/test_login.py` & `chai-guanaco-1.0.5/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.4/tests/test_submit.py` & `chai-guanaco-1.0.5/tests/test_submit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from mock import patch
 
 import pytest
+import pandas as pd
 
-from chai_guanaco import submit
+from chai_guanaco import submit, formatters
 
 
 @pytest.fixture(autouse="session")
 def mock_post():
     with patch("chai_guanaco.submit.requests.post") as func:
         func.return_value.status_code = 200
         func.return_value.json.return_value = {"submission_id": "name_123456"}
@@ -35,41 +36,55 @@
     submission = {
         "model_repo": "ChaiML/test_model",
         "generation_params": {
             "temperature": 1.0,
             "top_p": 1.0,
             "top_k": 40,
             "repetition_penalty": 1.0,
+            "stopping_words": ["\n"],
         },
-        "formatter": "PygmalionFormatter",
+        "formatter": formatters.PygmalionFormatter().dict(),
     }
     return submission
 
 
 def test_model_submitter(mock_submission, mock_post, mock_get_pending_to_success):
     model_submitter = submit.ModelSubmitter("mock-key")
     model_submitter._sleep_time = 0
     model_submitter._get_request_interval = 1
-    submission_id = model_submitter.submit(mock_submission)
+    model_submitter_params = {
+        "model_repo": "ChaiML/test_model",
+        "generation_params": {
+            "temperature": 1.0,
+            "top_p": 1.0,
+            "top_k": 40,
+            "repetition_penalty": 1.0,
+            "stopping_words": ["\n"],
+        },
+        "formatter": formatters.PygmalionFormatter(),
+    }
+    submission_id = model_submitter.submit(model_submitter_params)
     headers = {"Authorization": "Bearer mock-key"}
-    mock_post.assert_called_once_with(url=submit.SUBMISSION_URL, json=mock_submission, headers=headers)
+    expected_url = submit.get_url(submit.SUBMISSION_ENDPOINT)
+    mock_post.assert_called_once_with(url=expected_url, json=mock_submission, headers=headers)
     assert mock_get_pending_to_success.call_count == 3
     assert submission_id == "name_123456"
 
 
 def test_client(mock_post, mock_submission):
     response = submit.submit_model(mock_submission, developer_key="mock-key")
     expected_submission_id = "name_123456"
     assert response == {"submission_id": expected_submission_id}
 
 
 def test_submit_client_posts_with_correct_payload(mock_post, mock_submission):
     submit.submit_model(mock_submission, developer_key="mock-key")
     headers={"Authorization": "Bearer mock-key"}
-    mock_post.assert_called_once_with(url=submit.SUBMISSION_URL, json=mock_submission, headers=headers)
+    expected_url = submit.get_url(submit.SUBMISSION_ENDPOINT)
+    mock_post.assert_called_once_with(url=expected_url, json=mock_submission, headers=headers)
 
 
 def test_submit_client_posts_raises_for_failed_post(mock_post, mock_submission):
     mock_post.return_value.status_code = 500
     mock_post.return_value.json.return_value = {'error': 'some error'}
     with pytest.raises(AssertionError) as e:
         submit.submit_model(mock_submission, developer_key="mock-key")
@@ -88,16 +103,17 @@
     response = submit.get_model_info('name_123456', developer_key='key')
     expected = {'name_123456': {'status': 'pending'}}
     assert expected == response
 
 
 def test_get_model_info_called_with_correct_url(mock_get):
     submit.get_model_info('name_123456', developer_key='key')
+    expected_url = submit.get_url(submit.INFO_ENDPOINT)
     mock_get.assert_called_once_with(
-        url=submit.INFO_URL.format(submission_id='name_123456'),
+        url=expected_url.format(submission_id='name_123456'),
         headers={"Authorization": "Bearer key"}
     )
 
 
 def test_get_model_info_raises_with_error(mock_get):
     mock_get.return_value.status_code = 500
     mock_get.return_value.json.return_value = {'error': 'some error'}
@@ -106,16 +122,17 @@
     msg = "some error"
     assert msg in str(e)
 
 
 def test_get_my_submissions(mock_get):
     mock_get.return_value.json.return_value = {'123': 'pending', '456': 'failed'}
     out = submit.get_my_submissions('dev_key')
+    expected_url = submit.get_url(submit.ALL_SUBMISSION_STATUS_ENDPOINT)
     mock_get.assert_called_once_with(
-        url=submit.MY_SUBMISSIONS_STATUS_URL,
+        url=expected_url,
         headers={"Authorization": "Bearer dev_key"}
     )
     assert out == {'123': 'pending', '456': 'failed'}
 
 
 def test_get_my_submissions_raises(mock_get):
     mock_get.return_value.status_code = 500
@@ -127,51 +144,10 @@
 
 
 def test_deactivate_model(mock_get):
     mock_get.return_value.status_code = 200
     mock_get.return_value.json.return_value = ""
     submit.deactivate_model("test_model", developer_key="dev_key")
     expected_headers = {"Authorization": "Bearer dev_key"}
-    expected_url = submit.DEACTIVATE_URL.format(submission_id = "test_model")
+    expected_url = submit.get_url(submit.DEACTIVATE_ENDPOINT)
+    expected_url = expected_url.format(submission_id = "test_model")
     mock_get.assert_called_once_with(url=expected_url, headers=expected_headers)
-
-
-def test_get_leaderboard(mock_get, mock_leaderboard):
-    mock_get.return_value.json.return_value = mock_leaderboard
-    output = submit.get_leaderboard(developer_key="key")
-    expected_headers = {"developer_key": "key"}
-    expected_url = "https://guanaco-submitter.chai-research.com/leaderboard"
-    mock_get.assert_called_once_with(expected_url, headers=expected_headers)
-    expected_output = {
-        "alekseykorshuk-pygmalion-6b-v0-lmg_1686855359": {
-            "thumbs_down": 131,
-            "thumbs_up": 594,
-            "ratio": 0.82,
-        },
-        "vicuna-13b-reward-triton": {
-            "thumbs_down": 70,
-            "thumbs_up": 230,
-            "ratio": 0.77,
-        },
-        "alekseykorshuk-pygmalion-6b-v1-eos_1686954501": {
-            "thumbs_down": 187,
-            "thumbs_up": 537,
-            "ratio": 0.74,
-        },
-    }
-    assert output == expected_output
-
-
-@pytest.fixture
-def mock_leaderboard():
-    feedback = {
-        "alekseykorshuk-pygmalion-6b-v0-lmg_1686855359": {
-            "thumbs_down": 131,
-            "thumbs_up": 594,
-        },
-        "alekseykorshuk-pygmalion-6b-v1-eos_1686954501": {
-            "thumbs_down": 187,
-            "thumbs_up": 537,
-        },
-        "vicuna-13b-reward-triton": {"thumbs_down": 70, "thumbs_up": 230},
-    }
-    return feedback
```

