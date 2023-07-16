# Comparing `tmp/pytest-md-report-0.3.2.tar.gz` & `tmp/pytest-md-report-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-md-report-0.3.2.tar", last modified: Sun Jun 25 14:22:31 2023, max compression
+gzip compressed data, was "pytest-md-report-0.4.0.tar", last modified: Sun Jul 16 08:21:06 2023, max compression
```

## Comparing `pytest-md-report-0.3.2.tar` & `pytest-md-report-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      204 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    10153 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      801 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/pytest_md_report/
--rw-r--r--   0 toor      (1000) toor      (1000)      300 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4447 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16816 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/pytest_md_report.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      609 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 14:21:55.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       94 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       86 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2791 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       30 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tests/conftest.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1034 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tests/test_option.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5016 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tests/test_plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      857 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 08:21:06.716592 pytest-md-report-0.4.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      204 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11561 2023-07-16 08:21:06.716592 pytest-md-report-0.4.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    10095 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)      885 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 08:21:06.706592 pytest-md-report-0.4.0/pytest_md_report/
+-rw-r--r--   0 toor      (1000) toor      (1000)      300 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/pytest_md_report/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/pytest_md_report/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4531 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/pytest_md_report/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    17901 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/pytest_md_report/plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/pytest_md_report/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 08:21:06.716592 pytest-md-report-0.4.0/pytest_md_report.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11561 2023-07-16 08:21:06.000000 pytest-md-report-0.4.0/pytest_md_report.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      609 2023-07-16 08:21:06.000000 pytest-md-report-0.4.0/pytest_md_report.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 08:21:06.000000 pytest-md-report-0.4.0/pytest_md_report.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-07-16 08:21:06.000000 pytest-md-report-0.4.0/pytest_md_report.egg-info/entry_points.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-16 08:20:32.000000 pytest-md-report-0.4.0/pytest_md_report.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       94 2023-07-16 08:21:06.000000 pytest-md-report-0.4.0/pytest_md_report.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-07-16 08:21:06.000000 pytest-md-report-0.4.0/pytest_md_report.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 08:21:06.716592 pytest-md-report-0.4.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       86 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-16 08:21:06.716592 pytest-md-report-0.4.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2791 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-16 08:21:06.716592 pytest-md-report-0.4.0/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       30 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/tests/conftest.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1034 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/tests/test_option.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5016 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/tests/test_plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      857 2023-07-16 08:20:17.000000 pytest-md-report-0.4.0/tox.ini
```

### Comparing `pytest-md-report-0.3.2/LICENSE` & `pytest-md-report-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.2/PKG-INFO` & `pytest-md-report-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.3.2
+Version: 0.4.0
 Summary: A pytest plugin to make a test results report with Markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
 Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
@@ -151,83 +151,74 @@
                             you can also specify the value with PYTEST_MD_REPORT_VERBOSE environment variable.
       --md-report-output=FILEPATH
                             Path to a file to the outputs test report.
                             Overwrite a file content if the file already exists.
                             you can also specify the value with PYTEST_MD_REPORT_OUTPUT environment variable.
       --md-report-tee       output test report for both standard output and a file. you can also specify the value with PYTEST_MD_REPORT_TEE environment variable.
       --md-report-color={auto,text,never}
-                            How to color output reports.
-                            auto: render colored (text and background) reports using ANSI escape codes.
+                            How coloring output reports.
+                            auto: for terminal output, render colored (text and background) reports using ANSI escape codes.
+                            for file output, render the report without color.
                             text: render colored text reports by using ANSI escape codes.
                             never: render report without color.
-                            Defaults to 'auto'.
+                            Defaults to 'ColorPolicy.AUTO'.
                             you can also specify the value with PYTEST_MD_REPORT_COLOR environment variable.
       --md-report-margin=MARGIN
                             Margin size for each cell.
                             Defaults to 1.
                             you can also specify the value with PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
                             Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
                             Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive);
                             otherwise 'number'.
                             you can also specify the value with PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
                             Text color of succeeded results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_green'.
                             you can also specify the value with PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
       --md-report-skip-color=MD_REPORT_SKIP_COLOR
                             Text color of skipped results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_yellow'.
                             you can also specify the value with PYTEST_MD_REPORT_SKIP_COLOR environment variable.
       --md-report-error-color=MD_REPORT_ERROR_COLOR
                             Text color of failed results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_red'.
                             you can also specify the value with PYTEST_MD_REPORT_ERROR_COLOR environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
   md_report (bool):     Create Markdown report.
   md_report_verbose (string):
                         Verbosity level for pytest-md-report. If not set, use the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
-                        How to color output reports. auto: render colored (text and background) reports using ANSI escape codes. text: render colored text reports by using ANSI escape codes. never:
-                        render report without color. Defaults to 'auto'.
+                        How coloring output reports. auto: for terminal output, render colored (text and background) reports using ANSI escape codes. for file output, render the report without color. text: render colored text reports by using ANSI escape codes. never: render report without color. Defaults to
+                        'ColorPolicy.AUTO'.
   md_report_output (string):
                         Path to a file to the outputs test report. Overwrite a file content if the file already exists.
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
                         Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
-                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case
-                        insensitive); otherwise 'number'.
+                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive); otherwise 'number'.
   md_report_success_color (string):
-                        Text color of succeeded results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_green'.
+                        Text color of succeeded results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_green'.
   md_report_skip_color (string):
-                        Text color of skipped results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_yellow'.
+                        Text color of skipped results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_yellow'.
   md_report_error_color (string):
-                        Text color of failed results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_red'.
+                        Text color of failed results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_red'.
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.3.2/README.rst` & `pytest-md-report-0.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -117,83 +117,74 @@
                             you can also specify the value with PYTEST_MD_REPORT_VERBOSE environment variable.
       --md-report-output=FILEPATH
                             Path to a file to the outputs test report.
                             Overwrite a file content if the file already exists.
                             you can also specify the value with PYTEST_MD_REPORT_OUTPUT environment variable.
       --md-report-tee       output test report for both standard output and a file. you can also specify the value with PYTEST_MD_REPORT_TEE environment variable.
       --md-report-color={auto,text,never}
-                            How to color output reports.
-                            auto: render colored (text and background) reports using ANSI escape codes.
+                            How coloring output reports.
+                            auto: for terminal output, render colored (text and background) reports using ANSI escape codes.
+                            for file output, render the report without color.
                             text: render colored text reports by using ANSI escape codes.
                             never: render report without color.
-                            Defaults to 'auto'.
+                            Defaults to 'ColorPolicy.AUTO'.
                             you can also specify the value with PYTEST_MD_REPORT_COLOR environment variable.
       --md-report-margin=MARGIN
                             Margin size for each cell.
                             Defaults to 1.
                             you can also specify the value with PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
                             Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
                             Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive);
                             otherwise 'number'.
                             you can also specify the value with PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
                             Text color of succeeded results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_green'.
                             you can also specify the value with PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
       --md-report-skip-color=MD_REPORT_SKIP_COLOR
                             Text color of skipped results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_yellow'.
                             you can also specify the value with PYTEST_MD_REPORT_SKIP_COLOR environment variable.
       --md-report-error-color=MD_REPORT_ERROR_COLOR
                             Text color of failed results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_red'.
                             you can also specify the value with PYTEST_MD_REPORT_ERROR_COLOR environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
   md_report (bool):     Create Markdown report.
   md_report_verbose (string):
                         Verbosity level for pytest-md-report. If not set, use the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
-                        How to color output reports. auto: render colored (text and background) reports using ANSI escape codes. text: render colored text reports by using ANSI escape codes. never:
-                        render report without color. Defaults to 'auto'.
+                        How coloring output reports. auto: for terminal output, render colored (text and background) reports using ANSI escape codes. for file output, render the report without color. text: render colored text reports by using ANSI escape codes. never: render report without color. Defaults to
+                        'ColorPolicy.AUTO'.
   md_report_output (string):
                         Path to a file to the outputs test report. Overwrite a file content if the file already exists.
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
                         Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
-                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case
-                        insensitive); otherwise 'number'.
+                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive); otherwise 'number'.
   md_report_success_color (string):
-                        Text color of succeeded results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_green'.
+                        Text color of succeeded results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_green'.
   md_report_skip_color (string):
-                        Text color of skipped results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_yellow'.
+                        Text color of skipped results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_yellow'.
   md_report_error_color (string):
-                        Text color of failed results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_red'.
+                        Text color of failed results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_red'.
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.3.2/pyproject.toml` & `pytest-md-report-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -36,16 +36,20 @@
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
 python_version = 3.7
 
 pretty = true
+
+no_implicit_optional = true
 show_error_codes = true
 show_error_context = true
+warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
+warn_unused_ignores = true
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
```

### Comparing `pytest-md-report-0.3.2/pytest_md_report/_const.py` & `pytest-md-report-0.4.0/pytest_md_report/_const.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 
 class Header:
     FILEPATH = "filepath"
     TESTFUNC = "function"
     SUBTOTAL = "SUBTOTAL"
 
 
-class ColorPolicy:
+class ColorPolicy(Enum):
     AUTO = "auto"
     TEXT = "text"
     NEVER = "never"
-    LIST = (AUTO, TEXT, NEVER)
 
 
 class ZerosRender:
     NUMBER = "number"
     EMPTY = "empty"
     LIST = (NUMBER, EMPTY)
 
@@ -36,15 +35,15 @@
 class BGColor:
     EVEN_ROW = "#202020"
     ODD_ROW = "black"
     TOTAL_ROW = "#000000"
 
 
 class Default:
-    COLOR = ColorPolicy.AUTO
+    COLOR_POLICY = ColorPolicy.AUTO
     MARGIN = 1
     ZEROS = ZerosRender.NUMBER
 
     class FGColor:
         SUCCESS = "light_green"
         ERROR = "light_red"
         SKIP = "light_yellow"
@@ -80,21 +79,23 @@
         f"{OPTION_PREFIX}-tee",
         "output test report for both standard output and a file.",
     )
     MD_REPORT_COLOR = (
         f"{OPTION_PREFIX}-color",
         dedent(
             """\
-            How to color output reports.
-            auto: render colored (text and background) reports using ANSI escape codes.
+            How coloring output reports.
+            auto: for terminal output, render colored (text and background) reports
+            using ANSI escape codes.
+            for file output, render the report without color.
             text: render colored text reports by using ANSI escape codes.
             never: render report without color.
             Defaults to '{default}'.
             """
-        ).format(default=Default.COLOR),
+        ).format(default=Default.COLOR_POLICY),
     )
     MD_REPORT_MARGIN = (
         f"{OPTION_PREFIX}-margin",
         dedent(
             """\
             Margin size for each cell.
             Defaults to {default}.
```

### Comparing `pytest-md-report-0.3.2/pytest_md_report/plugin.py` & `pytest-md-report-0.4.0/pytest_md_report/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from collections import defaultdict
 from typing import Any, Dict, Mapping, Optional, Sequence, Tuple, cast
 
 from _pytest.config import Config
+from _pytest.config.argparsing import Parser
 from _pytest.terminal import TerminalReporter
 from pytablewriter import TableWriterFactory
 from pytablewriter.style import Cell, Style
 from pytablewriter.writer import AbstractTableWriter
 from typepy import Bool, Integer, StrictLevel
 from typepy.error import TypeConversionError
 
@@ -16,15 +17,15 @@
 def zero_to_nullstr(value: Any) -> Any:
     if value == 0:
         return ""
 
     return value
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("md report", "make test results report with markdown table format")
 
     group.addoption(
         Option.MD_REPORT.cmdoption_str,
         action="store_true",
         default=None,
         help=Option.MD_REPORT.help_msg
@@ -44,20 +45,21 @@
         default=None,
         help=Option.MD_REPORT_OUTPUT.help_msg
         + HelpMsg.EXTRA_MSG_TEMPLATE.format(Option.MD_REPORT_OUTPUT.envvar_str),
     )
     group.addoption(
         Option.MD_REPORT_TEE.cmdoption_str,
         action="store_true",
+        default=None,
         help=Option.MD_REPORT_TEE.help_msg
         + HelpMsg.EXTRA_MSG_TEMPLATE.format(Option.MD_REPORT_TEE.envvar_str),
     )
     group.addoption(
         Option.MD_REPORT_COLOR.cmdoption_str,
-        choices=ColorPolicy.LIST,
+        choices=[policy.value for policy in ColorPolicy],
         default=None,
         help=Option.MD_REPORT_COLOR.help_msg
         + HelpMsg.EXTRA_MSG_TEMPLATE.format(Option.MD_REPORT_COLOR.envvar_str),
     )
     group.addoption(
         Option.MD_REPORT_MARGIN.cmdoption_str,
         metavar="MARGIN",
@@ -130,15 +132,15 @@
     )
 
 
 def is_make_md_report(config: Config) -> bool:
     if config.option.help:
         return False
 
-    make_report = config.option.md_report
+    make_report: Optional[bool] = config.option.md_report
 
     if make_report is None:
         try:
             make_report = Bool(
                 os.environ.get(Option.MD_REPORT.envvar_str), strict_level=StrictLevel.MIN
             ).convert()
         except TypeConversionError:
@@ -180,15 +182,15 @@
     try:
         return Integer(value, strict_level=StrictLevel.MIN).convert()
     except TypeConversionError:
         return None
 
 
 def retrieve_verbosity_level(config: Config) -> int:
-    verbosity_level = config.option.md_report_verbose
+    verbosity_level: Optional[int] = config.option.md_report_verbose
 
     if verbosity_level is not None and verbosity_level < 0:
         verbosity_level = None
 
     if verbosity_level is None:
         verbosity_level = _to_int(os.environ.get(Option.MD_REPORT_VERBOSE.envvar_str))
 
@@ -198,50 +200,54 @@
     if verbosity_level is None:
         verbosity_level = config.option.verbose
 
     return verbosity_level
 
 
 def retrieve_output_filepath(config: Config) -> Optional[str]:
-    output_filepath = config.option.md_report_output
+    output_filepath: Optional[str] = config.option.md_report_output
 
     if not output_filepath:
         output_filepath = os.environ.get(Option.MD_REPORT_OUTPUT.envvar_str)
 
     if not output_filepath:
         output_filepath = config.getini(Option.MD_REPORT_OUTPUT.inioption_str)
 
     return output_filepath
 
 
 def retrieve_tee(config: Config) -> bool:
-    tee = config.option.md_report_tee
+    tee: Optional[bool] = config.option.md_report_tee
 
-    if not tee:
-        tee = os.environ.get(Option.MD_REPORT_TEE.envvar_str, False)
+    if tee is None:
+        envvar_str = os.environ.get(Option.MD_REPORT_TEE.envvar_str)
+        if envvar_str is not None:
+            tee = bool(envvar_str)
 
-    if not tee:
-        tee = config.getini(Option.MD_REPORT_TEE.inioption_str)
+    if tee is None:
+        inioption_str = config.getini(Option.MD_REPORT_TEE.inioption_str)
+        if inioption_str is not None:
+            tee = bool(inioption_str)
 
-    return tee
+    return tee if tee is not None else False
 
 
-def retrieve_report_color(config: Config) -> str:
-    report_color = config.option.md_report_color
+def retrieve_color_policy(config: Config) -> ColorPolicy:
+    color_policy = config.option.md_report_color
 
-    if not report_color:
-        report_color = os.environ.get(Option.MD_REPORT_COLOR.envvar_str)
+    if not color_policy:
+        color_policy = os.environ.get(Option.MD_REPORT_COLOR.envvar_str)
 
-    if not report_color:
-        report_color = config.getini(Option.MD_REPORT_COLOR.inioption_str)
+    if not color_policy:
+        color_policy = config.getini(Option.MD_REPORT_COLOR.inioption_str)
 
-    if not report_color:
-        return Default.COLOR
+    if not color_policy:
+        return Default.COLOR_POLICY
 
-    return report_color
+    return ColorPolicy[color_policy.upper()]
 
 
 def retrieve_report_margin(config: Config) -> int:
     margin = config.option.md_report_margin
 
     if margin is None:
         margin = _to_int(os.environ.get(Option.MD_REPORT_MARGIN.envvar_str))
@@ -303,37 +309,37 @@
         stat_count_map[name] = count
 
     return stat_count_map
 
 
 class ColorRetriever:
     def __init__(
-        self, row: int, is_grayout: bool, report_color: str, color_map: Dict[str, str]
+        self, row: int, is_grayout: bool, color_polilcy: ColorPolicy, color_map: Dict[str, str]
     ) -> None:
         self.__row = row
         self.__is_grayout = is_grayout
-        self.__report_color = report_color
+        self.__color_polilcy = color_polilcy
         self.__color_map = color_map
 
     def retrieve_fg_bg_color(self, base_color: str) -> Tuple[str, Optional[str]]:
         bg_color: Optional[str] = None
 
         if (self.__row % 2) == 0:
             fg_color = self.__color_map[FGColor.GRAYOUT] if self.__is_grayout else base_color
-            bg_color = BGColor.EVEN_ROW if self.__report_color == ColorPolicy.AUTO else None
+            bg_color = BGColor.EVEN_ROW if self.__color_polilcy == ColorPolicy.AUTO else None
         else:
             fg_color = self.__color_map[FGColor.GRAYOUT] if self.__is_grayout else base_color
-            bg_color = BGColor.ODD_ROW if self.__report_color == ColorPolicy.AUTO else None
+            bg_color = BGColor.ODD_ROW if self.__color_polilcy == ColorPolicy.AUTO else None
 
         return (fg_color, bg_color)
 
 
 def style_filter(cell: Cell, **kwargs: Any) -> Optional[Style]:
     writer = cast(AbstractTableWriter, kwargs["writer"])
-    report_color = cast(str, kwargs["report_color"])
+    color_policy = cast(ColorPolicy, kwargs["color_policy"])
     color_map = kwargs["color_map"]
     num_rows = cast(int, kwargs["num_rows"])
     fg_color = None
     bg_color = None
 
     is_grayout = False
     if cell.value == 0:
@@ -341,15 +347,15 @@
 
     if cell.is_header_row():
         if all([writer.value_matrix[r][cell.col] == 0 for r in range(len(writer.value_matrix))]):
             return Style(color=color_map[FGColor.GRAYOUT], font_weight="bold")
 
         return Style(font_weight="bold")
 
-    retriever = ColorRetriever(cell.row, is_grayout, report_color, color_map)
+    retriever = ColorRetriever(cell.row, is_grayout, color_policy, color_map)
     is_passed = False
     is_failed = False
     is_skipped = False
 
     headers = writer.headers
     if headers[cell.col] in (Header.FILEPATH, Header.TESTFUNC, Header.SUBTOTAL):
         error_ct_list = []
@@ -433,15 +439,18 @@
                 results_per_testfunc[key] = defaultdict(int)
             results_per_testfunc[key][stat_key] += 1
 
     return results_per_testfunc
 
 
 def make_md_report(
-    config: Config, reporter: TerminalReporter, total_stats: Mapping[str, int]
+    config: Config,
+    reporter: TerminalReporter,
+    total_stats: Mapping[str, int],
+    color_policy: ColorPolicy,
 ) -> str:
     verbosity_level = retrieve_verbosity_level(config)
 
     outcomes = ["passed", "failed", "error", "skipped", "xfailed", "xpassed"]
     outcomes = [key for key in outcomes if total_stats.get(key, 0) > 0]
     results_per_testfunc = extract_pytest_stats(
         reporter=reporter, outcomes=outcomes, verbosity_level=verbosity_level
@@ -465,18 +474,17 @@
             + [total_stats.get(key, 0) for key in outcomes]
             + [sum(total_stats.values())]
         )
 
     writer.margin = retrieve_report_margin(config)
     writer.value_matrix = matrix
 
-    report_color = retrieve_report_color(config)
-    if report_color != ColorPolicy.NEVER:
+    if color_policy != ColorPolicy.NEVER:
         writer.style_filter_kwargs = {
-            "report_color": report_color,
+            "color_policy": color_policy,
             "color_map": {
                 FGColor.SUCCESS: retrieve_report_results_color(
                     config, Option.MD_REPORT_SUCCESS_COLOR, Default.FGColor.SUCCESS
                 ),
                 FGColor.ERROR: retrieve_report_results_color(
                     config, Option.MD_REPORT_ERROR_COLOR, Default.FGColor.ERROR
                 ),
@@ -487,35 +495,54 @@
             },
             "num_rows": len(writer.value_matrix),
         }
 
         if not _is_travis_ci():
             writer.add_style_filter(style_filter)
 
-        if report_color == ColorPolicy.AUTO and not _is_ci():
+        if color_policy == ColorPolicy.AUTO and not _is_ci():
             writer.add_col_separator_style_filter(col_separator_style_filter)
 
     report_zeros = retrieve_report_zeros(config)
     if report_zeros == ZerosRender.EMPTY:
         writer.register_trans_func(zero_to_nullstr)
 
     return writer.dumps()
 
 
-def pytest_unconfigure(config):
+def pytest_unconfigure(config: Config) -> None:
     if not is_make_md_report(config):
         return
 
     reporter = config.pluginmanager.get_plugin("terminalreporter")
     stat_count_map = retrieve_stat_count_map(reporter)
-    report = make_md_report(config, reporter, stat_count_map)
-    output_filepath = retrieve_output_filepath(config)
     is_tee = retrieve_tee(config)
+    output_filepath = retrieve_output_filepath(config)
+    color_policy = retrieve_color_policy(config)
 
-    if is_tee or not output_filepath:
-        reporter._tw.write(report)
+    is_output_term = is_tee or not output_filepath
+    term_color_policy = color_policy
 
-    if not output_filepath:
+    is_output_file = is_tee or output_filepath
+    file_color_policy = color_policy
+    if is_output_file and color_policy == ColorPolicy.AUTO:
+        file_color_policy = ColorPolicy.NEVER
+
+    term_report = None
+    if is_output_term:
+        term_report = make_md_report(
+            config, reporter, stat_count_map, color_policy=term_color_policy
+        )
+        reporter._tw.write(term_report)
+
+    if not is_output_file:
         return
 
+    file_report = term_report
+    if not file_report or file_color_policy != term_color_policy:
+        file_report = make_md_report(
+            config, reporter, stat_count_map, color_policy=file_color_policy
+        )
+
+    assert output_filepath
     with open(output_filepath, "w") as f:
-        f.write(report)
+        f.write(file_report)
```

### Comparing `pytest-md-report-0.3.2/pytest_md_report.egg-info/PKG-INFO` & `pytest-md-report-0.4.0/pytest_md_report.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.3.2
+Version: 0.4.0
 Summary: A pytest plugin to make a test results report with Markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
 Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
@@ -151,83 +151,74 @@
                             you can also specify the value with PYTEST_MD_REPORT_VERBOSE environment variable.
       --md-report-output=FILEPATH
                             Path to a file to the outputs test report.
                             Overwrite a file content if the file already exists.
                             you can also specify the value with PYTEST_MD_REPORT_OUTPUT environment variable.
       --md-report-tee       output test report for both standard output and a file. you can also specify the value with PYTEST_MD_REPORT_TEE environment variable.
       --md-report-color={auto,text,never}
-                            How to color output reports.
-                            auto: render colored (text and background) reports using ANSI escape codes.
+                            How coloring output reports.
+                            auto: for terminal output, render colored (text and background) reports using ANSI escape codes.
+                            for file output, render the report without color.
                             text: render colored text reports by using ANSI escape codes.
                             never: render report without color.
-                            Defaults to 'auto'.
+                            Defaults to 'ColorPolicy.AUTO'.
                             you can also specify the value with PYTEST_MD_REPORT_COLOR environment variable.
       --md-report-margin=MARGIN
                             Margin size for each cell.
                             Defaults to 1.
                             you can also specify the value with PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
                             Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
                             Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive);
                             otherwise 'number'.
                             you can also specify the value with PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
                             Text color of succeeded results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_green'.
                             you can also specify the value with PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
       --md-report-skip-color=MD_REPORT_SKIP_COLOR
                             Text color of skipped results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_yellow'.
                             you can also specify the value with PYTEST_MD_REPORT_SKIP_COLOR environment variable.
       --md-report-error-color=MD_REPORT_ERROR_COLOR
                             Text color of failed results.
-                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
-                            color code (e.g. #ff1020).
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020).
                             Defaults to 'light_red'.
                             you can also specify the value with PYTEST_MD_REPORT_ERROR_COLOR environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
   md_report (bool):     Create Markdown report.
   md_report_verbose (string):
                         Verbosity level for pytest-md-report. If not set, use the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
-                        How to color output reports. auto: render colored (text and background) reports using ANSI escape codes. text: render colored text reports by using ANSI escape codes. never:
-                        render report without color. Defaults to 'auto'.
+                        How coloring output reports. auto: for terminal output, render colored (text and background) reports using ANSI escape codes. for file output, render the report without color. text: render colored text reports by using ANSI escape codes. never: render report without color. Defaults to
+                        'ColorPolicy.AUTO'.
   md_report_output (string):
                         Path to a file to the outputs test report. Overwrite a file content if the file already exists.
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
                         Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
-                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case
-                        insensitive); otherwise 'number'.
+                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive); otherwise 'number'.
   md_report_success_color (string):
-                        Text color of succeeded results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_green'.
+                        Text color of succeeded results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_green'.
   md_report_skip_color (string):
-                        Text color of skipped results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_yellow'.
+                        Text color of skipped results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_yellow'.
   md_report_error_color (string):
-                        Text color of failed results. Specify a color name (one of the
-                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
-                        to 'light_red'.
+                        Text color of failed results. Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults to 'light_red'.
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.3.2/pytest_md_report.egg-info/SOURCES.txt` & `pytest-md-report-0.4.0/pytest_md_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.2/setup.py` & `pytest-md-report-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.2/tests/test_option.py` & `pytest-md-report-0.4.0/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.2/tests/test_plugin.py` & `pytest-md-report-0.4.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.2/tox.ini` & `pytest-md-report-0.4.0/tox.ini`

 * *Files identical despite different names*

