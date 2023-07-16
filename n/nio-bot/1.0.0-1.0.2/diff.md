# Comparing `tmp/nio-bot-1.0.0.tar.gz` & `tmp/nio-bot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nio-bot-1.0.0.tar", last modified: Wed Jul 12 12:39:54 2023, max compression
+gzip compressed data, was "nio-bot-1.0.2.tar", last modified: Sun Jul 16 14:34:50 2023, max compression
```

## Comparing `nio-bot-1.0.0.tar` & `nio-bot-1.0.2.tar`

### file list

```diff
@@ -1,69 +1,84 @@
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.627895 nio-bot-1.0.0/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/.github/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 nex       (1000) nex       (1000)      797 2023-06-29 20:01:59.000000 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 nex       (1000) nex       (1000)      609 2023-06-29 20:01:59.000000 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 nex       (1000) nex       (1000)     7062 2023-07-12 12:39:09.000000 nio-bot-1.0.0/.gitignore
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/.idea/
--rw-r--r--   0 nex       (1000) nex       (1000)      176 2023-06-08 18:22:57.000000 nio-bot-1.0.0/.idea/.gitignore
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/.idea/inspectionProfiles/
--rw-r--r--   0 nex       (1000) nex       (1000)     3647 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      174 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      185 2023-06-08 18:47:53.000000 nio-bot-1.0.0/.idea/markdown.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      337 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/misc.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      266 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/modules.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      426 2023-06-13 20:35:20.000000 nio-bot-1.0.0/.idea/nio-bot.iml
--rw-r--r--   0 nex       (1000) nex       (1000)      180 2023-06-12 20:15:29.000000 nio-bot-1.0.0/.idea/vcs.xml
--rw-r--r--   0 nex       (1000) nex       (1000)    35149 2023-06-12 20:12:46.000000 nio-bot-1.0.0/LICENSE
--rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-12 12:39:54.627895 nio-bot-1.0.0/PKG-INFO
--rw-r--r--   0 nex       (1000) nex       (1000)     7969 2023-06-29 12:18:06.000000 nio-bot-1.0.0/README.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/guides/
--rw-r--r--   0 nex       (1000) nex       (1000)    14023 2023-07-05 11:52:24.000000 nio-bot-1.0.0/docs/guides/getting-started.md
--rw-r--r--   0 nex       (1000) nex       (1000)     1412 2023-07-03 21:42:38.000000 nio-bot-1.0.0/docs/index.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/reference/
--rw-r--r--   0 nex       (1000) nex       (1000)       36 2023-07-04 10:54:58.000000 nio-bot-1.0.0/docs/reference/attachment.md
--rw-r--r--   0 nex       (1000) nex       (1000)       27 2023-07-11 19:15:48.000000 nio-bot-1.0.0/docs/reference/client.md
--rw-r--r--   0 nex       (1000) nex       (1000)      100 2023-07-03 19:05:59.000000 nio-bot-1.0.0/docs/reference/commands.md
--rw-r--r--   0 nex       (1000) nex       (1000)      708 2023-07-03 20:33:05.000000 nio-bot-1.0.0/docs/reference/context.md
--rw-r--r--   0 nex       (1000) nex       (1000)       35 2023-07-03 19:08:54.000000 nio-bot-1.0.0/docs/reference/exceptions.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/docs/reference/utils/
--rw-r--r--   0 nex       (1000) nex       (1000)      229 2023-07-04 20:00:25.000000 nio-bot-1.0.0/docs/reference/utils/federation.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2764 2023-07-03 21:01:45.000000 nio-bot-1.0.0/docs/reference/utils/help_command.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2236 2023-07-04 09:49:11.000000 nio-bot-1.0.0/docs/reference/utils/parsers.md
--rw-r--r--   0 nex       (1000) nex       (1000)      707 2023-07-04 19:56:41.000000 nio-bot-1.0.0/docs/reference/utils/string_view.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2346 2023-07-03 21:31:35.000000 nio-bot-1.0.0/docs/reference/utils/typing.md
--rw-r--r--   0 nex       (1000) nex       (1000)     1960 2023-07-04 10:48:38.000000 nio-bot-1.0.0/docs/reference/utils/unblock.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/examples/
--rw-r--r--   0 nex       (1000) nex       (1000)     1636 2023-06-13 20:43:23.000000 nio-bot-1.0.0/examples/access_token.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1605 2023-06-13 20:35:19.000000 nio-bot-1.0.0/examples/hello_world.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1210 2023-06-15 08:59:25.000000 nio-bot-1.0.0/examples/uploading.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1243 2023-07-04 21:28:18.000000 nio-bot-1.0.0/mkdocs.yml
--rw-r--r--   0 nex       (1000) nex       (1000)      781 2023-07-04 21:26:46.000000 nio-bot-1.0.0/pyproject.toml
--rw-r--r--   0 nex       (1000) nex       (1000)       91 2023-07-04 18:30:33.000000 nio-bot-1.0.0/requirements.txt
--rw-r--r--   0 nex       (1000) nex       (1000)       38 2023-07-12 12:39:54.627895 nio-bot-1.0.0/setup.cfg
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/src/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/src/nio_bot.egg-info/
--rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/PKG-INFO
--rw-r--r--   0 nex       (1000) nex       (1000)     1409 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/SOURCES.txt
--rw-r--r--   0 nex       (1000) nex       (1000)        1 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/dependency_links.txt
--rw-r--r--   0 nex       (1000) nex       (1000)       58 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/entry_points.txt
--rw-r--r--   0 nex       (1000) nex       (1000)      203 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/requires.txt
--rw-r--r--   0 nex       (1000) nex       (1000)        7 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/top_level.txt
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/src/niobot/
--rw-r--r--   0 nex       (1000) nex       (1000)      806 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/__init__.py
--rw-r--r--   0 nex       (1000) nex       (1000)    13336 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/__main__.py
--rw-r--r--   0 nex       (1000) nex       (1000)      160 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/niobot/__version__.py
--rw-r--r--   0 nex       (1000) nex       (1000)    31604 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/attachment.py
--rw-r--r--   0 nex       (1000) nex       (1000)    32431 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/client.py
--rw-r--r--   0 nex       (1000) nex       (1000)    12273 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/commands.py
--rw-r--r--   0 nex       (1000) nex       (1000)     5146 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/context.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3952 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/exceptions.py
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.627895 nio-bot-1.0.0/src/niobot/utils/
--rw-r--r--   0 nex       (1000) nex       (1000)      777 2023-07-03 20:38:45.000000 nio-bot-1.0.0/src/niobot/utils/__init__.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1531 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/utils/federation.py
--rw-r--r--   0 nex       (1000) nex       (1000)     5027 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/utils/help_command.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3535 2023-06-28 19:12:30.000000 nio-bot-1.0.0/src/niobot/utils/parsers.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3467 2023-07-04 19:58:56.000000 nio-bot-1.0.0/src/niobot/utils/string_view.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1553 2023-07-03 21:16:02.000000 nio-bot-1.0.0/src/niobot/utils/typing.py
--rw-r--r--   0 nex       (1000) nex       (1000)     2071 2023-07-04 10:53:34.000000 nio-bot-1.0.0/src/niobot/utils/unblocking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.352550 nio-bot-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/markdown.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/nio-bot.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-16 14:34:38.000000 nio-bot-1.0.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 14:34:38.000000 nio-bot-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-16 14:34:50.352550 nio-bot-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-16 14:34:38.000000 nio-bot-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/docs/assets/guides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/docs/assets/guides/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/file-send.avif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/assets/guides/text/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/text/example_ffprobe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/text/example_identify.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/guides/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/guides/sending-attachments.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/attachment.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/client.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/context.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/exceptions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/federation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/help_command.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/string_view.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/unblock.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-16 14:34:38.000000 nio-bot-1.0.2/examples/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-16 14:34:38.000000 nio-bot-1.0.2/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-16 14:34:38.000000 nio-bot-1.0.2/examples/uploading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-16 14:34:38.000000 nio-bot-1.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-16 14:34:38.000000 nio-bot-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 14:34:38.000000 nio-bot-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 14:34:50.352550 nio-bot-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/src/nio_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.352550 nio-bot-1.0.2/src/niobot/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/niobot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34066 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33431 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.352550 nio-bot-1.0.2/src/niobot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/string_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/unblocking.py
```

### Comparing `nio-bot-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `nio-bot-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `nio-bot-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/.gitignore` & `nio-bot-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/.idea/inspectionProfiles/Project_Default.xml` & `nio-bot-1.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/LICENSE` & `nio-bot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/PKG-INFO` & `nio-bot-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,80 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 1.0.0
+Version: 1.0.2
 Summary: Making matrix bots simple
 Author-email: Nexus <packages@nexy7574.co.uk>
 License: GNU GPLv3
+Project-URL: Source, https://github.com/eekim10/niobot
+Project-URL: Tracker, https://github.com/eekim10/niobot/issues
+Project-URL: Documentation, https://eekim10.github.io/niobot/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: e2ee
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
-<details>
-    <summary>Version information & warning</summary>
-This library does not currently have a "stable" version, as such all versions will be <code>0.1.dev&lt;Commit Number&gt;+g&lt;Commit Hash&gt;</code>.
-In order to pin to a specific version you should use the following in a requirements.txt or equivalent:
-    
-```
-matrix-nio @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-# or for e2ee
-matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-```
-
-Please remember, until there is a "stable" version, all commits will be pushed to main! Version pinning is highly
-recommended.
-</details>
-
 # NioBot
 A simple, easy to use python Matrix bot library, based on the excellent 
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-look at [examples](/examples), open an issue, or [contact me on matrix](https://matrix.to/#/@nex:nexy7574.co.uk)
-
-## Examples
-You can see the [examples](/examples) directory, which contains a few examples of how to use NioBot.
-Note that these examples are not tested and will need some tweaking.
+Take a look at the [docs!](https://eekim10.github.io/niobot)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
 (DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
 
 ## Installation
+### Versions
+NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
+`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
+however `Minor` and `Patch` versions are.
+
+This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
+`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
+always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
+
+Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
+`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
+which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
+This minimises the number of breaking releases.
+
+### Release versions
+You can use the [PyPi](https://pypi.org/project/niobot) releases:
+```python
+niobot==1.0.0  # or whatever version
+# Or to install it with extras
+niobot[e2ee,cli]==1.0.0
+```
+
+### Development (master branch)
 You should use requirements.txt:
 ```python
 matrix-nio @ git+https://github.com/EEKIM10/niobot.git
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
-You can figure out how to install it in other ways. See the start of this README for more information on version
-pinning.
+You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
 Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
 intended or how you'd expect, however as with any matrix client.
 
 However, like any good client, NioBot tries to adhere to the 
@@ -122,42 +128,42 @@
 |- main.py  (your bot file, the bit that runs your bot)
 |- modules
     |- ping.py
 ```
 
 In main.py, you'll put some similar code:
 ```python
-import niolib
+import niobot
 
-bot = niolib.Bot(...)
+bot = niobot.Bot(...)
 bot.mount_module("modules.ping")  # mounts the ping module
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
 2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
-import niolib
+import niobot
 
 
 class MyPingModule(niolib.Module):
     # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
     
     # Now we will define a command
-    @niolib.command()
+    @niobot.command()
     async def ping(self, ctx: niolib.Context):
         """Shows the latency"""
         roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
 Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
```

### Comparing `nio-bot-1.0.0/README.md` & `nio-bot-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-<details>
-    <summary>Version information & warning</summary>
-This library does not currently have a "stable" version, as such all versions will be <code>0.1.dev&lt;Commit Number&gt;+g&lt;Commit Hash&gt;</code>.
-In order to pin to a specific version you should use the following in a requirements.txt or equivalent:
-    
-```
-matrix-nio @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-# or for e2ee
-matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-```
-
-Please remember, until there is a "stable" version, all commits will be pushed to main! Version pinning is highly
-recommended.
-</details>
-
 # NioBot
 A simple, easy to use python Matrix bot library, based on the excellent 
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-look at [examples](/examples), open an issue, or [contact me on matrix](https://matrix.to/#/@nex:nexy7574.co.uk)
-
-## Examples
-You can see the [examples](/examples) directory, which contains a few examples of how to use NioBot.
-Note that these examples are not tested and will need some tweaking.
+Take a look at the [docs!](https://eekim10.github.io/niobot)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
 (DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
 
 ## Installation
+### Versions
+NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
+`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
+however `Minor` and `Patch` versions are.
+
+This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
+`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
+always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
+
+Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
+`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
+which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
+This minimises the number of breaking releases.
+
+### Release versions
+You can use the [PyPi](https://pypi.org/project/niobot) releases:
+```python
+niobot==1.0.0  # or whatever version
+# Or to install it with extras
+niobot[e2ee,cli]==1.0.0
+```
+
+### Development (master branch)
 You should use requirements.txt:
 ```python
 matrix-nio @ git+https://github.com/EEKIM10/niobot.git
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
-You can figure out how to install it in other ways. See the start of this README for more information on version
-pinning.
+You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
 Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
 intended or how you'd expect, however as with any matrix client.
 
 However, like any good client, NioBot tries to adhere to the 
@@ -109,42 +112,42 @@
 |- main.py  (your bot file, the bit that runs your bot)
 |- modules
     |- ping.py
 ```
 
 In main.py, you'll put some similar code:
 ```python
-import niolib
+import niobot
 
-bot = niolib.Bot(...)
+bot = niobot.Bot(...)
 bot.mount_module("modules.ping")  # mounts the ping module
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
 2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
-import niolib
+import niobot
 
 
 class MyPingModule(niolib.Module):
     # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
     
     # Now we will define a command
-    @niolib.command()
+    @niobot.command()
     async def ping(self, ctx: niolib.Context):
         """Shows the latency"""
         roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
 Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
```

### Comparing `nio-bot-1.0.0/docs/guides/getting-started.md` & `nio-bot-1.0.2/docs/guides/getting-started.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/index.md` & `nio-bot-1.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/context.md` & `nio-bot-1.0.2/docs/reference/context.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/help_command.md` & `nio-bot-1.0.2/docs/reference/utils/help_command.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/parsers.md` & `nio-bot-1.0.2/docs/reference/utils/parsers.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/string_view.md` & `nio-bot-1.0.2/docs/reference/utils/string_view.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/typing.md` & `nio-bot-1.0.2/docs/reference/utils/typing.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/unblock.md` & `nio-bot-1.0.2/docs/reference/utils/unblock.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/examples/access_token.py` & `nio-bot-1.0.2/examples/access_token.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/examples/hello_world.py` & `nio-bot-1.0.2/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/examples/uploading.py` & `nio-bot-1.0.2/examples/uploading.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/mkdocs.yml` & `nio-bot-1.0.2/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 site_name: Nio-Bot Docs
 theme:
   name: "material"
   palette:
     scheme: slate
+  features:
+    - content.tabs.link
 markdown_extensions:
   - admonition
   - def_list
   - attr_list
   - md_in_html
   - abbr
   - toc:
@@ -17,14 +19,17 @@
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
+  - pymdownx.superfences
+  - pymdownx.tabbed:
+      alternate_style: true
 repo_url: https://github.com/EEKIM10/niobot
 plugins:
   - search
   - autorefs
   - glightbox
   - mkdocstrings:
       handlers:
```

### Comparing `nio-bot-1.0.0/pyproject.toml` & `nio-bot-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 requires-python = ">=3.11"
 license = { text = "GNU GPLv3" }
 authors = [
     {name = "Nexus", email = "packages@nexy7574.co.uk"}
 ]
 dynamic = ["version", "dependencies"]
 
+[project.urls]
+Source = "https://github.com/eekim10/niobot"
+Tracker = "https://github.com/eekim10/niobot/issues"
+Documentation = "https://eekim10.github.io/niobot/"
+
+
 [project.optional-dependencies]
 e2ee = ['matrix-nio[e2e]']
 cli = ['httpx', 'click']
 dev = ['mkdocs', 'mkdocs-material', 'black', 'mkdocs-autorefs', 'mkdocs-glightbox']
 
 [project.scripts]
 niocli = "niobot.__main__:cli_root [cli]"
```

### Comparing `nio-bot-1.0.0/src/nio_bot.egg-info/PKG-INFO` & `nio-bot-1.0.2/src/nio_bot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,80 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 1.0.0
+Version: 1.0.2
 Summary: Making matrix bots simple
 Author-email: Nexus <packages@nexy7574.co.uk>
 License: GNU GPLv3
+Project-URL: Source, https://github.com/eekim10/niobot
+Project-URL: Tracker, https://github.com/eekim10/niobot/issues
+Project-URL: Documentation, https://eekim10.github.io/niobot/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: e2ee
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
-<details>
-    <summary>Version information & warning</summary>
-This library does not currently have a "stable" version, as such all versions will be <code>0.1.dev&lt;Commit Number&gt;+g&lt;Commit Hash&gt;</code>.
-In order to pin to a specific version you should use the following in a requirements.txt or equivalent:
-    
-```
-matrix-nio @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-# or for e2ee
-matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-```
-
-Please remember, until there is a "stable" version, all commits will be pushed to main! Version pinning is highly
-recommended.
-</details>
-
 # NioBot
 A simple, easy to use python Matrix bot library, based on the excellent 
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-look at [examples](/examples), open an issue, or [contact me on matrix](https://matrix.to/#/@nex:nexy7574.co.uk)
-
-## Examples
-You can see the [examples](/examples) directory, which contains a few examples of how to use NioBot.
-Note that these examples are not tested and will need some tweaking.
+Take a look at the [docs!](https://eekim10.github.io/niobot)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
 (DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
 
 ## Installation
+### Versions
+NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
+`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
+however `Minor` and `Patch` versions are.
+
+This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
+`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
+always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
+
+Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
+`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
+which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
+This minimises the number of breaking releases.
+
+### Release versions
+You can use the [PyPi](https://pypi.org/project/niobot) releases:
+```python
+niobot==1.0.0  # or whatever version
+# Or to install it with extras
+niobot[e2ee,cli]==1.0.0
+```
+
+### Development (master branch)
 You should use requirements.txt:
 ```python
 matrix-nio @ git+https://github.com/EEKIM10/niobot.git
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
-You can figure out how to install it in other ways. See the start of this README for more information on version
-pinning.
+You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
 Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
 intended or how you'd expect, however as with any matrix client.
 
 However, like any good client, NioBot tries to adhere to the 
@@ -122,42 +128,42 @@
 |- main.py  (your bot file, the bit that runs your bot)
 |- modules
     |- ping.py
 ```
 
 In main.py, you'll put some similar code:
 ```python
-import niolib
+import niobot
 
-bot = niolib.Bot(...)
+bot = niobot.Bot(...)
 bot.mount_module("modules.ping")  # mounts the ping module
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
 2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
-import niolib
+import niobot
 
 
 class MyPingModule(niolib.Module):
     # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
     
     # Now we will define a command
-    @niolib.command()
+    @niobot.command()
     async def ping(self, ctx: niolib.Context):
         """Shows the latency"""
         roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
 Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
```

### Comparing `nio-bot-1.0.0/src/niobot/__main__.py` & `nio-bot-1.0.2/src/niobot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         "version_info": __version__,
         "version_tuple": __version_tuple__
     }
 
 
 @cli_root.command()
 @click.option("--no-colour", "--no-color", "-C", is_flag=True, default=False)
+@click.option("--homeserver", "-H", default=None, help="An optional homeserver to display information about.")
 @click.pass_context
 def version(ctx, no_colour: bool):
     """Shows version information."""
     logger.info("Gathering version info...")
     import platform
     from nio.crypto import ENCRYPTION_ENABLED
 
@@ -123,15 +124,14 @@
     t = ctx.obj["version_tuple"]
     if len(t) > 3:
         t3 = t[3] or 'gN/A.d%s' % (datetime.datetime.now().strftime("%Y%m%d"))
         try:
             t3_commit, t3_date_raw = t3.split(".", 1)
         except ValueError:
             t3_commit = t3
-            logger.warning("Failed to parse commit date from %r, using current date instead.", t3)
             t3_date = datetime.datetime.now()
             t3_date_raw = t3_date.strftime("%Y%m%d")
         t3_date = datetime.datetime.strptime(t3_date_raw[1:], "%Y%m%d")
     else:
         t3_commit = "<release>"
         mtime = pathlib.Path(__file__).stat().st_mtime
         t3_date = datetime.datetime.fromtimestamp(mtime)
@@ -147,24 +147,41 @@
         ctx.obj["version_info"],
         bot_version_deep["version"],
         bot_version_deep["build"],
         bot_version_deep["commit"][1:],
         bot_version_deep["date"].strftime("%d/%m/%Y")
     )
 
+    _os = platform.platform()
+    if hasattr(platform, "freedesktop_os_release"):
+        try:
+            _os_info = platform.freedesktop_os_release()
+        except OSError:
+            pass
+        else:
+            _os += " ({0}/{1} - {2})".format(
+                _os_info.get("NAME", "Unknown"),
+                _os_info.get("VERSION", "Unknown"),
+                _os_info.get("PRETTY_NAME", "Unknown")
+            )
+
     lines = [
         ["NioBot version", bot_version, lambda x: True],
         ["matrix-nio version", nio_version, lambda x: x.startswith("0.20")],
         ["Python version", platform.python_version(), lambda x: x.split(".")[0] == "3" and int(x.split(".")[1]) >= 9],
         ["Python implementation", platform.python_implementation(), lambda x: x == "CPython"],
-        ["Operating System", platform.platform(), lambda val: val.startswith(("Windows", "Linux"))],
+        ["Operating System", _os, lambda val: val.startswith(("Windows", "Linux"))],
         ["Architecture", platform.machine(), lambda x: x == "x86_64"],
         ["OLM Installed", "Yes" if ENCRYPTION_ENABLED else "No", lambda x: x != "No"],
     ]
 
+    _docker_path = pathlib.Path("/.dockerenv")
+    if _docker_path.is_file():
+        lines.append(["Running in Docker", "Probably (/.dockerenv exists)", lambda _: True])
+
     click.echo()
     for line in lines:
         if no_colour:
             click.echo("%s: %s" % tuple(line)[:2])
         else:
             click.echo(
                 click.style(line[0], fg="cyan") + ": " +
```

### Comparing `nio-bot-1.0.0/src/niobot/attachment.py` & `nio-bot-1.0.2/src/niobot/attachment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """
 Matrix file attachments. Full e2ee support is implemented.
-
-!!! danger "You need FFMPEG for this to work"
-    In order for most attachment-related operations, you must have `ffprobe` in your $PATH.
-    As a matter of fact,
 """
 import abc
 import tempfile
 import warnings
 
 import nio
 import subprocess
@@ -25,29 +21,22 @@
 
 from .utils import run_blocking
 from .exceptions import MediaUploadException, MetadataDetectionException, MediaCodecWarning
 
 if typing.TYPE_CHECKING:
     from .client import NioBot
 
-if not shutil.which("ffmpeg"):
-    raise RuntimeError(
-        "ffmpeg is not installed. You must install it to use this library. If its installed, is it in PATH?"
-    )
-if not shutil.which("ffprobe"):
-    raise RuntimeError(
-        "ffprobe is not installed. You must install it to use this library. If its installed, is it in PATH?"
-    )
-
 
 log = logging.getLogger(__name__)
 
 
 __all__ = (
     "detect_mime_type",
+    "get_metadata_ffmpeg",
+    "get_metadata_imagemagick",
     "get_metadata",
     "generate_blur_hash",
     "first_frame",
     "BaseAttachment",
     "FileAttachment",
     "ImageAttachment",
     "VideoAttachment",
@@ -108,46 +97,25 @@
         return mt
     elif isinstance(file, pathlib.Path):
         return magic.from_file(str(file), mime=True)
     else:
         raise TypeError("File must be a string, BytesIO, or Path object.")
 
 
-def get_metadata(file: typing.Union[str, pathlib.Path]) -> typing.Dict[str, typing.Any]:
+def get_metadata_ffmpeg(file: typing.Union[str, pathlib.Path]) -> typing.Dict[str, typing.Any]:
     """
     Gets metadata for a file via ffprobe.
 
-    ??? note "Example result"
-        ```json
-        {
-            "streams": [
-                {
-                    "index": 0,
-                    "codec_name": "h264",
-                    "codec_long_name": "H.264 / AVC / MPEG-4 AVC / MPEG-4 part 10",
-                    "profile": "High",
-                    "codec_type": "video",
-                    None
-                }
-            ],
-            "format": {
-                "filename": "./assets/peek.mp4",
-                "format_long_name": "QuickTime / MOV",
-                "start_time": "0.000000",
-                "duration": "16.283333",
-                "size": "4380760",
-                "bit_rate": "2152266",
-                None
-            }
-        }
-        ```
+    [example output (JSON)](https://github.com/EEKIM10/niobot/raw/master/docs/assets/guides/text/example_ffprobe.json)
 
     :param file: The file to get metadata for. **Must be a path-like object**
     :return: A dictionary containing the metadata.
     """
+    if not shutil.which("ffprobe"):
+        raise FileNotFoundError("ffprobe is not installed. If it is, check your $PATH.")
     command = [
         "ffprobe",
         "-of",
         "json",
         "-loglevel",
         "9",
         "-show_format",
@@ -156,15 +124,91 @@
         str(file)
     ]
     try:
         result = subprocess.run(command, capture_output=True, encoding="utf-8", errors="replace", check=True)
     except subprocess.SubprocessError as e:
         raise MetadataDetectionException("Failed to get metadata for file.", exception=e)
     log.debug("ffprobe output (%d): %s", result.returncode, result.stdout)
-    return json.loads(result.stdout or '{}')
+    data = json.loads(result.stdout or '{}')
+    log.debug("parsed ffprobe output:\n%s", json.dumps(data, indent=4))
+    return data
+
+
+def get_metadata_imagemagick(file: pathlib.Path) -> typing.Dict[str, typing.Any]:
+    """The same as `get_metadata_ffmpeg` but for ImageMagick.
+
+    Only returns a limited subset of the data, such as one stream, which contains the format, and size,
+    and the format, which contains the filename, format, and size.
+
+    [example output (JSON)](https://github.com/EEKIM10/niobot/raw/master/docs/assets/guides/text/example_identify.json)
+
+    :param file: The file to get metadata for. **Must be a path object**
+    :return: A slimmed-down dictionary containing the metadata.
+    """
+    file = file.resolve(True)
+    command = [
+        "identify",
+        str(file)
+    ]
+    try:
+        result = subprocess.run(command, capture_output=True, encoding="utf-8", errors="replace", check=True)
+    except subprocess.SubprocessError as e:
+        raise MetadataDetectionException("Failed to get metadata for file.", exception=e)
+    log.debug("identify output (%d): %s", result.returncode, result.stdout)
+    stdout = result.stdout
+    stdout = stdout[len(str(file)) + 1:]
+    img_format, img_size, *_ = stdout.split()
+    data = {
+        "streams": [
+            {
+                "index": 0,
+                "codec_name": img_format,
+                "codec_long_name": img_format,
+                "codec_type": "video",
+                "height": int(img_size.split("x")[1]),
+                "width": int(img_size.split("x")[0]),
+            }
+        ],
+        "format": {
+            "filename": str(file),
+            "format_long_name": img_format,
+            "size": str(file.stat().st_size),
+        }
+    }
+    log.debug("Parsed identify output:\n%s", json.dumps(data, indent=4))
+    return data
+
+
+def get_metadata(file: typing.Union[str, pathlib.Path], mime_type: str = None) -> typing.Dict[str, typing.Any]:
+    """
+    Gets metadata for a file.
+
+    This will use imagemagick (`identify`) for images where available, falling back to ffmpeg (`ffprobe`)
+    for everything else.
+
+    :param file: The file to get metadata for.
+    :param mime_type: The mime type of the file. If not provided, it will be detected.
+    :return: The metadata for the file. See [niobot.get_metadata_ffmpeg][] and [niobot.get_metadata_imagemagick][]
+     for more information.
+    """
+    file = _to_path(file)
+    mime = mime_type or detect_mime_type(file)
+    mime = mime.split("/")[0]
+    if mime == "image":
+        if not shutil.which("identify"):
+            log.warning(
+                "Imagemagick identify not found, falling back to ffmpeg for image metadata detection. "
+                "Check your $PATH."
+            )
+        else:
+            return get_metadata_imagemagick(file)
+
+    if mime not in ["audio", "video", "image"]:
+        raise MetadataDetectionException("Unsupported mime type. Must be an audio clip, video, or image.")
+    return get_metadata_ffmpeg(file)
 
 
 def first_frame(file: str | pathlib.Path, file_format: str = "webp") -> bytes:
     """
     Gets the first frame of a video file.
 
     !!! Danger "This function creates a file on disk"
@@ -175,24 +219,28 @@
 
         This also means that this function may be slow.
 
     :param file: The file to get the first frame of. **Must be a path-like object**
     :param file_format: The format to save the frame as. Defaults to webp.
     :return: The first frame of the video in bytes.
     """
+    if not shutil.which("ffmpeg"):
+        raise FileNotFoundError("ffmpeg is not installed. If it is, check your $PATH.")
     with tempfile.NamedTemporaryFile(suffix=f".{file_format}") as f:
         command = [
             "ffmpeg",
             "-loglevel",
             "9",
             "-i",
             str(file),
             "-frames:v",
             "1",
             '-y',
+            '-strict',
+            '-2',
             f.name
         ]
         log.debug("Extracting first frame of %r: %s", file, ' '.join(command))
         try:
             log.debug(
                 "Extraction return code: %d",
                 subprocess.run(command, capture_output=True, check=True).returncode
@@ -329,19 +377,19 @@
             file_name: str = None,
             mime_type: str = None,
             size_bytes: int = None,
             *,
             attachment_type: AttachmentType = AttachmentType.FILE
     ):
         self.file = _to_path(file)
-        self.file_name = file.name if isinstance(file, pathlib.Path) else file_name
-        if not file_name:
+        self.file_name = self.file.name if isinstance(self.file, pathlib.Path) else file_name
+        if not self.file_name:
             raise ValueError("file_name must be specified when uploading a BytesIO object.")
-        self.mime_type = mime_type or detect_mime_type(file)
-        self.size = size_bytes or os.path.getsize(file)
+        self.mime_type = mime_type or detect_mime_type(self.file)
+        self.size = size_bytes or os.path.getsize(self.file)
 
         self.type = attachment_type
         self.url = None
         self.keys = None
 
     def __repr__(self):
         return "<{0.__class__.__name__} file={0.file!r} file_name={0.file_name!r} " \
@@ -647,19 +695,21 @@
         else:
             if not file_name:
                 file_name = file.name
 
             if height is None or width is None:
                 metadata = await run_blocking(get_metadata, file)
                 for stream in metadata["streams"]:
+                    log.debug("Found stream in image:\n%s", stream)
                     if stream["codec_type"] == "video":
-                        if stream["codec_name"] not in SUPPORTED_IMAGE_CODECS and unsafe is False:
-                            continue
-                        else:
-                            break
+                        if stream["codec_name"].lower() not in SUPPORTED_IMAGE_CODECS and unsafe is False:
+                            warning = MediaCodecWarning(stream["codec_name"], *SUPPORTED_IMAGE_CODECS)
+                            warnings.warn(warning)
+                        log.debug("Selecting stream %r for image", stream)
+                        break
                 else:
                     raise ValueError("Unable to find an image stream in the given file. Are you sure its an image?")
                 # ffmpeg doesn't have an image type
                 height = stream["height"]
                 width = stream["width"]
 
         mime_type = await run_blocking(detect_mime_type, file)
@@ -763,15 +813,15 @@
             if not file_name:
                 file_name = file.name
 
             if height is None or width is None or duration is None:
                 metadata = await run_blocking(get_metadata, file)
                 for stream in metadata["streams"]:
                     if stream["codec_type"] == "video":
-                        if stream["codec_name"] not in SUPPORTED_VIDEO_CODECS \
+                        if stream["codec_name"].lower() not in SUPPORTED_VIDEO_CODECS \
                                 or not stream["codec_name"].startswith("pcm_"):  # usually, pcm is supported.
                             warning = MediaCodecWarning(stream["codec_name"], *SUPPORTED_VIDEO_CODECS)
                             warnings.warn(warning)
                         height = stream["height"]
                         width = stream["width"]
                         duration = round(float(metadata["format"]["duration"]) * 1000)
                         break
```

### Comparing `nio-bot-1.0.0/src/niobot/client.py` & `nio-bot-1.0.2/src/niobot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,33 +213,50 @@
 
         if self.case_insensitive:
             content = event.body.lower()
         else:
             content = event.body
 
         if content.startswith(self.command_prefix):
-            command = original_command = content[len(self.command_prefix):].splitlines()[0].split(" ")[0]
+            try:
+                command = original_command = content[len(self.command_prefix):].splitlines()[0].split(" ")[0]
+            except IndexError:
+                self.log.info(
+                    "Failed to parse message %r - message terminated early (was the content *just* the prefix?)",
+                    event.body
+                )
+                return
             command = self.get_command(command)
             if command:
                 if command.disabled is True:
                     raise CommandDisabledError(command)
                 context = command.construct_context(self, room, event, self.command_prefix + original_command)
                 self.dispatch("command", context)
+
+                def _task_callback(t: asyncio.Task):
+                    try:
+                        exc = t.exception()
+                    except asyncio.CancelledError:
+                        self.dispatch('command_cancelled', context, t)
+                    else:
+                        if exc:
+                            self.dispatch('command_error', context, CommandError(exception=exc))
+                        else:
+                            self.dispatch('command_complete', context, t)
                 self.log.debug(f"Running command {command.name} with context {context!r}")
                 try:
                     task = asyncio.create_task(command.invoke(context))
+                    context._task = task
                 except CommandArgumentsError as e:
                     self.dispatch("command_error", context, e)
                 except Exception as e:
                     self.log.exception("Failed to invoke command %s", command.name)
                     self.dispatch("command_error", context, CommandError(exception=e))
                 else:
-                    task.add_done_callback(
-                        lambda _res: self.dispatch("command_complete", context, _res)
-                    )
+                    task.add_done_callback(_task_callback)
             else:
                 self.log.debug(f"Command {original_command!r} not found.")
 
     def is_owner(self, user_id: str) -> bool:
         """
         Checks whether a user is the owner of the bot.
 
@@ -530,49 +547,53 @@
 
     async def send_message(
             self,
             room: nio.MatrixRoom | str,
             content: str = None,
             file: BaseAttachment = None,
             reply_to: nio.RoomMessageText | str = None,
-            message_type: str = None
+            message_type: str = None,
+            clean_mentions: bool = False
     ) -> nio.RoomSendResponse:
         """
         Sends a message.
 
         :param room: The room to send this message to
         :param content: The content to send. Cannot be used with file.
         :param file: A file to send, if any. Cannot be used with content.
         :param reply_to: A message to reply to.
         :param message_type: The message type to send. If none, defaults to NioBot.global_message_type,
         which itself is `m.notice` by default.
+        :param clean_mentions: Whether to escape all mentions
         :return: The response from the server.
         :raises MessageException: If the message fails to send, or if the file fails to upload.
         :raises ValueError: You specified neither file nor content.
         """
         if file and BaseAttachment is None:
             raise ValueError("You are missing required libraries to use attachments.")
         if not any((content, file)):
             raise ValueError("You must specify either content or file.")
 
         body = {
             "msgtype": message_type or self.global_message_type,
-            "body": content,
         }
 
         if file is not None:
             # We need to upload the file first.
             responses = await self._recursively_upload_attachments(file, encrypted=getattr(file, "encrypted", False))
             if any((isinstance(response, nio.UploadError) for response in responses)):
                 raise MessageException(
                     "Failed to upload media.", tuple(filter(lambda x: isinstance(x, nio.UploadError), responses))[0]
                 )
 
             body = file.as_body(content)
         else:
+            if clean_mentions:
+                content = content.replace("@", "@\u200b")
+            body['body'] = content
             if self.automatic_markdown_renderer:
                 parsed = await run_blocking(marko.parse, content)
                 if parsed.children:
                     rendered = await run_blocking(marko.render, parsed)
                     body["formatted_body"] = rendered
                     body["format"] = "org.matrix.custom.html"
 
@@ -602,27 +623,31 @@
     async def edit_message(
             self,
             room: nio.MatrixRoom | str,
             message: nio.Event | str,
             content: str,
             *,
             message_type: str = None,
+            clean_mentions: bool = False
     ) -> nio.RoomSendResponse:
         """
         Edit an existing message. You must be the sender of the message.
 
         You also cannot edit messages that are attachments.
 
         :param room: The room the message is in.
         :param message: The message to edit.
         :param content: The new content of the message.
         :param message_type: The new type of the message (i.e. m.text, m.notice. Defaults to client.global_message_type)
+        :param clean_mentions: Whether to escape all mentions
         :raises RuntimeError: If you are not the sender of the message.
         :raises TypeError: If the message is not text.
         """
+        if clean_mentions:
+            content = content.replace("@", "@\u200b")
         event_id = self._get_id(message)
         message_type = message_type or self.global_message_type
         content = {
             "msgtype": message_type,
             "body": content,
             "format": "org.matrix.custom.html",
             "formatted_body": await self._markdown_to_html(content),
@@ -634,16 +659,14 @@
             "m.new_content": {
                 **content
             },
             "m.relates_to": {
                 "rel_type": "m.replace",
                 "event_id": event_id,
             },
-            "format": "org.matrix.custom.html",
-            "formatted_body": content["formatted_body"]
         }
         async with Typing(self, room.room_id):
             response = await self.room_send(
                 self._get_id(room),
                 "m.room.message",
                 body,
             )
```

### Comparing `nio-bot-1.0.0/src/niobot/commands.py` & `nio-bot-1.0.2/src/niobot/commands.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/context.py` & `nio-bot-1.0.2/src/niobot/context.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/exceptions.py` & `nio-bot-1.0.2/src/niobot/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,30 +31,30 @@
     :var message: A simple humanised explanation of the issue, if available.
     :var response: The response object from the server, if available.
     :var exception: The exception that was raised, if available.
     :var original: The original response, or exception if response was not available.
     """
     message: str | None
     response: nio.ErrorResponse | None
-    exception: Exception | None
-    original: nio.ErrorResponse | Exception | None
+    exception: BaseException | None
+    original: nio.ErrorResponse | BaseException | None
 
     def __init__(
             self,
             message: str = None,
             response: nio.ErrorResponse = None,
             *,
-            exception: Exception = None,
-            original: typing.Union[nio.ErrorResponse, Exception] = None,
+            exception: BaseException = None,
+            original: typing.Union[nio.ErrorResponse, BaseException] = None,
     ):
         if original:
             warnings.warn(DeprecationWarning("original is deprecated, use response or exception instead"))
         self.original = original or response or exception
         self.response = response
-        self.exception: typing.Union[nio.ErrorResponse, Exception] = exception
+        self.exception: typing.Union[nio.ErrorResponse, BaseException] = exception
         self.message = message
 
         if self.original is None and self.message is None:
             raise ValueError("If there is no error history, at least a human readable message should be provided.")
 
     def __str__(self) -> str:
         """Returns a human-readable version of the exception."""
```

### Comparing `nio-bot-1.0.0/src/niobot/utils/__init__.py` & `nio-bot-1.0.2/src/niobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/federation.py` & `nio-bot-1.0.2/src/niobot/utils/federation.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/help_command.py` & `nio-bot-1.0.2/src/niobot/utils/help_command.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/parsers.py` & `nio-bot-1.0.2/src/niobot/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/string_view.py` & `nio-bot-1.0.2/src/niobot/utils/string_view.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/typing.py` & `nio-bot-1.0.2/src/niobot/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/unblocking.py` & `nio-bot-1.0.2/src/niobot/utils/unblocking.py`

 * *Files identical despite different names*

