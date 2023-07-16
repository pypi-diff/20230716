# Comparing `tmp/pytest-discord-0.1.3.tar.gz` & `tmp/pytest-discord-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-discord-0.1.3.tar", last modified: Sat Jul 15 15:09:59 2023, max compression
+gzip compressed data, was "pytest-discord-0.1.4.tar", last modified: Sun Jul 16 15:05:02 2023, max compression
```

## Comparing `pytest-discord-0.1.3.tar` & `pytest-discord-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.555878 pytest-discord-0.1.3/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      185 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     7275 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     5827 2023-07-15 13:52:23.000000 pytest-discord-0.1.3/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1253 2023-07-15 14:47:36.000000 pytest-discord-0.1.3/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/pytest_discord/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/pytest_discord/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-15 15:06:21.000000 pytest-discord-0.1.3/pytest_discord/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1913 2023-05-27 13:01:00.000000 pytest-discord-0.1.3/pytest_discord/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3120 2023-07-15 14:52:47.000000 pytest-discord-0.1.3/pytest_discord/_opt_retriever.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13579 2023-07-15 14:52:47.000000 pytest-discord-0.1.3/pytest_discord/plugin.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/pytest_discord.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     7275 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      573 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-15 15:09:41.000000 pytest-discord-0.1.3/pytest_discord.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      142 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       15 2023-07-15 15:09:59.000000 pytest-discord-0.1.3/pytest_discord.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)      159 2023-06-04 03:12:59.000000 pytest-discord-0.1.3/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        5 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-15 15:09:59.555878 pytest-discord-0.1.3/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2755 2023-02-25 22:32:35.000000 pytest-discord-0.1.3/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-15 15:09:59.545879 pytest-discord-0.1.3/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       30 2021-03-20 04:14:09.000000 pytest-discord-0.1.3/tests/conftest.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4423 2023-02-05 14:10:17.000000 pytest-discord-0.1.3/tests/test_plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      922 2023-06-25 13:04:56.000000 pytest-discord-0.1.3/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:05:02.578757 pytest-discord-0.1.4/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:09.000000 pytest-discord-0.1.4/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      185 2021-03-20 04:14:09.000000 pytest-discord-0.1.4/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     7275 2023-07-16 15:05:02.578757 pytest-discord-0.1.4/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     5827 2023-07-15 13:52:23.000000 pytest-discord-0.1.4/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)     1253 2023-07-15 14:47:36.000000 pytest-discord-0.1.4/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:05:02.568757 pytest-discord-0.1.4/pytest_discord/
+-rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-03-20 04:14:09.000000 pytest-discord-0.1.4/pytest_discord/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-16 15:03:29.000000 pytest-discord-0.1.4/pytest_discord/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1913 2023-05-27 13:01:00.000000 pytest-discord-0.1.4/pytest_discord/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3120 2023-07-15 14:52:47.000000 pytest-discord-0.1.4/pytest_discord/_opt_retriever.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13598 2023-07-16 14:44:27.000000 pytest-discord-0.1.4/pytest_discord/plugin.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:05:02.578757 pytest-discord-0.1.4/pytest_discord.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7275 2023-07-16 15:05:02.000000 pytest-discord-0.1.4/pytest_discord.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      573 2023-07-16 15:05:02.000000 pytest-discord-0.1.4/pytest_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 15:05:02.000000 pytest-discord-0.1.4/pytest_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-07-16 15:05:02.000000 pytest-discord-0.1.4/pytest_discord.egg-info/entry_points.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 15:04:39.000000 pytest-discord-0.1.4/pytest_discord.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      142 2023-07-16 15:05:02.000000 pytest-discord-0.1.4/pytest_discord.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       15 2023-07-16 15:05:02.000000 pytest-discord-0.1.4/pytest_discord.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:05:02.578757 pytest-discord-0.1.4/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)      159 2023-07-16 14:45:51.000000 pytest-discord-0.1.4/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        5 2021-03-20 04:14:09.000000 pytest-discord-0.1.4/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-16 15:05:02.578757 pytest-discord-0.1.4/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2755 2023-02-25 22:32:35.000000 pytest-discord-0.1.4/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 15:05:02.578757 pytest-discord-0.1.4/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       30 2021-03-20 04:14:09.000000 pytest-discord-0.1.4/tests/conftest.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4423 2023-02-05 14:10:17.000000 pytest-discord-0.1.4/tests/test_plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      922 2023-06-25 13:04:56.000000 pytest-discord-0.1.4/tox.ini
```

### Comparing `pytest-discord-0.1.3/LICENSE` & `pytest-discord-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/PKG-INFO` & `pytest-discord-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-discord
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytest plugin to notify test results to a Discord channel.
 Home-page: https://github.com/thombashi/pytest-discord
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-discord
 Project-URL: Tracker, https://github.com/thombashi/pytest-discord/issues
```

### Comparing `pytest-discord-0.1.3/README.rst` & `pytest-discord-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/pyproject.toml` & `pytest-discord-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/pytest_discord/_const.py` & `pytest-discord-0.1.4/pytest_discord/_const.py`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/pytest_discord/_opt_retriever.py` & `pytest-discord-0.1.4/pytest_discord/_opt_retriever.py`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/pytest_discord/plugin.py` & `pytest-discord-0.1.4/pytest_discord/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     if not hasattr(config.option, "md_report_margin"):
         config.option.md_report_margin = 1
 
     try:
         config.option.md_report_color = ColorPolicy.NEVER
         config.option.md_report_zeros = ZerosRender.EMPTY
 
-        return make_md_report(config, reporter, stat_count_map)
+        return make_md_report(config, reporter, stat_count_map, ColorPolicy.NEVER)
     finally:
         config.option.md_report_color = stash_md_report_color
         config.option.md_report_zeros = stash_md_report_zeros
 
 
 def _make_header(tests: int) -> str:
     msgs = [f"{tests} tests"]
```

### Comparing `pytest-discord-0.1.3/pytest_discord.egg-info/PKG-INFO` & `pytest-discord-0.1.4/pytest_discord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-discord
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytest plugin to notify test results to a Discord channel.
 Home-page: https://github.com/thombashi/pytest-discord
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-discord
 Project-URL: Tracker, https://github.com/thombashi/pytest-discord/issues
```

### Comparing `pytest-discord-0.1.3/pytest_discord.egg-info/SOURCES.txt` & `pytest-discord-0.1.4/pytest_discord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/setup.py` & `pytest-discord-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/tests/test_plugin.py` & `pytest-discord-0.1.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.3/tox.ini` & `pytest-discord-0.1.4/tox.ini`

 * *Files identical despite different names*

