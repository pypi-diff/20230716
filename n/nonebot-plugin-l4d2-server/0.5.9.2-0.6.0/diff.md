# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.9.2.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.9.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.6.0.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.9.2.tar` & `nonebot_plugin_l4d2_server-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0    35149 2023-07-12 15:48:48.898191 nonebot_plugin_l4d2_server-0.5.9.2/LICENSE
--rw-r--r--   0        0        0     5683 2023-07-12 15:48:48.898191 nonebot_plugin_l4d2_server-0.5.9.2/README.md
--rw-r--r--   0        0        0    18161 2023-07-12 15:48:48.902191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-07-12 15:48:48.902191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-07-12 15:48:48.902191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     9076 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1607 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1715 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3530 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3364 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1344 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4034 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1868 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1832 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     3074 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4211 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4174 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0      665 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9493 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1083 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     4018 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1421 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7216 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3854 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1040 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    11838 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4067 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1185 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9225 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6021 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1631 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0     1219 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2149 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     9329 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8469 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14982 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1606 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/pyproject.toml
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.9.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-16 09:49:04.006732 nonebot_plugin_l4d2_server-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5644 2023-07-16 09:49:04.006732 nonebot_plugin_l4d2_server-0.6.0/README.md
+-rw-r--r--   0        0        0    19094 2023-07-16 09:49:04.010732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-07-16 09:49:04.010732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-07-16 09:49:04.010732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     7067 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html
+-rw-r--r--   0        0        0     6135 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     9076 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1607 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     2054 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      369 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3574 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3363 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1344 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     3273 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1868 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1832 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     3074 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4211 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4174 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0      665 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9492 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1083 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     4019 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1421 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7593 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     1296 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1294 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py
+-rw-r--r--   0        0        0    12634 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     5211 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/utils.py
+-rw-r--r--   0        0        0     1587 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1337 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1551 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4067 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1185 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9345 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5979 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1631 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0     3220 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0     1219 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0      669 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     7725 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8521 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14963 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1695 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.6.0/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/LICENSE` & `nonebot_plugin_l4d2_server-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/README.md` & `nonebot_plugin_l4d2_server-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-# nonebot_plugin_l4d2_server 0.5
+# nonebot_plugin_l4d2_server 0.6
 
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
         <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
@@ -32,17 +32,15 @@
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
 ## 顶置公告
 
-0.5.0破坏式更新，不再使用env配置，采用web控制台管理
-
-同时不再支持远程查询，改为只允许本地查询
+0.6.0更新了适配器，初步实现了v11,v12,kook的适配，以及qq频道的部分适配
 
 文档暂时没时间更新ozr
 
 ## 安装
 
 以下方法任选其一：
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
- # nonebot_plugin_l4d2_server 0.5 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
+ # nonebot_plugin_l4d2_server 0.6 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## é¡¶ç½®å¬å
-0.5.0ç ´åå¼æ´æ°ï¼ä¸åä½¿ç¨envéç½®ï¼éç¨webæ§å¶å°ç®¡ç
-åæ¶ä¸åæ¯æè¿ç¨æ¥è¯¢ï¼æ¹ä¸ºåªåè®¸æ¬å°æ¥è¯¢
+0.6.0æ´æ°äºééå¨ï¼åæ­¥å®ç°äºv11,v12,kookçééï¼ä»¥åqqé¢éçé¨åéé
 ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr ## å®è£ ä»¥ä¸æ¹æ³ä»»éå¶ä¸ï¼ nb plugin
 install nonebot-plugin-l4d2-server pip install nonebot-plugin-l4d2-server pipx
 install nonebot-plugin-l4d2-server git clone https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server.git ## ä¸»è¦åè½ - æ±çæå¡å¨-
 æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 from nonebot import require
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 require("nonebot_plugin_txt2img")
+require("nonebot_plugin_saa")
 from .l4d2_web import web, webUI
 
 from typing import Tuple, Union, List
 from time import sleep
 import time
 
 from nonebot.matcher import Matcher
@@ -39,40 +40,42 @@
 from .l4d2_anne.server import updata_anne_server
 from .l4d2_data import sq_L4D2
 from .l4d2_push import *
 from .l4d2_image.vtfs import img_to_vtf
 from .l4d2_file import updown_l4d2_vpk, all_zip_to_one
 from .l4d2_file.input_json import *
 from .l4d2_utils.txt_to_img import mode_txt_to_img
+from .l4d2_queries.utils import queries_server
+from .l4d2_queries.qqgroup import add_ip,show_ip,del_ip,get_number_url
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 from nonebot.plugin import PluginMetadata
 
 driver = get_driver()
 
-__version__ = "0.5.9"
+__version__ = "0.6.0"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
-    description="群内对有关求生之路的查询和操作",
+    description="适配V11,v12,kook,qq频道的多平台nonebot2插件",
     usage="群内对有关求生之路的查询和操作",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
-    supported_adapters={"~onebot.v11"},
+    supported_adapters={"~onebot.v11", "~onebot.v12", "~qqguild", "~kaiheila"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 
 """相当于启动就检查数据库"""
 
 
 @up.handle()
-async def _(matcher: Matcher, event: NoticeEvent):
+async def _(matcher: Matcher, event: NoticeEvent_):
     args = event.dict()
     if args["notice_type"] != "offline_file":
         matcher.set_arg("txt", args)  # type: ignore
         return
     l4_file_path = l4_config.l4_ipall[l4_config.l4_number]["location"]
     map_path = Path(l4_file_path, vpk_path)  # type: ignore
     # 检查下载路径是否存在
@@ -153,19 +156,19 @@
     map_path = Path(l4_config.l4_ipall[l4_config.l4_number]["location"], vpk_path)
     name_vpk = get_vpk(map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
     msg = ""
     msg = mes_list(msg, name_vpk).replace(" ", "")
 
-    await matcher.finish(mode_txt_to_img(mes, msg))
+    await mode_txt_to_img(mes, msg).send()
 
 
 @del_vpk.handle()
-async def _(matcher: Matcher, args: Message = CommandArg()):
+async def _(matcher: Matcher, args: Message_ = CommandArg()):
     num1 = args.extract_plain_text()
     if num1:
         matcher.set_arg("num", args)
 
 
 @del_vpk.got("num", prompt="你要删除第几个序号的地图(阿拉伯数字)")
 async def _(matcher: Matcher, tag: str = ArgPlainText("num")):
@@ -190,15 +193,15 @@
         if map_name:
             await matcher.finish("改名成功\n原名:" + map_name + "\n新名称:" + rename)
     except ValueError:
         await matcher.finish("参数错误,请输入格式如【求生地图 5 改名 map.vpk】,或者输入【求生地图】获取全部名称")
 
 
 @anne_player.handle()
-async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
+async def _(matcher: Matcher, event: MessageEvent, args: Message_ = CommandArg()):
     name = args.extract_plain_text()
     name = name.strip()
     at = await get_message_at(event.json())
     usr_id = at_to_usrid(at)
     if not usr_id:
         usr_id = event.user_id
     # 没有参数则从db里找数据
@@ -206,15 +209,15 @@
     if isinstance(msg, str):
         await matcher.finish(msg)
     elif isinstance(msg, bytes):
         await matcher.finish(MessageSegment.image(msg))
 
 
 @anne_bind.handle()
-async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
+async def _(matcher: Matcher, event: MessageEvent, args: Message_ = CommandArg()):
     tag = args.extract_plain_text()
     tag = tag.strip()
     if tag == "" or tag.isspace():
         await matcher.finish("虚空绑定?")
     usr_id = str(event.user_id)
     nickname = event.sender.card or event.sender.nickname
     if not nickname:
@@ -226,32 +229,32 @@
 @del_bind.handle()
 async def _(matcher: Matcher, event: MessageEvent):
     usr_id = event.user_id
     await matcher.finish(name_exist(str(usr_id)))
 
 
 @rcon_to_server.handle()
-async def _(matcher: Matcher, args: Message = CommandArg()):
+async def _(matcher: Matcher, args: Message_ = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("command", args)
 
 
 @rcon_to_server.got("command", prompt="请输入向服务器发送的指令")
 async def _(matcher: Matcher, tag: str = ArgPlainText("command")):
     tag = tag.strip()
     msg = await command_server(tag)
     try:
-        await matcher.finish(mode_txt_to_img("服务器返回", msg))
+        await mode_txt_to_img("服务器返回", msg).send()
     except:
         await matcher.finish(msg, reply_message=True)
 
 
 @check_path.handle()
-async def _(matcher: Matcher, args: Message = CommandArg()):
+async def _(matcher: Matcher, args: Message_ = CommandArg()):
     msg = args.extract_plain_text()
     if msg.startswith("切换"):
         msg_number = int("".join(msg.replace("切换", " ").split()))
         if msg_number > len(l4_config.l4_ipall) or msg_number < 0:
             await matcher.send("没有这个序号的路径呐")
         else:
             l4_config.l4_number = msg_number - 1
@@ -279,26 +282,26 @@
         await matcher.finish()
     ip_list = split_maohao(one_msg)
     msg = await queries_server(ip_list)
     await str_to_picstr(msg, matcher, keyword)
 
 
 @add_queries.handle()
-async def _(matcher: Matcher, event: GroupMessageEvent, args: Message = CommandArg()):
+async def _(matcher: Matcher, event: GroupMessageEvent, args: Message_ = CommandArg()):
     msg = args.extract_plain_text()
     if len(msg) == 0:
         await matcher.finish("请在该指令后加入参数，例如【114.51.49.19:1810】")
     [host, port] = split_maohao(msg)
     group_id = event.group_id
     msg = await add_ip(group_id, host, port)
     await matcher.finish(msg)
 
 
 @del_queries.handle()
-async def _(event: GroupMessageEvent, matcher: Matcher, args: Message = CommandArg()):
+async def _(event: GroupMessageEvent, matcher: Matcher, args: Message_ = CommandArg()):
     msg = args.extract_plain_text()
     if not msg.isdigit():
         await matcher.finish("请输入正确的序号数字")
     group_id = event.group_id
     msg = await del_ip(group_id, msg)
     await matcher.finish(msg)
 
@@ -312,53 +315,54 @@
     if isinstance(msg, str):
         await matcher.finish(msg)
     else:
         await matcher.finish(MessageSegment.image(msg))
 
 
 @join_server.handle()
-async def _(args: Message = CommandArg()):
+async def _(args: Message_ = CommandArg()):
     msg = args.extract_plain_text()
     url = await get_number_url(msg)
     await join_server.finish(url)
 
 
 @up_workshop.handle()
-async def _(matcher: Matcher, args: Message = CommandArg()):
+async def _(matcher: Matcher, args: Message_ = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("ip", args)
 
 
 @up_workshop.got("ip", prompt="请输入创意工坊网址或者物品id")
 async def _(matcher: Matcher, state: T_State, tag: str = ArgPlainText("ip")):
+    # 这一部分注释类型有大问题，反正能跑就不改了
     msg = await workshop_msg(tag)
     if not msg:
         await matcher.finish("没有这个物品捏")
     elif isinstance(msg, dict):
         pic = await url_to_byte(msg["图片地址"])
         if not pic:
             return
-        message = ""
+        message:str = ''
         for item, value in msg.items():
-            if item in ["图片地址", "下载地址", "细节"]:
+            if item in ["图片地址", "下载地址", "细节"] or not isinstance(item,str):
                 continue
-            message += item + ":" + value + "\n"
+            message +=  item + ":" + value + "\n"
         state["dic"] = msg
-        await up_workshop.send(MessageSegment.image(pic) + Message(message))
+        await MessageFactory([Image(pic),Text(message)]).send()
     elif isinstance(msg, list):
         lenge = len(msg)
-        pic = await url_to_byte(msg[0]["图片地址"])
-        message = f"有{lenge}个文件\n"
+        pic = await url_to_byte(msg[0]["图片地址"]) # type: ignore
+        message:str = f"有{lenge}个文件\n"
         ones = []
         for one in msg:
             for item, value in one.items():
                 if item in ["图片地址", "下载地址", "细节"]:
                     continue
-                message += item + ":" + value + "\n"
+                message += f"{item}:{value}\n"
             ones.append(one)
         state["dic"] = ones
 
 
 @up_workshop.got("is_sure", prompt='如果需要上传，请发送 "yes"')
 async def _(matcher: Matcher, bot: Bot, event: GroupMessageEvent, state: T_State):
     is_sure = str(state["is_sure"])
@@ -383,25 +387,25 @@
                 await all_zip_to_one(data_file_list)
                 await upload_file(bot, event, data_file, file_name)
     else:
         await matcher.finish("已取消上传")
 
 
 @updata.handle()
-async def _(matcher: Matcher, args: Message = CommandArg()):
+async def _(matcher: Matcher, args: Message_ = CommandArg()):
     """更新"""
     anne_ip_dict = await updata_anne_server()
     if not anne_ip_dict:
         await matcher.finish("网络开小差了捏")
     server_number = len(anne_ip_dict["云"])
     await matcher.finish(f"更新成功\n一共更新了{server_number}个电信anne服ip")
 
 
 @vtf_make.handle()
-async def _(matcher: Matcher, state: T_State, args: Message = CommandArg()):
+async def _(matcher: Matcher, state: T_State, args: Message_ = CommandArg()):
     msg: str = args.extract_plain_text()
     if msg not in ["拉伸", "填充", "覆盖", ""]:
         await matcher.finish("错误的图片处理方式")
     if msg == "":
         msg = "拉伸"
     state["way"] = msg
     logger.info("方式", msg)
@@ -433,29 +437,44 @@
         "left4dead2/addons/sourcemod/plugins",
     )
     name_smx = get_vpk(smx_path, file_=".smx")
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下smx文件"
     msg = ""
     msg = mes_list(msg, name_smx).replace(" ", "")
-    await matcher.finish(mode_txt_to_img(mes, msg))
+    await mode_txt_to_img(mes, msg).send()
 
 
 # @search_api.handle()
-# async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
+# async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message_ = CommandArg()):
 #     msg:str = args.extract_plain_text()
 #     # if msg.startswith('代码'):
 #         # 建图代码返回三方图信息
 #     data = await seach_map(msg,l4_config.l4_master[0],l4_config.l4_key)
 #     # else:
 #     if type(data) == str:
 #         await matcher.finish(data)
 #     else:
 #         state['maps'] = data
 #         await matcher.send(await map_dict_to_str(data))
+@help_.handle()
+async def _(matcher:Matcher):
+    msg = [
+        "=====求生机器人帮助=====",
+        "1、电信服战绩查询【求生anne[id/steamid/@]】",
+        "2、电信服绑定【求生绑定[id/steamid]】",
+        "3、电信服状态查询【云xx】" "4、创意工坊下载【创意工坊下载[物品id/链接]】",
+        "5、指定ip查询【求生ip[ip]】(可以是域名)",
+        "6、求生喷漆制作【求生喷漆】",
+        "6、本地服务器操作(略，详情看项目地址)",
+    ]
+    messgae = ""
+    for i in msg:
+        messgae += i + "\n"
+    await matcher.finish(messgae)
 
 
 @search_api.got("is_sure", prompt='如果需要上传，请发送 "yes"')
 async def _(matcher: Matcher, bot: Bot, event: GroupMessageEvent, state: T_State):
     is_sure = str(state["is_sure"])
     if is_sure == "yes":
         data_dict: dict = state["maps"][0]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import httpx
 from bs4 import BeautifulSoup
 import json
 import asyncio
-from typing import Dict, List
+from typing import Dict, List, Set, Union, Tuple
 from pathlib import Path
 
+from nonebot.log import logger
 from ..l4d2_utils.config import CONFIG_PATH, anne_url, ANNE_IP, headers
 
-from ..l4d2_queries.ohter import ALL_HOST
+from ..l4d2_queries.localIP import ALL_HOST, Group_All_HOST
 
 # 储存anne服务器ip
 anne_url = "https://sb.trygek.com/"
 # ANNE_IP = {}
 headers = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
 }
@@ -52,13 +53,24 @@
     ANNE_IP.update(ip_dict)
     return ip_dict
 
 
 def server_key():
     """响应的服务器开头"""
     a = set()
-    try:
-        for tag1, value in ALL_HOST.items():
+    for tag1, value in ALL_HOST.items():
+        try:
             a.add(tag1)
-    except AttributeError:
-        a.add("希腊那我从来没有想过这个事情")
+        except AttributeError:
+            a.add("希腊那我从来没有想过这个事情")
+    return a
+
+
+def group_key():
+    """响应群组服务器开头"""
+    a = set()
+    for tag1, value in Group_All_HOST.items():
+        try:
+            a.add(tag1)
+        except AttributeError:
+            a.add("希腊那我从来没有想过这个事情")
     return a
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 
     def _check_data_validity(self) -> None:
         """
         检查数据库数据的合法性
         错误数据默认填充NULL或者False
         """
         c = self.conn.cursor()
+        columns = None
+        table = None
         for table in table_data:
             if table == "L4d2_players":
                 columns = L4d2_players_tag
             else:
                 columns = L4d2_server_tag
         if not columns:
             return
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Union, Tuple, Optional, List
 
 
 class L4D2Player:
     """数据库L4D2_Player表的操作"""
 
     def __init__(self):
-
         """连接数据库"""
         self.datasqlite_path = DATASQLITE
         self.conn = sqlite3.connect(self.datasqlite_path / "L4D2.db")
         self.c = self.conn.cursor()
 
     async def _add_player_nickname(self, qq, nickname):
         """绑定昵称"""
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     return img
 
 
 class CustomizeImage:
     def __init__(
         self, image: Union[str, Image.Image], based_w: int, based_h: int
     ) -> None:
-
         self.bg_img = self.get_image(image, based_w, based_h)
         self.bg_color = self.get_bg_color(self.bg_img, is_light=True)
         self.text_color = self.get_text_color(self.bg_color)
         self.highlight_color = self.get_highlight_color(self.bg_color)
         self.char_color = self.get_char_color(self.bg_color)
         self.bg_detail_color = self.get_bg_detail_color(self.bg_color)
         self.char_high_color = self.get_char_high_color(self.bg_color)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #         im2 = Image.open(io.BytesIO(headd)).resize((185, 185)).convert("RGBA")
 #         r, g, b, a2 = im2.split()
 #         # im.paste(im2,(20,20),mask=a2)
 #     except IndexError:
 #         pass
 #     return im
 
+
 # async def url_for_byte(url):
 #     """所有代理_url终将绳之以法"""
 #     if not l4_proxies:
 #         print("代理不存在")
 #         data = await url_to_byte(url)
 #     headers = {
 #         'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from pathlib import Path
 import re
 import a2s
-from typing import Dict, Union
+from typing import Dict, Union, Optional, Any
 
 try:
     import ujson as json
 except:
     import json
 
 from nonebot.log import logger
 from nonebot import get_driver, on_command, get_bot
 from nonebot import require
 from nonebot.permission import SUPERUSER
 from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, Message
+from nonebot.adapters.onebot.v11 import  MessageSegment
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
 )
-
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
+from ..l4d2_utils.rule import MessageFactory,Image,Text,GroupEvent_,Message_
 from ..l4d2_utils.command import get_ip_to_mes
-from ..l4d2_utils.utils import extract_last_digit, json_server_to_tag_dict, split_maohao
+from ..l4d2_utils.utils import extract_last_digit, split_maohao,get_group_id
+from ..l4d2_queries.utils import json_server_to_tag_dict, queries_dict
 from ..l4d2_utils.config import l4_config
-from ..l4d2_queries import queries_dict
 
 driver = get_driver()
 sch_json = Path("data/L4D2/scheduler.json")
 if not sch_json.exists():
     with sch_json.open("w") as f:
         json.dump({}, f, ensure_ascii=False)
 
@@ -45,38 +45,44 @@
     aliases={"求生定时删除"},
     priority=30,
     permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
 )
 
 
 @add_rss.handle()
-async def _(event: GroupMessageEvent, matcher: Matcher, args: Message = CommandArg()):
-    group_id = event.group_id
+async def _(event: GroupEvent_, matcher: Matcher, args: Message_ = CommandArg()):
+    group_id = get_group_id(event)
+    if not group_id:
+        return
     msg = args.extract_plain_text()
     command, message = await extract_last_digit(msg)
     push_msg = await get_ip_to_mes(msg=message, command=command)
     if not push_msg:
         return
     if push_msg in ["服务器无响应", None]:
         await matcher.finish("无响应的服务器，请检查")
     else:
         return_msg = await add_or_update_data(group_id, msg)
         if isinstance(push_msg, bytes):
-            await matcher.send(MessageSegment.image(push_msg))
+            await MessageFactory([Image(push_msg)]).send()
+        elif isinstance(push_msg, MessageFactory):
+            await push_msg.send()
         else:
             await matcher.send(push_msg)
         if return_msg == "add":
             await matcher.send(f"已添加群定时任务【{msg}】{l4_config.l4_push_times}次")
         elif return_msg in ["update", "change"]:
             await matcher.send(f"已更新群定时任务【{msg}】{l4_config.l4_push_times}次")
 
 
 @del_rss.handle()
-async def _(event: GroupMessageEvent, matcher: Matcher):
-    group_id = event.group_id
+async def _(event: GroupEvent_, matcher: Matcher):
+    group_id = get_group_id(event)
+    if not group_id:
+        return
     await add_or_update_data(group_id, "", ad_mode="del")
     await matcher.finish("已删除群定时任务")
 
 
 async def add_or_update_data(group_i: int, some_str: str = "", ad_mode: str = "add"):
     """添加或者删除定时任务
     mode == [new,update,del,change]
@@ -144,54 +150,56 @@
         with sch_json.open(encoding="utf-8") as f:
             scheduler_data: Dict[str, Dict[str, Union[int, str]]] = json.load(f)
 
             for key, value in scheduler_data.items():
                 try:
                     recipient_id = int(key)
                     count = value["times"]
-                    msg = value["msg"]
+                    msg = str(value["msg"])
+                    count = int(count)
 
                     if count > 0:
                         msg_read = await send_message(recipient_id, msg, value)
-                        print(msg_read)
-                        if msg_read:
+                        if msg_read and isinstance(msg_read, str):
                             scheduler_data[key]["ip_detail"] = msg_read
                         count -= 1
 
                     scheduler_data[key]["times"] = count
                 except TypeError:
                     continue
 
         with sch_json.open(mode="w", encoding="utf-8") as f:
             json.dump(scheduler_data, f, ensure_ascii=False)
 
 
 async def send_message(
-    recipient_id: int, msg: str, value: Dict[str, Union[int, str]] = None
+    recipient_id: int, msg: str, value: Optional[Dict[str, Union[int, str]]] = None
 ):
     # 执行发送消息的操作，参数可以根据需要进行传递和使用
     command, message = await extract_last_digit(msg)
     push_msg = await get_ip_to_mes(msg=message, command=command)
     if isinstance(push_msg, bytes):
         await get_bot().send_group_msg(
             group_id=recipient_id, message=MessageSegment.image(push_msg)
         )
     elif msg and isinstance(push_msg, str):
         # 单服务器
         message = await json_server_to_tag_dict(msg, command)
-        if len(message) == 0:
+        if len(message) == 0 or not value:
             # 关键词不匹配，忽略
             return
         try:
             old_msg = value.get("ip_detail", {})
+            if not isinstance(old_msg, dict):
+                return
             ip = str(message["ip"])
             host, port = split_maohao(ip)
-            msg: a2s.SourceInfo = await a2s.ainfo((host, port))
-            value["map_"] = msg.map_name
-            value["rank_players"] = f"{msg.player_count}/{msg.max_players}"
+            msg_: a2s.SourceInfo = await a2s.ainfo((host, port))
+            value["map_"] = msg_.map_name
+            value["rank_players"] = f"{msg_.player_count}/{msg_.max_players}"
             if (
                 old_msg["map_"] == value["map_"]
                 and old_msg["rank_players"] == value["rank_players"]
             ):
                 logger.info(f"{msg}{command}人数和地图未发生变化")
             else:
                 await get_bot().send_group_msg(group_id=recipient_id, message=push_msg)
@@ -201,13 +209,13 @@
         return value
 
 
 async def server_is_change():
     """检测服务器是否发生变化"""
 
 
-@driver.on_bot_connect
-async def _():
-    logger.success("已成功启动求生定时推送")
-    scheduler.add_job(
-        rss_ip, "interval", minutes=l4_config.l4_push_interval, id="rss_ip"
-    )
+# @driver.on_bot_connect
+# async def _():
+#     logger.success("已成功启动求生定时推送")
+#     scheduler.add_job(
+#         rss_ip, "interval", minutes=l4_config.l4_push_interval, id="rss_ip"
+#     )
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,31 +7,39 @@
 import os
 
 BOT_DIR = os.path.dirname(os.path.abspath(__file__))
 filename = "data/L4D2/l4d2.json"
 global_file = Path(Path(__file__).parent.parent, filename)
 
 
-def load_josn():
+def load_ip_json():
     # 本地模块
-    try:
-        LOCAL_HOST: dict = json.load(open(filename, "r", encoding="utf8"))
-    except IOError or FileNotFoundError:
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-        data = {}
-        with open(filename, "w") as f:
-            json.dump(data, f)
-        LOCAL_HOST: dict = {}
+    LOCAL_HOST: Dict[str, List[Dict[str, str]]] = {}
     try:
         # 获取所有json文件的路径
         json_files = Path("data/L4D2/l4d2").glob("*.json")
 
         # 将所有json文件中的字典对象合并为一个字典
         for file_path in json_files:
             with open(file_path, "r", encoding="utf-8") as f:
                 LOCAL_HOST.update(json.load(f))
     except:
         pass
     return LOCAL_HOST
 
 
-ALL_HOST: Dict[str, List[Dict[str, str]]] = load_josn()
+def load_group_json():
+    try:
+        GROUP_HOST: Dict[str, List[str]] = json.load(
+            open(filename, "r", encoding="utf8")
+        )
+    except IOError or FileNotFoundError:
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+        data: Dict[str, List[str]] = {"anne": ["云"]}
+        with open(filename, "w") as f:
+            json.dump(data, f)
+        GROUP_HOST: Dict[str, List[str]] = {}
+    return GROUP_HOST
+
+
+ALL_HOST: Dict[str, List[Dict[str, str]]] = load_ip_json()
+Group_All_HOST: Dict[str, List[str]] = load_group_json()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from ..l4d2_data.serverip import L4D2Server
 from ..l4d2_image import server_ip_pic
-from . import (
+from .utils import (
     queries,
     player_queries,
     queries_dict,
     player_queries_anne_dict,
     msg_ip_to_list,
-    server_rule_dict,
 )
 from nonebot.log import logger
 import random
 import asyncio
+from ..l4d2_utils.utils import split_maohao
 from ..l4d2_utils.message import PRISON, QUEREN, KAILAO
-from .ohter import ALL_HOST
-from typing import List, Dict, Any
+from .localIP import ALL_HOST
+from typing import List, Dict, Any, Tuple, Union
 
 try:
     import ujson as json
 except:
     import json
 si = L4D2Server()
 errors = (
@@ -64,28 +64,28 @@
         number, qqgroup, host, port = i
         msg2 = await player_queries(host, port)
         msg1 = await queries(host, port)
         messsage += "序号、" + str(number) + "\n" + msg1 + msg2 + "--------------------\n"
     return messsage
 
 
-async def qq_ip_querie(msg: list, igr: bool = True):
-    msg_list = []
+async def qq_ip_querie(msg: List[Tuple[str, str, int]], igr: bool = True):
+    msg_list: List[Dict[str, Any]] = []
     tasks = []  # 用来保存异步任务
     if msg != []:
         for i in msg:
             try:
                 number: str
                 host: str
                 port: int
                 qqgroup: str = ""  # 初始化为""
                 if len(i) == 3:
                     number, host, port = i
                 else:
-                    number, qqgroup, host, port = i
+                    number, qqgroup, host, port = i  # type: ignore
                 # 将异步任务添加到任务列表中
                 tasks.append(
                     asyncio.create_task(
                         process_message(
                             number,
                             host,
                             port,
@@ -96,28 +96,25 @@
                     )
                 )
             except ValueError:
                 continue  # 处理异常情况
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
-        msg_list.sort(key=lambda x: x["number"])
-        for i in msg_list:
-            print(i)
-            break
-        result = {"msg_list": msg_list}
+        # msg_list.sort(key=lambda x: x["number"])
+        send_list =  sorted(msg_list, key=lambda x: int(x["number"]))
+        result = {"msg_list": send_list}
 
     else:
-        result = {}
+        result: Dict[str, List[Dict[str, Any]]] = {}
     return result
 
 
 async def qq_ip_queries_pic(msg: list, igr=False):
     result = await qq_ip_querie(msg, igr)
-    print(result)
     if "msg_list" in result:
         pic = await server_ip_pic(result["msg_list"])
     else:
         pic = None
     return pic
 
 
@@ -249,44 +246,29 @@
         else:
             message = random.choice(QUEREN[4])
     if mode == 3:
         message = random.choice(KAILAO)
     message += "\n" + "名称：" + mse["name"] + "\n"
     message += "地图：" + mse["map_"] + "\n"
     message += f"玩家：{mse['players']} / {mse['max_players']}\n"
-    print(mse["Players"])
     try:
         message += await msg_ip_to_list(mse["Players"])
-    except (KeyError):
+    except KeyError:
         message += "服务器里，是空空的呢\n"
     return message
 
 
 async def get_server_ip(number):
     group, host, port = await si.query_number(number)
     try:
         return str(host) + ":" + str(port)
     except TypeError:
         return None
 
 
-def split_maohao(msg: str) -> List[str]:
-    """分割大小写冒号"""
-    if ":" in msg:
-        msgs: List[str] = msg.split(":")
-    elif "：" in msg:
-        msgs: List[str] = msg.split("：")
-    elif msg.replace(".", "").isdigit():
-        msgs: List[str] = [msg, "20715"]
-    else:
-        msgs = []
-    mse = [msgs[0], msgs[-1]]
-    return mse
-
-
 async def write_json(data_str: str):
     """
     添加数据或者删除数据
      - 【求生更新 添加 腐竹 ip 模式 序号】
      - 【求生更新 添加 腐竹 ip 模式】
      - 【求生更新 删除 腐竹 序号】
     """
@@ -340,7 +322,48 @@
                         if not value:
                             ALL_HOST.pop(key)
                         with open("data/L4D2/l4d2.json", "w", encoding="utf8") as f_new:
                             json.dump(ALL_HOST, f_new, ensure_ascii=False, indent=4)
                         return "删除成功喵"
                 return "序号不正确，请输入【求生更新 删除 腐竹 序号】"
         return "腐竹名不存在，请输入【求生更新 删除 腐竹 序号】"
+
+
+async def add_ip(group_id, host, port):
+    """先查找是否存在，如果不存在则创建"""
+    return await bind_group_ip(group_id, host, port)
+
+
+async def del_ip(group_id, number):
+    """删除群ip"""
+    return await del_group_ip(group_id, number)
+
+
+async def show_ip(group_id):
+    """先查找群ip，再根据群ip返回"""
+    data_list = await get_qqgroup_ip_msg(group_id)
+    logger.info(data_list)
+    if len(data_list) == 0:
+        return "本群没有订阅"
+    msg = await qq_ip_queries_pic(data_list)
+    return msg
+
+
+async def get_number_url(number):
+    ip = await get_server_ip(number)
+    if not ip:
+        return "该序号不存在"
+    url = f"connect {ip}"
+    return url
+
+
+async def server_rule_dict(ip: str, port: int):
+    port = int(port)
+    ip = str(ip)
+    msg_dict = {}
+    # message_dict = await l4d(ip,port)
+    try:
+        msg: dict = await a2s.arules((ip, port))  # type: ignore
+        msg_dict["tick"] = msg["l4d2_tickrate_enabler"] + "tick"
+    except:
+        msg_dict["tick"] = ""
+    return msg_dict
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import asyncio
-from rcon.source.proto import Packet,Type
-from rcon.source.async_rcon import communicate,close
+from rcon.source.proto import Packet, Type
+from rcon.source.async_rcon import communicate, close
+
 
 async def main(host):
-    host = '43.142.178.212'
+    host = "43.142.178.212"
     port = 40003
-    password = '1145149191810'
-    encoding = 'utf-8'
+    password = "1145149191810"
+    encoding = "utf-8"
 
     # Connect to RCON server
 
-
     # Main loop
     while True:
         # Read user input
-        command = input('> ')
+        command = input("> ")
         if not command:
             break
 
-   # 连接服务器
+    # 连接服务器
     reader, writer = await asyncio.open_connection(host, port)
     login = Packet.make_login(password, encoding=encoding)
     response = await communicate(reader, writer, login)
 
     # 等待 SERVERDATA_AUTH_RESPONSE 数据包
     while response.type != Type.SERVERDATA_AUTH_RESPONSE:
         response = await Packet.aread(reader)
@@ -30,33 +30,35 @@
     if response.id == -1:
         await close(writer)
         raise WrongPassword()
 
     # 循环接收用户输入并发送指令
     while True:
         try:
-            command = input('请输入指令：')
-            
+            command = input("请输入指令：")
+
         except EOFError:
             break
-        
-        if command=='停止':
+
+        if command == "停止":
             break
         # 发送指令
-        
-        command = f'say {command}'
+
+        command = f"say {command}"
         request = Packet.make_command(command, encoding=encoding)
         response = await communicate(reader, writer, request)
 
         # if response.id != request.id:
         #     raise SessionTimeout()
 
-        print(response.payload.decode(encoding, errors='ignore'))
+        print(response.payload.decode(encoding, errors="ignore"))
 
     # 断开连接
     await close(writer)
-    
+
+
 class WrongPassword(Exception):
     """Indicates a wrong password."""
-    
+
+
 class SessionTimeout(Exception):
-    """Indicates that the session timed out."""
+    """Indicates that the session timed out."""
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 from rcon.source import rcon
 import asyncio
 from pathlib import Path
-from ..l4d2_utils.config import l4_config,CHECK_FILE
-# from ..config import l4_rcon,l4_host,l4_port,l4_rcon
+from ..l4d2_utils.config import l4_config, CHECK_FILE
 
 
-async def rcon_server(PASSWORD:str,msg:str):
+async def rcon_server(PASSWORD: str, msg: str):
     # response = await rcon(command=msg, host=l4_host, port=l4_port, passwd=PASSWORD,encoding='utf-8')
     # return response
     try:
-        response = await asyncio.wait_for(rcon(command=msg, host=l4_config.l4_ipall[CHECK_FILE]['host'], port = l4_config.l4_ipall[CHECK_FILE]['port'], passwd=PASSWORD), timeout=30)
+        response = await asyncio.wait_for(
+            rcon(
+                command=msg,
+                host=l4_config.l4_ipall[CHECK_FILE]["host"],
+                port=l4_config.l4_ipall[CHECK_FILE]["port"],
+                passwd=PASSWORD,
+            ),
+            timeout=30,
+        )
         return response
     except asyncio.TimeoutError:
-        return '超时'
+        return "超时"
+
 
 async def read_server_cfg_rcon():
     """如果没有输入rcon，尝试自动获取"""
-    if not l4_config.l4_ipall[CHECK_FILE]['rcon']:
-        cfg_server = Path(l4_config.l4_ipall[CHECK_FILE]['location'],'left4dead2/cfg/server.cfg')
-        with open(cfg_server,'r')as cfg:
-            content:str = cfg.read()
-            lines = content.split('\n')
+    if not l4_config.l4_ipall[CHECK_FILE]["rcon"]:
+        cfg_server = Path(
+            l4_config.l4_ipall[CHECK_FILE]["location"], "left4dead2/cfg/server.cfg"
+        )
+        with open(cfg_server, "r") as cfg:
+            content: str = cfg.read()
+            lines = content.split("\n")
             for line in lines:
-                if line.startswith('rcon_password'):
-                    password = line.split(' ')[-1]
+                if line.startswith("rcon_password"):
+                    password = line.split(" ")[-1]
                     password = password.strip('"')
                     return password
-    return l4_config.l4_ipall[CHECK_FILE]['rcon']
+    return l4_config.l4_ipall[CHECK_FILE]["rcon"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,56 +3,39 @@
 from typing import Type, List, Tuple
 from time import sleep
 
 from nonebot import on_notice, on_command, on_regex, on_keyword
 from nonebot.params import CommandArg, RawCommand, CommandStart
 from nonebot.matcher import Matcher
 from nonebot.adapters.onebot.v11 import (
-    NoticeEvent,
-    MessageEvent,
-    Message,
-    MessageSegment,
-    GroupMessageEvent,
+    GroupMessageEvent
 )
 
-from ..l4d2_anne.server import server_key, ANNE_IP
+
+from ..l4d2_anne.server import server_key, ANNE_IP, group_key
+from ..l4d2_queries.localIP import ALL_HOST, Group_All_HOST
 from .config import *
-from ..l4d2_queries.qqgroup import split_maohao
+from ..l4d2_queries.qqgroup import split_maohao, get_tan_jian, qq_ip_queries_pic
+from ..l4d2_queries import get_group_ip_to_msg
+
+from ..l4d2_queries.utils import get_anne_server_ip, json_server_to_tag_dict
 
 # from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
 from .utils import *
 from .txt_to_img import mode_txt_to_img
 from ..l4d2_image.one import one_server_img
+from .rule import *
+
 
 help_ = on_command("l4_help", aliases={"求生帮助"}, priority=20, block=True)
 
 # 服务器
 # last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
 
 
-def wenjian(event: NoticeEvent):
-    args = event.dict()
-    try:
-        name: str = args["file"]["name"]
-        usr_id = str(args["user_id"])
-    except KeyError:
-        return False
-    if args["notice_type"] == "offline_file":
-        if l4_config.l4_master:
-            return name.endswith(file_format) and usr_id in l4_config.l4_master
-        else:
-            return name.endswith(file_format)
-    elif args["notice_type"] == "group_upload":
-        if l4_config.l4_master:
-            return usr_id in l4_config.l4_master and name.endswith(file_format)
-        else:
-            return False
-    return False
-
-
 up = on_notice(rule=wenjian)
 
 
 rename_vpk = on_regex(
     r"^求生地图\s*(\S+.*?)\s*(改|改名)?\s*(\S+.*?)\s*$",
     flags=re.S,
     block=True,
@@ -115,47 +98,28 @@
 # 下载内容
 up_workshop = on_command(
     "workshop", aliases={"创意工坊下载", "求生创意工坊"}, priority=20, block=True
 )
 vtf_make = on_command("vtf_make", aliases={"求生喷漆"}, priority=20, block=True)
 
 
-@help_.handle()
-async def _():
-    msg = [
-        "=====求生机器人帮助=====",
-        "1、电信服战绩查询【求生anne[id/steamid/@]】",
-        "2、电信服绑定【求生绑定[id/steamid]】",
-        "3、电信服状态查询【云xx】" "4、创意工坊下载【创意工坊下载[物品id/链接]】",
-        "5、指定ip查询【求生ip[ip]】(可以是域名)",
-        "6、求生喷漆制作【求生喷漆】",
-        "6、本地服务器操作(略，详情看项目地址)",
-    ]
-    messgae = ""
-    for i in msg:
-        messgae += i + "\n"
-    await help_.finish(messgae)
-
-
-def get_session_id(event: MessageEvent) -> str:
-    if isinstance(event, GroupMessageEvent):
-        return f"group_{event.group_id}"
-    else:
-        return f"private_{event.user_id}"
 
 
 matchers: Dict[str, List[Type[Matcher]]] = {}
 
 
 async def get_des_ip():
+    """初始化"""
     global ALL_HOST
     global ANNE_IP
     global matchers
+    global Group_All_HOST
 
     def count_ips(ip_dict: Dict[str, List[Dict[str, str]]]):
+        """输出加载ip"""
         global ANNE_IP
         for key, value in ip_dict.items():
             if key in ["error_", "success_"]:
                 ip_dict.pop(key)
                 break
             count = len(value)
             logger.info(f"已加载：{key} | {count}个")
@@ -164,19 +128,19 @@
         sleep(1)
 
     count_ips(ALL_HOST)
     ip_anne_list = []
     try:
         for one_tag in l4_config.l4_zl_tag:
             ips = ALL_HOST[one_tag]
-            ip_anne_list = []
+            ip_anne_list: List[Tuple[str, str, str]] = []
             for one_ip in ips:
                 host, port = split_maohao(one_ip["ip"])
                 ip_anne_list.append((one_ip["id"], host, port))
-    except KeyError:
+    except (KeyError, TypeError):
         pass
     await get_read_ip(ip_anne_list)
 
     @tan_jian.handle()
     async def _(matcher: Matcher, event: MessageEvent):
         msg = await get_tan_jian(ip_anne_list, 1)
         await str_to_picstr(push_msg=msg, matcher=matcher)
@@ -188,38 +152,56 @@
 
     @open_prison.handle()
     async def _(matcher: Matcher, event: MessageEvent):
         msg = await get_tan_jian(ip_anne_list, 3)
         await str_to_picstr(push_msg=msg, matcher=matcher)
 
 
-async def get_read_ip(ip_anne_list):
-    get_ip = on_command("anne", aliases=server_key(), priority=80, block=True)
+async def get_read_ip(ip_anne_list: List[Tuple[str, str, str]]):
+    get_ip = on_command("云", aliases=server_key(), priority=50, block=True)
 
     @get_ip.handle()
     async def _(
         matcher: Matcher,
+        event: Event_,
         start: str = CommandStart(),
         command: str = RawCommand(),
-        args: Message = CommandArg(),
+        args: Message_ = CommandArg(),
     ):
         if start:
             command = command.replace(start, "")
         if command == "anne":
             command = "云"
         msg: str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
-        if isinstance(push_msg, bytes):
-            await matcher.finish(MessageSegment.image(push_msg))
-        elif msg and isinstance(push_msg, list):
-            await matcher.finish(
-                MessageSegment.image(push_msg[0]) + Message(push_msg[-1])
-            )
+        if not push_msg:
+            return
+        if isinstance(push_msg,MessageFactory):
+            logger.info("构造")
+            try:
+                await push_msg.finish()
+            except Exception as E:
+                logger.warning(E)
+                return
+        elif isinstance(push_msg, bytes):
+            logger.info("直接发送图片")
+            send_msg = Image(push_msg)
+        elif msg and type(push_msg) == list:
+            logger.info("更加构造函数")
+            send_msg = MessageFactory([Image(push_msg[0]), Text(push_msg[-1])])
         elif msg and isinstance(push_msg, str):
-            await str_to_picstr(push_msg, matcher)
+            send_msg = MessageFactory(push_msg)
+        else:
+            logger.info("出错了")
+            return
+        logger.info(type(send_msg))
+        if not send_msg:
+            logger.warning("没有")
+        await send_msg.send()
+        await matcher.finish()
 
 
 async def get_ip_to_mes(msg: str, command: str = ""):
     if not msg:
         # 以图片输出全部当前
         igr = False
         # if command in gamemode_list:
@@ -249,26 +231,50 @@
         if len(message) == 0:
             # 关键词不匹配，忽略
             return
         ip = str(message["ip"])
         logger.info(ip)
 
         try:
-            #     if l4_config.l4_image:
-            #         host,port = split_maohao(ip)
-            #         msgs = await queries_dict(host,port)
-            #         msgs['Players'] += await player_queries_anne_dict(host,port)
-            #         imgs = await one_server_img()
-            # else:
             msgs = await get_anne_server_ip(ip)
             return msgs
         except (OSError, asyncio.exceptions.TimeoutError):
             return "服务器无响应"
 
 
+async def get_read_group_ip():
+    get_grou_ip = on_command("anne", aliases=group_key(), priority=80, block=True)
+
+    @get_grou_ip.handle()
+    async def _(
+        matcher: Matcher,
+        start: str = CommandStart(),
+        command: str = RawCommand(),
+        args: Message_ = CommandArg(),
+    ):
+        if start:
+            command = command.replace(start, "")
+        msg: str = args.extract_plain_text()
+        push_msg = await get_group_ip_to_msg(msg, command)
+        if isinstance(push_msg, bytes):
+            send_msg = MessageFactory(Image(push_msg))
+        elif msg and type(push_msg) == list:
+            send_msg = MessageFactory([Image(push_msg[0]), Text(push_msg[-1])])
+        elif msg and isinstance(push_msg, str):
+            await str_to_picstr(push_msg, matcher)
+
+
+# tests = on_command("测试1")     
+
+# @tests.handle()
+# async def _(event: Event,arg:Message=CommandArg()):
+#     logger.info(event)
+#     logger.info(arg.extract_plain_text())
+
+
 async def init():
     global matchers
     # print('启动辣')
     from ..l4d2_update import l4d_restart, l4d_update, get_update_log, driver
 
     await get_des_ip()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
     PRIVATE_FRIEND,
 )
 
-from ..l4d2_queries.ohter import ALL_HOST
 
 file_format = (".vpk", ".zip", ".7z", "rar")
 # 权限
 
 driver = get_driver()
 COMMAND_START = list(driver.config.command_start)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent
 from nonebot.log import logger
 from nonebot.matcher import Matcher
-import struct
 import httpx
 import os
 from pathlib import Path
-
 from typing import List, Dict, Union, Optional
-from .txt_to_img import txt_to_img
 from .config import *
 from ..l4d2_anne import write_player, del_player, anne_message
 from ..l4d2_server.rcon import read_server_cfg_rcon, rcon_server
-from ..l4d2_queries import queries, player_queries
-from ..l4d2_queries.qqgroup import *
 from ..l4d2_server.workshop import workshop_to_dict
 from ..l4d2_image.steam import url_to_byte
+from .rule import *
 from .txt_to_img import mode_txt_to_img
 import tempfile
-import random
+import json
 
 
 async def get_file(url: str, down_file: Path):
     """
     下载指定Url到指定位置
     """
     try:
@@ -75,19 +71,14 @@
     old_file = map_path / map_name
     new_file = map_path / rename
     os.rename(old_file, new_file)
     logger.info("改名成功")
     return map_name
 
 
-def text_to_png(msg: str) -> bytes:
-    """文字转png"""
-    return txt_to_img(msg)
-
-
 def solve(msg: str):
     """删除str最后一行"""
     lines = msg.splitlines()
     lines.pop()
     return "\n".join(lines)
 
 
@@ -125,59 +116,14 @@
     if not msg:
         msg = "你可能发送了一个无用指令，或者换图导致服务器无响应"
     elif msg.startswith("Unknown command"):
         msg = "无效指令：" + msg.replace("Unknown command", "").strip()
     return msg.strip().replace("\n", "")
 
 
-async def queries_server(msg: list) -> str:
-    """查询ip返回信息"""
-    ip = msg[0]
-    port = msg[1]
-    msgs = ""
-    try:
-        msgs = await queries(ip, port)
-        msgs += await player_queries(ip, port)
-    except (struct.error, TimeoutError):
-        pass
-    # except Exception:
-    # msgs = '有无法识别的用户名'
-    # return msgs
-    return msgs
-
-
-async def add_ip(group_id, host, port):
-    """先查找是否存在，如果不存在则创建"""
-    return await bind_group_ip(group_id, host, port)
-
-
-async def del_ip(group_id, number):
-    """删除群ip"""
-    return await del_group_ip(group_id, number)
-
-
-async def show_ip(group_id):
-    """先查找群ip，再根据群ip返回"""
-    data_list = await get_qqgroup_ip_msg(group_id)
-    logger.info(data_list)
-    if len(data_list) == 0:
-        return "本群没有订阅"
-    msg = await qq_ip_queries_pic(data_list)
-    return msg
-
-
-async def get_number_url(number):
-    "connect AGNES.DIGITAL.LINE.PM:40001"
-    ip = await get_server_ip(number)
-    if not ip:
-        return "该序号不存在"
-    url = f"connect {ip}"
-    return url
-
-
 async def workshop_msg(msg: str):
     """url变成id，拼接post请求"""
     if msg.startswith("https://steamcommunity.com/sharedfiles/filedetails/?id"):
         try:
             msg = msg.split("&")[0]
         except:
             pass
@@ -191,24 +137,14 @@
 
 async def save_file(file: bytes, path_name):
     """保存文件"""
     with open(path_name, "wb") as files:
         files.write(file)
 
 
-async def get_anne_server_ip(ip, ismsg: bool = False):
-    """输出查询ip和ping"""
-    host, port = split_maohao(ip)
-    data = await queries_server([host, port])
-    lines = data.splitlines()
-    msg = "\n".join(lines[1:])
-    msg += "\nconnect " + ip
-    return msg
-
-
 async def upload_file(bot: Bot, event: MessageEvent, file_data: bytes, filename: str):
     """上传临时文件"""
     if systems == "win" or "other":
         with tempfile.TemporaryDirectory() as temp_dir:
             with open(Path(temp_dir) / filename, "wb") as f:
                 f.write(file_data)
             if isinstance(event, GroupMessageEvent):
@@ -241,40 +177,14 @@
                     "upload_private_file",
                     user_id=event.user_id,
                     file=f.name,
                     name=filename,
                 )
 
 
-async def json_server_to_tag_dict(key: str, msg: str):
-    """
-    l4d2字典转tag的dict结果
-     - 1、先匹配腐竹
-     - 2、匹配数字（几服），没有参数则从结果里随机返回一个
-    """
-    data_dict = {}
-    msg = msg.replace(" ", "")
-    # 腐竹循环
-    for tag, value in ALL_HOST.items():
-        value: List[dict]
-        if tag == key:
-            data_dict.update({"server": tag})
-            if not msg:
-                # 腐竹
-                data_dict.update(random.choice(value))
-            elif msg.isdigit():
-                logger.info("腐竹 + 序号")
-                for server in value:
-                    if msg == str(server["id"]):
-                        data_dict.update(server)
-                        break
-
-    return data_dict
-
-
 sub_menus = []
 
 
 def register_menu_func(
     func: str,
     trigger_condition: str,
     brief_des: str,
@@ -314,15 +224,43 @@
     """判断图片输出还是正常输出"""
     if l4_config.l4_image:
         lines = push_msg.splitlines()
         first_str = lines[0]
         last_str = lines[-1]
         push_msg = "\n".join(lines[1:-1])
         if l4_config.l4_connect:
-            await matcher.send(mode_txt_to_img(first_str, push_msg) + last_str)
+            await mode_txt_to_img(first_str, push_msg,last_str).send()
         else:
-            await matcher.send(mode_txt_to_img(first_str, push_msg))
+            await mode_txt_to_img(first_str, push_msg).send()
     else:
         if l4_config.l4_connect or keyword == "connect":
             await matcher.send(push_msg)
         else:
             await matcher.send("\n".join(push_msg.splitlines()[1:-2]))
+
+
+def split_maohao(msg: str) -> List[str]:
+    """分割大小写冒号"""
+    if ":" in msg:
+        msgs: List[str] = msg.split(":")
+    elif "：" in msg:
+        msgs: List[str] = msg.split("：")
+    elif msg.replace(".", "").isdigit():
+        msgs: List[str] = [msg, "20715"]
+    else:
+        msgs = []
+    mse = [msgs[0], msgs[-1]]
+    return mse
+
+def get_group_id(event: GroupEvent_) -> Optional[int]:
+    if isinstance(event, (V11GroupMessageEvent, V12GroupMessageEvent)):
+        group_id = event.group_id
+    elif isinstance(event, kaiheilaChannelMessageEvent):
+        group_id = int(event.group_id)
+    elif isinstance(event, qqguidChannelEvent):
+        if event.id:
+            group_id = event.id
+        else:
+            group_id = None
+    else:
+        group_id =  None
+    return group_id
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 from typing import Optional, Union
 
 from fastapi import FastAPI
 from fastapi import Header, HTTPException, Depends
 from fastapi.responses import JSONResponse, HTMLResponse, RedirectResponse
 from jose import jwt
+from jose.exceptions import JWTError, ExpiredSignatureError
 from nonebot import get_bot, get_app
 
 from pathlib import Path
 
 from nonebot import get_driver, logger
 from ..l4d2_utils.config import *
 from ..l4d2_utils.utils import split_maohao
@@ -50,15 +51,15 @@
                 token, config_manager.config.web_secret_key, algorithms="HS256"
             )
             if (
                 not (username := payload.get("username"))
                 or username != config_manager.config.web_username
             ):
                 raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
-        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
+        except (JWTError, ExpiredSignatureError, AttributeError):
             raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
 
     return Depends(inner)
 
 
 COMMAND_START = driver.config.command_start.copy()
 if "" in COMMAND_START:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,14 @@
 
 query_table = TableCRUD(
     mode="table",
     title="",
     syncLocation=False,
     api="/l4d2/api/get_query_contexts",
     interval=60000,
-    footable=True,
     itemActions=[
         ActionType.Url(
             tooltip="加入游戏",
             icon="fa fa-gamepad",
             confirmText="加入steam://connect/" + "${ip}",
             url="steam://connect/" + "${ip}",
             # url= "http://"+'${ip}',
```

#### html2text {}

```diff
@@ -120,33 +120,33 @@
 content="è¿ç¨æå¡å¨çç»å½è´¦æ·å"), ), InputPassword
 ( label="è¿ç¨å¯ç ", name="password", value="${password}", visibleOn="$
 {place}", labelRemark=Remark(shape="circle",
 content="è¿ç¨æå¡å¨çç»å½å¯ç "), ), ], actions=[ Action
 (label="ä¿å­", level=LevelEnum.success, type="submit"), Action
 (label="éç½®", level=LevelEnum.warning, type="reset"), ], ) query_table =
 TableCRUD( mode="table", title="", syncLocation=False, api="/l4d2/api/
-get_query_contexts", interval=60000, footable=True, itemActions=
-[ ActionType.Url( tooltip="å å¥æ¸¸æ", icon="fa fa-gamepad",
-confirmText="å å¥steam://connect/" + "${ip}", url="steam://connect/" + "$
-{ip}", # url= "http://"+'${ip}', blank=True, ), ], columns=[ TableColumn
-(label="æä¸»", name="master", searchable=True), TableColumn(label="åç§°",
-name="name", searchable=True), TableColumn(label="å°å¾", name="map_",
-searchable=True), TableColumn(label="ç©å®¶", name="rank_players",
-searchable=True), TableColumn(label="å»¶è¿", name="ping", searchable=True),
-TableColumn(label="IP å°å", name="ip", searchable=True), ], ) server_page =
-PageSchema( url="/messages", icon="fa fa-comment",
-label="æ¬å°æå¡å¨ç®¡ç", schema=Page( title="æ¬å°æå¡å¨ç®¡ç",
-interval=120000, initApi="/l4d2/api/get_l4d2_messages", body=[ Alert
-( level=LevelEnum.info, className="white-space-pre-wrap", body=
-(f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n"
-f"Â· åè½ææªå®å"), ), server_control, server_ditail, ], ), ) query_page
-= PageSchema( url="/contexts", icon="fa fa-comments",
-label="è¿ç¨æå¡å¨æ¥è¯¢", schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢",
-body=[ Alert( level=LevelEnum.info, className="white-space-pre-wrap", body=
-( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
+get_query_contexts", interval=60000, itemActions=[ ActionType.Url
+( tooltip="å å¥æ¸¸æ", icon="fa fa-gamepad", confirmText="å å¥steam://
+connect/" + "${ip}", url="steam://connect/" + "${ip}", # url= "http://"+'$
+{ip}', blank=True, ), ], columns=[ TableColumn(label="æä¸»", name="master",
+searchable=True), TableColumn(label="åç§°", name="name", searchable=True),
+TableColumn(label="å°å¾", name="map_", searchable=True), TableColumn
+(label="ç©å®¶", name="rank_players", searchable=True), TableColumn
+(label="å»¶è¿", name="ping", searchable=True), TableColumn(label="IP å°å",
+name="ip", searchable=True), ], ) server_page = PageSchema( url="/messages",
+icon="fa fa-comment", label="æ¬å°æå¡å¨ç®¡ç", schema=Page
+( title="æ¬å°æå¡å¨ç®¡ç", interval=120000, initApi="/l4d2/api/
+get_l4d2_messages", body=[ Alert( level=LevelEnum.info, className="white-space-
+pre-wrap", body=(f"æ­¤æ°æ®åºè®°å½äº
+{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n" f"Â· åè½ææªå®å"),
+), server_control, server_ditail, ], ), ) query_page = PageSchema( url="/
+contexts", icon="fa fa-comments", label="è¿ç¨æå¡å¨æ¥è¯¢", schema=Page
+( title="è¿ç¨æå¡å¨æ¥è¯¢", body=[ Alert( level=LevelEnum.info,
+className="white-space-pre-wrap", body=( f"æ­¤æ°æ®åºè®°å½äº
+{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
 f"Â· åè½ææªå®å" ), ), query_table, ], ), ) database_page = PageSchema
 ( label="æ°æ®åº", icon="fa fa-database", children=[server_page, query_page]
 ) # type: ignore config_page = PageSchema( url="/configs", isDefaultPage=True,
 icon="fa fa-wrench", label="éç½®", schema=Page( title="éç½®", initApi="/
 l4d2/api/get_group_list", body=[global_config_form, group_select,
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/pyproject.toml` & `nonebot_plugin_l4d2_server-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.9.2"
+version = "0.6.0"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
@@ -18,40 +18,44 @@
     "Operating System :: OS Independent",
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 nonebot2 = "^2.0.0"
-nonebot-adapter-onebot = ">=2.1.5"
+nonebot-adapter-onebot = ">=2.2.1"
 nonebot-plugin-htmlrender = "^0.2.0.3"
 nonebot_plugin_txt2img = ">=0.3.0"
 nonebot_plugin_apscheduler = "^0.2.0"
+nonebot-plugin-send-anything-anywhere = "0.2.7"
 asyncio = ">=3.4.3"
 aiohttp = "^3.8.4"
 jinja2 = ">=3.0.0"
 srctools="^2.3.9"
+bs4 = "0.0.1"
 httpx = ">=0.22.0"
-beautifulsoup4 = ">=4.8.0"
 rcon = "^2.1.0"
 pillow = "^9.4.0"
 pyunpack = "^0.3.0"
 "ruamel.yaml" = "^0.17.21"
 rarfile = "^4.0"
 patool = "^1.12"
 python-a2s = "^1.3.0"
 amis-python = "^1.0.6"
-jieba = "^0.42.1"
 pandas = ">=1.5.2"
-python-jose = "^3.3.0"
+python-jose = ">=3.3.0"
 gitpython = ">=3.1.27"
 attrs = "^23.1.0"
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.1.0"
+pycln = "^2.1.2"
+
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
 priority = "default"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.2/PKG-INFO` & `nonebot_plugin_l4d2_server-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.9.2
+Version: 0.6.0
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: beautifulsoup4 (>=4.8.0)
+Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: gitpython (>=3.1.27)
 Requires-Dist: httpx (>=0.22.0)
-Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jinja2 (>=3.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (==0.2.7)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
 Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: patool (>=1.12,<2.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
-Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: python-jose (>=3.3.0)
 Requires-Dist: pyunpack (>=0.3.0,<0.4.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: rcon (>=2.1.0,<3.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: srctools (>=2.3.9,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 Description-Content-Type: text/markdown
@@ -47,15 +48,15 @@
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-# nonebot_plugin_l4d2_server 0.5
+# nonebot_plugin_l4d2_server 0.6
 
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
         <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
@@ -77,17 +78,15 @@
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
 ## 顶置公告
 
-0.5.0破坏式更新，不再使用env配置，采用web控制台管理
-
-同时不再支持远程查询，改为只允许本地查询
+0.6.0更新了适配器，初步实现了v11,v12,kook的适配，以及qq频道的部分适配
 
 文档暂时没时间更新ozr
 
 ## 安装
 
 以下方法任选其一：
```

#### html2text {}

```diff
@@ -1,43 +1,42 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.9.2
-Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.6.0 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
-Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+Z735803792@163.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: amis-python
-(>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-Dist: attrs
-(>=23.1.0,<24.0.0) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist:
-gitpython (>=3.1.27) Requires-Dist: httpx (>=0.22.0) Requires-Dist: jieba
-(>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-
-adapter-onebot (>=2.1.5) Requires-Dist: nonebot-plugin-htmlrender
-(>=0.2.0.3,<0.3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
-nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
-nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
-patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.4.0,<10.0.0) Requires-Dist:
-python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
+(>=3.8.4,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
+asyncio (>=3.4.3) Requires-Dist: attrs (>=23.1.0,<24.0.0) Requires-Dist: bs4
+(==0.0.1) Requires-Dist: gitpython (>=3.1.27) Requires-Dist: httpx (>=0.22.0)
+Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
+Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist:
+nonebot-plugin-send-anything-anywhere (==0.2.7) Requires-Dist: nonebot2
+(>=2.0.0,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2)
+Requires-Dist: patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0)
 Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
 (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
 Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server Description-
 Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
- # nonebot_plugin_l4d2_server 0.5 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
+ # nonebot_plugin_l4d2_server 0.6 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## é¡¶ç½®å¬å
-0.5.0ç ´åå¼æ´æ°ï¼ä¸åä½¿ç¨envéç½®ï¼éç¨webæ§å¶å°ç®¡ç
-åæ¶ä¸åæ¯æè¿ç¨æ¥è¯¢ï¼æ¹ä¸ºåªåè®¸æ¬å°æ¥è¯¢
+0.6.0æ´æ°äºééå¨ï¼åæ­¥å®ç°äºv11,v12,kookçééï¼ä»¥åqqé¢éçé¨åéé
 ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr ## å®è£ ä»¥ä¸æ¹æ³ä»»éå¶ä¸ï¼ nb plugin
 install nonebot-plugin-l4d2-server pip install nonebot-plugin-l4d2-server pipx
 install nonebot-plugin-l4d2-server git clone https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server.git ## ä¸»è¦åè½ - æ±çæå¡å¨-
 æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
```

