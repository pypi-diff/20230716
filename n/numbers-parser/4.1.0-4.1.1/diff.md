# Comparing `tmp/numbers_parser-4.1.0.tar.gz` & `tmp/numbers_parser-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.1.0.tar", max compression
+gzip compressed data, was "numbers_parser-4.1.1.tar", max compression
```

## Comparing `numbers_parser-4.1.0.tar` & `numbers_parser-4.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.1.0/LICENSE.rst
--rw-r--r--   0        0        0    19997 2023-07-16 12:27:47.599605 numbers_parser-4.1.0/README.md
--rw-r--r--   0        0        0     2096 2023-07-16 09:51:33.459176 numbers_parser-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     2045 2023-07-08 11:12:33.341467 numbers_parser-4.1.0/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4393 2023-07-08 11:18:53.021077 numbers_parser-4.1.0/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5866 2023-07-08 11:12:33.342613 numbers_parser-4.1.0/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.1.0/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    17962 2023-07-16 12:54:10.190164 numbers_parser-4.1.0/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    29708 2023-07-14 19:05:10.686584 numbers_parser-4.1.0/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     1689 2023-07-16 11:18:31.505310 numbers_parser-4.1.0/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.1.0/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.1.0/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    17568 2023-07-16 08:43:05.982097 numbers_parser-4.1.0/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.1.0/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      234 2023-07-08 11:12:33.345442 numbers_parser-4.1.0/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     3865 2023-07-14 19:05:10.688785 numbers_parser-4.1.0/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.1.0/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-07-10 11:50:37.380120 numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-07-10 11:50:37.381233 numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-07-10 11:50:37.381940 numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-07-10 11:50:37.383021 numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17361 2023-07-10 11:50:37.383432 numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-07-10 11:50:37.383703 numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-10 11:50:37.383945 numbers_parser-4.1.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-07-10 11:50:37.384822 numbers_parser-4.1.0/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-07-10 11:50:37.385161 numbers_parser-4.1.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-07-10 11:50:37.385944 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-07-10 11:50:37.386335 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    22717 2023-07-10 11:50:37.386667 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-07-10 11:50:37.387194 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-07-10 11:50:37.387691 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-07-10 11:50:37.387967 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-07-10 11:50:37.388832 numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-07-10 11:50:37.389137 numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-07-10 11:50:37.389550 numbers_parser-4.1.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-07-10 11:50:37.390046 numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-07-10 11:50:37.390302 numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-07-10 11:50:37.390611 numbers_parser-4.1.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-07-10 11:50:37.390860 numbers_parser-4.1.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12611 2023-07-10 11:50:37.391120 numbers_parser-4.1.0/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9717 2023-07-10 11:50:37.391599 numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-07-10 11:50:37.391866 numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-07-10 11:50:37.392988 numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-07-10 11:50:37.393496 numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-07-10 11:50:37.394520 numbers_parser-4.1.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-07-10 11:50:37.394909 numbers_parser-4.1.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    58663 2023-07-10 11:50:37.396073 numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2023-07-10 11:50:37.396468 numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-07-10 11:50:37.397211 numbers_parser-4.1.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-07-10 11:50:37.401529 numbers_parser-4.1.0/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22604 2023-07-16 09:02:55.094582 numbers_parser-4.1.0/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-07-14 19:05:10.690473 numbers_parser-4.1.0/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    12032 2023-07-15 11:47:48.837033 numbers_parser-4.1.0/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32100 2023-07-10 11:51:11.630380 numbers_parser-4.1.0/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    74772 2023-07-16 12:53:29.919068 numbers_parser-4.1.0/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2690 2023-07-08 11:12:33.356950 numbers_parser-4.1.0/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    21174 1970-01-01 00:00:00.000000 numbers_parser-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.1.1/LICENSE.rst
+-rw-r--r--   0        0        0    20092 2023-07-16 14:26:24.846490 numbers_parser-4.1.1/README.md
+-rw-r--r--   0        0        0     2096 2023-07-16 17:08:47.778752 numbers_parser-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2045 2023-07-08 11:12:33.341467 numbers_parser-4.1.1/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4350 2023-07-16 15:02:05.843221 numbers_parser-4.1.1/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5826 2023-07-16 15:04:36.595811 numbers_parser-4.1.1/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.1.1/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    17976 2023-07-16 17:03:54.394032 numbers_parser-4.1.1/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    29688 2023-07-16 17:05:59.012525 numbers_parser-4.1.1/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1689 2023-07-16 11:18:31.505310 numbers_parser-4.1.1/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.1.1/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.1.1/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    17568 2023-07-16 14:14:17.514493 numbers_parser-4.1.1/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.1.1/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.1.1/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     3865 2023-07-14 19:05:10.688785 numbers_parser-4.1.1/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.1.1/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-07-10 11:50:37.380120 numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-07-10 11:50:37.381233 numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-07-10 11:50:37.381940 numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-07-10 11:50:37.383021 numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17361 2023-07-10 11:50:37.383432 numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-07-10 11:50:37.383703 numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-10 11:50:37.383945 numbers_parser-4.1.1/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-07-10 11:50:37.384822 numbers_parser-4.1.1/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-07-10 11:50:37.385161 numbers_parser-4.1.1/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-07-10 11:50:37.385944 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-07-10 11:50:37.386335 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    22717 2023-07-10 11:50:37.386667 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-07-10 11:50:37.387194 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-07-10 11:50:37.387691 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-07-10 11:50:37.387967 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-07-10 11:50:37.388832 numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-07-10 11:50:37.389137 numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-07-10 11:50:37.389550 numbers_parser-4.1.1/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-07-10 11:50:37.390046 numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-07-10 11:50:37.390302 numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-07-10 11:50:37.390611 numbers_parser-4.1.1/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-07-10 11:50:37.390860 numbers_parser-4.1.1/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12611 2023-07-10 11:50:37.391120 numbers_parser-4.1.1/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9717 2023-07-10 11:50:37.391599 numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-07-10 11:50:37.391866 numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-07-10 11:50:37.392988 numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-07-10 11:50:37.393496 numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-07-10 11:50:37.394520 numbers_parser-4.1.1/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-07-10 11:50:37.394909 numbers_parser-4.1.1/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    58663 2023-07-10 11:50:37.396073 numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-07-10 11:50:37.396468 numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-07-10 11:50:37.397211 numbers_parser-4.1.1/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:50:37.401529 numbers_parser-4.1.1/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22604 2023-07-16 09:02:55.094582 numbers_parser-4.1.1/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-07-14 19:05:10.690473 numbers_parser-4.1.1/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    12032 2023-07-15 11:47:48.837033 numbers_parser-4.1.1/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32100 2023-07-10 11:51:11.630380 numbers_parser-4.1.1/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    75106 2023-07-16 16:55:17.689748 numbers_parser-4.1.1/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2690 2023-07-08 11:12:33.356950 numbers_parser-4.1.1/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    21269 1970-01-01 00:00:00.000000 numbers_parser-4.1.1/PKG-INFO
```

### Comparing `numbers_parser-4.1.0/LICENSE.rst` & `numbers_parser-4.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/README.md` & `numbers_parser-4.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -327,14 +327,16 @@
     italic=True,
     alignment=Alignment("right", "top"),
 )
 table.write("B2", "Red", style=red_text)
 table.set_cell_style("C2", red_text)
 ```
 
+New styles are automatically added to the list of styles selectable in the Numbers Text pane.
+
 Cell styles can also be referred to by name in both `Table.write` and `Table.set_cell_style`. A `dict` of available styles is returned by `Document.styles`. This contains key value pairs of style names and `Style` objects. Any changes to `Style` objects in the document are written back such that those styles are changed for all cells that use them.
 
 ``` python
 doc = Document("styles.numbers")
 styles = doc.styles
 styles["Title"].font_size = 20.0
 ```
```

### Comparing `numbers_parser-4.1.0/pyproject.toml` & `numbers_parser-4.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.1.0"
+version = "4.1.1"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
```

### Comparing `numbers_parser-4.1.0/src/numbers_parser/__init__.py` & `numbers_parser-4.1.1/src/numbers_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.1.1/src/numbers_parser/_cat_numbers.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             try:
                 if args.list_sheets:
                     print_sheet_names(filename)
                 elif args.list_tables:
                     print_table_names(filename)
                 else:
                     print_table(args, filename)
-            except FileFormatError as e:  # pragma: no cover”
+            except FileFormatError as e:
                 print(f"{filename}:", str(e), file=sys.stderr)
                 sys.exit(1)
 
 
 if __name__ == "__main__":
     # execute only if run as a script
-    main()  # pragma: no cover
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `numbers_parser-4.1.0/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.1.1/src/numbers_parser/_unpack_numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             try:
                 read_numbers_file(
                     document,
                     file_handler=lambda filename, blob: process_file(
                         filename, blob, output_dir, args
                     ),
                 )
-            except (FileFormatError, FileError) as e:  # pragma: no cover
+            except (FileFormatError, FileError) as e:
                 print(f"{document}:", str(e), file=sys.stderr)
                 sys.exit(1)
 
 
 if __name__ == "__main__":
     # execute only if run as a script
-    main()  # pragma: no cover
+    main()
```

### Comparing `numbers_parser-4.1.0/src/numbers_parser/bullets.py` & `numbers_parser-4.1.1/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/cell.py` & `numbers_parser-4.1.1/src/numbers_parser/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,26 @@
 from enum import IntEnum
 from functools import lru_cache
 from pendulum import duration, Duration, DateTime
 from typing import Any, List, Tuple, Union
 
 
 class BackgroundImage:
-    def __init__(self, image_data: bytes, filename: str):
+    def __init__(self, image_data: bytes = None, filename: str = None):
         self._data = image_data
         self._filename = filename
 
     @property
     def data(self) -> bytes:
         """The background image as byts for a cell, or None if no image."""
         return self._data
 
     @property
     def filename(self) -> str:
         """The image filename for a cell, or None if no image."""
-        if self._data is None:
-            return None
         return self._filename
 
 
 # Style return types
 _Alignment = namedtuple("Alignment", ["horizontal", "vertical"])
 RGB = namedtuple("RGB", ["r", "g", "b"])
 
@@ -151,31 +149,33 @@
         )
         return style
 
     def __post_init__(self):
         if not isinstance(self.alignment, Alignment):
             raise TypeError("value must be an Alignment class")
 
-        check_rgb_type(self.bg_color)
-        check_rgb_type(self.font_color)
+        self.bg_color = rgb_color(self.bg_color)
+        self.font_color = rgb_color(self.font_color)
 
         if not isinstance(self.font_size, float):
             raise TypeError("size must be a float number of points")
         if not isinstance(self.font_name, str):
-            raise TypeError("argument must be a string")
+            raise TypeError("font name must be a string")
 
         for field in ["bold", "italic", "underline", "strikethrough"]:
             if not isinstance(getattr(self, field), bool):
                 raise TypeError(f"{field} argument must be boolean")
 
     def __setattr__(self, name: str, value: Any) -> None:
         """Detect changes to cell styles and flag the style for
         possible updates when saving the document"""
         if name in self.__dict__:
             # Init has been done
+            if name in ["bg_color", "font_color"]:
+                value = rgb_color(value)
             if name in ["bg_color"]:
                 self.__dict__["_update_cell_style"] = True
             elif name in ["alignment"]:
                 self.__dict__["_update_text_style"] = True
                 self.__dict__["_update_cell_style"] = True
             elif name in Style._text_attrs():
                 self.__dict__["_update_text_style"] = True
@@ -187,25 +187,26 @@
             and value[1] != DEFAULT_ALIGNMENT_CLASS[1]
         ):
             self.__dict__["_update_cell_style"] = True
         if name not in ["_update_text_style", "_update_cell_style"]:
             self.__dict__[name] = value
 
 
-def check_rgb_type(color) -> RGB:
+def rgb_color(color) -> RGB:
     """Raise a TypeError if a color is not a valid RGB value"""
     if color is None:
-        return
+        return None
     if isinstance(color, RGB):
-        return
+        return color
     if isinstance(color, tuple):
         if not (len(color) == 3 and all([isinstance(x, int) for x in color])):
             raise TypeError("RGB color must be an RGB or a tuple of 3 integers")
+        return RGB(*color)
     elif isinstance(color, list):
-        [check_rgb_type(c) for c in color]
+        return [rgb_color(c) for c in color]
 
 
 class Cell:
     @classmethod
     def empty_cell(cls, table_id: int, row_num: int, col_num: int, model: object):
         row_col = (row_num, col_num)
         merge_cells = model.merge_cell_ranges(table_id)
@@ -241,17 +242,17 @@
             value = duration(seconds=cell_storage.value)
             cell = DurationCell(*row_col, value)
         elif cell_storage.type == CellType.ERROR:
             cell = ErrorCell(*row_col)
         elif cell_storage.type == CellType.RICH_TEXT:
             cell = RichTextCell(*row_col, cell_storage.value)
         else:
-            raise UnsupportedError(  # pragma: no cover
-                f"Unsupport cell type {cell_storage.type} "
-                + "@:({cell_storage.row_num},{cell_storage.col_num})"
+            raise UnsupportedError(
+                f"Unsupported cell type {cell_storage.type} "
+                + f"@:({cell_storage.row_num},{cell_storage.col_num})"
             )
 
         cell._table_id = cell_storage.table_id
         cell._model = cell_storage.model
         cell._storage = cell_storage
         cell._formula_key = cell_storage.formula_id
         cell._style = None
@@ -518,18 +519,18 @@
        row:     The cell row.    Int.
        col:     The cell column. Int.
        row_abs: Optional flag to make the row absolute.    Bool.
        col_abs: Optional flag to make the column absolute. Bool.
     Returns:
         A1 style string.
     """
-    if row < 0:  # pragma: no cover
-        raise IndexError(f"Row reference {row} below zero")
+    if row < 0:
+        raise IndexError(f"row reference {row} below zero")
 
-    if col < 0:  # pragma: no cover
+    if col < 0:
         raise IndexError(f"column reference {col} below zero")
 
     row += 1  # Change to 1-index.
     row_abs = "$" if row_abs else ""
 
     col_str = xl_col_to_name(col, col_abs)
 
@@ -542,26 +543,26 @@
     Args:
        col:     The cell column. Int.
        col_abs: Optional flag to make the column absolute. Bool.
     Returns:
         Column style string.
     """
     col_num = col
-    if col_num < 0:  # pragma: no cover
-        raise IndexError(f"Column reference {col_num} below zero")
+    if col_num < 0:
+        raise IndexError(f"column reference {col_num} below zero")
 
     col_num += 1  # Change to 1-index.
     col_str = ""
     col_abs = "$" if col_abs else ""
 
     while col_num:
         # Set remainder from 1 .. 26
         remainder = col_num % 26
 
-        if remainder == 0:  # pragma: no cover
+        if remainder == 0:
             remainder = 26
 
         # Convert the remainder to a character.
         col_letter = chr(ord("A") + remainder - 1)
 
         # Accumulate the column letters, right to left.
         col_str = col_letter + col_str
```

### Comparing `numbers_parser-4.1.0/src/numbers_parser/cell_storage.py` & `numbers_parser-4.1.1/src/numbers_parser/cell_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
             self.type = CellType.ERROR
         elif cell_type == TSTArchives.automaticCellType:
             self.value = self.model.table_rich_text(self.table_id, self.rich_id)
             self.type = CellType.RICH_TEXT
         elif cell_type == 10:
             self.value = self.d128
             self.type = CellType.NUMBER
-        else:  # pragma: no cover
+        else:
             raise UnsupportedError(f"Cell type ID {cell_type} is not recognised")
 
         # debug(
         #     "cell@[%d,%d]: table_id=%d, type=%s, value=%s",
         #     row_num,
         #     col_num,
         #     table_id,
```

### Comparing `numbers_parser-4.1.0/src/numbers_parser/constants.py` & `numbers_parser-4.1.1/src/numbers_parser/constants.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/containers.py` & `numbers_parser-4.1.1/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/data/empty.numbers` & `numbers_parser-4.1.1/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/document.py` & `numbers_parser-4.1.1/src/numbers_parser/document.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/exceptions.py` & `numbers_parser-4.1.1/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/file.py` & `numbers_parser-4.1.1/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/formula.py` & `numbers_parser-4.1.1/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/fontmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.1.1/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/iwafile.py` & `numbers_parser-4.1.1/src/numbers_parser/iwafile.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/mapping.py` & `numbers_parser-4.1.1/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/src/numbers_parser/model.py` & `numbers_parser-4.1.1/src/numbers_parser/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
         self.objects = ObjectStore(filename)
         self._merge_cells = {}
         self._row_heights = {}
         self._col_widths = {}
         self._table_formats = DataLists(self, "format_table")
         self._table_styles = DataLists(self, "styleTable", "reference")
         self._table_strings = DataLists(self, "stringTable", "string")
+        self._styles = None
 
     @property
     def file_store(self):
         return self.objects.file_store
 
     def find_refs(self, ref: str) -> list:
         return self.objects.find_refs(ref)
@@ -1148,15 +1149,17 @@
             TSPMessages.Reference(identifier=sheet_id)
         )
 
         return sheet_id
 
     @property
     def styles(self):
-        return self.available_paragraph_styles()
+        if self._styles is None:
+            self._styles = self.available_paragraph_styles()
+        return self._styles
 
     @lru_cache(maxsize=None)
     def available_paragraph_styles(self) -> List[Style]:
         theme_id = self.objects[DOCUMENT_ID].theme.identifier
         presets = find_extension(
             self.objects[theme_id].super, "paragraph_style_presets"
         )
@@ -1242,15 +1245,21 @@
         )
         self.objects[stylesheet_id].identifier_to_style_map.append(
             TSSArchives.StylesheetArchive.IdentifiedStyleEntry(
                 identifier=style_id_name,
                 style=TSPMessages.Reference(identifier=para_style_id),
             )
         )
-        # TODO: add style to theme
+
+        theme_id = self.objects[DOCUMENT_ID].theme.identifier
+        presets = find_extension(
+            self.objects[theme_id].super, "paragraph_style_presets"
+        )
+        presets.append(TSPMessages.Reference(identifier=para_style_id))
+        self._styles[style.name] = style
         return para_style_id
 
     def update_paragraph_style(self, style: Style):
         if style.underline:
             underline = CharacterStyle.UnderlineType.kSingleUnderline
         else:
             underline = CharacterStyle.UnderlineType.kNoUnderline
@@ -1456,15 +1465,15 @@
                 flags = 0
                 cell_type = TSTArchives.emptyCellValueType
                 value = b""
             else:
                 return None
         elif isinstance(cell, MergedCell):
             return None
-        else:  # pragma: no cover
+        else:
             data_type = type(cell).__name__
             table_name = self.table_name(table_id)
             warn(
                 f"@{table_name}:[{row_num},{col_num}]: unsupported data type {data_type} for save",
                 UnsupportedWarning,
             )
             return None
```

### Comparing `numbers_parser-4.1.0/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.1.1/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.0/PKG-INFO` & `numbers_parser-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-parser
-Version: 4.1.0
+Version: 4.1.1
 Summary: Read and write Apple Numbers spreadsheets
 Home-page: https://github.com/masaccio/numbers-parser
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -355,14 +355,16 @@
     italic=True,
     alignment=Alignment("right", "top"),
 )
 table.write("B2", "Red", style=red_text)
 table.set_cell_style("C2", red_text)
 ```
 
+New styles are automatically added to the list of styles selectable in the Numbers Text pane.
+
 Cell styles can also be referred to by name in both `Table.write` and `Table.set_cell_style`. A `dict` of available styles is returned by `Document.styles`. This contains key value pairs of style names and `Style` objects. Any changes to `Style` objects in the document are written back such that those styles are changed for all cells that use them.
 
 ``` python
 doc = Document("styles.numbers")
 styles = doc.styles
 styles["Title"].font_size = 20.0
 ```
```

