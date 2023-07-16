# Comparing `tmp/threads-py-0.0.6.tar.gz` & `tmp/threads_py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-py-0.0.6.tar", last modified: Sun Jul  9 16:08:34 2023, max compression
+gzip compressed data, was "threads_py-0.0.7.tar", max compression
```

## Comparing `threads-py-0.0.6.tar` & `threads_py-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,40 @@
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.616391 threads-py-0.0.6/
--rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.6/LICENSE
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 16:08:34.616238 threads-py-0.0.6/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     3730 2023-07-09 08:19:43.000000 threads-py-0.0.6/README.md
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.610067 threads-py-0.0.6/models/
--rw-r--r--   0 mineru     (501) staff       (20)        0 2023-07-09 08:19:43.000000 threads-py-0.0.6/models/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-09 16:08:34.616445 threads-py-0.0.6/setup.cfg
--rw-r--r--   0 mineru     (501) staff       (20)      941 2023-07-09 05:30:57.000000 threads-py-0.0.6/setup.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.610780 threads-py-0.0.6/threads_py.egg-info/
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     1378 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/SOURCES.txt
--rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/dependency_links.txt
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/requires.txt
--rw-r--r--   0 mineru     (501) staff       (20)       17 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/top_level.txt
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.611271 threads-py-0.0.6/threadspy/
--rw-r--r--   0 mineru     (501) staff       (20)      167 2023-07-09 16:08:18.000000 threads-py-0.0.6/threadspy/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)     5500 2023-07-09 15:58:32.000000 threads-py-0.0.6/threadspy/_agent.py
--rw-r--r--   0 mineru     (501) staff       (20)      676 2023-07-09 07:59:50.000000 threads-py-0.0.6/threadspy/_constant.py
--rw-r--r--   0 mineru     (501) staff       (20)    21217 2023-07-09 15:58:58.000000 threads-py-0.0.6/threadspy/_thread.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.611536 threads-py-0.0.6/threadspy/templates/
--rw-r--r--   0 mineru     (501) staff       (20)       29 2023-07-09 08:19:43.000000 threads-py-0.0.6/threadspy/templates/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)      128 2023-07-09 08:19:43.000000 threads-py-0.0.6/threadspy/templates/qna.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.616027 threads-py-0.0.6/threadspy/types/
--rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 19:54:05.000000 threads-py-0.0.6/threadspy/types/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.6/threadspy/types/candidate.py
--rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.6/threadspy/types/caption.py
--rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.6/threadspy/types/common.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.6/threadspy/types/extensions.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.6/threadspy/types/get_thread_likers_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.6/threadspy/types/get_user_profile_replies_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.6/threadspy/types/get_user_profile_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.6/threadspy/types/get_user_profile_thread_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.6/threadspy/types/get_user_profile_threads_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/image_versions2.py
--rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/media_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.6/threadspy/types/post.py
--rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.6/threadspy/types/quoted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.6/threadspy/types/reply_facepile_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.6/threadspy/types/reposted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/share_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.6/threadspy/types/text_post_app_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/thread.py
--rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 19:54:05.000000 threads-py-0.0.6/threadspy/types/thread_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/thread_item.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.6/threadspy/types/threads_bio_link.py
--rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.6/threadspy/types/threads_hd_profile_pic_version.py
--rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.6/threadspy/types/threads_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.6/threadspy/types/threads_user_summary.py
--rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/user_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.6/threadspy/types/user_profile_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.6/threadspy/types/users.py
--rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.6/threadspy/types/video_version.py
+-rw-r--r--   0        0        0     1066 2023-07-16 04:06:05.352298 threads_py-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5016 2023-07-16 12:39:36.358642 threads_py-0.0.7/README.md
+-rw-r--r--   0        0        0      778 2023-07-16 12:42:05.324792 threads_py-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-07-16 12:39:36.364127 threads_py-0.0.7/threadspy/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-16 12:39:36.364575 threads_py-0.0.7/threadspy/ai/__init__.py
+-rw-r--r--   0        0        0     5537 2023-07-16 12:39:36.364749 threads_py-0.0.7/threadspy/ai/agent.py
+-rw-r--r--   0        0        0       29 2023-07-16 12:39:36.364876 threads_py-0.0.7/threadspy/ai/templates/__init__.py
+-rw-r--r--   0        0        0      128 2023-07-16 12:39:36.364956 threads_py-0.0.7/threadspy/ai/templates/qna.py
+-rw-r--r--   0        0        0      261 2023-07-16 12:39:36.365613 threads_py-0.0.7/threadspy/constants.py
+-rw-r--r--   0        0        0    25214 2023-07-16 12:39:36.366733 threads_py-0.0.7/threadspy/threads_api.py
+-rw-r--r--   0        0        0     1950 2023-07-16 12:39:36.367180 threads_py-0.0.7/threadspy/types/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-16 12:39:36.367376 threads_py-0.0.7/threadspy/types/candidate.py
+-rw-r--r--   0        0        0      136 2023-07-16 12:39:36.367602 threads_py-0.0.7/threadspy/types/caption.py
+-rw-r--r--   0        0        0      622 2023-07-16 03:01:37.259110 threads_py-0.0.7/threadspy/types/common.py
+-rw-r--r--   0        0        0      144 2023-07-16 12:39:36.367812 threads_py-0.0.7/threadspy/types/extensions.py
+-rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259277 threads_py-0.0.7/threadspy/types/get_thread_likers_response.py
+-rw-r--r--   0        0        0      314 2023-07-16 03:01:37.259370 threads_py-0.0.7/threadspy/types/get_user_profile_replies_response.py
+-rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259449 threads_py-0.0.7/threadspy/types/get_user_profile_response.py
+-rw-r--r--   0        0        0      315 2023-07-16 03:01:37.259525 threads_py-0.0.7/threadspy/types/get_user_profile_thread_response.py
+-rw-r--r--   0        0        0      314 2023-07-16 03:22:06.009163 threads_py-0.0.7/threadspy/types/get_user_profile_threads_response.py
+-rw-r--r--   0        0        0      233 2023-07-16 03:43:54.986708 threads_py-0.0.7/threadspy/types/image_versions2.py
+-rw-r--r--   0        0        0      216 2023-07-16 03:01:37.259923 threads_py-0.0.7/threadspy/types/media_data.py
+-rw-r--r--   0        0        0      772 2023-07-16 03:01:37.260014 threads_py-0.0.7/threadspy/types/post.py
+-rw-r--r--   0        0        0      766 2023-07-16 03:01:37.260090 threads_py-0.0.7/threadspy/types/quoted_post.py
+-rw-r--r--   0        0        0      191 2023-07-16 12:39:36.368023 threads_py-0.0.7/threadspy/types/reply_facepile_user.py
+-rw-r--r--   0        0        0      812 2023-07-16 03:01:37.260232 threads_py-0.0.7/threadspy/types/reposted_post.py
+-rw-r--r--   0        0        0      304 2023-07-16 03:01:37.260298 threads_py-0.0.7/threadspy/types/share_info.py
+-rw-r--r--   0        0        0      313 2023-07-16 03:42:07.939582 threads_py-0.0.7/threadspy/types/text_post_app_info.py
+-rw-r--r--   0        0        0      299 2023-07-16 03:01:37.260436 threads_py-0.0.7/threadspy/types/thread.py
+-rw-r--r--   0        0        0      280 2023-07-16 03:01:37.260503 threads_py-0.0.7/threadspy/types/thread_data.py
+-rw-r--r--   0        0        0      433 2023-07-16 03:41:29.770812 threads_py-0.0.7/threadspy/types/thread_item.py
+-rw-r--r--   0        0        0      142 2023-07-16 03:01:37.260628 threads_py-0.0.7/threadspy/types/threads_bio_link.py
+-rw-r--r--   0        0        0      185 2023-07-16 03:01:37.260692 threads_py-0.0.7/threadspy/types/threads_hd_profile_pic_version.py
+-rw-r--r--   0        0        0      729 2023-07-16 03:43:52.128369 threads_py-0.0.7/threadspy/types/threads_user.py
+-rw-r--r--   0        0        0      222 2023-07-16 03:01:37.260815 threads_py-0.0.7/threadspy/types/threads_user_summary.py
+-rw-r--r--   0        0        0      198 2023-07-16 03:01:37.260877 threads_py-0.0.7/threadspy/types/user_data.py
+-rw-r--r--   0        0        0      200 2023-07-16 03:01:37.260949 threads_py-0.0.7/threadspy/types/user_profile_data.py
+-rw-r--r--   0        0        0      230 2023-07-16 03:01:37.261016 threads_py-0.0.7/threadspy/types/users.py
+-rw-r--r--   0        0        0      176 2023-07-16 12:39:36.368230 threads_py-0.0.7/threadspy/types/video_version.py
+-rw-r--r--   0        0        0     6922 1970-01-01 00:00:00.000000 threads_py-0.0.7/PKG-INFO
```

### Comparing `threads-py-0.0.6/LICENSE` & `threads_py-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.6/threadspy/_agent.py` & `threads_py-0.0.7/threadspy/ai/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import sys
-import json
 import itertools
 from datetime import datetime
 from langchain import PromptTemplate, LLMChain
 from langchain.llms import LlamaCpp, OpenAIChat
 from langchain.callbacks.manager import CallbackManager
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
-from ._thread import ThreadsAPI
+from ..threads_api import ThreadsAPI
 from .templates import QA_template
 
 
 class ThreadsAgent:
     mode = None
     model = None
     mode_cpu = False
@@ -65,15 +64,17 @@
             else:
                 self.mode_cpu = False
                 self.mode_gpu = False
                 self.mode_mps = False
         else:
             raise "Choose a mode between 'llama' and 'openai'"
 
-    def analysis_profile(self, username: str, boundary: str = "all", onlyText=False, sort="DESC"):
+    def analysis_profile(
+        self, username: str, boundary: str = "all", onlyText=False, sort="DESC"
+    ):
         self.threads_api.username = username
         user_id = self.threads_api.get_user_id_from_username(username=username)
         if user_id is None:
             raise "[Auth] Private profiles cannot be analyzed."
         if boundary in ["all", "replies", "threads"]:
             threads = []
             if boundary in ["all", "replies"]:
@@ -82,15 +83,17 @@
                 )
                 threads.extend(replies_tab)
             if boundary in ["all", "threads"]:
                 threads_tab = self.threads_api.get_user_profile_threads(
                     username=username, user_id=self.threads_api.user_id
                 )
                 threads.extend(threads_tab)
-            threads = [[item["post"] for item in x.to_dict()["thread_items"]] for x in threads]
+            threads = [
+                [item["post"] for item in x.to_dict()["thread_items"]] for x in threads
+            ]
             threads = list(itertools.chain(*threads))
             if sort == "DESC":
                 threads.sort(key=lambda x: (x["taken_at"],))
             else:
                 threads.sort(key=lambda x: (x["taken_at"] * -1,))
             threads = [
                 {
```

### Comparing `threads-py-0.0.6/threadspy/_thread.py` & `threads_py-0.0.7/threadspy/threads_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,152 +1,237 @@
 import os
 import re
 import time
 import json
 import uuid
+import base64
 import urllib
+from urllib.parse import quote
 import random
 import requests
 import mimetypes
 from typing import List
 from datetime import datetime
+from Crypto.Random import get_random_bytes
+from Crypto.PublicKey import RSA
+from Crypto.Cipher import (
+    AES,
+    PKCS1_v1_5,
+)
 
 from threadspy.types import (
     Thread,
     UsersData,
     ThreadsUser,
     ThreadData,
     GetUserProfileResponse,
     GetThreadLikersResponse,
     GetUserProfileThreadResponse,
     GetUserProfileRepliesResponse,
     GetUserProfileThreadsResponse,
 )
 
-from threadspy._constant import (
+from threadspy.constants import (
+    LATEST_ANDROID_APP_VERSION,
     DEFAULT_LSD_TOKEN,
     DEFAULT_DEVICE_ID,
-    LOGIN_URL,
-    POST_URL,
-    POST_HEADERS_DEFAULT,
-    POST_WITH_IMAGE_URL,
+    BASE_API_URL,
 )
 
 
 class ThreadsAPI:
     fbLSDToken = DEFAULT_LSD_TOKEN
     verbose = False
     noUpdateLSD = False
     username = None
     password = None
     user_id = None
     token = None
     device_id = DEFAULT_DEVICE_ID
     http_client = requests.Session()
+    timestamp_string = None
+    encrypted_password = None
 
     def __init__(
         self,
-        verbose=None,
-        noUpdateLSD=None,
-        fbLSDToken=None,
-        username=None,
-        password=None,
-        device_id=None,
-    ):
-        if fbLSDToken is not None and "<class 'str'>" == str(type(fbLSDToken)):
+        verbose: str | None = None,
+        noUpdateLSD: str | None = None,
+        fbLSDToken: str | None = None,
+        username: str | None = None,
+        password: str | None = None,
+        device_id: str | None = None,
+        token: str | None = None,
+    ) -> None:
+        if fbLSDToken is not None and isinstance(fbLSDToken, str):
             self.fbLSDToken = fbLSDToken
-        if username is not None and "<class 'str'>" == str(type(username)):
-            self.username = username
-        if password is not None and "<class 'str'>" == str(type(password)):
-            self.password = password
-        if device_id is not None and "<class 'str'>" == str(type(device_id)):
+        if device_id is not None and isinstance(device_id, str):
             self.device_id = device_id
-        if noUpdateLSD is not None and "<class 'bool'>" == str(type(noUpdateLSD)):
+        if noUpdateLSD is not None and isinstance(noUpdateLSD, str):
             self.noUpdateLSD = noUpdateLSD
-        if verbose is not None and "<class 'bool'>" == str(type(verbose)):
+        if verbose is not None and isinstance(verbose, str):
             self.verbose = verbose
 
+        if (
+            username is not None
+            and isinstance(username, str)
+            and password is not None
+            and isinstance(password, str)
+        ):
+            self.username = username
+            self.password = password
+            self.public_key, self.public_key_id = self._get_ig_public_key()
+            self.encrypted_password, self.timestamp_string = self._password_encryption(
+                password
+            )
+
+        if token is not None and isinstance(token, str):
+            self.token = token
+        else:
+            self.token = self.get_token()
+
     def __is_valid_url(self, url: str) -> bool:
-        url_pattern = re.compile(
-            r"^(https?://)?"
-            r"((([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9-]*[a-zA-Z0-9])\.)+[a-zA-Z]{2,})"
-            r"(/?|/[-a-zA-Z0-9_%+.~!@#$^&*(){}[\]|/\\<>]*)$"
-        )
+        url_pattern = re.compile(r"https?://(?:[-\w.]|(?:%[\da-fA-F]{2}))+")
         if re.match(url_pattern, url) is not None:
             try:
                 response = requests.head(url)
-                return response.status_code == 200
-            except requests.exceptions.RequestException:
+                return response.status_code == 200 or response.status_code == 302
+            except requests.exceptions.RequestException as e:
                 return False
         return False
 
     def __download(self, url: str) -> bytes:
         try:
             response = requests.get(url, stream=True)
             response.raise_for_status()
             return response.content
         except requests.exceptions.RequestException as e:
             print("[ERROR] fail to file load: ", e)
             return None
 
-    def __get_default_headers(self, username: str = None):
-        if username is None:
-            return {
-                "authority": "www.threads.net",
-                "accept": "*/*",
-                "accept-language": "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7",
-                "cache-control": "no-cache",
-                "origin": "https://www.threads.net",
-                "pragma": "no-cache",
-                "referer": None,
-                "x-asbd-id": "129477",
-                "x-fb-lsd": self.fbLSDToken,
-                "x-ig-app-id": "238260118697367",
-            }
-        else:
+    def __get_app_headers(self) -> dict:
+        headers = {
+            "User-Agent": f"Barcelona {LATEST_ANDROID_APP_VERSION} Android",
+            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+        }
+        if self.token is not None:
+            headers["Authorization"] = f"Bearer IGT:2:{self.token}"
+        return headers
+
+    def __get_default_headers(self, username: str = None) -> dict:
+        headers = {
+            "authority": "www.threads.net",
+            "accept": "*/*",
+            "accept-language": "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7",
+            "cache-control": "no-cache",
+            "origin": "https://www.threads.net",
+            "pragma": "no-cache",
+            "x-asbd-id": "129477",
+            "x-fb-lsd": self.fbLSDToken,
+            "x-ig-app-id": "238260118697367",
+        }
+
+        if username is not None:
             self.username = username
-            return {
-                "authority": "www.threads.net",
-                "accept": "*/*",
-                "accept-language": "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7",
-                "cache-control": "no-cache",
-                "origin": "https://www.threads.net",
-                "pragma": "no-cache",
-                "referer": f"https://www.threads.net/@{username}",
-                "x-asbd-id": "129477",
-                "x-fb-lsd": self.fbLSDToken,
-                "x-ig-app-id": "238260118697367",
-            }
+            headers["referer"] = f"https://www.threads.net/@{username}"
+
+        return headers
+
+    def _get_ig_public_key(self) -> tuple[str, int]:
+        """
+        Get Instagram public key to encrypt the password.
+
+        Returns:
+            The public key and the key identifier as tuple(str, int).
+        """
+        str_parameters = json.dumps(
+            {
+                "id": str(uuid.uuid4()),
+            },
+        )
+        encoded_parameters = quote(string=str_parameters, safe="!~*'()")
+
+        response = requests.post(
+            url=f"{BASE_API_URL}/api/v1/qe/sync/",
+            headers={
+                "User-Agent": f"Barcelona {LATEST_ANDROID_APP_VERSION} Android",
+                "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+            },
+            data=f"params={encoded_parameters}",
+        )
+        public_key = response.headers.get("ig-set-password-encryption-pub-key")
+        public_key_id = response.headers.get("ig-set-password-encryption-key-id")
+
+        return public_key, int(public_key_id)
+
+    def _password_encryption(self, password: str) -> tuple[str, str]:
+        password_bytes = password.encode("utf-8")
+
+        timestamp = int(time.time())
+        timestamp_string = str(timestamp).encode("utf-8")
+
+        secret_key = get_random_bytes(32)
+        key_id_mixed_bytes = int(1).to_bytes(1, "big") + self.public_key_id.to_bytes(
+            1, "big"
+        )
+        initialization_vector = get_random_bytes(12)
+        encrypted_rsa_key_mixed_bytes = int(0).to_bytes(1, "big") + int(1).to_bytes(
+            1, "big"
+        )
+        public_key_bytes = base64.b64decode(self.public_key)
+        public_key = RSA.import_key(extern_key=public_key_bytes)
+        cipher = PKCS1_v1_5.new(public_key)
+        encrypted_secret_key = cipher.encrypt(secret_key)
+        cipher = AES.new(secret_key, AES.MODE_GCM, nonce=initialization_vector)
+        cipher.update(timestamp_string)
+        encrypted_password, auth_tag = cipher.encrypt_and_digest(password_bytes)
+
+        password_as_encryption_sequence = (
+            key_id_mixed_bytes
+            + initialization_vector
+            + encrypted_rsa_key_mixed_bytes
+            + encrypted_secret_key
+            + auth_tag
+            + encrypted_password
+        )
+        password_encryption_base64 = base64.b64encode(
+            s=password_as_encryption_sequence,
+        ).decode("ascii")
+
+        return password_encryption_base64, str(timestamp)
 
     def get_user_id_from_username(self, username) -> str:
         """
         set user id by username.
 
         Args:
             username (str): username on threads.net
 
         Returns:
             string: user_id if not valid return None
         """
         headers = self.__get_default_headers(username)
-        headers[
-            "accept"
-        ] = "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7"
-        headers["accept-language"] = "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7"
-        headers["pragma"] = "no-cache"
-        headers["referer"] = "https://www.instagram.com/"
-        headers["sec-fetch-dest"] = "document"
-        headers["sec-fetch-mode"] = "navigate"
-        headers["sec-fetch-site"] = "cross-site"
-        headers["sec-fetch-user"] = "?1"
-        headers["upgrade-insecure-requests"] = "1"
-        headers["x-asbd-id"] = None
-        headers["x-fb-lsd"] = None
-        headers["x-ig-app-id"] = None
-        response = self.http_client.get(f"https://www.instagram.com/{username}", headers=headers)
+        headers.update(
+            {
+                "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+                "accept-language": "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7",
+                "pragma": "no-cache",
+                "referer": "https://www.instagram.com/",
+                "sec-fetch-dest": "document",
+                "sec-fetch-mode": "navigate",
+                "sec-fetch-site": "cross-site",
+                "sec-fetch-user": "?1",
+                "upgrade-insecure-requests": "1",
+                "x-asbd-id": None,
+                "x-fb-lsd": None,
+                "x-ig-app-id": None,
+            }
+        )
+        response = self.http_client.get(
+            f"https://www.instagram.com/{username}", headers=headers
+        )
 
         text = response.text.replace("\n", "")
 
         user_id_match = re.search('"user_id":"(\d+)",', text)
         user_id = user_id_match.group(1) if user_id_match else None
 
         lsd_token_match = re.search('"LSD",\[\],{"token":"(\w+)"},\d+\]', text)
@@ -158,14 +243,26 @@
                 print("[fbLSDToken] UPDATED", self.fbLSDToken)
         if user_id is not None:
             self.user_id = user_id
             return self.user_id
         else:
             return None
 
+    def get_current_user_id(self) -> str:
+        if self.user_id:
+            if self.verbose:
+                print("[userID] USING", self.user_id)
+            return self.user_id
+        if self.username is None:
+            raise "username is not defined"
+        self.user_id = self.get_user_id_from_username(self.username)
+        if self.verbose:
+            print("[userID] UPDATED", self.user_id)
+        return self.user_id
+
     def get_user_profile(self, username, user_id=None) -> ThreadsUser:
         """
         Returns profile info by username.
 
         Args:
             username (str): username on threads.net
             user_id (str, optional):: user_id which is unique to each user.
@@ -282,19 +379,20 @@
 
         Args:
             thread_id (str): thread_id which is unique to each thread.
 
         Returns:
             str: a post id
         """
-        thread_id = thread_id.split("?")[0]
-        thread_id = thread_id.replace("/", "")
-        post_url = f"https://www.threads.net/t/{thread_id}"
-        result = self.get_post_id_from_url(post_url=post_url)
-        return result
+        alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_"
+        post_id = 0
+        for letter in thread_id:
+            post_id = (post_id * 64) + alphabet.index(letter)
+
+        return str(post_id)
 
     def get_post_id_from_url(self, post_url) -> str:
         """
         Returns the post_id of a specific one thread.
 
         Args:
             post_url (str): a threads app direct link
@@ -378,200 +476,229 @@
             thread = GetThreadLikersResponse.from_dict(response.json())
             return thread.data.likers
         except Exception as e:
             if self.verbose:
                 print("[ERROR] ", e)
             return UsersData(users=[])
 
+    def __toggle_auth__post_request(self, url: str):
+        if self.token is None:
+            token = self.get_token()
+        else:
+            token = self.token
+        if token is None:
+            raise "Token not found"
+        headers = self.__get_default_headers()
+        res = self.http_client.post(url, headers=headers)
+        return res
+
+    def like(self, post_id: str) -> bool:
+        user_id = self.get_current_user_id()
+        res = self.__toggle_auth__post_request(
+            f"{BASE_API_URL}/api/v1/media/{post_id}_${user_id}/like/"
+        )
+        return res.json()["status"] == "ok"
+
+    def unlike(self, post_id: str) -> bool:
+        user_id = self.get_current_user_id()
+        res = self.__toggle_auth__post_request(
+            f"{BASE_API_URL}/api/v1/media/{post_id}_${user_id}/unlike/"
+        )
+        return res.json()["status"] == "ok"
+
+    def follow(self, user_id: str) -> bool:
+        res = self.__toggle_auth__post_request(
+            f"{BASE_API_URL}/api/v1/friendships/create/{user_id}/"
+        )
+        if self.verbose:
+            print("[FOLLOW]", res.json())
+        return res.json()
+
+    def unfollow(self, user_id: str) -> bool:
+        res = self.__toggle_auth__post_request(
+            f"{BASE_API_URL}/api/v1/friendships/destroy/{user_id}/"
+        )
+        if self.verbose:
+            print("[UNFOLLOW]", res.json())
+        return res.json()
+
     def get_token(self) -> str:
         """
         set fb login token
 
         Returns:
             str: validate token string None if not valid
         """
-        if self.username is None or self.password is None:
-            return None
         try:
-            blockVersion = "5f56efad68e1edec7801f630b5c122704ec5378adbee6609a448f105f34a9c73"
-            headers = {
-                "User-Agent": "Barcelona 289.0.0.77.109 Android",
-                "Sec-Fetch-Site": "same-origin",
-                "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
-            }
+            blockVersion = (
+                "5f56efad68e1edec7801f630b5c122704ec5378adbee6609a448f105f34a9c73"
+            )
             params = json.dumps(
                 {
                     "client_input_params": {
-                        "password": self.password,
+                        "password": f"#PWD_INSTAGRAM:4:{self.timestamp_string}:{self.encrypted_password}",
                         "contact_point": self.username,
                         "device_id": self.device_id,
                     },
                     "server_params": {
                         "credential_type": "password",
                         "device_id": self.device_id,
                     },
-                }
+                },
             )
             bk_client_context = json.dumps(
                 {"bloks_version": blockVersion, "styles_id": "instagram"}
             )
-            payload = f"params={urllib.parse.quote(params)}&bk_client_context={urllib.parse.quote(bk_client_context)}&bloks_versioning_id={blockVersion}"
-            response = requests.post(LOGIN_URL, timeout=60 * 1000, headers=headers, data=payload)
+            params_quote = quote(string=params, safe="!~*'()")
+            bk_client_context_quote = quote(string=bk_client_context, safe="!~*'()")
+
+            response = requests.post(
+                url=f"{BASE_API_URL}/api/v1/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/",
+                headers={
+                    "User-Agent": "Barcelona 289.0.0.77.109 Android",
+                    "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+                },
+                data=f"params={params_quote}&bk_client_context={bk_client_context_quote}&bloks_versioning_id={blockVersion}",
+            )
+
             data = response.text
             if data == "Oops, an error occurred.":
                 return None
-            pos = data.split("Bearer IGT:2:")
-            if len(pos) > 1:
-                pos = pos[1]
-                pos = pos.split("==")[0]
-                token = f"{pos}=="
-                self.token = token
-                return self.token
-            return None
+            pos = data.find("Bearer IGT:2:")
+            data_txt = data[pos:]
+            backslash_pos = data_txt.find("\\\\")
+            token = data_txt[13:backslash_pos]
+
+            return token
+
         except Exception as e:
             print("[ERROR] ", e)
+
             return None
 
-    def publish(self, caption: str) -> bool:
+    def publish(
+        self,
+        caption: str,
+        image_path: str = None,
+        url: str = None,
+        parent_post_id: str = None,
+    ) -> bool:
         """
         Returns publish post
 
         Args:
             caption (str): post_id which is unique to each post.
+            image_path (str, optional): image_path which is unique to each user.
+            url (str, optional): url which is unique to each user.
+            parent_post_id (str, optional): parent_post_id which is unique to each user.
 
         Returns:
             bool: verify that the post went publish
         """
         if self.username is None or self.password is None:
             return False
 
         user_id = self.get_user_id_from_username(self.username)
         if user_id is None:
             return False
-        token = self.get_token()
-        if token is None:
-            return False
-        params = json.dumps(
-            {
-                "publish_mode": "text_post",
-                "text_post_app_info": '{"reply_control":0}',
-                "timezone_offset": "-25200",
-                "source_type": "4",
-                "_uid": self.user_id,
-                "device_id": str(self.device_id),
-                "caption": caption,
-                "upload_id": str(int(datetime.now().timestamp() * 1000)),
-                "device": {
-                    "manufacturer": "OnePlus",
-                    "model": "ONEPLUS+A3010",
-                    "android_version": 25,
-                    "android_release": "7.1.1",
-                },
-            }
-        )
+        if self.token is None:
+            token = self.get_token()
+            if token is not None:
+                return False
+        now = datetime.now()
+        timezone_offset = (datetime.now() - datetime.utcnow()).seconds
+
+        params = {
+            "text_post_app_info": {"reply_control": 0},
+            "timezone_offset": "-" + str(timezone_offset),
+            "source_type": "4",
+            "_uid": self.user_id,
+            "device_id": str(self.device_id),
+            "caption": caption,
+            "upload_id": str(int(now.timestamp() * 1000)),
+            "device": {
+                "manufacturer": "OnePlus",
+                "model": "ONEPLUS+A3010",
+                "android_version": 25,
+                "android_release": "7.1.1",
+            },
+        }
+        post_url = f"{BASE_API_URL}/api/v1/media/configure_text_only_post/"
+        if image_path is not None:
+            post_url = f"{BASE_API_URL}/api/v1/media/configure_text_post_app_feed/"
+
+            image_content = None
+            if not (os.path.isfile(image_path) and os.path.exists(image_path)):
+                if not self.__is_valid_url(image_path):
+                    return False
+                else:
+                    image_content = self.__download(image_path)
+            upload_id = self.upload_image(
+                image_url=image_path, image_content=image_content
+            )
+            if upload_id == None:
+                return False
+            params["upload_id"] = upload_id["upload_id"]
+            params["scene_capture_type"] = ""
+        elif url is not None:
+            params["text_post_app_info"]["link_attachment_url"] = url
+        if image_path is None:
+            params["publish_mode"] = "text_post"
+
+        if parent_post_id is not None:
+            params["text_post_app_info"]["reply_id"] = parent_post_id
+        params = json.dumps(params)
         payload = f"signed_body=SIGNATURE.{urllib.parse.quote(params)}"
-        headers = POST_HEADERS_DEFAULT.copy()
-        headers.update({"Authorization": f"Bearer IGT:2:{self.token}"})
+        headers = self.__get_app_headers().copy()
         try:
-            response = requests.post(POST_URL, headers=headers, data=payload)
+            response = requests.post(post_url, headers=headers, data=payload)
             if response.status_code == 200:
                 return True
             else:
                 return False
         except Exception as e:
             if self.verbose:
                 print("[ERROR] ", e)
             return False
 
     def publish_with_image(self, caption: str, image_path: str) -> bool:
         """
+        @@deprecated
         Returns publish post with image
 
         Args:
             caption (str): post_id which is unique to each post.
             image_path (str): image path
 
         Returns:
             bool: verify that the post with image went publish
         """
-        if self.username is None or self.password is None:
-            return False
-        user_id = self.get_user_id_from_username(self.username)
-        if user_id is None:
-            return False
-        token = self.get_token()
-        if token is None:
-            return False
-        image_content = None
-        if not (os.path.isfile(image_path) and os.path.exists(image_path)):
-            if not self.__is_valid_url(image_path):
-                return False
-            else:
-                image_content = self.__download(image_path)
-        content = self.upload_image(image_path, image_content=image_content)
-        if content is not None:
-            try:
-                content = json.loads(content)
-                upload_id = content["upload_id"]
-                headers = POST_HEADERS_DEFAULT.copy()
-                headers.update({"Authorization": f"Bearer IGT:2:{self.token}"})
-                params = json.dumps(
-                    {
-                        "text_post_app_info": '{"reply_control":0}',
-                        "scene_capture_type": "",
-                        "timezone_offset": "-25200",
-                        "source_type": "4",
-                        "_uid": self.user_id,
-                        "device_id": str(self.device_id),
-                        "caption": caption,
-                        "upload_id": upload_id,
-                        "device": {
-                            "manufacturer": "OnePlus",
-                            "model": "ONEPLUS+A3010",
-                            "android_version": 25,
-                            "android_release": "7.1.1",
-                        },
-                    }
-                )
-                payload = f"signed_body=SIGNATURE.{urllib.parse.quote(params)}"
-
-                with self.http_client.post(
-                    POST_WITH_IMAGE_URL, headers=headers, data=payload
-                ) as res:
-                    post_result = res.json()
-                    if "status" in post_result.keys() and post_result["status"] == "ok":
-                        return True
-                    else:
-                        return False
-            except Exception as e:
-                print("[ERROR] ", e)
-                return False
-        else:
-            return False
+        return self.publish(caption=caption, image_path=image_path)
 
     def upload_image(self, image_url: str, image_content: bytes) -> str:
-        headers = POST_HEADERS_DEFAULT.copy()
-        headers.update({"Authorization": f"Bearer IGT:2:{self.token}"})
+        headers = self.__get_app_headers().copy()
 
         upload_id = int(time.time() * 1000)
         name = f"{upload_id}_0_{random.randint(1000000000, 9999999999)}"
         url = "https://www.instagram.com/rupload_igphoto/" + name
-
+        mime_type = None
         if image_content is None:
             f = open(image_url, mode="rb")
             content = f.read()
             f.close()
             mime_type, _ = mimetypes.guess_type(image_url)
         else:
             content = image_content
             response = requests.head(image_url)
             content_type = response.headers.get("Content-Type")
             if not content_type:
                 file_name = url.split("/")[-1]
                 mime_type, _ = mimetypes.guess_type(file_name)
+            if mime_type == None:
+                mime_type = "jpeg"
 
         x_instagram_rupload_params = {
             "upload_id": f"{upload_id}",
             "media_type": "1",
             "sticker_burnin_params": "[]",
             "image_compression": json.dumps(
                 {"lib_name": "moz", "lib_version": "3.1.m", "quality": "80"}
@@ -598,10 +725,10 @@
             "Content-Length": f"{contentLength}",
             "Accept-Encoding": "gzip",
         }
 
         headers.update(image_headers)
         response = self.http_client.post(url, headers=headers, data=content)
         if response.status_code == 200:
-            return response.text
+            return response.json()
         else:
             return None
```

### Comparing `threads-py-0.0.6/threadspy/types/common.py` & `threads_py-0.0.7/threadspy/types/common.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.6/threadspy/types/post.py` & `threads_py-0.0.7/threadspy/types/post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.6/threadspy/types/quoted_post.py` & `threads_py-0.0.7/threadspy/types/quoted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.6/threadspy/types/reposted_post.py` & `threads_py-0.0.7/threadspy/types/reposted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.6/threadspy/types/threads_user.py` & `threads_py-0.0.7/threadspy/types/threads_user.py`

 * *Files identical despite different names*

