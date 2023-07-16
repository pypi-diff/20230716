# Comparing `tmp/approvaltests-8.4.0.tar.gz` & `tmp/approvaltests-8.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approvaltests-8.4.0.tar", last modified: Sun Jul 16 18:13:11 2023, max compression
+gzip compressed data, was "approvaltests-8.4.1.tar", last modified: Sun Jul 16 18:37:47 2023, max compression
```

## Comparing `approvaltests-8.4.0.tar` & `approvaltests-8.4.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-16 18:12:50.000000 approvaltests-8.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 18:12:50.000000 approvaltests-8.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-16 18:13:11.961105 approvaltests-8.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-16 18:12:50.000000 approvaltests-8.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.953105 approvaltests-8.4.0/approvaltests/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/approval_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/binary_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/combination_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/commandline_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/core/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/format_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/namer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/scenario_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/core/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/existing_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/file_approver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/mrjob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/mrjob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/mrjob/mrjob_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/namer/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/cli_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/default_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/default_namer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/namer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/namer/stack_frame_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/pairwise_combinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.957105 approvaltests-8.4.0/approvaltests/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/pytest/py_test_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporter_missing_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/clipboard_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/default_reporter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/diff_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/executable_command_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/file_capture_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/first_working_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/multi_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/python_native_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/quiet_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/received_file_launcher_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_all_to_clipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_by_creating_diff_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_on_cyber_dojo.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_to_diff_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_with_beyond_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_with_diff_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/report_with_vscode.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/reporter_that_automatically_approves.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/reporters.json
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/reporters/testing_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/scrubbers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/scrubbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/scrubbers/date_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/scrubbers/scrubbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/storyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/string_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/command_line_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/utilities/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logger/simple_logger_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/utilities/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/utilities/logging/logging_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.961105 approvaltests-8.4.0/approvaltests/verifiable_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/verifiable_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-16 18:12:50.000000 approvaltests-8.4.0/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:13:05.000000 approvaltests-8.4.0/approvaltests/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:11.953105 approvaltests-8.4.0/approvaltests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 18:13:11.000000 approvaltests-8.4.0/approvaltests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 18:12:50.000000 approvaltests-8.4.0/requirements.prod.extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 18:12:50.000000 approvaltests-8.4.0/requirements.prod.required.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 18:12:50.000000 approvaltests-8.4.0/requirements.prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 18:13:11.961105 approvaltests-8.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-16 18:12:50.000000 approvaltests-8.4.0/setup.publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-16 18:12:50.000000 approvaltests-8.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-16 18:12:50.000000 approvaltests-8.4.0/setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:13:05.000000 approvaltests-8.4.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.478899 approvaltests-8.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-16 18:37:30.000000 approvaltests-8.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 18:37:30.000000 approvaltests-8.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-16 18:37:47.478899 approvaltests-8.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-16 18:37:30.000000 approvaltests-8.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.474899 approvaltests-8.4.1/approvaltests/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/approval_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/binary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/combination_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/commandline_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.474899 approvaltests-8.4.1/approvaltests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/format_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/scenario_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/core/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/existing_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/file_approver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.474899 approvaltests-8.4.1/approvaltests/mrjob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/mrjob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/mrjob/mrjob_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.474899 approvaltests-8.4.1/approvaltests/namer/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/namer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/namer/cli_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/namer/default_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/namer/default_namer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/namer/namer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/namer/stack_frame_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/pairwise_combinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.474899 approvaltests-8.4.1/approvaltests/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/pytest/py_test_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporter_missing_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.478899 approvaltests-8.4.1/approvaltests/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/clipboard_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/default_reporter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/diff_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/executable_command_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/file_capture_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/first_working_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/generic_diff_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/generic_diff_reporter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/generic_diff_reporter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/multi_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/python_native_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/quiet_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/received_file_launcher_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/report_all_to_clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/report_by_creating_diff_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/report_on_cyber_dojo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/report_to_diff_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/report_with_beyond_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/report_with_diff_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/report_with_vscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/reporter_that_automatically_approves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/reporters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/reporters/testing_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.478899 approvaltests-8.4.1/approvaltests/scrubbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/scrubbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/scrubbers/date_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/scrubbers/scrubbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/storyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/string_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.478899 approvaltests-8.4.1/approvaltests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/utilities/command_line_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.478899 approvaltests-8.4.1/approvaltests/utilities/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/utilities/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/utilities/logger/simple_logger_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.478899 approvaltests-8.4.1/approvaltests/utilities/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/utilities/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/utilities/logging/logging_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.478899 approvaltests-8.4.1/approvaltests/verifiable_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/verifiable_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-16 18:37:30.000000 approvaltests-8.4.1/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:37:41.000000 approvaltests-8.4.1/approvaltests/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:47.474899 approvaltests-8.4.1/approvaltests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-16 18:37:47.000000 approvaltests-8.4.1/approvaltests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-16 18:37:47.000000 approvaltests-8.4.1/approvaltests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:37:47.000000 approvaltests-8.4.1/approvaltests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-16 18:37:47.000000 approvaltests-8.4.1/approvaltests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 18:37:47.000000 approvaltests-8.4.1/approvaltests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 18:37:30.000000 approvaltests-8.4.1/requirements.prod.extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 18:37:30.000000 approvaltests-8.4.1/requirements.prod.required.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 18:37:30.000000 approvaltests-8.4.1/requirements.prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 18:37:47.478899 approvaltests-8.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-16 18:37:30.000000 approvaltests-8.4.1/setup.publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-16 18:37:30.000000 approvaltests-8.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-16 18:37:30.000000 approvaltests-8.4.1/setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:37:41.000000 approvaltests-8.4.1/version.py
```

### Comparing `approvaltests-8.4.0/LICENSE` & `approvaltests-8.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/PKG-INFO` & `approvaltests-8.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approvaltests
-Version: 8.4.0
+Version: 8.4.1
 Summary: Assertion/verification library to aid testing
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approvaltests-8.4.0/README.md` & `approvaltests-8.4.1/README.md`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/approvals.py` & `approvaltests-8.4.1/approvaltests/approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/asserts.py` & `approvaltests-8.4.1/approvaltests/asserts.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/binary_writer.py` & `approvaltests-8.4.1/approvaltests/binary_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/combination_approvals.py` & `approvaltests-8.4.1/approvaltests/combination_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/command.py` & `approvaltests-8.4.1/approvaltests/command.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/commandline_interface.py` & `approvaltests-8.4.1/approvaltests/commandline_interface.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/core/comparator.py` & `approvaltests-8.4.1/approvaltests/core/comparator.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/core/options.py` & `approvaltests-8.4.1/approvaltests/core/options.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/core/reporter.py` & `approvaltests-8.4.1/approvaltests/core/reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/core/scenario_namer.py` & `approvaltests-8.4.1/approvaltests/core/scenario_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/existing_file_writer.py` & `approvaltests-8.4.1/approvaltests/existing_file_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/file_approver.py` & `approvaltests-8.4.1/approvaltests/file_approver.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/mrjob/mrjob_approvals.py` & `approvaltests-8.4.1/approvaltests/mrjob/mrjob_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/namer/default_namer_factory.py` & `approvaltests-8.4.1/approvaltests/namer/default_namer_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/namer/namer_base.py` & `approvaltests-8.4.1/approvaltests/namer/namer_base.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/namer/stack_frame_namer.py` & `approvaltests-8.4.1/approvaltests/namer/stack_frame_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/pytest/py_test_namer.py` & `approvaltests-8.4.1/approvaltests/pytest/py_test_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/__init__.py` & `approvaltests-8.4.1/approvaltests/reporters/__init__.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/clipboard_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/clipboard_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/default_reporter_factory.py` & `approvaltests-8.4.1/approvaltests/reporters/default_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/diff_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/diff_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/executable_command_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/executable_command_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/file_capture_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/file_capture_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/first_working_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/first_working_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/generic_diff_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/generic_diff_reporter_factory.py` & `approvaltests-8.4.1/approvaltests/reporters/generic_diff_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/python_native_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/python_native_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/received_file_launcher_reporter.py` & `approvaltests-8.4.1/approvaltests/reporters/received_file_launcher_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/report_all_to_clipboard.py` & `approvaltests-8.4.1/approvaltests/reporters/report_all_to_clipboard.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/report_by_creating_diff_file.py` & `approvaltests-8.4.1/approvaltests/reporters/report_by_creating_diff_file.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/report_to_diff_engine.py` & `approvaltests-8.4.1/approvaltests/reporters/report_to_diff_engine.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/report_with_beyond_compare.py` & `approvaltests-8.4.1/approvaltests/reporters/report_with_beyond_compare.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/reporters/reporters.json` & `approvaltests-8.4.1/approvaltests/reporters/reporters.json`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/scrubbers/date_scrubber.py` & `approvaltests-8.4.1/approvaltests/scrubbers/date_scrubber.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/scrubbers/scrubbers.py` & `approvaltests-8.4.1/approvaltests/scrubbers/scrubbers.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/storyboard.py` & `approvaltests-8.4.1/approvaltests/storyboard.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/string_writer.py` & `approvaltests-8.4.1/approvaltests/string_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/utilities/command_line_approvals.py` & `approvaltests-8.4.1/approvaltests/utilities/command_line_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/utilities/logger/simple_logger_approvals.py` & `approvaltests-8.4.1/approvaltests/utilities/logger/simple_logger_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests/utilities/logging/logging_approvals.py` & `approvaltests-8.4.1/approvaltests/utilities/logging/logging_approvals.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,24 +12,22 @@
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
     options: Optional[Options] = None
 ) -> ContextManager:
     class VerifyLogging:
         def __init__(self):
             self.l = LogCapture()
             self.output = "anything"
-            self.options = options
-            if not options:
-                self.options = Options()
+            self.options = options if options else Options()
 
         def __enter__(self):
             self.l.__enter__()
 
             pass
 
         def __exit__(self, exc_type, exc_val, exc_tb):
             self.l.__exit__(exc_type, exc_val, exc_tb)
-            self.options = self.options.with_scrubber(
+            self.options = self.options.add_scrubber(
                 DateScrubber.get_scrubber_for("2023-07-16 17:39:03.293919")
             )
             verify(self.l, options=self.options)
 
     return VerifyLogging()
```

### Comparing `approvaltests-8.4.0/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py` & `approvaltests-8.4.1/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/approvaltests.egg-info/PKG-INFO` & `approvaltests-8.4.1/approvaltests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approvaltests
-Version: 8.4.0
+Version: 8.4.1
 Summary: Assertion/verification library to aid testing
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approvaltests-8.4.0/approvaltests.egg-info/SOURCES.txt` & `approvaltests-8.4.1/approvaltests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `approvaltests-8.4.0/setup_utils.py` & `approvaltests-8.4.1/setup_utils.py`

 * *Files identical despite different names*

