# Comparing `tmp/atro_rsync-0.0.8.tar.gz` & `tmp/atro_rsync-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_rsync-0.0.8.tar", max compression
+gzip compressed data, was "atro_rsync-0.0.9.tar", max compression
```

## Comparing `atro_rsync-0.0.8.tar` & `atro_rsync-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-17 12:33:58.233092 atro_rsync-0.0.8/README.md
--rw-r--r--   0        0        0     1417 2023-07-16 21:26:13.797613 atro_rsync-0.0.8/atro_rsync/__init__.py
--rw-r--r--   0        0        0       72 2023-06-24 20:11:31.873997 atro_rsync-0.0.8/atro_rsync/helpers.py
--rw-r--r--   0        0        0      323 2023-07-16 21:29:43.298555 atro_rsync-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 atro_rsync-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 12:33:58.233092 atro_rsync-0.0.9/README.md
+-rw-r--r--   0        0        0     1425 2023-07-16 21:33:07.436053 atro_rsync-0.0.9/atro_rsync/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-24 20:11:31.873997 atro_rsync-0.0.9/atro_rsync/helpers.py
+-rw-r--r--   0        0        0      328 2023-07-16 21:34:16.627464 atro_rsync-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 atro_rsync-0.0.9/PKG-INFO
```

### Comparing `atro_rsync-0.0.8/atro_rsync/__init__.py` & `atro_rsync-0.0.9/atro_rsync/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 from pathlib import Path
 
-from pylog import set_logger
-from pyrsync.helpers import wrap_in_double_quotes
+from atro_pylog import set_logger
+from atro_rsync.helpers import wrap_in_double_quotes
 
 
 def rsync(source: Path, destination: Path, options: list[str] = [], exclusions: list[str] = [], cwd=os.getcwd(), logger=set_logger()):
     log_msg = f"Running rsync from {source.as_posix()} to {destination.as_posix()}"
     if len(options) == 1:
         log_msg += f" with option {options[0]}"
     elif len(options) > 1:
```

