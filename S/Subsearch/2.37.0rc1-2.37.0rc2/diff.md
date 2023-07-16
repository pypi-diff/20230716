# Comparing `tmp/Subsearch-2.37.0rc1.tar.gz` & `tmp/Subsearch-2.37.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.37.0rc1.tar", last modified: Sun Jul 16 03:08:31 2023, max compression
+gzip compressed data, was "Subsearch-2.37.0rc2.tar", last modified: Sun Jul 16 03:35:22 2023, max compression
```

## Comparing `Subsearch-2.37.0rc1.tar` & `Subsearch-2.37.0rc2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.586747 Subsearch-2.37.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/data_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/gui_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resource_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/spritesheet.png
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/sprites.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screen_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/screens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/language_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/search_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/subsearch_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/system_tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/app_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.120061 Subsearch-2.37.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-16 03:35:22.120061 Subsearch-2.37.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 03:35:22.120061 Subsearch-2.37.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.104061 Subsearch-2.37.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.108061 Subsearch-2.37.0rc2/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-16 03:35:22.000000 Subsearch-2.37.0rc2/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-16 03:35:22.000000 Subsearch-2.37.0rc2/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:35:22.000000 Subsearch-2.37.0rc2/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 03:35:22.000000 Subsearch-2.37.0rc2/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:35:21.000000 Subsearch-2.37.0rc2/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-16 03:35:22.000000 Subsearch-2.37.0rc2/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 03:35:22.000000 Subsearch-2.37.0rc2/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.108061 Subsearch-2.37.0rc2/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.112061 Subsearch-2.37.0rc2/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/data/data_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.112061 Subsearch-2.37.0rc2/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/gui_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resource_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.112061 Subsearch-2.37.0rc2/src/subsearch/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.112061 Subsearch-2.37.0rc2/src/subsearch/gui/resources/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/assets/spritesheet.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/assets/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.112061 Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/sprites.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/style_subsearch.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/theme_setter.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/screen_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.116061 Subsearch-2.37.0rc2/src/subsearch/gui/screens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/screens/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/screens/language_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/screens/search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/screens/subsearch_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/gui/system_tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.116061 Subsearch-2.37.0rc2/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:35:22.120061 Subsearch-2.37.0rc2/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/app_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-16 03:35:05.000000 Subsearch-2.37.0rc2/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.37.0rc1/LICENSE` & `Subsearch-2.37.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/PKG-INFO` & `Subsearch-2.37.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.37.0rc1
+Version: 2.37.0rc2
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.37.0rc1/README.md` & `Subsearch-2.37.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/pyproject.toml` & `Subsearch-2.37.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/setup.py` & `Subsearch-2.37.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.37.0rc2/src/Subsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.37.0rc1
+Version: 2.37.0rc2
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.37.0rc1/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.37.0rc2/src/Subsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/__init__.py` & `Subsearch-2.37.0rc2/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/core.py` & `Subsearch-2.37.0rc2/src/subsearch/core.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/data/data_initializer.py` & `Subsearch-2.37.0rc2/src/subsearch/data/data_initializer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/data/data_objects.py` & `Subsearch-2.37.0rc2/src/subsearch/data/data_objects.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/data/languages.json` & `Subsearch-2.37.0rc2/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/__init__.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/gui_toolkit.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/gui_toolkit.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/resource_loader.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/resource_loader.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/spritesheet.png` & `Subsearch-2.37.0rc2/src/subsearch/gui/resources/assets/spritesheet.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/subsearch.ico` & `Subsearch-2.37.0rc2/src/subsearch/gui/resources/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/resources/config.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/resources/config.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/sprites.tcl` & `Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/sprites.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl` & `Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/style_subsearch.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl` & `Subsearch-2.37.0rc2/src/subsearch/gui/resources/styles/theme_setter.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/screen_manager.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/screen_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/screens/download_manager.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/screens/download_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/screens/language_options.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/screens/language_options.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/screens/search_filters.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/screens/search_filters.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/screens/subsearch_options.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/screens/subsearch_options.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/gui/system_tray.py` & `Subsearch-2.37.0rc2/src/subsearch/gui/system_tray.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/providers/generic.py` & `Subsearch-2.37.0rc2/src/subsearch/providers/generic.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.37.0rc2/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/providers/subscene.py` & `Subsearch-2.37.0rc2/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.37.0rc2/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/app_integrity.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/app_integrity.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/exceptions.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/file_manager.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/io_json.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/io_json.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/io_winreg.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/log.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/log.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/mutex_synchronizer.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/mutex_synchronizer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/state_machine.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/state_machine.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/string_parser.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.0rc1/src/subsearch/utils/update.py` & `Subsearch-2.37.0rc2/src/subsearch/utils/update.py`

 * *Files identical despite different names*

