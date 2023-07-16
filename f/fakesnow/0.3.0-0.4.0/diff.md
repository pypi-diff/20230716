# Comparing `tmp/fakesnow-0.3.0.tar.gz` & `tmp/fakesnow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.3.0.tar", last modified: Sat Jul 15 01:02:08 2023, max compression
+gzip compressed data, was "fakesnow-0.4.0.tar", last modified: Sun Jul 16 11:31:35 2023, max compression
```

## Comparing `fakesnow-0.3.0.tar` & `fakesnow-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.483699 fakesnow-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 01:01:57.000000 fakesnow-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-15 01:01:57.000000 fakesnow-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-15 01:02:08.483699 fakesnow-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-15 01:01:57.000000 fakesnow-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.479699 fakesnow-0.3.0/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22362 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21842 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.479699 fakesnow-0.3.0/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-15 01:01:57.000000 fakesnow-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 01:02:08.483699 fakesnow-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-15 01:01:57.000000 fakesnow-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.479699 fakesnow-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    28884 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.246721 fakesnow-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 11:31:24.000000 fakesnow-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 11:31:24.000000 fakesnow-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-16 11:31:35.246721 fakesnow-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-16 11:31:24.000000 fakesnow-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.242721 fakesnow-0.4.0/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-07-16 11:31:24.000000 fakesnow-0.4.0/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.246721 fakesnow-0.4.0/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-16 11:31:34.000000 fakesnow-0.4.0/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 11:31:35.000000 fakesnow-0.4.0/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-16 11:31:24.000000 fakesnow-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:31:35.246721 fakesnow-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-16 11:31:24.000000 fakesnow-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:31:35.246721 fakesnow-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29993 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-16 11:31:24.000000 fakesnow-0.4.0/tests/test_transforms.py
```

### Comparing `fakesnow-0.3.0/LICENSE` & `fakesnow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.3.0/PKG-INFO` & `fakesnow-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -57,15 +57,15 @@
 
     print(conn.cursor().execute("SELECT 'Hello fake world!'").fetchone())
 ```
 
 The following imports are automatically patched:
 
 - `import snowflake.connector.connect`
-- `import  snowflake.connector.pandas_tools.write_pandas`
+- `import snowflake.connector.pandas_tools.write_pandas`
 
 To patch modules that use the `from ... import` syntax, manually specify them, eg: if _mymodule.py_ has the import:
 
 ```python
 from snowflake.connector.pandas_tools import write_pandas
 ```
```

### Comparing `fakesnow-0.3.0/README.md` & `fakesnow-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     print(conn.cursor().execute("SELECT 'Hello fake world!'").fetchone())
 ```
 
 The following imports are automatically patched:
 
 - `import snowflake.connector.connect`
-- `import  snowflake.connector.pandas_tools.write_pandas`
+- `import snowflake.connector.pandas_tools.write_pandas`
 
 To patch modules that use the `from ... import` syntax, manually specify them, eg: if _mymodule.py_ has the import:
 
 ```python
 from snowflake.connector.pandas_tools import write_pandas
 ```
```

### Comparing `fakesnow-0.3.0/fakesnow/__init__.py` & `fakesnow-0.4.0/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.3.0/fakesnow/checks.py` & `fakesnow-0.4.0/fakesnow/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from sqlglot import exp
 
 
 def is_unqualified_table_expression(expression: exp.Expression) -> tuple[bool, bool]:
-    """Checks if the table expression is unqualified, eg: no a database or schema.
+    """Checks if the table expression is unqualified, eg: no database or schema.
 
     NB: sqlglot treats the identifier in "CREATE SCHEMA schema1" as a table expression.
 
     Example:
         >>> import sqlglot
         >>> is_unqualified_table_expression("SELECT * FROM customers")
         (True, True)
```

### Comparing `fakesnow-0.3.0/fakesnow/expr.py` & `fakesnow-0.4.0/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.3.0/fakesnow/fakes.py` & `fakesnow-0.4.0/fakesnow/fakes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import re
-from string import Template
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Iterable, Iterator, Literal, Optional, Sequence, Type, Union, cast
 
 import duckdb
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -17,59 +16,19 @@
 from snowflake.connector.cursor import DictCursor, ResultMetadata, SnowflakeCursor
 from snowflake.connector.result_batch import ResultBatch
 from sqlglot import exp, parse_one
 from typing_extensions import Self
 
 import fakesnow.checks as checks
 import fakesnow.expr as expr
+import fakesnow.info_schema as info_schema
 import fakesnow.transforms as transforms
 
 SCHEMA_UNSET = "schema_unset"
 
-# use ext prefix in columns to disambiguate when joining with information_schema.tables
-SQL_CREATE_INFORMATION_SCHEMA_TABLES_EXT = Template(
-    """
-create table ${catalog}.information_schema.tables_ext (
-    ext_table_catalog varchar,
-    ext_table_schema varchar,
-    ext_table_name varchar,
-    comment varchar,
-    PRIMARY KEY(ext_table_catalog, ext_table_schema, ext_table_name)
-)
-"""
-)
-SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_EXT = Template(
-    """
-create table ${catalog}.information_schema.columns_ext (
-    ext_table_catalog varchar,
-    ext_table_schema varchar,
-    ext_table_name varchar,
-    ext_column_name varchar,
-    ext_character_maximum_length integer,
-    ext_character_octet_length integer,
-    PRIMARY KEY(ext_table_catalog, ext_table_schema, ext_table_name, ext_column_name)
-)
-"""
-)
-# only include fields applicable to snowflake (as mentioned by describe table information_schema.columns)
-
-SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_VIEW = Template(
-    """
-create view ${catalog}.information_schema.columns_snowflake AS
-select table_catalog, table_schema, table_name, column_name, ordinal_position, column_default, is_nullable, data_type,
-ext_character_maximum_length as character_maximum_length, ext_character_octet_length as character_octet_length,
-numeric_precision, numeric_precision_radix, numeric_scale,
-collation_name, is_identity, identity_generation, identity_cycle
-from ${catalog}.information_schema.columns
-left join ${catalog}.information_schema.columns_ext ext
-on ext_table_catalog = table_catalog AND ext_table_schema = table_schema
-AND ext_table_name = table_name AND ext_column_name = column_name
-"""
-)
-
 
 class FakeSnowflakeCursor:
     def __init__(
         self,
         conn: FakeSnowflakeConnection,
         duck_conn: DuckDBPyConnection,
         use_dict_result: bool = False,
@@ -162,32 +121,34 @@
             .transform(transforms.set_schema, current_database=self._conn.database)
             .transform(transforms.create_database)
             .transform(transforms.extract_comment)
             .transform(transforms.information_schema_columns_snowflake)
             .transform(transforms.information_schema_tables_ext)
             .transform(transforms.drop_schema_cascade)
             .transform(transforms.tag)
-            .transform(transforms.regex)
             .transform(transforms.semi_structured_types)
             .transform(transforms.parse_json)
-            .transform(transforms.indices_to_array)
-            .transform(transforms.indices_to_object)
+            # indices_to_json_extract must be before regex_substr
+            .transform(transforms.indices_to_json_extract)
+            .transform(transforms.regex_replace)
+            .transform(transforms.regex_substr)
             .transform(transforms.values_columns)
             .transform(transforms.to_date)
             .transform(transforms.object_construct)
             .transform(transforms.timestamp_ntz_ns)
             .transform(transforms.float_to_double)
             .transform(transforms.integer_precision)
             .transform(transforms.extract_text_length)
         )
         sql = transformed.sql(dialect="duckdb")
 
         try:
             self._last_sql = sql
             self._last_params = params
+            print(f"{sql};")
             self._duck_conn.execute(sql, params)
         except duckdb.BinderException as e:
             msg = e.args[0]
             raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2043, sqlstate="02000") from None
         except duckdb.CatalogException as e:
             # minimal processing to make it look like a snowflake exception, message content may differ
             msg = cast(str, e.args[0]).split("\n")[0]
@@ -199,48 +160,32 @@
 
         if cmd == "USE SCHEMA" and (ident := expression.find(exp.Identifier)) and isinstance(ident.this, str):
             self._conn.schema = ident.this.upper()
             self._conn.schema_set = True
 
         if create_db_name := transformed.args.get("create_db_name"):
             # we created a new database, so create the info schema extensions
-            self._conn._create_info_schema_ext(create_db_name)  # noqa: SLF001
+            self._duck_conn.execute(info_schema.creation_sql(create_db_name))
 
-        if table_comment := transformed.args.get("table_comment"):
+        if table_comment := cast(tuple[exp.Table, str], transformed.args.get("table_comment")):
             # record table comment
             table, comment = table_comment
             catalog = table.catalog or self._conn.database
             schema = table.db or self._conn.schema
-            self._duck_conn.execute(
-                f"""
-                INSERT INTO {catalog}.information_schema.tables_ext
-                values ('{catalog}', '{schema}', '{table.name}', '{comment}')
-                ON CONFLICT (ext_table_catalog, ext_table_schema, ext_table_name)
-                DO UPDATE SET comment = excluded.comment
-                """
-            )
+            assert catalog and schema
+            self._duck_conn.execute(info_schema.insert_table_comment_sql(catalog, schema, table.name, comment))
 
-        if (text_lengths := transformed.args.get("text_lengths")) and (table := transformed.find(exp.Table)):
+        if (text_lengths := cast(list[tuple[str, int]], transformed.args.get("text_lengths"))) and (
+            table := transformed.find(exp.Table)
+        ):
             # record text lengths
             catalog = table.catalog or self._conn.database
             schema = table.db or self._conn.schema
-            values = ", ".join(
-                f"('{catalog}', '{schema}', '{table.name}', '{col_name}', {size}, {min(size*4,16777216)})"
-                for (col_name, size) in text_lengths
-            )
-
-            self._duck_conn.execute(
-                f"""
-                INSERT INTO {catalog}.information_schema.columns_ext
-                values {values}
-                ON CONFLICT (ext_table_catalog, ext_table_schema, ext_table_name, ext_column_name)
-                DO UPDATE SET ext_character_maximum_length = excluded.ext_character_maximum_length,
-                                ext_character_octet_length = excluded.ext_character_octet_length
-                """
-            )
+            assert catalog and schema
+            self._duck_conn.execute(info_schema.insert_text_lengths_sql(catalog, schema, table.name, text_lengths))
 
         return self
 
     def executemany(
         self,
         command: str,
         seqparams: Sequence[Any] | dict[str, Any],
@@ -293,55 +238,59 @@
             try:
                 batches.append(FakeResultBatch(self._use_dict_result, reader.read_next_batch()))
             except StopIteration:
                 break
 
         return batches
 
+    @property
+    def rowcount(self) -> int | None:
+        # TODO: return number of rows updated/inserted (using returning)
+        return None
+
     @staticmethod
     def _describe_as_result_metadata(describe_results: list) -> list[ResultMetadata]:
         # fmt: off
         def as_result_metadata(column_name: str, column_type: str, _: str) -> ResultMetadata:
             # see https://docs.snowflake.com/en/user-guide/python-connector-api.html#type-codes
             # and https://arrow.apache.org/docs/python/api/datatypes.html#type-checking
-            # type ignore because of https://github.com/snowflakedb/snowflake-connector-python/issues/1423
-            if column_type == "INTEGER":
+            if column_type == "BIGINT":
                 return ResultMetadata(
-                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True                    # type: ignore # noqa: E501
+                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True               # noqa: E501
                 )
             elif column_type.startswith("DECIMAL"):
                 match = re.search(r'\((\d+),(\d+)\)', column_type)
                 if match:
                     precision = int(match[1])
                     scale = int(match[2])
                 else:
                     precision = scale = None
                 return ResultMetadata(
-                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=precision, scale=scale, is_nullable=True # type: ignore # noqa: E501
+                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=precision, scale=scale, is_nullable=True    # noqa: E501
                 )
             elif column_type == "VARCHAR":
                 # TODO: fetch internal_size from varchar size
                 return ResultMetadata(
-                    name=column_name, type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True   # type: ignore # noqa: E501
+                    name=column_name, type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True      # noqa: E501
                 )
             elif column_type == "DOUBLE":
                 return ResultMetadata(
-                    name=column_name, type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True       # type: ignore # noqa: E501
+                    name=column_name, type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True          # noqa: E501
                 )
             elif column_type == "BOOLEAN":
                 return ResultMetadata(
-                    name=column_name, type_code=13, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True      # type: ignore # noqa: E501
+                    name=column_name, type_code=13, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True         # noqa: E501
                 )
             elif column_type == "DATE":
                 return ResultMetadata(
-                    name=column_name, type_code=3, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True       # type: ignore # noqa: E501
+                    name=column_name, type_code=3, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True          # noqa: E501
                 )
-            elif column_type in ["TIMESTAMP", "TIMESTAMP_NS"]:
+            elif column_type in {"TIMESTAMP", "TIMESTAMP_NS"}:
                 return ResultMetadata(
-                    name=column_name, type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True             # type: ignore # noqa: E501
+                    name=column_name, type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True                # noqa: E501
                 )
             else:
                 # TODO handle more types
                 raise NotImplementedError(f"for column type {column_type}")
 
         # fmt: on
 
@@ -392,15 +341,15 @@
             and self.database
             and not duck_conn.execute(
                 f"""select * from information_schema.schemata
                 where catalog_name = '{self.database}'"""
             ).fetchone()
         ):
             duck_conn.execute(f"ATTACH DATABASE ':memory:' AS {self.database}")
-            self._create_info_schema_ext(self.database)
+            duck_conn.execute(info_schema.creation_sql(self.database))
 
         # create schema if needed
         if (
             create_schema
             and self.database
             and self.schema
             and not duck_conn.execute(
@@ -478,20 +427,14 @@
         # whereas duckdb loads them as a struct, so we convert them to json here
         cols = [f"TO_JSON({c})" if isinstance(df[c][0], dict) else c for c in df.columns]
         cols = ",".join(cols)
 
         self._duck_conn.execute(f"INSERT INTO {table_name}({','.join(df.columns.to_list())}) SELECT {cols} FROM df")
         return self._duck_conn.fetchall()[0][0]
 
-    def _create_info_schema_ext(self, catalog: str) -> None:
-        """Create the info schema extension tables/views used for storing snowflake metadata not captured by duckdb."""
-        self._duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_TABLES_EXT.substitute(catalog=catalog))
-        self._duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_EXT.substitute(catalog=catalog))
-        self._duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_VIEW.substitute(catalog=catalog))
-
 
 class FakeResultBatch(ResultBatch):
     def __init__(self, use_dict_result: bool, batch: pyarrow.RecordBatch):
         self._use_dict_result = use_dict_result
         self._batch = batch
 
     def create_iter(
```

### Comparing `fakesnow-0.3.0/fakesnow/transforms.py` & `fakesnow-0.4.0/fakesnow/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import cast
 
+import snowflake.connector
 import sqlglot
 from sqlglot import exp
 
 MISSING_DATABASE = "missing_database"
 SUCCESS_NOP = sqlglot.parse_one("SELECT 'Statement executed successfully.'")
 
 
@@ -144,15 +145,15 @@
     duckdb doesn't have fixed-sized text types. So we capture the size of text types and store that in the
     character_maximum_length arg.
 
     Args:
         expression (exp.Expression): the expression that will be transformed.
 
     Returns:
-        exp.Expression: The original expression, with any comment stored in the new 'table_comment' arg.
+        exp.Expression: The original expression, with any text lengths stored in the new 'text_lengths' arg.
     """
 
     if isinstance(expression, (exp.Create, exp.AlterTable)):
         text_lengths = []
         for dt in expression.find_all(exp.DataType):
             if dt.this in (exp.DataType.Type.VARCHAR, exp.DataType.Type.TEXT):
                 col_name = dt.parent and dt.parent.this and dt.parent.this.this
@@ -184,76 +185,41 @@
         new = expression.copy()
         new.args["this"] = exp.DataType.Type.DOUBLE
         return new
 
     return expression
 
 
-def indices_to_array(expression: exp.Expression) -> exp.Expression:
-    """Convert to 1-based list indices.
+def indices_to_json_extract(expression: exp.Expression) -> exp.Expression:
+    """Convert indices on objects and arrays to json_extract.
 
-    Snowflake uses 0-based array indexing, whereas duckdb using 1-based list indexing.
-
-    See https://docs.snowflake.com/en/sql-reference/data-types-semistructured#accessing-elements-of-an-array-by-index-or-by-slice
-
-    Example:
-        >>> import sqlglot
-        >>> sqlglot.parse_one("SELECT myarray[0] FROM table1").transform(indices_to_array).sql()
-        'SELECT myarray[1] FROM table1'
-    Args:
-        expression (exp.Expression): the expression that will be transformed.
-
-    Returns:
-        exp.Expression: The transformed expression.
-    """
-    if (
-        isinstance(expression, exp.Bracket)
-        and len(expression.expressions) == 1
-        and (index := expression.expressions[0])
-        and isinstance(index, exp.Literal)
-        and index.this
-        and not index.is_string
-    ):
-        new = expression.copy()
-        new.expressions[0] = exp.Literal(this=str(int(index.this) + 1), is_string=False)
-        return new
-    return expression
-
-
-def indices_to_object(expression: exp.Expression) -> exp.Expression:
-    """Convert object indices to JSON extraction.
-
-    Supports Snowflake object indices, see
+    Supports Snowflake array indices, see
+    https://docs.snowflake.com/en/sql-reference/data-types-semistructured#accessing-elements-of-an-array-by-index-or-by-slice
+    and object indices, see
     https://docs.snowflake.com/en/sql-reference/data-types-semistructured#accessing-elements-of-an-object-by-key
 
     Duckdb uses the -> operator, or the json_extract function, see
     https://duckdb.org/docs/extensions/json#json-extraction-functions
 
-    Example:
-        >>> import sqlglot
-        >>> sqlglot.parse_one("select name['k'] from semi").transform(indices_to_object).sql()
-        'SELECT name -> '$.k' FROM semi'
-    Args:
-        expression (exp.Expression): the expression that will be transformed.
-
-    Returns:
-        exp.Expression: The transformed expression.
+    This works for Snowflake arrays too because we convert them to JSON[] in duckdb.
     """
     if (
         isinstance(expression, exp.Bracket)
         and len(expression.expressions) == 1
         and (index := expression.expressions[0])
         and isinstance(index, exp.Literal)
         and index.this
-        and index.is_string
-        and (ident := expression.find(exp.Identifier))
     ):
-        # use sql() to handle quoting
-        ident_sql = ident.sql()
-        return sqlglot.parse_one(f"{ident_sql} -> '$.{index.this}'", read="duckdb")
+        if index.is_string:
+            return exp.JSONExtract(this=expression.this, expression=exp.Literal(this=f"$.{index.this}", is_string=True))
+        else:
+            return exp.JSONExtract(
+                this=expression.this, expression=exp.Literal(this=f"$[{index.this}]", is_string=True)
+            )
+
     return expression
 
 
 def information_schema_columns_snowflake(expression: exp.Expression) -> exp.Expression:
     """Redirect to the information_schema.columns_snowflake view which has metadata that matches snowflake.
 
     Because duckdb doesn't store character_maximum_length or character_octet_length.
@@ -291,36 +257,29 @@
             join_type="left",
         )
 
     return expression
 
 
 def integer_precision(expression: exp.Expression) -> exp.Expression:
-    """Snowflake integers are 38 digits.
+    """Convert integers to bigint.
 
-    See https://docs.snowflake.com/en/sql-reference/data-types-numeric
+    So dataframes will return them with a dtype of int64.
     """
 
-    decimal_38_0 = exp.DataType(
-        this=exp.DataType.Type.DECIMAL,
-        expressions=[
-            exp.DataTypeSize(this=exp.Literal(this="38", is_string=False)),
-            exp.DataTypeSize(this=exp.Literal(this="0", is_string=False)),
-        ],
-        nested=False,
-        prefix=False,
-    )
-
     if (
         isinstance(expression, exp.DataType)
         and (expression.this == exp.DataType.Type.DECIMAL and not expression.expressions)
-        or expression.this
-        in (exp.DataType.Type.BIGINT, exp.DataType.Type.INT, exp.DataType.Type.SMALLINT, exp.DataType.Type.TINYINT)
+        or expression.this in (exp.DataType.Type.INT, exp.DataType.Type.SMALLINT, exp.DataType.Type.TINYINT)
     ):
-        return decimal_38_0
+        return exp.DataType(
+            this=exp.DataType.Type.BIGINT,
+            nested=False,
+            prefix=False,
+        )
 
     return expression
 
 
 def object_construct(expression: exp.Expression) -> exp.Expression:
     """Convert object_construct to return a json string
 
@@ -365,56 +324,109 @@
         new = expression.copy()
         new.args["this"] = "JSON"
         return new
 
     return expression
 
 
-def regex(expression: exp.Expression) -> exp.Expression:
-    """Transform regex expressions from snowflake to duckdb.
-
-    Example:
-        >>> import sqlglot
-        >>> sqlglot.parse_one("SELECT regexp_replace('abc123', '\\\\D', '')").transform(tag).sql()
-        "SELECT regexp_replace('abc123', '\\D', '', 'g')"
-    Args:
-        expression (exp.Expression): the expression that will be transformed.
-
-    Returns:
-        exp.Expression: The transformed expression.
-    """
+def regex_replace(expression: exp.Expression) -> exp.Expression:
+    """Transform regex_replace expressions from snowflake to duckdb."""
 
     if (
         isinstance(expression, exp.Anonymous)
         and isinstance(expression.this, str)
-        and "REGEXP_REPLACE" == expression.this.upper()
+        and expression.this.upper() == "REGEXP_REPLACE"
     ):
-        new = expression.copy()
-        new_args = new.expressions
+        expressions = expression.expressions
 
-        if len(new_args) > 3:
+        if len(expressions) > 3:
             # see https://docs.snowflake.com/en/sql-reference/functions/regexp_replace
             raise NotImplementedError(
                 "REGEXP_REPLACE with additional parameters (eg: <position>, <occurrence>, <parameters>) not supported"
             )
 
-        # snowflake requires escaping backslashes in single-quoted string constants, but duckdb doesn't
+        # pattern: snowflake requires escaping backslashes in single-quoted string constants, but duckdb doesn't
         # see https://docs.snowflake.com/en/sql-reference/functions-regexp#label-regexp-escape-character-caveats
-        new_args[1].args["this"] = new_args[1].this.replace("\\\\", "\\")
+        expressions[1].args["this"] = expressions[1].this.replace("\\\\", "\\")
 
-        if len(new_args) == 2:
+        if len(expressions) == 2:
             # if no replacement string, the snowflake default is ''
-            new_args.append(exp.Literal(this="", is_string=True))
+            expressions.append(exp.Literal(this="", is_string=True))
 
         # snowflake regex replacements are global
-        new_args.append(exp.Literal(this="g", is_string=True))
+        expressions.append(exp.Literal(this="g", is_string=True))
+
+    return expression
 
-        new.set("expressions", new_args)
 
-        return new
+def regex_substr(expression: exp.Expression) -> exp.Expression:
+    """Transform regex_substr expressions from snowflake to duckdb."""
+
+    if (
+        isinstance(expression, exp.Anonymous)
+        and isinstance(expression.this, str)
+        and expression.this.upper() == "REGEXP_SUBSTR"
+    ):
+        expressions = expression.expressions
+
+        if len(expressions) < 2:
+            raise snowflake.connector.errors.ProgrammingError(
+                msg=f"SQL compilation error:\nnot enough arguments for function [{expression.sql()}], expected 2, got {len(expressions)}",  # noqa: E501
+                errno=938,
+                sqlstate="22023",
+            )
+
+        subject = expressions[0]
+
+        # pattern: snowflake requires escaping backslashes in single-quoted string constants, but duckdb doesn't
+        # see https://docs.snowflake.com/en/sql-reference/functions-regexp#label-regexp-escape-character-caveats
+        pattern = expressions[1]
+        pattern.args["this"] = pattern.this.replace("\\\\", "\\")
+
+        # number of characters from the beginning of the string where the function starts searching for matches
+        try:
+            position = expressions[2]
+        except IndexError:
+            position = exp.Literal(this="1", is_string=False)
+
+        # which occurrence of the pattern to match
+        try:
+            occurrence = expressions[3]
+        except IndexError:
+            occurrence = exp.Literal(this="1", is_string=False)
+
+        try:
+            regex_parameters_value = str(expressions[4].this)
+            # 'e' parameter doesn't make sense for duckdb
+            regex_parameters = exp.Literal(this=regex_parameters_value.replace("e", ""), is_string=True)
+        except IndexError:
+            regex_parameters = exp.Literal(is_string=True)
+
+        try:
+            group_num = expressions[5]
+        except IndexError:
+            if isinstance(regex_parameters.this, str) and "e" in regex_parameters.this:
+                group_num = exp.Literal(this="1", is_string=False)
+            else:
+                group_num = exp.Literal(this="0", is_string=False)
+
+        expression = exp.Bracket(
+            this=exp.Anonymous(
+                this="regexp_extract_all",
+                expressions=[
+                    # slice subject from position onwards
+                    exp.Bracket(this=subject, expressions=[exp.Slice(this=position)]),
+                    pattern,
+                    group_num,
+                    regex_parameters,
+                ],
+            ),
+            # select index of occurrence
+            expressions=[occurrence],
+        )
 
     return expression
 
 
 # TODO: move this into a Dialect as a transpilation
 def set_schema(expression: exp.Expression, current_database: str | None) -> exp.Expression:
     """Transform USE SCHEMA/DATABASE to SET schema.
@@ -598,32 +610,20 @@
 
 
 def values_columns(expression: exp.Expression) -> exp.Expression:
     """Support column1, column2 expressions in VALUES.
 
     Snowflake uses column1, column2 .. for unnamed columns in VALUES. Whereas duckdb uses col0, col1 ..
     See https://docs.snowflake.com/en/sql-reference/constructs/values#examples
-
-    Example:
-        >>> import sqlglot
-        >>> sqlglot.parse_one("SELECT * FROM VALUES ('Amsterdam', 1)").transform(values_columns).sql()
-        'SELECT * FROM (VALUES ('Amsterdam', 1)) AS _("column1", "column2")'
-    Args:
-        expression (exp.Expression): the expression that will be transformed.
-
-    Returns:
-        exp.Expression: The transformed expression.
     """
 
     if (
         isinstance(expression, exp.Values)
         and not expression.alias
         and expression.find_ancestor(exp.Select)
         and (values := expression.find(exp.Tuple))
     ):
-        new = expression.copy()
         num_columns = len(values.expressions)
-        columns = [exp.Identifier(this=f"column{i + 1}", quoted=True) for i in range(num_columns)]
-        new.set("alias", exp.TableAlias(this=exp.Identifier(this="_", quoted=False), columns=columns))
-        return new
+        columns = [exp.Identifier(this=f"COLUMN{i + 1}", quoted=True) for i in range(num_columns)]
+        expression.set("alias", exp.TableAlias(this=exp.Identifier(this="_", quoted=False), columns=columns))
 
     return expression
```

### Comparing `fakesnow-0.3.0/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.4.0/fakesnow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -57,15 +57,15 @@
 
     print(conn.cursor().execute("SELECT 'Hello fake world!'").fetchone())
 ```
 
 The following imports are automatically patched:
 
 - `import snowflake.connector.connect`
-- `import  snowflake.connector.pandas_tools.write_pandas`
+- `import snowflake.connector.pandas_tools.write_pandas`
 
 To patch modules that use the `from ... import` syntax, manually specify them, eg: if _mymodule.py_ has the import:
 
 ```python
 from snowflake.connector.pandas_tools import write_pandas
 ```
```

### Comparing `fakesnow-0.3.0/pyproject.toml` & `fakesnow-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run Snowflake DB locally."
-version = "0.3.0"
+version = "0.4.0"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.8.0",
```

### Comparing `fakesnow-0.3.0/tests/test_checks.py` & `fakesnow-0.4.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.3.0/tests/test_expr.py` & `fakesnow-0.4.0/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.3.0/tests/test_fakes.py` & `fakesnow-0.4.0/tests/test_fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,15 +340,16 @@
 
     expected_df = pd.DataFrame.from_records(
         [
             {"ID": 1, "FIRST_NAME": "Jenny", "LAST_NAME": "P"},
             {"ID": 2, "FIRST_NAME": "Jasper", "LAST_NAME": "M"},
         ]
     )
-    assert_frame_equal(cur.fetch_pandas_all(), expected_df, check_dtype=False)
+    # integers have dtype int64
+    assert_frame_equal(cur.fetch_pandas_all(), expected_df)
 
 
 def test_floats_are_64bit(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create or replace table example (f float, f4 float4, f8 float8, d double, r real)")
     cur.execute("insert into example values (1.23, 1.23, 1.23, 1.23, 1.23)")
     cur.execute("select * from example")
     # 32 bit floats will return 1.2300000190734863 rather than 1.23
@@ -386,38 +387,38 @@
 
 
 def test_information_schema_columns_numeric(cur: snowflake.connector.cursor.SnowflakeCursor):
     # see https://docs.snowflake.com/en/sql-reference/data-types-numeric
     cur.execute(
         """
         create table example (
-            XNUMBER20 NUMBER(2,0), XNUMBER NUMBER, XDECIMAL DECIMAL, XNUMERIC NUMERIC,
+            XNUMBER82 NUMBER(8,2), XNUMBER NUMBER, XDECIMAL DECIMAL, XNUMERIC NUMERIC,
             XINT INT, XINTEGER INTEGER, XBIGINT BIGINT, XSMALLINT SMALLINT, XTINYINT TINYINT, XBYTEINT BYTEINT
         )
         """
     )
 
     cur.execute(
         """
-        select column_name,numeric_precision,numeric_precision_radix,numeric_scale
+        select column_name,data_type,numeric_precision,numeric_precision_radix,numeric_scale
         from information_schema.columns where table_name = 'EXAMPLE' order by ordinal_position
         """
     )
 
     assert cur.fetchall() == [
-        ("XNUMBER20", 2, 10, 0),
-        ("XNUMBER", 38, 10, 0),
-        ("XDECIMAL", 38, 10, 0),
-        ("XNUMERIC", 38, 10, 0),
-        ("XINT", 38, 10, 0),
-        ("XINTEGER", 38, 10, 0),
-        ("XBIGINT", 38, 10, 0),
-        ("XSMALLINT", 38, 10, 0),
-        ("XTINYINT", 38, 10, 0),
-        ("XBYTEINT", 38, 10, 0),
+        ("XNUMBER82", "NUMBER", 8, 10, 2),
+        ("XNUMBER", "NUMBER", 38, 10, 0),
+        ("XDECIMAL", "NUMBER", 38, 10, 0),
+        ("XNUMERIC", "NUMBER", 38, 10, 0),
+        ("XINT", "NUMBER", 38, 10, 0),
+        ("XINTEGER", "NUMBER", 38, 10, 0),
+        ("XBIGINT", "NUMBER", 38, 10, 0),
+        ("XSMALLINT", "NUMBER", 38, 10, 0),
+        ("XTINYINT", "NUMBER", 38, 10, 0),
+        ("XBYTEINT", "NUMBER", 38, 10, 0),
     ]
 
 
 def test_information_schema_columns_text(cur: snowflake.connector.cursor.SnowflakeCursor):
     # see https://docs.snowflake.com/en/sql-reference/data-types-text
     cur.execute(
         """
@@ -425,23 +426,23 @@
             XVARCHAR20 VARCHAR(20), XVARCHAR VARCHAR, XTEXT TEXT
         )
         """
     )
 
     cur.execute(
         """
-        select column_name,character_maximum_length,character_octet_length
+        select column_name,data_type,character_maximum_length,character_octet_length
         from information_schema.columns where table_name = 'EXAMPLE' order by ordinal_position
         """
     )
 
     assert cur.fetchall() == [
-        ("XVARCHAR20", 20, 80),
-        ("XVARCHAR", 16777216, 16777216),
-        ("XTEXT", 16777216, 16777216),
+        ("XVARCHAR20", "TEXT", 20, 80),
+        ("XVARCHAR", "TEXT", 16777216, 16777216),
+        ("XTEXT", "TEXT", 16777216, 16777216),
     ]
 
 
 def test_non_existent_table_throws_snowflake_exception(cur: snowflake.connector.cursor.SnowflakeCursor):
     with pytest.raises(snowflake.connector.errors.ProgrammingError) as _:
         cur.execute("select * from this_table_does_not_exist")
 
@@ -459,14 +460,35 @@
 
 
 def test_regex(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("select regexp_replace('abc123', '\\\\D', '')")
     assert cur.fetchone() == ("123",)
 
 
+def test_regex_substr(cur: snowflake.connector.cursor.SnowflakeCursor):
+    # see https://docs.snowflake.com/en/sql-reference/functions/regexp_substr
+    string1 = "It was the best of times, it was the worst of times."
+
+    cur.execute(f"select regexp_substr('{string1}', 'the\\\\W+\\\\w+')")
+    assert cur.fetchone() == ("the best",)
+
+    cur.execute(f"select regexp_substr('{string1}', 'the\\\\W+\\\\w+', 1, 2)")
+    assert cur.fetchone() == ("the worst",)
+
+    cur.execute(f"select regexp_substr('{string1}', 'the\\\\W+(\\\\w+)', 1, 2, 'e', 1)")
+    assert cur.fetchone() == ("worst",)
+
+
+def test_rowcount(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute("create table example(id int)")
+    cur.execute("insert into example SELECT * FROM (VALUES (1), (2), (3));")
+    # TODO: rows inserted ie: 3
+    assert cur.rowcount is None
+
+
 def test_schema_create_and_use(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create schema jaffles")
     cur.execute("create table jaffles.customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
     cur.execute("use schema jaffles")
     # fully qualified works too
     cur.execute("use schema db1.jaffles")
     cur.execute("insert into customers values (1, 'Jenny', 'P')")
@@ -481,25 +503,28 @@
 
 def test_semi_structured_types(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create table semis (emails array, name object, notes variant)")
     cur.execute(
         """insert into semis(emails, name, notes) SELECT [1, 2], parse_json('{"k": "v1"}'), parse_json('["foo"]')"""
     )
     cur.execute(
-        """insert into semis(emails, name, notes) VALUES ([3,4], parse_json('{"k": "v2"}'), parse_json('["bar"]'))"""  # noqa: E501
+        """insert into semis(emails, name, notes) VALUES ([3,4], parse_json('{"k": "v2"}'), parse_json('{"b": "ar"}'))"""  # noqa: E501
     )
 
+    # results are returned as strings, because the underlying type is JSON (duckdb) / VARIANT (snowflake)
+
     cur.execute("select emails[0] from semis")
-    # returned as strings, because the underlying type is JSON (duckdb) / VARIANT (snowflake)
     assert cur.fetchall() == [("1",), ("3",)]
 
     cur.execute("select name['k'] from semis")
-    # returned as json strings, because the underlying type is JSON (duckdb) / VARIANT (snowflake)
     assert cur.fetchall() == [('"v1"',), ('"v2"',)]
 
+    cur.execute("select notes[0] from semis")
+    assert cur.fetchall() == [('"foo"',), (None,)]
+
 
 def test_table_comments(cur: snowflake.connector.cursor.SnowflakeCursor):
     def read_comment() -> str:
         cur.execute(
             """SELECT COALESCE(COMMENT, '') FROM INFORMATION_SCHEMA.TABLES
                     WHERE TABLE_NAME = 'INGREDIENTS' AND TABLE_SCHEMA = 'SCHEMA1' LIMIT 1"""
         )
@@ -607,23 +632,25 @@
 
 
 def test_values(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor(snowflake.connector.cursor.DictCursor) as cur:
         cur.execute("SELECT * FROM VALUES ('Amsterdam', 1), ('London', 2)")
 
         assert cur.fetchall() == [
-            {"column1": "Amsterdam", "column2": 1},
-            {"column1": "London", "column2": 2},
+            {"COLUMN1": "Amsterdam", "COLUMN2": 1},
+            {"COLUMN1": "London", "COLUMN2": 2},
         ]
 
-        cur.execute("SELECT column2, column1 FROM VALUES ('Amsterdam', 1), ('London', 2)")
+        cur.execute(
+            "SELECT column2, column1, parse_json(column3) as pj FROM VALUES ('Amsterdam', 1, '[]'), ('London', 2, '{}')"
+        )
 
         assert cur.fetchall() == [
-            {"column2": 1, "column1": "Amsterdam"},
-            {"column2": 2, "column1": "London"},
+            {"COLUMN2": 1, "COLUMN1": "Amsterdam", "PJ": "[]"},
+            {"COLUMN2": 2, "COLUMN1": "London", "PJ": "{}"},
         ]
 
 
 def test_write_pandas(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor() as cur:
         cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
```

### Comparing `fakesnow-0.3.0/tests/test_patch.py` & `fakesnow-0.4.0/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.3.0/tests/test_transforms.py` & `fakesnow-0.4.0/tests/test_transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     SUCCESS_NOP,
     as_describe,
     create_database,
     drop_schema_cascade,
     extract_comment,
     extract_text_length,
     float_to_double,
-    indices_to_array,
-    indices_to_object,
+    indices_to_json_extract,
     information_schema_columns_snowflake,
     information_schema_tables_ext,
     integer_precision,
     object_construct,
     parse_json,
-    regex,
+    regex_replace,
+    regex_substr,
     semi_structured_types,
     set_schema,
     tag,
     timestamp_ntz_ns,
     to_date,
     upper_case_unquoted_identifiers,
     values_columns,
@@ -63,57 +63,55 @@
 
     e = sqlglot.parse_one("ALTER TABLE table1 SET COMMENT = 'comment1'", read="snowflake").transform(extract_comment)
     assert e.sql() == "SELECT 'Statement executed successfully.'"
     assert e.args["table_comment"] == (table1, "comment1")
 
 
 def test_extract_text_length() -> None:
-    sql = "CREATE TABLE table1 (t1 VARCHAR, t2 VARCHAR(10), t3 TEXT(20), d1 DECIMAL(38, 0))"
+    sql = "CREATE TABLE table1 (t1 VARCHAR, t2 VARCHAR(10), t3 TEXT(20), i1 BIGINT)"
     e = sqlglot.parse_one(sql).transform(extract_text_length)
     assert e.sql() == sql
     assert e.args["text_lengths"] == [("t1", 16777216), ("t2", 10), ("t3", 20)]
 
 
 def test_float_to_double() -> None:
     assert (
         sqlglot.parse_one("create table example (f float, f4 float4, f8 float8, d double, r real)")
         .transform(float_to_double)
         .sql()
         == "CREATE TABLE example (f DOUBLE, f4 DOUBLE, f8 DOUBLE, d DOUBLE, r DOUBLE)"
     )
 
 
-def test_indices_to_array() -> None:
+def test_indices_to_object() -> None:
     assert (
-        sqlglot.parse_one("SELECT myarray[0] FROM table1").transform(indices_to_array).sql()
-        == "SELECT myarray[1] FROM table1"
+        sqlglot.parse_one("SELECT myarray[0] FROM table1").transform(indices_to_json_extract).sql()
+        == "SELECT JSON_EXTRACT(myarray, '$[0]') FROM table1"
     )
 
-
-def test_indices_to_object() -> None:
     assert (
-        sqlglot.parse_one("SELECT name['k'] FROM semi").transform(indices_to_object).sql(dialect="duckdb")
+        sqlglot.parse_one("SELECT name['k'] FROM semi").transform(indices_to_json_extract).sql(dialect="duckdb")
         == "SELECT name -> '$.k' FROM semi"
     )
 
 
 def test_integer_precision() -> None:
     assert (
         sqlglot.parse_one(
             """
                 create table example (
-                    ENUMBER NUMBER, ENUMBER20 NUMBER(2,0), EDECIMAL DECIMAL, ENUMERIC NUMERIC,
-                    EINT INT, EINTEGER INTEGER, EBIGINT BIGINT, ESMALLINT SMALLINT, ETINYINT TINYINT, EBYTEINT BYTEINT
+                    XNUMBER82 NUMBER(8, 2), XNUMBER NUMBER,  XDECIMAL DECIMAL, XNUMERIC NUMERIC,
+                    XINT INT, XINTEGER INTEGER, XBIGINT BIGINT, XSMALLINT SMALLINT, XTINYINT TINYINT, XBYTEINT BYTEINT
                 )
             """,
             read="snowflake",
         )
         .transform(integer_precision)
         .sql(dialect="duckdb")
-        == "CREATE TABLE example (ENUMBER DECIMAL(38, 0), ENUMBER20 DECIMAL(2, 0), EDECIMAL DECIMAL(38, 0), ENUMERIC DECIMAL(38, 0), EINT DECIMAL(38, 0), EINTEGER DECIMAL(38, 0), EBIGINT DECIMAL(38, 0), ESMALLINT DECIMAL(38, 0), ETINYINT DECIMAL(38, 0), EBYTEINT DECIMAL(38, 0))"  # noqa: E501
+        == "CREATE TABLE example (XNUMBER82 DECIMAL(8, 2), XNUMBER BIGINT, XDECIMAL BIGINT, XNUMERIC BIGINT, XINT BIGINT, XINTEGER BIGINT, XBIGINT BIGINT, XSMALLINT BIGINT, XTINYINT BIGINT, XBYTEINT BIGINT)"  # noqa: E501
     )
 
 
 def test_information_schema_columns_snowflake() -> None:
     assert (
         sqlglot.parse_one("SELECT * FROM INFORMATION_SCHEMA.COLUMNS")
         .transform(information_schema_columns_snowflake)
@@ -143,21 +141,28 @@
         sqlglot.parse_one("""insert into table1 (name) select parse_json('{"first":"foo", "last":"bar"}')""")
         .transform(parse_json)
         .sql()
         == """INSERT INTO table1 (name) SELECT JSON('{"first":"foo", "last":"bar"}')"""
     )
 
 
-def test_regex() -> None:
+def test_regex_replace() -> None:
     assert (
-        sqlglot.parse_one("SELECT regexp_replace('abc123', '\\\\D', '')").transform(regex).sql()
+        sqlglot.parse_one("SELECT regexp_replace('abc123', '\\\\D', '')").transform(regex_replace).sql()
         == "SELECT REGEXP_REPLACE('abc123', '\\D', '', 'g')"
     )
 
 
+def test_regex_substr() -> None:
+    assert (
+        sqlglot.parse_one("SELECT regexp_substr(string1, 'the\\\\W+\\\\w+')").transform(regex_substr).sql()
+        == "SELECT REGEXP_EXTRACT_ALL(string1[1 : ], 'the\\W+\\w+', 0, '')[1]"
+    )
+
+
 def test_semi_structured_types() -> None:
     assert (
         sqlglot.parse_one("CREATE TABLE table1 (name object)").transform(semi_structured_types).sql()
         == "CREATE TABLE table1 (name JSON)"
     )
 
     assert (
@@ -219,15 +224,15 @@
         == "SELECT NAME, NAME AS FNAME FROM TABLE1"
     )
 
 
 def test_values_columns() -> None:
     assert (
         sqlglot.parse_one("SELECT * FROM VALUES ('Amsterdam', 1)").transform(values_columns).sql()
-        == """SELECT * FROM (VALUES ('Amsterdam', 1)) AS _("column1", "column2")"""
+        == """SELECT * FROM (VALUES ('Amsterdam', 1)) AS _("COLUMN1", "COLUMN2")"""
     )
 
     # values without select aren't transformed
     assert (
         sqlglot.parse_one("INSERT INTO cities VALUES ('Amsterdam', 1)").transform(values_columns).sql()
         == "INSERT INTO cities VALUES ('Amsterdam', 1)"
     )
```

