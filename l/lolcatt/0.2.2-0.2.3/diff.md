# Comparing `tmp/lolcatt-0.2.2.tar.gz` & `tmp/lolcatt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.2.2.tar", last modified: Sun Jul 16 11:07:42 2023, max compression
+gzip compressed data, was "lolcatt-0.2.3.tar", last modified: Sun Jul 16 12:48:18 2023, max compression
```

## Comparing `lolcatt-0.2.2.tar` & `lolcatt-0.2.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.2/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.2/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 11:07:42.861907 lolcatt-0.2.2/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2875 2023-07-16 00:40:56.000000 lolcatt-0.2.2/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.841907 lolcatt-0.2.2/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.837907 lolcatt-0.2.2/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.837907 lolcatt-0.2.2/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 23:27:13.000000 lolcatt-0.2.2/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.2/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.2/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 23:27:13.000000 lolcatt-0.2.2/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.2/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 23:27:13.000000 lolcatt-0.2.2/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.2/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-16 00:40:56.000000 lolcatt-0.2.2/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.2/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.2/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 23:27:11.000000 lolcatt-0.2.2/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.2/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.2/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 23:27:11.000000 lolcatt-0.2.2/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       41 2023-07-16 00:01:30.000000 lolcatt-0.2.2/lolcatt/.githash
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-16 11:06:32.000000 lolcatt-0.2.2/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-16 01:35:15.000000 lolcatt-0.2.2/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.2/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     9943 2023-07-16 10:55:02.000000 lolcatt-0.2.2/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/casting/youtube_playlist_handler.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1694 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.2/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-16 01:35:15.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4860 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-16 00:40:53.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2664 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      991 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.2/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2422 2023-07-16 10:50:45.000000 lolcatt-0.2.2/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1297 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       54 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-16 11:06:32.000000 lolcatt-0.2.2/pyproject.toml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-16 11:07:42.861907 lolcatt-0.2.2/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-16 11:06:32.000000 lolcatt-0.2.2/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.2/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.2/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.3/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.3/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4187 2023-07-16 12:48:18.288195 lolcatt-0.2.3/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3508 2023-07-16 12:36:17.000000 lolcatt-0.2.3/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.284195 lolcatt-0.2.3/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.284195 lolcatt-0.2.3/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-16 12:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-16 12:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-16 12:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-16 00:40:56.000000 lolcatt-0.2.3/docs/_build/html/_static/screenshot.png
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-16 00:40:56.000000 lolcatt-0.2.3/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.3/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.3/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-16 12:36:23.000000 lolcatt-0.2.3/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.3/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.3/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-16 12:36:23.000000 lolcatt-0.2.3/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       41 2023-07-16 00:01:30.000000 lolcatt-0.2.3/lolcatt/.githash
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-16 12:39:51.000000 lolcatt-0.2.3/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-16 01:35:15.000000 lolcatt-0.2.3/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.3/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    10010 2023-07-16 12:11:43.000000 lolcatt-0.2.3/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-16 00:40:56.000000 lolcatt-0.2.3/lolcatt/casting/youtube_playlist_handler.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1801 2023-07-16 12:19:23.000000 lolcatt-0.2.3/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.3/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-16 01:35:15.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4860 2023-07-16 00:40:56.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-16 00:40:53.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3068 2023-07-16 12:16:20.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2917 2023-07-16 12:16:38.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.3/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2422 2023-07-16 10:50:45.000000 lolcatt-0.2.3/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4187 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1297 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       52 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-16 12:39:51.000000 lolcatt-0.2.3/pyproject.toml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-16 12:48:18.292195 lolcatt-0.2.3/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-16 12:39:51.000000 lolcatt-0.2.3/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.3/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.3/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.2.2/LICENSE` & `lolcatt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/PKG-INFO` & `lolcatt-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.2
+Version: 0.2.3
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -44,45 +44,49 @@
 .. image:: https://raw.githubusercontent.com/LokiLuciferase/lolcatt/master/docs/_static/screenshot.png
    :align: center
    :alt:
 
 
 Dependencies
 ------------
-
-- A font containing FontAwesome icons. The freely available NerdFont_ collection is recommended.
+- Python 3.8+
+- catt_ (will be installed automatically)
+- yt-dlp_ (will be installed automatically)
+- Optional: A font containing FontAwesome icons to allow displaying of fancy icons on buttons. The freely available NerdFont_ collection is recommended. Fancy icons can be disabled and replaced by text (see below).
 
 
 Installation
 ------------
 
 .. code-block:: bash
 
     pip install lolcatt
 
 
 Quckstart
 ----------
 
-To determine the names of local chromecast devices, run ``lolcatt --scan``.
-Afterwards, run ``lolcatt --device '<device name>'`` to start the UI targeting the specified device.
-A default device and device aliases can be set in the ``catt`` configuration file, see catt_'s documentation for more information.
+At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
+To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
+A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To prepend a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
-Youtube playlists are supported, and each contained video will be played in sequence. By specifying a cookie file in the config file (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL).
+Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
 ---------------
 
 If button icons are not displayed correctly, ensure you are using a font containing FontAwesome icons. Alternatively, you can disable the use of fancy icons in the config file.
 
+If casting does not work for no apparent reason, ensure you have the latest version of ``yt_dlp`` installed: ``pip install --upgrade yt-dlp``.
+
 If you encounter any other issues, please open an issue.
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `LokiLuciferase/cookiecutter-pypackage`_ project template.
```

### Comparing `lolcatt-0.2.2/README.rst` & `lolcatt-0.2.3/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -24,45 +24,49 @@
 .. image:: https://raw.githubusercontent.com/LokiLuciferase/lolcatt/master/docs/_static/screenshot.png
    :align: center
    :alt:
 
 
 Dependencies
 ------------
-
-- A font containing FontAwesome icons. The freely available NerdFont_ collection is recommended.
+- Python 3.8+
+- catt_ (will be installed automatically)
+- yt-dlp_ (will be installed automatically)
+- Optional: A font containing FontAwesome icons to allow displaying of fancy icons on buttons. The freely available NerdFont_ collection is recommended. Fancy icons can be disabled and replaced by text (see below).
 
 
 Installation
 ------------
 
 .. code-block:: bash
 
     pip install lolcatt
 
 
 Quckstart
 ----------
 
-To determine the names of local chromecast devices, run ``lolcatt --scan``.
-Afterwards, run ``lolcatt --device '<device name>'`` to start the UI targeting the specified device.
-A default device and device aliases can be set in the ``catt`` configuration file, see catt_'s documentation for more information.
+At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
+To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
+A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To prepend a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
-Youtube playlists are supported, and each contained video will be played in sequence. By specifying a cookie file in the config file (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL).
+Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
 ---------------
 
 If button icons are not displayed correctly, ensure you are using a font containing FontAwesome icons. Alternatively, you can disable the use of fancy icons in the config file.
 
+If casting does not work for no apparent reason, ensure you have the latest version of ``yt_dlp`` installed: ``pip install --upgrade yt-dlp``.
+
 If you encounter any other issues, please open an issue.
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `LokiLuciferase/cookiecutter-pypackage`_ project template.
```

### Comparing `lolcatt-0.2.2/docs/Makefile` & `lolcatt-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/_build/html/_static/basic.css` & `lolcatt-0.2.3/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/_build/html/_static/nature.css` & `lolcatt-0.2.3/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/_build/html/_static/pygments.css` & `lolcatt-0.2.3/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/_build/html/_static/screenshot.png` & `lolcatt-0.2.3/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/_static/screenshot.png` & `lolcatt-0.2.3/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/conf.py` & `lolcatt-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/installation.rst` & `lolcatt-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/lolcatt.rst` & `lolcatt-0.2.3/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/lolcatt.ui.rst` & `lolcatt-0.2.3/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/docs/make.bat` & `lolcatt-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt/app.py` & `lolcatt-0.2.3/lolcatt/app.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt/casting/caster.py` & `lolcatt-0.2.3/lolcatt/casting/caster.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 class CastState:
     """Dataclass for cast state, encapsulating info dictionaries of a catt controller."""
 
     cast_info: dict
     info: dict
     is_loading: bool = False
     media_loaded: bool = False
+    queue_len: int = 0
 
 
 class Caster:
     """
     Class encapsulating the catt.api.CattDevice.
 
     Provides a simple interface and enables exchange of the CattDevice on the fly.
@@ -291,9 +292,10 @@
             cs = CastState({}, {}, False, False)
         else:
             cs = CastState(
                 self._device.controller.cast_info,
                 self._device.controller.info,
                 is_loading=self._is_loading_cast,
                 media_loaded=self._media_loaded,
+                queue_len=len(self._queue),
             )
         return cs
```

### Comparing `lolcatt-0.2.2/lolcatt/casting/youtube_playlist_handler.py` & `lolcatt-0.2.3/lolcatt/casting/youtube_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt/cli.py` & `lolcatt-0.2.3/lolcatt/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 from pathlib import Path
 
 import click
 import toml
 
+from lolcatt import __version__
 from lolcatt.app import LolCatt
 from lolcatt.utils.utils import scan as do_scan
 from lolcatt.utils.utils import write_initial_config
 
 
 @click.command(
     'lolcatt',
     context_settings=dict(help_option_names=['-h', '--help']),
 )
+@click.version_option(__version__, '-v', '--version', prog_name='lolcatt')
 @click.argument(
     'url_or_path',
     nargs=1,
     default=None,
     required=False,
 )
 @click.option(
```

### Comparing `lolcatt-0.2.2/lolcatt/ui/lolcatt.css` & `lolcatt-0.2.3/lolcatt/ui/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.2.3/lolcatt/ui/lolcatt_controls.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.2.3/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.2.3/lolcatt/ui/lolcatt_playback_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.2.3/lolcatt/ui/lolcatt_progress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,63 @@
+from typing import Optional
 from typing import Tuple
 
 from catt.error import CastError
 from textual.containers import Container
 from textual.events import Click
 from textual.reactive import reactive
 from textual.widgets import Label
 from textual.widgets import ProgressBar
 from textual.widgets import Static
 
 
 class LolCattProgress(Static):
     current = reactive(0)
     duration = reactive(0)
+    queue_len = reactive(0)
     percent_complete = reactive(0)
 
     @staticmethod
-    def _extract_progress(cast_info: dict) -> Tuple[float, float, float]:
-        current = cast_info.get('current_time', 0.0)
-        duration = cast_info.get('duration', 0.0)
+    def _extract_progress(cast_info: dict) -> Tuple[Optional[float], Optional[float], float]:
+        current = cast_info.get('current_time')
+        duration = cast_info.get('duration')
         percent_complete = current / duration * 100 if duration else 0.0
         return current, duration, percent_complete
 
-    def _format_time(self, seconds: float) -> str:
+    @staticmethod
+    def _format_time(seconds: float) -> str:
         if seconds is None:
             return '--:--'
         minutes, seconds = divmod(seconds, 60)
         hours, minutes = divmod(minutes, 60)
         if hours:
             return f'{hours:02.0f}:{minutes:02.0f}:{seconds:02.0f}'
         return f'{minutes:02.0f}:{seconds:02.0f}'
 
+    @staticmethod
+    def _format_queue_len(queue_len: int, current: Optional[float]) -> str:
+        if queue_len == 0 or current is None:
+            return ''
+        return f'(1/{queue_len + 1})'
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.pb = ProgressBar(total=100, show_percentage=False, show_eta=False, id='progress_bar')
         self.pblabel = Label('', id='progress_label')
         self._needed_width = 16  # FIXME: learn CSS
 
     def update_progress(self) -> int:
-        self.current, self.duration, self.percent_complete = self._extract_progress(
-            self.app.caster.get_cast_state().cast_info
-        )
+        state = self.app.caster.get_cast_state()
+        self.current, self.duration, self.percent_complete = self._extract_progress(state.cast_info)
+        self.queue_len = state.queue_len
         self.pb.update(progress=self.percent_complete)
         current_fmt = self._format_time(self.current)
         duration_fmt = self._format_time(self.duration)
-        upd_str = f'({current_fmt}/{duration_fmt})'
+        queue_fmt = self._format_queue_len(self.queue_len, self.current)
+        upd_str = f'[{current_fmt}/{duration_fmt}]{queue_fmt}'
         padding = ' ' * max(0, (self._needed_width - len(upd_str)))
         self.pblabel.update(f'{padding}{upd_str}')
 
     def on_mount(self):
         self.update_progress()
         self.set_interval(
             interval=self.app.caster.get_update_interval(), callback=self.update_progress
```

### Comparing `lolcatt-0.2.2/lolcatt/utils/utils.py` & `lolcatt-0.2.3/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.2.3/lolcatt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.2
+Version: 0.2.3
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -44,45 +44,49 @@
 .. image:: https://raw.githubusercontent.com/LokiLuciferase/lolcatt/master/docs/_static/screenshot.png
    :align: center
    :alt:
 
 
 Dependencies
 ------------
-
-- A font containing FontAwesome icons. The freely available NerdFont_ collection is recommended.
+- Python 3.8+
+- catt_ (will be installed automatically)
+- yt-dlp_ (will be installed automatically)
+- Optional: A font containing FontAwesome icons to allow displaying of fancy icons on buttons. The freely available NerdFont_ collection is recommended. Fancy icons can be disabled and replaced by text (see below).
 
 
 Installation
 ------------
 
 .. code-block:: bash
 
     pip install lolcatt
 
 
 Quckstart
 ----------
 
-To determine the names of local chromecast devices, run ``lolcatt --scan``.
-Afterwards, run ``lolcatt --device '<device name>'`` to start the UI targeting the specified device.
-A default device and device aliases can be set in the ``catt`` configuration file, see catt_'s documentation for more information.
+At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
+To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
+A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To prepend a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
-Youtube playlists are supported, and each contained video will be played in sequence. By specifying a cookie file in the config file (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL).
+Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
 ---------------
 
 If button icons are not displayed correctly, ensure you are using a font containing FontAwesome icons. Alternatively, you can disable the use of fancy icons in the config file.
 
+If casting does not work for no apparent reason, ensure you have the latest version of ``yt_dlp`` installed: ``pip install --upgrade yt-dlp``.
+
 If you encounter any other issues, please open an issue.
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `LokiLuciferase/cookiecutter-pypackage`_ project template.
```

### Comparing `lolcatt-0.2.2/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.2.3/lolcatt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.2/pyproject.toml` & `lolcatt-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.2.2"
+current_version = "0.2.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.2.2/setup.py` & `lolcatt-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.2.2',
+    version='0.2.3',
     zip_safe=False,
 )
```

