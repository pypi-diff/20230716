# Comparing `tmp/Abg-2.3.2.tar.gz` & `tmp/Abg-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-2.3.2.tar", last modified: Thu Jul 13 11:24:17 2023, max compression
+gzip compressed data, was "Abg-2.3.3.tar", last modified: Sun Jul 16 14:45:33 2023, max compression
```

## Comparing `Abg-2.3.2.tar` & `Abg-2.3.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.584144 Abg-2.3.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.572145 Abg-2.3.2/Abg/
--rw-r--r--   0 root         (0) root         (0)      325 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.576145 Abg-2.3.2/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/get_user.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/msg_types.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/ratelimit.py
--rw-r--r--   0 root         (0) root         (0)     5335 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.576145 Abg-2.3.2/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11979 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/decorators/
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11704 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/adminsOnly.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/on_cb.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/on_cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.576145 Abg-2.3.2/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5221 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      937 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5221 2023-07-13 11:24:17.584144 Abg-2.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2657 2023-07-13 11:24:00.000000 Abg-2.3.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 11:24:17.584144 Abg-2.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3006 2023-07-13 11:24:00.000000 Abg-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.429920 Abg-2.3.3/Abg/
+-rw-r--r--   0 root         (0) root         (0)      325 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/get_user.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/msg_types.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/ratelimit.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/Abg/patch/decorators/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13387 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/adminsOnly.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/on_cb.py
+-rw-r--r--   0 root         (0) root         (0)     5333 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/on_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/Abg/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.429920 Abg-2.3.3/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-16 14:45:33.437919 Abg-2.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2657 2023-07-16 14:45:05.000000 Abg-2.3.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 14:45:33.437919 Abg-2.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-07-16 14:45:05.000000 Abg-2.3.3/setup.py
```

### Comparing `Abg-2.3.2/Abg/helpers/__init__.py` & `Abg-2.3.3/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/get_user.py` & `Abg-2.3.3/Abg/helpers/get_user.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/helpers.py` & `Abg-2.3.3/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/http_helper.py` & `Abg-2.3.3/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/human_read.py` & `Abg-2.3.3/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/msg_types.py` & `Abg-2.3.3/Abg/helpers/msg_types.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/parser.py` & `Abg-2.3.3/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/pyro_progress.py` & `Abg-2.3.3/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/ratelimit.py` & `Abg-2.3.3/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/helpers/string.py` & `Abg-2.3.3/Abg/helpers/string.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/inline/inline_keyboard.py` & `Abg-2.3.3/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/inline/inline_pagination_keyboard.py` & `Abg-2.3.3/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/inline/reply_keyboard.py` & `Abg-2.3.3/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/patch/bound/message.py` & `Abg-2.3.3/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/patch/decorators/adminsOnly.py` & `Abg-2.3.3/Abg/patch/decorators/adminsOnly.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import typing
 from functools import wraps
 from logging import getLogger
 from typing import Union
 
 import pyrogram
 from cachetools import TTLCache
@@ -10,14 +11,28 @@
 from pyrogram.methods import Decorators
 from pyrogram.types import CallbackQuery, ChatPrivileges, Message
 
 LOGGER = getLogger(__name__)
 
 ANON = TTLCache(maxsize=250, ttl=30)
 
+# ENV
+try:
+    OWNER_ID = int(os.environ.get("OWNER_ID"))
+except ValueError:
+    raise Exception("Your OWNER_ID env variable is not a valid integer.")
+
+try:
+    DEV_USERS = {int(x) for x in os.environ.get("DEV_USER", "").split()}
+except ValueError:
+    raise Exception("Your DEV_USER list does not contain valid integers.")
+
+DEV_USER = list(DEV_USERS)
+DEVS = list(set([int(OWNER_ID)] + DEV_USER))
+
 
 async def anonymous_admin_verification(
     self, CallbackQuery: pyrogram.types.CallbackQuery
 ):
     if int(
         f"{CallbackQuery.message.chat.id}{CallbackQuery.data.split('.')[1]}"
     ) not in set(ANON.keys()):
@@ -59,47 +74,48 @@
 def adminsOnly(
     self,
     permissions: Union[list, str] = None,
     is_bot: bool = False,
     is_user: bool = False,
     is_both: bool = False,
     only_owner: bool = False,
+    only_dev: bool = False,
     no_reply: object = False,
     pass_anon: typing.Union[bool, bool] = False,
 ):
     """Check for permission level to perform some operations
 
     Args:
         permissions (str, optional): permission type to check. Defaults to None.
         is_bot (bool, optional): If bot can perform the action. Defaults to False.
         is_user (bool, optional): If user can perform the action. Defaults to False.
         is_both (bool, optional): If both user and bot can perform the action. Defaults to False.
-        only_owner (bool, optional): If only owner can perform the action. Defaults to False.
-        no_reply (boot, optional): If should not reply. Defaults to False.
+        only_owner (bool, optional): If only owner can perform the action. Defaults to False. (It's Chat Owner)
+        only_dev (bool, optional): if only dev users can perform the operation. Defaults to False.
+        no_reply (boot, optional): If should not reply. Defaults to False. (when isinstance is `callback` it's give alert and if isinstance is `command` it's give reply)
         pass_anon (boot, optional): If the user is an Anonymous Admin, then it bypasses his right check.
     """
 
     def decorator(func):
         @wraps(func)
         async def wrapper(
             abg: Client, message: Union[CallbackQuery, Message], *args, **kwargs
         ):
             if isinstance(message, CallbackQuery):
                 msg = message.message
             elif isinstance(message, Message):
                 msg = message
-                is_anon = message.sender_chat
             else:
                 raise NotImplementedError(
                     f"require_admin can't process updates with the type '{message.__name__}' yet."
                 )
             chat = msg.chat
             user = msg.from_user
 
-            if msg.chat.type == ChatType.PRIVATE:
+            if msg.chat.type == ChatType.PRIVATE and not (only_dev or only_owner):
                 return await func(abg, message, *args, *kwargs)
 
             if msg.chat.type == ChatType.CHANNEL:
                 return await func(abg, message, *args, *kwargs)
 
             if not message.from_user and not pass_anon:
                 ANON[int(f"{msg.chat.id}{msg.id}")] = (
@@ -128,23 +144,39 @@
                 else None
             )
             user = (
                 await abg.get_chat_member(chat.id, user.id)
                 if is_user or is_both
                 else None
             )
-            # looks like todo for now (when pyrogram support `ChatMemberOwner`)
             if only_owner:
-                if user.status in ChatMemberStatus.OWNER:
+                user_ = await msg.chat.get_member(msg.from_user.id)
+                if user_.status == ChatMemberStatus.OWNER:
                     return await func(abg, message, *args, **kwargs)
+                elif no_reply:
+                    return await msg.answer(
+                        "ᴏɴʟʏ ᴄʜᴀᴛ ᴏᴡɴᴇʀ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ.", show_alert=True
+                    )
                 else:
-                    return await msg.reply_text(
+                    return await message.reply_text(
                         "ᴏɴʟʏ ᴄʜᴀᴛ ᴏᴡɴᴇʀ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ."
                     )
 
+            if only_dev:
+                if msg.from_user.id in DEVS:
+                    return await func(abg, message, *args, **kwargs)
+                elif no_reply:
+                    return await msg.answer(
+                        "ᴏɴʟʏ ᴏɴʟʏ ʙᴏᴛ ᴅᴇᴠ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ.", show_alert=True
+                    )
+                else:
+                    return await message.reply_text(
+                        "ᴏɴʟʏ ʙᴏᴛ ᴅᴇᴠ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ.",
+                    )
+
             if permissions:
                 if permissions == "can_promote_members":
                     no_permission = "ᴀᴅᴅ ɴᴇᴡ ᴀᴅᴍɪɴs"
                 elif permissions == "can_change_info":
                     no_permission = "ᴄʜᴀɴɢᴇ ɢʀᴏᴜᴘ ɪɴғᴏ"
                 elif permissions == "can_pin_messages":
                     no_permission = "ᴘɪɴ/ᴜɴᴘɪɴ ᴍᴇssᴀɢᴇs"
@@ -174,15 +206,15 @@
                         return await message.reply_text(
                             f"ɪ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}."
                         )
                 if is_user:
                     if (
                         getattr(user.privileges, permissions)
                         if isinstance(user.privileges, ChatPrivileges)
-                        else False
+                        else False or user.id in DEVS
                     ):
                         return await func(abg, message, *args, **kwargs)
                     elif no_reply:
                         return await msg.answer(
                             f"ʏᴏᴜ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}",
                             show_alert=True,
                         )
@@ -206,15 +238,15 @@
                         return await message.reply_text(
                             f"ɪ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}."
                         )
 
                     if (
                         getattr(user.privileges, permissions)
                         if isinstance(user.privileges, ChatPrivileges)
-                        else False
+                        else False or user.id in DEVS
                     ):
                         pass
                     elif no_reply:
                         return await msg.answer(
                             f"ʏᴏᴜ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}",
                             show_alert=True,
                         )
@@ -231,27 +263,31 @@
                             return await message.reply_text("ɪ'ᴍ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
                     elif is_user:
                         if user.status in [
                             ChatMemberStatus.ADMINISTRATOR,
                             ChatMemberStatus.OWNER,
                         ]:
                             return await func(abg, message, *args, **kwargs)
+                        elif user.id in DEVS:
+                            return await func(abg, message, *args, **kwargs)
                         else:
                             return await message.reply_text("ʏᴏᴜ ᴀʀᴇ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
                     elif is_both:
                         if user.status == ChatMemberStatus.ADMINISTRATOR:
                             pass
                         else:
                             return await message.reply_text("ɪ'ᴍ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
 
                         if user.status in [
                             ChatMemberStatus.ADMINISTRATOR,
                             ChatMemberStatus.OWNER,
                         ]:
                             pass
+                        elif user.id in DEVS:
+                            pass
                         else:
                             return await message.reply_text("ʏᴏᴜ ᴀʀᴇ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
                         return await func(abg, message, *args, **kwargs)
 
         self.add_handler(
             pyrogram.handlers.CallbackQueryHandler(
                 anonymous_admin_verification,
```

### Comparing `Abg-2.3.2/Abg/patch/decorators/on_cb.py` & `Abg-2.3.3/Abg/patch/decorators/on_cb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import asyncio
 import typing
 from logging import getLogger
 
 import pyrogram
-from pyrogram.errors import (
-    ChatAdminRequired,
-    FloodWait,
-    Forbidden,
-    MessageNotModified,
-    SlowmodeWait,
-)
+from pyrogram.errors import ChatAdminRequired, FloodWait, Forbidden, MessageNotModified
 from pyrogram.methods import Decorators
 
+from .utils import handle_error
+
 LOGGER = getLogger(__name__)
 
 
 def callback(
     self,
     data: typing.Union[str, list],
     self_admin: typing.Union[bool, bool] = False,
@@ -86,24 +82,21 @@
                 LOGGER.info(
                     "The message was not modified because you tried to edit it using the same content "
                 )
                 return await CallbackQuery.answer(
                     "The message was not modified because you tried to edit it using the same content ",
                     show_alert=True,
                 )
-            except (Forbidden, SlowmodeWait, ChatAdminRequired):
+            except (Forbidden, ChatAdminRequired):
                 LOGGER.info(
                     f"You cannot write in this chat: {CallbackQuery.message.chat.title} [{CallbackQuery.message.chat.id}]"
                 )
-                return await CallbackQuery.answer(
-                    "Bot need to message write permission "
-                )
+                return await CallbackQuery.answer("Bot need to be  Admin permission ")
             except BaseException as e:
-                LOGGER.error(f"Error Found in callback Handler : {e}")
-                return await CallbackQuery.message.edit_text(f"ᴇʀʀᴏʀ ғᴏᴜɴᴅ:\n{e}")
+                return await handle_error(e, CallbackQuery)
 
         self.add_handler(pyrogram.handlers.CallbackQueryHandler(decorator, filter))
         return decorator
 
     return wrapper
```

### Comparing `Abg-2.3.2/Abg/patch/decorators/on_cmd.py` & `Abg-2.3.3/Abg/patch/decorators/on_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import asyncio
 import typing
 from logging import getLogger
 
 import pyrogram
-from pyrogram.errors import ChatAdminRequired, FloodWait, Forbidden, SlowmodeWait
+from pyrogram.errors import FloodWait, Forbidden, SlowmodeWait
 from pyrogram.methods import Decorators
 
+from .utils import handle_error
+
 HANDLER = ["/", "!", "~", ".", "+", "*", "$"]
 
 LOGGER = getLogger(__name__)
 
 
 def command(
     self,
@@ -111,22 +113,21 @@
             if pm_only and message.chat.type != pyrogram.enums.ChatType.PRIVATE:
                 return await message.reply_text("ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ ʙᴇ ᴜsᴇᴅ ɪɴ ᴘᴍs ᴏɴʟʏ.")
             try:
                 await func(client, message)
             except FloodWait as fw:
                 LOGGER.warning(str(fw))
                 await asyncio.sleep(fw.value)
-            except (Forbidden, SlowmodeWait, ChatAdminRequired):
+            except (Forbidden, SlowmodeWait):
                 LOGGER.info(
                     f"Leaving chat : {message.chat.title} [{message.chat.id}], because doesn't have admin permission."
                 )
                 return await client.leave_chat(message.chat.id)
             except BaseException as e:
-                LOGGER.error(f"Error found in command handler: {e}")
-                return await message.reply_text(f"ᴇʀʀᴏʀ ғᴏᴜɴᴅ:\n{e}")
+                return await handle_error(e, message)
 
         self.add_handler(
             pyrogram.handlers.MessageHandler(callback=decorator, filters=filter)
         )
         return decorator
 
     return wrapper
```

### Comparing `Abg-2.3.2/Abg/patch/listen/listen.py` & `Abg-2.3.3/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/patch/listen/utils.py` & `Abg-2.3.3/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/patch/methods/edit_message_text.py` & `Abg-2.3.3/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/patch/methods/send_as_file.py` & `Abg-2.3.3/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg/patch/methods/send_message.py` & `Abg-2.3.3/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/Abg.egg-info/PKG-INFO` & `Abg-2.3.3/Abg.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,20 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3.2
+Version: 2.3.3
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69/Abg
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
-Description: # ᴀʙɢ :-> [![Downloads](https://static.pepy.tech/personalized-badge/abg?period=total&units=abbreviation&left_color=black&right_color=black&left_text=Downloads:)](https://pepy.tech/project/abg)
-        
-        > 
-        ### • Abg
-        
-        ```python
-        from pyrogram import filters, Client
-        from pyrogram.types import CallbackQuery, Message
-        from Abg import patch  # type : ignore
-        from Abg.helpers import ikb
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("myinfo")
-        async def my_info(self: Client, ctx: Message):
-            if not ctx.from_user:
-                return
-            name = await ctx.chat.ask("Type Your Name")
-            age = await ctx.chat.ask("Type your age")
-            add = await ctx.chat.ask("Type your address")
-            # you can also use : ctx.reply_text(...)
-            await self.send_msg(
-                chat_id=ctx.chat.id,
-                text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
-                reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
-            )
-        
-        # callback 
-        @app.on_cb("hello")
-        async def hello(c: Client, q: CallbackQuery):
-            await q.answer("Hello From Abg", show_alert=True)
-        
-          app.run()
-        ```
-        >
-        ### • User Rights 
-        
-        ```python
-        from Abg import patch  # all patch
-        from pyrogram.types import Message
-        from pyrogram import Client
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("del", group_only=True)
-        @app.adminsOnly(permissions="can_delete_messages", is_both=True)
-        async def del_msg(c: Client, m: Message):
-            if m.reply_to_message:
-                await m.delete()
-                await c.delete_messages(
-                    chat_id=m.chat.id,
-                    message_ids=m.reply_to_message.id,
-                )
-            else:
-                await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
-            return
-          
-          app.run()
-        ```
-        
-        
-        >
-        ### • Keyboards
-        
-        ```python
-        from Abg.inline import InlineKeyboard, InlineButton
-        
-        
-        keyboard = InlineKeyboard(row_width=3)
-        keyboard.add(
-            InlineButton('1', 'inline_keyboard:1'),
-            InlineButton('2', 'inline_keyboard:2'),
-            InlineButton('3', 'inline_keyboard:3'),
-            InlineButton('4', 'inline_keyboard:4'),
-            InlineButton('5', 'inline_keyboard:5'),
-            InlineButton('6', 'inline_keyboard:6'),
-            InlineButton('7', 'inline_keyboard:7')
-        )
-        ```
-        
-        #### Result
-        
-        <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
-        
-        
-        ### ɪɴsᴛᴀʟʟɪɴɢ :->
-        
-        ```bash
-        pip install -U Abg
-        ```
-        
-        ━━━━━━━━━━━━━━━━━━━━
-        ## ɴᴏᴛᴇ :->
-        
-        - This library is made for my personal Project so don't take it deeply .
-        - My Project [@GuardxRobot](https://t.me/GuardxRobot) 
-        
-        - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
-        
-        ━━━━━━━━━━━━━━━━━━━━ 
-        
-        
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -133,7 +31,111 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+
+# ᴀʙɢ :-> [![Downloads](https://static.pepy.tech/personalized-badge/abg?period=total&units=abbreviation&left_color=black&right_color=black&left_text=Downloads:)](https://pepy.tech/project/abg)
+
+> 
+### • Abg
+
+```python
+from pyrogram import filters, Client
+from pyrogram.types import CallbackQuery, Message
+from Abg import patch  # type : ignore
+from Abg.helpers import ikb
+
+app = Client("my_account")
+
+@app.on_cmd("myinfo")
+async def my_info(self: Client, ctx: Message):
+    if not ctx.from_user:
+        return
+    name = await ctx.chat.ask("Type Your Name")
+    age = await ctx.chat.ask("Type your age")
+    add = await ctx.chat.ask("Type your address")
+    # you can also use : ctx.reply_text(...)
+    await self.send_msg(
+        chat_id=ctx.chat.id,
+        text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+        reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
+    )
+
+# callback 
+@app.on_cb("hello")
+async def hello(c: Client, q: CallbackQuery):
+    await q.answer("Hello From Abg", show_alert=True)
+
+  app.run()
+```
+>
+### • User Rights 
+
+```python
+from Abg import patch  # all patch
+from pyrogram.types import Message
+from pyrogram import Client
+
+app = Client("my_account")
+
+@app.on_cmd("del", group_only=True)
+@app.adminsOnly(permissions="can_delete_messages", is_both=True)
+async def del_msg(c: Client, m: Message):
+    if m.reply_to_message:
+        await m.delete()
+        await c.delete_messages(
+            chat_id=m.chat.id,
+            message_ids=m.reply_to_message.id,
+        )
+    else:
+        await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
+    return
+  
+  app.run()
+```
+
+
+>
+### • Keyboards
+
+```python
+from Abg.inline import InlineKeyboard, InlineButton
+
+
+keyboard = InlineKeyboard(row_width=3)
+keyboard.add(
+    InlineButton('1', 'inline_keyboard:1'),
+    InlineButton('2', 'inline_keyboard:2'),
+    InlineButton('3', 'inline_keyboard:3'),
+    InlineButton('4', 'inline_keyboard:4'),
+    InlineButton('5', 'inline_keyboard:5'),
+    InlineButton('6', 'inline_keyboard:6'),
+    InlineButton('7', 'inline_keyboard:7')
+)
+```
+
+#### Result
+
+<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+
+
+### ɪɴsᴛᴀʟʟɪɴɢ :->
+
+```bash
+pip install -U Abg
+```
+
+━━━━━━━━━━━━━━━━━━━━
+## ɴᴏᴛᴇ :->
+
+- This library is made for my personal Project so don't take it deeply .
+- My Project [@GuardxRobot](https://t.me/GuardxRobot) 
+
+- ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
+
+━━━━━━━━━━━━━━━━━━━━ 
+
+
+
```

### Comparing `Abg-2.3.2/Abg.egg-info/SOURCES.txt` & `Abg-2.3.3/Abg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 Abg/patch/__init__.py
 Abg/patch/bound/__init__.py
 Abg/patch/bound/message.py
 Abg/patch/decorators/__init__.py
 Abg/patch/decorators/adminsOnly.py
 Abg/patch/decorators/on_cb.py
 Abg/patch/decorators/on_cmd.py
+Abg/patch/decorators/utils.py
 Abg/patch/listen/__init__.py
 Abg/patch/listen/listen.py
 Abg/patch/listen/utils.py
 Abg/patch/methods/__init__.py
 Abg/patch/methods/edit_message_text.py
 Abg/patch/methods/send_as_file.py
 Abg/patch/methods/send_message.py
```

### Comparing `Abg-2.3.2/PKG-INFO` & `Abg-2.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,20 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3.2
+Version: 2.3.3
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69/Abg
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
-Description: # ᴀʙɢ :-> [![Downloads](https://static.pepy.tech/personalized-badge/abg?period=total&units=abbreviation&left_color=black&right_color=black&left_text=Downloads:)](https://pepy.tech/project/abg)
-        
-        > 
-        ### • Abg
-        
-        ```python
-        from pyrogram import filters, Client
-        from pyrogram.types import CallbackQuery, Message
-        from Abg import patch  # type : ignore
-        from Abg.helpers import ikb
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("myinfo")
-        async def my_info(self: Client, ctx: Message):
-            if not ctx.from_user:
-                return
-            name = await ctx.chat.ask("Type Your Name")
-            age = await ctx.chat.ask("Type your age")
-            add = await ctx.chat.ask("Type your address")
-            # you can also use : ctx.reply_text(...)
-            await self.send_msg(
-                chat_id=ctx.chat.id,
-                text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
-                reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
-            )
-        
-        # callback 
-        @app.on_cb("hello")
-        async def hello(c: Client, q: CallbackQuery):
-            await q.answer("Hello From Abg", show_alert=True)
-        
-          app.run()
-        ```
-        >
-        ### • User Rights 
-        
-        ```python
-        from Abg import patch  # all patch
-        from pyrogram.types import Message
-        from pyrogram import Client
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("del", group_only=True)
-        @app.adminsOnly(permissions="can_delete_messages", is_both=True)
-        async def del_msg(c: Client, m: Message):
-            if m.reply_to_message:
-                await m.delete()
-                await c.delete_messages(
-                    chat_id=m.chat.id,
-                    message_ids=m.reply_to_message.id,
-                )
-            else:
-                await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
-            return
-          
-          app.run()
-        ```
-        
-        
-        >
-        ### • Keyboards
-        
-        ```python
-        from Abg.inline import InlineKeyboard, InlineButton
-        
-        
-        keyboard = InlineKeyboard(row_width=3)
-        keyboard.add(
-            InlineButton('1', 'inline_keyboard:1'),
-            InlineButton('2', 'inline_keyboard:2'),
-            InlineButton('3', 'inline_keyboard:3'),
-            InlineButton('4', 'inline_keyboard:4'),
-            InlineButton('5', 'inline_keyboard:5'),
-            InlineButton('6', 'inline_keyboard:6'),
-            InlineButton('7', 'inline_keyboard:7')
-        )
-        ```
-        
-        #### Result
-        
-        <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
-        
-        
-        ### ɪɴsᴛᴀʟʟɪɴɢ :->
-        
-        ```bash
-        pip install -U Abg
-        ```
-        
-        ━━━━━━━━━━━━━━━━━━━━
-        ## ɴᴏᴛᴇ :->
-        
-        - This library is made for my personal Project so don't take it deeply .
-        - My Project [@GuardxRobot](https://t.me/GuardxRobot) 
-        
-        - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
-        
-        ━━━━━━━━━━━━━━━━━━━━ 
-        
-        
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -133,7 +31,111 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+
+# ᴀʙɢ :-> [![Downloads](https://static.pepy.tech/personalized-badge/abg?period=total&units=abbreviation&left_color=black&right_color=black&left_text=Downloads:)](https://pepy.tech/project/abg)
+
+> 
+### • Abg
+
+```python
+from pyrogram import filters, Client
+from pyrogram.types import CallbackQuery, Message
+from Abg import patch  # type : ignore
+from Abg.helpers import ikb
+
+app = Client("my_account")
+
+@app.on_cmd("myinfo")
+async def my_info(self: Client, ctx: Message):
+    if not ctx.from_user:
+        return
+    name = await ctx.chat.ask("Type Your Name")
+    age = await ctx.chat.ask("Type your age")
+    add = await ctx.chat.ask("Type your address")
+    # you can also use : ctx.reply_text(...)
+    await self.send_msg(
+        chat_id=ctx.chat.id,
+        text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+        reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
+    )
+
+# callback 
+@app.on_cb("hello")
+async def hello(c: Client, q: CallbackQuery):
+    await q.answer("Hello From Abg", show_alert=True)
+
+  app.run()
+```
+>
+### • User Rights 
+
+```python
+from Abg import patch  # all patch
+from pyrogram.types import Message
+from pyrogram import Client
+
+app = Client("my_account")
+
+@app.on_cmd("del", group_only=True)
+@app.adminsOnly(permissions="can_delete_messages", is_both=True)
+async def del_msg(c: Client, m: Message):
+    if m.reply_to_message:
+        await m.delete()
+        await c.delete_messages(
+            chat_id=m.chat.id,
+            message_ids=m.reply_to_message.id,
+        )
+    else:
+        await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
+    return
+  
+  app.run()
+```
+
+
+>
+### • Keyboards
+
+```python
+from Abg.inline import InlineKeyboard, InlineButton
+
+
+keyboard = InlineKeyboard(row_width=3)
+keyboard.add(
+    InlineButton('1', 'inline_keyboard:1'),
+    InlineButton('2', 'inline_keyboard:2'),
+    InlineButton('3', 'inline_keyboard:3'),
+    InlineButton('4', 'inline_keyboard:4'),
+    InlineButton('5', 'inline_keyboard:5'),
+    InlineButton('6', 'inline_keyboard:6'),
+    InlineButton('7', 'inline_keyboard:7')
+)
+```
+
+#### Result
+
+<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+
+
+### ɪɴsᴛᴀʟʟɪɴɢ :->
+
+```bash
+pip install -U Abg
+```
+
+━━━━━━━━━━━━━━━━━━━━
+## ɴᴏᴛᴇ :->
+
+- This library is made for my personal Project so don't take it deeply .
+- My Project [@GuardxRobot](https://t.me/GuardxRobot) 
+
+- ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
+
+━━━━━━━━━━━━━━━━━━━━ 
+
+
+
```

### Comparing `Abg-2.3.2/README.md` & `Abg-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `Abg-2.3.2/setup.py` & `Abg-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="2.3.2",
+    version="2.3.3",
     description="Telegram bot helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69/Abg",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi",
     author_email="Abishnoi69@Abg.org",
```

