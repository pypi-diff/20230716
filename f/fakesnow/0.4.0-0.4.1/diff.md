# Comparing `tmp/fakesnow-0.4.0.tar.gz` & `tmp/fakesnow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.4.0.tar", last modified: Sun Jul 16 11:31:35 2023, max compression
+gzip compressed data, was "fakesnow-0.4.1.tar", last modified: Sun Jul 16 11:59:10 2023, max compression
```

## Comparing `fakesnow-0.4.0.tar` & `fakesnow-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.246721 fakesnow-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 11:31:24.000000 fakesnow-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 11:31:24.000000 fakesnow-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-16 11:31:35.246721 fakesnow-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-16 11:31:24.000000 fakesnow-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.242721 fakesnow-0.4.0/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/info_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.246721 fakesnow-0.4.0/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-16 11:31:34.000000 fakesnow-0.4.0/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-16 11:31:24.000000 fakesnow-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:31:35.246721 fakesnow-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-16 11:31:24.000000 fakesnow-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.246721 fakesnow-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    29993 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:59:10.324233 fakesnow-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 11:59:00.000000 fakesnow-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 11:59:00.000000 fakesnow-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-16 11:59:10.324233 fakesnow-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-16 11:59:00.000000 fakesnow-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:59:10.320232 fakesnow-0.4.1/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-07-16 11:59:00.000000 fakesnow-0.4.1/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:59:10.324233 fakesnow-0.4.1/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-16 11:59:10.000000 fakesnow-0.4.1/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 11:59:10.000000 fakesnow-0.4.1/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:59:10.000000 fakesnow-0.4.1/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-16 11:59:10.000000 fakesnow-0.4.1/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 11:59:10.000000 fakesnow-0.4.1/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-16 11:59:00.000000 fakesnow-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:59:10.324233 fakesnow-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-16 11:59:00.000000 fakesnow-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:59:10.324233 fakesnow-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-16 11:59:00.000000 fakesnow-0.4.1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-16 11:59:00.000000 fakesnow-0.4.1/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29993 2023-07-16 11:59:00.000000 fakesnow-0.4.1/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-16 11:59:00.000000 fakesnow-0.4.1/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-16 11:59:00.000000 fakesnow-0.4.1/tests/test_transforms.py
```

### Comparing `fakesnow-0.4.0/LICENSE` & `fakesnow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/PKG-INFO` & `fakesnow-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `fakesnow-0.4.0/README.md` & `fakesnow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/fakesnow/__init__.py` & `fakesnow-0.4.1/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/fakesnow/checks.py` & `fakesnow-0.4.1/fakesnow/checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/fakesnow/expr.py` & `fakesnow-0.4.1/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/fakesnow/fakes.py` & `fakesnow-0.4.1/fakesnow/fakes.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             .transform(transforms.extract_text_length)
         )
         sql = transformed.sql(dialect="duckdb")
 
         try:
             self._last_sql = sql
             self._last_params = params
-            print(f"{sql};")
+            # print(f"{sql};")
             self._duck_conn.execute(sql, params)
         except duckdb.BinderException as e:
             msg = e.args[0]
             raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2043, sqlstate="02000") from None
         except duckdb.CatalogException as e:
             # minimal processing to make it look like a snowflake exception, message content may differ
             msg = cast(str, e.args[0]).split("\n")[0]
```

### Comparing `fakesnow-0.4.0/fakesnow/info_schema.py` & `fakesnow-0.4.1/fakesnow/info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/fakesnow/transforms.py` & `fakesnow-0.4.1/fakesnow/transforms.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.4.1/fakesnow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `fakesnow-0.4.0/pyproject.toml` & `fakesnow-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run Snowflake DB locally."
-version = "0.4.0"
+version = "0.4.1"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.8.0",
```

### Comparing `fakesnow-0.4.0/tests/test_checks.py` & `fakesnow-0.4.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/tests/test_expr.py` & `fakesnow-0.4.1/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/tests/test_fakes.py` & `fakesnow-0.4.1/tests/test_fakes.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/tests/test_patch.py` & `fakesnow-0.4.1/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.4.0/tests/test_transforms.py` & `fakesnow-0.4.1/tests/test_transforms.py`

 * *Files identical despite different names*

