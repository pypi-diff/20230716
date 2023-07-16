# Comparing `tmp/Subsearch-2.36.4.tar.gz` & `tmp/Subsearch-2.37.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.36.4.tar", last modified: Sat Jul  8 22:38:11 2023, max compression
+gzip compressed data, was "Subsearch-2.37.0rc1.tar", last modified: Sun Jul 16 03:08:31 2023, max compression
```

## Comparing `Subsearch-2.36.4.tar` & `Subsearch-2.37.0rc1.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.017771 Subsearch-2.36.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 22:37:53.000000 Subsearch-2.36.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-08 22:37:53.000000 Subsearch-2.36.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-08 22:38:11.017771 Subsearch-2.36.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-08 22:37:53.000000 Subsearch-2.36.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-08 22:37:53.000000 Subsearch-2.36.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:38:11.017771 Subsearch-2.36.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-08 22:37:53.000000 Subsearch-2.36.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.005771 Subsearch-2.36.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.009771 Subsearch-2.36.4/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-08 22:38:10.000000 Subsearch-2.36.4/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-08 22:38:11.000000 Subsearch-2.36.4/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:38:10.000000 Subsearch-2.36.4/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 22:38:10.000000 Subsearch-2.36.4/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:38:10.000000 Subsearch-2.36.4/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-08 22:38:10.000000 Subsearch-2.36.4/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 22:38:10.000000 Subsearch-2.36.4/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.009771 Subsearch-2.36.4/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.013771 Subsearch-2.36.4/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/data/data_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.013771 Subsearch-2.36.4/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.013771 Subsearch-2.36.4/src/subsearch/gui/app_theme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/app_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/app_theme/spritesheet_data.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.013771 Subsearch-2.36.4/src/subsearch/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/assets/spritesheet.png
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/assets/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/gui_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.013771 Subsearch-2.36.4/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/gui/tabs/settings_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.017771 Subsearch-2.36.4/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:38:11.017771 Subsearch-2.36.4/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/app_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-08 22:37:53.000000 Subsearch-2.36.4/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.586747 Subsearch-2.37.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 03:08:31.000000 Subsearch-2.37.0rc1/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/data_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/gui_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resource_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/spritesheet.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/sprites.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screen_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.590746 Subsearch-2.37.0rc1/src/subsearch/gui/screens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/language_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/screens/subsearch_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/gui/system_tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:08:31.594746 Subsearch-2.37.0rc1/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/app_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-16 03:08:13.000000 Subsearch-2.37.0rc1/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.36.4/LICENSE` & `Subsearch-2.37.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/PKG-INFO` & `Subsearch-2.37.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.36.4
+Version: 2.37.0rc1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
@@ -83,21 +83,21 @@
 <div align="center">
 
 ![prtsc_example](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/example.gif)
 
 <details>
 <summary>Screenshots of the interface</summary>
 
-![prtsc_language](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_language.png)
+![prtsc_language](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/language_options.png)
 
-![prtsc_search](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_search.png)
+![prtsc_search](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/search_filters.png)
 
-![prtsc_settings](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_settings.png)
+![prtsc_settings](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/subsearch_options.png)
 
-![prtsc_download](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/gui_download.png)
+![prtsc_download](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/download_manager.png)
 
 </details>
 
 </div>
 
 ## Getting Started <a name = "getting_started_src"></a>
```

### Comparing `Subsearch-2.36.4/README.md` & `Subsearch-2.37.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 <div align="center">
 
 ![prtsc_example](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/example.gif)
 
 <details>
 <summary>Screenshots of the interface</summary>
 
-![prtsc_language](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_language.png)
+![prtsc_language](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/language_options.png)
 
-![prtsc_search](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_search.png)
+![prtsc_search](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/search_filters.png)
 
-![prtsc_settings](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_settings.png)
+![prtsc_settings](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/subsearch_options.png)
 
-![prtsc_download](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/gui_download.png)
+![prtsc_download](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/download_manager.png)
 
 </details>
 
 </div>
 
 ## Getting Started <a name = "getting_started_src"></a>
```

### Comparing `Subsearch-2.36.4/pyproject.toml` & `Subsearch-2.37.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop"
 ]
-dependencies = ["selectolax==0.3.14", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.31.0", "pillow==9.5.0"]
+dependencies = ["selectolax==0.3.14", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.31.0", "pillow==10.0.0", "pystray==0.19.4"]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/vagabondHustler/subsearch"
 
 [project.scripts]
 subsearch = "subsearch:main"
@@ -40,15 +40,15 @@
 include = ["subsearch*"]
 exclude = ["examples*", "tools*", "subsearch.test*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "subsearch.data.__version__"}
 
 [project.optional-dependencies]
-optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.15.2", "mypy==1.4.1", "pipreqs==0.4.13"]
+optional = ["black==23.7.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.15.3", "mypy==1.4.1", "pipreqs==0.4.13"]
 dev = ["pytest==7.4.0", "pytest-cov==4.1.0", "tox==4.6.4"]
 
 
 [tool.pytest.ini_options]
 filterwarnings =[
     'ignore::DeprecationWarning'
 ]
```

### Comparing `Subsearch-2.36.4/setup.py` & `Subsearch-2.37.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from importlib import util
 
 
+
 def _cx_freeze():
     """
     Builds an executable and MSI installer using cx_Freeze.
 
     """
     import os
     import sys
 
     from cx_Freeze import Executable, setup
 
     from subsearch.data import __guid__
 
     sys.path.insert(0, os.path.abspath(os.path.dirname(__file__)))
 
-    icon = "src/subsearch/gui/assets/subsearch.ico"
+    icon = "src/subsearch/gui/resources/assets/subsearch.ico"
     app_name = "Subsearch"
     registry_path = rf"Software\Classes\*\shell\Subsearch"
     script_component = "_cx_executable0__Executable_script_src_subsearch___main__.py_"
     subsearch_key = (f"{app_name}_key", -1, registry_path, None, None, script_component)
     subsearch_icon = (f"{app_name}_regz_icon", -1, registry_path, "Icon", None, script_component)
     subsearch_appliesto = (f"{app_name}_regz_appliesto", -1, registry_path, "AppliesTo", None, script_component)
     subsearch_command = (f"{app_name}_key_command", -1, rf"{registry_path}\command", None, "", script_component)
```

### Comparing `Subsearch-2.36.4/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.37.0rc1/src/Subsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.36.4
+Version: 2.37.0rc1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
@@ -83,21 +83,21 @@
 <div align="center">
 
 ![prtsc_example](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/example.gif)
 
 <details>
 <summary>Screenshots of the interface</summary>
 
-![prtsc_language](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_language.png)
+![prtsc_language](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/language_options.png)
 
-![prtsc_search](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_search.png)
+![prtsc_search](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/search_filters.png)
 
-![prtsc_settings](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/gui_settings.png)
+![prtsc_settings](https://raw.githubusercontent.com/vagabondHustler/subsearch/main/assets/subsearch_options.png)
 
-![prtsc_download](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/gui_download.png)
+![prtsc_download](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/download_manager.png)
 
 </details>
 
 </div>
 
 ## Getting Started <a name = "getting_started_src"></a>
```

### Comparing `Subsearch-2.36.4/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.37.0rc1/src/Subsearch.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 src/subsearch/data/data_initializer.py
 src/subsearch/data/data_objects.py
 src/subsearch/data/guid.py
 src/subsearch/data/languages.json
 src/subsearch/data/version.py
 src/subsearch/gui/__init__.py
 src/subsearch/gui/gui_toolkit.py
-src/subsearch/gui/tab_manager.py
-src/subsearch/gui/app_theme/__init__.py
-src/subsearch/gui/app_theme/spritesheet_data.tcl
-src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl
-src/subsearch/gui/app_theme/ttk_theme_initializer.tcl
-src/subsearch/gui/assets/__init__.py
-src/subsearch/gui/assets/spritesheet.png
-src/subsearch/gui/assets/subsearch.ico
-src/subsearch/gui/tabs/__init__.py
-src/subsearch/gui/tabs/dowload_tab.py
-src/subsearch/gui/tabs/language_tab.py
-src/subsearch/gui/tabs/search_tab.py
-src/subsearch/gui/tabs/settings_tab.py
+src/subsearch/gui/resource_loader.py
+src/subsearch/gui/screen_manager.py
+src/subsearch/gui/system_tray.py
+src/subsearch/gui/resources/__init__.py
+src/subsearch/gui/resources/config.py
+src/subsearch/gui/resources/assets/__init__.py
+src/subsearch/gui/resources/assets/spritesheet.png
+src/subsearch/gui/resources/assets/subsearch.ico
+src/subsearch/gui/resources/styles/__init__.py
+src/subsearch/gui/resources/styles/sprites.tcl
+src/subsearch/gui/resources/styles/style_subsearch.tcl
+src/subsearch/gui/resources/styles/theme_setter.tcl
+src/subsearch/gui/screens/__init__.py
+src/subsearch/gui/screens/download_manager.py
+src/subsearch/gui/screens/language_options.py
+src/subsearch/gui/screens/search_filters.py
+src/subsearch/gui/screens/subsearch_options.py
 src/subsearch/providers/__init__.py
 src/subsearch/providers/generic.py
 src/subsearch/providers/opensubtitles.py
 src/subsearch/providers/subscene.py
 src/subsearch/providers/yifysubtitles.py
 src/subsearch/utils/__init__.py
 src/subsearch/utils/app_integrity.py
```

### Comparing `Subsearch-2.36.4/src/subsearch/__init__.py` & `Subsearch-2.37.0rc1/src/subsearch/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from pathlib import Path
 from threading import Thread
 
 from subsearch import core
 from subsearch.data import __guid__
-from subsearch.gui import tab_manager
+from subsearch.gui import screen_manager
 from subsearch.utils import io_json, io_winreg, mutex_synchronizer
 
 PACKAGEPATH = Path(__file__).resolve().parent.as_posix()
 HOMEPATH = Path(PACKAGEPATH).parent.as_posix()
 sys.path.append(HOMEPATH)
 sys.path.append(PACKAGEPATH)
 
@@ -72,54 +72,54 @@
         Download zip files containing the .srt files, extract, rename and clean up tmp files
         """
         self._download_files()
         self._not_downloaded()
         self._extract_zip_files()
         self._clean_up()
 
-    def pre_exit(self) -> None:
+    def on_exit(self) -> None:
         """
         Stop pref counter, log elapsed time and keep the terminal open if show_terminal is True
         """
-        self._pre_exit()
+        self._on_exit()
 
 
 def console() -> None:
     r"""
     Usages: subsearch [OPTIONS]
 
     Options:
         --settings [lang, search, app, dl]      Open the GUI settings menu
-                                                    ang: opens tab with available languages
-                                                    search: opens tab with settings such as available providers
-                                                    app: opens tab with app settings
-                                                    dl: opens tab for subtitles not downloaded
+                                                    ang: opens screen with available languages
+                                                    search: opens screen with settings such as available providers
+                                                    app: opens screen with app settings
+                                                    dl: opens screen for subtitles not downloaded
 
         --registry-key [add, del]               Edit the registry
                                                     add: adds the context menu  / replaces the context menu with default values
                                                     del: deletes the context menu
                                                     e.g: subsearch --registry-key add
 
         --help                                  Prints usage information
     """
 
     for num, arg in enumerate(sys.argv[1:], 1):
         if arg.startswith("--settings"):
             if sys.argv[num + 1] == "lang":
                 sys.argv.pop(num), sys.argv.pop(num)
-                tab_manager.open_tab("language")
+                screen_manager.open_screen("language")
             elif sys.argv[num + 1] == "search":
                 sys.argv.pop(num), sys.argv.pop(num)
-                tab_manager.open_tab("search")
+                screen_manager.open_screen("search")
             elif sys.argv[num + 1] == "app":
                 sys.argv.pop(num), sys.argv.pop(num)
-                tab_manager.open_tab("settings")
+                screen_manager.open_screen("settings")
             elif sys.argv[num + 1] == "dl":
                 sys.argv.pop(num), sys.argv.pop(num)
-                tab_manager.open_tab("download")
+                screen_manager.open_screen("download")
 
             break
         elif arg.startswith("--registry-key") or arg.startswith("--add-key"):
             if sys.argv[num + 1] == "add":
                 sys.argv.pop(num), sys.argv.pop(num)
                 io_winreg.add_context_menu()
                 break
@@ -142,12 +142,12 @@
         if i.startswith("--"):
             console()
             return None
 
     app = Subsearch()
     app.search_for_subtitles()
     app.process_files()
-    app.pre_exit()
+    app.on_exit()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `Subsearch-2.36.4/src/subsearch/core.py` & `Subsearch-2.37.0rc1/src/subsearch/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import ctypes
 import time
 
 from subsearch.data import __version__, app_paths, video_data
 from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
-from subsearch.gui import tab_manager
+from subsearch.gui import screen_manager, system_tray
 from subsearch.providers import opensubtitles, subscene, yifysubtitles
-from subsearch.utils import (
-    app_integrity,
-    file_manager,
-    io_json,
-    log,
-    state_machine,
-    string_parser,
-)
+from subsearch.utils import app_integrity, file_manager, io_json, log, string_parser
 
 
-class Initializer(state_machine.CoreState):
+class Initializer:
     def __init__(self) -> None:
-        state_machine.CoreState.__create__(self.unknown)
-        self.set_state(self.initializing)
         app_integrity.initialize_application()
         self.app_config = io_json.get_app_config()
+        system_tray.enable_system_tray = self.app_config.system_tray
+        self.system_tray = system_tray.SystemTray()
+        self.system_tray.start()
+        self.system_tray.update_progress_state()
         if video_data is not None:
+            self.file_exist = True
             file_manager.create_directory(video_data.subs_directory)
             self.file_hash = file_manager.get_hash(video_data.file_path)
         else:
-            self.set_state(self.no_file_found)
+            self.system_tray.lock_to_state("no_file")
+            self.file_exist = False
             self.file_hash = ""
         self.results: dict[str, list[DownloadData]] = {}
         self.skipped_downloads: dict[str, list[PrettifiedDownloadData]] = {}
         self.skipped_combined: list[PrettifiedDownloadData] = []
         self.downloads: dict[str, int] = {}
         self.language_data = io_json.get_language_data()
 
@@ -51,15 +48,15 @@
                 release_data=self.release_data,
                 app_config=self.app_config,
                 provider_urls=self.provider_urls,
                 language_data=self.language_data,
             )
             log.set_logger_data(**self.search_kwargs)
             log.output_parameters()
-            self.set_state(self.initialized)
+            self.system_tray.update_progress_state()
 
     def all_providers_disabled(self) -> bool:
         self.app_config = io_json.get_app_config()
         if (
             self.app_config.providers["subscene_site"] is False
             and self.app_config.providers["opensubtitles_site"] is False
             and self.app_config.providers["opensubtitles_hash"] is False
@@ -76,54 +73,55 @@
 
 class AppSteps(Initializer):
     def __init__(self) -> None:
         self.start = time.perf_counter()
         Initializer.__init__(self)
         ctypes.windll.kernel32.SetConsoleTitleW(f"subsearch - {__version__}")
         if not self.file_exist:
-            tab_manager.open_tab("search")
+            self.system_tray.lock_to_state("gui")
+            screen_manager.open_screen("search_filters")
             return None
 
         if " " in video_data.filename:
             log.warning_spaces_in_filename()
         log.output_header("Search started")
 
     def _provider_opensubtitles(self) -> None:
+        self.system_tray.update_progress_state()
         if self.skip_step.opensubtitles():
             return None
-        self.set_state(self.scraping_opensubtitles)
         # log.output_header("Searching on opensubtitles")
         _opensubs = opensubtitles.OpenSubtitles(**self.search_kwargs)
         if self.app_config.providers["opensubtitles_hash"] and self.file_hash != "":
             self.results["opensubtitles_hash"] = _opensubs.parse_hash_results()
         if self.app_config.providers["opensubtitles_site"]:
             self.results["opensubtitles_site"] = _opensubs.parse_site_results()
         self.skipped_downloads["opensubtitles_site"] = _opensubs._sorted_list()
 
     def _provider_subscene(self) -> None:
+        self.system_tray.update_progress_state()
         if self.skip_step.subscene():
             return None
-        self.set_state(self.scraping_subscene)
         _subscene = subscene.Subscene(**self.search_kwargs)
         self.results["subscene_site"] = _subscene.parse_site_results()
         self.skipped_downloads["subscene_site"] = _subscene._sorted_list()
 
     def _provider_yifysubtitles(self) -> None:
+        self.system_tray.update_progress_state()
         if self.skip_step.yifysubtitles():
             return None
-        self.set_state(self.scraping_yifysubtitles)
         _yifysubs = yifysubtitles.YifiSubtitles(**self.search_kwargs)
         self.results["yifysubtitles_site"] = _yifysubs.parse_site_results()
         self.skipped_downloads["yifysubtitles_site"] = _yifysubs._sorted_list()
 
     def _download_files(self) -> None:
+        self.system_tray.update_progress_state()
         if self.skip_step.download_files():
             return None
         log.output_header(f"Downloading subtitles")
-        self.set_state(self.downloading_files)
         for provider, data in self.results.items():
             if self.app_config.providers[provider] is False:
                 continue
             if not data:
                 continue
             self.downloads[provider] = self.download_results(data)
         log.output_done_with_tasks(end_new_line=True)
@@ -134,47 +132,60 @@
         for data_list in self.skipped_downloads.values():
             if not data_list:
                 continue
             for data in data_list:
                 self.skipped_combined.append(data)
 
         if self.skipped_combined:
-            tab_manager.open_tab("download", data=self.skipped_combined)
+            screen_manager.open_screen("download_manager", data=self.skipped_combined)
             self.ran_download_tab = True
         log.output_done_with_tasks(end_new_line=True)
 
     def _extract_zip_files(self) -> None:
+        self.system_tray.update_progress_state()
         if self.skip_step.extract_zip():
             return None
-        self.set_state(self.extracting_files)
         log.output_header("Extracting downloads")
         file_manager.extract_files(app_paths.tmpdir, video_data.subs_directory, ".zip")
         log.output_done_with_tasks(end_new_line=True)
 
     def _clean_up(self) -> None:
+        self.system_tray.update_progress_state()
         if not self.file_exist:
             return None
-        self.set_state(self.cleaning_up)
         if self.app_config.rename_best_match:
             log.output_header("Renaming best match")
             file_manager.rename_best_match(f"{self.release_data.release}.srt", video_data.directory_path, ".srt")
             log.output_done_with_tasks(end_new_line=True)
 
         log.output_header("Cleaning up")
         file_manager.clean_up_files(video_data.subs_directory, "nfo")
         file_manager.delete_temp_files(app_paths.tmpdir)
         if file_manager.directory_is_empty(video_data.subs_directory):
             file_manager.del_directory(video_data.subs_directory)
         log.output_done_with_tasks(end_new_line=True)
 
-    def _pre_exit(self) -> None:
+    def _summary_toast(self, elapsed) -> None:
+        self.system_tray.update_progress_state()
+        if not self.file_exist or not self.app_config.toast_summary:
+            return None
+        elapsed_summary = f"Finished in {elapsed} seconds"
+        matches = len(self.results.items())
+        download_summary = f"Matches found {matches}"
+        self.system_tray.update_progress_state()
+        if matches > 0:
+            self.system_tray.toast_message(f"Search Succeeded", f"{download_summary}\n{elapsed_summary}")
+        elif matches == 0:
+            self.system_tray.toast_message(f"Search Failed", f"{download_summary}\n{elapsed_summary}")
+
+    def _on_exit(self) -> None:
         elapsed = time.perf_counter() - self.start
-        self.set_state(self.exiting)
+        self._summary_toast(elapsed)
         log.output(f"Finished in {elapsed} seconds")
-
+        self.system_tray.stop()
         if self.app_config.show_terminal is False:
             return None
         if file_manager.running_from_exe():
             return None
 
         try:
             input("Ctrl + c or Enter to exit")
```

### Comparing `Subsearch-2.36.4/src/subsearch/data/data_initializer.py` & `Subsearch-2.37.0rc1/src/subsearch/data/data_initializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         AppPaths: An instance of AppPaths representing the path configuration for Subsearch application.
     """
     home = Path(__file__).resolve().parent.parent
     return AppPaths(
         home=home,
         data=Path(home) / "data",
         gui=Path(home) / "gui",
-        gui_assets=Path(home) / "gui" / "assets",
-        gui_app_theme=Path(home) / "gui" / "app_theme",
+        gui_assets=Path(home) / "gui" / "resources" / "assets",
+        gui_styles=Path(home) / "gui" / "resources" / "styles",
         providers=Path(home) / "providers",
         utils=Path(home) / "utils",
         tmpdir=Path(tempfile.gettempdir()) / f"tmp_subsearch",
         appdata_local=Path.home() / "AppData" / "Local" / "Subsearch",
     )
```

### Comparing `Subsearch-2.36.4/src/subsearch/data/languages.json` & `Subsearch-2.37.0rc1/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/gui/__init__.py` & `Subsearch-2.37.0rc1/src/subsearch/gui/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import re
 from tkinter import Tk
 
 from subsearch.data import app_paths
 
 
-def get_spritesheet_data() -> dict:
+def get_sprites() -> dict:
     pattern = r"\b(\w+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\b"
     data = {}
-    file_path = app_paths.gui_app_theme / "spritesheet_data.tcl"
+    file_path = app_paths.gui_styles / "sprites.tcl"
     with file_path.open() as file:
         content = file.read()
         matches = re.findall(pattern, content)
 
         for match in matches:
             key = match[0]
             values = tuple(map(int, match[1:]))
             data[key] = values
 
     return data
 
 
 root = Tk(className="Subsearch")
-spritesheet_data = get_spritesheet_data()
+sprites = get_sprites()
```

### Comparing `Subsearch-2.36.4/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl` & `Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-source [file join [file dirname [info script]] spritesheet_data.tcl]
+source [file join [file dirname [info script]] sprites.tcl]
 
-namespace eval ttk_subsearch_theme {
-    package provide ttk::theme::ttk_subsearch_theme 0.1.0
+namespace eval style_subsearch {
+    package provide ttk::theme::style_subsearch 0.1.0
 
     # Load Images
     proc load_images {imgfile} {
         variable sprites
         image create photo spritesheet -file $imgfile -format png
         foreach {name x y width height} $::sprite_data {
             set sprites($name) [image create photo -width $width -height $height]
@@ -13,15 +13,15 @@
         }
     }
 
     load_images [file join [file dirname [file dirname [info script]]] assets spritesheet.png]
 
 
     # Theme Creation
-    ttk::style theme create ttk_subsearch_theme -parent clam -settings {
+    ttk::style theme create style_subsearch -parent clam -settings {
 
         # Color Settings
         array set colors {
             -fg             "#bdbdbd"
             -bg             "#1a1b1b"
             -disabledfg     "#595959"
             -selectfg       "#ffffff"
@@ -65,15 +65,15 @@
             }
         }
 
         # Button Configuration
         ttk::style configure TButton -padding {4 4} -anchor center -foreground $colors(-fg)
 
         ttk::style map TButton -foreground \
-            [list disabled #bdbdbd \
+            [list disabled #232323 \
                 pressed #4c4c4c]
 
         ttk::style element create Button.button image \
             [list $sprites(btn_rest) \
                 {selected disabled} $sprites(btn_disabled) \
                 disabled $sprites(btn_disabled) \
                 selected $sprites(btn_rest) \
@@ -119,9 +119,47 @@
                 alternate $sprites(check_tri_rest) \
                 {pressed selected} $sprites(check_hover) \
                 {active selected} $sprites(check_hover) \
                 selected $sprites(check_rest) \
                 {pressed !selected} $sprites(check_unsel_pressed) \
                 active $sprites(check_unsel_hover) \
             ] -width 26 -sticky w
+
+        ttk::style map TCheckbutton -foreground \
+            [list disabled #565656 \
+            ]
+        
+        # Card
+        ttk::style layout Card.TFrame {
+        Card.field {
+            Card.padding -expand 1 
+            }
+        }
+
+        ttk::style element create Card.field image $sprites(card) -border 0 -padding 4 -sticky nsew
+
+        # Labelframe
+        ttk::style layout TLabelframe {
+        Labelframe.border {
+            Labelframe.padding -expand 1 -children {
+            Labelframe.label -side left
+                }
+            }
+        
+        }
+        # Labelframe
+        ttk::style layout TLabelframePlain {
+        Labelframe.plain {
+            Labelframe.padding -expand 1 -children {
+            Labelframe.label -side left
+                }
+            }
+        
+        }
+
+        ttk::style element create Labelframe.border image $sprites(card) -border 5 -padding 4 -sticky nsew
+        ttk::style configure TLabelframe.border.Label -font "Cascadia 8 bold" -foreground $colors(-fg) -background $colors(-bg)
+        ttk::style configure TLabelframe.plain.Label -font "Cascadia 8 bold" -foreground $colors(-fg) -background $colors(-bg)
+
+
     }
 }
```

### Comparing `Subsearch-2.36.4/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl` & `Subsearch-2.37.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-source [file join [file dirname [info script]] ttk_subsearch_theme.tcl]
+source [file join [file dirname [info script]] style_subsearch.tcl]
 
 option add *tearOff 0
 
 proc set_theme {} {
     
-    ttk::style theme use "ttk_subsearch_theme"
+    ttk::style theme use "style_subsearch"
 
     array set colors {
-        -fg             "#ffffff"
-        -bg             "#1c1c1c"
+        -fg             "#bdbdbd"
+        -bg             "#1a1b1b"
         -disabledfg     "#59959"
         -selectfg       "#ffffff"
         -selectbg       "#2f60d8"
     }
     
     ttk::style configure . \
         -background $colors(-bg) \
```

### Comparing `Subsearch-2.36.4/src/subsearch/gui/assets/subsearch.ico` & `Subsearch-2.37.0rc1/src/subsearch/gui/resources/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/gui/gui_toolkit.py` & `Subsearch-2.37.0rc1/src/subsearch/gui/gui_toolkit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,23 @@
 import tkinter as tk
 from tkinter import Label, StringVar, ttk
 
-from PIL import Image, ImageTk
-
-from subsearch.data import __version__, app_paths, gui
-from subsearch.gui import spritesheet_data
+from subsearch.data import __version__, app_paths
+from subsearch.gui.resources import config as cfg
 from subsearch.utils import file_manager, io_json, io_winreg
 
 GWL_EXSTYLE = -20
 WS_EX_APPWINDOW = 0x00040000
 WS_EX_TOOLWINDOW = 0x00000080
 
-DEFAULT_LABEL_CONFIG = dict(bg=gui.colors.dark_grey, fg=gui.colors.white_grey, font=gui.fonts.cas8b)
+DEFAULT_LABEL_CONFIG = dict(bg=cfg.color.dark_grey, fg=cfg.color.white_grey, font=cfg.font.cas8b)
 DEFAULT_LABEL_GRID = dict(row=0, column=0, sticky="w", padx=2, pady=2)
 DEFAULT_BTN_TOGGLE_GRID = dict(row=0, column=2, pady=2)
 
 
-def get_sprite(sprite_name):
-    spritesheet_path = app_paths.gui_assets / "spritesheet.png"
-    spritesheet_image = Image.open(spritesheet_path)
-    sprite_x = spritesheet_data[sprite_name][0]
-    sprite_y = spritesheet_data[sprite_name][1]
-    sprite_width = spritesheet_data[sprite_name][2]
-    sprite_height = spritesheet_data[sprite_name][3]
-    sprite = spritesheet_image.crop((sprite_x, sprite_y, sprite_x + sprite_width, sprite_y + sprite_height))
-    return sprite
-
-
 def calculate_btn_size(cls, width_=18, height_=2) -> tuple[int, int]:
     """
     Calculate the required size of a button based on its content.
 
     Args:
         cls: The class from which the method is being called.
         width_ (optional): The initial width of the button before calculation. Defaults to 18.
@@ -78,65 +65,14 @@
     for col in range(col_count):
         cls.grid_columnconfigure(col, minsize=x)
 
     for row in range(row_count):
         cls.grid_rowconfigure(row, minsize=0)
 
 
-def asset_tab(cls, img, type, x=27, y=27) -> None:
-    """
-    Attach an image displayed as a tab onto the application window.
-
-    Args:
-        cls (class): The class representing the application.
-        img (str): The name of the image file.
-        type (str): The type of the image file.
-        x (int, optional): The width of the image in pixels. Defaults to 27.
-        y (int, optional): The height of the image in pixels. Defaults to 27.
-    """
-    path = get_sprite(f"{img}_{type}")
-    png = ImageTk.PhotoImage(path)
-    update_asset(cls, png, x, y)
-
-
-def update_asset(cls, img, x, y) -> None:
-    """
-    Updates an asset in a tkinter canvas with the provided image.
-
-    Args:
-        cls: The canvas instance that houses the current asset.
-        img: The image asset to replace the current asset within the canvas.
-        x: The X coordinate for positioning of the new asset.
-        y: The Y coordinate for positioning of the new asset.
-
-    Returns:
-        None
-    """
-
-    cls.delete("all")
-    cls.create_image(x, y, image=img)
-    cls.photoimage = img
-
-
-def set_custom_btn_styles() -> None:
-    """
-    Sets custom button styles
-
-    Args:
-        None
-
-    Returns:
-        None
-    """
-
-    custom_style = ttk.Style()
-    custom_style.configure("True.TButton", foreground=gui.colors.green)
-    custom_style.configure("False.TButton", foreground=gui.colors.red)
-
-
 class WindowPosition(tk.Frame):
     """
     A class that creates and manages the positioning of a tkinter frame.
 
     Args:
         parent: The parent widget.
 
@@ -160,16 +96,16 @@
         Args:
             parent: The parent widget.
         """
         tk.Frame.__init__(self, parent)
 
     def set(
         self,
-        w=gui.size.root_width,
-        h=gui.size.root_height,
+        w=cfg.size.width,
+        h=cfg.size.height,
         ws_value_offset=0,
         hs_value_offset=0,
         other: bool = False,
     ):
         """
         Set the size of the current window/Frame
 
@@ -216,32 +152,32 @@
         self.string_var = string_var
         self.clabel = clabel
         self.is_pct = is_pct
         self.pick()
 
     def pick(self) -> None:
         if self.string_var.get() == "True":
-            self.clabel.configure(fg=gui.colors.green)
+            self.clabel.configure(fg=cfg.color.green)
         elif self.string_var.get() == "False":
-            self.clabel.configure(fg=gui.colors.red)
+            self.clabel.configure(fg=cfg.color.red)
         elif self.string_var.get() == "Both":
-            self.clabel.configure(fg=gui.colors.blue)
+            self.clabel.configure(fg=cfg.color.blue)
         elif self.string_var.get().startswith("Only"):
-            self.clabel.configure(fg=gui.colors.green)
+            self.clabel.configure(fg=cfg.color.green)
 
         if self.is_pct:
             _pct = io_json.get_json_key("percentage_threshold")
             if _pct in range(75, 101):
-                self.clabel.configure(fg=gui.colors.green)
+                self.clabel.configure(fg=cfg.color.green)
             elif _pct in range(50, 75):
-                self.clabel.configure(fg=gui.colors.green_brown)
+                self.clabel.configure(fg=cfg.color.green_brown)
             elif _pct in range(25, 50):
-                self.clabel.configure(fg=gui.colors.red_brown)
+                self.clabel.configure(fg=cfg.color.red_brown)
             elif _pct in range(0, 25):
-                self.clabel.configure(fg=gui.colors.red)
+                self.clabel.configure(fg=cfg.color.red)
 
 
 class ToolTip(tk.Toplevel):
     """
     A toplevel widget that displays a message when the user hovers over a specified widget
 
     Args:
@@ -250,33 +186,33 @@
         *_text (str): The text to be displayed in the tooltip
         _background (str): The background color of the tooltip
 
     Methods:
         show(): Creates and displays a toplevel widget containing the text to be displayed in the tooltip
     """
 
-    def __init__(self, parent, _widget, *_text, _background=gui.colors.light_black):
+    def __init__(self, parent, _widget, *_text, _background=cfg.color.light_black):
         self.parent = parent
         self.widget = _widget
         self.text = _text
         self.background = _background
 
     def show(self) -> None:
         tk.Toplevel.__init__(self, self.parent)
-        self.configure(background=gui.colors.light_black)
+        self.configure(background=cfg.color.light_black)
         # remove the standard window titlebar from the tooltip
         self.overrideredirect(True)
         # unpack *args and put each /n on a new line
         lines = "\n".join(self.text)
-        frame = tk.Frame(self, background=gui.colors.light_black)
+        frame = tk.Frame(self, background=cfg.color.light_black)
         label = tk.Label(
             frame,
             text=lines,
             background=self.background,
-            foreground=gui.colors.white_grey,
+            foreground=cfg.color.white_grey,
             justify="left",
         )
         # get size of the label to use later for positioning and sizing of the tooltip
         x, y = label.winfo_reqwidth(), label.winfo_reqheight()
         # set the size of the tooltip background to be 1px larger than the label
         frame.configure(width=x + 1, height=y + 1)
 
@@ -309,15 +245,15 @@
         config_key (str): Key in the configuration file where the state is stored.
         write_to_reg (bool, optional): Whether to also write the state to registry. Defaults to False.
         show_if_exe (bool, optional): Only show the button if the program is not running from an executable. Defaults to True.
     """
 
     def __init__(self, parent, setting_label: str, config_key: str, **kwargs) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=gui.colors.dark_grey)
+        self.configure(bg=cfg.color.dark_grey)
         self.string_var = tk.StringVar()
         self.string_var.set(f"{io_json.get_json_key(config_key)}")
         self.setting_name = setting_label
         self.config_key = config_key
         self.write_to_reg = kwargs.get("write_to_reg", False)
         self.show_if_exe = kwargs.get("write_to_reg", True)
         self.tip_text = kwargs.get("tip_text", None)
@@ -395,26 +331,20 @@
         btn["style"] = f"{self.string_var.get()}.TButton"
         io_json.set_config_key_value(self.config_key, False)
         if self.write_to_reg:
             io_winreg.remove_context_menu()
         self.enter_button(event)
 
 
-def set_ttk_theme(root):
-    initializer_tcl = app_paths.gui_app_theme / "ttk_theme_initializer.tcl"
-    root.tk.call("source", str(initializer_tcl))
-    root.tk.call("set_theme")
-
-
 def configure_root(root):
     """
     Initialize the root Tkinter window for the Subsearch application.
 
     Returns:
         tk.Tk: The initialized Tkinter root window.
     """
     if io_json.get_json_key("context_menu"):
         io_winreg.add_context_menu()
-    root.configure(background=gui.colors.dark_grey)
+    root.configure(background=cfg.color.dark_grey)
     root.iconbitmap(app_paths.gui_assets / "subsearch.ico")
     root.geometry(WindowPosition.set(root))  # type: ignore
     root.resizable(False, False)
```

### Comparing `Subsearch-2.36.4/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.37.0rc1/src/subsearch/gui/screens/download_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import re
 import tkinter as tk
 from tkinter import ttk
 
-from subsearch.data import app_paths, gui, video_data
+from subsearch.data import app_paths, video_data
 from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
+from subsearch.gui.resources import config as cfg
 from subsearch.providers import subscene
 from subsearch.utils import file_manager, log
 
 
 class DownloadList(tk.Frame):
     def __init__(self, parent, formatted_data: list[PrettifiedDownloadData]) -> None:
         tk.Frame.__init__(self, parent)
         root_posx, root_posy = parent.winfo_reqwidth(), parent.winfo_reqheight()
-        self.configure(bg=gui.colors.dark_grey, width=root_posx, height=root_posy - 82)
+        self.configure(bg=cfg.color.dark_grey, width=root_posx, height=root_posy - 82)
         if formatted_data is not None:
             formatted_data.sort(key=lambda x: x.pct_result, reverse=True)
         self.formatted_data = formatted_data
         self.subscene_scrape = subscene.SubsceneScraper()
         self.extent = 0
         self.scrollbar = ttk.Scrollbar(self, orient="vertical", style="Vertical.TScrollbar")
         self.sub_listbox = tk.Listbox(
             self,
             height=root_posy,
-            bg=gui.colors.dark_grey,
-            fg=gui.colors.light_grey,
-            font=gui.fonts.cas8b,
+            bg=cfg.color.dark_grey,
+            fg=cfg.color.light_grey,
+            font=cfg.font.cas8b,
             bd=0,
             border=0,
             borderwidth=0,
             highlightthickness=0,
             activestyle="none",
             yscrollcommand=self.scrollbar.set,
         )
@@ -75,15 +76,15 @@
         self.sub_listbox.delete(int(item_num))
         self.sub_listbox.insert(int(item_num), f"» DOWNLOADING «")
         for enum, _provider, _release, _url in zip(
             self._providers.keys(), self._providers.values(), self._releases.values(), self._urls.values()
         ):
             if enum != int(item_num):
                 continue
-            self.sub_listbox.itemconfig(int(enum), {"fg": gui.colors.blue})
+            self.sub_listbox.itemconfig(int(enum), {"fg": cfg.color.blue})
             if _provider == "subscene":
                 download_url = self.subscene_scrape.get_download_url(_url)
             else:
                 download_url = _url
             path = f"{ app_paths.tmpdir}\\__{_provider}__{item_num}.zip"
             enum = DownloadData(
                 provider=f"Downloading from {_provider}",
@@ -95,8 +96,8 @@
             )  # type: ignore
             file_manager.download_subtitle(enum)  # type: ignore
             file_manager.extract_files(app_paths.tmpdir, video_data.subs_directory, ".zip")
             file_manager.delete_temp_files(app_paths.tmpdir)
             break
         self.sub_listbox.delete(int(item_num))
         self.sub_listbox.insert(int(item_num), f"✔ {_release}")
-        self.sub_listbox.itemconfig(int(item_num), {"fg": gui.colors.green})
+        self.sub_listbox.itemconfig(int(item_num), {"fg": cfg.color.green})
```

### Comparing `Subsearch-2.36.4/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.37.0rc1/src/subsearch/gui/screens/language_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import tkinter as tk
-from tkinter import ttk
+from tkinter import IntVar, ttk
 
-from subsearch.data import gui
 from subsearch.gui import gui_toolkit
 from subsearch.utils import io_json
 
 
-class SelectLanguage(tk.Frame):
+class SelectLanguage(ttk.Labelframe):
     def __init__(self, parent) -> None:
-        tk.Frame.__init__(self, parent)
-        self.configure(bg=gui.colors.dark_grey)
+        ttk.Labelframe.__init__(self, parent)
+        self.configure(text="Languages", padding=10)
         self.active_btn = None
         self.rownum = 0
         self.colnum = 1
         self.checkbox_values = {}
         self.name_find_key = {}
         self.tip_present = False
         self.languages = io_json.get_available_languages()
         self.current_language = io_json.get_json_key("current_language")
-        for language, language_data in self.languages.items():
-            if self.rownum == 14:
-                self.rownum = 0
-                self.colnum += 1
+        self.checkbuttons: dict[ttk.Checkbutton, IntVar] = {}
+        frame = None
+        for enum, (language, language_data) in enumerate(self.languages.items()):
+            if enum % 14 == 0:
+                frame = ttk.Frame(self)
+                frame.pack(side=tk.LEFT, anchor="n")
+
             valuevar = tk.IntVar()
-            btn = ttk.Checkbutton(self, text=language_data["name"], onvalue=1, offvalue=9, variable=valuevar, width=20)
+            btn = ttk.Checkbutton(frame, text=language_data["name"], onvalue=1, offvalue=9, variable=valuevar, width=20)
             if self.current_language == language:
                 valuevar.set(1)
                 self.checkbox_values[btn] = valuevar
             else:
                 valuevar.set(0)
                 self.checkbox_values[btn] = valuevar
-            btn.grid(row=self.rownum, column=self.colnum, pady=8)
+            btn.pack(padx=2, pady=8)
             if valuevar.get() == 1:
                 self.active_btn = btn
 
             btn.bind("<Enter>", self.enter_button)
             btn.bind("<Leave>", self.leave_button)
-            self.rownum += 1
             self.name_find_key[language_data["name"]] = language
-        gui_toolkit.set_default_grid_size(self, width_=6)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         json_key = self.name_find_key[btn["text"]]
         providers = ", ".join(([_i.title() for _i in self.languages[json_key]["incompatibility"]]))
         if providers:
             tip_text = f"If enabled, '{providers}' will be automatically skipped."
```

### Comparing `Subsearch-2.36.4/src/subsearch/providers/generic.py` & `Subsearch-2.37.0rc1/src/subsearch/providers/generic.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.37.0rc1/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/providers/subscene.py` & `Subsearch-2.37.0rc1/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.37.0rc1/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/app_integrity.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/app_integrity.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/exceptions.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/file_manager.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/io_json.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/io_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from pathlib import Path
 from typing import Any, Union
 
 from subsearch.data import SUPPORTED_FILE_EXTENSIONS, SUPPORTED_PROVIDERS, app_paths
 from subsearch.data.data_objects import AppConfig, LanguageData, ProviderAlphaCodeData
-from subsearch.utils import file_manager
 from subsearch.utils.exceptions import ProviderNotImplemented
 
 APPCON_JSON = Path(app_paths.appdata_local) / "application_config.json"
 LANGS_JSON = Path(app_paths.data) / "languages.json"
 
 
 def get_json_data(json_file: Path = APPCON_JSON) -> Any:
@@ -85,14 +84,16 @@
         "current_language": "english",
         "subtitle_type": dict.fromkeys(subtitle_types, True),
         "foreign_only": False,
         "percentage_threshold": 90,
         "rename_best_match": True,
         "context_menu": True,
         "context_menu_icon": True,
+        "system_tray": True,
+        "toast_summary": False,
         "manual_download_fail": True,
         "manual_download_mode": False,
         "use_threading": True,
         "multiple_app_instances": False,
         "show_terminal": False,
         "log_to_file": False,
         "file_extensions": dict.fromkeys(SUPPORTED_FILE_EXTENSIONS, True),
```

### Comparing `Subsearch-2.36.4/src/subsearch/utils/io_winreg.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/log.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/log.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/mutex_synchronizer.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/mutex_synchronizer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/string_parser.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.4/src/subsearch/utils/update.py` & `Subsearch-2.37.0rc1/src/subsearch/utils/update.py`

 * *Files identical despite different names*

