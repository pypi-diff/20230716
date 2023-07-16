# Comparing `tmp/pymino-1.2.3.3.tar.gz` & `tmp/pymino-1.2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymino-1.2.3.3.tar", last modified: Sat Jul 15 00:07:18 2023, max compression
+gzip compressed data, was "pymino-1.2.3.4.tar", last modified: Sun Jul 16 00:33:33 2023, max compression
```

## Comparing `pymino-1.2.3.3.tar` & `pymino-1.2.3.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 00:07:18.214981 pymino-1.2.3.3/
--rw-rw-rw-   0        0        0     1085 2023-07-14 23:58:40.000000 pymino-1.2.3.3/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-07-15 00:07:18.214981 pymino-1.2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-07-15 00:06:35.000000 pymino-1.2.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 00:07:18.108213 pymino-1.2.3.3/pymino/
--rw-rw-rw-   0        0        0      775 2023-07-15 00:00:48.000000 pymino-1.2.3.3/pymino/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/async_bot.py
--rw-rw-rw-   0        0        0    37317 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/async_client.py
--rw-rw-rw-   0        0        0    31005 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/bot.py
--rw-rw-rw-   0        0        0    36840 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:07:18.158200 pymino-1.2.3.3/pymino/ext/
--rw-rw-rw-   0        0        0      651 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    11196 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/account.py
--rw-rw-rw-   0        0        0    11496 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/async_account.py
--rw-rw-rw-   0        0        0   345197 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21402 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25878 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0    67975 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/async_global_client.py
--rw-rw-rw-   0        0        0     7233 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   344129 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45520 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1856 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:07:18.190596 pymino-1.2.3.3/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31608 2023-07-14 23:59:58.000000 pymino-1.2.3.3/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    70299 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6657 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:07:18.212984 pymino-1.2.3.3/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11544 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10404 2023-07-14 23:58:40.000000 pymino-1.2.3.3/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:07:18.126481 pymino-1.2.3.3/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-07-15 00:07:18.000000 pymino-1.2.3.3/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1640 2023-07-15 00:07:18.000000 pymino-1.2.3.3/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 00:07:18.000000 pymino-1.2.3.3/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-07-15 00:07:18.000000 pymino-1.2.3.3/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 00:07:18.000000 pymino-1.2.3.3/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-07-15 00:07:18.224037 pymino-1.2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-07-14 23:58:40.000000 pymino-1.2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:33:33.754833 pymino-1.2.3.4/
+-rw-rw-rw-   0        0        0     1085 2023-07-14 23:58:40.000000 pymino-1.2.3.4/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-07-16 00:33:33.754833 pymino-1.2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-07-16 00:32:59.000000 pymino-1.2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 00:33:33.640522 pymino-1.2.3.4/pymino/
+-rw-rw-rw-   0        0        0      775 2023-07-16 00:29:24.000000 pymino-1.2.3.4/pymino/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    37317 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/async_client.py
+-rw-rw-rw-   0        0        0    31005 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/bot.py
+-rw-rw-rw-   0        0        0    36840 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:33:33.692481 pymino-1.2.3.4/pymino/ext/
+-rw-rw-rw-   0        0        0      651 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    11196 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/account.py
+-rw-rw-rw-   0        0        0    11496 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/async_account.py
+-rw-rw-rw-   0        0        0   345197 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21402 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25878 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0    69631 2023-07-16 00:29:06.000000 pymino-1.2.3.4/pymino/ext/async_global_client.py
+-rw-rw-rw-   0        0        0     7233 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344129 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    45520 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1856 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:33:33.736881 pymino-1.2.3.4/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-07-16 00:08:19.000000 pymino-1.2.3.4/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    32441 2023-07-16 00:18:02.000000 pymino-1.2.3.4/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    71945 2023-07-16 00:28:53.000000 pymino-1.2.3.4/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6657 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:33:33.752841 pymino-1.2.3.4/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11544 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10404 2023-07-14 23:58:40.000000 pymino-1.2.3.4/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:33:33.658569 pymino-1.2.3.4/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-07-16 00:33:33.000000 pymino-1.2.3.4/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1640 2023-07-16 00:33:33.000000 pymino-1.2.3.4/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 00:33:33.000000 pymino-1.2.3.4/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-16 00:33:33.000000 pymino-1.2.3.4/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 00:33:33.000000 pymino-1.2.3.4/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-07-16 00:33:33.757825 pymino-1.2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-07-14 23:58:40.000000 pymino-1.2.3.4/setup.py
```

### Comparing `pymino-1.2.3.3/LICENSE` & `pymino-1.2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/PKG-INFO` & `pymino-1.2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.3.3
+Version: 1.2.3.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.3.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.3.3/README.md` & `pymino-1.2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/__init__.py` & `pymino-1.2.3.4/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.3.3'
+__version__ = '1.2.3.4'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 from .async_client import AsyncClient as AsyncClient
```

### Comparing `pymino-1.2.3.3/pymino/async_bot.py` & `pymino-1.2.3.4/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/async_client.py` & `pymino-1.2.3.4/pymino/async_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/bot.py` & `pymino-1.2.3.4/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/client.py` & `pymino-1.2.3.4/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/__init__.py` & `pymino-1.2.3.4/pymino/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/account.py` & `pymino-1.2.3.4/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/async_account.py` & `pymino-1.2.3.4/pymino/ext/async_account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/async_community.py` & `pymino-1.2.3.4/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/async_context.py` & `pymino-1.2.3.4/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/async_event_handler.py` & `pymino-1.2.3.4/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/async_global_client.py` & `pymino-1.2.3.4/pymino/ext/async_global_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,15 +805,14 @@
         """
         return UserProfileList(await self.make_request(
             method = "GET",
             url = f"/g/s/user-profile/{userId}/member?start={start}&size={size}"
         ))
 
 
-    @authenticated
     async def fetch_following(self, userId: str, start: int = 0, size: int = 25) -> UserProfileList:
         """
         Fetches the user profiles of the users that the specified user is following.
 
         :param userId: The ID of the user.
         :type userId: str
         :param start: The index to start fetching from. (Default: 0)
@@ -834,16 +833,50 @@
         ...     print(profile)
         """
         return UserProfileList(await self.make_request(
             method = "GET",
             url = f"/g/s/user-profile/{userId}/joined?start={start}&size={size}"
         ))
 
+    async def large_fetch_following(self, userId: str, size: int = 25, pageToken: str = None, ignoreMembership: bool = True) -> FollowerList:
+        """
+        Fetches the user profiles of the users that the specified user is following.
+        :param userId: The ID of the user.
+        :type userId: str
+        :param size: The number of user profiles to fetch. (Default: 25)
+        :type size: int, optional
+        :param pageToken: The page token to fetch from. (Default: None)
+        :type pageToken: str, optional
+        :param ignoreMembership: Whether to ignore membership. (Default: True)
+        :type ignoreMembership: bool, optional
+        :return: A `FollowerList` object containing the user profiles.
+        :rtype: FollowerList
+        
+        This function sends a GET request to the API to fetch the user profiles of the users that the specified user is following.
+        
+        `FollowerList` represents a list of user profiles.
+        
+        **Example usage:**
+    
+        >>> following = client.large_fetch_following("user123")
+        ... for userId in following.members.userId:
+        ...     print(userId)
+        """
+        if pageToken:
+            return FollowerList(await self.make_request(
+                method = "GET",
+                url = f"/g/s/user-profile/{userId}/joined?size={size}&pageToken={pageToken}&pagingType=t&ignoreMembership={1 if ignoreMembership else 0}"
+            ))
+
+        return FollowerList(await self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/joined?pagingType=t&size={size}&ignoreMembership={1 if ignoreMembership else 0}"
+        ))
+
 
-    @authenticated
     async def fetch_visitors(self, userId: str, start: int = 0, size: int = 25) -> UserProfileList:
         """
         Fetches the visitors of a user profile.
 
         :param userId: The ID of the user profile to fetch visitors for.
         :type userId: str
         :param start: The index of the first visitor to retrieve. (Default: 0)
```

### Comparing `pymino-1.2.3.3/pymino/ext/async_socket.py` & `pymino-1.2.3.4/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/community.py` & `pymino-1.2.3.4/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/console.py` & `pymino-1.2.3.4/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/context.py` & `pymino-1.2.3.4/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/dispatcher.py` & `pymino-1.2.3.4/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/acm.py` & `pymino-1.2.3.4/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/admin_log.py` & `pymino-1.2.3.4/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/api_response.py` & `pymino-1.2.3.4/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/bubble.py` & `pymino-1.2.3.4/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/chat_threads.py` & `pymino-1.2.3.4/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/comments.py` & `pymino-1.2.3.4/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/enums.py` & `pymino-1.2.3.4/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/exceptions.py` & `pymino-1.2.3.4/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/general.py` & `pymino-1.2.3.4/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/handlers.py` & `pymino-1.2.3.4/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/link_info.py` & `pymino-1.2.3.4/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/member.py` & `pymino-1.2.3.4/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/messages.py` & `pymino-1.2.3.4/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/notification.py` & `pymino-1.2.3.4/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/sticker.py` & `pymino-1.2.3.4/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/threads.py` & `pymino-1.2.3.4/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/entities/userprofile.py` & `pymino-1.2.3.4/pymino/ext/entities/userprofile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1319,8 +1319,34 @@
 		self.comments_count:			list = [x.comments_count for x in parser]
 		self.ndcId:						list = [x.ndcId for x in parser]
 		self.comId:						list = self.ndcId
 		self.created_time:				list = [x.created_time for x in parser]
 		#self.extensions:				list = [x.extensions for x in parser]
 		self.visit_privacy:				list = [x.visit_privacy for x in parser]
 		self.stories_count:				list = [x.stories_count for x in parser]
-		self.blogs_count:				list = [x.blogs_count for x in parser]
+		self.blogs_count:				list = [x.blogs_count for x in parser]
+
+class Pagging:
+    def __init__(self, data: dict):
+        self._data = data.get("paging") if isinstance(data, dict) else data
+        self.prev_page_token = None
+        self.next_page_token = None
+
+        if isinstance(data, dict):
+            self.prev_page_token: Union[str, None] = self._data.get("prevPageToken")
+            self.next_page_token: Union[str, None] = self._data.get("nextPageToken")
+    
+    def json(self) -> dict:
+        return self._data
+
+class FollowerList:
+    def __init__(self, data: dict):
+        self._data = data
+        self.paging = None
+        self.members = None
+        
+        if isinstance(data, dict):
+            self.paging = Pagging(self._data)
+            self.members = UserProfileList(self._data)
+    
+    def json(self) -> dict:
+        return self._data
```

### Comparing `pymino-1.2.3.3/pymino/ext/entities/wsevents.py` & `pymino-1.2.3.4/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/global_client.py` & `pymino-1.2.3.4/pymino/ext/global_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -886,15 +886,14 @@
         """
         return UserProfileList(self.make_request(
             method = "GET",
             url = f"/g/s/user-profile/{userId}/member?start={start}&size={size}"
         ))
 
 
-    @authenticated
     def fetch_following(self, userId: str, start: int = 0, size: int = 25) -> UserProfileList:
         """
         Fetches the user profiles of the users that the specified user is following.
 
         :param userId: The ID of the user.
         :type userId: str
         :param start: The index to start fetching from. (Default: 0)
@@ -910,21 +909,55 @@
 
         **Example usage:**
 
         >>> following = client.fetch_following("user123")
         ... for profile in following.userId:
         ...     print(profile)
         """
+        
         return UserProfileList(self.make_request(
             method = "GET",
             url = f"/g/s/user-profile/{userId}/joined?start={start}&size={size}"
         ))
 
+    def large_fetch_following(self, userId: str, size: int = 25, pageToken: str = None, ignoreMembership: bool = True) -> FollowerList:
+        """
+        Fetches the user profiles of the users that the specified user is following.
+        :param userId: The ID of the user.
+        :type userId: str
+        :param size: The number of user profiles to fetch. (Default: 25)
+        :type size: int, optional
+        :param pageToken: The page token to fetch from. (Default: None)
+        :type pageToken: str, optional
+        :param ignoreMembership: Whether to ignore membership. (Default: True)
+        :type ignoreMembership: bool, optional
+        :return: A `FollowerList` object containing the user profiles.
+        :rtype: FollowerList
+        
+        This function sends a GET request to the API to fetch the user profiles of the users that the specified user is following.
+        
+        `FollowerList` represents a list of user profiles.
+        
+        **Example usage:**
+    
+        >>> following = client.large_fetch_following("user123")
+        ... for userId in following.members.userId:
+        ...     print(userId)
+        """
+        if pageToken:
+            return FollowerList(self.make_request(
+                method = "GET",
+                url = f"/g/s/user-profile/{userId}/joined?size={size}&pageToken={pageToken}&pagingType=t&ignoreMembership={1 if ignoreMembership else 0}"
+            ))
+
+        return FollowerList(self.make_request(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/joined?pagingType=t&size={size}&ignoreMembership={1 if ignoreMembership else 0}"
+        ))
 
-    @authenticated
     def fetch_visitors(self, userId: str, start: int = 0, size: int = 25) -> UserProfileList:
         """
         Fetches the visitors of a user profile.
 
         :param userId: The ID of the user profile to fetch visitors for.
         :type userId: str
         :param start: The index of the first visitor to retrieve. (Default: 0)
```

### Comparing `pymino-1.2.3.3/pymino/ext/handle_queue.py` & `pymino-1.2.3.4/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/socket.py` & `pymino-1.2.3.4/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.3.4/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/chat_console.py` & `pymino-1.2.3.4/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/commands.py` & `pymino-1.2.3.4/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/community_console.py` & `pymino-1.2.3.4/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/generate.py` & `pymino-1.2.3.4/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/menu.py` & `pymino-1.2.3.4/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/profile_console.py` & `pymino-1.2.3.4/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino/ext/utilities/request_handler.py` & `pymino-1.2.3.4/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/pymino.egg-info/PKG-INFO` & `pymino-1.2.3.4/pymino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.3.3
+Version: 1.2.3.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.3.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.3.3/pymino.egg-info/SOURCES.txt` & `pymino-1.2.3.4/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.3/setup.cfg` & `pymino-1.2.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e33 2e33 0d0a 6175  on = 1.2.3.3..au
+00000020: 6f6e 203d 2031 2e32 2e33 2e34 0d0a 6175  on = 1.2.3.4..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.3.3/setup.py` & `pymino-1.2.3.4/setup.py`

 * *Files identical despite different names*

