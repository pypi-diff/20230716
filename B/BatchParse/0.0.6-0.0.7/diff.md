# Comparing `tmp/BatchParse-0.0.6.tar.gz` & `tmp/BatchParse-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BatchParse-0.0.6.tar", last modified: Sun Jun  4 02:30:16 2023, max compression
+gzip compressed data, was "BatchParse-0.0.7.tar", last modified: Sun Jul 16 01:57:00 2023, max compression
```

## Comparing `BatchParse-0.0.6.tar` & `BatchParse-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/BatchParse/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/BatchParse/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/BatchParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-04 02:30:06.000000 BatchParse-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-04 02:30:16.339444 BatchParse-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 02:30:06.000000 BatchParse-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 02:30:16.339444 BatchParse-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-04 02:30:06.000000 BatchParse-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-04 02:30:06.000000 BatchParse-0.0.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:57:00.167838 BatchParse-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:57:00.163838 BatchParse-0.0.7/BatchParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 01:56:49.000000 BatchParse-0.0.7/BatchParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-16 01:56:49.000000 BatchParse-0.0.7/BatchParse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:57:00.163838 BatchParse-0.0.7/BatchParse/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 01:56:49.000000 BatchParse-0.0.7/BatchParse/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-16 01:56:49.000000 BatchParse-0.0.7/BatchParse/util/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-16 01:56:49.000000 BatchParse-0.0.7/BatchParse/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-16 01:56:49.000000 BatchParse-0.0.7/BatchParse/util/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:57:00.163838 BatchParse-0.0.7/BatchParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-16 01:57:00.000000 BatchParse-0.0.7/BatchParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-16 01:57:00.000000 BatchParse-0.0.7/BatchParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:57:00.000000 BatchParse-0.0.7/BatchParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 01:57:00.000000 BatchParse-0.0.7/BatchParse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 01:57:00.000000 BatchParse-0.0.7/BatchParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-16 01:56:49.000000 BatchParse-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-16 01:57:00.163838 BatchParse-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 01:56:49.000000 BatchParse-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 01:57:00.167838 BatchParse-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-16 01:56:49.000000 BatchParse-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:57:00.163838 BatchParse-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-16 01:56:49.000000 BatchParse-0.0.7/test/test.py
```

### Comparing `BatchParse-0.0.6/BatchParse/main.py` & `BatchParse-0.0.7/BatchParse/main.py`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.6/BatchParse/util/info.py` & `BatchParse-0.0.7/BatchParse/util/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     info = {
         "method": get_method(code),
         "args": get_args(code),
         "length": __get_length(code),
         "valid_command_length": valid_length(__get_length(code)),
         "echo_to_file": echo_to_file(code),
         "get_from_file": get_from_file(code),
+        "variable": __check_variable(code),
         "raw": code,
     }
 
     if info["method"] == "for":
         info["for_args"] = get_info_for(code)
 
     return info
@@ -64,14 +65,23 @@
         int: Returns the length of the code
     """
 
     # NOTE THIS MIGHT NOT BE ACCURATE DUE TO CODEPAGES AND OTHER FACTORS!!!
     return len(code)
 
 
+def __check_variable(code: str) -> bool:
+    variable_regex_1 = re.compile(r"%.*%")
+    variable_regex_2 = re.compile(r"%~.*")
+
+    if variable_regex_1.findall(code) or variable_regex_2.findall(code):
+        return True
+    return False
+
+
 def valid_length(length: int) -> bool:
     """Check if the length of the code is valid with windows batch standards or else the command overflows
 
     Args:
         length (int): Initial Length of command
 
     Returns:
```

### Comparing `BatchParse-0.0.6/BatchParse/util/splitting.py` & `BatchParse-0.0.7/BatchParse/util/splitting.py`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.6/LICENSE` & `BatchParse-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.6/setup.py` & `BatchParse-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "A Batch Parser"
 LONG_DESCRIPTION = "Easy Way to Parse Batch Code in Python"
 
 setup(
     name="BatchParse",
     version=VERSION,
     description=DESCRIPTION,
```

