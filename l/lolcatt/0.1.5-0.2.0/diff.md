# Comparing `tmp/lolcatt-0.1.5.tar.gz` & `tmp/lolcatt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.1.5.tar", last modified: Sat Jul 15 16:24:39 2023, max compression
+gzip compressed data, was "lolcatt-0.2.0.tar", last modified: Sat Jul 15 23:52:37 2023, max compression
```

## Comparing `lolcatt-0.1.5.tar` & `lolcatt-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.1.5/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.1.5/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 16:24:39.580939 lolcatt-0.1.5/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-07 17:09:03.000000 lolcatt-0.1.5/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.576939 lolcatt-0.1.5/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.576939 lolcatt-0.1.5/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.576939 lolcatt-0.1.5/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 14:28:35.000000 lolcatt-0.1.5/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.5/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.5/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 14:28:35.000000 lolcatt-0.1.5/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.5/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 14:28:35.000000 lolcatt-0.1.5/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.1.5/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 14:28:33.000000 lolcatt-0.1.5/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 14:28:33.000000 lolcatt-0.1.5/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-15 16:24:08.000000 lolcatt-0.1.5/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1288 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.5/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5421 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1079 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.5/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1480 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3861 2023-07-15 16:19:23.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2646 2023-07-15 14:07:42.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      894 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.1.5/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-07 17:09:03.000000 lolcatt-0.1.5/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1236 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-15 16:24:08.000000 lolcatt-0.1.5/pyproject.toml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-15 16:24:39.584939 lolcatt-0.1.5/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-15 16:24:08.000000 lolcatt-0.1.5/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.1.5/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.1.5/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.0/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.0/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-15 23:52:37.751730 lolcatt-0.2.0/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2875 2023-07-15 23:28:47.000000 lolcatt-0.2.0/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.743730 lolcatt-0.2.0/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.743730 lolcatt-0.2.0/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 23:27:13.000000 lolcatt-0.2.0/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 23:27:13.000000 lolcatt-0.2.0/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 23:27:13.000000 lolcatt-0.2.0/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.0/docs/_build/html/_static/screenshot.png
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-15 23:26:41.000000 lolcatt-0.2.0/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.0/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.0/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 23:27:11.000000 lolcatt-0.2.0/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.0/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.0/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 23:27:11.000000 lolcatt-0.2.0/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.0/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-15 23:49:49.000000 lolcatt-0.2.0/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-15 23:33:36.000000 lolcatt-0.2.0/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.0/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     9247 2023-07-15 22:10:13.000000 lolcatt-0.2.0/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-15 22:39:08.000000 lolcatt-0.2.0/lolcatt/casting/youtube_playlist_handler.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1694 2023-07-15 22:09:07.000000 lolcatt-0.2.0/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.0/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-15 23:33:36.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4614 2023-07-15 23:44:24.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 16:19:10.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2646 2023-07-15 14:07:42.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      991 2023-07-15 22:09:07.000000 lolcatt-0.2.0/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.0/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1752 2023-07-15 23:09:49.000000 lolcatt-0.2.0/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.747730 lolcatt-0.2.0/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3554 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1280 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       54 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-15 23:52:37.000000 lolcatt-0.2.0/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-15 23:49:49.000000 lolcatt-0.2.0/pyproject.toml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-15 23:52:37.751730 lolcatt-0.2.0/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-15 23:49:49.000000 lolcatt-0.2.0/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 23:52:37.751730 lolcatt-0.2.0/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.0/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.0/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.1.5/LICENSE` & `lolcatt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/Makefile` & `lolcatt-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/_build/html/_static/basic.css` & `lolcatt-0.2.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/_build/html/_static/nature.css` & `lolcatt-0.2.0/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/_build/html/_static/pygments.css` & `lolcatt-0.2.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/conf.py` & `lolcatt-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/installation.rst` & `lolcatt-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/lolcatt.rst` & `lolcatt-0.2.0/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/lolcatt.ui.rst` & `lolcatt-0.2.0/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/docs/make.bat` & `lolcatt-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/lolcatt/app.py` & `lolcatt-0.2.0/lolcatt/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Dict
+
 from textual.app import App
 from textual.containers import Container
 from textual.screen import Screen
 
 from lolcatt.casting.caster import Caster
 from lolcatt.ui.lolcatt_controls import LolCattControls
 from lolcatt.ui.lolcatt_device_info import LolCattDeviceInfo
@@ -25,16 +27,17 @@
 
 
 class LolCatt(App):
     """The main application class for lolcatt."""
 
     CSS_PATH = 'ui/lolcatt.css'
 
-    def __init__(self, device_name: str = None, *args, **kwargs):
-        self.caster = Caster(device_name)
+    def __init__(self, device_name: str = None, config: Dict = None, *args, **kwargs):
+        self.config = config
+        self.caster = Caster(device_name, config=config)
         self.remote_screen = None
         super().__init__(*args, **kwargs)
 
     def on_mount(self):
         self.remote_screen = RemoteScreen()
         self.install_screen(self.remote_screen, name='remote')
         self.push_screen('remote')
```

### Comparing `lolcatt-0.1.5/lolcatt/ui/lolcatt.css` & `lolcatt-0.2.0/lolcatt/ui/lolcatt.css`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,25 @@
     align: center middle;
 }
 
 Button {
     color: white;
     background: $background-lighten-2;
     border-bottom: tall $accent;
-    min-width: 14;
+    min-width: 15;
     margin-left: 1;
 }
 
+#prev_button,
+#rewind_button,
+#ffwd_button,
+#next_button {
+    min-width: 7;
+}
+
 #play_pause_button {
     border-bottom: tall $success;
 }
 
 #stop_button {
     border-bottom: tall $error;
 }
@@ -27,14 +34,15 @@
 #volume_buttons,
 #playback_buttons,
 #wind_buttons {
     layout: horizontal;
     align: center middle;
     height: 3;
     width: 32;
+    min-width: 14;
     margin-top: 1;
 }
 
 #controls {
     layout: vertical;
     align: center top;
     width: 100%;
```

### Comparing `lolcatt-0.1.5/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.2.0/lolcatt/ui/lolcatt_controls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 from dataclasses import dataclass
 
-from catt.cli import get_config_as_dict
 from catt.error import CastError
 from textual import on
 from textual.app import DEFAULT_COLORS
 from textual.containers import Container
 from textual.events import Key
 from textual.widgets import Button
 from textual.widgets import Static
 
 
 @dataclass
 class ControlsConfig:
     ffwd_secs: int = 30
     rewind_secs: int = 10
     vol_step: float = 0.1
-    use_utf8: bool = False
+    fancy_icons: bool = False
 
 
 class LolCattControls(Static):
     CONTROLS = {
-        'play_pause': '⏯',
-        'stop': '⏹',
-        'rewind': '⏪',
-        'ffwd': '⏩',
+        'play_pause': '',
+        'stop': '',
+        'previous': '',
+        'rewind': '',
+        'ffwd': '',
+        'next': '',
         'vol_down': '',
         'vol_up': '',
     }
 
     CONTROLS_ASCII = {
         'play_pause': 'Play/Pause',
         'stop': 'Stop',
-        'rewind': 'RW',
-        'ffwd': 'FW',
+        'previous': '|<',
+        'rewind': '<<',
+        'ffwd': '>>',
+        'next': '>|',
         'vol_down': 'Vol-',
         'vol_up': 'Vol+',
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._config = ControlsConfig(
-            use_utf8=get_config_as_dict()['options'].get('lolcatt_use_utf8', 'false').lower()
-            == 'true'
+            fancy_icons=self.app.config['options'].get('fancy_icons', False)
         )
         self._pp_button_colors = [DEFAULT_COLORS['dark'].success, DEFAULT_COLORS['dark'].warning]
         self._pp_button = Button(self._get_control_label('play_pause'), id='play_pause_button')
         self._pp_button.styles.border_bottom = ('tall', self._pp_button_colors[0])
         self._stop_button = Button(self._get_control_label('stop'), id='stop_button')
 
     def _get_control_label(self, control: str) -> str:
-        if self._config.use_utf8:
+        if self._config.fancy_icons:
             return self.CONTROLS[control]
         else:
             return self.CONTROLS_ASCII[control]
 
     def compose(self):
         with Container(id='controls'):
             with Container(id='playback_buttons'):
                 yield self._pp_button
                 yield self._stop_button
 
             with Container(id='wind_buttons'):
+                yield Button(self._get_control_label('previous'), id='prev_button')
                 yield Button(self._get_control_label('rewind'), id='rewind_button')
                 yield Button(self._get_control_label('ffwd'), id='ffwd_button')
+                yield Button(self._get_control_label('next'), id='next_button')
 
             with Container(id='volume_buttons'):
                 yield Button(self._get_control_label('vol_down'), id='vol_down_button')
                 yield Button(self._get_control_label('vol_up'), id='vol_up_button')
 
     @on(Button.Pressed, "#play_pause_button")
     def toggle_play_pause(self):
@@ -76,15 +80,15 @@
             self._pp_button_colors.reverse()
         except ValueError:
             pass
 
     @on(Button.Pressed, "#stop_button")
     def stop(self):
         if self.app.caster.get_cast_state().cast_info.get('player_state') in ['PLAYING', 'PAUSED']:
-            self.app.caster.get_device().stop()
+            self.app.caster.stop_cast()
         else:
             self.app.exit()
 
     @on(Button.Pressed, "#vol_down_button")
     def vol_down(self):
         self.app.caster.get_device().volumedown(self._config.vol_step)
 
@@ -102,18 +106,40 @@
     @on(Button.Pressed, "#rewind_button")
     def rewind(self):
         try:
             self.app.caster.get_device().rewind(self._config.rewind_secs)
         except CastError:
             pass
 
+    @on(Button.Pressed, '#next_button')
+    def next(self):
+        try:
+            self.app.caster.cast_next()
+        except CastError:
+            pass
+
+    @on(Button.Pressed, '#prev_button')
+    def prev(self):
+        try:
+            self.app.caster.cast_previous()
+        except CastError:
+            pass
+
     def on_key(self, event: Key) -> None:
         if event.key == 'space':
             self.toggle_play_pause()
         elif event.key == ('q'):
             self.app.exit()
         elif event.key in ('h', 'left'):
             self.rewind()
         elif event.key in ('l', 'right'):
             self.ffwd()
+        elif event.key in ('j', 'down'):
+            self.next()
+        elif event.key in ('k', 'up'):
+            self.prev()
+        elif event.key == 'plus':
+            self.vol_up()
+        elif event.key == 'minus':
+            self.vol_down()
         else:
             pass
```

### Comparing `lolcatt-0.1.5/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.2.0/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.2.0/lolcatt/ui/lolcatt_playback_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.2.0/lolcatt/ui/lolcatt_progress.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.5/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.2.0/lolcatt/ui/lolcatt_url_input.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,17 @@
         self._input.cursor_blink = False
 
     @on(Input.Submitted, "#url_input")
     def cast_url(self):
         if self._input.value == '':
             return
         if self._input.value:
-            self.app.caster.cast(self._input.value)
+            self.app.caster.enqueue(self._input.value, front=True)
+            print(self.app.caster._queue)
+            self.app.caster.cast_next()
             self._input.value = ''
 
     def compose(self):
         yield Container(self._input, id='url_input_container')
 
     def on_key(self, event: Key):
         if event.key == 'escape':
```

### Comparing `lolcatt-0.1.5/lolcatt/utils/utils.py` & `lolcatt-0.2.0/lolcatt/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+from pathlib import Path
+
 from catt.api import discover
 
 
 def marquee(s: str, max_len: int, step_size: int) -> str:
     """
     Yields a string that is max_len characters long, and shifts the string by step_size each time.
 
@@ -37,7 +39,15 @@
     deduped = sorted(deduped, key=lambda x: x[1])
 
     print('Found {} device(s):'.format(len(found_ips)))
     print(f'Device name{" " * (max_name_len - 11)}\tDevice IP')
     print('=' * (max_name_len + 19))
     for name, ip in deduped:
         print(f'{name}\t{ip}')
+
+
+def write_initial_config(p: Path):
+    p.write_text(
+        "[options]\n"
+        "fancy_icons = true  # Whether to use fancy icons\n"
+        "#youtube_cookies_file = \"~/.config/lolcatt/cookies.txt\"  # Path to a cookies.txt file for YouTube"
+    )
```

### Comparing `lolcatt-0.1.5/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.2.0/lolcatt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 lolcatt.egg-info/dependency_links.txt
 lolcatt.egg-info/entry_points.txt
 lolcatt.egg-info/not-zip-safe
 lolcatt.egg-info/requires.txt
 lolcatt.egg-info/top_level.txt
 lolcatt/casting/__init__.py
 lolcatt/casting/caster.py
+lolcatt/casting/youtube_playlist_handler.py
 lolcatt/ui/__init__.py
 lolcatt/ui/lolcatt.css
 lolcatt/ui/lolcatt_controls.py
 lolcatt/ui/lolcatt_device_info.py
 lolcatt/ui/lolcatt_playback_info.py
 lolcatt/ui/lolcatt_progress.py
 lolcatt/ui/lolcatt_url_input.py
```

### Comparing `lolcatt-0.1.5/pyproject.toml` & `lolcatt-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.1.5"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.1.5/setup.py` & `lolcatt-0.2.0/setup.py`

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
-    version='0.1.5',
+    version='0.2.0',
     zip_safe=False,
 )
```

