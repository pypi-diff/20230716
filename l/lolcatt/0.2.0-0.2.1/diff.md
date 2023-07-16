# Comparing `tmp/lolcatt-0.2.0.tar.gz` & `tmp/lolcatt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.2.0.tar", last modified: Sat Jul 15 23:52:37 2023, max compression
+gzip compressed data, was "lolcatt-0.2.1.tar", last modified: Sun Jul 16 00:16:45 2023, max compression
```

## Comparing `lolcatt-0.2.0.tar` & `lolcatt-0.2.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.0/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.0/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-15 23:52:37.751730 lolcatt-0.2.0/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2875 2023-07-15 23:28:47.000000 lolcatt-0.2.0/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.743730 lolcatt-0.2.0/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.743730 lolcatt-0.2.0/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 23:27:13.000000 lolcatt-0.2.0/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 23:27:13.000000 lolcatt-0.2.0/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 23:27:13.000000 lolcatt-0.2.0/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.0/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.0/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.0/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.0/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 23:27:11.000000 lolcatt-0.2.0/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.0/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.0/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 23:27:11.000000 lolcatt-0.2.0/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-15 23:49:49.000000 lolcatt-0.2.0/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-15 23:33:36.000000 lolcatt-0.2.0/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.0/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     9247 2023-07-15 22:10:13.000000 lolcatt-0.2.0/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-15 22:39:08.000000 lolcatt-0.2.0/lolcatt/casting/youtube_playlist_handler.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1694 2023-07-15 22:09:07.000000 lolcatt-0.2.0/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.0/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-15 23:33:36.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4614 2023-07-15 23:44:24.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 16:19:10.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2646 2023-07-15 14:07:42.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      991 2023-07-15 22:09:07.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.0/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1752 2023-07-15 23:09:49.000000 lolcatt-0.2.0/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1280 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       54 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-15 23:49:49.000000 lolcatt-0.2.0/pyproject.toml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-15 23:52:37.751730 lolcatt-0.2.0/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-15 23:49:49.000000 lolcatt-0.2.0/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.0/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.0/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.993017 lolcatt-0.2.1/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.1/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.1/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 00:16:45.993017 lolcatt-0.2.1/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2875 2023-07-15 23:28:47.000000 lolcatt-0.2.1/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.985017 lolcatt-0.2.1/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.985017 lolcatt-0.2.1/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 23:27:13.000000 lolcatt-0.2.1/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 23:27:13.000000 lolcatt-0.2.1/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 23:27:13.000000 lolcatt-0.2.1/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.1/docs/_build/html/_static/screenshot.png
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.1/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.1/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.1/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 23:27:11.000000 lolcatt-0.2.1/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.1/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.1/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 23:27:11.000000 lolcatt-0.2.1/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.1/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       41 2023-07-16 00:01:30.000000 lolcatt-0.2.1/lolcatt/.githash
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-16 00:16:20.000000 lolcatt-0.2.1/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-15 23:33:36.000000 lolcatt-0.2.1/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.1/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     9247 2023-07-16 00:05:22.000000 lolcatt-0.2.1/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-15 22:39:08.000000 lolcatt-0.2.1/lolcatt/casting/youtube_playlist_handler.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1694 2023-07-15 22:09:07.000000 lolcatt-0.2.1/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.1/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-15 23:33:36.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4860 2023-07-16 00:13:16.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 16:19:10.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2664 2023-07-16 00:14:35.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      991 2023-07-15 22:09:07.000000 lolcatt-0.2.1/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.993017 lolcatt-0.2.1/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.1/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1752 2023-07-15 23:09:49.000000 lolcatt-0.2.1/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.989017 lolcatt-0.2.1/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1297 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       54 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-16 00:16:45.000000 lolcatt-0.2.1/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-16 00:16:20.000000 lolcatt-0.2.1/pyproject.toml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-16 00:16:45.993017 lolcatt-0.2.1/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-16 00:16:20.000000 lolcatt-0.2.1/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 00:16:45.993017 lolcatt-0.2.1/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.1/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.1/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.2.0/LICENSE` & `lolcatt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/PKG-INFO` & `lolcatt-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.0
+Version: 0.2.1
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.2.0/README.rst` & `lolcatt-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/Makefile` & `lolcatt-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/_build/html/_static/basic.css` & `lolcatt-0.2.1/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/_build/html/_static/nature.css` & `lolcatt-0.2.1/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/_build/html/_static/pygments.css` & `lolcatt-0.2.1/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/_build/html/_static/screenshot.png` & `lolcatt-0.2.1/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/_static/screenshot.png` & `lolcatt-0.2.1/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/conf.py` & `lolcatt-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/installation.rst` & `lolcatt-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/lolcatt.rst` & `lolcatt-0.2.1/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/lolcatt.ui.rst` & `lolcatt-0.2.1/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/docs/make.bat` & `lolcatt-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/app.py` & `lolcatt-0.2.1/lolcatt/app.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/casting/caster.py` & `lolcatt-0.2.1/lolcatt/casting/caster.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -230,24 +230,24 @@
         self._loading_started = time.time()
         self._is_loading_cast = True
 
     def _tick(self):
         """
         Internal method that is called on every call to update the CastState.
         """
+        if self._device is None:
+            return
+
         if (
             self._autoplay
             and self._device.controller.info.get('idle_reason') == 'FINISHED'
             and len(self._queue) > 0
         ):
             self.cast_next()
 
-        if self._device is None:
-            return
-
         if time.time() - self._state_last_updated > self._update_interval:
             self._device.controller._update_status()
             self._state_last_updated = time.time()
 
         if self._is_loading_cast and time.time() - self._loading_started > self._loading_timeout:
             self._loading_started = None
             self._is_loading_cast = False
```

### Comparing `lolcatt-0.2.0/lolcatt/casting/youtube_playlist_handler.py` & `lolcatt-0.2.1/lolcatt/casting/youtube_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/cli.py` & `lolcatt-0.2.1/lolcatt/cli.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/ui/lolcatt.css` & `lolcatt-0.2.1/lolcatt/ui/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.2.1/lolcatt/ui/lolcatt_controls.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,58 +74,64 @@
 
     @on(Button.Pressed, "#play_pause_button")
     def toggle_play_pause(self):
         try:
             self.app.caster.get_device().controller.play_toggle()
             self._pp_button.styles.border_bottom = ('tall', self._pp_button_colors[-1])
             self._pp_button_colors.reverse()
-        except ValueError:
+        except (ValueError, AttributeError):
             pass
 
     @on(Button.Pressed, "#stop_button")
     def stop(self):
         if self.app.caster.get_cast_state().cast_info.get('player_state') in ['PLAYING', 'PAUSED']:
             self.app.caster.stop_cast()
         else:
             self.app.exit()
 
     @on(Button.Pressed, "#vol_down_button")
     def vol_down(self):
-        self.app.caster.get_device().volumedown(self._config.vol_step)
+        try:
+            self.app.caster.get_device().volumedown(self._config.vol_step)
+        except (CastError, AttributeError):
+            pass
 
     @on(Button.Pressed, "#vol_up_button")
     def vol_up(self):
-        self.app.caster.get_device().volumeup(self._config.vol_step)
+        try:
+            self.app.caster.get_device().volumeup(self._config.vol_step)
+        except (CastError, AttributeError):
+            pass
 
     @on(Button.Pressed, "#ffwd_button")
     def ffwd(self):
         try:
             self.app.caster.get_device().ffwd(self._config.ffwd_secs)
-        except CastError:
+        except (CastError, AttributeError):
             pass
 
     @on(Button.Pressed, "#rewind_button")
     def rewind(self):
         try:
             self.app.caster.get_device().rewind(self._config.rewind_secs)
-        except CastError:
+        except (CastError, AttributeError):
             pass
 
     @on(Button.Pressed, '#next_button')
     def next(self):
         try:
             self.app.caster.cast_next()
-        except CastError:
+        except (CastError, AttributeError):
             pass
 
     @on(Button.Pressed, '#prev_button')
     def prev(self):
         try:
             self.app.caster.cast_previous()
-        except CastError:
+        except (CastError, AttributeError):
             pass
 
     def on_key(self, event: Key) -> None:
         if event.key == 'space':
             self.toggle_play_pause()
         elif event.key == ('q'):
             self.app.exit()
```

### Comparing `lolcatt-0.2.0/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.2.1/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.2.1/lolcatt/ui/lolcatt_playback_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.2.1/lolcatt/ui/lolcatt_progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,12 +59,12 @@
             self.pb.content_region.x + self.pb.content_region.width,
         )
         click_x = min(max(event.screen_x, min_x), max_x)
         fraction = min(1, (click_x - min_x) / (max_x - min_x))
         duration = self.app.caster.get_cast_state().cast_info.get('duration', 0.0)
         try:
             self.app.caster.get_device().seek(duration * fraction)
-        except CastError:
+        except (CastError, AttributeError):
             pass
 
     def compose(self):
         yield Container(self.pb, self.pblabel, id='progress')
```

### Comparing `lolcatt-0.2.0/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.2.1/lolcatt/ui/lolcatt_url_input.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt/utils/utils.py` & `lolcatt-0.2.1/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.0/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.2.1/lolcatt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.0
+Version: 0.2.1
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.2.0/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.2.1/lolcatt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/nature.css
 docs/_build/html/_static/plus.png
 docs/_build/html/_static/pygments.css
 docs/_build/html/_static/screenshot.png
 docs/_static/custom.css
 docs/_static/screenshot.png
+lolcatt/.githash
 lolcatt/__init__.py
 lolcatt/app.py
 lolcatt/cli.py
 lolcatt.egg-info/PKG-INFO
 lolcatt.egg-info/SOURCES.txt
 lolcatt.egg-info/dependency_links.txt
 lolcatt.egg-info/entry_points.txt
```

### Comparing `lolcatt-0.2.0/pyproject.toml` & `lolcatt-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.2.0/setup.py` & `lolcatt-0.2.1/setup.py`

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
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```

