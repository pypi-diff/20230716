# Comparing `tmp/signalbot-0.6.0.tar.gz` & `tmp/signalbot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signalbot-0.6.0.tar", max compression
+gzip compressed data, was "signalbot-0.7.0.tar", max compression
```

## Comparing `signalbot-0.6.0.tar` & `signalbot-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1051 2022-03-13 21:44:12.886721 signalbot-0.6.0/LICENSE
--rw-r--r--   0        0        0     4480 2022-03-13 21:44:12.886721 signalbot-0.6.0/README.md
--rw-r--r--   0        0        0      796 2022-03-13 21:44:12.886721 signalbot-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      481 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/__init__.py
--rw-r--r--   0        0        0     3901 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/api.py
--rw-r--r--   0        0        0     9739 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/bot.py
--rw-r--r--   0        0        0     1416 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/command.py
--rw-r--r--   0        0        0      787 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/context.py
--rw-r--r--   0        0        0     3442 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/message.py
--rw-r--r--   0        0        0     1763 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/storage.py
--rw-r--r--   0        0        0      249 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/utils/__init__.py
--rw-r--r--   0        0        0     4036 2022-03-13 21:44:12.886721 signalbot-0.6.0/signalbot/utils/chat_testing.py
--rw-r--r--   0        0        0     5318 2022-03-13 21:44:34.599840 signalbot-0.6.0/setup.py
--rw-r--r--   0        0        0     5277 2022-03-13 21:44:34.600317 signalbot-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1051 2023-07-16 18:29:23.896105 signalbot-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4323 2023-07-16 18:29:23.896105 signalbot-0.7.0/README.md
+-rw-r--r--   0        0        0      796 2023-07-16 18:29:23.896105 signalbot-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      481 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/__init__.py
+-rw-r--r--   0        0        0     3901 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/api.py
+-rw-r--r--   0        0        0    11043 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/bot.py
+-rw-r--r--   0        0        0     1416 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/command.py
+-rw-r--r--   0        0        0      787 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/context.py
+-rw-r--r--   0        0        0     4199 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/message.py
+-rw-r--r--   0        0        0     1763 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/storage.py
+-rw-r--r--   0        0        0      249 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/utils/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-16 18:29:23.896105 signalbot-0.7.0/signalbot/utils/chat_testing.py
+-rw-r--r--   0        0        0     5171 1970-01-01 00:00:00.000000 signalbot-0.7.0/PKG-INFO
```

### Comparing `signalbot-0.6.0/LICENSE` & `signalbot-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signalbot-0.6.0/README.md` & `signalbot-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,23 +63,24 @@
 - Do you see "consumers" picking up jobs and handling incoming messages?
 - Do you see the response in the bot's logs?
 
 ## Local development and package
 
 *Section work in progress. Feel free to open an issue for questions.*
 
-```
+```bash
 poetry install
 poetry run pre-commit install
 ```
 
 ## Other Projects
 
 There are a few other related projects similar to this one. You may want to check them out and see if it fits your needs.
 
-|Project|Description|Language|Status|
-|-------|-----------|--------|------|
-|https://github.com/signalapp/libsignal-service-java|Signal Library|Java|Last change 12 Nov 2019|
-|https://github.com/AsamK/signal-cli|A CLI and D-Bus interface for Signal|Java|active, build on top of https://github.com/signalapp/libsignal-service-java|
-|https://github.com/bbernhard/signal-cli-rest-api|REST API Wrapper for Signal CLI|Go|active, build on top of https://github.com/AsamK/signal-cli|
-|https://github.com/aaronetz/signal-bot|Bot Framework|Java|Last change 18 Feb 2021|
-|https://github.com/signal-bot/signal-bot|Bot Framework|Python|Last change 6 Jul 2018|
+|Project|Description|Language|
+|-------|-----------|--------|
+|https://github.com/lwesterhof/semaphore|Bot Framework|Python|
+|https://github.com/signalapp/libsignal-service-java|Signal Library|Java|
+|https://github.com/AsamK/signal-cli|A CLI and D-Bus interface for Signal|Java|
+|https://github.com/bbernhard/signal-cli-rest-api|REST API Wrapper for Signal CLI|
+|https://github.com/aaronetz/signal-bot|Bot Framework|Java|
+|https://github.com/signal-bot/signal-bot|Bot Framework|Python|
```

### Comparing `signalbot-0.6.0/pyproject.toml` & `signalbot-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   "Home Automation",
 ]
 license = "MIT"
 maintainers = ["René Filip"]
 name = "signalbot"
 readme = "README.md"
 repository = "https://github.com/filipre/signalbot"
-version = "0.6.0"
+version = "0.7.0"
 
 [tool.poetry.dependencies]
 APScheduler = "^3.9.1"
 aiohttp = "^3.8.1"
 python = "^3.9"
 redis = "^4.1.4"
 websockets = "^10.2"
```

### Comparing `signalbot-0.6.0/signalbot/api.py` & `signalbot-0.7.0/signalbot/api.py`

 * *Files identical despite different names*

### Comparing `signalbot-0.6.0/signalbot/bot.py` & `signalbot-0.7.0/signalbot/bot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import time
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 import logging
+import traceback
 
 
 from .api import SignalAPI, ReceiveMessagesError
 from .command import Command
 from .message import Message, UnknownMessageFormatError, MessageType
 from .storage import RedisStorage, InMemoryStorage
 from .context import Context
@@ -112,15 +113,19 @@
             return
 
         self.group_chats[internal_id] = group_id
 
     def _is_phone_number(self, phone_number: str) -> bool:
         if phone_number is None:
             return False
-        return phone_number[0] == "+"
+        if phone_number[0] != "+":
+            return False
+        if len(phone_number[1:]) > 15:
+            return False
+        return True
 
     def _is_group_id(self, group_id: str) -> bool:
         if group_id is None:
             return False
         prefix = "group."
         if group_id[: len(prefix)] != prefix:
             return False
@@ -212,25 +217,53 @@
             return group_id
 
         raise SignalBotError(
             f"receiver {receiver} is not a phone number and not in self.group_chats. "
             "This should never happen."
         )
 
+    # see https://stackoverflow.com/questions/55184226/catching-exceptions-in-individual-tasks-and-restarting-them
+    @classmethod
+    async def _rerun_on_exception(cls, coro, *args, **kwargs):
+        """Restart coroutine by waiting an exponential time deplay"""
+        max_sleep = 5 * 60  # sleep for at most 5 mins until rerun
+        reset = 3 * 60  # reset after 3 minutes running successfully
+        init_sleep = 1  # always start with sleeping for 1 second
+
+        next_sleep = init_sleep
+        while True:
+            start_t = int(time.monotonic())  # seconds
+
+            try:
+                await coro(*args, **kwargs)
+            except asyncio.CancelledError:
+                raise
+            except Exception:
+                traceback.print_exc()
+
+            end_t = int(time.monotonic())  # seconds
+
+            if end_t - start_t < reset:
+                sleep_t = next_sleep
+                next_sleep = min(max_sleep, next_sleep * 2)  # double sleep time
+            else:
+                next_sleep = init_sleep  # reset sleep time
+                sleep_t = next_sleep
+
+            logging.warning(f"Restarting coroutine in {sleep_t} seconds")
+            await asyncio.sleep(sleep_t)
+
     async def _produce_consume_messages(self, producers=1, consumers=3) -> None:
-        producers = [
-            asyncio.create_task(self._produce(n)) for n in range(1, producers + 1)
-        ]
-        consumers = [
-            asyncio.create_task(self._consume(n)) for n in range(1, consumers + 1)
-        ]
-        await asyncio.gather(*producers)
-        await self._q.join()
-        for c in consumers:
-            c.cancel()
+        for n in range(1, producers + 1):
+            produce_task = self._rerun_on_exception(self._produce, n)
+            asyncio.create_task(produce_task)
+
+        for n in range(1, consumers + 1):
+            consume_task = self._rerun_on_exception(self._consume, n)
+            asyncio.create_task(consume_task)
 
     async def _produce(self, name: int) -> None:
         logging.info(f"[Bot] Producer #{name} started")
         try:
             async for raw_message in self._signal.receive():
                 logging.info(f"[Raw Message] {raw_message}")
```

### Comparing `signalbot-0.6.0/signalbot/command.py` & `signalbot-0.7.0/signalbot/command.py`

 * *Files identical despite different names*

### Comparing `signalbot-0.6.0/signalbot/context.py` & `signalbot-0.7.0/signalbot/context.py`

 * *Files identical despite different names*

### Comparing `signalbot-0.6.0/signalbot/message.py` & `signalbot-0.7.0/signalbot/message.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,27 +13,36 @@
         source: str,
         timestamp: int,
         type: MessageType,
         text: str,
         base64_attachments: list = None,
         group: str = None,
         reaction: str = None,
+        mentions: list = None,
         raw_message: str = None,
     ):
         # required
         self.source = source
         self.timestamp = timestamp
         self.type = type
         self.text = text
+
         # optional
-        if base64_attachments is None:
+        self.base64_attachments = base64_attachments
+        if self.base64_attachments is None:
             self.base64_attachments = []
+
         self.group = group
+
         self.reaction = reaction
 
+        self.mentions = mentions
+        if self.mentions is None:
+            self.mentions = []
+
         self.raw_message = raw_message
 
     def recipient(self) -> str:
         # Case 1: Group chat
         if self.group:
             return self.group
 
@@ -60,29 +69,43 @@
             text = cls._parse_sync_message(raw_message["envelope"]["syncMessage"])
             group = cls._parse_group_information(
                 raw_message["envelope"]["syncMessage"]["sentMessage"]
             )
             reaction = cls._parse_reaction(
                 raw_message["envelope"]["syncMessage"]["sentMessage"]
             )
+            mentions = cls._parse_mentions(
+                raw_message["envelope"]["syncMessage"]["sentMessage"]
+            )
 
         # Option 2: dataMessage
         elif "dataMessage" in raw_message["envelope"]:
             type = MessageType.DATA_MESSAGE
             text = cls._parse_data_message(raw_message["envelope"]["dataMessage"])
             group = cls._parse_group_information(raw_message["envelope"]["dataMessage"])
             reaction = cls._parse_reaction(raw_message["envelope"]["dataMessage"])
+            mentions = cls._parse_mentions(raw_message["envelope"]["dataMessage"])
 
         else:
             raise UnknownMessageFormatError
 
         # TODO: base64_attachments
         base64_attachments = []
 
-        return cls(source, timestamp, type, text, base64_attachments, group, reaction)
+        return cls(
+            source,
+            timestamp,
+            type,
+            text,
+            base64_attachments,
+            group,
+            reaction,
+            mentions,
+            raw_message,
+        )
 
     @classmethod
     def _parse_sync_message(cls, sync_message: dict) -> str:
         try:
             text = sync_message["sentMessage"]["message"]
             return text
         except Exception:
@@ -101,14 +124,22 @@
         try:
             group = message["groupInfo"]["groupId"]
             return group
         except Exception:
             return None
 
     @classmethod
+    def _parse_mentions(cls, data_message: dict) -> list:
+        try:
+            mentions = data_message["mentions"]
+            return mentions
+        except Exception:
+            return []
+
+    @classmethod
     def _parse_reaction(self, message: dict) -> str:
         try:
             reaction = message["reaction"]["emoji"]
             return reaction
         except Exception:
             return None
```

### Comparing `signalbot-0.6.0/signalbot/storage.py` & `signalbot-0.7.0/signalbot/storage.py`

 * *Files identical despite different names*

### Comparing `signalbot-0.6.0/signalbot/utils/chat_testing.py` & `signalbot-0.7.0/signalbot/utils/chat_testing.py`

 * *Files identical despite different names*

### Comparing `signalbot-0.6.0/setup.py` & `signalbot-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,110 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: signalbot
+Version: 0.7.0
+Summary: Framework to create your own Signal bots
+Home-page: https://github.com/filipre/signalbot
+License: MIT
+Keywords: Signal,Bot,Framework,Home Automation
+Author: René Filip
+Maintainer: René Filip
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: APScheduler (>=3.9.1,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: redis (>=4.1.4,<5.0.0)
+Requires-Dist: websockets (>=10.2,<11.0)
+Project-URL: Repository, https://github.com/filipre/signalbot
+Description-Content-Type: text/markdown
+
+# Signal Bot Framework
+
+Python package to build your own Signal bots. To run the the bot you need to start the [signal-cli-rest-api](https://github.com/bbernhard/signal-cli-rest-api) service and link your device with it. Please refer to that project for more details. The API server must run in `json-rpc` mode.
+
+## Getting Started
+
+Please see https://github.com/filipre/signalbot-example for an example how to use the package and how to build a simple bot.
+
+## Classes and API
+
+*Documentation work in progress. Feel free to open an issue for questions.*
+
+The package provides methods to easily listen for incoming messages and responding or reacting on them. It also provides a class to develop new commands which then can be registered within the bot.
+
+### Signalbot
+
+- `bot.listen(group_id, internal_id)`: Listen for messages in a group chat. `group_id` must be prefixed with `group.`
+- `bot.listen(phone_number)`: Listen for messages in a user chat.
+- `bot.register(command)`: Register a new command
+- `bot.start()`: Start the bot
+- `bot.send(receiver, text, listen=False)`: Send a new message
+- `bot.react(message, emoji)`: React to a message
+- `bot.start_typing(receiver)`: Start typing
+- `bot.stop_typing(receiver)`: Stop typing
+- `bot.scheduler`: APScheduler > AsyncIOScheduler, see [here](https://apscheduler.readthedocs.io/en/3.x/modules/schedulers/asyncio.html?highlight=AsyncIOScheduler#apscheduler.schedulers.asyncio.AsyncIOScheduler)
+- `bot.storage`: In-memory or Redis stroage, see `storage.py`
+
+### Command
+
+To implement your own commands, you need to inherent `Command` and overwrite following methods:
+
+- `setup(self)`: Start any task that requires to send messages already, optional
+- `describe(self)`: String to describe your command, optional
+- `handle(self, c: Context)`: Handle an incoming message. By default, any command will read any incoming message. `Context` can be used to easily reply (`c.send(text)`), react (`c.react(emoji)`) and to type in a group (`c.start_typing()` and `c.stop_typing()`). You can use the `@triggered` decorator to listen for specific commands or you can inspect `c.message.text`.
+
+### Unit Testing
+
+In many cases, we can mock receiving and sending messages to speed up development time. To do so, you can use `signalbot.utils.ChatTestCase` which sets up a "skeleton" bot. Then, you can send messages using the `@chat` decorator in `signalbot.utils` like this:
+```python
+class PingChatTest(ChatTestCase):
+    def setUp(self):
+        # initialize self.singal_bot
+        super().setUp()
+        # all that is left to do is to register the commands that you want to test
+        self.signal_bot.register(PingCommand())
+
+    @chat("ping", "ping")
+    async def test_ping(self, query, replies, reactions):
+        self.assertEqual(replies.call_count, 2)
+        for recipient, message in replies.results():
+            self.assertEqual(recipient, ChatTestCase.group_secret)
+            self.assertEqual(message, "pong")
+```
+In `signalbot.utils`, check out `ReceiveMessagesMock`, `SendMessagesMock` and `ReactMessageMock` to learn more about their API.
+
+## Troubleshooting
+
+- Check that you linked your account successfully
+- Is the API server running in `json-rpc` mode?
+- Can you receive messages using `wscat` (websockets) and send messages using `curl` (http)?
+- Do you see incoming messages in the API logs?
+- Do you see the "raw" messages in the bot's logs?
+- Do you see "consumers" picking up jobs and handling incoming messages?
+- Do you see the response in the bot's logs?
+
+## Local development and package
+
+*Section work in progress. Feel free to open an issue for questions.*
+
+```bash
+poetry install
+poetry run pre-commit install
+```
+
+## Other Projects
+
+There are a few other related projects similar to this one. You may want to check them out and see if it fits your needs.
+
+|Project|Description|Language|
+|-------|-----------|--------|
+|https://github.com/lwesterhof/semaphore|Bot Framework|Python|
+|https://github.com/signalapp/libsignal-service-java|Signal Library|Java|
+|https://github.com/AsamK/signal-cli|A CLI and D-Bus interface for Signal|Java|
+|https://github.com/bbernhard/signal-cli-rest-api|REST API Wrapper for Signal CLI|
+|https://github.com/aaronetz/signal-bot|Bot Framework|Java|
+|https://github.com/signal-bot/signal-bot|Bot Framework|Python|
 
-packages = \
-['signalbot', 'signalbot.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['APScheduler>=3.9.1,<4.0.0',
- 'aiohttp>=3.8.1,<4.0.0',
- 'redis>=4.1.4,<5.0.0',
- 'websockets>=10.2,<11.0']
-
-setup_kwargs = {
-    'name': 'signalbot',
-    'version': '0.6.0',
-    'description': 'Framework to create your own Signal bots',
-    'long_description': '# Signal Bot Framework\n\nPython package to build your own Signal bots. To run the the bot you need to start the [signal-cli-rest-api](https://github.com/bbernhard/signal-cli-rest-api) service and link your device with it. Please refer to that project for more details. The API server must run in `json-rpc` mode.\n\n## Getting Started\n\nPlease see https://github.com/filipre/signalbot-example for an example how to use the package and how to build a simple bot.\n\n## Classes and API\n\n*Documentation work in progress. Feel free to open an issue for questions.*\n\nThe package provides methods to easily listen for incoming messages and responding or reacting on them. It also provides a class to develop new commands which then can be registered within the bot.\n\n### Signalbot\n\n- `bot.listen(group_id, internal_id)`: Listen for messages in a group chat. `group_id` must be prefixed with `group.`\n- `bot.listen(phone_number)`: Listen for messages in a user chat.\n- `bot.register(command)`: Register a new command\n- `bot.start()`: Start the bot\n- `bot.send(receiver, text, listen=False)`: Send a new message\n- `bot.react(message, emoji)`: React to a message\n- `bot.start_typing(receiver)`: Start typing\n- `bot.stop_typing(receiver)`: Stop typing\n- `bot.scheduler`: APScheduler > AsyncIOScheduler, see [here](https://apscheduler.readthedocs.io/en/3.x/modules/schedulers/asyncio.html?highlight=AsyncIOScheduler#apscheduler.schedulers.asyncio.AsyncIOScheduler)\n- `bot.storage`: In-memory or Redis stroage, see `storage.py`\n\n### Command\n\nTo implement your own commands, you need to inherent `Command` and overwrite following methods:\n\n- `setup(self)`: Start any task that requires to send messages already, optional\n- `describe(self)`: String to describe your command, optional\n- `handle(self, c: Context)`: Handle an incoming message. By default, any command will read any incoming message. `Context` can be used to easily reply (`c.send(text)`), react (`c.react(emoji)`) and to type in a group (`c.start_typing()` and `c.stop_typing()`). You can use the `@triggered` decorator to listen for specific commands or you can inspect `c.message.text`.\n\n### Unit Testing\n\nIn many cases, we can mock receiving and sending messages to speed up development time. To do so, you can use `signalbot.utils.ChatTestCase` which sets up a "skeleton" bot. Then, you can send messages using the `@chat` decorator in `signalbot.utils` like this:\n```python\nclass PingChatTest(ChatTestCase):\n    def setUp(self):\n        # initialize self.singal_bot\n        super().setUp()\n        # all that is left to do is to register the commands that you want to test\n        self.signal_bot.register(PingCommand())\n\n    @chat("ping", "ping")\n    async def test_ping(self, query, replies, reactions):\n        self.assertEqual(replies.call_count, 2)\n        for recipient, message in replies.results():\n            self.assertEqual(recipient, ChatTestCase.group_secret)\n            self.assertEqual(message, "pong")\n```\nIn `signalbot.utils`, check out `ReceiveMessagesMock`, `SendMessagesMock` and `ReactMessageMock` to learn more about their API.\n\n## Troubleshooting\n\n- Check that you linked your account successfully\n- Is the API server running in `json-rpc` mode?\n- Can you receive messages using `wscat` (websockets) and send messages using `curl` (http)?\n- Do you see incoming messages in the API logs?\n- Do you see the "raw" messages in the bot\'s logs?\n- Do you see "consumers" picking up jobs and handling incoming messages?\n- Do you see the response in the bot\'s logs?\n\n## Local development and package\n\n*Section work in progress. Feel free to open an issue for questions.*\n\n```\npoetry install\npoetry run pre-commit install\n```\n\n## Other Projects\n\nThere are a few other related projects similar to this one. You may want to check them out and see if it fits your needs.\n\n|Project|Description|Language|Status|\n|-------|-----------|--------|------|\n|https://github.com/signalapp/libsignal-service-java|Signal Library|Java|Last change 12 Nov 2019|\n|https://github.com/AsamK/signal-cli|A CLI and D-Bus interface for Signal|Java|active, build on top of https://github.com/signalapp/libsignal-service-java|\n|https://github.com/bbernhard/signal-cli-rest-api|REST API Wrapper for Signal CLI|Go|active, build on top of https://github.com/AsamK/signal-cli|\n|https://github.com/aaronetz/signal-bot|Bot Framework|Java|Last change 18 Feb 2021|\n|https://github.com/signal-bot/signal-bot|Bot Framework|Python|Last change 6 Jul 2018|\n',
-    'author': 'René Filip',
-    'author_email': None,
-    'maintainer': 'René Filip',
-    'maintainer_email': None,
-    'url': 'https://github.com/filipre/signalbot',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

