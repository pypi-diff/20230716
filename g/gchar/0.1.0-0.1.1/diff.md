# Comparing `tmp/gchar-0.1.0.tar.gz` & `tmp/gchar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gchar-0.1.0.tar", last modified: Thu Jul 13 11:10:29 2023, max compression
+gzip compressed data, was "gchar-0.1.1.tar", last modified: Sun Jul 16 09:50:28 2023, max compression
```

## Comparing `gchar-0.1.0.tar` & `gchar-0.1.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 11:09:10.000000 gchar-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-13 11:09:10.000000 gchar-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-13 11:10:29.370192 gchar-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-13 11:09:10.000000 gchar-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/arknights/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/azurlane/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/base/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/character.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/skin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/bluearchive/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/dispatch/access.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/fgo/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/genshin/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/character.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/girlsfrontline/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/neuralcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/character.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/nikke/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/character.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/pathtonowhere/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/character.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/starrail/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/character.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/resources/pixiv/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/resources/sites/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/sites/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/sites/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-crawl.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-speedup.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:10:29.370192 gchar-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-13 11:09:10.000000 gchar-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.480051 gchar-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 09:48:51.000000 gchar-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-16 09:48:51.000000 gchar-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-16 09:50:28.480051 gchar-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-16 09:48:51.000000 gchar-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.464051 gchar-0.1.1/gchar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.468051 gchar-0.1.1/gchar/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.468051 gchar-0.1.1/gchar/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.468051 gchar-0.1.1/gchar/games/arknights/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/arknights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/arknights/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/arknights/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/arknights/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.468051 gchar-0.1.1/gchar/games/azurlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/azurlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/azurlane/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/azurlane/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/azurlane/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.468051 gchar-0.1.1/gchar/games/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/base/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/base/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/base/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/base/skin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.472051 gchar-0.1.1/gchar/games/bluearchive/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/bluearchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/bluearchive/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/bluearchive/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/bluearchive/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.472051 gchar-0.1.1/gchar/games/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/dispatch/access.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.472051 gchar-0.1.1/gchar/games/fgo/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/fgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/fgo/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/fgo/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/fgo/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.472051 gchar-0.1.1/gchar/games/genshin/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/genshin/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/genshin/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/genshin/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.472051 gchar-0.1.1/gchar/games/girlsfrontline/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/girlsfrontline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/girlsfrontline/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/girlsfrontline/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/girlsfrontline/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.472051 gchar-0.1.1/gchar/games/neuralcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/neuralcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/neuralcloud/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/neuralcloud/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/neuralcloud/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.476051 gchar-0.1.1/gchar/games/nikke/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/nikke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/nikke/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/nikke/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/nikke/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.476051 gchar-0.1.1/gchar/games/pathtonowhere/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/pathtonowhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/pathtonowhere/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/pathtonowhere/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/pathtonowhere/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.476051 gchar-0.1.1/gchar/games/starrail/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/starrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/starrail/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/starrail/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/games/starrail/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.476051 gchar-0.1.1/gchar/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.476051 gchar-0.1.1/gchar/resources/pixiv/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/pixiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/pixiv/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/pixiv/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/pixiv/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.476051 gchar-0.1.1/gchar/resources/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/sites/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/resources/sites/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.480051 gchar-0.1.1/gchar/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-16 09:48:51.000000 gchar-0.1.1/gchar/utils/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:50:28.468051 gchar-0.1.1/gchar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-16 09:50:28.000000 gchar-0.1.1/gchar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-16 09:50:28.000000 gchar-0.1.1/gchar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:50:28.000000 gchar-0.1.1/gchar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-16 09:50:28.000000 gchar-0.1.1/gchar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 09:50:28.000000 gchar-0.1.1/gchar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-16 09:48:51.000000 gchar-0.1.1/requirements-crawl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-16 09:48:51.000000 gchar-0.1.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 09:48:51.000000 gchar-0.1.1/requirements-speedup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-16 09:48:51.000000 gchar-0.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-16 09:48:51.000000 gchar-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 09:50:28.480051 gchar-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-16 09:48:51.000000 gchar-0.1.1/setup.py
```

### Comparing `gchar-0.1.0/LICENSE` & `gchar-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/PKG-INFO` & `gchar-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gchar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Game character manager.
 Home-page: https://github.com/narugo1992/gchar
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: speedup
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 # gchar
 
 [![PyPI](https://img.shields.io/pypi/v/gchar)](https://pypi.org/project/gchar/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gchar)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/254442dea2e77cf46366df97f499242f/raw/loc.json)
@@ -172,14 +172,15 @@
 * [Konachan.Net](https://konachan.net), named `konachan_net`
 * [Lolibooru](https://lolibooru.moe), named `lolibooru`
 * [Rule34](https://rule34.xxx), named `rule34`
 * [Safebooru](https://safebooru.donmai.us), named `safebooru`
 * [Xbooru](https://xbooru.com), named `xbooru`
 * [Yande](https://yande.re), named `yande`
 * [Zerochan](https://zerochan.net), named `zerochan`
+* [WallHaven](https://wallhaven.cc), named `wallhaven` (`id:xxxx` will be used for explicit searching)
 
 ```
 >>> from gchar.resources.sites import get_site_tag
 >>> 
 >>> # first one is all, second one is r18
 >>> get_site_tag('CEO', 'danbooru')
 'penthesilea_(fate)'
```

### Comparing `gchar-0.1.0/README.md` & `gchar-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 * [Konachan.Net](https://konachan.net), named `konachan_net`
 * [Lolibooru](https://lolibooru.moe), named `lolibooru`
 * [Rule34](https://rule34.xxx), named `rule34`
 * [Safebooru](https://safebooru.donmai.us), named `safebooru`
 * [Xbooru](https://xbooru.com), named `xbooru`
 * [Yande](https://yande.re), named `yande`
 * [Zerochan](https://zerochan.net), named `zerochan`
+* [WallHaven](https://wallhaven.cc), named `wallhaven` (`id:xxxx` will be used for explicit searching)
 
 ```
 >>> from gchar.resources.sites import get_site_tag
 >>> 
 >>> # first one is all, second one is r18
 >>> get_site_tag('CEO', 'danbooru')
 'penthesilea_(fate)'
```

### Comparing `gchar-0.1.0/gchar/games/arknights/character.py` & `gchar-0.1.1/gchar/games/arknights/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/arknights/name.py` & `gchar-0.1.1/gchar/games/arknights/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/arknights/property.py` & `gchar-0.1.1/gchar/games/arknights/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/azurlane/character.py` & `gchar-0.1.1/gchar/games/azurlane/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/azurlane/name.py` & `gchar-0.1.1/gchar/games/azurlane/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/azurlane/property.py` & `gchar-0.1.1/gchar/games/azurlane/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/base/character.py` & `gchar-0.1.1/gchar/games/base/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/base/name.py` & `gchar-0.1.1/gchar/games/base/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/base/property.py` & `gchar-0.1.1/gchar/games/base/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/base/skin.py` & `gchar-0.1.1/gchar/games/base/skin.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/bluearchive/character.py` & `gchar-0.1.1/gchar/games/bluearchive/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/bluearchive/name.py` & `gchar-0.1.1/gchar/games/bluearchive/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/bluearchive/property.py` & `gchar-0.1.1/gchar/games/bluearchive/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/dispatch/access.py` & `gchar-0.1.1/gchar/games/dispatch/access.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/fgo/character.py` & `gchar-0.1.1/gchar/games/fgo/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/fgo/name.py` & `gchar-0.1.1/gchar/games/fgo/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/fgo/property.py` & `gchar-0.1.1/gchar/games/fgo/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/genshin/character.py` & `gchar-0.1.1/gchar/games/genshin/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/genshin/property.py` & `gchar-0.1.1/gchar/games/genshin/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/girlsfrontline/character.py` & `gchar-0.1.1/gchar/games/girlsfrontline/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/girlsfrontline/name.py` & `gchar-0.1.1/gchar/games/girlsfrontline/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/girlsfrontline/property.py` & `gchar-0.1.1/gchar/games/girlsfrontline/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/neuralcloud/character.py` & `gchar-0.1.1/gchar/games/neuralcloud/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/neuralcloud/name.py` & `gchar-0.1.1/gchar/games/neuralcloud/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/neuralcloud/property.py` & `gchar-0.1.1/gchar/games/neuralcloud/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/nikke/character.py` & `gchar-0.1.1/gchar/games/nikke/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/nikke/property.py` & `gchar-0.1.1/gchar/games/nikke/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/pathtonowhere/character.py` & `gchar-0.1.1/gchar/games/pathtonowhere/character.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,19 @@
     def _index(self):
         return self.__raw_data['id']
 
     def _cnname(self):
         return self.__raw_data['cnname']
 
     def _jpname(self):
-        return []
+        jpnames = self.__raw_data['jpnames']
+        return jpnames[0] if jpnames else None
+
+    def _jpnames(self):
+        return self.__raw_data['jpnames']
 
     def _enname(self):
         return self.__raw_data['enname']
 
     def _gender(self):
         return self.__raw_data['gender']
```

### Comparing `gchar-0.1.0/gchar/games/pathtonowhere/property.py` & `gchar-0.1.1/gchar/games/pathtonowhere/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/games/starrail/character.py` & `gchar-0.1.1/gchar/games/starrail/character.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .property import Rarity
 from ..base import Character as _BaseCharacter, Gender
 from ..base.name import _BaseName
 
 
 class Character(_BaseCharacter):
     __game_name__ = 'starrail'
-    __official_name__ = 'Honkai Star Rail'
+    __official_name__ = 'Honkai: Star Rail'
     __cnname_class__ = ChineseName
     __enname_class__ = EnglishName
     __jpname_class__ = JapaneseName
 
     def __init__(self, raw_data):
         self.__raw_data = raw_data
```

### Comparing `gchar-0.1.0/gchar/games/starrail/property.py` & `gchar-0.1.1/gchar/games/starrail/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/resources/pixiv/base.py` & `gchar-0.1.1/gchar/resources/pixiv/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _GAMES = {
     'arknights': ('アークナイツ', 'アークナイツ'),
     'fgo': ('Fate/GrandOrder', 'Fate'),
     'azurlane': ('アズールレーン', 'アズールレーン'),
     'genshin': ('原神', '原神'),
     'girlsfrontline': ('ドールズフロントライン', 'ドールズフロントライン'),
-    'neuralcloud': ('云图计划', '云图计划'),
+    'neuralcloud': ('ニューラルクラウド', 'ニューラルクラウド'),
     'bluearchive': ('ブルーアーカイブ', 'ブルーアーカイブ'),
     'pathtonowhere': ('無期迷途', '無期迷途'),
     'nikke': ('勝利の女神:NIKKE', '勝利の女神:NIKKE'),
     'starrail': ('崩壊スターレイル', 'スターレイル'),
 }
```

### Comparing `gchar-0.1.0/gchar/resources/pixiv/keyword.py` & `gchar-0.1.1/gchar/resources/pixiv/keyword.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/resources/pixiv/tag.py` & `gchar-0.1.1/gchar/resources/pixiv/tag.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/resources/sites/base.py` & `gchar-0.1.1/gchar/resources/sites/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     'konachan_net': 'konachan.net',
     'lolibooru': 'lolibooru.moe',
     'rule34': 'rule34.xxx',
     'safebooru': 'safebooru.donmai.us',
     'xbooru': 'xbooru.com',
     'yande': 'yande.re',
     'zerochan': 'zerochan.net',
+    'wallhaven': 'wallhaven.cc',
 }
 
 
 def list_available_sites() -> List[str]:
     """
     List the available supported image website names.
```

### Comparing `gchar-0.1.0/gchar/resources/sites/tags.py` & `gchar-0.1.1/gchar/resources/sites/tags.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/utils/cache.py` & `gchar-0.1.1/gchar/utils/cache.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/utils/cli.py` & `gchar-0.1.1/gchar/utils/cli.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/utils/compare.py` & `gchar-0.1.1/gchar/utils/compare.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/utils/download.py` & `gchar-0.1.1/gchar/utils/download.py`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar/utils/session.py` & `gchar-0.1.1/gchar/utils/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
     session = session or requests.session()
     retries = Retry(
         total=max_retries, backoff_factor=1,
         status_forcelist=[413, 429, 500, 501, 502, 503, 504, 505, 506, 507, 509, 510, 511],
         allowed_methods=["HEAD", "GET", "POST", "PUT", "DELETE", "OPTIONS", "TRACE"],
     )
-    adapter = TimeoutHTTPAdapter(max_retries=retries, timeout=timeout)
+    adapter = TimeoutHTTPAdapter(max_retries=retries, timeout=timeout, pool_connections=32, pool_maxsize=32)
     session.mount('http://', adapter)
     session.mount('https://', adapter)
     session.headers.update({
         "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
                       "(KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36",
         **dict(headers or {}),
     })
```

### Comparing `gchar-0.1.0/gchar.egg-info/PKG-INFO` & `gchar-0.1.1/gchar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gchar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Game character manager.
 Home-page: https://github.com/narugo1992/gchar
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: speedup
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 # gchar
 
 [![PyPI](https://img.shields.io/pypi/v/gchar)](https://pypi.org/project/gchar/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gchar)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/254442dea2e77cf46366df97f499242f/raw/loc.json)
@@ -172,14 +172,15 @@
 * [Konachan.Net](https://konachan.net), named `konachan_net`
 * [Lolibooru](https://lolibooru.moe), named `lolibooru`
 * [Rule34](https://rule34.xxx), named `rule34`
 * [Safebooru](https://safebooru.donmai.us), named `safebooru`
 * [Xbooru](https://xbooru.com), named `xbooru`
 * [Yande](https://yande.re), named `yande`
 * [Zerochan](https://zerochan.net), named `zerochan`
+* [WallHaven](https://wallhaven.cc), named `wallhaven` (`id:xxxx` will be used for explicit searching)
 
 ```
 >>> from gchar.resources.sites import get_site_tag
 >>> 
 >>> # first one is all, second one is r18
 >>> get_site_tag('CEO', 'danbooru')
 'penthesilea_(fate)'
```

### Comparing `gchar-0.1.0/gchar.egg-info/SOURCES.txt` & `gchar-0.1.1/gchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gchar-0.1.0/gchar.egg-info/requires.txt` & `gchar-0.1.1/gchar.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 enum_tools
 sphinx-toolbox
 plantumlcli>=0.0.2
 packaging
 sphinx-multiversion~=0.2.4
 where~=1.0.2
 easydict<2,>=1.7
+tabulate
 
 [speedup]
 thefuzz[speedup]
 
 [test]
 coverage>=5
 mock>=4.0.3
```

### Comparing `gchar-0.1.0/setup.py` & `gchar-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 def _load_req(file: str):
     with open(file, 'r', 'utf-8') as f:
         return [line.strip() for line in f.readlines() if line.strip()]
 
 
 requirements = _load_req('requirements.txt')
 
+# do not put requirements-crawl.txt inside
 _REQ_BLACKLIST = ['crawl']
 _REQ_PATTERN = re.compile('^requirements-([a-zA-Z0-9_]+)\\.txt$')
 group_requirements = {
     item.group(1): _load_req(item.group(0))
     for item in [_REQ_PATTERN.fullmatch(reqpath) for reqpath in os.listdir()]
     if item and item.group(1) not in _REQ_BLACKLIST
 }
```

