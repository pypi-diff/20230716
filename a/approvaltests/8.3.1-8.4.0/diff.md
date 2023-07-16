# Comparing `tmp/approvaltests-8.3.1.tar.gz` & `tmp/approvaltests-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approvaltests-8.3.1.tar", last modified: Sun Jul  2 10:58:45 2023, max compression
+gzip compressed data, was "approvaltests-8.4.0.tar", last modified: Sun Jul 16 18:13:11 2023, max compression
```

## Comparing `approvaltests-8.3.1.tar` & `approvaltests-8.4.0.tar`

### file list

```diff
@@ -1,96 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.433962 approvaltests-8.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-02 10:58:29.000000 approvaltests-8.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-02 10:58:29.000000 approvaltests-8.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-02 10:58:45.433962 approvaltests-8.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-02 10:58:29.000000 approvaltests-8.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.425962 approvaltests-8.3.1/approvaltests/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/approval_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/binary_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/combination_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/commandline_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.429962 approvaltests-8.3.1/approvaltests/core/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/format_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/namer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/scenario_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/core/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/existing_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/file_approver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.429962 approvaltests-8.3.1/approvaltests/mrjob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/mrjob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/mrjob/mrjob_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.429962 approvaltests-8.3.1/approvaltests/namer/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/namer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/namer/cli_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/namer/default_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/namer/default_namer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/namer/namer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/namer/stack_frame_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/pairwise_combinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.429962 approvaltests-8.3.1/approvaltests/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/pytest/py_test_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporter_missing_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.429962 approvaltests-8.3.1/approvaltests/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/clipboard_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/default_reporter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/diff_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/executable_command_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/file_capture_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/first_working_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/generic_diff_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/generic_diff_reporter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/generic_diff_reporter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/multi_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/python_native_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/quiet_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/received_file_launcher_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/report_all_to_clipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/report_by_creating_diff_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/report_on_cyber_dojo.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/report_to_diff_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/report_with_beyond_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/report_with_diff_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/report_with_vscode.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/reporter_that_automatically_approves.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/reporters.json
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/reporters/testing_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.429962 approvaltests-8.3.1/approvaltests/scrubbers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/scrubbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/scrubbers/date_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/scrubbers/scrubbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/storyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/string_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.429962 approvaltests-8.3.1/approvaltests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/utilities/command_line_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.433962 approvaltests-8.3.1/approvaltests/utilities/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/utilities/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/utilities/logger/simple_logger_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.433962 approvaltests-8.3.1/approvaltests/verifiable_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/verifiable_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-02 10:58:29.000000 approvaltests-8.3.1/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 10:58:39.000000 approvaltests-8.3.1/approvaltests/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:45.425962 approvaltests-8.3.1/approvaltests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-02 10:58:45.000000 approvaltests-8.3.1/approvaltests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-02 10:58:45.000000 approvaltests-8.3.1/approvaltests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:58:45.000000 approvaltests-8.3.1/approvaltests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-02 10:58:45.000000 approvaltests-8.3.1/approvaltests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 10:58:45.000000 approvaltests-8.3.1/approvaltests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-02 10:58:29.000000 approvaltests-8.3.1/requirements.prod.extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-02 10:58:29.000000 approvaltests-8.3.1/requirements.prod.required.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 10:58:29.000000 approvaltests-8.3.1/requirements.prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 10:58:45.433962 approvaltests-8.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-02 10:58:29.000000 approvaltests-8.3.1/setup.publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-02 10:58:29.000000 approvaltests-8.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-02 10:58:29.000000 approvaltests-8.3.1/setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 10:58:39.000000 approvaltests-8.3.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-16 18:12:50.000000 approvaltests-8.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 18:12:50.000000 approvaltests-8.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-16 18:13:11.961105 approvaltests-8.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-16 18:12:50.000000 approvaltests-8.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.953105 approvaltests-8.4.0/approvaltests/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/approval_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/binary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/combination_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/commandline_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/format_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/scenario_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/existing_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/file_approver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/mrjob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/mrjob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/mrjob/mrjob_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/namer/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/cli_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/default_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/default_namer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/namer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/stack_frame_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/pairwise_combinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/pytest/py_test_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporter_missing_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/clipboard_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/default_reporter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/diff_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/executable_command_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/file_capture_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/first_working_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/multi_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/python_native_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/quiet_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/received_file_launcher_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_all_to_clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_by_creating_diff_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_on_cyber_dojo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_to_diff_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_with_beyond_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_with_diff_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_with_vscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/reporter_that_automatically_approves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/reporters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/testing_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/scrubbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/scrubbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/scrubbers/date_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/scrubbers/scrubbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/storyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/string_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/command_line_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/utilities/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logger/simple_logger_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/utilities/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logging/logging_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/verifiable_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/verifiable_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:13:05.000000 approvaltests-8.4.0/approvaltests/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.953105 approvaltests-8.4.0/approvaltests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 18:12:50.000000 approvaltests-8.4.0/requirements.prod.extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 18:12:50.000000 approvaltests-8.4.0/requirements.prod.required.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 18:12:50.000000 approvaltests-8.4.0/requirements.prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 18:13:11.961105 approvaltests-8.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-16 18:12:50.000000 approvaltests-8.4.0/setup.publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-16 18:12:50.000000 approvaltests-8.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-16 18:12:50.000000 approvaltests-8.4.0/setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:13:05.000000 approvaltests-8.4.0/version.py
```

### Comparing `approvaltests-8.3.1/LICENSE` & `approvaltests-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/PKG-INFO` & `approvaltests-8.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approvaltests
-Version: 8.3.1
+Version: 8.4.0
 Summary: Assertion/verification library to aid testing
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,20 +22,20 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ApprovalTests.Python
 
-
 <!-- toc -->
 ## Contents
 
   * [What can I use ApprovalTests for?](#what-can-i-use-approvaltests-for)
   * [Getting Started](#getting-started)
+    * [What Are Approvals](#what-are-approvals)
     * [New Projects](#new-projects)
       * [Minimal Example Tutorial](#minimal-example-tutorial)
     * [Adding to Existing Projects](#adding-to-existing-projects)
   * [Overview](#overview)
     * [Example using pytest](#example-using-pytest)
     * [Example using unittest](#example-using-unittest)
     * [Example using CLI](#example-using-cli)
@@ -44,14 +44,15 @@
   * [Reporters](#reporters)
     * [Selecting a Reporter](#selecting-a-reporter)
     * [JSON file for collection of reporters](#json-file-for-collection-of-reporters)
   * [Support and Documentation](#support-and-documentation)
     * [Missing Documentation?](#missing-documentation)
     * [Dependencies](#dependencies)
       * [Required dependencies](#required-dependencies)
+      * [Extra dependencies](#extra-dependencies)
   * [For developers](#for-developers)
     * [Weekly Ensemble](#weekly-ensemble)
     * [Pull Requests](#pull-requests)<!-- endToc -->
 
 Capturing Human Intelligence - ApprovalTests is an open source assertion/verification library to aid testing.  
 `approvaltests` is the ApprovalTests port for Python.
 
@@ -59,51 +60,52 @@
 
 [![PyPI version](https://img.shields.io/pypi/v/approvaltests.svg)](https://pypi.org/project/approvaltests)
 [![Python versions](https://img.shields.io/pypi/pyversions/approvaltests.svg)](https://pypi.org/project/approvaltests)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/Test/badge.svg?branch=master)](https://github.com/approvals/ApprovalTests.Python/actions)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/on-push-do-doco/badge.svg)](https://github.com/approvals/ApprovalTests.Python/actions?query=workflow%3Aon-push-do-doco)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/Upload%20Python%20Package/badge.svg)](https://github.com/approvals/ApprovalTests.Python/actions?query=workflow%3A%22Upload+Python+Package%22)
 
-
 ## What can I use ApprovalTests for?
 
-You can use ApprovalTests to verify objects that require more than a simple assert including long strings, large arrays, 
-and complex hash structures and objects.  ApprovalTests really shines when you need a more granular look at the test 
-failure.  Sometimes, trying to find a small difference in a long string printed to STDOUT is just too hard!  
-ApprovalTests solves this problem by providing reporters which let you view the test results in one of many popular diff 
+You can use ApprovalTests to verify objects that require more than a simple assert including long strings, large arrays,
+and complex hash structures and objects. ApprovalTests really shines when you need a more granular look at the test
+failure. Sometimes, trying to find a small difference in a long string printed to STDOUT is just too hard!  
+ApprovalTests solves this problem by providing reporters which let you view the test results in one of many popular diff
 utilities.
 
-
 ## Getting Started
 
+### What Are Approvals
+
+If you need to gain a better understanding or are new to this concept, start [here](docs/explanation/what_are_approvals.md).
+
 ### New Projects
 
 If you are starting a new project, we suggest you use the [Starter Project](https://github.com/approvals/ApprovalTests.Python.StarterProject).
 You can just clone this and go. It's great for exercises, katas, and green field projects.
 
 #### Minimal Example Tutorial
 
 If this is first time approvaltesting in python, consider starting here: [Minimal Example Tutorial](docs/tutorial/minimal-example.md)
 
-###  Adding to Existing Projects 
+### Adding to Existing Projects
 
 From [pypi](https://pypi.org/project/approvaltests/):
 
-	pip install approvaltests
+    pip install approvaltests
 
 ## Overview
 
-Approvals work by comparing the test results to a golden master.  If no golden master exists you can create a snapshot 
-of the current test results and use that as the golden master.  The reporter helps you manage the golden master.  
-Whenever your current results differ from the golden master, Approvals will launch an external application for you to 
-examine the differences.  Either you will update the master because you expected the changes and they are good,
-or you will go back to your code and update or roll back your changes to get your results back in line with the 
+Approvals work by comparing the test results to a golden master. If no golden master exists you can create a snapshot
+of the current test results and use that as the golden master. The reporter helps you manage the golden master.  
+Whenever your current results differ from the golden master, Approvals will launch an external application for you to
+examine the differences. Either you will update the master because you expected the changes and they are good,
+or you will go back to your code and update or roll back your changes to get your results back in line with the
 golden master.
 
-
 ### Example using pytest
 
 <!-- snippet: getting_started_with_pytest.py -->
 <a id='snippet-getting_started_with_pytest.py'></a>
 ```py
 from approvaltests.approvals import verify
 
@@ -116,19 +118,18 @@
 <!-- endSnippet -->
 
 Install the plugin pytest-approvaltests and use it to select a reporter:
 
     pip install pytest-approvaltests
     pytest --approvaltests-use-reporter='PythonNative'
 
-The reporter is used both to alert you to changes in your test output, and to provide a tool to update the golden 
+The reporter is used both to alert you to changes in your test output, and to provide a tool to update the golden
 master. In this snippet, we chose the 'PythonNative' reporter when we ran the tests. For more information about selecting
 reporters see [the documentation](https://github.com/approvals/ApprovalTests.Python.PytestPlugin)
 
-
 ### Example using unittest
 
 <!-- snippet: getting_started_with_unittest.py -->
 <a id='snippet-getting_started_with_unittest.py'></a>
 ```py
 import unittest
 
@@ -153,33 +154,34 @@
 You can invoke a verify() call from the command line. This allows invoking python approvals from any other stack via subprocesses.
 
 #### Usage
 
 ```
 python -m approvaltests --test-id hello --received "hello world!"
 ```
+
 or
+
 ```
 python -m approvaltests -t hello -r "hello world!"
 ```
 
-or 
+or
 
 ```
 echo "hello world!" | python -m approvaltests -t hello
 ```
 
 #### Argument Definitions
 
-- __`--test-id`__ or __`-t`__: Test identifier used to name the `approved.txt` and `received.txt` files for the test.
-
-- __`--received`__ or __`-r`__: The output of the program under test (a string) that is passed to the verify method.
+-   **`--test-id`** or **`-t`**: Test identifier used to name the `approved.txt` and `received.txt` files for the test.
 
-  - __`stdin`__: Instead of providing a `received` argument, you may use `stdin`.
+-   **`--received`** or **`-r`**: The output of the program under test (a string) that is passed to the verify method.
 
+    -   **`stdin`**: Instead of providing a `received` argument, you may use `stdin`.
 
 ## Reporters
 
 ### Selecting a Reporter
 
 All verify functions take an optional `options` parameter that can configure reporters (as well as many other aspects).
 
@@ -212,16 +214,14 @@
         verify(
             "Hello", options=Options().with_reporter(self.factory.get("BeyondCompare"))
         )
 ```
 <sup><a href='/tests/samples/test_getting_started.py#L11-L22' title='Snippet source file'>snippet source</a> | <a href='#snippet-select_reporter_from_factory' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
-
-
 Or you can build your own GenericDiffReporter on the fly
 
 <!-- snippet: custom_generic_diff_reporter -->
 <a id='snippet-custom_generic_diff_reporter'></a>
 ```py
 class GettingStartedTest(unittest.TestCase):
     def test_simple(self):
@@ -231,39 +231,30 @@
                 GenericDiffReporter.create(r"C:\my\favorite\diff\utility.exe")
             ),
         )
 ```
 <sup><a href='/tests/samples/test_getting_started.py#L34-L45' title='Snippet source file'>snippet source</a> | <a href='#snippet-custom_generic_diff_reporter' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
-As long as `C:/my/favorite/diff/utility.exe` can be invoked from the command line using the format `utility.exe file1 file2` 
-then it will be compatible with GenericDiffReporter.  Otherwise you will have to derive your own reporter, which 
+As long as `C:/my/favorite/diff/utility.exe` can be invoked from the command line using the format `utility.exe file1 file2`
+then it will be compatible with GenericDiffReporter. Otherwise you will have to derive your own reporter, which
 we won't cover here.
 
 ### JSON file for collection of reporters
 
-To wrap things up, I should note that you can completely replace the collection of reporters known to the reporter 
+To wrap things up, I should note that you can completely replace the collection of reporters known to the reporter
 factory by writing your own JSON file and loading it.
 
 For example if you had `C:/myreporters.json`
 
 ```json
 [
-    [
-        "BeyondCompare4",
-        "C:/Program Files (x86)/Beyond Compare 4/BCompare.exe"
-    ],
-    [
-        "WinMerge",
-        "C:/Program Files (x86)/WinMerge/WinMergeU.exe"
-    ],
-    [
-        "Tortoise",
-        "C:/Program Files (x86)/TortoiseSVN/bin/tortoisemerge.exe"
-    ]
+    ["BeyondCompare4", "C:/Program Files (x86)/Beyond Compare 4/BCompare.exe"],
+    ["WinMerge", "C:/Program Files (x86)/WinMerge/WinMergeU.exe"],
+    ["Tortoise", "C:/Program Files (x86)/TortoiseSVN/bin/tortoisemerge.exe"]
 ]
 ```
 
 You could then use that file by loading it into the factory:
 
 ```python
 
@@ -282,68 +273,77 @@
     def test_simple(self):
         verify('Hello', self.reporter)
 
 if __name__ == "__main__":
     unittest.main()
 ```
 
-Of course, if you have some interesting new reporters in `myreporters.json` then please consider updating the 
+Of course, if you have some interesting new reporters in `myreporters.json` then please consider updating the
 `reporters.json` file that ships with Approvals and submitting a pull request.
 
 ## Support and Documentation
 
-* [Documentation](/docs/README.md)
+-   [Documentation](/docs/README.md)
 
-* GitHub: [https://github.com/approvals/ApprovalTests.Python](https://github.com/approvals/ApprovalTests.Python)
+-   GitHub: [https://github.com/approvals/ApprovalTests.Python](https://github.com/approvals/ApprovalTests.Python)
 
-* ApprovalTests Homepage: [http://www.approvaltests.com](http://www.approvaltests.com)
+-   ApprovalTests Homepage: [http://www.approvaltests.com](http://www.approvaltests.com)
 
 ### Missing Documentation?
-If there is documentation you wish existed, please add a `page request` to [this issue](https://github.com/approvals/ApprovalTests.Python/issues/135).
 
+If there is documentation you wish existed, please add a `page request` to [this issue](https://github.com/approvals/ApprovalTests.Python/issues/135).
 
 ### Dependencies
 
 ApprovalTests require Python 3.7 or greater and the following dependencies:
+
 #### Required dependencies
+
 These dependencies are always required for approvaltests
+
 <!-- snippet: requirements.prod.required.txt -->
 <a id='snippet-requirements.prod.required.txt'></a>
 ```txt
 pytest>=4.0.0
 empty-files>=0.0.3
 typing_extensions>=3.6.2
 ```
 <sup><a href='/requirements.prod.required.txt#L1-L5' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.required.txt' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
+
 #### Extra dependencies
+
 These dependencies are required if you are going to use the related functionality
-If you want the bare minimum you can use the pypi project 
-[approvaltests-minimal](https://pypi.org/project/approvaltests-minimal/) 
+If you want the bare minimum you can use the pypi project
+[approvaltests-minimal](https://pypi.org/project/approvaltests-minimal/)
 
 <!-- snippet: requirements.prod.extras.txt -->
 <a id='snippet-requirements.prod.extras.txt'></a>
 ```txt
 pyperclip>=1.5.29     # For Clipboard Reporter
 beautifulsoup4>=4.4.0 # For verify_html
 allpairspy>=2.1.0     # For PairwiseCombinations
 mrjob>=0.7.4          # For MrJob
+testfixtures >= 7.1.0 # For verify_logging
+mock >= 5.1.0         # For verify_logging
 ```
-<sup><a href='/requirements.prod.extras.txt#L1-L4' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.extras.txt' title='Start of snippet'>anchor</a></sup>
+<sup><a href='/requirements.prod.extras.txt#L1-L6' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.extras.txt' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
 ## For developers
+
 ### Weekly Ensemble
 
 The best way to contribute is to [join our weekly mob/ensemble](./docs/Contribute.md)
 
 ### Pull Requests
+
 Pull requests are welcomed, particularly those accompanied by automated tests.
 
 To run the self-tests, install pytest and tox, then execute
 
     python -m tox
 
-This will run the self-tests on several python versions. We support python 3.7 and above. 
+This will run the self-tests on several python versions. We support python 3.7 and above.
 
 All pull requests will be pre-checked using GitHub actions to execute all these tests. You can see the [results of test
 runs here](https://github.com/approvals/ApprovalTests.Python/actions).
```

### Comparing `approvaltests-8.3.1/README.md` & `approvaltests-8.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ApprovalTests.Python
 
-
 <!-- toc -->
 ## Contents
 
   * [What can I use ApprovalTests for?](#what-can-i-use-approvaltests-for)
   * [Getting Started](#getting-started)
+    * [What Are Approvals](#what-are-approvals)
     * [New Projects](#new-projects)
       * [Minimal Example Tutorial](#minimal-example-tutorial)
     * [Adding to Existing Projects](#adding-to-existing-projects)
   * [Overview](#overview)
     * [Example using pytest](#example-using-pytest)
     * [Example using unittest](#example-using-unittest)
     * [Example using CLI](#example-using-cli)
@@ -18,14 +18,15 @@
   * [Reporters](#reporters)
     * [Selecting a Reporter](#selecting-a-reporter)
     * [JSON file for collection of reporters](#json-file-for-collection-of-reporters)
   * [Support and Documentation](#support-and-documentation)
     * [Missing Documentation?](#missing-documentation)
     * [Dependencies](#dependencies)
       * [Required dependencies](#required-dependencies)
+      * [Extra dependencies](#extra-dependencies)
   * [For developers](#for-developers)
     * [Weekly Ensemble](#weekly-ensemble)
     * [Pull Requests](#pull-requests)<!-- endToc -->
 
 Capturing Human Intelligence - ApprovalTests is an open source assertion/verification library to aid testing.  
 `approvaltests` is the ApprovalTests port for Python.
 
@@ -33,51 +34,52 @@
 
 [![PyPI version](https://img.shields.io/pypi/v/approvaltests.svg)](https://pypi.org/project/approvaltests)
 [![Python versions](https://img.shields.io/pypi/pyversions/approvaltests.svg)](https://pypi.org/project/approvaltests)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/Test/badge.svg?branch=master)](https://github.com/approvals/ApprovalTests.Python/actions)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/on-push-do-doco/badge.svg)](https://github.com/approvals/ApprovalTests.Python/actions?query=workflow%3Aon-push-do-doco)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/Upload%20Python%20Package/badge.svg)](https://github.com/approvals/ApprovalTests.Python/actions?query=workflow%3A%22Upload+Python+Package%22)
 
-
 ## What can I use ApprovalTests for?
 
-You can use ApprovalTests to verify objects that require more than a simple assert including long strings, large arrays, 
-and complex hash structures and objects.  ApprovalTests really shines when you need a more granular look at the test 
-failure.  Sometimes, trying to find a small difference in a long string printed to STDOUT is just too hard!  
-ApprovalTests solves this problem by providing reporters which let you view the test results in one of many popular diff 
+You can use ApprovalTests to verify objects that require more than a simple assert including long strings, large arrays,
+and complex hash structures and objects. ApprovalTests really shines when you need a more granular look at the test
+failure. Sometimes, trying to find a small difference in a long string printed to STDOUT is just too hard!  
+ApprovalTests solves this problem by providing reporters which let you view the test results in one of many popular diff
 utilities.
 
-
 ## Getting Started
 
+### What Are Approvals
+
+If you need to gain a better understanding or are new to this concept, start [here](docs/explanation/what_are_approvals.md).
+
 ### New Projects
 
 If you are starting a new project, we suggest you use the [Starter Project](https://github.com/approvals/ApprovalTests.Python.StarterProject).
 You can just clone this and go. It's great for exercises, katas, and green field projects.
 
 #### Minimal Example Tutorial
 
 If this is first time approvaltesting in python, consider starting here: [Minimal Example Tutorial](docs/tutorial/minimal-example.md)
 
-###  Adding to Existing Projects 
+### Adding to Existing Projects
 
 From [pypi](https://pypi.org/project/approvaltests/):
 
-	pip install approvaltests
+    pip install approvaltests
 
 ## Overview
 
-Approvals work by comparing the test results to a golden master.  If no golden master exists you can create a snapshot 
-of the current test results and use that as the golden master.  The reporter helps you manage the golden master.  
-Whenever your current results differ from the golden master, Approvals will launch an external application for you to 
-examine the differences.  Either you will update the master because you expected the changes and they are good,
-or you will go back to your code and update or roll back your changes to get your results back in line with the 
+Approvals work by comparing the test results to a golden master. If no golden master exists you can create a snapshot
+of the current test results and use that as the golden master. The reporter helps you manage the golden master.  
+Whenever your current results differ from the golden master, Approvals will launch an external application for you to
+examine the differences. Either you will update the master because you expected the changes and they are good,
+or you will go back to your code and update or roll back your changes to get your results back in line with the
 golden master.
 
-
 ### Example using pytest
 
 <!-- snippet: getting_started_with_pytest.py -->
 <a id='snippet-getting_started_with_pytest.py'></a>
 ```py
 from approvaltests.approvals import verify
 
@@ -90,19 +92,18 @@
 <!-- endSnippet -->
 
 Install the plugin pytest-approvaltests and use it to select a reporter:
 
     pip install pytest-approvaltests
     pytest --approvaltests-use-reporter='PythonNative'
 
-The reporter is used both to alert you to changes in your test output, and to provide a tool to update the golden 
+The reporter is used both to alert you to changes in your test output, and to provide a tool to update the golden
 master. In this snippet, we chose the 'PythonNative' reporter when we ran the tests. For more information about selecting
 reporters see [the documentation](https://github.com/approvals/ApprovalTests.Python.PytestPlugin)
 
-
 ### Example using unittest
 
 <!-- snippet: getting_started_with_unittest.py -->
 <a id='snippet-getting_started_with_unittest.py'></a>
 ```py
 import unittest
 
@@ -127,33 +128,34 @@
 You can invoke a verify() call from the command line. This allows invoking python approvals from any other stack via subprocesses.
 
 #### Usage
 
 ```
 python -m approvaltests --test-id hello --received "hello world!"
 ```
+
 or
+
 ```
 python -m approvaltests -t hello -r "hello world!"
 ```
 
-or 
+or
 
 ```
 echo "hello world!" | python -m approvaltests -t hello
 ```
 
 #### Argument Definitions
 
-- __`--test-id`__ or __`-t`__: Test identifier used to name the `approved.txt` and `received.txt` files for the test.
-
-- __`--received`__ or __`-r`__: The output of the program under test (a string) that is passed to the verify method.
+-   **`--test-id`** or **`-t`**: Test identifier used to name the `approved.txt` and `received.txt` files for the test.
 
-  - __`stdin`__: Instead of providing a `received` argument, you may use `stdin`.
+-   **`--received`** or **`-r`**: The output of the program under test (a string) that is passed to the verify method.
 
+    -   **`stdin`**: Instead of providing a `received` argument, you may use `stdin`.
 
 ## Reporters
 
 ### Selecting a Reporter
 
 All verify functions take an optional `options` parameter that can configure reporters (as well as many other aspects).
 
@@ -186,16 +188,14 @@
         verify(
             "Hello", options=Options().with_reporter(self.factory.get("BeyondCompare"))
         )
 ```
 <sup><a href='/tests/samples/test_getting_started.py#L11-L22' title='Snippet source file'>snippet source</a> | <a href='#snippet-select_reporter_from_factory' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
-
-
 Or you can build your own GenericDiffReporter on the fly
 
 <!-- snippet: custom_generic_diff_reporter -->
 <a id='snippet-custom_generic_diff_reporter'></a>
 ```py
 class GettingStartedTest(unittest.TestCase):
     def test_simple(self):
@@ -205,39 +205,30 @@
                 GenericDiffReporter.create(r"C:\my\favorite\diff\utility.exe")
             ),
         )
 ```
 <sup><a href='/tests/samples/test_getting_started.py#L34-L45' title='Snippet source file'>snippet source</a> | <a href='#snippet-custom_generic_diff_reporter' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
-As long as `C:/my/favorite/diff/utility.exe` can be invoked from the command line using the format `utility.exe file1 file2` 
-then it will be compatible with GenericDiffReporter.  Otherwise you will have to derive your own reporter, which 
+As long as `C:/my/favorite/diff/utility.exe` can be invoked from the command line using the format `utility.exe file1 file2`
+then it will be compatible with GenericDiffReporter. Otherwise you will have to derive your own reporter, which
 we won't cover here.
 
 ### JSON file for collection of reporters
 
-To wrap things up, I should note that you can completely replace the collection of reporters known to the reporter 
+To wrap things up, I should note that you can completely replace the collection of reporters known to the reporter
 factory by writing your own JSON file and loading it.
 
 For example if you had `C:/myreporters.json`
 
 ```json
 [
-    [
-        "BeyondCompare4",
-        "C:/Program Files (x86)/Beyond Compare 4/BCompare.exe"
-    ],
-    [
-        "WinMerge",
-        "C:/Program Files (x86)/WinMerge/WinMergeU.exe"
-    ],
-    [
-        "Tortoise",
-        "C:/Program Files (x86)/TortoiseSVN/bin/tortoisemerge.exe"
-    ]
+    ["BeyondCompare4", "C:/Program Files (x86)/Beyond Compare 4/BCompare.exe"],
+    ["WinMerge", "C:/Program Files (x86)/WinMerge/WinMergeU.exe"],
+    ["Tortoise", "C:/Program Files (x86)/TortoiseSVN/bin/tortoisemerge.exe"]
 ]
 ```
 
 You could then use that file by loading it into the factory:
 
 ```python
 
@@ -256,68 +247,77 @@
     def test_simple(self):
         verify('Hello', self.reporter)
 
 if __name__ == "__main__":
     unittest.main()
 ```
 
-Of course, if you have some interesting new reporters in `myreporters.json` then please consider updating the 
+Of course, if you have some interesting new reporters in `myreporters.json` then please consider updating the
 `reporters.json` file that ships with Approvals and submitting a pull request.
 
 ## Support and Documentation
 
-* [Documentation](/docs/README.md)
+-   [Documentation](/docs/README.md)
 
-* GitHub: [https://github.com/approvals/ApprovalTests.Python](https://github.com/approvals/ApprovalTests.Python)
+-   GitHub: [https://github.com/approvals/ApprovalTests.Python](https://github.com/approvals/ApprovalTests.Python)
 
-* ApprovalTests Homepage: [http://www.approvaltests.com](http://www.approvaltests.com)
+-   ApprovalTests Homepage: [http://www.approvaltests.com](http://www.approvaltests.com)
 
 ### Missing Documentation?
-If there is documentation you wish existed, please add a `page request` to [this issue](https://github.com/approvals/ApprovalTests.Python/issues/135).
 
+If there is documentation you wish existed, please add a `page request` to [this issue](https://github.com/approvals/ApprovalTests.Python/issues/135).
 
 ### Dependencies
 
 ApprovalTests require Python 3.7 or greater and the following dependencies:
+
 #### Required dependencies
+
 These dependencies are always required for approvaltests
+
 <!-- snippet: requirements.prod.required.txt -->
 <a id='snippet-requirements.prod.required.txt'></a>
 ```txt
 pytest>=4.0.0
 empty-files>=0.0.3
 typing_extensions>=3.6.2
 ```
 <sup><a href='/requirements.prod.required.txt#L1-L5' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.required.txt' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
+
 #### Extra dependencies
+
 These dependencies are required if you are going to use the related functionality
-If you want the bare minimum you can use the pypi project 
-[approvaltests-minimal](https://pypi.org/project/approvaltests-minimal/) 
+If you want the bare minimum you can use the pypi project
+[approvaltests-minimal](https://pypi.org/project/approvaltests-minimal/)
 
 <!-- snippet: requirements.prod.extras.txt -->
 <a id='snippet-requirements.prod.extras.txt'></a>
 ```txt
 pyperclip>=1.5.29     # For Clipboard Reporter
 beautifulsoup4>=4.4.0 # For verify_html
 allpairspy>=2.1.0     # For PairwiseCombinations
 mrjob>=0.7.4          # For MrJob
+testfixtures >= 7.1.0 # For verify_logging
+mock >= 5.1.0         # For verify_logging
 ```
-<sup><a href='/requirements.prod.extras.txt#L1-L4' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.extras.txt' title='Start of snippet'>anchor</a></sup>
+<sup><a href='/requirements.prod.extras.txt#L1-L6' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.extras.txt' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
 ## For developers
+
 ### Weekly Ensemble
 
 The best way to contribute is to [join our weekly mob/ensemble](./docs/Contribute.md)
 
 ### Pull Requests
+
 Pull requests are welcomed, particularly those accompanied by automated tests.
 
 To run the self-tests, install pytest and tox, then execute
 
     python -m tox
 
-This will run the self-tests on several python versions. We support python 3.7 and above. 
+This will run the self-tests on several python versions. We support python 3.7 and above.
 
 All pull requests will be pre-checked using GitHub actions to execute all these tests. You can see the [results of test
 runs here](https://github.com/approvals/ApprovalTests.Python/actions).
```

### Comparing `approvaltests-8.3.1/approvaltests/approvals.py` & `approvaltests-8.4.0/approvaltests/approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/asserts.py` & `approvaltests-8.4.0/approvaltests/asserts.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/binary_writer.py` & `approvaltests-8.4.0/approvaltests/binary_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/combination_approvals.py` & `approvaltests-8.4.0/approvaltests/combination_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/command.py` & `approvaltests-8.4.0/approvaltests/command.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/commandline_interface.py` & `approvaltests-8.4.0/approvaltests/commandline_interface.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/core/comparator.py` & `approvaltests-8.4.0/approvaltests/core/comparator.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/core/options.py` & `approvaltests-8.4.0/approvaltests/core/options.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/core/reporter.py` & `approvaltests-8.4.0/approvaltests/core/reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/core/scenario_namer.py` & `approvaltests-8.4.0/approvaltests/core/scenario_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/existing_file_writer.py` & `approvaltests-8.4.0/approvaltests/existing_file_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/file_approver.py` & `approvaltests-8.4.0/approvaltests/file_approver.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/mrjob/mrjob_approvals.py` & `approvaltests-8.4.0/approvaltests/mrjob/mrjob_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/namer/default_namer_factory.py` & `approvaltests-8.4.0/approvaltests/namer/default_namer_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/namer/namer_base.py` & `approvaltests-8.4.0/approvaltests/namer/namer_base.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/namer/stack_frame_namer.py` & `approvaltests-8.4.0/approvaltests/namer/stack_frame_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/pytest/py_test_namer.py` & `approvaltests-8.4.0/approvaltests/pytest/py_test_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/__init__.py` & `approvaltests-8.4.0/approvaltests/reporters/__init__.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/clipboard_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/clipboard_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/default_reporter_factory.py` & `approvaltests-8.4.0/approvaltests/reporters/default_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/diff_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/diff_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/executable_command_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/executable_command_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/file_capture_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/file_capture_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/first_working_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/first_working_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/generic_diff_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/generic_diff_reporter_factory.py` & `approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/python_native_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/python_native_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/received_file_launcher_reporter.py` & `approvaltests-8.4.0/approvaltests/reporters/received_file_launcher_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/report_all_to_clipboard.py` & `approvaltests-8.4.0/approvaltests/reporters/report_all_to_clipboard.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/report_by_creating_diff_file.py` & `approvaltests-8.4.0/approvaltests/reporters/report_by_creating_diff_file.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/report_to_diff_engine.py` & `approvaltests-8.4.0/approvaltests/reporters/report_to_diff_engine.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/report_with_beyond_compare.py` & `approvaltests-8.4.0/approvaltests/reporters/report_with_beyond_compare.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/reporters/reporters.json` & `approvaltests-8.4.0/approvaltests/reporters/reporters.json`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/scrubbers/date_scrubber.py` & `approvaltests-8.4.0/approvaltests/scrubbers/date_scrubber.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,18 @@
                 "\\d{4}-\\d{1,2}-\\d{1,2}T\\d{1,2}:\\d{2}:\\d{2}Z",
                 ["2020-09-10T08:07:89Z"],
             ),
             (
                 "\\d{4}-\\d{1,2}-\\d{1,2}T\\d{1,2}:\\d{2}\\:\\d{2}\\.\\d{3}Z",
                 ["2020-09-10T01:23:45.678Z"],
             ),
+            (
+                "\\d{4}-\\d{1,2}-\\d{1,2} \\d{1,2}:\\d{2}\\:\\d{2}\\.\\d{6}",
+                ["2023-07-16 17:39:03.293919"],
+            ),
             ("\\d{8}T\\d{6}Z", ["20210505T091112Z"]),
         ]
 
     def __init__(self, date_regex: str):
         self.date_regex = date_regex
 
     def scrub(self, date_str: str):
```

### Comparing `approvaltests-8.3.1/approvaltests/scrubbers/scrubbers.py` & `approvaltests-8.4.0/approvaltests/scrubbers/scrubbers.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/storyboard.py` & `approvaltests-8.4.0/approvaltests/storyboard.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/string_writer.py` & `approvaltests-8.4.0/approvaltests/string_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/utilities/command_line_approvals.py` & `approvaltests-8.4.0/approvaltests/utilities/command_line_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/utilities/logger/simple_logger_approvals.py` & `approvaltests-8.4.0/approvaltests/utilities/logger/simple_logger_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py` & `approvaltests-8.4.0/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.3.1/approvaltests.egg-info/PKG-INFO` & `approvaltests-8.4.0/approvaltests.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approvaltests
-Version: 8.3.1
+Version: 8.4.0
 Summary: Assertion/verification library to aid testing
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,20 +22,20 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ApprovalTests.Python
 
-
 <!-- toc -->
 ## Contents
 
   * [What can I use ApprovalTests for?](#what-can-i-use-approvaltests-for)
   * [Getting Started](#getting-started)
+    * [What Are Approvals](#what-are-approvals)
     * [New Projects](#new-projects)
       * [Minimal Example Tutorial](#minimal-example-tutorial)
     * [Adding to Existing Projects](#adding-to-existing-projects)
   * [Overview](#overview)
     * [Example using pytest](#example-using-pytest)
     * [Example using unittest](#example-using-unittest)
     * [Example using CLI](#example-using-cli)
@@ -44,14 +44,15 @@
   * [Reporters](#reporters)
     * [Selecting a Reporter](#selecting-a-reporter)
     * [JSON file for collection of reporters](#json-file-for-collection-of-reporters)
   * [Support and Documentation](#support-and-documentation)
     * [Missing Documentation?](#missing-documentation)
     * [Dependencies](#dependencies)
       * [Required dependencies](#required-dependencies)
+      * [Extra dependencies](#extra-dependencies)
   * [For developers](#for-developers)
     * [Weekly Ensemble](#weekly-ensemble)
     * [Pull Requests](#pull-requests)<!-- endToc -->
 
 Capturing Human Intelligence - ApprovalTests is an open source assertion/verification library to aid testing.  
 `approvaltests` is the ApprovalTests port for Python.
 
@@ -59,51 +60,52 @@
 
 [![PyPI version](https://img.shields.io/pypi/v/approvaltests.svg)](https://pypi.org/project/approvaltests)
 [![Python versions](https://img.shields.io/pypi/pyversions/approvaltests.svg)](https://pypi.org/project/approvaltests)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/Test/badge.svg?branch=master)](https://github.com/approvals/ApprovalTests.Python/actions)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/on-push-do-doco/badge.svg)](https://github.com/approvals/ApprovalTests.Python/actions?query=workflow%3Aon-push-do-doco)
 [![Build Status](https://github.com/approvals/ApprovalTests.Python/workflows/Upload%20Python%20Package/badge.svg)](https://github.com/approvals/ApprovalTests.Python/actions?query=workflow%3A%22Upload+Python+Package%22)
 
-
 ## What can I use ApprovalTests for?
 
-You can use ApprovalTests to verify objects that require more than a simple assert including long strings, large arrays, 
-and complex hash structures and objects.  ApprovalTests really shines when you need a more granular look at the test 
-failure.  Sometimes, trying to find a small difference in a long string printed to STDOUT is just too hard!  
-ApprovalTests solves this problem by providing reporters which let you view the test results in one of many popular diff 
+You can use ApprovalTests to verify objects that require more than a simple assert including long strings, large arrays,
+and complex hash structures and objects. ApprovalTests really shines when you need a more granular look at the test
+failure. Sometimes, trying to find a small difference in a long string printed to STDOUT is just too hard!  
+ApprovalTests solves this problem by providing reporters which let you view the test results in one of many popular diff
 utilities.
 
-
 ## Getting Started
 
+### What Are Approvals
+
+If you need to gain a better understanding or are new to this concept, start [here](docs/explanation/what_are_approvals.md).
+
 ### New Projects
 
 If you are starting a new project, we suggest you use the [Starter Project](https://github.com/approvals/ApprovalTests.Python.StarterProject).
 You can just clone this and go. It's great for exercises, katas, and green field projects.
 
 #### Minimal Example Tutorial
 
 If this is first time approvaltesting in python, consider starting here: [Minimal Example Tutorial](docs/tutorial/minimal-example.md)
 
-###  Adding to Existing Projects 
+### Adding to Existing Projects
 
 From [pypi](https://pypi.org/project/approvaltests/):
 
-	pip install approvaltests
+    pip install approvaltests
 
 ## Overview
 
-Approvals work by comparing the test results to a golden master.  If no golden master exists you can create a snapshot 
-of the current test results and use that as the golden master.  The reporter helps you manage the golden master.  
-Whenever your current results differ from the golden master, Approvals will launch an external application for you to 
-examine the differences.  Either you will update the master because you expected the changes and they are good,
-or you will go back to your code and update or roll back your changes to get your results back in line with the 
+Approvals work by comparing the test results to a golden master. If no golden master exists you can create a snapshot
+of the current test results and use that as the golden master. The reporter helps you manage the golden master.  
+Whenever your current results differ from the golden master, Approvals will launch an external application for you to
+examine the differences. Either you will update the master because you expected the changes and they are good,
+or you will go back to your code and update or roll back your changes to get your results back in line with the
 golden master.
 
-
 ### Example using pytest
 
 <!-- snippet: getting_started_with_pytest.py -->
 <a id='snippet-getting_started_with_pytest.py'></a>
 ```py
 from approvaltests.approvals import verify
 
@@ -116,19 +118,18 @@
 <!-- endSnippet -->
 
 Install the plugin pytest-approvaltests and use it to select a reporter:
 
     pip install pytest-approvaltests
     pytest --approvaltests-use-reporter='PythonNative'
 
-The reporter is used both to alert you to changes in your test output, and to provide a tool to update the golden 
+The reporter is used both to alert you to changes in your test output, and to provide a tool to update the golden
 master. In this snippet, we chose the 'PythonNative' reporter when we ran the tests. For more information about selecting
 reporters see [the documentation](https://github.com/approvals/ApprovalTests.Python.PytestPlugin)
 
-
 ### Example using unittest
 
 <!-- snippet: getting_started_with_unittest.py -->
 <a id='snippet-getting_started_with_unittest.py'></a>
 ```py
 import unittest
 
@@ -153,33 +154,34 @@
 You can invoke a verify() call from the command line. This allows invoking python approvals from any other stack via subprocesses.
 
 #### Usage
 
 ```
 python -m approvaltests --test-id hello --received "hello world!"
 ```
+
 or
+
 ```
 python -m approvaltests -t hello -r "hello world!"
 ```
 
-or 
+or
 
 ```
 echo "hello world!" | python -m approvaltests -t hello
 ```
 
 #### Argument Definitions
 
-- __`--test-id`__ or __`-t`__: Test identifier used to name the `approved.txt` and `received.txt` files for the test.
-
-- __`--received`__ or __`-r`__: The output of the program under test (a string) that is passed to the verify method.
+-   **`--test-id`** or **`-t`**: Test identifier used to name the `approved.txt` and `received.txt` files for the test.
 
-  - __`stdin`__: Instead of providing a `received` argument, you may use `stdin`.
+-   **`--received`** or **`-r`**: The output of the program under test (a string) that is passed to the verify method.
 
+    -   **`stdin`**: Instead of providing a `received` argument, you may use `stdin`.
 
 ## Reporters
 
 ### Selecting a Reporter
 
 All verify functions take an optional `options` parameter that can configure reporters (as well as many other aspects).
 
@@ -212,16 +214,14 @@
         verify(
             "Hello", options=Options().with_reporter(self.factory.get("BeyondCompare"))
         )
 ```
 <sup><a href='/tests/samples/test_getting_started.py#L11-L22' title='Snippet source file'>snippet source</a> | <a href='#snippet-select_reporter_from_factory' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
-
-
 Or you can build your own GenericDiffReporter on the fly
 
 <!-- snippet: custom_generic_diff_reporter -->
 <a id='snippet-custom_generic_diff_reporter'></a>
 ```py
 class GettingStartedTest(unittest.TestCase):
     def test_simple(self):
@@ -231,39 +231,30 @@
                 GenericDiffReporter.create(r"C:\my\favorite\diff\utility.exe")
             ),
         )
 ```
 <sup><a href='/tests/samples/test_getting_started.py#L34-L45' title='Snippet source file'>snippet source</a> | <a href='#snippet-custom_generic_diff_reporter' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
-As long as `C:/my/favorite/diff/utility.exe` can be invoked from the command line using the format `utility.exe file1 file2` 
-then it will be compatible with GenericDiffReporter.  Otherwise you will have to derive your own reporter, which 
+As long as `C:/my/favorite/diff/utility.exe` can be invoked from the command line using the format `utility.exe file1 file2`
+then it will be compatible with GenericDiffReporter. Otherwise you will have to derive your own reporter, which
 we won't cover here.
 
 ### JSON file for collection of reporters
 
-To wrap things up, I should note that you can completely replace the collection of reporters known to the reporter 
+To wrap things up, I should note that you can completely replace the collection of reporters known to the reporter
 factory by writing your own JSON file and loading it.
 
 For example if you had `C:/myreporters.json`
 
 ```json
 [
-    [
-        "BeyondCompare4",
-        "C:/Program Files (x86)/Beyond Compare 4/BCompare.exe"
-    ],
-    [
-        "WinMerge",
-        "C:/Program Files (x86)/WinMerge/WinMergeU.exe"
-    ],
-    [
-        "Tortoise",
-        "C:/Program Files (x86)/TortoiseSVN/bin/tortoisemerge.exe"
-    ]
+    ["BeyondCompare4", "C:/Program Files (x86)/Beyond Compare 4/BCompare.exe"],
+    ["WinMerge", "C:/Program Files (x86)/WinMerge/WinMergeU.exe"],
+    ["Tortoise", "C:/Program Files (x86)/TortoiseSVN/bin/tortoisemerge.exe"]
 ]
 ```
 
 You could then use that file by loading it into the factory:
 
 ```python
 
@@ -282,68 +273,77 @@
     def test_simple(self):
         verify('Hello', self.reporter)
 
 if __name__ == "__main__":
     unittest.main()
 ```
 
-Of course, if you have some interesting new reporters in `myreporters.json` then please consider updating the 
+Of course, if you have some interesting new reporters in `myreporters.json` then please consider updating the
 `reporters.json` file that ships with Approvals and submitting a pull request.
 
 ## Support and Documentation
 
-* [Documentation](/docs/README.md)
+-   [Documentation](/docs/README.md)
 
-* GitHub: [https://github.com/approvals/ApprovalTests.Python](https://github.com/approvals/ApprovalTests.Python)
+-   GitHub: [https://github.com/approvals/ApprovalTests.Python](https://github.com/approvals/ApprovalTests.Python)
 
-* ApprovalTests Homepage: [http://www.approvaltests.com](http://www.approvaltests.com)
+-   ApprovalTests Homepage: [http://www.approvaltests.com](http://www.approvaltests.com)
 
 ### Missing Documentation?
-If there is documentation you wish existed, please add a `page request` to [this issue](https://github.com/approvals/ApprovalTests.Python/issues/135).
 
+If there is documentation you wish existed, please add a `page request` to [this issue](https://github.com/approvals/ApprovalTests.Python/issues/135).
 
 ### Dependencies
 
 ApprovalTests require Python 3.7 or greater and the following dependencies:
+
 #### Required dependencies
+
 These dependencies are always required for approvaltests
+
 <!-- snippet: requirements.prod.required.txt -->
 <a id='snippet-requirements.prod.required.txt'></a>
 ```txt
 pytest>=4.0.0
 empty-files>=0.0.3
 typing_extensions>=3.6.2
 ```
 <sup><a href='/requirements.prod.required.txt#L1-L5' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.required.txt' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
+
 #### Extra dependencies
+
 These dependencies are required if you are going to use the related functionality
-If you want the bare minimum you can use the pypi project 
-[approvaltests-minimal](https://pypi.org/project/approvaltests-minimal/) 
+If you want the bare minimum you can use the pypi project
+[approvaltests-minimal](https://pypi.org/project/approvaltests-minimal/)
 
 <!-- snippet: requirements.prod.extras.txt -->
 <a id='snippet-requirements.prod.extras.txt'></a>
 ```txt
 pyperclip>=1.5.29     # For Clipboard Reporter
 beautifulsoup4>=4.4.0 # For verify_html
 allpairspy>=2.1.0     # For PairwiseCombinations
 mrjob>=0.7.4          # For MrJob
+testfixtures >= 7.1.0 # For verify_logging
+mock >= 5.1.0         # For verify_logging
 ```
-<sup><a href='/requirements.prod.extras.txt#L1-L4' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.extras.txt' title='Start of snippet'>anchor</a></sup>
+<sup><a href='/requirements.prod.extras.txt#L1-L6' title='Snippet source file'>snippet source</a> | <a href='#snippet-requirements.prod.extras.txt' title='Start of snippet'>anchor</a></sup>
 <!-- endSnippet -->
 
 ## For developers
+
 ### Weekly Ensemble
 
 The best way to contribute is to [join our weekly mob/ensemble](./docs/Contribute.md)
 
 ### Pull Requests
+
 Pull requests are welcomed, particularly those accompanied by automated tests.
 
 To run the self-tests, install pytest and tox, then execute
 
     python -m tox
 
-This will run the self-tests on several python versions. We support python 3.7 and above. 
+This will run the self-tests on several python versions. We support python 3.7 and above.
 
 All pull requests will be pre-checked using GitHub actions to execute all these tests. You can see the [results of test
 runs here](https://github.com/approvals/ApprovalTests.Python/actions).
```

### Comparing `approvaltests-8.3.1/approvaltests.egg-info/SOURCES.txt` & `approvaltests-8.4.0/approvaltests.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -75,9 +75,11 @@
 approvaltests/scrubbers/__init__.py
 approvaltests/scrubbers/date_scrubber.py
 approvaltests/scrubbers/scrubbers.py
 approvaltests/utilities/__init__.py
 approvaltests/utilities/command_line_approvals.py
 approvaltests/utilities/logger/__init__.py
 approvaltests/utilities/logger/simple_logger_approvals.py
+approvaltests/utilities/logging/__init__.py
+approvaltests/utilities/logging/logging_approvals.py
 approvaltests/verifiable_objects/__init__.py
 approvaltests/verifiable_objects/formatter_of_argparse_namespace.py
```

### Comparing `approvaltests-8.3.1/setup_utils.py` & `approvaltests-8.4.0/setup_utils.py`

 * *Files identical despite different names*

