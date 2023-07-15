# Comparing `tmp/examon_core-1.0.3.tar.gz` & `tmp/examon_core-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.0.3.tar", max compression
+gzip compressed data, was "examon_core-1.0.4.tar", max compression
```

## Comparing `examon_core-1.0.3.tar` & `examon_core-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.3/examon_core/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-15 20:10:36.790579 examon_core-1.0.3/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      705 2023-05-28 20:45:23.567671 examon_core-1.0.3/examon_core/examon_item.py
--rwxr-xr-x   0        0        0      478 2023-06-23 14:39:27.007604 examon_core-1.0.3/examon_core/examon_item_registry.py
--rwxr-xr-x   0        0        0     1761 2023-06-23 14:39:27.015545 examon_core-1.0.3/examon_core/function_raw_code.py
--rw-r--r--   0        0        0      389 2023-06-23 14:39:26.999135 examon_core-1.0.3/examon_core/multi_choice_factory.py
--rw-r--r--   0        0        0      865 2023-07-15 22:00:22.670689 examon_core-1.0.3/examon_core/print_ext.py
--rwxr-xr-x   0        0        0      621 2023-05-23 09:37:48.400052 examon_core-1.0.3/examon_core/question.py
--rw-r--r--   0        0        0     2525 2023-06-23 14:33:10.050623 examon_core-1.0.3/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.3/examon_core/question_response.py
--rw-r--r--   0        0        0      107 2023-06-23 14:39:27.010739 examon_core-1.0.3/examon_core/todo.md
--rw-r--r--   0        0        0      517 2023-07-15 22:00:22.667922 examon_core-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.4/examon_core/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-15 20:10:36.790579 examon_core-1.0.4/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      705 2023-05-28 20:45:23.567671 examon_core-1.0.4/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0      478 2023-06-23 14:39:27.007604 examon_core-1.0.4/examon_core/examon_item_registry.py
+-rwxr-xr-x   0        0        0     1761 2023-06-23 14:39:27.015545 examon_core-1.0.4/examon_core/function_raw_code.py
+-rw-r--r--   0        0        0      389 2023-06-23 14:39:26.999135 examon_core-1.0.4/examon_core/multi_choice_factory.py
+-rw-r--r--   0        0        0      950 2023-07-15 22:19:35.785327 examon_core-1.0.4/examon_core/print_ext.py
+-rwxr-xr-x   0        0        0      621 2023-05-23 09:37:48.400052 examon_core-1.0.4/examon_core/question.py
+-rw-r--r--   0        0        0     2525 2023-06-23 14:33:10.050623 examon_core-1.0.4/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.4/examon_core/question_response.py
+-rw-r--r--   0        0        0      107 2023-06-23 14:39:27.010739 examon_core-1.0.4/examon_core/todo.md
+-rw-r--r--   0        0        0      517 2023-07-15 22:21:58.826766 examon_core-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.4/PKG-INFO
```

### Comparing `examon_core-1.0.3/examon_core/code_metrics.py` & `examon_core-1.0.4/examon_core/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.3/examon_core/examon_item.py` & `examon_core-1.0.4/examon_core/examon_item.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.3/examon_core/function_raw_code.py` & `examon_core-1.0.4/examon_core/function_raw_code.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.3/examon_core/print_ext.py` & `examon_core-1.0.4/examon_core/print_ext.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 from inspect import getframeinfo, stack
 
 @dataclass
 class PrintLogItem:
     output: str
     line_no: int
 
+
 class PrintLog:
     print_logs = []
 
     @classmethod
     def append(cls, value):
         cls.print_logs.append(value)
 
     @classmethod
     def logs(cls):
         return cls.print_logs
 
     @classmethod
     def apply_offset(cls, offset):
-        cls.print_logs = list(
-            map(lambda x: (x[0], x[1] - offset), cls.print_logs)
-        )
+        def offset_pl(print_log_item):
+            return PrintLogItem(print_log_item.output, print_log_item.line_no - offset)
+
+        cls.print_logs = list(map(offset_pl, cls.print_logs))
 
     @classmethod
     def reset(cls):
         cls.print_logs = []
 
 
 def print(*args, **kwargs):
```

### Comparing `examon_core-1.0.3/examon_core/question.py` & `examon_core-1.0.4/examon_core/question.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.3/examon_core/question_factory.py` & `examon_core-1.0.4/examon_core/question_factory.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.3/pyproject.toml` & `examon_core-1.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "examon_core"
-version = "1.0.3"
+version = "1.0.4"
 description = "Examon Core Libs"
 authors = ["Jarrod Folino <jdfolino@icloud.com>"]
 packages = [{include = "examon_core"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 radon = "^6.0.1"
```

