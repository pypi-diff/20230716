# Comparing `tmp/threads_py-0.0.7.tar.gz` & `tmp/threads_py-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads_py-0.0.7.tar", max compression
+gzip compressed data, was "threads_py-0.0.8.tar", max compression
```

## Comparing `threads_py-0.0.7.tar` & `threads_py-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1066 2023-07-16 04:06:05.352298 threads_py-0.0.7/LICENSE
--rw-r--r--   0        0        0     5016 2023-07-16 12:39:36.358642 threads_py-0.0.7/README.md
--rw-r--r--   0        0        0      778 2023-07-16 12:42:05.324792 threads_py-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      117 2023-07-16 12:39:36.364127 threads_py-0.0.7/threadspy/__init__.py
--rw-r--r--   0        0        0       58 2023-07-16 12:39:36.364575 threads_py-0.0.7/threadspy/ai/__init__.py
--rw-r--r--   0        0        0     5537 2023-07-16 12:39:36.364749 threads_py-0.0.7/threadspy/ai/agent.py
--rw-r--r--   0        0        0       29 2023-07-16 12:39:36.364876 threads_py-0.0.7/threadspy/ai/templates/__init__.py
--rw-r--r--   0        0        0      128 2023-07-16 12:39:36.364956 threads_py-0.0.7/threadspy/ai/templates/qna.py
--rw-r--r--   0        0        0      261 2023-07-16 12:39:36.365613 threads_py-0.0.7/threadspy/constants.py
--rw-r--r--   0        0        0    25214 2023-07-16 12:39:36.366733 threads_py-0.0.7/threadspy/threads_api.py
--rw-r--r--   0        0        0     1950 2023-07-16 12:39:36.367180 threads_py-0.0.7/threadspy/types/__init__.py
--rw-r--r--   0        0        0      190 2023-07-16 12:39:36.367376 threads_py-0.0.7/threadspy/types/candidate.py
--rw-r--r--   0        0        0      136 2023-07-16 12:39:36.367602 threads_py-0.0.7/threadspy/types/caption.py
--rw-r--r--   0        0        0      622 2023-07-16 03:01:37.259110 threads_py-0.0.7/threadspy/types/common.py
--rw-r--r--   0        0        0      144 2023-07-16 12:39:36.367812 threads_py-0.0.7/threadspy/types/extensions.py
--rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259277 threads_py-0.0.7/threadspy/types/get_thread_likers_response.py
--rw-r--r--   0        0        0      314 2023-07-16 03:01:37.259370 threads_py-0.0.7/threadspy/types/get_user_profile_replies_response.py
--rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259449 threads_py-0.0.7/threadspy/types/get_user_profile_response.py
--rw-r--r--   0        0        0      315 2023-07-16 03:01:37.259525 threads_py-0.0.7/threadspy/types/get_user_profile_thread_response.py
--rw-r--r--   0        0        0      314 2023-07-16 03:22:06.009163 threads_py-0.0.7/threadspy/types/get_user_profile_threads_response.py
--rw-r--r--   0        0        0      233 2023-07-16 03:43:54.986708 threads_py-0.0.7/threadspy/types/image_versions2.py
--rw-r--r--   0        0        0      216 2023-07-16 03:01:37.259923 threads_py-0.0.7/threadspy/types/media_data.py
--rw-r--r--   0        0        0      772 2023-07-16 03:01:37.260014 threads_py-0.0.7/threadspy/types/post.py
--rw-r--r--   0        0        0      766 2023-07-16 03:01:37.260090 threads_py-0.0.7/threadspy/types/quoted_post.py
--rw-r--r--   0        0        0      191 2023-07-16 12:39:36.368023 threads_py-0.0.7/threadspy/types/reply_facepile_user.py
--rw-r--r--   0        0        0      812 2023-07-16 03:01:37.260232 threads_py-0.0.7/threadspy/types/reposted_post.py
--rw-r--r--   0        0        0      304 2023-07-16 03:01:37.260298 threads_py-0.0.7/threadspy/types/share_info.py
--rw-r--r--   0        0        0      313 2023-07-16 03:42:07.939582 threads_py-0.0.7/threadspy/types/text_post_app_info.py
--rw-r--r--   0        0        0      299 2023-07-16 03:01:37.260436 threads_py-0.0.7/threadspy/types/thread.py
--rw-r--r--   0        0        0      280 2023-07-16 03:01:37.260503 threads_py-0.0.7/threadspy/types/thread_data.py
--rw-r--r--   0        0        0      433 2023-07-16 03:41:29.770812 threads_py-0.0.7/threadspy/types/thread_item.py
--rw-r--r--   0        0        0      142 2023-07-16 03:01:37.260628 threads_py-0.0.7/threadspy/types/threads_bio_link.py
--rw-r--r--   0        0        0      185 2023-07-16 03:01:37.260692 threads_py-0.0.7/threadspy/types/threads_hd_profile_pic_version.py
--rw-r--r--   0        0        0      729 2023-07-16 03:43:52.128369 threads_py-0.0.7/threadspy/types/threads_user.py
--rw-r--r--   0        0        0      222 2023-07-16 03:01:37.260815 threads_py-0.0.7/threadspy/types/threads_user_summary.py
--rw-r--r--   0        0        0      198 2023-07-16 03:01:37.260877 threads_py-0.0.7/threadspy/types/user_data.py
--rw-r--r--   0        0        0      200 2023-07-16 03:01:37.260949 threads_py-0.0.7/threadspy/types/user_profile_data.py
--rw-r--r--   0        0        0      230 2023-07-16 03:01:37.261016 threads_py-0.0.7/threadspy/types/users.py
--rw-r--r--   0        0        0      176 2023-07-16 12:39:36.368230 threads_py-0.0.7/threadspy/types/video_version.py
--rw-r--r--   0        0        0     6922 1970-01-01 00:00:00.000000 threads_py-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-16 04:06:05.352298 threads_py-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5016 2023-07-16 13:38:52.326551 threads_py-0.0.8/README.md
+-rw-r--r--   0        0        0      783 2023-07-16 13:38:50.963547 threads_py-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-07-16 13:38:44.023233 threads_py-0.0.8/threadspy/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-16 12:39:36.364575 threads_py-0.0.8/threadspy/ai/__init__.py
+-rw-r--r--   0        0        0     5537 2023-07-16 12:39:36.364749 threads_py-0.0.8/threadspy/ai/agent.py
+-rw-r--r--   0        0        0       29 2023-07-16 12:39:36.364876 threads_py-0.0.8/threadspy/ai/templates/__init__.py
+-rw-r--r--   0        0        0      128 2023-07-16 12:39:36.364956 threads_py-0.0.8/threadspy/ai/templates/qna.py
+-rw-r--r--   0        0        0      261 2023-07-16 12:39:36.365613 threads_py-0.0.8/threadspy/constants.py
+-rw-r--r--   0        0        0    25214 2023-07-16 12:39:36.366733 threads_py-0.0.8/threadspy/threads_api.py
+-rw-r--r--   0        0        0     1950 2023-07-16 12:39:36.367180 threads_py-0.0.8/threadspy/types/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-16 12:39:36.367376 threads_py-0.0.8/threadspy/types/candidate.py
+-rw-r--r--   0        0        0      136 2023-07-16 12:39:36.367602 threads_py-0.0.8/threadspy/types/caption.py
+-rw-r--r--   0        0        0      622 2023-07-16 03:01:37.259110 threads_py-0.0.8/threadspy/types/common.py
+-rw-r--r--   0        0        0      144 2023-07-16 12:39:36.367812 threads_py-0.0.8/threadspy/types/extensions.py
+-rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259277 threads_py-0.0.8/threadspy/types/get_thread_likers_response.py
+-rw-r--r--   0        0        0      314 2023-07-16 03:01:37.259370 threads_py-0.0.8/threadspy/types/get_user_profile_replies_response.py
+-rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259449 threads_py-0.0.8/threadspy/types/get_user_profile_response.py
+-rw-r--r--   0        0        0      315 2023-07-16 03:01:37.259525 threads_py-0.0.8/threadspy/types/get_user_profile_thread_response.py
+-rw-r--r--   0        0        0      314 2023-07-16 03:22:06.009163 threads_py-0.0.8/threadspy/types/get_user_profile_threads_response.py
+-rw-r--r--   0        0        0      233 2023-07-16 03:43:54.986708 threads_py-0.0.8/threadspy/types/image_versions2.py
+-rw-r--r--   0        0        0      216 2023-07-16 03:01:37.259923 threads_py-0.0.8/threadspy/types/media_data.py
+-rw-r--r--   0        0        0      772 2023-07-16 03:01:37.260014 threads_py-0.0.8/threadspy/types/post.py
+-rw-r--r--   0        0        0      766 2023-07-16 03:01:37.260090 threads_py-0.0.8/threadspy/types/quoted_post.py
+-rw-r--r--   0        0        0      191 2023-07-16 12:39:36.368023 threads_py-0.0.8/threadspy/types/reply_facepile_user.py
+-rw-r--r--   0        0        0      812 2023-07-16 03:01:37.260232 threads_py-0.0.8/threadspy/types/reposted_post.py
+-rw-r--r--   0        0        0      304 2023-07-16 03:01:37.260298 threads_py-0.0.8/threadspy/types/share_info.py
+-rw-r--r--   0        0        0      313 2023-07-16 03:42:07.939582 threads_py-0.0.8/threadspy/types/text_post_app_info.py
+-rw-r--r--   0        0        0      299 2023-07-16 03:01:37.260436 threads_py-0.0.8/threadspy/types/thread.py
+-rw-r--r--   0        0        0      280 2023-07-16 03:01:37.260503 threads_py-0.0.8/threadspy/types/thread_data.py
+-rw-r--r--   0        0        0      433 2023-07-16 03:41:29.770812 threads_py-0.0.8/threadspy/types/thread_item.py
+-rw-r--r--   0        0        0      142 2023-07-16 03:01:37.260628 threads_py-0.0.8/threadspy/types/threads_bio_link.py
+-rw-r--r--   0        0        0      185 2023-07-16 03:01:37.260692 threads_py-0.0.8/threadspy/types/threads_hd_profile_pic_version.py
+-rw-r--r--   0        0        0      729 2023-07-16 03:43:52.128369 threads_py-0.0.8/threadspy/types/threads_user.py
+-rw-r--r--   0        0        0      222 2023-07-16 03:01:37.260815 threads_py-0.0.8/threadspy/types/threads_user_summary.py
+-rw-r--r--   0        0        0      198 2023-07-16 03:01:37.260877 threads_py-0.0.8/threadspy/types/user_data.py
+-rw-r--r--   0        0        0      200 2023-07-16 03:01:37.260949 threads_py-0.0.8/threadspy/types/user_profile_data.py
+-rw-r--r--   0        0        0      230 2023-07-16 03:01:37.261016 threads_py-0.0.8/threadspy/types/users.py
+-rw-r--r--   0        0        0      176 2023-07-16 12:39:36.368230 threads_py-0.0.8/threadspy/types/video_version.py
+-rw-r--r--   0        0        0     6927 1970-01-01 00:00:00.000000 threads_py-0.0.8/PKG-INFO
```

### Comparing `threads_py-0.0.7/LICENSE` & `threads_py-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/README.md` & `threads_py-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,26 +93,26 @@
 api.publish({
   text: '🤖 Beep',
   link: 'https://github.com/junhoyeo/threads-py',
   parent_post_id: parent_post_id,
 })
 ```
 
-#### ✨ Like/Unlike a Thread (from v0.0.7)
+#### ✨ Like/Unlike a Thread (from v0.0.8)
 
 ```python
 post_url = 'https://www.threads.net/t/CugF-EjhQ3r'
 post_id = api.get_post_id_from_url(post_url) # or use `get_post_id_from_thread_id`
 
 # 💡 Uses current credentials
 api.like(postIDToLike)
 api.unlike(postIDToLike)
 ```
 
-#### ✨ Follow/Unfollow a User (from v0.0.7)
+#### ✨ Follow/Unfollow a User (from v0.0.8)
 
 ```python
 user_id_to_follow = api.get_user_id_from_username('junhoyeo')
 
 # 💡 Uses current credentials
 api.follow(user_id_to_follow)
 api.unfollow(user_id_to_follow)
```

### Comparing `threads_py-0.0.7/pyproject.toml` & `threads_py-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 packages = [{ include = "threadspy", from = "." }]
 name = "threads-py"
-version = "0.0.7"
+version = "0.0.8"
 description = "Unofficial, Reverse-Engineered Python client for Meta's Threads."
 license = "MIT"
 authors = [
   "Junho Yeo <i@junho.io>",
   "iamiks <rmstjr1030@naver.com>",
   "DrunkLeen <reza.df.x@gmail.com>",
   "Ashrf <ashrftvm1@gmail.com>",
@@ -16,13 +16,13 @@
 keywords = ["threads", "instagram", "facebook", "meta", "api"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2.31.0"
 dataclasses = "^0.6"
 dataclasses-json = "^0.5.9"
-pycrypto = "^2.6.1"
+pycryptodome = "^3.18.0"
 
 [tool.poetry.group.ai]
 optional = true
 [tool.poetry.group.ai.dependencies]
 langchain = "^0.0.227"
```

### Comparing `threads_py-0.0.7/threadspy/ai/agent.py` & `threads_py-0.0.8/threadspy/ai/agent.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/threadspy/threads_api.py` & `threads_py-0.0.8/threadspy/threads_api.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/threadspy/types/__init__.py` & `threads_py-0.0.8/threadspy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/threadspy/types/common.py` & `threads_py-0.0.8/threadspy/types/common.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/threadspy/types/post.py` & `threads_py-0.0.8/threadspy/types/post.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/threadspy/types/quoted_post.py` & `threads_py-0.0.8/threadspy/types/quoted_post.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/threadspy/types/reposted_post.py` & `threads_py-0.0.8/threadspy/types/reposted_post.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/threadspy/types/threads_user.py` & `threads_py-0.0.8/threadspy/types/threads_user.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.7/PKG-INFO` & `threads_py-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: threads-py
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unofficial, Reverse-Engineered Python client for Meta's Threads.
 Home-page: https://github.com/junhoyeo/threads-py
 License: MIT
 Keywords: threads,instagram,facebook,meta,api
 Author: Junho Yeo
 Author-email: i@junho.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses (>=0.6,<0.7)
 Requires-Dist: dataclasses-json (>=0.5.9,<0.6.0)
-Requires-Dist: pycrypto (>=2.6.1,<3.0.0)
+Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/junhoyeo/threads-py
 Description-Content-Type: text/markdown
 
 # [<img src="./.github/logo.jpg" width="36" height="36" />](https://github.com/junhoyeo) threads-py
 
 [![pypi](https://img.shields.io/pypi/v/threads-py.svg?style=flat-square&labelColor=black)](https://pypi.org/project/threads-py) [![MIT License](https://img.shields.io/badge/license-MIT-blue?style=flat-square&labelColor=black)](https://github.com/junhoyeo/threads-py/blob/main/LICENSE)
@@ -115,26 +115,26 @@
 api.publish({
   text: '🤖 Beep',
   link: 'https://github.com/junhoyeo/threads-py',
   parent_post_id: parent_post_id,
 })
 ```
 
-#### ✨ Like/Unlike a Thread (from v0.0.7)
+#### ✨ Like/Unlike a Thread (from v0.0.8)
 
 ```python
 post_url = 'https://www.threads.net/t/CugF-EjhQ3r'
 post_id = api.get_post_id_from_url(post_url) # or use `get_post_id_from_thread_id`
 
 # 💡 Uses current credentials
 api.like(postIDToLike)
 api.unlike(postIDToLike)
 ```
 
-#### ✨ Follow/Unfollow a User (from v0.0.7)
+#### ✨ Follow/Unfollow a User (from v0.0.8)
 
 ```python
 user_id_to_follow = api.get_user_id_from_username('junhoyeo')
 
 # 💡 Uses current credentials
 api.follow(user_id_to_follow)
 api.unfollow(user_id_to_follow)
```

