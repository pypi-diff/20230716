# Comparing `tmp/Algo_Vi-1.0.1.tar.gz` & `tmp/Algo-Vi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Algo_Vi-1.0.1.tar", last modified: Tue Mar 22 02:22:19 2022, max compression
+gzip compressed data, was "Algo-Vi-1.0.3.tar", last modified: Sun Jul 16 18:05:08 2023, max compression
```

## Comparing `Algo_Vi-1.0.1.tar` & `Algo-Vi-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,838 @@
-drwxrwxrwx   0        0        0        0 2022-03-22 02:22:19.480206 Algo_Vi-1.0.1/
-drwxrwxrwx   0        0        0        0 2022-03-22 02:22:19.475805 Algo_Vi-1.0.1/Algo_Vi.egg-info/
--rw-rw-rw-   0        0        0      722 2022-03-22 02:22:17.000000 Algo_Vi-1.0.1/Algo_Vi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2022-03-22 02:22:18.000000 Algo_Vi-1.0.1/Algo_Vi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-22 02:22:18.000000 Algo_Vi-1.0.1/Algo_Vi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-03-22 02:22:18.000000 Algo_Vi-1.0.1/Algo_Vi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2022-03-22 02:22:18.000000 Algo_Vi-1.0.1/Algo_Vi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2021-11-12 04:43:11.000000 Algo_Vi-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       25 2021-11-13 18:28:15.000000 Algo_Vi-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      722 2022-03-22 02:22:19.478654 Algo_Vi-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      149 2022-03-21 11:01:41.000000 Algo_Vi-1.0.1/README.md
--rw-rw-rw-   0        0        0        0 2022-03-22 02:20:31.000000 Algo_Vi-1.0.1/__init__.py
--rw-rw-rw-   0        0        0     5062 2022-03-22 02:20:31.000000 Algo_Vi-1.0.1/__main__.py
--rw-rw-rw-   0        0        0       42 2022-03-22 02:22:19.481205 Algo_Vi-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      985 2022-03-22 02:21:52.000000 Algo_Vi-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.830479 Algo-Vi-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.406947 Algo-Vi-1.0.3/AlgoVi.egg-info/
+-rw-rw-rw-   0        0        0        0 2023-07-16 17:48:23.000000 Algo-Vi-1.0.3/AlgoVi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 17:52:45.000000 Algo-Vi-1.0.3/AlgoVi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-16 17:52:45.000000 Algo-Vi-1.0.3/AlgoVi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2021-11-12 04:43:12.000000 Algo-Vi-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       25 2021-11-13 18:28:16.000000 Algo-Vi-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      699 2023-07-16 18:05:08.819508 Algo-Vi-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2022-03-21 11:01:42.000000 Algo-Vi-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.409939 Algo-Vi-1.0.3/Search-Vi/
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.424899 Algo-Vi-1.0.3/Search-Vi/AlgoVi.egg-info/
+-rw-rw-rw-   0        0        0    42674 2023-07-16 17:57:09.000000 Algo-Vi-1.0.3/Search-Vi/AlgoVi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 17:57:09.000000 Algo-Vi-1.0.3/Search-Vi/AlgoVi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 17:57:09.000000 Algo-Vi-1.0.3/Search-Vi/AlgoVi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.485736 Algo-Vi-1.0.3/Search-Vi/Algo_Vi.egg-info/
+-rw-rw-rw-   0        0        0      699 2023-07-16 18:04:58.000000 Algo-Vi-1.0.3/Search-Vi/Algo_Vi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    42803 2023-07-16 18:04:59.000000 Algo-Vi-1.0.3/Search-Vi/Algo_Vi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 18:04:58.000000 Algo-Vi-1.0.3/Search-Vi/Algo_Vi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 18:04:58.000000 Algo-Vi-1.0.3/Search-Vi/Algo_Vi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5066 2023-07-16 17:56:12.000000 Algo-Vi-1.0.3/Search-Vi/__main__.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 18:05:08.831476 Algo-Vi-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-16 18:03:57.000000 Algo-Vi-1.0.3/setup.py
+-rw-rw-rw-   0        0        0        0 2023-01-26 04:23:12.000000 Algo-Vi-1.0.3/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.190525 Algo-Vi-1.0.3/venv/
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.191522 Algo-Vi-1.0.3/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.351100 Algo-Vi-1.0.3/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.491721 Algo-Vi-1.0.3/venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     6128 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/_distutils_hack/override.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.504685 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      357 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.729086 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10234 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0    10734 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.860734 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     7842 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    29381 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2472 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10817 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18172 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.000817 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7582 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1685 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4129 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9815 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6573 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5289 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4762 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3374 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    31726 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12343 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6129 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3680 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     7396 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13529 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.053676 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      729 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6494 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1164 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    20942 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.070631 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16503 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37596 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6557 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.137222 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    17552 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6302 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7867 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2573 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.167553 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4280 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25277 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.218547 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      107 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8181 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7457 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0     9773 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.354641 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     5877 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2617 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    18083 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4644 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.403125 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    12190 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2145 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6096 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18443 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.446425 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.488312 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1404 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1456 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1063 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1405 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5109 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9784 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.504270 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1354 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0     4105 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
+-rw-rw-rw-   0        0        0    27407 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    25091 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     7074 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.607654 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2807 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17646 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    35600 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     2858 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24045 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.615632 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.623611 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24129 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:00.760156 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18963 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    27878 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9914 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     2526 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5455 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    11533 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8020 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:01.068180 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     1015 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     5764 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     1115 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
+-rw-rw-rw-   0        0        0     2203 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     4831 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11632 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    21617 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     5662 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9197 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7702 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3459 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4549 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:01.135809 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3518 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18116 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5238 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11728 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22811 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    13079 2023-01-22 16:43:40.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:01.173320 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4966 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:01.240121 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      465 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     5033 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1535 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:01.334869 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      242 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1033 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      778 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    16416 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     3946 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4154 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7105 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      774 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:01.385892 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.329204 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     3705 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1741 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0     9608 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3817 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     4801 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.337178 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     2406 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3559 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0     1838 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1619 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     3864 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12021 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3676 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1731 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1731 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1737 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    13919 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1730 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    26797 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5260 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     3367 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2056 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30068 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.345156 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13280 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0     6199 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4129 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     3749 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    13288 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8289 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2709 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      242 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.492763 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      239 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10830 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.692229 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41259 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51697 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20834 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51991 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5058 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39801 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18102 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    66262 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43898 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.724144 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    48841 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.783987 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.823877 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6080 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34557 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:02.963505 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:03.233599 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/
+-rw-rw-rw-   0        0        0      130 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/_compat.py
+-rw-rw-rw-   0        0        0     3443 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/build.py
+-rw-rw-rw-   0        0        0     6083 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/check.py
+-rw-rw-rw-   0        0        0     3994 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-rw-rw-   0        0        0      607 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-rw-rw-   0        0        0     6081 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:03.445022 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/in_process/
+-rw-rw-rw-   0        0        0      872 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-rw-rw-   0        0        0    10801 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-rw-rw-   0        0        0     2520 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
+-rw-rw-rw-   0        0        0    12721 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:03.502437 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   108287 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:03.567149 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12831 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1176 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6910 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0       78 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6439 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:03.830108 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2999 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:03.868696 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.025576 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     4810 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5086 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35441 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     5871 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    32005 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.089203 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    11174 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    70232 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53376 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     4630 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.101954 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3419 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63187 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0     9110 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.249849 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9171 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213344 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.265589 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23685 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.426234 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5178 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      440 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21443 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35287 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33240 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.448176 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:04.517806 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5872 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1583 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    17592 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4794 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:05.686657 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     5944 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8808 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2114 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0     9695 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     7063 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6820 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9864 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4503 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    17957 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    95885 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     7954 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1616 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2507 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9585 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5051 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14074 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14172 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11471 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0     8744 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    36576 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59746 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8161 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4449 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4773 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2842 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24224 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4374 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    26240 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    34697 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39515 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    44666 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3627 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    26060 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:05.733766 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    18364 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     1944 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1496 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1376 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     1908 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     7550 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     2790 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2145 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8011 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:05.786052 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    80114 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:05.905252 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20070 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39093 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:05.975064 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.004989 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11034 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4538 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17182 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.020941 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.038947 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30109 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.157585 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22001 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10003 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14287 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-rw-   0        0        0      469 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/vendor.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.267928 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:04:59.555549 Algo-Vi-1.0.3/venv/Lib/site-packages/pip-22.3.1.dist-info/
+-rw-rw-rw-   0        0        0     1093 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0      125 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip-22.3.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-01-22 16:43:42.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pip-22.3.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.270919 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   106278 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.374203 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.412230 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.515952 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     6488 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13515 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.531910 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.550859 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0      148 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   133344 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    22975 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.656648 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8496 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4706 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.718481 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12806 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6911 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6596 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.830445 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.834436 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-rw-rw-   0        0        0    80078 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-01-22 16:43:06.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:06.886347 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2459 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:07.418021 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     9170 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:07.731995 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      359 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0      411 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0       43 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_log.py
+-rw-rw-rw-   0        0        0      239 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0    19641 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8572 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14752 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    47311 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17867 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:07.886319 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5409 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4666 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    22016 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5585 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7693 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31514 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16544 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5605 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4872 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2595 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13078 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30165 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2763 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2788 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1181 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8410 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1933 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      672 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11818 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19196 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7492 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4911 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9397 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    11942 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3414 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     8072 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50190 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10270 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17901 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8213 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13715 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1201 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30204 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23580 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      217 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0      639 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3495 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18774 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12096 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15602 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18097 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12952 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5205 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     2282 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2392 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1311 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0      749 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_path.py
+-rw-rw-rw-   0        0        0      501 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:07.901849 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.014469 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    30130 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     1862 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1828 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1154 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     2166 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.100177 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.112144 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     6488 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13512 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.116135 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.129158 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.268823 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8493 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4700 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.404519 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.421572 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.471439 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7346 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    19595 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.736590 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16623 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6589 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4423 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    15821 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    14115 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     7012 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     4800 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85662 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    31188 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    27411 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5163 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2226 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2612 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     7071 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8102 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7470 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.775646 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/
+-rw-rw-rw-   0        0        0     1121 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    13579 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.802574 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   269900 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     8736 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16319 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    19598 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25574 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      949 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    20818 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    45522 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2464 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5591 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:08.815518 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2512 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     3824 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1232 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0     4857 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47724 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    39682 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      144 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     8376 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      718 2023-01-22 16:43:08.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:05:07.437970 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools-66.1.1.dist-info/
+-rw-rw-rw-   0        0        0     2740 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools-66.1.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-01-22 16:43:10.000000 Algo-Vi-1.0.3/venv/Lib/site-packages/setuptools-66.1.1.dist-info/top_level.txt
```

### Comparing `Algo_Vi-1.0.1/Algo_Vi.egg-info/PKG-INFO` & `Algo-Vi-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: Algo-Vi
-Version: 1.0.1
+Version: 1.0.3
 Summary: It visual the Search Algorithm
 Home-page: https://github.com/punithanae/Python_library
 Author: Punithan
 Author-email: punithanae@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,9 +18,7 @@
 # Install_library
 pip install Algo-Vi
 
 # Description
 1.Run the library and enter the list value
 2.Select your Algo
 3.See the Visual
-
-
```

### Comparing `Algo_Vi-1.0.1/LICENSE` & `Algo-Vi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Algo_Vi-1.0.1/PKG-INFO` & `Algo-Vi-1.0.3/Search-Vi/Algo_Vi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: Algo_Vi
-Version: 1.0.1
+Name: Algo-Vi
+Version: 1.0.3
 Summary: It visual the Search Algorithm
 Home-page: https://github.com/punithanae/Python_library
 Author: Punithan
 Author-email: punithanae@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,9 +18,7 @@
 # Install_library
 pip install Algo-Vi
 
 # Description
 1.Run the library and enter the list value
 2.Select your Algo
 3.See the Visual
-
-
```

### Comparing `Algo_Vi-1.0.1/__main__.py` & `Algo-Vi-1.0.3/Search-Vi/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             print(arr[i], "greater than previous value ")
             print(arr[0:i], '\x1b[6;30;42m' + str(arr[i]) + '\x1b[0m', " ", arr[i + 1:len(l)])
             time.sleep(1)
         gap //= 2
     print("Sorted output",arr)
 
 
-def Algo():
+def __init__():
     l = list(map(int, input("Enter the list in space separated value : ").strip().split()))
     m=input("Enter your Algo Sort or Search :")
     if(m== "Search"):
      v = int(input("Enter the Target value to find : "))
      n = input("Enter the Search mode Binary or Linear : ")
     else:
      n=input("Enter Bubble sort ,Insertion sort, Shell sort,Selection sort :")
```

### Comparing `Algo_Vi-1.0.1/setup.py` & `Algo-Vi-1.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
-    name="Algo_Vi",
-    version="1.0.1",
+    name='Algo-Vi',
+    version='1.0.3',
     description="It visual the Search Algorithm",
     long_description=README,
     long_description_content_type="text/markdown",
-    entry_points={
-        'console_scripts': [
-            'Search-Vi = __main__:Algo',
-        ]
-    },
     url="https://github.com/punithanae/Python_library",
     author="Punithan",
     author_email="punithanae@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
-    package_dir={"__main__.py": "Search-Vi"},
+    py_modules=['AlgoVi'],
+    package_dir={'':'Search-Vi'},
     include_package_data=True,
-    install_requires=[],    keyword=['Search', 'Sort']
+    keyword=['Search', 'Sort']
 
 )
```

