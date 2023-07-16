# Comparing `tmp/nonebot_plugin_spark_gpt-1.1.7.tar.gz` & `tmp/nonebot_plugin_spark_gpt-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_spark_gpt-1.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_spark_gpt-1.1.8.tar", max compression
```

## Comparing `nonebot_plugin_spark_gpt-1.1.7.tar` & `nonebot_plugin_spark_gpt-1.1.8.tar`

### file list

```diff
@@ -1,85 +1,87 @@
--rw-r--r--   0        0        0      219 2023-07-11 09:53:31.539890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/__init__.py
--rw-r--r--   0        0        0    17261 2023-07-11 09:53:31.540890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/adapter.py
--rw-r--r--   0        0        0      138 2023-07-11 09:53:31.541890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/__init__.py
--rw-r--r--   0        0        0       27 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/client.py
--rw-r--r--   0        0        0    51932 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/client.pyi
--rw-r--r--   0        0        0    98693 2023-07-11 09:53:31.543890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/handle.py
--rw-r--r--   0        0        0   115238 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/model.py
--rw-r--r--   0        0        0     1482 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/request.py
--rw-r--r--   0        0        0    34839 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/types.py
--rw-r--r--   0        0        0     2441 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/utils.py
--rw-r--r--   0        0        0     7255 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/bot.py
--rw-r--r--   0        0        0     2192 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/config.py
--rw-r--r--   0        0        0    28334 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/event.py
--rw-r--r--   0        0        0     2076 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/exception.py
--rw-r--r--   0        0        0    13603 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/message.py
--rw-r--r--   0        0        0     2874 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/payload.py
--rw-r--r--   0        0        0     1946 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/typing.py
--rw-r--r--   0        0        0      626 2023-07-11 09:53:31.548892 nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/utils.py
--rw-r--r--   0        0        0      809 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/__init__.py
--rw-r--r--   0        0        0     4008 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/bard.py
--rw-r--r--   0        0        0     9680 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py
--rw-r--r--   0        0        0     9032 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/claude_ai.py
--rw-r--r--   0        0        0     3976 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/load_config.py
--rw-r--r--   0        0        0     6760 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/newbing.py
--rw-r--r--   0        0        0     6131 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/poe.py
--rw-r--r--   0        0        0     7619 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/slack_claude.py
--rw-r--r--   0        0        0     8129 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/spark_desk.py
--rw-r--r--   0        0        0     7435 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/sydneybing.py
--rw-r--r--   0        0        0     6802 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py
--rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/__init__.py
--rw-r--r--   0        0        0    17078 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py
--rw-r--r--   0        0        0    11565 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py
--rw-r--r--   0        0        0     2057 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py
--rw-r--r--   0        0        0     4460 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py
--rw-r--r--   0        0        0     1256 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py
--rw-r--r--   0        0        0     7856 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py
--rw-r--r--   0        0        0    14237 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py
--rw-r--r--   0        0        0       46 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/exceptions.py
--rw-r--r--   0        0        0      267 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/ImageGen.py
--rw-r--r--   0        0        0     2247 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py
--rw-r--r--   0        0        0     7512 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py
--rw-r--r--   0        0        0     5792 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py
--rw-r--r--   0        0        0      955 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py
--rw-r--r--   0        0        0       83 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/__init__.py
--rw-r--r--   0        0        0     1454 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py
--rw-r--r--   0        0        0      127 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/main.py
--rw-r--r--   0        0        0     5878 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py
--rw-r--r--   0        0        0      719 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py
--rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/__init__.py
--rw-r--r--   0        0        0     5559 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/config.py
--rw-r--r--   0        0        0     1694 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/load_config.py
--rw-r--r--   0        0        0     4951 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/mytypes.py
--rw-r--r--   0        0        0     4583 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/prefix_data.py
--rw-r--r--   0        0        0    30736 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/prompt_data.py
--rw-r--r--   0        0        0     9955 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/user_data.py
--rw-r--r--   0        0        0    14446 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/app.py
--rw-r--r--   0        0        0      547 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json
--rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/__init__.py
--rw-r--r--   0        0        0     4722 2023-07-15 11:48:23.369184 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/config.html
--rw-r--r--   0        0        0     2246 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/index.html
--rw-r--r--   0        0        0    10215 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/prefix.html
--rw-r--r--   0        0        0    10211 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/prompt.html
--rw-r--r--   0        0        0       23 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/__init__.py
--rw-r--r--   0        0        0       51 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/__init__.py
--rw-r--r--   0        0        0    17618 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py
--rw-r--r--   0        0        0    22733 2023-07-15 11:24:03.425067 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py
--rw-r--r--   0        0        0     2275 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py
--rw-r--r--   0        0        0    15735 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py
--rw-r--r--   0        0        0     6458 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/temp_bots.py
--rw-r--r--   0        0        0     2421 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/render.py
--rw-r--r--   0        0        0  1458204 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0    20838 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/markdown.css
--rw-r--r--   0        0        0     1834 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/markdown.html
--rw-r--r--   0        0        0     4366 2023-07-15 11:25:27.711221 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/menu.html
--rw-r--r--   0        0        0 10968356 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/PingFang.ttf
--rw-r--r--   0        0        0     4963 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css
--rw-r--r--   0        0        0     3138 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/template.html
--rw-r--r--   0        0        0      125 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/text.css
--rw-r--r--   0        0        0      233 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/text.html
--rw-r--r--   0        0        0     1113 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/utils.py
--rw-r--r--   0        0        0      968 2023-07-15 10:58:27.197493 nonebot_plugin_spark_gpt-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     8772 2023-07-15 12:25:20.190400 nonebot_plugin_spark_gpt-1.1.7/README.md
--rw-r--r--   0        0        0     9923 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0      219 2023-07-11 09:53:31.539890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/__init__.py
+-rw-r--r--   0        0        0    17261 2023-07-11 09:53:31.540890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/adapter.py
+-rw-r--r--   0        0        0      138 2023-07-11 09:53:31.541890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/client.py
+-rw-r--r--   0        0        0    51932 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/client.pyi
+-rw-r--r--   0        0        0    98693 2023-07-11 09:53:31.543890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/handle.py
+-rw-r--r--   0        0        0   115238 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/model.py
+-rw-r--r--   0        0        0     1482 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/request.py
+-rw-r--r--   0        0        0    34839 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/types.py
+-rw-r--r--   0        0        0     2441 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/utils.py
+-rw-r--r--   0        0        0     7255 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/bot.py
+-rw-r--r--   0        0        0     2192 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/config.py
+-rw-r--r--   0        0        0    28334 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/event.py
+-rw-r--r--   0        0        0     2076 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/exception.py
+-rw-r--r--   0        0        0    13603 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/message.py
+-rw-r--r--   0        0        0     2874 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/payload.py
+-rw-r--r--   0        0        0     1946 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/typing.py
+-rw-r--r--   0        0        0      626 2023-07-11 09:53:31.548892 nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/utils.py
+-rw-r--r--   0        0        0      809 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/__init__.py
+-rw-r--r--   0        0        0     4008 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/bard.py
+-rw-r--r--   0        0        0     9680 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py
+-rw-r--r--   0        0        0     9032 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/claude_ai.py
+-rw-r--r--   0        0        0     3976 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/load_config.py
+-rw-r--r--   0        0        0     6760 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/newbing.py
+-rw-r--r--   0        0        0     6131 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/poe.py
+-rw-r--r--   0        0        0     7619 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/slack_claude.py
+-rw-r--r--   0        0        0     8129 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/spark_desk.py
+-rw-r--r--   0        0        0     7435 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/sydneybing.py
+-rw-r--r--   0        0        0     6802 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py
+-rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/__init__.py
+-rw-r--r--   0        0        0    17078 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py
+-rw-r--r--   0        0        0    11565 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py
+-rw-r--r--   0        0        0     2057 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py
+-rw-r--r--   0        0        0     4460 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py
+-rw-r--r--   0        0        0     1256 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py
+-rw-r--r--   0        0        0     7856 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py
+-rw-r--r--   0        0        0    14237 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py
+-rw-r--r--   0        0        0       46 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/exceptions.py
+-rw-r--r--   0        0        0      267 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/ImageGen.py
+-rw-r--r--   0        0        0     2247 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py
+-rw-r--r--   0        0        0     7512 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py
+-rw-r--r--   0        0        0     5792 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py
+-rw-r--r--   0        0        0      955 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py
+-rw-r--r--   0        0        0       83 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/__init__.py
+-rw-r--r--   0        0        0     1454 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py
+-rw-r--r--   0        0        0      127 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/main.py
+-rw-r--r--   0        0        0     5878 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py
+-rw-r--r--   0        0        0      719 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py
+-rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/__init__.py
+-rw-r--r--   0        0        0     5559 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/config.py
+-rw-r--r--   0        0        0     1694 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/load_config.py
+-rw-r--r--   0        0        0     4951 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/mytypes.py
+-rw-r--r--   0        0        0     4583 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/prefix_data.py
+-rw-r--r--   0        0        0    30736 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/prompt_data.py
+-rw-r--r--   0        0        0     9955 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/user_data.py
+-rw-r--r--   0        0        0    14446 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/app.py
+-rw-r--r--   0        0        0      547 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json
+-rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/__init__.py
+-rw-r--r--   0        0        0     4585 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/config.html
+-rw-r--r--   0        0        0     2246 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/index.html
+-rw-r--r--   0        0        0    10215 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/prefix.html
+-rw-r--r--   0        0        0    10211 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/prompt.html
+-rw-r--r--   0        0        0       23 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/__init__.py
+-rw-r--r--   0        0        0       51 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/__init__.py
+-rw-r--r--   0        0        0    17720 2023-07-16 11:09:47.173879 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py
+-rw-r--r--   0        0        0    24891 2023-07-16 09:59:39.618598 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py
+-rw-r--r--   0        0        0     2275 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py
+-rw-r--r--   0        0        0    15735 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py
+-rw-r--r--   0        0        0     6458 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/temp_bots.py
+-rw-r--r--   0        0        0     5070 2023-07-16 10:00:31.992160 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/render.py
+-rw-r--r--   0        0        0  1458204 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0     4336 2023-07-16 07:02:47.151477 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/list.html
+-rw-r--r--   0        0        0    19983 2023-07-16 07:22:32.039006 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/markdown.css
+-rw-r--r--   0        0        0     1320 2023-07-16 10:00:31.995390 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/markdown.html
+-rw-r--r--   0        0        0     3589 2023-07-16 06:01:06.406590 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/menu.html
+-rw-r--r--   0        0        0     4205 2023-07-16 09:08:53.905095 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/menus.html
+-rw-r--r--   0        0        0 10968356 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/PingFang.ttf
+-rw-r--r--   0        0        0     4963 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css
+-rw-r--r--   0        0        0     3138 2023-07-16 10:00:31.997900 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/template.html
+-rw-r--r--   0        0        0      125 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/text.css
+-rw-r--r--   0        0        0      233 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/text.html
+-rw-r--r--   0        0        0     1113 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/utils.py
+-rw-r--r--   0        0        0      968 2023-07-16 06:01:48.330631 nonebot_plugin_spark_gpt-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     8456 2023-07-16 06:01:48.333638 nonebot_plugin_spark_gpt-1.1.8/README.md
+-rw-r--r--   0        0        0     9608 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-1.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/adapter.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/client.pyi` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/handle.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/model.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/request.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/types.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/api/utils.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/bot.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/config.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/event.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/exception.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/message.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/payload.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/payload.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/typing.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot/adapters/discord/utils.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot/adapters/discord/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/__init__.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/bard.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/bard.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/claude_ai.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/claude_ai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/load_config.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/newbing.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/poe.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/poe.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/slack_claude.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/slack_claude.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/spark_desk.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/spark_desk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/sydneybing.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/sydneybing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/config.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/load_config.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/mytypes.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/mytypes.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/prefix_data.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/prefix_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/prompt_data.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/prompt_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/user_data.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/user_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/app.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/app.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/config.html` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/config.html`

 * *Files 6% similar despite different names*

```diff
@@ -117,29 +117,21 @@
 
 <!-- 引入所需的JavaScript库 -->
 <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"></script>
 <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>
 
 <!-- 使用JavaScript动态设置sidebar的高度 -->
-<script>
-(function() {
-  var sidebar = document.querySelector('.sidebar');
-  var sidebarHeight = sidebar.offsetHeight;
-
-  var main = document.querySelector('.main'); 
-  var mainHeight = main.offsetHeight;
-
-  var maxHeight = Math.max(sidebarHeight, mainHeight);
-
-  sidebar.style.height = maxHeight + 'px';
-  main.style.height = maxHeight + 'px';
-
-})();  
-</script>
+<script> (function () {
+    var sidebar = document.querySelector('.sidebar');
+    var sidebarHeight = sidebar.offsetHeight;
+
+    var main = document.querySelector('.main');
+    main.style.height = sidebarHeight + 'px';
+})(); </script>
 
 {% if saved %}
     <script> $(document).ready(function () {
         alert('保存成功！');
     }); </script> {% endif %}
 
 </body>
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/index.html` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/prefix.html` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/prefix.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/common/web/templates/prompt.html` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/common/web/templates/prompt.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 from ..temp_bots import temp_bots
 from ...chatbot.load_config import get_able_source
 from ...common.mytypes import BotInfo, BotData
 from ...common.prefix_data import prefixes
 from ...common.prompt_data import prompts
 from ...common.user_data import common_users
-from ...utils.render import menu_to_pic
+from ...utils.render import list_to_pic
 from ...utils.utils import is_valid_string
 
 REFRESH_KEYWORDS = [
     "清除对话",
     "清空对话",
     "清除历史",
     "清空历史",
@@ -120,15 +120,15 @@
             msg,
             matcher,
             bot,
             event,
         )
     )
     if not Generated_Source_Pic:
-        pic_bytes = await menu_to_pic(menu=source_des_dict, width=700, headline="来源列表", description="",
+        pic_bytes = await list_to_pic(source_des_dict, width=700, headline="来源列表", description="",
                                       font_size=20)
         get_source_pic()
         with open(Source_Msg_Path, "wb") as f:
             f.write(pic_bytes)
     else:
         with open(Source_Msg_Path, "rb") as f:
             pic_bytes = f.read()
@@ -196,23 +196,23 @@
 
     if not (
             state["able_source_dict"][state["source_index"]] == "bing"
             or state["able_source_dict"][state["source_index"]] == "bard"
             or state["able_source_dict"][state["source_index"]] == "通义千问"
     ):
         prompts_dict = prompts.show_list()
-        msg = '请设置这个bot的预设\n预设是每次对话开始时向bot首先静默发送过去的内容\n如果不使用预设,请输入"无"或"无预设"\n如果使用本地预设,请输入预设前的数字索引,如使用自己的预设直接发送即可\n输入"算了"或"取消"可以结束当前操作'
+        msg = '请设置这个bot的预设\n预设是每次连续对话开始时发送初始化过去的内容,清除bot的对话历史后也会重新初始化\n\n如果不使用预设,请输入"无"或"无预设"\n如果使用本地预设,请输入预设前的数字索引\n如使用自己的预设直接发送即可\n\n输入"算了"或"取消"可以结束当前操作\n本地预设列表图片将在下面发送:'
         state["replys"].append(
             await send_message(
                 msg, matcher, bot, event,
             )
         )
 
         if not prompts.Generated:
-            pic_bytes = await menu_to_pic(menu=prompts_dict, headline="预设列表", width=800,
+            pic_bytes = await list_to_pic(prompts_dict, headline="预设列表", width=800,
                                           description="下面只展示了前200个字符")
             prompts.generate_pic()
             with open(Prompt_Msg_Path, "wb") as f:
                 f.write(pic_bytes)
         else:
             with open(Prompt_Msg_Path, "rb") as f:
                 pic_bytes = f.read()
@@ -259,23 +259,23 @@
     state["prompt_nickname"] = prompt_nickname
     state["prompt"] = prompt
 
     try:
         state["prefix_nickname"]
     except Exception:
         prefixes_dict = prefixes.show_list()
-        msg = f'请设置这个bot的前缀\n前缀是指每次对话时都在你的问题前添加一些要求内容,来使boy的回答符合要求\n如果不使用前缀,请输入"无"或"无前缀"\n如果使用本地前缀,请发送前缀前的数字索引,如使用自己的前缀直接发送即可\n输入"算了"或"取消"可以结束当前操作'
+        msg = f'请设置这个bot的前缀\n前缀是指每次对话时都在你的问题前自动添加的一些内容\n\n如果不使用前缀,请输入"无"或"无前缀"\n如果使用本地前缀,请发送前缀前的数字索引,如使用自己的前缀直接发送即可\n\n输入"算了"或"取消"可以结束当前操作\n本地前缀列表图片将在下面发送:'
 
         state["replys"].append(
             await send_message(
                 msg, matcher, bot, event
             )
         )
         if not prefixes.Generated:
-            pic_bytes = await menu_to_pic(menu=prefixes_dict, headline="前缀列表", width=800,
+            pic_bytes = await list_to_pic(prefixes_dict, headline="前缀列表", width=800,
                                           description="下面只展示了前200个字符")
             prefixes.generate_pic()
             with open(Prefix_Msg_Path, "wb") as f:
                 f.write(pic_bytes)
         else:
             with open(Prefix_Msg_Path, "rb") as f:
                 pic_bytes = f.read()
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Bot,
 )
 from ...common.mytypes import CommonUserInfo
 from ...common.prefix_data import prefixes
 from ...common.prompt_data import prompts
 from ...common.user_data import common_users
 from ...common.web.app import start_web_ui, stop_web_ui, HOST, PORT
-from ...utils.render import menu_to_pic
+from ...utils.render import list_to_pic, menu_to_pic
 
 Help_Msg_Path = Path(__file__).parent / "HelpMsg.jpeg"
 Help_Msg_Path.touch()
 Super_Msg_Path = Path(__file__).parent / "SuperMsg.jpeg"
 Super_Msg_Path.touch()
 
 help = on_command("shelp", aliases={"s帮助", "sparkhelp"}, priority=1, block=False)
@@ -48,68 +48,83 @@
         Generated_Super_Msg_Pic,
         get_super_pic,
         Generated_Help_Msg_Pic,
         get_help_pic
     )
     command_start = str(foo)
     if is_super_user(event, bot):
-        help_dict = {
-            f"{PRIVATE_COMMAND}bot名称+询问的问题": "与指定属于自己的bot对话\n(可使用'回复'来连续对话)",
-            f"{PUBLIC_COMMAND}bot名称+询问的问题": "与指定属于公共的bot对话\n(可使用'回复'来连续对话)",
-            f"{PRIVATE_COMMAND}所有bot": "查询所有的可用的属于自己的bot",
-            f"{PUBLIC_COMMAND}所有bot": "查询所有的可用的公共的bot",
-            f"{PUBLIC_COMMAND}创建bot": "创建新的公用的bot",
-            f"{PUBLIC_COMMAND}改名bot": "更改公用的bot的名称",
-            f"{PUBLIC_COMMAND}删除bot": "删除指定公用的bot",
-            f"{PRIVATE_COMMAND}创建bot": "创建新的属于自己的bot",
-            f"{PRIVATE_COMMAND}改名bot": "更改自己的bot的名称",
-            f"{PRIVATE_COMMAND}删除bot": "删除指定自己的bot",
-            f"{command_start}所有预设": "给出所有预设的名称",
-            f"{command_start}查询预设": "查询指定预设的内容",
-            f"{command_start}添加预设": "添加新的预设(可覆盖同名预设)",
-            f"{command_start}改名预设": "修改预设的名字(可覆盖同名预设)",
-            f"{command_start}删除预设": "删除指定预设",
-            f"{command_start}所有前缀": "给出所有前缀的名称",
-            f"{command_start}查询前缀": "查询指定前缀的内容",
-            f"{command_start}添加前缀": "添加新的前缀(可覆盖同名前缀)",
-            f"{command_start}改名前缀": "修改前缀的名字(可覆盖同名前缀)",
-            f"{command_start}删除前缀": "删除指定前缀",
-            f"{command_start}用户信息": "查询当前用户的通用用户的用户名和密钥.建议私聊使用",
-            f"{command_start}更改绑定": "将当前平台账户绑定到指定通用账户,实现跨平台数据互通",
-            f"{command_start}开启webui": "默认开启,打开webui,并返回webui开启的端口(管理员可用)",
-            f"{command_start}关闭webui": "请在使用webui后关闭(管理员可用)",
-        }
         if not Generated_Super_Msg_Pic:
-            pic_bytes = await menu_to_pic(help_dict, 800, font_size=30)
+            help_dict = {
+                "私有bot": {"des": "使用和管理自己独有的bot的命令,私有bot只有主人可使用,其他人无法使用", "funcs": {
+                    f"{PRIVATE_COMMAND}bot名称+询问的问题": "与指定属于自己的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)",
+                    f"{PRIVATE_COMMAND}所有bot": "查询所有的可用的私有的bot,以获取bot名称和相关信息",
+                    f"{PRIVATE_COMMAND}创建bot": "创建新的私有的bot",
+                    f"{PRIVATE_COMMAND}改名bot": "更改自己的bot的名称",
+                    f"{PRIVATE_COMMAND}删除bot": "删除指定自己的bot",
+                }},
+                "公有bot": {"des": "使用和管理公有的bot的命令", "funcs": {
+                    f"{PUBLIC_COMMAND}bot名称+询问的问题": "与指定属于公共的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)",
+                    f"{PUBLIC_COMMAND}所有bot": "查询所有的可用的公共的bot,以获取bot名称和相关信息",
+                    f"{PUBLIC_COMMAND}创建bot": "创建新的公用的bot",
+                    f"{PUBLIC_COMMAND}改名bot": "更改公用的bot的名称",
+                    f"{PUBLIC_COMMAND}删除bot": "删除指定公用的bot",
+                }}, "预设": {"des": "查看和管理预设", "funcs": {
+                    f"{command_start}所有预设": "列出所有预设的名称和缩略的内容",
+                    f"{command_start}查询预设": "查询指定预设的具体详尽内容",
+                    f"{command_start}添加预设": "添加新的预设",
+                    f"{command_start}删除预设": "删除指定预设",
+                    f"{command_start}改名预设": "修改指定预设的名字",
+                }}, "前缀": {"des": "查看和管理前缀", "funcs": {
+                    f"{command_start}所有前缀": "列出所有前缀的的名称和缩略的内容",
+                    f"{command_start}查询前缀": "查询指定前缀的具体详尽内容",
+                    f"{command_start}添加前缀": "添加新的前缀",
+                    f"{command_start}删除前缀": "删除指定前缀",
+                    f"{command_start}改名前缀": "修改指定前缀的名字",
+                }}, "账户信息": {"des": "用来实现跨平台(qq,tg等)同账户身份,同步你的数据", "funcs": {
+                    f"{command_start}用户信息": "查询当前用户的通用用户的用户名和密钥.(5秒后撤回,但建议私聊使用)",
+                    f"{command_start}更改绑定": "将当前平台账户绑定到指定通用账户,实现跨平台数据互通",
+                }}, "webui": {"des": "管理webui", "funcs": {
+                    f"{command_start}开启webui": "默认开启,打开webui,并返回webui开启的端口(管理员可用)",
+                    f"{command_start}关闭webui": "请在使用webui后关闭(管理员可用)",
+                }}
+            }
+            pic_bytes = await menu_to_pic(help_dict, 800)
             with open(Super_Msg_Path, "wb") as f:
                 f.write(pic_bytes)
             get_super_pic()
         else:
             with open(Super_Msg_Path, "rb") as f:
                 pic_bytes = f.read()
         await send_img(pic_bytes, matcher, bot, event)
         await matcher.finish()
     else:
-        help_dict = {
-            f"{PRIVATE_COMMAND}bot名称\n+询问的问题": "与指定属于自己的bot对话\n(可使用'回复'来连续对话)",
-            f"{PUBLIC_COMMAND}bot名称\n+询问的问题": "与指定属于公共的bot对话\n(可使用'回复'来连续对话)",
-            f"{PRIVATE_COMMAND}所有bot": "查询所有的可用的属于自己的bot",
-            f"{PUBLIC_COMMAND}所有bot": "查询所有的可用的公共的bot",
-            f"{PRIVATE_COMMAND}创建bot": "创建新的属于自己的bot",
-            f"{PRIVATE_COMMAND}改名bot": "更改自己的bot的名称",
-            f"{PRIVATE_COMMAND}删除bot": "删除指定自己的bot",
-            f"{command_start}所有预设": "给出所有预设的名称",
-            f"{command_start}查询预设": "查询指定预设的内容",
-            f"{command_start}所有前缀": "给出所有前缀的名称",
-            f"{command_start}查询前缀": "查询指定前缀的内容",
-            f"{command_start}用户信息": "查询当前平台账户的通用账户的用户名和密钥.(建议私聊使用)",
-            f"{command_start}更改绑定": "将当前平台账户绑定到指定通用账户,实现跨平台数据互通",
-        }
         if not Generated_Help_Msg_Pic:
-            pic_bytes = await menu_to_pic(help_dict, 800, font_size=30)
+            help_dict = {
+                "私有bot": {"des": "使用和管理自己独有的bot的命令,私有bot只有主人可使用,其他人无法使用", "funcs": {
+                    f"{PRIVATE_COMMAND}bot名称+询问的问题": "与指定属于自己的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)",
+                    f"{PRIVATE_COMMAND}所有bot": "查询所有的可用的私有的bot,以获取bot名称和相关信息",
+                    f"{PRIVATE_COMMAND}创建bot": "创建新的私有的bot",
+                    f"{PRIVATE_COMMAND}改名bot": "更改自己的bot的名称",
+                    f"{PRIVATE_COMMAND}删除bot": "删除指定自己的bot",
+                }},
+                "公有bot": {"des": "使用公有bot的命令", "funcs": {
+                    f"{PUBLIC_COMMAND}bot名称+询问的问题": "与指定属于公共的bot对话\n(可使用'回复'某bot最后一个答案来连续和它对话)\n(可回复'清除历史','刷新对话'来清除bot的对话记忆)",
+                    f"{PUBLIC_COMMAND}所有bot": "查询所有的可用的公共的bot,以获取bot名称和相关信息",
+                }}, "预设": {"des": "预设将在一次和bot的连续对话开始时发送给bot进行初始化,清除对话历史后也将重新初始化", "funcs": {
+                    f"{command_start}所有预设": "列出所有预设的名称和缩略的内容",
+                    f"{command_start}查询预设": "查询指定预设的具体详尽内容",
+                }}, "前缀": {"des": "前缀在每次和bot对话时都会附带在消息前面", "funcs": {
+                    f"{command_start}所有前缀": "列出所有前缀的的名称和缩略的内容",
+                    f"{command_start}查询前缀": "查询指定前缀的具体详尽内容",
+                }}, "账户信息": {"des": "用来实现跨平台(qq,tg等)同账户身份,同步你的数据", "funcs": {
+                    f"{command_start}用户信息": "查询当前用户的通用用户的用户名和密钥.(5秒后撤回,但建议私聊使用)",
+                    f"{command_start}更改绑定": "将当前平台账户绑定到指定通用账户,实现跨平台数据互通",
+                }}
+            }
+            pic_bytes = await menu_to_pic(help_dict, 800)
             with open(Help_Msg_Path, "wb") as f:
                 f.write(pic_bytes)
             get_help_pic()
         else:
             with open(Help_Msg_Path, "rb") as f:
                 pic_bytes = f.read()
         await send_img(pic_bytes, matcher, bot, event)
@@ -225,15 +240,15 @@
 Prompt_Msg_Path.touch()
 
 
 @all_prompts.handle()
 async def all_prompts_(bot: Bot, matcher: Matcher, event: MessageEvent):
     prompts_dict = prompts.show_list()
     if not prompts.Generated:
-        pic_bytes = await menu_to_pic(menu=prompts_dict, headline="预设列表", width=800,
+        pic_bytes = await list_to_pic(prompts_dict, headline="预设列表", width=800,
                                       description="下面只展示了前200个字符")
         prompts.generate_pic()
         with open(Prompt_Msg_Path, "wb") as f:
             f.write(pic_bytes)
     else:
         with open(Prompt_Msg_Path, "rb") as f:
             pic_bytes = f.read()
@@ -431,15 +446,15 @@
 Prefix_Msg_Path.touch()
 
 
 @all_prefixes.handle()
 async def all_prefixes_(bot: Bot, matcher: Matcher, event: MessageEvent):
     prefixes_dict = prefixes.show_list()
     if not prefixes.Generated:
-        pic_bytes = await menu_to_pic(menu=prefixes_dict, headline="前缀列表", width=800,
+        pic_bytes = await list_to_pic(prefixes_dict, headline="前缀列表", width=800,
                                       description="下面只展示了前200个字符")
         prefixes.generate_pic()
         with open(Prefix_Msg_Path, "wb") as f:
             f.write(pic_bytes)
     else:
         with open(Prefix_Msg_Path, "rb") as f:
             pic_bytes = f.read()
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/platforms/temp_bots.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/platforms/temp_bots.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/markdown.css` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/markdown.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,1007 +1,1006 @@
 .markdown-body {
-    -ms-text-size-adjust: 100%;
-    -webkit-text-size-adjust: 100%;
-    margin: 0;
-    color: #24292f;
-    background-color: #ffffff;
-    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji";
-    font-size: 16px;
-    line-height: 1.5;
-    word-wrap: break-word;
+  -ms-text-size-adjust: 100%;
+  -webkit-text-size-adjust: 100%;
+  margin: 0;
+  color: #24292f;
+  background-color: #ffffff;
+  font-family: -apple-system,BlinkMacSystemFont,"Segoe UI","Noto Sans",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji";
+  font-size: 16px;
+  line-height: 1.5;
+  word-wrap: break-word;
 }
 
 .markdown-body .octicon {
-    display: inline-block;
-    fill: currentColor;
-    vertical-align: text-bottom;
+  display: inline-block;
+  fill: currentColor;
+  vertical-align: text-bottom;
 }
 
 .markdown-body h1:hover .anchor .octicon-link:before,
 .markdown-body h2:hover .anchor .octicon-link:before,
 .markdown-body h3:hover .anchor .octicon-link:before,
 .markdown-body h4:hover .anchor .octicon-link:before,
 .markdown-body h5:hover .anchor .octicon-link:before,
 .markdown-body h6:hover .anchor .octicon-link:before {
-    width: 16px;
-    height: 16px;
-    content: ' ';
-    display: inline-block;
-    background-color: currentColor;
-    -webkit-mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
-    mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
+  width: 16px;
+  height: 16px;
+  content: ' ';
+  display: inline-block;
+  background-color: currentColor;
+  -webkit-mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
+  mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
 }
 
 .markdown-body details,
 .markdown-body figcaption,
 .markdown-body figure {
-    display: block;
+  display: block;
 }
 
 .markdown-body summary {
-    display: list-item;
+  display: list-item;
 }
 
 .markdown-body [hidden] {
-    display: none !important;
+  display: none !important;
 }
 
 .markdown-body a {
-    background-color: transparent;
-    color: #0969da;
-    text-decoration: none;
+  background-color: transparent;
+  color: #0969da;
+  text-decoration: none;
 }
 
 .markdown-body abbr[title] {
-    border-bottom: none;
-    text-decoration: underline dotted;
+  border-bottom: none;
+  text-decoration: underline dotted;
 }
 
 .markdown-body b,
 .markdown-body strong {
-    font-weight: 600;
+  font-weight: 600;
 }
 
 .markdown-body dfn {
-    font-style: italic;
+  font-style: italic;
 }
 
 .markdown-body h1 {
-    margin: .67em 0;
-    font-weight: 600;
-    padding-bottom: .3em;
-    font-size: 2em;
-    border-bottom: 1px solid hsla(210, 18%, 87%, 1);
+  margin: .67em 0;
+  font-weight: 600;
+  padding-bottom: .3em;
+  font-size: 2em;
+  border-bottom: 1px solid hsla(210,18%,87%,1);
 }
 
 .markdown-body mark {
-    background-color: #fff8c5;
-    color: #24292f;
+  background-color: #fff8c5;
+  color: #24292f;
 }
 
 .markdown-body small {
-    font-size: 90%;
+  font-size: 90%;
 }
 
 .markdown-body sub,
 .markdown-body sup {
-    font-size: 75%;
-    line-height: 0;
-    position: relative;
-    vertical-align: baseline;
+  font-size: 75%;
+  line-height: 0;
+  position: relative;
+  vertical-align: baseline;
 }
 
 .markdown-body sub {
-    bottom: -0.25em;
+  bottom: -0.25em;
 }
 
 .markdown-body sup {
-    top: -0.5em;
+  top: -0.5em;
 }
 
 .markdown-body img {
-    border-style: none;
-    max-width: 100%;
-    box-sizing: content-box;
-    background-color: #ffffff;
+  border-style: none;
+  max-width: 100%;
+  box-sizing: content-box;
+  background-color: #ffffff;
 }
 
 .markdown-body code,
 .markdown-body kbd,
 .markdown-body pre,
 .markdown-body samp {
-    font-family: monospace;
-    font-size: 1em;
+  font-family: monospace;
+  font-size: 1em;
 }
 
 .markdown-body figure {
-    margin: 1em 40px;
+  margin: 1em 40px;
 }
 
 .markdown-body hr {
-    box-sizing: content-box;
-    overflow: hidden;
-    background: transparent;
-    border-bottom: 1px solid hsla(210, 18%, 87%, 1);
-    height: .25em;
-    padding: 0;
-    margin: 24px 0;
-    background-color: #d0d7de;
-    border: 0;
+  box-sizing: content-box;
+  overflow: hidden;
+  background: transparent;
+  border-bottom: 1px solid hsla(210,18%,87%,1);
+  height: .25em;
+  padding: 0;
+  margin: 24px 0;
+  background-color: #d0d7de;
+  border: 0;
 }
 
 .markdown-body input {
-    font: inherit;
-    margin: 0;
-    overflow: visible;
-    font-family: inherit;
-    font-size: inherit;
-    line-height: inherit;
+  font: inherit;
+  margin: 0;
+  overflow: visible;
+  font-family: inherit;
+  font-size: inherit;
+  line-height: inherit;
 }
 
 .markdown-body [type=button],
 .markdown-body [type=reset],
 .markdown-body [type=submit] {
-    -webkit-appearance: button;
+  -webkit-appearance: button;
 }
 
 .markdown-body [type=checkbox],
 .markdown-body [type=radio] {
-    box-sizing: border-box;
-    padding: 0;
+  box-sizing: border-box;
+  padding: 0;
 }
 
 .markdown-body [type=number]::-webkit-inner-spin-button,
 .markdown-body [type=number]::-webkit-outer-spin-button {
-    height: auto;
+  height: auto;
 }
 
 .markdown-body [type=search]::-webkit-search-cancel-button,
 .markdown-body [type=search]::-webkit-search-decoration {
-    -webkit-appearance: none;
+  -webkit-appearance: none;
 }
 
 .markdown-body ::-webkit-input-placeholder {
-    color: inherit;
-    opacity: .54;
+  color: inherit;
+  opacity: .54;
 }
 
 .markdown-body ::-webkit-file-upload-button {
-    -webkit-appearance: button;
-    font: inherit;
+  -webkit-appearance: button;
+  font: inherit;
 }
 
 .markdown-body a:hover {
-    text-decoration: underline;
+  text-decoration: underline;
 }
 
 .markdown-body ::placeholder {
-    color: #6e7781;
-    opacity: 1;
+  color: #6e7781;
+  opacity: 1;
 }
 
 .markdown-body hr::before {
-    display: table;
-    content: "";
+  display: table;
+  content: "";
 }
 
 .markdown-body hr::after {
-    display: table;
-    clear: both;
-    content: "";
+  display: table;
+  clear: both;
+  content: "";
 }
 
 .markdown-body table {
-    border-spacing: 0;
-    border-collapse: collapse;
-    background-color: #d3efd8 !important;
-    display: inline-table;
-    width: max-content;
-    max-width: 100%;
-    overflow: auto;
+  border-spacing: 0;
+  border-collapse: collapse;
+  display: block;
+  width: max-content;
+  max-width: 100%;
+  overflow: auto;
 }
 
 .markdown-body td,
 .markdown-body th {
-    padding: 0;
+  padding: 0;
 }
 
 .markdown-body details summary {
-    cursor: pointer;
+  cursor: pointer;
 }
 
-.markdown-body details:not([open]) > *:not(summary) {
-    display: none !important;
+.markdown-body details:not([open])>*:not(summary) {
+  display: none !important;
 }
 
 .markdown-body a:focus,
 .markdown-body [role=button]:focus,
 .markdown-body input[type=radio]:focus,
 .markdown-body input[type=checkbox]:focus {
-    outline: 2px solid #0969da;
-    outline-offset: -2px;
-    box-shadow: none;
+  outline: 2px solid #0969da;
+  outline-offset: -2px;
+  box-shadow: none;
 }
 
 .markdown-body a:focus:not(:focus-visible),
 .markdown-body [role=button]:focus:not(:focus-visible),
 .markdown-body input[type=radio]:focus:not(:focus-visible),
 .markdown-body input[type=checkbox]:focus:not(:focus-visible) {
-    outline: solid 1px transparent;
+  outline: solid 1px transparent;
 }
 
 .markdown-body a:focus-visible,
 .markdown-body [role=button]:focus-visible,
 .markdown-body input[type=radio]:focus-visible,
 .markdown-body input[type=checkbox]:focus-visible {
-    outline: 2px solid #0969da;
-    outline-offset: -2px;
-    box-shadow: none;
+  outline: 2px solid #0969da;
+  outline-offset: -2px;
+  box-shadow: none;
 }
 
 .markdown-body a:not([class]):focus,
 .markdown-body a:not([class]):focus-visible,
 .markdown-body input[type=radio]:focus,
 .markdown-body input[type=radio]:focus-visible,
 .markdown-body input[type=checkbox]:focus,
 .markdown-body input[type=checkbox]:focus-visible {
-    outline-offset: 0;
+  outline-offset: 0;
 }
 
 .markdown-body kbd {
-    display: inline-block;
-    padding: 3px 5px;
-    font: 11px ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, Liberation Mono, monospace;
-    line-height: 10px;
-    color: #24292f;
-    vertical-align: middle;
-    background-color: #e7ffeb;
-    border: solid 1px #e4f8e8;
-    border-bottom-color: #e4f8e8;
-    border-radius: 6px;
-    box-shadow: inset 0 -1px 0 #e4f8e8;
+  display: inline-block;
+  padding: 3px 5px;
+  font: 11px ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
+  line-height: 10px;
+  color: #24292f;
+  vertical-align: middle;
+  background-color: #f6f8fa;
+  border: solid 1px rgba(175,184,193,0.2);
+  border-bottom-color: rgba(175,184,193,0.2);
+  border-radius: 6px;
+  box-shadow: inset 0 -1px 0 rgba(175,184,193,0.2);
 }
 
 .markdown-body h1,
 .markdown-body h2,
 .markdown-body h3,
 .markdown-body h4,
 .markdown-body h5,
 .markdown-body h6 {
-    margin-top: 24px;
-    margin-bottom: 16px;
-    font-weight: 600;
-    line-height: 1.25;
+  margin-top: 24px;
+  margin-bottom: 16px;
+  font-weight: 600;
+  line-height: 1.25;
 }
 
 .markdown-body h2 {
-    font-weight: 600;
-    padding-bottom: .3em;
-    font-size: 1.5em;
-    border-bottom: 1px solid hsla(210, 18%, 87%, 1);
+  font-weight: 600;
+  padding-bottom: .3em;
+  font-size: 1.5em;
+  border-bottom: 1px solid hsla(210,18%,87%,1);
 }
 
 .markdown-body h3 {
-    font-weight: 600;
-    font-size: 1.25em;
+  font-weight: 600;
+  font-size: 1.25em;
 }
 
 .markdown-body h4 {
-    font-weight: 600;
-    font-size: 1em;
+  font-weight: 600;
+  font-size: 1em;
 }
 
 .markdown-body h5 {
-    font-weight: 600;
-    font-size: .875em;
+  font-weight: 600;
+  font-size: .875em;
 }
 
 .markdown-body h6 {
-    font-weight: 600;
-    font-size: .85em;
-    color: #57606a;
+  font-weight: 600;
+  font-size: .85em;
+  color: #57606a;
 }
 
 .markdown-body p {
-    margin-top: 0;
-    margin-bottom: 10px;
+  margin-top: 0;
+  margin-bottom: 10px;
 }
 
 .markdown-body blockquote {
-    margin: 0;
-    padding: 0 1em;
-    color: #57606a;
-    border-left: .25em solid #d0d7de;
+  margin: 0;
+  padding: 0 1em;
+  color: #57606a;
+  border-left: .25em solid #d0d7de;
 }
 
 .markdown-body ul,
 .markdown-body ol {
-    margin-top: 0;
-    margin-bottom: 0;
-    padding-left: 2em;
+  margin-top: 0;
+  margin-bottom: 0;
+  padding-left: 2em;
 }
 
 .markdown-body ol ol,
 .markdown-body ul ol {
-    list-style-type: lower-roman;
+  list-style-type: lower-roman;
 }
 
 .markdown-body ul ul ol,
 .markdown-body ul ol ol,
 .markdown-body ol ul ol,
 .markdown-body ol ol ol {
-    list-style-type: lower-alpha;
+  list-style-type: lower-alpha;
 }
 
 .markdown-body dd {
-    margin-left: 0;
+  margin-left: 0;
 }
 
 .markdown-body tt,
 .markdown-body code,
 .markdown-body samp {
-    font-family: ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, Liberation Mono, monospace;
-    font-size: 12px;
+  font-family: ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
+  font-size: 12px;
 }
 
 .markdown-body pre {
-    margin-top: 0;
-    margin-bottom: 0;
-    font-family: ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, Liberation Mono, monospace;
-    font-size: 12px;
-    word-wrap: normal;
+  margin-top: 0;
+  margin-bottom: 0;
+  font-family: ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
+  font-size: 12px;
+  word-wrap: normal;
 }
 
 .markdown-body .octicon {
-    display: inline-block;
-    overflow: visible !important;
-    vertical-align: text-bottom;
-    fill: currentColor;
+  display: inline-block;
+  overflow: visible !important;
+  vertical-align: text-bottom;
+  fill: currentColor;
 }
 
 .markdown-body input::-webkit-outer-spin-button,
 .markdown-body input::-webkit-inner-spin-button {
-    margin: 0;
-    -webkit-appearance: none;
-    appearance: none;
+  margin: 0;
+  -webkit-appearance: none;
+  appearance: none;
 }
 
 .markdown-body::before {
-    display: table;
-    content: "";
+  display: table;
+  content: "";
 }
 
 .markdown-body::after {
-    display: table;
-    clear: both;
-    content: "";
+  display: table;
+  clear: both;
+  content: "";
 }
 
-.markdown-body > *:first-child {
-    margin-top: 0 !important;
+.markdown-body>*:first-child {
+  margin-top: 0 !important;
 }
 
-.markdown-body > *:last-child {
-    margin-bottom: 0 !important;
+.markdown-body>*:last-child {
+  margin-bottom: 0 !important;
 }
 
 .markdown-body a:not([href]) {
-    color: inherit;
-    text-decoration: none;
+  color: inherit;
+  text-decoration: none;
 }
 
 .markdown-body .absent {
-    color: #cf222e;
+  color: #cf222e;
 }
 
 .markdown-body .anchor {
-    float: left;
-    padding-right: 4px;
-    margin-left: -20px;
-    line-height: 1;
+  float: left;
+  padding-right: 4px;
+  margin-left: -20px;
+  line-height: 1;
 }
 
 .markdown-body .anchor:focus {
-    outline: none;
+  outline: none;
 }
 
 .markdown-body p,
 .markdown-body blockquote,
 .markdown-body ul,
 .markdown-body ol,
 .markdown-body dl,
 .markdown-body table,
 .markdown-body pre,
 .markdown-body details {
-    margin-top: 0;
-    margin-bottom: 16px;
+  margin-top: 0;
+  margin-bottom: 16px;
 }
 
-.markdown-body blockquote > :first-child {
-    margin-top: 0;
+.markdown-body blockquote>:first-child {
+  margin-top: 0;
 }
 
-.markdown-body blockquote > :last-child {
-    margin-bottom: 0;
+.markdown-body blockquote>:last-child {
+  margin-bottom: 0;
 }
 
 .markdown-body h1 .octicon-link,
 .markdown-body h2 .octicon-link,
 .markdown-body h3 .octicon-link,
 .markdown-body h4 .octicon-link,
 .markdown-body h5 .octicon-link,
 .markdown-body h6 .octicon-link {
-    color: #24292f;
-    vertical-align: middle;
-    visibility: hidden;
+  color: #24292f;
+  vertical-align: middle;
+  visibility: hidden;
 }
 
 .markdown-body h1:hover .anchor,
 .markdown-body h2:hover .anchor,
 .markdown-body h3:hover .anchor,
 .markdown-body h4:hover .anchor,
 .markdown-body h5:hover .anchor,
 .markdown-body h6:hover .anchor {
-    text-decoration: none;
+  text-decoration: none;
 }
 
 .markdown-body h1:hover .anchor .octicon-link,
 .markdown-body h2:hover .anchor .octicon-link,
 .markdown-body h3:hover .anchor .octicon-link,
 .markdown-body h4:hover .anchor .octicon-link,
 .markdown-body h5:hover .anchor .octicon-link,
 .markdown-body h6:hover .anchor .octicon-link {
-    visibility: visible;
+  visibility: visible;
 }
 
 .markdown-body h1 tt,
 .markdown-body h1 code,
 .markdown-body h2 tt,
 .markdown-body h2 code,
 .markdown-body h3 tt,
 .markdown-body h3 code,
 .markdown-body h4 tt,
 .markdown-body h4 code,
 .markdown-body h5 tt,
 .markdown-body h5 code,
 .markdown-body h6 tt,
 .markdown-body h6 code {
-    padding: 0 .2em;
-    font-size: inherit;
+  padding: 0 .2em;
+  font-size: inherit;
 }
 
 .markdown-body summary h1,
 .markdown-body summary h2,
 .markdown-body summary h3,
 .markdown-body summary h4,
 .markdown-body summary h5,
 .markdown-body summary h6 {
-    display: inline-block;
+  display: inline-block;
 }
 
 .markdown-body summary h1 .anchor,
 .markdown-body summary h2 .anchor,
 .markdown-body summary h3 .anchor,
 .markdown-body summary h4 .anchor,
 .markdown-body summary h5 .anchor,
 .markdown-body summary h6 .anchor {
-    margin-left: -40px;
+  margin-left: -40px;
 }
 
 .markdown-body summary h1,
 .markdown-body summary h2 {
-    padding-bottom: 0;
-    border-bottom: 0;
+  padding-bottom: 0;
+  border-bottom: 0;
 }
 
 .markdown-body ul.no-list,
 .markdown-body ol.no-list {
-    padding: 0;
-    list-style-type: none;
+  padding: 0;
+  list-style-type: none;
 }
 
 .markdown-body ol[type=a] {
-    list-style-type: lower-alpha;
+  list-style-type: lower-alpha;
 }
 
 .markdown-body ol[type=A] {
-    list-style-type: upper-alpha;
+  list-style-type: upper-alpha;
 }
 
 .markdown-body ol[type=i] {
-    list-style-type: lower-roman;
+  list-style-type: lower-roman;
 }
 
 .markdown-body ol[type=I] {
-    list-style-type: upper-roman;
+  list-style-type: upper-roman;
 }
 
 .markdown-body ol[type="1"] {
-    list-style-type: decimal;
+  list-style-type: decimal;
 }
 
-.markdown-body div > ol:not([type]) {
-    list-style-type: decimal;
+.markdown-body div>ol:not([type]) {
+  list-style-type: decimal;
 }
 
 .markdown-body ul ul,
 .markdown-body ul ol,
 .markdown-body ol ol,
 .markdown-body ol ul {
-    margin-top: 0;
-    margin-bottom: 0;
+  margin-top: 0;
+  margin-bottom: 0;
 }
 
-.markdown-body li > p {
-    margin-top: 16px;
+.markdown-body li>p {
+  margin-top: 16px;
 }
 
-.markdown-body li + li {
-    margin-top: .25em;
+.markdown-body li+li {
+  margin-top: .25em;
 }
 
 .markdown-body dl {
-    padding: 0;
+  padding: 0;
 }
 
 .markdown-body dl dt {
-    padding: 0;
-    margin-top: 16px;
-    font-size: 1em;
-    font-style: italic;
-    font-weight: 600;
+  padding: 0;
+  margin-top: 16px;
+  font-size: 1em;
+  font-style: italic;
+  font-weight: 600;
 }
 
 .markdown-body dl dd {
-    padding: 0 16px;
-    margin-bottom: 16px;
+  padding: 0 16px;
+  margin-bottom: 16px;
 }
 
 .markdown-body table th {
-    font-weight: 600;
+  font-weight: 600;
 }
 
 .markdown-body table th,
 .markdown-body table td {
-    padding: 6px 13px;
-    border: 1px solid #d0d7de;
+  padding: 6px 13px;
+  border: 1px solid #d0d7de;
 }
 
 .markdown-body table tr {
-    background-color: #e7ffeb;
-    border-top: 1px solid hsla(210, 18%, 87%, 1);
+  background-color: #ffffff;
+  border-top: 1px solid hsla(210,18%,87%,1);
 }
 
 .markdown-body table tr:nth-child(2n) {
-    background-color: #e4f8e8 !important;
+  background-color: #f6f8fa;
 }
 
 .markdown-body table img {
-    background-color: transparent;
+  background-color: transparent;
 }
 
 .markdown-body img[align=right] {
-    padding-left: 20px;
+  padding-left: 20px;
 }
 
 .markdown-body img[align=left] {
-    padding-right: 20px;
+  padding-right: 20px;
 }
 
 .markdown-body .emoji {
-    max-width: none;
-    vertical-align: text-top;
-    background-color: transparent;
+  max-width: none;
+  vertical-align: text-top;
+  background-color: transparent;
 }
 
 .markdown-body span.frame {
-    display: block;
-    overflow: hidden;
+  display: block;
+  overflow: hidden;
 }
 
-.markdown-body span.frame > span {
-    display: block;
-    float: left;
-    width: auto;
-    padding: 7px;
-    margin: 13px 0 0;
-    overflow: hidden;
-    border: 1px solid #d0d7de;
+.markdown-body span.frame>span {
+  display: block;
+  float: left;
+  width: auto;
+  padding: 7px;
+  margin: 13px 0 0;
+  overflow: hidden;
+  border: 1px solid #d0d7de;
 }
 
 .markdown-body span.frame span img {
-    display: block;
-    float: left;
+  display: block;
+  float: left;
 }
 
 .markdown-body span.frame span span {
-    display: block;
-    padding: 5px 0 0;
-    clear: both;
-    color: #24292f;
+  display: block;
+  padding: 5px 0 0;
+  clear: both;
+  color: #24292f;
 }
 
 .markdown-body span.align-center {
-    display: block;
-    overflow: hidden;
-    clear: both;
+  display: block;
+  overflow: hidden;
+  clear: both;
 }
 
-.markdown-body span.align-center > span {
-    display: block;
-    margin: 13px auto 0;
-    overflow: hidden;
-    text-align: center;
+.markdown-body span.align-center>span {
+  display: block;
+  margin: 13px auto 0;
+  overflow: hidden;
+  text-align: center;
 }
 
 .markdown-body span.align-center span img {
-    margin: 0 auto;
-    text-align: center;
+  margin: 0 auto;
+  text-align: center;
 }
 
 .markdown-body span.align-right {
-    display: block;
-    overflow: hidden;
-    clear: both;
+  display: block;
+  overflow: hidden;
+  clear: both;
 }
 
-.markdown-body span.align-right > span {
-    display: block;
-    margin: 13px 0 0;
-    overflow: hidden;
-    text-align: right;
+.markdown-body span.align-right>span {
+  display: block;
+  margin: 13px 0 0;
+  overflow: hidden;
+  text-align: right;
 }
 
 .markdown-body span.align-right span img {
-    margin: 0;
-    text-align: right;
+  margin: 0;
+  text-align: right;
 }
 
 .markdown-body span.float-left {
-    display: block;
-    float: left;
-    margin-right: 13px;
-    overflow: hidden;
+  display: block;
+  float: left;
+  margin-right: 13px;
+  overflow: hidden;
 }
 
 .markdown-body span.float-left span {
-    margin: 13px 0 0;
+  margin: 13px 0 0;
 }
 
 .markdown-body span.float-right {
-    display: block;
-    float: right;
-    margin-left: 13px;
-    overflow: hidden;
+  display: block;
+  float: right;
+  margin-left: 13px;
+  overflow: hidden;
 }
 
-.markdown-body span.float-right > span {
-    display: block;
-    margin: 13px auto 0;
-    overflow: hidden;
-    text-align: right;
+.markdown-body span.float-right>span {
+  display: block;
+  margin: 13px auto 0;
+  overflow: hidden;
+  text-align: right;
 }
 
 .markdown-body code,
 .markdown-body tt {
-    padding: .2em .4em;
-    margin: 0;
-    font-size: 85%;
-    white-space: break-spaces;
-    background-color: #e4f8e8;
-    border-radius: 6px;
+  padding: .2em .4em;
+  margin: 0;
+  font-size: 85%;
+  white-space: break-spaces;
+  background-color: rgba(175,184,193,0.2);
+  border-radius: 6px;
 }
 
 .markdown-body code br,
 .markdown-body tt br {
-    display: none;
+  display: none;
 }
 
 .markdown-body del code {
-    text-decoration: inherit;
+  text-decoration: inherit;
 }
 
 .markdown-body samp {
-    font-size: 85%;
+  font-size: 85%;
 }
 
 .markdown-body pre code {
-    font-size: 100%;
+  font-size: 100%;
 }
 
-.markdown-body pre > code {
-    padding: 0;
-    margin: 0;
-    word-break: normal;
-    white-space: pre;
-    background: transparent;
-    border: 0;
+.markdown-body pre>code {
+  padding: 0;
+  margin: 0;
+  word-break: normal;
+  white-space: pre;
+  background: transparent;
+  border: 0;
 }
 
 .markdown-body .highlight {
-    margin-bottom: 16px;
+  margin-bottom: 16px;
 }
 
 .markdown-body .highlight pre {
-    margin-bottom: 0;
-    word-break: normal;
+  margin-bottom: 0;
+  word-break: normal;
 }
 
 .markdown-body .highlight pre,
 .markdown-body pre {
-    padding: 16px;
-    overflow: auto;
-    font-size: 85%;
-    line-height: 1.45;
-    background-color: #e7ffeb;
-    border-radius: 6px;
+  padding: 16px;
+  overflow: auto;
+  font-size: 85%;
+  line-height: 1.45;
+  background-color: #f6f8fa;
+  border-radius: 6px;
 }
 
 .markdown-body pre code,
 .markdown-body pre tt {
-    display: inline;
-    max-width: auto;
-    padding: 0;
-    margin: 0;
-    overflow: visible;
-    line-height: inherit;
-    word-wrap: normal;
-    background-color: transparent;
-    border: 0;
+  display: inline;
+  max-width: auto;
+  padding: 0;
+  margin: 0;
+  overflow: visible;
+  line-height: inherit;
+  word-wrap: normal;
+  background-color: transparent;
+  border: 0;
 }
 
 .markdown-body .csv-data td,
 .markdown-body .csv-data th {
-    padding: 5px;
-    overflow: hidden;
-    font-size: 12px;
-    line-height: 1;
-    text-align: left;
-    white-space: nowrap;
+  padding: 5px;
+  overflow: hidden;
+  font-size: 12px;
+  line-height: 1;
+  text-align: left;
+  white-space: nowrap;
 }
 
 .markdown-body .csv-data .blob-num {
-    padding: 10px 8px 9px;
-    text-align: right;
-    background: #ffffff;
-    border: 0;
+  padding: 10px 8px 9px;
+  text-align: right;
+  background: #ffffff;
+  border: 0;
 }
 
 .markdown-body .csv-data tr {
-    border-top: 0;
+  border-top: 0;
 }
 
 .markdown-body .csv-data th {
-    font-weight: 600;
-    background: #e7ffeb;
-    border-top: 0;
+  font-weight: 600;
+  background: #f6f8fa;
+  border-top: 0;
 }
 
 .markdown-body [data-footnote-ref]::before {
-    content: "[";
+  content: "[";
 }
 
 .markdown-body [data-footnote-ref]::after {
-    content: "]";
+  content: "]";
 }
 
 .markdown-body .footnotes {
-    font-size: 12px;
-    color: #57606a;
-    border-top: 1px solid #d0d7de;
+  font-size: 12px;
+  color: #57606a;
+  border-top: 1px solid #d0d7de;
 }
 
 .markdown-body .footnotes ol {
-    padding-left: 16px;
+  padding-left: 16px;
 }
 
 .markdown-body .footnotes ol ul {
-    display: inline-block;
-    padding-left: 16px;
-    margin-top: 16px;
+  display: inline-block;
+  padding-left: 16px;
+  margin-top: 16px;
 }
 
 .markdown-body .footnotes li {
-    position: relative;
+  position: relative;
 }
 
 .markdown-body .footnotes li:target::before {
-    position: absolute;
-    top: -8px;
-    right: -8px;
-    bottom: -8px;
-    left: -24px;
-    pointer-events: none;
-    content: "";
-    border: 2px solid #0969da;
-    border-radius: 6px;
+  position: absolute;
+  top: -8px;
+  right: -8px;
+  bottom: -8px;
+  left: -24px;
+  pointer-events: none;
+  content: "";
+  border: 2px solid #0969da;
+  border-radius: 6px;
 }
 
 .markdown-body .footnotes li:target {
-    color: #24292f;
+  color: #24292f;
 }
 
 .markdown-body .footnotes .data-footnote-backref g-emoji {
-    font-family: monospace;
+  font-family: monospace;
 }
 
 .markdown-body .pl-c {
-    color: #6e7781;
+  color: #6e7781;
 }
 
 .markdown-body .pl-c1,
 .markdown-body .pl-s .pl-v {
-    color: #0550ae;
+  color: #0550ae;
 }
 
 .markdown-body .pl-e,
 .markdown-body .pl-en {
-    color: #8250df;
+  color: #8250df;
 }
 
 .markdown-body .pl-smi,
 .markdown-body .pl-s .pl-s1 {
-    color: #24292f;
+  color: #24292f;
 }
 
 .markdown-body .pl-ent {
-    color: #116329;
+  color: #116329;
 }
 
 .markdown-body .pl-k {
-    color: #cf222e;
+  color: #cf222e;
 }
 
 .markdown-body .pl-s,
 .markdown-body .pl-pds,
 .markdown-body .pl-s .pl-pse .pl-s1,
 .markdown-body .pl-sr,
 .markdown-body .pl-sr .pl-cce,
 .markdown-body .pl-sr .pl-sre,
 .markdown-body .pl-sr .pl-sra {
-    color: #0a3069;
+  color: #0a3069;
 }
 
 .markdown-body .pl-v,
 .markdown-body .pl-smw {
-    color: #953800;
+  color: #953800;
 }
 
 .markdown-body .pl-bu {
-    color: #82071e;
+  color: #82071e;
 }
 
 .markdown-body .pl-ii {
-    color: #e7ffeb;
-    background-color: #82071e;
+  color: #f6f8fa;
+  background-color: #82071e;
 }
 
 .markdown-body .pl-c2 {
-    color: #e7ffeb;
-    background-color: #cf222e;
+  color: #f6f8fa;
+  background-color: #cf222e;
 }
 
 .markdown-body .pl-sr .pl-cce {
-    font-weight: bold;
-    color: #116329;
+  font-weight: bold;
+  color: #116329;
 }
 
 .markdown-body .pl-ml {
-    color: #3b2300;
+  color: #3b2300;
 }
 
 .markdown-body .pl-mh,
 .markdown-body .pl-mh .pl-en,
 .markdown-body .pl-ms {
-    font-weight: bold;
-    color: #0550ae;
+  font-weight: bold;
+  color: #0550ae;
 }
 
 .markdown-body .pl-mi {
-    font-style: italic;
-    color: #24292f;
+  font-style: italic;
+  color: #24292f;
 }
 
 .markdown-body .pl-mb {
-    font-weight: bold;
-    color: #24292f;
+  font-weight: bold;
+  color: #24292f;
 }
 
 .markdown-body .pl-md {
-    color: #82071e;
-    background-color: #ffebe9;
+  color: #82071e;
+  background-color: #ffebe9;
 }
 
 .markdown-body .pl-mi1 {
-    color: #116329;
-    background-color: #dafbe1;
+  color: #116329;
+  background-color: #dafbe1;
 }
 
 .markdown-body .pl-mc {
-    color: #953800;
-    background-color: #ffd8b5;
+  color: #953800;
+  background-color: #ffd8b5;
 }
 
 .markdown-body .pl-mi2 {
-    color: #eaeef2;
-    background-color: #0550ae;
+  color: #eaeef2;
+  background-color: #0550ae;
 }
 
 .markdown-body .pl-mdr {
-    font-weight: bold;
-    color: #8250df;
+  font-weight: bold;
+  color: #8250df;
 }
 
 .markdown-body .pl-ba {
-    color: #57606a;
+  color: #57606a;
 }
 
 .markdown-body .pl-sg {
-    color: #8c959f;
+  color: #8c959f;
 }
 
 .markdown-body .pl-corl {
-    text-decoration: underline;
-    color: #0a3069;
+  text-decoration: underline;
+  color: #0a3069;
 }
 
 .markdown-body g-emoji {
-    display: inline-block;
-    min-width: 1ch;
-    font-family: "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
-    font-size: 1em;
-    font-style: normal !important;
-    font-weight: 400;
-    line-height: 1;
-    vertical-align: -0.075em;
+  display: inline-block;
+  min-width: 1ch;
+  font-family: "Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
+  font-size: 1em;
+  font-style: normal !important;
+  font-weight: 400;
+  line-height: 1;
+  vertical-align: -0.075em;
 }
 
 .markdown-body g-emoji img {
-    width: 1em;
-    height: 1em;
+  width: 1em;
+  height: 1em;
 }
 
 .markdown-body .task-list-item {
-    list-style-type: none;
+  list-style-type: none;
 }
 
 .markdown-body .task-list-item label {
-    font-weight: 400;
+  font-weight: 400;
 }
 
 .markdown-body .task-list-item.enabled label {
-    cursor: pointer;
+  cursor: pointer;
 }
 
-.markdown-body .task-list-item + .task-list-item {
-    margin-top: 4px;
+.markdown-body .task-list-item+.task-list-item {
+  margin-top: 4px;
 }
 
 .markdown-body .task-list-item .handle {
-    display: none;
+  display: none;
 }
 
 .markdown-body .task-list-item-checkbox {
-    margin: 0 .2em .25em -1.4em;
-    vertical-align: middle;
+  margin: 0 .2em .25em -1.4em;
+  vertical-align: middle;
 }
 
 .markdown-body .contains-task-list:dir(rtl) .task-list-item-checkbox {
-    margin: 0 -1.6em .25em .2em;
+  margin: 0 -1.6em .25em .2em;
 }
 
 .markdown-body .contains-task-list {
-    position: relative;
+  position: relative;
 }
 
 .markdown-body .contains-task-list:hover .task-list-item-convert-container,
 .markdown-body .contains-task-list:focus-within .task-list-item-convert-container {
-    display: block;
-    width: auto;
-    height: 24px;
-    overflow: visible;
-    clip: auto;
+  display: block;
+  width: auto;
+  height: 24px;
+  overflow: visible;
+  clip: auto;
 }
 
 .markdown-body ::-webkit-calendar-picker-indicator {
-    filter: invert(50%);
+  filter: invert(50%);
 }
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/menu.html` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/list.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html>
 <head>
     <style>
-        .eyecare {
-            background-color: #C7EDCC;
+        .back {
+            background-color: #d4baad29;
         }
 
         html {
             font-family: "Custom Font";
             font-size: 27px;
         }
 
@@ -15,20 +15,18 @@
             font-family: "Custom Font";
             src: url("{{font_path}}");
         }
 
         .box {
             font-family: "Custom Font";
             display: flex;
-            padding: 20px;
-            border-radius: 10px;
-            box-shadow: 2px 2px 4px rgba(213, 208, 208, 0);
+            padding-bottom: 20px;
+            padding-top: 20px;
             align-items: center;
             margin-bottom: 10px;
-
         }
 
         .index {
             font-family: "Custom Font";
             width: 30px;
             height: 30px;
             background: #E3EDCD;
@@ -40,46 +38,46 @@
             justify-content: center;
             border-radius: 4px;
             margin-right: 10px;
         }
 
         .left {
             font-family: "Custom Font";
-            flex: 1;
+            flex: 0.5;
             font-size: 30px;
             font-weight: bolder;
             color: #000000;
             padding: 6px;
-            border-radius: 10px;
+            border-radius: 20px;
             text-align: center;
+            border:2px solid black;
         }
 
         .right {
             font-family: "Custom Font";
             flex: 3;
             font-size: {{ font_size }}px;
             font-weight: normal;
             color: black;
-            padding: 6px;
             background: #fff;
             border-radius: 10px;
             border: 2px solid #efefef;
             position: relative;
             text-align: center;
             white-space: pre-wrap;
         }
 
         .right:before {
             font-family: "Custom Font";
             content: "";
             position: absolute;
-            left: -20px;
-            top: -20px;
-            width: calc(100% + 40px);
-            height: calc(100% + 40px);
+            left: -15px;
+            top: -15px;
+            width: calc(100% + 30px);
+            height: calc(100% + 30px);
             border-radius: 10px;
             z-index: -1;
             background: var(--pseudo-color);
         }
 
         h1 {
             font-family: "Custom Font";
@@ -92,23 +90,23 @@
             font-weight: normal;
             color: black;
             text-align: center;
         }
     </style>
 </head>
 
-<body class="eyecare">
+<body class="back">
 <h1>{{ headline }}</h1>
 <div class="description">{{ description }}</div>
-{% for key, value in menu.items() %}
-<div class="box">
-    <div class="index">{{ loop.index }}</div>
-    <div class="left">{{ key }}</div>
-    <div class="right">{{ value }}</div>
-</div>
+{% for key, value in list.items() %}
+    <div class="box">
+        <div class="index">{{ loop.index }}</div>
+        <div class="left">{{ key }}</div>
+        <div class="right">{{ value }}</div>
+    </div>
 {% endfor %}
 
 
 <script>
     var leftColors = [
         ["#ffd7d7", "#ffdfdf"],
         ["#fff0c2", "#fff7e6"],
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 ****** {{ headline }} ******
 {{ description }}
-{% for key, value in menu.items() %}
+{% for key, value in list.items() %}
 {{ loop.index }}
 {{ key }}
 {{ value }}
 {% endfor %}
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/PingFang.ttf` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/PingFang.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/templates/template.html` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/templates/template.html`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             padding: 10px;
             max-width: 100% !important;
             margin: auto;
             margin-bottom: 25px;
         }
 
         #content::after {
-            content: "Spark GPT 1.1.7";
+            content: "Spark GPT 1.1.8";
             position: absolute;
             bottom: 0px;
             right: 26px;
             font-size: 27px;
             color: gray;
         }
     </style>
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/nonebot_plugin_spark_gpt/utils/utils.py` & `nonebot_plugin_spark_gpt-1.1.8/nonebot_plugin_spark_gpt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.1.7/pyproject.toml` & `nonebot_plugin_spark_gpt-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_spark_gpt"
-version = "1.1.7"
+version = "1.1.8"
 description = "Spark-GPT,将多种来源的gpt接入qq,TG,Kook,Discord及更多平台,提供webui进行实时配置热更新,效率高超,使用便捷,管理完善,功能强大"
 authors = ["canxin121 <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_spark_gpt"},{ include = "nonebot"}]
 
 [tool.poetry.dependencies]
 nonebot-adapter-onebot = "^2.2.1"
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/README.md` & `nonebot_plugin_spark_gpt-1.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
     <img src="https://img.shields.io/github/last-commit/canxin121/Spark-GPT" alt="github">
     </a>
 </p>
 <div align="left">
 
-> 注意本插件使用了一个第三方程序进行文转图，所以不管你是否熟悉nonebot，请务必查看[(2).安装 wkhtmltopdf用以高效的文转图:](https://canxin121.github.io/docs/docs/Spark_GPT.html#_2-%E5%AE%89%E8%A3%85%E6%9C%AC%E6%8F%92%E4%BB%B6%E5%8F%8A%E4%BE%9D%E8%B5%96%E8%BD%AF%E4%BB%B6)
-
-## 最新版本号1.1.7
+## 最新版本号1.1.8
 # 详细教程-> [![残心文档库](source/doc.png)](https://canxin121.github.io/docs/docs/Spark_GPT.html)  
   
 ---
 # 介绍部分
 
 ## 功能特性
 
@@ -125,8 +123,8 @@
 | 删除前缀 | 删除指定前缀                   | SparkGPT管理员可用 |
 
 #### 6.以下是webui管理命令列表,所有命令前需要加上前缀/才能触发
 
 | 命令      | 命令含义                                             | 命令可用用户       |
 | --------- | ---------------------------------------------------- | ------------------ |
 | 开启webui | 默认开启,打开webui,并返回webui开启的端口(管理员可用) | SparkGPT管理员可用 |
-| 关闭webui | 请在使用webui后关闭(管理员可用)                      | SparkGPT管理员可用 |
+| 关闭webui | 请在使用webui后关闭(管理员可用)                      | SparkGPT管理员可用 |
```

#### html2text {}

```diff
@@ -1,19 +1,14 @@
                 [https://socialify.git.ci/canxin121/Spark-GPT/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                          ****** Spark-GPTä»åº ******
                                    Spark-GPT
                             [pypi] [python] [pypi]
                                [onebot]_[github]
->
-æ³¨ææ¬æä»¶ä½¿ç¨äºä¸ä¸ªç¬¬ä¸æ¹ç¨åºè¿è¡æè½¬å¾ï¼æä»¥ä¸ç®¡ä½ æ¯å¦çænonebotï¼è¯·å¡å¿æ¥ç
-[(2).å®è£ wkhtmltopdfç¨ä»¥é«æçæè½¬å¾:](https://canxin121.github.io/
-docs/docs/Spark_GPT.html#_2-
-%E5%AE%89%E8%A3%85%E6%9C%AC%E6%8F%92%E4%BB%B6%E5%8F%8A%E4%BE%9D%E8%B5%96%E8%BD%AF%E4%BB%B6)
-## ææ°çæ¬å·1.1.7 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
+## ææ°çæ¬å·1.1.8 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
 (https://canxin121.github.io/docs/docs/Spark_GPT.html) --- # ä»ç»é¨å ##
 åè½ç¹æ§ - æ±èä¼å¤æ¥æºçgpt(poe
 (chatgpt+claude),chatgptç½é¡µç,Newbing,slack
 claude,è®¯é£æç«,éä¹åé®),æ¯æå¤å¹³å°(tg,kook( åå¼é»å¦),qq
 (gocq),discord)ä½¿ç¨ä¸ä¸åå¹³å°ç¨æ·æ°æ®ç»å®äºé -
 æ¯æäººæ ¼é¢è®¾ååç¼ç³»ç»,æ¯ææè½¬å¾æè½¬é¾æ¥,æ¯ææ¯ä¸ªç¨æ·åå»ºä¸åæ¥æºä¸åäººæ ¼çbot,åæ¶æ¯æå¬ç¨å±åçbot
 -
```

### Comparing `nonebot_plugin_spark_gpt-1.1.7/PKG-INFO` & `nonebot_plugin_spark_gpt-1.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-spark-gpt
-Version: 1.1.7
+Version: 1.1.8
 Summary: Spark-GPT,将多种来源的gpt接入qq,TG,Kook,Discord及更多平台,提供webui进行实时配置热更新,效率高超,使用便捷,管理完善,功能强大
 Author: canxin121
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -46,17 +46,15 @@
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
     <img src="https://img.shields.io/github/last-commit/canxin121/Spark-GPT" alt="github">
     </a>
 </p>
 <div align="left">
 
-> 注意本插件使用了一个第三方程序进行文转图，所以不管你是否熟悉nonebot，请务必查看[(2).安装 wkhtmltopdf用以高效的文转图:](https://canxin121.github.io/docs/docs/Spark_GPT.html#_2-%E5%AE%89%E8%A3%85%E6%9C%AC%E6%8F%92%E4%BB%B6%E5%8F%8A%E4%BE%9D%E8%B5%96%E8%BD%AF%E4%BB%B6)
-
-## 最新版本号1.1.7
+## 最新版本号1.1.8
 # 详细教程-> [![残心文档库](source/doc.png)](https://canxin121.github.io/docs/docs/Spark_GPT.html)  
   
 ---
 # 介绍部分
 
 ## 功能特性
 
@@ -155,7 +153,8 @@
 
 #### 6.以下是webui管理命令列表,所有命令前需要加上前缀/才能触发
 
 | 命令      | 命令含义                                             | 命令可用用户       |
 | --------- | ---------------------------------------------------- | ------------------ |
 | 开启webui | 默认开启,打开webui,并返回webui开启的端口(管理员可用) | SparkGPT管理员可用 |
 | 关闭webui | 请在使用webui后关闭(管理员可用)                      | SparkGPT管理员可用 |
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 1.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 1.1.8 Summary:
 Spark-
 GPT,å°å¤ç§æ¥æºçgptæ¥å¥qq,TG,Kook,Discordåæ´å¤å¹³å°,æä¾webuiè¿è¡å®æ¶éç½®ç­æ´æ°,æçé«è¶,ä½¿ç¨ä¾¿æ·,ç®¡çå®å,åè½å¼ºå¤§
 Author: canxin121 Author-email: 1969730106@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Sydneygpt (==0.11.8) Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: bardapi (>=0.1.24,<0.2.0) Requires-Dist: bidict
@@ -18,20 +18,15 @@
 markdown
                 [https://socialify.git.ci/canxin121/Spark-GPT/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                          ****** Spark-GPTä»åº ******
                                    Spark-GPT
                             [pypi] [python] [pypi]
                                [onebot]_[github]
->
-æ³¨ææ¬æä»¶ä½¿ç¨äºä¸ä¸ªç¬¬ä¸æ¹ç¨åºè¿è¡æè½¬å¾ï¼æä»¥ä¸ç®¡ä½ æ¯å¦çænonebotï¼è¯·å¡å¿æ¥ç
-[(2).å®è£ wkhtmltopdfç¨ä»¥é«æçæè½¬å¾:](https://canxin121.github.io/
-docs/docs/Spark_GPT.html#_2-
-%E5%AE%89%E8%A3%85%E6%9C%AC%E6%8F%92%E4%BB%B6%E5%8F%8A%E4%BE%9D%E8%B5%96%E8%BD%AF%E4%BB%B6)
-## ææ°çæ¬å·1.1.7 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
+## ææ°çæ¬å·1.1.8 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
 (https://canxin121.github.io/docs/docs/Spark_GPT.html) --- # ä»ç»é¨å ##
 åè½ç¹æ§ - æ±èä¼å¤æ¥æºçgpt(poe
 (chatgpt+claude),chatgptç½é¡µç,Newbing,slack
 claude,è®¯é£æç«,éä¹åé®),æ¯æå¤å¹³å°(tg,kook( åå¼é»å¦),qq
 (gocq),discord)ä½¿ç¨ä¸ä¸åå¹³å°ç¨æ·æ°æ®ç»å®äºé -
 æ¯æäººæ ¼é¢è®¾ååç¼ç³»ç»,æ¯ææè½¬å¾æè½¬é¾æ¥,æ¯ææ¯ä¸ªç¨æ·åå»ºä¸åæ¥æºä¸åäººæ ¼çbot,åæ¶æ¯æå¬ç¨å±åçbot
 -
```

