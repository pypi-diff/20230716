# Comparing `tmp/pytest-discord-0.1.2.tar.gz` & `tmp/pytest-discord-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-discord-0.1.2.tar", last modified: Sun Feb  5 15:05:27 2023, max compression
+gzip compressed data, was "pytest-discord-0.1.3.tar", last modified: Sat Jul 15 15:09:59 2023, max compression
```

## Comparing `pytest-discord-0.1.2.tar` & `pytest-discord-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 15:05:27.603666 pytest-discord-0.1.2/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:09.000000 pytest-discord-0.1.2/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      185 2021-03-20 04:14:09.000000 pytest-discord-0.1.2/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     7799 2023-02-05 15:05:27.603666 pytest-discord-0.1.2/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     6351 2023-02-05 14:07:22.000000 pytest-discord-0.1.2/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1190 2023-02-05 14:01:51.000000 pytest-discord-0.1.2/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 15:05:27.593666 pytest-discord-0.1.2/pytest_discord/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-03-20 04:14:09.000000 pytest-discord-0.1.2/pytest_discord/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-02-05 14:35:29.000000 pytest-discord-0.1.2/pytest_discord/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1931 2023-02-05 13:44:23.000000 pytest-discord-0.1.2/pytest_discord/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3110 2022-03-27 05:58:15.000000 pytest-discord-0.1.2/pytest_discord/_opt_retriever.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13550 2022-03-27 05:58:37.000000 pytest-discord-0.1.2/pytest_discord/plugin.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 15:05:27.603666 pytest-discord-0.1.2/pytest_discord.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     7799 2023-02-05 15:05:27.000000 pytest-discord-0.1.2/pytest_discord.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      573 2023-02-05 15:05:27.000000 pytest-discord-0.1.2/pytest_discord.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-02-05 15:05:27.000000 pytest-discord-0.1.2/pytest_discord.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-02-05 15:05:27.000000 pytest-discord-0.1.2/pytest_discord.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-02-05 15:04:27.000000 pytest-discord-0.1.2/pytest_discord.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      142 2023-02-05 15:05:27.000000 pytest-discord-0.1.2/pytest_discord.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       15 2023-02-05 15:05:27.000000 pytest-discord-0.1.2/pytest_discord.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 15:05:27.603666 pytest-discord-0.1.2/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)      129 2023-02-05 13:50:52.000000 pytest-discord-0.1.2/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        5 2021-03-20 04:14:09.000000 pytest-discord-0.1.2/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-02-05 15:05:27.603666 pytest-discord-0.1.2/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2743 2023-02-05 14:01:28.000000 pytest-discord-0.1.2/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 15:05:27.603666 pytest-discord-0.1.2/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       30 2021-03-20 04:14:09.000000 pytest-discord-0.1.2/tests/conftest.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4423 2023-02-05 14:10:17.000000 pytest-discord-0.1.2/tests/test_plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      998 2023-02-05 15:04:10.000000 pytest-discord-0.1.2/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.555878 pytest-discord-0.1.3/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      185 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     7275 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     5827 2023-07-15 13:52:23.000000 pytest-discord-0.1.3/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)     1253 2023-07-15 14:47:36.000000 pytest-discord-0.1.3/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/pytest_discord/
+-rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/pytest_discord/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-15 15:06:21.000000 pytest-discord-0.1.3/pytest_discord/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1913 2023-05-27 13:01:00.000000 pytest-discord-0.1.3/pytest_discord/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3120 2023-07-15 14:52:47.000000 pytest-discord-0.1.3/pytest_discord/_opt_retriever.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13579 2023-07-15 14:52:47.000000 pytest-discord-0.1.3/pytest_discord/plugin.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/pytest_discord.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7275 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      573 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/entry_points.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-15 15:09:41.000000 pytest-discord-0.1.3/pytest_discord.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      142 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       15 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)      159 2023-06-04 03:12:59.000000 pytest-discord-0.1.3/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        5 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-15 15:09:59.555878 pytest-discord-0.1.3/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2755 2023-02-25 22:32:35.000000 pytest-discord-0.1.3/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       30 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/tests/conftest.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4423 2023-02-05 14:10:17.000000 pytest-discord-0.1.3/tests/test_plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      922 2023-06-25 13:04:56.000000 pytest-discord-0.1.3/tox.ini
```

### Comparing `pytest-discord-0.1.2/LICENSE` & `pytest-discord-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.2/PKG-INFO` & `pytest-discord-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-discord
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin to notify test results to a Discord channel.
 Home-page: https://github.com/thombashi/pytest-discord
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-discord
 Project-URL: Tracker, https://github.com/thombashi/pytest-discord/issues
@@ -122,70 +122,52 @@
 
 Command options
 --------------------------------------------
 ::
 
     notify test results to a discord channel:
       --discord-webhook=WEBHOOK_URL
-                            discord webhook url of a discord channel to notify
-                            pytest results. you can also specify the value with
-                            PYTEST_DISCORD_WEBHOOK environment variable.
+                            discord webhook url of a discord channel to notify pytest results. you can also specify the value with PYTEST_DISCORD_WEBHOOK environment variable.
       --discord-verbose=VERBOSITY_LEVEL
-                            verbosity level for pytest-discord.
-                            if not set, the verbosity level will be the same as with
-                            pytest.
-                            defaults to 0.
-                            you can also specify the value with
-                            PYTEST_DISCORD_VERBOSE environment variable.
+                            Verbosity level for pytest-discord.
+                            If not set, use the verbosity level of pytest.
+                            Defaults to 0.
+                            you can also specify the value with PYTEST_DISCORD_VERBOSE environment variable.
       --discord-username=DISCORD_USERNAME
-                            name for a message. defaults to pytest. you can also
-                            specify the value with PYTEST_DISCORD_USERNAME
-                            environment variable.
+                            name for a message. defaults to pytest. you can also specify the value with PYTEST_DISCORD_USERNAME environment variable.
       --discord-success-icon=ICON_URL
-                            url to an icon of a successful run. you can also specify
-                            the value with PYTEST_DISCORD_SUCCESS_ICON environment
-                            variable.
+                            url to an icon of a successful run. you can also specify the value with PYTEST_DISCORD_SUCCESS_ICON environment variable.
       --discord-skip-icon=ICON_URL
-                            url to an icon of a skipped run. you can also specify
-                            the value with PYTEST_DISCORD_SKIP_ICON environment
-                            variable.
+                            url to an icon of a skipped run. you can also specify the value with PYTEST_DISCORD_SKIP_ICON environment variable.
       --discord-fail-icon=ICON_URL
-                            url to an icon of a failed run. you can also specify the
-                            value with PYTEST_DISCORD_FAIL_ICON environment
-                            variable.
+                            url to an icon of a failed run. you can also specify the value with PYTEST_DISCORD_FAIL_ICON environment variable.
       --discord-attach-file
-                            post pytest results as a markdown file to a discord
-                            channel. you can also specify the value with
-                            PYTEST_DISCORD_ATTACH_FILE environment variable.
+                            post pytest results as a markdown file to a discord channel. you can also specify the value with PYTEST_DISCORD_ATTACH_FILE environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
   discord_webhook (string):
-                        discord webhook url of a discord channel to notify
-                        pytest results.
+                        discord webhook url of a discord channel to notify pytest results.
   discord_verbose (string):
-                        verbosity level for pytest-discord. if not set, the
-                        verbosity level will be the same as with pytest.
-                        defaults to 0.
+                        Verbosity level for pytest-discord. If not set, use the verbosity level of pytest. Defaults to 0.
   discord_username (string):
                         name for a message. defaults to pytest.
   discord_success_icon (string):
                         url to an icon of a successful run.
   discord_skip_icon (string):
                         url to an icon of a skipped run.
   discord_fail_icon (string):
                         url to an icon of a failed run.
   discord_attach_file (bool):
-                        post pytest results as a markdown file to a discord
-                        channel.
+                        post pytest results as a markdown file to a discord channel.
 
 :Example of ``pyproject.toml``:
     .. code-block:: toml
 
         [tool.pytest.ini_options]
         discord_webhook = "https://discordapp.com/api/webhooks/..."
         md_report_verbose = 1
```

### Comparing `pytest-discord-0.1.2/README.rst` & `pytest-discord-0.1.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -88,70 +88,52 @@
 
 Command options
 --------------------------------------------
 ::
 
     notify test results to a discord channel:
       --discord-webhook=WEBHOOK_URL
-                            discord webhook url of a discord channel to notify
-                            pytest results. you can also specify the value with
-                            PYTEST_DISCORD_WEBHOOK environment variable.
+                            discord webhook url of a discord channel to notify pytest results. you can also specify the value with PYTEST_DISCORD_WEBHOOK environment variable.
       --discord-verbose=VERBOSITY_LEVEL
-                            verbosity level for pytest-discord.
-                            if not set, the verbosity level will be the same as with
-                            pytest.
-                            defaults to 0.
-                            you can also specify the value with
-                            PYTEST_DISCORD_VERBOSE environment variable.
+                            Verbosity level for pytest-discord.
+                            If not set, use the verbosity level of pytest.
+                            Defaults to 0.
+                            you can also specify the value with PYTEST_DISCORD_VERBOSE environment variable.
       --discord-username=DISCORD_USERNAME
-                            name for a message. defaults to pytest. you can also
-                            specify the value with PYTEST_DISCORD_USERNAME
-                            environment variable.
+                            name for a message. defaults to pytest. you can also specify the value with PYTEST_DISCORD_USERNAME environment variable.
       --discord-success-icon=ICON_URL
-                            url to an icon of a successful run. you can also specify
-                            the value with PYTEST_DISCORD_SUCCESS_ICON environment
-                            variable.
+                            url to an icon of a successful run. you can also specify the value with PYTEST_DISCORD_SUCCESS_ICON environment variable.
       --discord-skip-icon=ICON_URL
-                            url to an icon of a skipped run. you can also specify
-                            the value with PYTEST_DISCORD_SKIP_ICON environment
-                            variable.
+                            url to an icon of a skipped run. you can also specify the value with PYTEST_DISCORD_SKIP_ICON environment variable.
       --discord-fail-icon=ICON_URL
-                            url to an icon of a failed run. you can also specify the
-                            value with PYTEST_DISCORD_FAIL_ICON environment
-                            variable.
+                            url to an icon of a failed run. you can also specify the value with PYTEST_DISCORD_FAIL_ICON environment variable.
       --discord-attach-file
-                            post pytest results as a markdown file to a discord
-                            channel. you can also specify the value with
-                            PYTEST_DISCORD_ATTACH_FILE environment variable.
+                            post pytest results as a markdown file to a discord channel. you can also specify the value with PYTEST_DISCORD_ATTACH_FILE environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
   discord_webhook (string):
-                        discord webhook url of a discord channel to notify
-                        pytest results.
+                        discord webhook url of a discord channel to notify pytest results.
   discord_verbose (string):
-                        verbosity level for pytest-discord. if not set, the
-                        verbosity level will be the same as with pytest.
-                        defaults to 0.
+                        Verbosity level for pytest-discord. If not set, use the verbosity level of pytest. Defaults to 0.
   discord_username (string):
                         name for a message. defaults to pytest.
   discord_success_icon (string):
                         url to an icon of a successful run.
   discord_skip_icon (string):
                         url to an icon of a skipped run.
   discord_fail_icon (string):
                         url to an icon of a failed run.
   discord_attach_file (bool):
-                        post pytest results as a markdown file to a discord
-                        channel.
+                        post pytest results as a markdown file to a discord channel.
 
 :Example of ``pyproject.toml``:
     .. code-block:: toml
 
         [tool.pytest.ini_options]
         discord_webhook = "https://discordapp.com/api/webhooks/..."
         md_report_verbose = 1
```

### Comparing `pytest-discord-0.1.2/pyproject.toml` & `pytest-discord-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
@@ -54,14 +55,15 @@
 
 [tool.mypy]
 ignore_missing_imports = true
 python_version = 3.7
 
 pretty = true
 
+check_untyped_defs = true
 no_implicit_optional = true
 show_error_codes = true
 show_error_context = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
```

### Comparing `pytest-discord-0.1.2/pytest_discord/_const.py` & `pytest-discord-0.1.3/pytest_discord/_const.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         "discord-webhook",
         "discord webhook url of a discord channel to notify pytest results.",
     )
     DISCORD_VERBOSE = (
         "discord-verbose",
         dedent(
             """\
-            verbosity level for pytest-discord.
-            if not set, the verbosity level will be the same as with pytest.
-            defaults to 0.
+            Verbosity level for pytest-discord.
+            If not set, use the verbosity level of pytest.
+            Defaults to 0.
             """
         ),
     )
     DISCORD_USERNAME = (
         "discord-username",
         f"name for a message. defaults to {Default.USERNAME}.",
     )
```

### Comparing `pytest-discord-0.1.2/pytest_discord/_opt_retriever.py` & `pytest-discord-0.1.3/pytest_discord/_opt_retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional
+from typing import Any, Optional
 
 from _pytest.config import Config
 from typepy import Bool, Integer, StrictLevel
 from typepy.error import TypeConversionError
 
 from ._const import Default, Option
 
@@ -90,12 +90,12 @@
 
         if not value:
             value = config.getini(discord_opt.inioption_str)
 
         return value
 
     @staticmethod
-    def _to_int(value) -> Optional[int]:
+    def _to_int(value: Any) -> Optional[int]:
         try:
             return Integer(value, strict_level=StrictLevel.MIN).convert()
         except TypeConversionError:
             return None
```

### Comparing `pytest-discord-0.1.2/pytest_discord/plugin.py` & `pytest-discord-0.1.3/pytest_discord/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 from collections import defaultdict
 from datetime import datetime
 from typing import Dict, List, Mapping, Optional, Sequence, Tuple
 
 import aiohttp
 import pytest
 from _pytest.config import Config
+from _pytest.config.argparsing import Parser
 from _pytest.terminal import TerminalReporter
 from discord import AsyncWebhookAdapter, Colour, Embed, File, Webhook
 from discord.errors import Forbidden, HTTPException, InvalidArgument, NotFound
 from pytest_md_report.plugin import extract_pytest_stats
 
 from ._const import HelpMsg, Option, TestResultType
 from ._opt_retriever import DiscordOptRetriever
 
 
 MAX_EMBED_LEN = 2048
 MAX_EMBEDS_LEN = 6000
 MAX_EMBED_CT = 10
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("discord", "notify test results to a discord channel")
 
     group.addoption(
         Option.DISCORD_WEBHOOK.cmdoption_str,
         metavar="WEBHOOK_URL",
         help=Option.DISCORD_WEBHOOK.help_msg
         + HelpMsg.EXTRA_MSG_TEMPLATE.format(Option.DISCORD_WEBHOOK.envvar_str),
@@ -299,15 +300,15 @@
 _result_type_to_colour = {
     TestResultType.SUCCESS: Colour.green(),
     TestResultType.SKIP: Colour.gold(),
     TestResultType.FAIL: Colour.red(),
 }
 
 
-def pytest_unconfigure(config):
+def pytest_unconfigure(config: Config) -> None:
     if config.option.help:
         return
 
     opt_retriever = DiscordOptRetriever(config)
     url = opt_retriever.retrieve_webhook_url()
     if not url:
         return
@@ -385,16 +386,15 @@
                 ).encode("utf8")
             ),
             datetime.fromtimestamp(reporter._sessionstarttime).strftime(
                 "pytest_%Y-%m-%dT%H:%M:%S.md"
             ),
         )
 
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(
+    asyncio.run(
         _send_message(
             reporter=reporter,
             url=url,
             header=header,
             username=opt_retriever.retrieve_username(),
             avatar_url=avatar_url,
             embeds=embeds,
```

### Comparing `pytest-discord-0.1.2/pytest_discord.egg-info/PKG-INFO` & `pytest-discord-0.1.3/pytest_discord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-discord
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin to notify test results to a Discord channel.
 Home-page: https://github.com/thombashi/pytest-discord
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-discord
 Project-URL: Tracker, https://github.com/thombashi/pytest-discord/issues
@@ -122,70 +122,52 @@
 
 Command options
 --------------------------------------------
 ::
 
     notify test results to a discord channel:
       --discord-webhook=WEBHOOK_URL
-                            discord webhook url of a discord channel to notify
-                            pytest results. you can also specify the value with
-                            PYTEST_DISCORD_WEBHOOK environment variable.
+                            discord webhook url of a discord channel to notify pytest results. you can also specify the value with PYTEST_DISCORD_WEBHOOK environment variable.
       --discord-verbose=VERBOSITY_LEVEL
-                            verbosity level for pytest-discord.
-                            if not set, the verbosity level will be the same as with
-                            pytest.
-                            defaults to 0.
-                            you can also specify the value with
-                            PYTEST_DISCORD_VERBOSE environment variable.
+                            Verbosity level for pytest-discord.
+                            If not set, use the verbosity level of pytest.
+                            Defaults to 0.
+                            you can also specify the value with PYTEST_DISCORD_VERBOSE environment variable.
       --discord-username=DISCORD_USERNAME
-                            name for a message. defaults to pytest. you can also
-                            specify the value with PYTEST_DISCORD_USERNAME
-                            environment variable.
+                            name for a message. defaults to pytest. you can also specify the value with PYTEST_DISCORD_USERNAME environment variable.
       --discord-success-icon=ICON_URL
-                            url to an icon of a successful run. you can also specify
-                            the value with PYTEST_DISCORD_SUCCESS_ICON environment
-                            variable.
+                            url to an icon of a successful run. you can also specify the value with PYTEST_DISCORD_SUCCESS_ICON environment variable.
       --discord-skip-icon=ICON_URL
-                            url to an icon of a skipped run. you can also specify
-                            the value with PYTEST_DISCORD_SKIP_ICON environment
-                            variable.
+                            url to an icon of a skipped run. you can also specify the value with PYTEST_DISCORD_SKIP_ICON environment variable.
       --discord-fail-icon=ICON_URL
-                            url to an icon of a failed run. you can also specify the
-                            value with PYTEST_DISCORD_FAIL_ICON environment
-                            variable.
+                            url to an icon of a failed run. you can also specify the value with PYTEST_DISCORD_FAIL_ICON environment variable.
       --discord-attach-file
-                            post pytest results as a markdown file to a discord
-                            channel. you can also specify the value with
-                            PYTEST_DISCORD_ATTACH_FILE environment variable.
+                            post pytest results as a markdown file to a discord channel. you can also specify the value with PYTEST_DISCORD_ATTACH_FILE environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
   discord_webhook (string):
-                        discord webhook url of a discord channel to notify
-                        pytest results.
+                        discord webhook url of a discord channel to notify pytest results.
   discord_verbose (string):
-                        verbosity level for pytest-discord. if not set, the
-                        verbosity level will be the same as with pytest.
-                        defaults to 0.
+                        Verbosity level for pytest-discord. If not set, use the verbosity level of pytest. Defaults to 0.
   discord_username (string):
                         name for a message. defaults to pytest.
   discord_success_icon (string):
                         url to an icon of a successful run.
   discord_skip_icon (string):
                         url to an icon of a skipped run.
   discord_fail_icon (string):
                         url to an icon of a failed run.
   discord_attach_file (bool):
-                        post pytest results as a markdown file to a discord
-                        channel.
+                        post pytest results as a markdown file to a discord channel.
 
 :Example of ``pyproject.toml``:
     .. code-block:: toml
 
         [tool.pytest.ini_options]
         discord_webhook = "https://discordapp.com/api/webhooks/..."
         md_report_verbose = 1
```

### Comparing `pytest-discord-0.1.2/pytest_discord.egg-info/SOURCES.txt` & `pytest-discord-0.1.3/pytest_discord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.2/setup.py` & `pytest-discord-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "pytest-discord"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
```

### Comparing `pytest-discord-0.1.2/tests/test_plugin.py` & `pytest-discord-0.1.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.2/tox.ini` & `pytest-discord-0.1.3/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [tox]
 envlist =
     py{37,38,39,310,311}
     pypy3
     build
-    clean
     cov
     fmt
     lint
 
 [testenv]
 passenv = *
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
@@ -40,24 +39,23 @@
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:fmt]
 skip_install = true
 deps =
-    autoflake>=1.4
+    autoflake>=2
     black>=23.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
     black setup.py tests pytest_discord
 
 [testenv:lint]
 skip_install = true
 deps =
-    mypy>=0.991
+    mypy>=1
     pylama>=8.4.1
 commands =
-    python setup.py check
     mypy pytest_discord setup.py
     pylama
```

