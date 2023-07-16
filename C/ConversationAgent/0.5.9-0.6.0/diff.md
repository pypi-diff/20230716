# Comparing `tmp/ConversationAgent-0.5.9.tar.gz` & `tmp/ConversationAgent-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConversationAgent-0.5.9.tar", last modified: Sat Jun 24 13:13:34 2023, max compression
+gzip compressed data, was "ConversationAgent-0.6.0.tar", last modified: Sun Jul 16 12:56:11 2023, max compression
```

## Comparing `ConversationAgent-0.5.9.tar` & `ConversationAgent-0.6.0.tar`

### file list

```diff
@@ -1,53 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.426685 ConversationAgent-0.5.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.398685 ConversationAgent-0.5.9/ConversationAgent/
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/LibStage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/SentenceStage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/__agent__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/__stage__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/__tool__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.402685 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.414685 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)  6200957 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/idf.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/textrank.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4313 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)  4154486 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/dict.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.414685 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/finalseg/
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/finalseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   864307 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/finalseg/prob_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/finalseg/prob_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/finalseg/prob_trans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.422685 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1618015 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/char_state_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)  3987090 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/prob_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/prob_start.py
--rw-r--r--   0 runner    (1001) docker     (123)   247312 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/prob_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/viterbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/nlp_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.426685 ConversationAgent-0.5.9/ConversationAgent/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16488 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__test_v1__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__test_v2__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__test_v3__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__test_v4__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__test_v5__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__test_v6__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/ConversationAgent/test/__test_v7__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:13:34.398685 ConversationAgent-0.5.9/ConversationAgent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-24 13:13:34.000000 ConversationAgent-0.5.9/ConversationAgent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-24 13:13:34.000000 ConversationAgent-0.5.9/ConversationAgent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:13:34.000000 ConversationAgent-0.5.9/ConversationAgent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:13:34.000000 ConversationAgent-0.5.9/ConversationAgent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 13:13:34.000000 ConversationAgent-0.5.9/ConversationAgent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-24 13:13:34.426685 ConversationAgent-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 13:13:34.426685 ConversationAgent-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-24 13:13:23.000000 ConversationAgent-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.890474 ConversationAgent-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.866474 ConversationAgent-0.6.0/ConversationAgent/
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/LibStage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/__agent__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/__memory__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/__nlp_tool__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/__stage__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/__tool__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.870474 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.882474 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)  6200957 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/idf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/textrank.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4313 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4154486 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/dict.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.882474 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/finalseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/finalseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   864307 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/finalseg/prob_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/finalseg/prob_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/finalseg/prob_trans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.890474 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1618015 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/char_state_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)  3987090 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/prob_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/prob_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)   247312 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/prob_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/viterbi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.890474 ConversationAgent-0.6.0/ConversationAgent/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/types/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/types/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/ConversationAgent/types/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:56:11.870474 ConversationAgent-0.6.0/ConversationAgent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-16 12:56:11.000000 ConversationAgent-0.6.0/ConversationAgent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-16 12:56:11.000000 ConversationAgent-0.6.0/ConversationAgent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:56:11.000000 ConversationAgent-0.6.0/ConversationAgent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:56:11.000000 ConversationAgent-0.6.0/ConversationAgent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-16 12:56:11.000000 ConversationAgent-0.6.0/ConversationAgent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-16 12:56:11.890474 ConversationAgent-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:56:11.890474 ConversationAgent-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-16 12:56:01.000000 ConversationAgent-0.6.0/setup.py
```

### Comparing `ConversationAgent-0.5.9/ConversationAgent/LibStage.py` & `ConversationAgent-0.6.0/ConversationAgent/LibStage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
 from .__stage__ import Stage, __USER_TEXT__, StageType
 from .__agent__ import Agent, MultiAgent
 from .__tool__ import get_value_from_dict_by_multi_name, compute_by_string
 from .jieba_zh import analyse
 import re
 import random
+from typing import Dict, Any, List, Tuple
+from .__nlp_tool__ import similar_text_distance, SimilarResult
+from .__memory__ import StageMemoryFragOperation
+from .types.memory import Memory
+
 
 __RE_STAGE__ = "__RE_STAGE__"
 __QA_STAGE__ = "__QA_STAGE__"
 __Similarly_STAGE__ = "__Similarly_STAGE__"
 __SWITCH_STAGE__ = StageType.SWITCH
 __LIB_SWITCH_STAGE__ = "__LIB_SWITCH_STAGE__"
 __Classify_STAGE__ = "__Classify_STAGE__"
@@ -16,15 +22,15 @@
 __QUESTIONS_LABEL__ = ["__SYS_QUESTION__", "question", "says", "corpus"]
 __WELCOME_SAYING_LABELS__ = ["__SYS_WELCOME__", "sys_reply_q1", "sys_welcome"]
 __REFUSE_SAYING_LABELS__ = ["__SYS_REFUSE__", "sys_reply_q2", "sys_refuse"]
 __COMPLETE_SAYING_LABELS__ = ["__SYS_COMPLETE__", "sys_reply_complete", "sys_complete"]
 __DISABLE_WELCOME_LABEL__ = ["__DISABLE_WELCOME__", "__DISSABLE_Q1__", "DISSABLE_WELCOME"]
 __DISABLE_REFUSE_LABEL__ = ["__DISABLE_REFUSE__"]
 
-from .nlp_tool import similar
+
 
 
 class QAStage(Stage):
     __QA_RESPOND__ = ["__QA_RESPOND__"]
     __QA_RESPOND_SCORE__ = ["__QA_RESPOND_SCORE__"]
     __QA_RESPOND_QUESTION__ = ["__QA_RESPOND_QUESTION__"]
     __QA_RESPOND_THRESHOLD__ = ["__QA_RESPOND_THRESHOLD__"]
@@ -56,44 +62,48 @@
         self.saved_name: dict = data.get(self.__SAVED_NAME__, {})
         self.qa_threshold = data.get(self.__QA_THRESHOLD__, 0.1)
 
         # TODO: RENAME `refactor_questions` -> `refactor_corpus_questions`
         self.refactor_questions = data.get(self.__REFACTOR_QUESTION__, False)
 
         if get_value_from_dict_by_multi_name(d=data, names=__DISABLE_WELCOME_LABEL__, default=False):
-            self.is_first_access = self.disabel_is_first_access
+            # self.is_first_access = self.disabel_is_first_access
+          self.switch_welcome = False
 
         self.disable_refuse_question = get_value_from_dict_by_multi_name(d=data, names=__DISABLE_REFUSE_LABEL__,
                                                                          default=False)
 
-    def __request_similar_api__(self, text, corpus):
-        return similar(text, corpus)
+    def __request_similar_api__(self, text, corpus) -> SimilarResult:
+        return similar_text_distance(text, corpus)
 
     def __encode_corpus__(self):
         source_corpus = list(self.corpus.keys())
         dict_corpus = {self.__keyword__(self.__stop_word__(s)): s for s in source_corpus}
         return list(self.corpus.keys() if not self.refactor_questions else dict_corpus.keys()), dict_corpus
 
-    def __decode_corpus__(self, worker_response, new_dict_corpus):
-        best_res_content = str(worker_response[0][0])
+    def __decode_corpus__(self, worker_response: str, new_dict_corpus: Dict[str, Any]):
+        best_res_content = str(worker_response)
         if self.refactor_questions:
             best_res_content = new_dict_corpus[best_res_content] if best_res_content in new_dict_corpus else '0'
         return best_res_content
 
-    def is_fit_needs_n_gen_entity(self, kwargs) -> (bool, dict):
+    def is_fit_needs_n_gen_entity(self, kwargs) -> Tuple[bool, Memory]:
         user_text = kwargs.get(__USER_TEXT__, "")
-
+        
         corpus, new_dict_corpus = self.__encode_corpus__()
 
-        responds = self.__request_similar_api__(user_text, corpus)
-        worker_response = responds["worker response"]["ans"]
+
+        # print(f"user_text: {user_text}")
+        # print(f"corpus: {corpus}")
+        responds: SimilarResult = self.__request_similar_api__(user_text, corpus)
+        worker_response = responds.ans
         best_res_content = self.__decode_corpus__(worker_response, new_dict_corpus)
 
         ##
-        best_res_score = worker_response[0][1]
+        best_res_score = responds.score
         best_res_responds = self.corpus[best_res_content] if best_res_content in self.corpus else None
         if isinstance(best_res_responds,list):
             best_res_responds = random.choice(best_res_responds)
 
         ##
         __RUNNING_CORPUS__ = get_value_from_dict_by_multi_name(d=self.saved_name, names=self.__RUNNING_CORPUS__,
                                                                default=self.__RUNNING_CORPUS__[0])
@@ -108,33 +118,29 @@
                                                                  names=self.__QA_RESPOND_SCORE__,
                                                                  default=self.__QA_RESPOND_SCORE__[0])
         __QA_RESPOND_THRESHOLD__ = get_value_from_dict_by_multi_name(d=self.saved_name,
                                                                  names=self.__QA_RESPOND_THRESHOLD__,
                                                                  default=self.__QA_RESPOND_THRESHOLD__[0])
 
         #
-        kwargs = self.set_default_var(kwargs, __RUNNING_CORPUS__, corpus)
-        kwargs = self.set_default_var(kwargs, __QA_RESPOND__, best_res_responds)
-        kwargs = self.set_default_var(kwargs, __QA_RESPOND_QUESTION__, best_res_content)
-        kwargs = self.set_default_var(kwargs, __QA_RESPOND_SCORE__, best_res_score)
+        kwargs = StageMemoryFragOperation.set_default_frag(kwargs, __RUNNING_CORPUS__, corpus)
+        kwargs = StageMemoryFragOperation.set_default_frag(kwargs, __QA_RESPOND__, best_res_responds)
+        kwargs = StageMemoryFragOperation.set_default_frag(kwargs, __QA_RESPOND_QUESTION__, best_res_content)
+        kwargs = StageMemoryFragOperation.set_default_frag(kwargs, __QA_RESPOND_SCORE__, best_res_score)
         if best_res_score >= self.qa_threshold:
             pass_token = True
-            kwargs = self.set_default_var(kwargs, __QA_RESPOND_THRESHOLD__, True)
+            kwargs = StageMemoryFragOperation.set_default_frag(kwargs, __QA_RESPOND_THRESHOLD__, True)
         else:
             pass_token = False if self.disable_refuse_question is False else True
 
-            kwargs = self.set_default_var(kwargs, __QA_RESPOND_THRESHOLD__, False)
+            kwargs = StageMemoryFragOperation.set_default_frag(kwargs, __QA_RESPOND_THRESHOLD__, False)
 
         return pass_token, kwargs
 
     @staticmethod
-    def disabel_is_first_access(kwargs, stage_id):
-        return False
-
-    @staticmethod
     def __stop_word__(text, pronouns=True, common_skip=True, road_name=True, symbol=True):
         text = text.replace(" ", "")
         filter_set = []
         if pronouns:
             filter_set += ["我", "你", "妳"]
         if common_skip:
             filter_set += ["請問", "不好意思", "這裡", "可以", "要", "怎麼", "如何"]
@@ -169,48 +175,46 @@
         self.questions = get_value_from_dict_by_multi_name(d=data, names=__QUESTIONS_LABEL__)
         self.sys_reply_q1 = get_value_from_dict_by_multi_name(d=self.questions, names=__WELCOME_SAYING_LABELS__)
         self.sys_reply_q2 = get_value_from_dict_by_multi_name(d=self.questions, names=__REFUSE_SAYING_LABELS__)
         self.sys_reply_complete = get_value_from_dict_by_multi_name(d=self.questions,
                                                                     names=__COMPLETE_SAYING_LABELS__)
         self.is_fits = data.get("is_fits", [])
         if get_value_from_dict_by_multi_name(d=data, names=__DISABLE_WELCOME_LABEL__, default=False):
-            self.is_first_access = self.disabel_is_first_access
+            # self.is_first_access = self.disabel_is_first_access
+            self.switch_welcome = False
 
         self.disable_refuse_question = get_value_from_dict_by_multi_name(d=data, names=__DISABLE_REFUSE_LABEL__,
                                                                          default=False)
 
-    @staticmethod
-    def disabel_is_first_access(kwargs, stage_id):
-        return False
 
     @staticmethod
     def __get_entity__(rule, text):
         entities = []
         results = re.findall(rule, text)
         for r in results:
             if isinstance(r, tuple):
                 entities += list(r)
             else:
                 entities.append(r)
         return entities
 
-    def is_fit_needs_n_gen_entity(self, kwargs) -> (bool, dict):
+    def is_fit_needs_n_gen_entity(self, kwargs) -> Tuple[bool, dict]:
         user_text = kwargs.get(__USER_TEXT__, "")
         pass_token = True
 
         missing_entities = []
         for (rule, entity_name) in self.is_fits:
             entities = self.__get_entity__(rule, user_text)
             if len(entities) > 0:
-                kwargs = self.set_default_var(kwargs, entity_name, " ".join(entities))
+                kwargs = StageMemoryFragOperation. set_default_frag(kwargs, entity_name, " ".join(entities))
             else:
                 missing_entities.append(entity_name)
 
         for entity_name in missing_entities:
-            if self.get_default_var(kwargs, entity_name) is None:
+            if StageMemoryFragOperation. get_default_frag(kwargs, entity_name) is None:
                 pass_token = False
 
         if self.disable_refuse_question:
             pass_token = True
 
         return pass_token, kwargs
 
@@ -260,23 +264,23 @@
             #
             assert len(symbol) == len(
                 text), f"變數比較條件與限定結果的數量不一致len(symbol) == len(text): {symbol},{text}"
 
             #
             pass_token = True
             for l, s, t in zip(label, symbol, text):
-                l_var = self.get_default_var(kwargs, l)
+                l_var = StageMemoryFragOperation. get_default_frag(kwargs, l)
                 pass_token = compute_by_string(l_var, s, t)
 
             if pass_token:
                 return stages_label
 
         raise RuntimeError(f"Not Found Path: {stages_searched}")
 
-    def is_fit_needs_n_gen_entity(self, kwargs) -> (bool, dict):
+    def is_fit_needs_n_gen_entity(self, kwargs) -> Tuple[bool, dict]:
         raise RuntimeError
 
 
 class SimilarlyStage(QAStage):
     pass
 
 
@@ -303,38 +307,38 @@
         return re_dict
 
     def __init__(self, data):
         super().__init__(data)
         self.__Classify_THRESHOLD__ = data.get(self.__Classify_THRESHOLD__, 0.5)
         self.__SAVED_NAME__ = data.get("__SAVED_NAME__", {})
 
-    def is_fit_needs_n_gen_entity(self, kwargs) -> (bool, dict):
+    def is_fit_needs_n_gen_entity(self, kwargs) -> Tuple[bool, dict]:
 
         user_text = kwargs.get(__USER_TEXT__, "")
         pass_token = False
 
         classify_values_dict = self.get_classify_text(text=user_text, rules=self.is_fits)
         for entity_name, value in classify_values_dict.items():
             if value >= self.__Classify_THRESHOLD__:
                 pass_token = True
-            kwargs = self.set_default_var(kwargs, entity_name, value)
+            kwargs = StageMemoryFragOperation. set_default_frag(kwargs, entity_name, value)
 
         # Save
         __LABEL_SAVE_Classify_THRESHOLD__ = self.__SAVED_NAME__.get(self.__SAVE_Classify_THRESHOLD__,
                                                                     self.__SAVE_Classify_THRESHOLD__)
         __LABEL_SAVE_Classify_PASS__ = self.__SAVED_NAME__.get(self.__SAVE_Classify_PASS__, self.__SAVE_Classify_PASS__)
         __LABEL_SAVE_Classify_Best__ = self.__SAVED_NAME__.get(self.__SAVE_Classify_Best__, self.__SAVE_Classify_Best__)
         __LABEL_SAVE_Classify_result__ = self.__SAVED_NAME__.get(self.__SAVE_Classify_result__,
                                                                  self.__SAVE_Classify_result__)
 
         ##
-        kwargs = self.set_default_var(kwargs, __LABEL_SAVE_Classify_result__, classify_values_dict)
-        kwargs = self.set_default_var(kwargs, __LABEL_SAVE_Classify_THRESHOLD__, self.__Classify_THRESHOLD__)
-        kwargs = self.set_default_var(kwargs, __LABEL_SAVE_Classify_PASS__, pass_token)
-        kwargs = self.set_default_var(kwargs, __LABEL_SAVE_Classify_Best__,
+        kwargs = StageMemoryFragOperation. set_default_frag(kwargs, __LABEL_SAVE_Classify_result__, classify_values_dict)
+        kwargs = StageMemoryFragOperation. set_default_frag(kwargs, __LABEL_SAVE_Classify_THRESHOLD__, self.__Classify_THRESHOLD__)
+        kwargs = StageMemoryFragOperation. set_default_frag(kwargs, __LABEL_SAVE_Classify_PASS__, pass_token)
+        kwargs = StageMemoryFragOperation. set_default_frag(kwargs, __LABEL_SAVE_Classify_Best__,
                                       max(classify_values_dict, key=classify_values_dict.get))
 
         if self.disable_refuse_question:
             pass_token = True
 
         return pass_token, kwargs
 
@@ -348,18 +352,18 @@
     __SWITCH_STAGE__: LibSwitchStage,
     __LIB_SWITCH_STAGE__: LibSwitchStage,
     __Similarly_STAGE__: SimilarlyStage,
     __Classify_STAGE__: ClassifyStage
 }
 
 
-def gen_multi_agent(stage_dict: dict, stages_classes=None):
+def gen_multi_agent(stage_dict: Dict[str, Any], stages_classes: None | Dict[str, Any] = None) -> MultiAgent:
     if stages_classes is None:
         stages_classes = __LIB_STAGES__
-    stages = {}
+    stages:Dict[str, List[Stage]] = {}
     for stages_label, stage_jsons in stage_dict.items():
         stages[stages_label] = []
         for stage_json in stage_jsons:
             stage_class = stages_classes[stage_json["stage_type"]]
             stages[stages_label].append(stage_class(stage_json))
 
     return MultiAgent(stages)
```

### Comparing `ConversationAgent-0.5.9/ConversationAgent/README.md` & `ConversationAgent-0.6.0/ConversationAgent/README.md`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/__agent__.py` & `ConversationAgent-0.6.0/ConversationAgent/__agent__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import json
 import uuid
 import re
-
-from .__stage__ import Stage, __USER_TEXT__, __SYS_REPLY__, StageStatus, \
-    __LOCAL_VAR_LABEL__, __LOCAL_VAR_VALUE__, StageType, __PASS_TOKEN__, __KEEP_VAR__, \
-    __KEEP_DEFAULT_VAR__
-
+from typing import Tuple, List, Dict, Any
+from .__stage__ import Stage, StageStatus, StageType
+from .types.static import __USER_TEXT__, __SYS_REPLY__, __LOCAL_VAR_LABEL__, __LOCAL_VAR_VALUE__, __PASS_TOKEN__, __KEEP_VAR__, __KEEP_DEFAULT_VAR__
+from .__memory__ import StagePassTokenOperation, StageStatusOperation
 
 class SingleThreadAgent:
 
-    def __init__(self, stages: [Stage]):
+    def __init__(self, stages: List[Stage]):
         self.stages = stages
 
     @staticmethod
     def is_not_complete(data) -> bool:
-        status = Stage.get_sys_stage_status(data)
+        status = StageStatusOperation.get_sys_stage_status(data)
         return True if status in [StageStatus.FIRST, StageStatus.REFUSE] else False
 
     @staticmethod
     def is_final_stage(stages, idx) -> bool:
         return True if len(stages) == (idx + 1) else False
 
     @staticmethod
     def clear_sys_reply(data):
         data.pop(__SYS_REPLY__, None)
         return data
 
     @classmethod
-    def get_sys_reply(cls, data):
-        reply: list = data.get(__SYS_REPLY__, [])
+    def get_sys_reply(cls, data: Dict[str, Any]) -> list[str]:
+        reply: List[str] = data.get(__SYS_REPLY__, [])
         reply = [line for line in reply if line != ""]
         return reply
 
     @staticmethod
     def set_sys_reply(data, texts: [str]):
         data[__SYS_REPLY__] = texts
         return data
 
-    def run_all_stages(self, **kwargs) -> (list, dict):
+    def run_all_stages(self, **kwargs: Dict[str, Any]) -> Tuple[List[str], Dict[str, Any]]:
         #
         kwargs = self.clear_sys_reply(kwargs)
 
         #
         for idx, stage in enumerate(self.stages):
             # print(f"kwargs in: {kwargs}")
             kwargs = stage.run(**kwargs)
```

### Comparing `ConversationAgent-0.5.9/ConversationAgent/__init__.py` & `ConversationAgent-0.6.0/ConversationAgent/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import uuid
 import re
+from typing import Dict, Any, Tuple, List
 
-from .__agent__ import Agent
-from .__stage__ import Stage, __USER_TEXT__, __SYS_REPLY__, StageStatus, \
-    __LOCAL_VAR_LABEL__, __LOCAL_VAR_VALUE__
+from .__agent__ import Agent, SingleThreadAgent
+from .__stage__ import Stage, StageStatus
+from .types.static import __USER_TEXT__, __SYS_REPLY__, __LOCAL_VAR_LABEL__, __LOCAL_VAR_VALUE__
 
 __version__ = "0.1.10"
 __MOCK_STAGES_LABEL_1__ = "__MOCK_STAGES_LABEL_1__"
 
 
 def mock_client_with_test(agent, says, tests):
     data = {}
@@ -26,25 +27,25 @@
         if show_user_text:
             print("\t用戶:", s)
         print("系統:", reply_text)
         if show_data:
             print("\t系統資料:", data)
 
 
-def mock_client_human(agent):
+def mock_client_human(agent: SingleThreadAgent):
     data = {}
     while True:
         s = input("請輸入：")
         data[__USER_TEXT__] = s
         if s == "exit":
             break
         reply_text, data = agent.run_all_stages(**data)
         print("系統:", reply_text)
 
 
-def mock_client_once(agent: Agent, text: str, data: dict):
+def mock_client_once(agent: SingleThreadAgent, text: str, data: Dict[str, Any]) -> Tuple[List[str], Dict[str, Any]]:
     data[__USER_TEXT__] = text
     return agent.run_all_stages(**data)
 
 
-def to_bot(agent: Agent, text: str, data: dict):
+def to_bot(agent: Agent, text: str, data: Dict[str, Any]) -> Tuple[List[str], Dict[str, Any]]:
     return mock_client_once(agent, text, data)
```

### Comparing `ConversationAgent-0.5.9/ConversationAgent/__tool__.py` & `ConversationAgent-0.6.0/ConversationAgent/__tool__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-def get_value_from_dict_by_multi_name(d: dict, names: [str], default=None):
+from typing import Dict, Any, List
+def get_value_from_dict_by_multi_name(d: Dict[str, Any], names: List[str], default=None):
     for name in names:
         if name in d:
             return d[name]
     return default
 
 
 def compute_by_string(a, symbol, b):
```

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/__init__.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/__init__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/__main__.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/__main__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/_compat.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/_compat.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/analyzer.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/analyzer.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/idf.txt` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/idf.txt`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/textrank.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/textrank.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/analyse/tfidf.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/analyse/tfidf.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/dict.txt` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/dict.txt`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/finalseg/__init__.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/finalseg/__init__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/finalseg/prob_emit.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/finalseg/prob_emit.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/__init__.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/__init__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/char_state_tab.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/char_state_tab.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/prob_emit.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/prob_emit.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/prob_start.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/prob_start.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/prob_trans.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/prob_trans.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/jieba_zh/posseg/viterbi.py` & `ConversationAgent-0.6.0/ConversationAgent/jieba_zh/posseg/viterbi.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.9/ConversationAgent/nlp_tool.py` & `ConversationAgent-0.6.0/ConversationAgent/__nlp_tool__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,55 @@
-def result_format(sentence,corpus,ans,score):
-    return {
-      "get parameter": {
-        "sentence": [
-          sentence
-        ],
-        "corpus": corpus
-      },
-      "worker response": {
-        "ans": [
-          [
-            ans,
-            score
-          ]
-
-        ]
-      }
-    }
-
-def MED(sent_01, sent_02):
-    n = len(sent_01)
-    m = len(sent_02)
-
-    matrix = [[i + j for j in range(m + 1)] for i in range(n + 1)]
-
-    for i in range(1, n + 1):
-        for j in range(1, m + 1):
-            if sent_01[i - 1] == sent_02[j - 1]:
-                d = 0
-            else:
-                d = 1
-
-            matrix[i][j] = min(matrix[i - 1][j] + 1, matrix[i][j - 1] + 1, matrix[i - 1][j - 1] + d)
-
-    distance_score = matrix[n][m]
-
-    return distance_score
-
-
-def similar(sentence, corpus):
-    ans = None
-    min_distance = 999
-    max_distance = 1
+from typing import NamedTuple, List, Tuple
+
+class SimilarResult(NamedTuple):
+    sentence: str
+    corpus: List[str]
+    ans: str
+    score: float
+
+
+def result_format(sentence: str,corpus: List[str], ans:str, score:float) -> SimilarResult:
+    return SimilarResult(
+      sentence=sentence,
+      corpus=corpus,
+      ans=ans,
+      score=score
+    )
+
+def MED(s1: str, s2: str) -> float:
+    # Create a matrix of size (len(s1) + 1) x (len(s2) + 1)
+    s1a = [w for w in s1]
+    s2a = [w for w in s2]
+    if len(s1a) <= len(s2a):
+      s1a,s2a = s2a,s1a
+
+    for w in s2a:
+      if w in s1a:
+        del s1a[s1a.index(w)]
+
+    # Return the Levenshtein distance
+    score= len(s1a)
+    if score == 0:
+      return 1
+    return (1 / score)-0.0000001
+
+
+
+def similar_text_distance(sentence: str, corpus: List[str]) -> SimilarResult:
+    socres: List[Tuple[str, float]] = []
     for c in corpus:
         distance = MED(sentence, c)
-        max_distance = distance if distance > max_distance else max_distance
-        if distance < min_distance:
-            min_distance = distance
-            ans = c
-    score = 1-(min_distance/max_distance)
-    result = result_format(sentence, corpus, ans, score)
-    return result
+        socres.append((c, distance))
+    sorted_data = sorted(socres, key=lambda x: x[1])
+    return result_format(sentence, corpus, sorted_data[-1][0], sorted_data[-1][1])
 #
 # corpus= [
 #     "我想去醫院",
 #     "我想去大學",
 #     "我想去台北",
 #     "我想去跑步",
 #     "我想去公園"
 # ]
 # sentence="我想去大公園"
-# print(similar(sentence,corpus))
+# print(similar(sentence,corpus))
+# print("socre", MED('廁所在哪裡', '附近有廁所嗎'))
+# print("socre", MED('廁所在哪裡', '詢問處在哪裡'))
```

### Comparing `ConversationAgent-0.5.9/ConversationAgent.egg-info/PKG-INFO` & `ConversationAgent-0.6.0/ConversationAgent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConversationAgent
-Version: 0.5.9
+Version: 0.6.0
 Summary: ConversationAgent
 Home-page: https://github.com/Chunshan-Theta/ConversationAgent
 Author: Theta
 Description-Content-Type: text/markdown
 
 ## 說明
 不需資料庫之對話腳本代理。
```

### Comparing `ConversationAgent-0.5.9/ConversationAgent.egg-info/SOURCES.txt` & `ConversationAgent-0.6.0/ConversationAgent.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 README.md
 setup.py
 ConversationAgent/LibStage.py
 ConversationAgent/README.md
-ConversationAgent/SentenceStage.py
 ConversationAgent/__agent__.py
 ConversationAgent/__init__.py
+ConversationAgent/__memory__.py
+ConversationAgent/__nlp_tool__.py
 ConversationAgent/__stage__.py
 ConversationAgent/__tool__.py
-ConversationAgent/nlp_tool.py
 ConversationAgent.egg-info/PKG-INFO
 ConversationAgent.egg-info/SOURCES.txt
 ConversationAgent.egg-info/dependency_links.txt
 ConversationAgent.egg-info/not-zip-safe
 ConversationAgent.egg-info/top_level.txt
 ConversationAgent/jieba_zh/README.md
 ConversationAgent/jieba_zh/__init__.py
@@ -29,15 +29,11 @@
 ConversationAgent/jieba_zh/finalseg/prob_trans.py
 ConversationAgent/jieba_zh/posseg/__init__.py
 ConversationAgent/jieba_zh/posseg/char_state_tab.py
 ConversationAgent/jieba_zh/posseg/prob_emit.py
 ConversationAgent/jieba_zh/posseg/prob_start.py
 ConversationAgent/jieba_zh/posseg/prob_trans.py
 ConversationAgent/jieba_zh/posseg/viterbi.py
-ConversationAgent/test/__init__.py
-ConversationAgent/test/__test_v1__.py
-ConversationAgent/test/__test_v2__.py
-ConversationAgent/test/__test_v3__.py
-ConversationAgent/test/__test_v4__.py
-ConversationAgent/test/__test_v5__.py
-ConversationAgent/test/__test_v6__.py
-ConversationAgent/test/__test_v7__.py
+ConversationAgent/types/__init__.py
+ConversationAgent/types/memory.py
+ConversationAgent/types/stage.py
+ConversationAgent/types/static.py
```

### Comparing `ConversationAgent-0.5.9/PKG-INFO` & `ConversationAgent-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConversationAgent
-Version: 0.5.9
+Version: 0.6.0
 Summary: ConversationAgent
 Home-page: https://github.com/Chunshan-Theta/ConversationAgent
 Author: Theta
 Description-Content-Type: text/markdown
 
 ## 說明
 不需資料庫之對話腳本代理。
```

### Comparing `ConversationAgent-0.5.9/setup.py` & `ConversationAgent-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("./ConversationAgent/README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 setuptools.setup(
     name='ConversationAgent',
-    version='0.5.9',
+    version='0.6.0',
     description='ConversationAgent',
     author='Theta',
     license='',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={
```

