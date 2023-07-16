# Comparing `tmp/lolcatt-0.2.1.tar.gz` & `tmp/lolcatt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.2.1.tar", last modified: Sun Jul 16 00:16:45 2023, max compression
+gzip compressed data, was "lolcatt-0.2.2.tar", last modified: Sun Jul 16 11:07:42 2023, max compression
```

## Comparing `lolcatt-0.2.1.tar` & `lolcatt-0.2.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.993017 lolcatt-0.2.1/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.1/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.1/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 00:16:45.993017 lolcatt-0.2.1/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2875 2023-07-15 23:28:47.000000 lolcatt-0.2.1/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.985017 lolcatt-0.2.1/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.985017 lolcatt-0.2.1/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 23:27:13.000000 lolcatt-0.2.1/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 23:27:13.000000 lolcatt-0.2.1/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 23:27:13.000000 lolcatt-0.2.1/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.1/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.1/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.1/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.1/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 23:27:11.000000 lolcatt-0.2.1/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.1/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.1/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 23:27:11.000000 lolcatt-0.2.1/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       41 2023-07-16 00:01:30.000000 lolcatt-0.2.1/lolcatt/.githash
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-16 00:16:20.000000 lolcatt-0.2.1/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-15 23:33:36.000000 lolcatt-0.2.1/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.1/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     9247 2023-07-16 00:05:22.000000 lolcatt-0.2.1/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-15 22:39:08.000000 lolcatt-0.2.1/lolcatt/casting/youtube_playlist_handler.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1694 2023-07-15 22:09:07.000000 lolcatt-0.2.1/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.1/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-15 23:33:36.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4860 2023-07-16 00:13:16.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 16:19:10.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2664 2023-07-16 00:14:35.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      991 2023-07-15 22:09:07.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.993017 lolcatt-0.2.1/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.1/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1752 2023-07-15 23:09:49.000000 lolcatt-0.2.1/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1297 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       54 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-16 00:16:20.000000 lolcatt-0.2.1/pyproject.toml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-16 00:16:45.993017 lolcatt-0.2.1/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-16 00:16:20.000000 lolcatt-0.2.1/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.993017 lolcatt-0.2.1/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.1/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.1/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.2/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.2/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 11:07:42.861907 lolcatt-0.2.2/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2875 2023-07-16 00:40:56.000000 lolcatt-0.2.2/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.841907 lolcatt-0.2.2/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.837907 lolcatt-0.2.2/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.837907 lolcatt-0.2.2/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 23:27:13.000000 lolcatt-0.2.2/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 23:27:13.000000 lolcatt-0.2.2/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 23:27:13.000000 lolcatt-0.2.2/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.2/docs/_build/html/_static/screenshot.png
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-16 00:40:56.000000 lolcatt-0.2.2/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.2/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.2/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 23:27:11.000000 lolcatt-0.2.2/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.2/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.2/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 23:27:11.000000 lolcatt-0.2.2/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.2/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       41 2023-07-16 00:01:30.000000 lolcatt-0.2.2/lolcatt/.githash
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-16 11:06:32.000000 lolcatt-0.2.2/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-16 01:35:15.000000 lolcatt-0.2.2/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.2/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     9943 2023-07-16 10:55:02.000000 lolcatt-0.2.2/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/casting/youtube_playlist_handler.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1694 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.2/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-16 01:35:15.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4860 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-16 00:40:53.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2664 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      991 2023-07-16 00:40:56.000000 lolcatt-0.2.2/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.2/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2422 2023-07-16 10:50:45.000000 lolcatt-0.2.2/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.857907 lolcatt-0.2.2/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1297 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       54 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-16 11:07:42.000000 lolcatt-0.2.2/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-16 11:06:32.000000 lolcatt-0.2.2/pyproject.toml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-16 11:07:42.861907 lolcatt-0.2.2/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-16 11:06:32.000000 lolcatt-0.2.2/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 11:07:42.861907 lolcatt-0.2.2/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.2/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.2/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.2.1/LICENSE` & `lolcatt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/PKG-INFO` & `lolcatt-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.1
+Version: 0.2.2
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.2.1/README.rst` & `lolcatt-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/Makefile` & `lolcatt-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/_build/html/_static/basic.css` & `lolcatt-0.2.2/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/_build/html/_static/nature.css` & `lolcatt-0.2.2/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/_build/html/_static/pygments.css` & `lolcatt-0.2.2/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/_build/html/_static/screenshot.png` & `lolcatt-0.2.2/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/_static/screenshot.png` & `lolcatt-0.2.2/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/conf.py` & `lolcatt-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/installation.rst` & `lolcatt-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/lolcatt.rst` & `lolcatt-0.2.2/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/lolcatt.ui.rst` & `lolcatt-0.2.2/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/docs/make.bat` & `lolcatt-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/app.py` & `lolcatt-0.2.2/lolcatt/app.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/casting/caster.py` & `lolcatt-0.2.2/lolcatt/casting/caster.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 import subprocess
 import time
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from catt.api import CattDevice
 from catt.api import discover
 from catt.cli import get_config_as_dict
@@ -57,14 +58,29 @@
         self._media_loaded = False
         self._loading_timeout = 8
         self._update_interval = update_interval
         self._autoplay = autoplay
         self._state_last_updated = time.time()
         self.change_device(name_or_alias)
 
+    def _build_cast_args(self) -> List[str]:
+        catt_cast_args = self.CAST_ARGS[:]
+
+        # if we have a cookies file for youtube, attempt to mark videos as watched
+        if self._config.get('options', {}).get('youtube_mark_watched', False):
+            cookies_file = self._config.get('options', {}).get('youtube_cookies_file')
+            if cookies_file is not None:
+                cookies_file = str(Path(cookies_file).expanduser().resolve())
+                catt_cast_args += [
+                    '--ytdl-option=mark_watched=true',
+                    f'--ytdl-option=cookiefile={cookies_file}',
+                ]
+
+        return catt_cast_args
+
     def cast(self, url_or_path: str):
         """
         Casts the given url or path to the currently active device.
 
         :param url_or_path: The url or path to cast.
         """
         if self._catt_call is not None:
@@ -73,15 +89,15 @@
             raise ValueError('Can\'t cast: No device selected.')
         full_catt_args = [
             'catt',
             *self.CATT_ARGS,
             '-d',
             self._device_name,
             'cast',
-            *self.CAST_ARGS,
+            *self._build_cast_args(),
             url_or_path,
         ]
         self._catt_call = subprocess.Popen(
             full_catt_args,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
```

### Comparing `lolcatt-0.2.1/lolcatt/casting/youtube_playlist_handler.py` & `lolcatt-0.2.2/lolcatt/casting/youtube_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/cli.py` & `lolcatt-0.2.2/lolcatt/cli.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/ui/lolcatt.css` & `lolcatt-0.2.2/lolcatt/ui/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.2.2/lolcatt/ui/lolcatt_controls.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.2.2/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.2.2/lolcatt/ui/lolcatt_playback_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.2.2/lolcatt/ui/lolcatt_progress.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.2.2/lolcatt/ui/lolcatt_url_input.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/lolcatt/utils/utils.py` & `lolcatt-0.2.2/lolcatt/utils/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 from pathlib import Path
 
 from catt.api import discover
+from catt.cli import get_config_as_dict
 
 
 def marquee(s: str, max_len: int, step_size: int) -> str:
     """
     Yields a string that is max_len characters long, and shifts the string by step_size each time.
 
     :param s: The string to be shifted
@@ -21,33 +22,47 @@
             yield s[:max_len]
 
 
 def scan():
     """Scans the network for Chromecast devices and prints the results."""
     print('Scanning for Chromecast devices...')
 
+    # Invert aliases dict
+    aliases = get_config_as_dict().get('aliases', {})
+    devices_to_aliases = {v: k for k, v in aliases.items()}
+
     discovered = discover()
     deduped = []
     found_ips = set()
     max_name_len = 11  # len('Device name')
+    max_alias_len = 5  # len('Alias')
     for device in discovered:
         if device.ip_addr not in found_ips:
             found_ips.add(device.ip_addr)
             max_name_len = max(max_name_len, len(device.name))
-            deduped.append((device.name, device.ip_addr))
+            max_alias_len = max(max_alias_len, len(devices_to_aliases.get(device.name, '')))
+            deduped.append((device.name, devices_to_aliases.get(device.name, ''), device.ip_addr))
 
-    deduped = [('"' + x + '"' + ' ' * (max_name_len - len(x)), y) for x, y in deduped]
+    deduped = [
+        (
+            '"' + x + '"' + ' ' * (max_name_len - len(x)),
+            ('"' + y + '"' if len(y) else '') + ' ' * (max_alias_len - len(y)),
+            z,
+        )
+        for x, y, z in deduped
+    ]
     deduped = sorted(deduped, key=lambda x: x[1])
 
     print('Found {} device(s):'.format(len(found_ips)))
-    print(f'Device name{" " * (max_name_len - 11)}\tDevice IP')
-    print('=' * (max_name_len + 19))
-    for name, ip in deduped:
-        print(f'{name}\t{ip}')
+    print(f'Device name{" " * (max_name_len - 11)}\tAlias{" " * (max_alias_len - 5) }\tDevice IP')
+    print('=' * (max_name_len + max_alias_len + 22))
+    for name, alias, ip in deduped:
+        print(f'{name}\t{alias}\t{ip}')
 
 
 def write_initial_config(p: Path):
     p.write_text(
         "[options]\n"
         "fancy_icons = true  # Whether to use fancy icons\n"
-        "#youtube_cookies_file = \"~/.config/lolcatt/cookies.txt\"  # Path to a cookies.txt file for YouTube"
+        "#youtube_cookies_file = \"~/.config/lolcatt/cookies.txt\"  # Path to a cookies.txt file for YouTube\n"
+        "youtube_mark_watched = true # Whether to mark YouTube videos as watched (only if we have cookies)"
     )
```

### Comparing `lolcatt-0.2.1/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.2.2/lolcatt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.1
+Version: 0.2.2
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.2.1/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.2.2/lolcatt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.1/pyproject.toml` & `lolcatt-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.2.1"
+current_version = "0.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.2.1/setup.py` & `lolcatt-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
```

