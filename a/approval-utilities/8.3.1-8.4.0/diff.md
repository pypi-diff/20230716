# Comparing `tmp/approval_utilities-8.3.1.tar.gz` & `tmp/approval_utilities-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approval_utilities-8.3.1.tar", last modified: Sun Jul  2 10:58:41 2023, max compression
+gzip compressed data, was "approval_utilities-8.4.0.tar", last modified: Sun Jul 16 18:13:08 2023, max compression
```

## Comparing `approval_utilities-8.3.1.tar` & `approval_utilities-8.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.673840 approval_utilities-8.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-02 10:58:41.673840 approval_utilities-8.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.669840 approval_utilities-8.3.1/approval_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.669840 approval_utilities-8.3.1/approval_utilities/approvaltests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/approvaltests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.669840 approval_utilities-8.3.1/approval_utilities/approvaltests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/approvaltests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/approvaltests/core/executable_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/approvaltests/core/verifiable.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/approvaltests/core/verify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/list_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.673840 approval_utilities-8.3.1/approval_utilities/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/clipboard_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.673840 approval_utilities-8.3.1/approval_utilities/utilities/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/exceptions/exception_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/exceptions/exception_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/exceptions/multiple_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.673840 approval_utilities-8.3.1/approval_utilities/utilities/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/logger/logging_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/logger/simple_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/markdown_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/multiline_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/os_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.673840 approval_utilities-8.3.1/approval_utilities/utilities/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/persistence/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/persistence/saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/stack_frame_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/string_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/time_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utilities/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/approval_utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:41.669840 approval_utilities-8.3.1/approval_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-02 10:58:41.000000 approval_utilities-8.3.1/approval_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-02 10:58:41.000000 approval_utilities-8.3.1/approval_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:58:41.000000 approval_utilities-8.3.1/approval_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 10:58:41.000000 approval_utilities-8.3.1/approval_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/requirements.prod.extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/requirements.prod.required.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/requirements.prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 10:58:41.673840 approval_utilities-8.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-02 10:58:40.000000 approval_utilities-8.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-02 10:58:29.000000 approval_utilities-8.3.1/setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 10:58:39.000000 approval_utilities-8.3.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.056891 approval_utilities-8.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-16 18:13:08.056891 approval_utilities-8.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.052891 approval_utilities-8.4.0/approval_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.052891 approval_utilities-8.4.0/approval_utilities/approvaltests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/approvaltests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.052891 approval_utilities-8.4.0/approval_utilities/approvaltests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/approvaltests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/approvaltests/core/executable_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/approvaltests/core/verifiable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/approvaltests/core/verify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/list_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.052891 approval_utilities-8.4.0/approval_utilities/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/clipboard_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.056891 approval_utilities-8.4.0/approval_utilities/utilities/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/exceptions/exception_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/exceptions/exception_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/exceptions/multiple_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.056891 approval_utilities-8.4.0/approval_utilities/utilities/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/logger/logging_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/logger/simple_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/markdown_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/multiline_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/os_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.056891 approval_utilities-8.4.0/approval_utilities/utilities/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/persistence/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/persistence/saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/stack_frame_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/string_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/time_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utilities/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/approval_utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:13:08.052891 approval_utilities-8.4.0/approval_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-16 18:13:07.000000 approval_utilities-8.4.0/approval_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-16 18:13:08.000000 approval_utilities-8.4.0/approval_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:13:07.000000 approval_utilities-8.4.0/approval_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 18:13:07.000000 approval_utilities-8.4.0/approval_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/requirements.prod.extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/requirements.prod.required.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/requirements.prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 18:13:08.056891 approval_utilities-8.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-16 18:13:06.000000 approval_utilities-8.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-16 18:12:50.000000 approval_utilities-8.4.0/setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:13:05.000000 approval_utilities-8.4.0/version.py
```

### Comparing `approval_utilities-8.3.1/LICENSE` & `approval_utilities-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/PKG-INFO` & `approval_utilities-8.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approval_utilities
-Version: 8.3.1
+Version: 8.4.0
 Summary: Utilities for your production code that work well with approvaltests
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approval_utilities-8.3.1/README.md` & `approval_utilities-8.4.0/README.md`

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

### Comparing `approval_utilities-8.3.1/approval_utilities/list_utils.py` & `approval_utilities-8.4.0/approval_utilities/list_utils.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utilities/deprecated.py` & `approval_utilities-8.4.0/approval_utilities/utilities/deprecated.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utilities/exceptions/exception_collector.py` & `approval_utilities-8.4.0/approval_utilities/utilities/exceptions/exception_collector.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utilities/logger/logging_instance.py` & `approval_utilities-8.4.0/approval_utilities/utilities/logger/logging_instance.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utilities/logger/simple_logger.py` & `approval_utilities-8.4.0/approval_utilities/utilities/logger/simple_logger.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utilities/markdown_table.py` & `approval_utilities-8.4.0/approval_utilities/utilities/markdown_table.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utilities/time_utilities.py` & `approval_utilities-8.4.0/approval_utilities/utilities/time_utilities.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utilities/wrapper.py` & `approval_utilities-8.4.0/approval_utilities/utilities/wrapper.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities/utils.py` & `approval_utilities-8.4.0/approval_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/approval_utilities.egg-info/PKG-INFO` & `approval_utilities-8.4.0/approval_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approval-utilities
-Version: 8.3.1
+Version: 8.4.0
 Summary: Utilities for your production code that work well with approvaltests
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approval_utilities-8.3.1/approval_utilities.egg-info/SOURCES.txt` & `approval_utilities-8.4.0/approval_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/setup.py` & `approval_utilities-8.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.3.1/setup_utils.py` & `approval_utilities-8.4.0/setup_utils.py`

 * *Files identical despite different names*

