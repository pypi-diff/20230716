# Comparing `tmp/numbers_parser-4.0.0.tar.gz` & `tmp/numbers_parser-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.0.0.tar", max compression
+gzip compressed data, was "numbers_parser-4.1.0.tar", max compression
```

## Comparing `numbers_parser-4.0.0.tar` & `numbers_parser-4.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.0.0/LICENSE.rst
--rw-r--r--   0        0        0    18173 2023-07-14 19:12:21.819626 numbers_parser-4.0.0/README.md
--rw-r--r--   0        0        0     2096 2023-07-14 19:05:10.684871 numbers_parser-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     2045 2023-07-08 11:12:33.341467 numbers_parser-4.0.0/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4393 2023-07-08 11:18:53.021077 numbers_parser-4.0.0/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5866 2023-07-08 11:12:33.342613 numbers_parser-4.0.0/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.0.0/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    18088 2023-07-14 19:05:10.685880 numbers_parser-4.0.0/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    29708 2023-07-14 19:05:10.686584 numbers_parser-4.0.0/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     2404 2023-07-14 19:05:10.687055 numbers_parser-4.0.0/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.0.0/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.0.0/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    15806 2023-07-14 19:05:10.687768 numbers_parser-4.0.0/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.0.0/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      234 2023-07-08 11:12:33.345442 numbers_parser-4.0.0/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     3865 2023-07-14 19:05:10.688785 numbers_parser-4.0.0/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.0.0/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-07-10 11:50:37.380120 numbers_parser-4.0.0/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-07-10 11:50:37.381233 numbers_parser-4.0.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-07-10 11:50:37.381940 numbers_parser-4.0.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-07-10 11:50:37.383021 numbers_parser-4.0.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17361 2023-07-10 11:50:37.383432 numbers_parser-4.0.0/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-07-10 11:50:37.383703 numbers_parser-4.0.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-10 11:50:37.383945 numbers_parser-4.0.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-07-10 11:50:37.384822 numbers_parser-4.0.0/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-07-10 11:50:37.385161 numbers_parser-4.0.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-07-10 11:50:37.385944 numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-07-10 11:50:37.386335 numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    22717 2023-07-10 11:50:37.386667 numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-07-10 11:50:37.387194 numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-07-10 11:50:37.387691 numbers_parser-4.0.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-07-10 11:50:37.387967 numbers_parser-4.0.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-07-10 11:50:37.388832 numbers_parser-4.0.0/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-07-10 11:50:37.389137 numbers_parser-4.0.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-07-10 11:50:37.389550 numbers_parser-4.0.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-07-10 11:50:37.390046 numbers_parser-4.0.0/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-07-10 11:50:37.390302 numbers_parser-4.0.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-07-10 11:50:37.390611 numbers_parser-4.0.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-07-10 11:50:37.390860 numbers_parser-4.0.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12611 2023-07-10 11:50:37.391120 numbers_parser-4.0.0/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9717 2023-07-10 11:50:37.391599 numbers_parser-4.0.0/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-07-10 11:50:37.391866 numbers_parser-4.0.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-07-10 11:50:37.392988 numbers_parser-4.0.0/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-07-10 11:50:37.393496 numbers_parser-4.0.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-07-10 11:50:37.394520 numbers_parser-4.0.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-07-10 11:50:37.394909 numbers_parser-4.0.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    58663 2023-07-10 11:50:37.396073 numbers_parser-4.0.0/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2023-07-10 11:50:37.396468 numbers_parser-4.0.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-07-10 11:50:37.397211 numbers_parser-4.0.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-07-10 11:50:37.401529 numbers_parser-4.0.0/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22598 2023-07-14 19:05:10.690127 numbers_parser-4.0.0/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-07-14 19:05:10.690473 numbers_parser-4.0.0/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    11647 2023-07-14 19:05:10.691139 numbers_parser-4.0.0/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32100 2023-07-10 11:51:11.630380 numbers_parser-4.0.0/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    68192 2023-07-14 19:05:10.691815 numbers_parser-4.0.0/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2690 2023-07-08 11:12:33.356950 numbers_parser-4.0.0/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    19350 1970-01-01 00:00:00.000000 numbers_parser-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.1.0/LICENSE.rst
+-rw-r--r--   0        0        0    19997 2023-07-16 12:27:47.599605 numbers_parser-4.1.0/README.md
+-rw-r--r--   0        0        0     2096 2023-07-16 09:51:33.459176 numbers_parser-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2045 2023-07-08 11:12:33.341467 numbers_parser-4.1.0/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4393 2023-07-08 11:18:53.021077 numbers_parser-4.1.0/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5866 2023-07-08 11:12:33.342613 numbers_parser-4.1.0/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.1.0/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    17962 2023-07-16 12:54:10.190164 numbers_parser-4.1.0/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    29708 2023-07-14 19:05:10.686584 numbers_parser-4.1.0/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1689 2023-07-16 11:18:31.505310 numbers_parser-4.1.0/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.1.0/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.1.0/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    17568 2023-07-16 08:43:05.982097 numbers_parser-4.1.0/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.1.0/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      234 2023-07-08 11:12:33.345442 numbers_parser-4.1.0/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     3865 2023-07-14 19:05:10.688785 numbers_parser-4.1.0/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.1.0/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-07-10 11:50:37.380120 numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-07-10 11:50:37.381233 numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-07-10 11:50:37.381940 numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-07-10 11:50:37.383021 numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17361 2023-07-10 11:50:37.383432 numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-07-10 11:50:37.383703 numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-10 11:50:37.383945 numbers_parser-4.1.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-07-10 11:50:37.384822 numbers_parser-4.1.0/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-07-10 11:50:37.385161 numbers_parser-4.1.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-07-10 11:50:37.385944 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-07-10 11:50:37.386335 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    22717 2023-07-10 11:50:37.386667 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-07-10 11:50:37.387194 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-07-10 11:50:37.387691 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-07-10 11:50:37.387967 numbers_parser-4.1.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-07-10 11:50:37.388832 numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-07-10 11:50:37.389137 numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-07-10 11:50:37.389550 numbers_parser-4.1.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-07-10 11:50:37.390046 numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-07-10 11:50:37.390302 numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-07-10 11:50:37.390611 numbers_parser-4.1.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-07-10 11:50:37.390860 numbers_parser-4.1.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12611 2023-07-10 11:50:37.391120 numbers_parser-4.1.0/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9717 2023-07-10 11:50:37.391599 numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-07-10 11:50:37.391866 numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-07-10 11:50:37.392988 numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-07-10 11:50:37.393496 numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-07-10 11:50:37.394520 numbers_parser-4.1.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-07-10 11:50:37.394909 numbers_parser-4.1.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    58663 2023-07-10 11:50:37.396073 numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-07-10 11:50:37.396468 numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-07-10 11:50:37.397211 numbers_parser-4.1.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:50:37.401529 numbers_parser-4.1.0/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22604 2023-07-16 09:02:55.094582 numbers_parser-4.1.0/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-07-14 19:05:10.690473 numbers_parser-4.1.0/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    12032 2023-07-15 11:47:48.837033 numbers_parser-4.1.0/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32100 2023-07-10 11:51:11.630380 numbers_parser-4.1.0/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    74772 2023-07-16 12:53:29.919068 numbers_parser-4.1.0/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2690 2023-07-08 11:12:33.356950 numbers_parser-4.1.0/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    21174 1970-01-01 00:00:00.000000 numbers_parser-4.1.0/PKG-INFO
```

### Comparing `numbers_parser-4.0.0/LICENSE.rst` & `numbers_parser-4.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/README.md` & `numbers_parser-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: numbers-parser
+Version: 4.1.0
+Summary: Read and write Apple Numbers spreadsheets
+Home-page: https://github.com/masaccio/numbers-parser
+License: MIT
+Author: Jon Connell
+Author-email: python@figsandfudge.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
+Requires-Dist: compact-json (>=1.1.3,<2.0.0)
+Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: protobuf (>=4.21.1,<5.0.0)
+Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
+Requires-Dist: regex (>=2022.9.13,<2023.0.0)
+Requires-Dist: roman (>=3.3,<4.0)
+Project-URL: Documentation, https://github.com/masaccio/numbers-parser/blob/main/README.md
+Project-URL: Repository, https://github.com/masaccio/numbers-parser
+Description-Content-Type: text/markdown
+
 # numbers-parser
 
 [![build:](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml)
 [![build:](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml)
 [![codecov](https://codecov.io/gh/masaccio/numbers-parser/branch/main/graph/badge.svg?token=EKIUFGT05E)](https://codecov.io/gh/masaccio/numbers-parser)
 
 `numbers-parser` is a Python module for parsing [Apple Numbers](https://www.apple.com/numbers/)
@@ -10,15 +38,15 @@
 
 It supports and is tested against Python versions from 3.8 onwards. It is not compatible with earlier versions of Python.
 
 Formula evaluation relies on Numbers storing current values which should usually be the case. Formulas themselves rather than the computed values can optionally be extracted. [Style support](#styles) is somewhat limited, but has grown significantly as of version 4.0.
 
 ## API changes in version 4.0
 
-To better partition cell styles, the new cell property `style` contains all style information for a cell including background image data which was supported in earlier versions. Image information is now found in `cell.style.bg_image`. Using the deprecated methods `image_data` and `image_filename` will issue a `DeprecationWarning` if used.The legacy methods will be removed in a future version of numbers-parser.
+To better partition cell styles, background image data which was supported in earlier versions through the methods `image_data` and `image_filename` is now part of the new `cell_style` property. Using the deprecated methods `image_data` and `image_filename` will issue a `DeprecationWarning` if used.The legacy methods will be removed in a future version of numbers-parser.
 
 `NumberCell` cell types return [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html) types rather than `float`. These are created in a [decimal128](https://en.wikipedia.org/wiki/Decimal128_floating-point_format) context to preserve the precision used by Numbers. Previously, using float resulted in rounding errors in unpacking internal numbers.
 
 ## Installation
 
 ``` bash
 python3 -m pip install numbers-parser
@@ -173,37 +201,40 @@
 ``` python
 cell = table.cell(0, 0)
 (text, url) = cell.hyperlinks[0]
 ```
 
 ### Styles
 
-`numbers_parser` has very limited support for cell styles. Currently only cell backgrounds are supported.
-
-#### Cell background colour
-
-The `bg_color` cell property returns either a tuple of RGB values or, in the case of gradient backgrounds, a list of tuples with each colour in the gradient. If no background color is defined, `None` is returned.
-
-``` python
-rgb = table.cell("B1").bg_color
-print("B1 RGB =", rgb[0], rgb[1], rgb[2])
-```
+`numbers_parser` currently only supports paragraph styles and cell styles. The following paragraph styles are suppoprted:
 
-#### Cell text attributes
-
-Cell text fonts can be returned using a number of methods. Formatting changes within cells such as "This is **bold** text" are not supported.
-
-* `cell.style.name`: cell style (`str`)
-* `cell.style.is_bold`: `True` if the cell font is bold
-* `cell.style.is_italic`: `True` if the cell font is italic
-* `cell.style.is_underline`: `True` if the cell font is underline
-* `cell.style.is_strikethrough`: `True` if the cell font is strikethrough
-* `cell.style.font_color`: font color as a tuple of RGB values
-* `cell.style.font_size`: font size in points (`float`)
-* `cell.style.font_name`: font name (`str`)
+* font attributes: bold, italic, underline, strikethrough
+* font selection and size
+* text foreground color
+* horizontal and vertical alignment
+* cell background color
+
+Table styles that allow new tables to adopt a style across the whole table are not planned.
+
+#### Reading styles
+
+The cell method `style` returns a `Style` object containing all the style information for that cell. Cells with identical style settings contain references to a single style object.
+
+Cell text fonts can be returned using a number of methods.
+
+* `Cell.style.alignment`: the horizontal and vertical alignment of the cell as an `Alignment` names tuple
+* `Cell.style.bg_color`: cell background color as an `RGB` named tuple, or a list of `RGB` values for gradients
+* `Cell.style.bold`: `True` if the cell font is bold
+* `Cell.style.font_color`: font color as an `RGB` named tuple
+* `Cell.style.font_size`: font size in points (`float`)
+* `Cell.style.font_name`: font name (`str`)
+* `Cell.style.italic`: `True` if the cell font is italic
+* `Cell.style.name`: cell style (`str`)
+* `Cell.style.underline`: `True` if the cell font is underline
+* `Cell.style.strikethrough`: `True` if the cell font is strikethrough
 
 #### Cell images
 
 The methods `style.bg_image.filename` and `style.bg_image.data` return data about the image used for a cell's background, where set. If a cell has no background image, `style.bg_image`  is `None`.
 
 ``` python
 cell = table.cell("B1")
@@ -213,23 +244,23 @@
 
 ## Writing Numbers files
 
 Whilst support for writing numbers files has been stable since version 3.4.0, you are highly recommened not to overwrite working Numbers files and instead save data to a new file.
 
 ### Limitations
 
-Since version 3.4.0, adding tables and sheets is supported. Known limitations to write support are:
+Current limitations to write support are:
 
 * Creating cells of type `BulletedTextCell` is not supported
 * Formats cannot be defined for `DurationCell` or `DateCell`
 * New tables are inserted with a fixed offset below the last table in a worksheet which does not take into account title or caption size
 * New sheets insert tables with formats copied from the first table in the previous sheet rather than default table formats
-* Style cannot be saved.
+* Style editing is limited to paragraph styles.
 
-### Editing cells
+### Cell values
 
 `numbers-parser` will automatically empty rows and columns for any cell references that are out of range of the current table. The `write` method accepts the same cell numbering notation as `cell` plus an additional argument representing the new cell value. The type of the new value will be used to determine the cell type.
 
 ``` python
 doc = Document("old-sheet.numbers")
 sheets = doc.sheets
 tables = sheets[0].tables
@@ -258,19 +289,19 @@
 table.write(1, 1, 1000)
 table.write(1, 2, 2000)
 table.write(1, 3, 3000)
 
 doc.save("sheet.numbers")
 ```
 
-## Table geometries
+### Table geometries
 
 `numbers-parser` can query and change the position and size of tables. Changes made to a table's row height or column width is retained when files are saved.
 
-###  Row and column sizes
+####  Row and column sizes
 
 Row heights and column widths are queried and set using the `row_height` and `col_width` methods:
 
 ```python
 doc = Document("sheet.numbers")
 table = doc.sheets[0].tables[0]
 print(f"Table size is {table.height} x {table.width}")
@@ -278,38 +309,70 @@
 table.row_height(0, 40)
 print(f"Table row 1 height is now {table.row_height(0)}")
 print(f"Table column A width is {table.col_width(0)}")
 table.col_width(0, 200)
 print(f"Table column A width is {table.col_width(0)}")
 ```
 
-###  Header row and columns
+####  Header row and columns
 
 When new tables are created, `numbers-parser` follows the Numbers convention of creating a table with one row header and one column header. You can change the number of headers by modifying the appopriate property:
 
 ```python
 doc = Document("sheet.numbers")
 table = doc.sheets[0].tables[0]
 table.num_header_rows = 2
 table.num_header_cols = 0
 doc.save("saved.numbers")
 ```
 
 A zero header count will remove the headers from the table. Attempting to set a negative number of headers, or using more headers that rows or columns in the table will raise a `ValueError` exception.
 
-### Positioning tables
+#### Positioning tables
 
 By default, new tables are positioned at a fixed offset below the last table vertically in a sheet and on the left side of the sheet. Large table headers and captions may result in new tables overlapping existing ones. The `add_table` method takes optional coordinates for positioning a table. A table's height and coordinates can also be queried to help aligning new tables:
 
 ```python
 (x, y) = sheet.table[0].coordinates
 y += sheet.table[0].height + 200.0
 new_table = sheet.add_table("Offset Table", x, y)
 ```
 
+### Editing paragraph styles
+
+Cell text styles, known as paragraph styles, are those applied by the Text tab in Numbers Format pane. To simplify the API, when writing documents, it is not possible to make ad hoc changes to cells without assigning an existing style or creating a new one. This differs to the Numbers interface where cells can have modified styles on a per cell basis. Such styles are read correctly when reading Numbers files.
+
+Character styles, which allow formatting changes within cells such as "This is **bold** text" are not supported.
+
+Styles are created using the `Document`'s `add_style` method, and can be applied to cells either as part of a `write` or using `set_cell_style`:
+
+``` python
+red_text = doc.add_style(
+    name="Red Text",
+    font_name="Lucida Grande",
+    font_color=RGB(230, 25, 25),
+    font_size=14.0,
+    bold=True,
+    italic=True,
+    alignment=Alignment("right", "top"),
+)
+table.write("B2", "Red", style=red_text)
+table.set_cell_style("C2", red_text)
+```
+
+Cell styles can also be referred to by name in both `Table.write` and `Table.set_cell_style`. A `dict` of available styles is returned by `Document.styles`. This contains key value pairs of style names and `Style` objects. Any changes to `Style` objects in the document are written back such that those styles are changed for all cells that use them.
+
+``` python
+doc = Document("styles.numbers")
+styles = doc.styles
+styles["Title"].font_size = 20.0
+```
+
+Since `Style` objects are shared, changing `Cell.style.font_size` will have the effect of changing the font size for that style and will in turn affect the styles of all cells using that style.
+
 ## Command-line scripts
 
 When installed from [PyPI](https://pypi.org/project/numbers-parser/), a command-like script `cat-numbers` is installed in Python's scripts folder. This script dumps Numbers spreadsheets into Excel-compatible CSV format, iterating through all the spreadsheets passed on the command-line.
 
 ``` text
 usage: cat-numbers [-h] [-T | -S | -b] [-V] [--debug] [--formulas]
                    [--formatting] [-s SHEET] [-t TABLE] [document ...]
@@ -377,7 +440,8 @@
 
 Decimal128 conversion to and from byte storage was adapted from work done by the
 [SheetsJS project](https://github.com/SheetJS/sheetjs). SheetJS also helped greatly with some of the steps required to successfully save a Numbers spreadsheet.
 
 ## License
 
 All code in this repository is licensed under the [MIT License](https://github.com/masaccio/numbers-parser/blob/master/LICENSE.rst)
+
```

### Comparing `numbers_parser-4.0.0/pyproject.toml` & `numbers_parser-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.0.0"
+version = "4.1.0"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
```

### Comparing `numbers_parser-4.0.0/src/numbers_parser/__init__.py` & `numbers_parser-4.1.0/src/numbers_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.1.0/src/numbers_parser/_cat_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.1.0/src/numbers_parser/_unpack_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/bullets.py` & `numbers_parser-4.1.0/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/cell.py` & `numbers_parser-4.1.0/src/numbers_parser/cell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import re
 import warnings
 
 from numbers_parser.generated import TSTArchives_pb2 as TSTArchives
+from numbers_parser.generated.TSWPArchives_pb2 import (
+    ParagraphStylePropertiesArchive as ParagraphStyle,
+)
 from numbers_parser.exceptions import UnsupportedError
 from numbers_parser.cell_storage import CellType, CellStorage
-from numbers_parser.constants import EMPTY_STORAGE_BUFFER, Alignment, RGB
-
+from numbers_parser.constants import (
+    EMPTY_STORAGE_BUFFER,
+    DEFAULT_FONT,
+    DEFAULT_FONT_SIZE,
+    DEFAULT_ALIGNMENT,
+)
+
+from dataclasses import dataclass
+from collections import namedtuple
+from enum import IntEnum
 from functools import lru_cache
 from pendulum import duration, Duration, DateTime
-from typing import List, Tuple, Union
+from typing import Any, List, Tuple, Union
 
 
 class BackgroundImage:
     def __init__(self, image_data: bytes, filename: str):
         self._data = image_data
         self._filename = filename
 
@@ -25,183 +36,176 @@
     def filename(self) -> str:
         """The image filename for a cell, or None if no image."""
         if self._data is None:
             return None
         return self._filename
 
 
-class Style:
-    def __init__(self, cell_storage: object, model: object):
-        self._storage = cell_storage
-        self._model = model
-        self._cell_style_updated = False
-        self._text_style_updated = False
-
-        self._alignment = self._model.cell_alignment(self._storage)
-        if self._storage.image_data is not None:
-            self._bg_image = BackgroundImage(*self._storage.image_data)
-        else:
-            self._bg_image = None
-        self._bg_color = self._model.cell_bg_color(self._storage)
-        self._font_color = self._model.cell_font_color(self._storage)
-        self._font_size = self._model.cell_font_size(self._storage)
-        self._font_name = self._model.cell_font_name(self._storage)
-        self._is_bold = self._model.cell_is_bold(self._storage)
-        self._is_italic = self._model.cell_is_italic(self._storage)
-        self._is_strikethrough = self._model.cell_is_strikethrough(self._storage)
-        self._is_underline = self._model.cell_is_underline(self._storage)
-        self._name = self._model.cell_style_name(self._storage)
+# Style return types
+_Alignment = namedtuple("Alignment", ["horizontal", "vertical"])
+RGB = namedtuple("RGB", ["r", "g", "b"])
 
-    @property
-    def alignment(self) -> Alignment:
-        """The horizontal and vertical alignment of the cell as a named tuple."""
-        return self._alignment
-
-    @alignment.setter
-    def alignment(self, value: Alignment):
-        """Set the horizontal and vertical alignment of the cell."""
-        if not isinstance(value, Alignment):
-            raise TypeError("value must be an Alignment class")
 
-        if self._alignment != value:
-            self._alignment = value
-            self._text_style_updated = True
-            self._cell_style_updated = True
-
-    def check_rgb_type(self, color) -> RGB:
-        if isinstance(color, RGB):
-            return color
-        elif len(color) != 3 or not all([isinstance(x, int) for x in color]):
-            raise TypeError("RGB color must be an RGB or a tuple of 3 integers")
-        else:
-            return RGB(color)
+class HorizontalJustification(IntEnum):
+    LEFT = ParagraphStyle.TextAlignmentType.TATvalue0
+    RIGHT = ParagraphStyle.TextAlignmentType.TATvalue1
+    CENTER = ParagraphStyle.TextAlignmentType.TATvalue2
+    JUSTIFIED = ParagraphStyle.TextAlignmentType.TATvalue3
+    AUTO = ParagraphStyle.TextAlignmentType.TATvalue4
 
-    @property
-    def bg_image(self) -> object:
-        """The background image object for a cell, or None if no background
-        is assigned"""
-        return self._bg_image
 
-    @property
-    def bg_color(self) -> Union[RGB, List[RGB]]:
-        """An named tuple containing the integer (0-255) RGB values for the
-        background color of a cell. For gradients, a list of named tuples
-        for each colr point in the gradient."""
-        return self._bg_color
-
-    @bg_color.setter
-    def bg_color(self, color: Union[RGB, Tuple]):
-        """Set the cell background color to a new RGB value."""
-        color = self.check_rgb_type(color)
-        if self._bg_color != color:
-            self._bg_color = color
-            self._cell_style_updated = True
+class VerticalJustification(IntEnum):
+    TOP = ParagraphStyle.ParagraphBorderType.PBTvalue0
+    MIDDLE = ParagraphStyle.ParagraphBorderType.PBTvalue1
+    BOTTOM = ParagraphStyle.ParagraphBorderType.PBTvalue2
 
-    @property
-    def font_color(self) -> bool:
-        """A named tuple containing the integer (0-255) RGB values for the
-        color f the font for text in the cell."""
-        return self._font_color
-
-    @font_color.setter
-    def font_color(self, color: RGB):
-        """Set the font color to a new RGB value."""
-        color = self.check_rgb_type(color)
-        if self._font_color != color:
-            self._font_color = color
-            self._text_style_updated = True
 
-    @property
-    def font_size(self) -> float:
-        """The point size of the font for the cell."""
-        return self._font_size
-
-    @font_size.setter
-    def font_size(self, size: float):
-        """Set the size of the font for the cell."""
-        if not isinstance(size, float):
-            raise TypeError("size must be a float number of points")
-        if self._font_size != size:
-            self._font_size = size
-            self._text_style_updated = True
+HORIZONTAL_MAP = {
+    "left": HorizontalJustification.LEFT,
+    "right": HorizontalJustification.RIGHT,
+    "center": HorizontalJustification.CENTER,
+    "justified": HorizontalJustification.JUSTIFIED,
+    "auto": HorizontalJustification.AUTO,
+}
 
-    @property
-    def font_name(self) -> str:
-        """The font family assigned to the cell."""
-        return self._font_name
-
-    @font_name.setter
-    def font_name(self, font_name: str):
-        """Set the font for the cell."""
-        if not isinstance(font_name, str):
-            raise TypeError("argument must be a string")
-        if self._font_name != font_name:
-            self._font_name = font_name
-            self._text_style_updated = True
+VERTICAL_MAP = {
+    "top": VerticalJustification.TOP,
+    "middle": VerticalJustification.MIDDLE,
+    "bottom": VerticalJustification.BOTTOM,
+}
 
-    @property
-    def is_bold(self) -> bool:
-        """True if the cell is formatted to bold."""
-        return self._is_bold
-
-    @is_bold.setter
-    def is_bold(self, bold: bool):
-        """Set the size of the font for the cell."""
-        if not isinstance(bold, bool):
-            raise TypeError("argument must be boolean")
-        if self._is_bold != bold:
-            self._is_bold = bold
-            self._text_style_updated = True
 
-    @property
-    def is_italic(self) -> bool:
-        """True if the cell is formatted to italic."""
-        return self._is_italic
-
-    @is_italic.setter
-    def is_italic(self, italic: bool):
-        """Set the size of the font for the cell."""
-        if not isinstance(italic, bool):
-            raise TypeError("argument must be boolean")
-        if self._is_italic != italic:
-            self._is_italic = italic
-            self._text_style_updated = True
+class Alignment(_Alignment):
+    def __new__(cls, horizontal=DEFAULT_ALIGNMENT[0], vertical=DEFAULT_ALIGNMENT[1]):
+        if isinstance(horizontal, str):
+            horizontal = horizontal.lower()
+            if horizontal not in HORIZONTAL_MAP:
+                raise TypeError("invalid horizontal alignment")
+            horizontal = HORIZONTAL_MAP[horizontal]
 
-    @property
-    def is_strikethrough(self) -> bool:
-        """True if the cell is formatted to strikethrough."""
-        return self._is_strikethrough
-
-    @is_strikethrough.setter
-    def is_strikethrough(self, strikethrough: bool):
-        """Set the size of the font for the cell."""
-        if not isinstance(strikethrough, bool):
-            raise TypeError("argument must be boolean")
-        if self._is_strikethrough != strikethrough:
-            self._is_strikethrough = strikethrough
-            self._text_style_updated = True
+        if isinstance(vertical, str):
+            vertical = vertical.lower()
+            if vertical not in VERTICAL_MAP:
+                raise TypeError("invalid vertical alignment")
+            vertical = VERTICAL_MAP[vertical]
 
-    @property
-    def is_underline(self) -> bool:
-        """True if the cell is formatted to underline."""
-        return self._is_underline
-
-    @is_underline.setter
-    def is_underline(self, underline: bool):
-        """Set the size of the font for the cell."""
-        if not isinstance(underline, bool):
-            raise TypeError("argument must be boolean")
-        if self._is_underline != underline:
-            self._is_underline = underline
-            self._text_style_updated = True
+        self = super(_Alignment, cls).__new__(cls, (horizontal, vertical))
+        return self
 
-    @property
-    def name(self) -> str:
-        """The style name for the cell."""
-        return self._name
+
+DEFAULT_ALIGNMENT_CLASS = Alignment(*DEFAULT_ALIGNMENT)
+
+
+@dataclass
+class Style:
+    alignment: Alignment = DEFAULT_ALIGNMENT_CLASS
+    bg_image: object = None
+    bg_color: Union[RGB, List[RGB]] = None
+    font_color: RGB = RGB(0, 0, 0)
+    font_size: float = DEFAULT_FONT_SIZE
+    font_name: str = DEFAULT_FONT
+    bold: bool = False
+    italic: bool = False
+    strikethrough: bool = False
+    underline: bool = False
+    name: str = None
+    _text_style_id: int = None
+    _cell_style_id: int = None
+    _update_cell_style: bool = False
+    _update_text_style: bool = False
+
+    @staticmethod
+    def _text_attrs():
+        return [
+            "font_color",
+            "font_size",
+            "font_name",
+            "bold",
+            "italic",
+            "strikethrough",
+            "underline",
+            "name",
+        ]
+
+    @classmethod
+    def from_storage(cls, cell_storage: object, model: object):
+        style = Style()
+
+        if cell_storage.image_data is not None:
+            bg_image = BackgroundImage(*cell_storage.image_data)
+        else:
+            bg_image = None
+        style = Style(
+            alignment=model.cell_alignment(cell_storage),
+            bg_image=bg_image,
+            bg_color=model.cell_bg_color(cell_storage),
+            font_color=model.cell_font_color(cell_storage),
+            font_size=model.cell_font_size(cell_storage),
+            font_name=model.cell_font_name(cell_storage),
+            bold=model.cell_is_bold(cell_storage),
+            italic=model.cell_is_italic(cell_storage),
+            strikethrough=model.cell_is_strikethrough(cell_storage),
+            underline=model.cell_is_underline(cell_storage),
+            name=model.cell_style_name(cell_storage),
+            _text_style_id=model.text_style_object_id(cell_storage),
+            _cell_style_id=model.cell_style_object_id(cell_storage),
+        )
+        return style
+
+    def __post_init__(self):
+        if not isinstance(self.alignment, Alignment):
+            raise TypeError("value must be an Alignment class")
+
+        check_rgb_type(self.bg_color)
+        check_rgb_type(self.font_color)
+
+        if not isinstance(self.font_size, float):
+            raise TypeError("size must be a float number of points")
+        if not isinstance(self.font_name, str):
+            raise TypeError("argument must be a string")
+
+        for field in ["bold", "italic", "underline", "strikethrough"]:
+            if not isinstance(getattr(self, field), bool):
+                raise TypeError(f"{field} argument must be boolean")
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        """Detect changes to cell styles and flag the style for
+        possible updates when saving the document"""
+        if name in self.__dict__:
+            # Init has been done
+            if name in ["bg_color"]:
+                self.__dict__["_update_cell_style"] = True
+            elif name in ["alignment"]:
+                self.__dict__["_update_text_style"] = True
+                self.__dict__["_update_cell_style"] = True
+            elif name in Style._text_attrs():
+                self.__dict__["_update_text_style"] = True
+        elif name == "bg_color" and value is not None:
+            self.__dict__["_update_cell_style"] = True
+        elif (
+            name == "alignment"
+            and value is not None
+            and value[1] != DEFAULT_ALIGNMENT_CLASS[1]
+        ):
+            self.__dict__["_update_cell_style"] = True
+        if name not in ["_update_text_style", "_update_cell_style"]:
+            self.__dict__[name] = value
+
+
+def check_rgb_type(color) -> RGB:
+    """Raise a TypeError if a color is not a valid RGB value"""
+    if color is None:
+        return
+    if isinstance(color, RGB):
+        return
+    if isinstance(color, tuple):
+        if not (len(color) == 3 and all([isinstance(x, int) for x in color])):
+            raise TypeError("RGB color must be an RGB or a tuple of 3 integers")
+    elif isinstance(color, list):
+        [check_rgb_type(c) for c in color]
 
 
 class Cell:
     @classmethod
     def empty_cell(cls, table_id: int, row_num: int, col_num: int, model: object):
         row_col = (row_num, col_num)
         merge_cells = model.merge_cell_ranges(table_id)
@@ -210,15 +214,15 @@
         if is_merged and merge_cells[row_col]["merge_type"] == "ref":
             cell = MergedCell(*merge_cells[row_col]["rect"])
         else:
             cell = EmptyCell(row_num, col_num)
         cell.size = None
         cell._model = model
         cell._table_id = table_id
-        cell._style = None
+        cell.style = None
         return cell
 
     @classmethod
     def from_storage(cls, cell_storage: CellStorage):  # noqa: C901
         row_col = (cell_storage.row_num, cell_storage.col_num)
         merge_cells = cell_storage.model.merge_cell_ranges(cell_storage.table_id)
         is_merged = row_col in merge_cells
@@ -318,19 +322,22 @@
 
     @property
     def style(self):
         if self._storage is None:
             self._storage = CellStorage(
                 self._model, self._table_id, EMPTY_STORAGE_BUFFER, self.row, self.col
             )
-            self._style = Style(self._storage, self._model)
-        elif self._style is None:
-            self._style = Style(self._storage, self._model)
+        if self._style is None:
+            self._style = Style.from_storage(self._storage, self._model)
         return self._style
 
+    @style.setter
+    def style(self, style):
+        self._style = style
+
 
 class NumberCell(Cell):
     def __init__(self, row_num: int, col_num: int, value: float):
         self._type = TSTArchives.numberCellType
         super().__init__(row_num, col_num, value)
 
     @property
```

### Comparing `numbers_parser-4.0.0/src/numbers_parser/cell_storage.py` & `numbers_parser-4.1.0/src/numbers_parser/cell_storage.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/containers.py` & `numbers_parser-4.1.0/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/data/empty.numbers` & `numbers_parser-4.1.0/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/document.py` & `numbers_parser-4.1.0/src/numbers_parser/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,36 @@
     TextCell,
     DurationCell,
     DateCell,
     Cell,
     MergedCell,
     xl_cell_to_rowcol,
     xl_range,
+    Style,
 )
 from numbers_parser.cell_storage import CellStorage
 from numbers_parser.constants import DEFAULT_COLUMN_COUNT, DEFAULT_ROW_COUNT
 
 
 class Document:
     def __init__(self, filename=None):
         self._model = _NumbersModel(filename)
         refs = self._model.sheet_ids()
         self._sheets = ItemsList(self._model, refs, Sheet)
 
     @property
-    def sheets(self):
+    def sheets(self) -> list:
+        """Return a list of all sheets in the document"""
         return self._sheets
 
+    @property
+    def styles(self) -> list:
+        """Return a list of styles available in the document"""
+        return self._model.styles
+
     def save(self, filename):
         for sheet in self.sheets:
             for table in sheet.tables:
                 self._model.recalculate_table_data(table._table_id, table._data)
         write_numbers_file(filename, self._model.file_store)
 
     def add_sheet(
@@ -71,14 +78,27 @@
                 ),
             )
         )
         self._sheets.append(new_sheet)
 
         return new_sheet
 
+    def add_style(self, **kwargs) -> Style:
+        """Add a new style to the current document. If no style name is
+        provided, the next available numbered style will be generated"""
+        if "name" in kwargs and kwargs["name"] is not None:
+            if kwargs["name"] in self._model.styles.keys():
+                raise IndexError(f"style '{kwargs['name']}' already exists")
+        style = Style(**kwargs)
+        if style.name is None:
+            style.name = self._model.custom_style_name(self._model.styles.keys())
+        style._update_styles = True
+        self._model.styles[style.name] = style
+        return style
+
 
 class Sheet:
     def __init__(self, model, sheet_id):
         self._sheet_id = sheet_id
         self._model = model
         refs = self._model.table_ids(self._sheet_id)
         self._tables = ItemsList(self._model, refs, Table)
@@ -342,15 +362,17 @@
         rows = self.rows()
         for col_num in range(min_col, max_col + 1):
             if values_only:
                 yield tuple(row[col_num].value for row in rows[min_row : max_row + 1])
             else:
                 yield tuple(row[col_num] for row in rows[min_row : max_row + 1])
 
-    def write(self, *args):
+    def _validate_cell_coords(self, *args):
+        """Check first arguments are value cell references and pad
+        the table with empty cells if outside current bounds"""
         if type(args[0]) == str:
             (row_num, col_num) = xl_cell_to_rowcol(args[0])
             value = args[1]
         elif len(args) < 2:
             raise IndexError("invalid cell reference " + str(args))
         else:
             (row_num, col_num) = args[0:2]
@@ -363,14 +385,19 @@
 
         for row in range(self.num_rows, row_num + 1):
             self.add_row()
 
         for row in range(self.num_cols, col_num + 1):
             self.add_column()
 
+        return (row_num, col_num, value)
+
+    def write(self, *args, style=None):
+        (row_num, col_num, value) = self._validate_cell_coords(*args)
+
         if type(value) == str:
             self._data[row_num][col_num] = TextCell(row_num, col_num, value)
         elif type(value) == int or type(value) == float:
             self._data[row_num][col_num] = NumberCell(row_num, col_num, value)
         elif type(value) == bool:
             self._data[row_num][col_num] = BoolCell(row_num, col_num, value)
         elif type(value) == builtin_datetime or type(value) == DateTime:
@@ -385,14 +412,28 @@
             )
         self._data[row_num][col_num]._storage = CellStorage(
             self._model, self._table_id, None, row_num, col_num
         )
         self._data[row_num][col_num]._table_id = self._table_id
         self._data[row_num][col_num]._model = self._model
 
+        if style is not None:
+            self.set_cell_style(row_num, col_num, style)
+
+    def set_cell_style(self, *args):
+        (row_num, col_num, style) = self._validate_cell_coords(*args)
+        if isinstance(style, Style):
+            self._data[row_num][col_num]._style = style
+        elif isinstance(style, str):
+            if style not in self._model.styles:
+                raise IndexError(f"style '{style}' does not exist")
+            self._data[row_num][col_num]._style = self._model.styles[style]
+        else:
+            raise TypeError("style must be a Style object or style name")
+
     def add_row(self, num_rows=1):
         row = [
             EmptyCell(self.num_rows - 1, col_num) for col_num in range(self.num_cols)
         ]
         for _ in range(num_rows):
             self._data.append(row.copy())
             self.num_rows += 1
```

### Comparing `numbers_parser-4.0.0/src/numbers_parser/exceptions.py` & `numbers_parser-4.1.0/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/file.py` & `numbers_parser-4.1.0/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/formula.py` & `numbers_parser-4.1.0/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/fontmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FONT_NAME_MAP = {
+FONT_NAME_TO_FAMILY = {
     "AcademyEngravedLetPlain": "Academy Engraved LET",
     "AlBayan": "Al Bayan",
     "AlBayan-Bold": "Al Bayan",
     "AlNile": "Al Nile",
     "AlNile-Bold": "Al Nile",
     "AlTarikh": "Al Tarikh",
     "AmericanTypewriter": "American Typewriter",
```

### Comparing `numbers_parser-4.0.0/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.1.0/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/iwafile.py` & `numbers_parser-4.1.0/src/numbers_parser/iwafile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Forked from https://github.com/psobot/keynote-parser/blob/master/keynote_parser/codec.py
 
 import logging
 import struct
 import snappy
+from typing import List
 
 from functools import partial
 from struct import unpack
 
 from numbers_parser.mapping import ID_NAME_MAP, NAME_CLASS_MAP, NAME_ID_MAP
 from numbers_parser.exceptions import NotImplementedError
 from numbers_parser.generated.TSPArchiveMessages_pb2 import ArchiveInfo
@@ -336,7 +337,21 @@
         if first_byte != 0x00:
             return False
 
         segment_length = unpack("<I", bytes(header[1:]) + b"\x00")[0]
         length += segment_length + 4
         data = data[4 + segment_length :]
     return length == data_length
+
+
+def extensions(obj) -> List[object]:
+    return [
+        obj.Extensions[field] for field, _ in obj.ListFields() if field.is_extension
+    ]
+
+
+def find_extension(obj, name: str) -> object:
+    all_extensions = extensions(obj)
+    filtered = [
+        getattr(x, name) for x in all_extensions if getattr(x, name, None) is not None
+    ]
+    return filtered[0]
```

### Comparing `numbers_parser-4.0.0/src/numbers_parser/mapping.py` & `numbers_parser-4.1.0/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/src/numbers_parser/model.py` & `numbers_parser-4.1.0/src/numbers_parser/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,65 +4,78 @@
 from array import array
 from functools import lru_cache
 from struct import pack
 from typing import Dict, List, Tuple, Union
 from warnings import warn
 
 from numbers_parser.containers import ObjectStore
+from numbers_parser.iwafile import find_extension
 from numbers_parser.constants import (
     EPOCH,
     DEFAULT_COLUMN_WIDTH,
     DEFAULT_DOCUMENT,
     DEFAULT_PRE_BNC_BYTES,
     DEFAULT_ROW_HEIGHT,
     DEFAULT_TABLE_OFFSET,
     DEFAULT_TILE_SIZE,
     DOCUMENT_ID,
     PACKAGE_ID,
     MAX_TILE_SIZE,
-    Alignment,
-    HorizontalJustification,
-    VerticalJustification,
-    RGB,
 )
 from numbers_parser.cell import (
     xl_rowcol_to_cell,
     xl_col_to_name,
     BoolCell,
     DateCell,
     DurationCell,
     EmptyCell,
     MergedCell,
     NumberCell,
     TextCell,
     Style,
+    Alignment,
+    HorizontalJustification,
+    VerticalJustification,
+    RGB,
 )
 from numbers_parser.exceptions import UnsupportedError, UnsupportedWarning
 from numbers_parser.formula import TableFormulas
 from numbers_parser.bullets import (
     BULLET_PREFIXES,
     BULLET_CONVERTION,
     BULLET_SUFFIXES,
 )
 from numbers_parser.cell_storage import CellStorage
 from numbers_parser.numbers_uuid import NumbersUUID
 
-from numbers_parser.generated.fontmap import FONT_NAME_MAP
+from numbers_parser.generated.fontmap import FONT_NAME_TO_FAMILY
 from numbers_parser.generated import TNArchives_pb2 as TNArchives
 from numbers_parser.generated import TSDArchives_pb2 as TSDArchives
 from numbers_parser.generated import TSPMessages_pb2 as TSPMessages
 from numbers_parser.generated import TSPArchiveMessages_pb2 as TSPArchiveMessages
 from numbers_parser.generated import TSTArchives_pb2 as TSTArchives
 from numbers_parser.generated import TSCEArchives_pb2 as TSCEArchives
 from numbers_parser.generated import TSWPArchives_pb2 as TSWPArchives
+from numbers_parser.generated import TSSArchives_pb2 as TSSArchives
 from numbers_parser.generated.TSWPArchives_pb2 import (
     CharacterStylePropertiesArchive as CharacterStyle,
 )
 
 
+def create_font_name_map(font_map: dict) -> dict:
+    new_font_map = {}
+    for k, v in font_map.items():
+        if v not in new_font_map:
+            new_font_map[v] = k
+    return new_font_map
+
+
+FONT_FAMILY_TO_NAME = create_font_name_map(FONT_NAME_TO_FAMILY)
+
+
 class DataLists:
     """Model for TST.DataList with caching and key generation for new values"""
 
     def __init__(self, model: object, datalist_name: str, value_attr: str = None):
         self._model = model
         self._datalists = {}
         self._value_attr = value_attr
@@ -649,22 +662,27 @@
         row_info.cell_offsets_pre_bnc = DEFAULT_PRE_BNC_BYTES
         row_info.cell_storage_buffer = cell_storage
         row_info.cell_storage_buffer_pre_bnc = DEFAULT_PRE_BNC_BYTES
         row_info.has_wide_offsets = True
         return row_info
 
     @lru_cache(maxsize=None)
-    def metadata_component(self, component_name: str) -> int:
-        """Return the ID of an object in the document metadata given it's name"""
+    def metadata_component(self, reference: Union[str, int] = None) -> int:
+        """Return the ID of an object in the document metadata given it's name or ID"""
         component_map = {c.identifier: c for c in self.objects[PACKAGE_ID].components}
-        component_ids = [
-            id
-            for id, c in component_map.items()
-            if c.preferred_locator == component_name
-        ]
+        if isinstance(reference, str):
+            component_ids = [
+                id
+                for id, c in component_map.items()
+                if c.preferred_locator == reference
+            ]
+        else:
+            component_ids = [
+                id for id, c in component_map.items() if c.identifier == reference
+            ]
         return component_map[component_ids[0]]
 
     def add_component_metadata(self, object_id: int, parent: str, locator: str):
         """Add a new ComponentInfo record to the parent object in the document metadata"""
         locator = locator.format(object_id)
         preferred_locator = re.sub(r"\-\d+.*", "", locator)
         component_info = TSPArchiveMessages.ComponentInfo(
@@ -678,20 +696,20 @@
         )
         self.objects[PACKAGE_ID].components.append(component_info)
         self.add_component_reference(object_id, parent)
 
     def add_component_reference(
         self,
         object_id: int,
-        location: str,
+        location: str = None,
         parent_id: int = None,
         is_weak: bool = False,
     ):
         """Add an external reference to an object in a metadata component"""
-        component = self.metadata_component(location)
+        component = self.metadata_component(location or parent_id)
         if parent_id is not None:
             params = {"object_identifier": object_id, "component_identifier": parent_id}
         else:
             params = {"component_identifier": object_id}
         if is_weak:
             params["is_weak"] = True
         component.external_references.append(
@@ -703,14 +721,16 @@
         table_model.number_of_rows = len(data)
         table_model.number_of_columns = len(data[0])
 
         self.init_table_strings(table_id)
         self.recalculate_row_headers(table_id, data)
         self.recalculate_column_headers(table_id, data)
         self.recalculate_merged_cells(table_id)
+        self.update_paragraph_styles()
+        self.update_cell_styles(table_id, data)
 
         table_model.ClearField("base_column_row_uids")
 
         tile_idx = 0
         max_tile_idx = len(data) >> 8
         base_data_store = self.objects[table_id].base_data_store
         base_data_store.tiles.ClearField("tiles")
@@ -1126,146 +1146,287 @@
 
         self.objects[DOCUMENT_ID].sheets.append(
             TSPMessages.Reference(identifier=sheet_id)
         )
 
         return sheet_id
 
-    def add_cell_style(self, table_id: int, style: Style) -> int:
-        table_model = self.objects[table_id]
-        cell_style_id, cell_style = self.objects.create_object_from_dict(
-            # TODO: lookup a new style name
+    @property
+    def styles(self):
+        return self.available_paragraph_styles()
+
+    @lru_cache(maxsize=None)
+    def available_paragraph_styles(self) -> List[Style]:
+        theme_id = self.objects[DOCUMENT_ID].theme.identifier
+        presets = find_extension(
+            self.objects[theme_id].super, "paragraph_style_presets"
+        )
+        presets_map = {
+            self.objects[x.identifier].super.name: {
+                "id": x.identifier,
+                "obj": self.objects[x.identifier],
+            }
+            for x in presets
+        }
+        return {
+            k: Style(
+                font_color=self.cell_font_color(v["obj"]),
+                font_size=self.cell_font_size(v["obj"]),
+                font_name=self.cell_font_name(v["obj"]),
+                bold=self.cell_is_bold(v["obj"]),
+                italic=self.cell_is_italic(v["obj"]),
+                underline=self.cell_is_underline(v["obj"]),
+                strikethrough=self.cell_is_strikethrough(v["obj"]),
+                name=self.cell_style_name(v["obj"]),
+                _text_style_id=v["id"],
+            )
+            for k, v in presets_map.items()
+        }
+
+    def add_paragraph_style(self, style: Style) -> int:
+        if style.underline:
+            underline = CharacterStyle.UnderlineType.kSingleUnderline
+        else:
+            underline = CharacterStyle.UnderlineType.kNoUnderline
+        if style.strikethrough:
+            strikethru = CharacterStyle.StrikethruType.kSingleStrikethru
+        else:
+            strikethru = CharacterStyle.StrikethruType.kNoStrikethru
+
+        style_id_name = "numbers-parser-" + style.name.lower().replace(" ", "-")
+        para_style_id, para_style = self.objects.create_object_from_dict(
             "DocumentStylesheet",
             {
                 "super": {
-                    "name": "Custom Style 99",
-                    "style_identifier": "text-98-paragraphstyle-Custom Style 98",
+                    "name": style.name,
+                    "style_identifier": style_id_name,
                 },
                 "override_count": 1,
-                "cell_properties": {
-                    "cell_fill": {
+                "char_properties": {
+                    "font_color": {
+                        "model": "rgb",
+                        "r": style.font_color.r / 255,
+                        "g": style.font_color.g / 255,
+                        "b": style.font_color.b / 255,
+                        "a": 1.0,
+                        "rgbspace": "srgb",
+                    },
+                    "bold": style.bold,
+                    "italic": style.italic,
+                    "underline": underline,
+                    "strikethru": strikethru,
+                    "font_size": style.font_size,
+                    "font_name": FONT_FAMILY_TO_NAME[style.font_name],
+                    "tsd_fill": {
                         "color": {
                             "model": "rgb",
-                            "r": style._bg_color.r / 255,
-                            "g": style._bg_color.g / 255,
-                            "b": style._bg_color.b / 255,
+                            "r": style.font_color.r / 255,
+                            "g": style.font_color.g / 255,
+                            "b": style.font_color.b / 255,
                             "a": 1.0,
                             "rgbspace": "srgb",
-                        }
+                        },
                     },
-                    "vertical_alignment": style.alignment.vertical,
+                },
+                "para_properties": {
+                    "alignment": style.alignment.horizontal,
                 },
             },
-            TSTArchives.CellStyleArchive,
-        )
-        cell_style.super.parent.MergeFrom(
-            TSPMessages.Reference(identifier=table_model.body_text_style.identifier)
+            TSWPArchives.ParagraphStyleArchive,
         )
         stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
-        cell_style.super.stylesheet.MergeFrom(
+        para_style.super.stylesheet.MergeFrom(
             TSPMessages.Reference(identifier=stylesheet_id)
         )
         self.objects[stylesheet_id].styles.append(
-            TSPMessages.Reference(identifier=cell_style_id)
+            TSPMessages.Reference(identifier=para_style_id)
         )
-        return cell_style_id
+        self.objects[stylesheet_id].identifier_to_style_map.append(
+            TSSArchives.StylesheetArchive.IdentifiedStyleEntry(
+                identifier=style_id_name,
+                style=TSPMessages.Reference(identifier=para_style_id),
+            )
+        )
+        # TODO: add style to theme
+        return para_style_id
 
-    def add_text_style(self, table_id: int, style: Style) -> int:
-        table_model = self.objects[table_id]
-        if style._is_underline:
+    def update_paragraph_style(self, style: Style):
+        if style.underline:
             underline = CharacterStyle.UnderlineType.kSingleUnderline
         else:
             underline = CharacterStyle.UnderlineType.kNoUnderline
-        if style._is_strikethrough:
+        if style.strikethrough:
             strikethru = CharacterStyle.StrikethruType.kSingleStrikethru
         else:
             strikethru = CharacterStyle.StrikethruType.kNoStrikethru
-        text_style_id, text_style = self.objects.create_object_from_dict(
+        style_obj = self.objects[style._text_style_id]
+        style_obj.char_properties.font_color.r = style.font_color.r / 255
+        style_obj.char_properties.font_color.g = style.font_color.g / 255
+        style_obj.char_properties.font_color.b = style.font_color.b / 255
+        style_obj.char_properties.bold = style.bold
+        style_obj.char_properties.italic = style.italic
+        style_obj.char_properties.underline = underline
+        style_obj.char_properties.strikethru = strikethru
+        style_obj.char_properties.font_size = style.font_size
+        style_obj.char_properties.font_name = FONT_FAMILY_TO_NAME[style.font_name]
+        style_obj.char_properties.tsd_fill.color.r = style.font_color.r / 255
+        style_obj.char_properties.tsd_fill.color.g = style.font_color.g / 255
+        style_obj.char_properties.tsd_fill.color.b = style.font_color.b / 255
+        style_obj.para_properties.alignment = style.alignment.horizontal
+
+    def update_paragraph_styles(self):
+        """Create new paragraph style archives for any new styles that
+        have been created for this document"""
+        new_styles = [x for x in self.styles.values() if x._text_style_id is None]
+        updated_styles = [
+            x
+            for x in self.styles.values()
+            if x._text_style_id is not None and x._update_text_style
+        ]
+        for style in new_styles:
+            style._text_style_id = self.add_paragraph_style(style)
+            style._update_text_style = True
+
+        for style in updated_styles:
+            self.update_paragraph_style(style)
+
+    def update_cell_styles(self, table_id: int, data: List):
+        """Create new cell style archives for any cells whose styles
+        have changes that require a cell style"""
+        cell_styles = {}
+        for row_num, row in enumerate(data):
+            for col_num, cell in enumerate(row):
+                if cell._style is not None and cell._style._update_cell_style:
+                    if cell._style.bg_color is None:
+                        fingerprint = str(cell.style.alignment.vertical)
+                    else:
+                        fingerprint = "{0}-{1}-{2}-{3}".format(
+                            cell.style.alignment.vertical,
+                            cell.style.bg_color.r,
+                            cell.style.bg_color.g,
+                            cell.style.bg_color.b,
+                        )
+                    if fingerprint not in cell_styles:
+                        cell_styles[fingerprint] = self.add_cell_style(cell._style)
+                    cell._style._cell_style_id = cell_styles[fingerprint]
+
+    def add_cell_style(self, style: Style) -> int:
+        if style.bg_color is not None:
+            color_attrs = {
+                "cell_fill": {
+                    "color": {
+                        "model": "rgb",
+                        "r": style.bg_color.r / 255,
+                        "g": style.bg_color.g / 255,
+                        "b": style.bg_color.b / 255,
+                        "a": 1.0,
+                        "rgbspace": "srgb",
+                    }
+                }
+            }
+        else:
+            color_attrs = {}
+        style_id_name = f"numbers-parser-custom-{style._cell_style_id}"
+        cell_style_id, cell_style = self.objects.create_object_from_dict(
             "DocumentStylesheet",
             {
                 "super": {
-                    "name": "Custom Style 99",
-                    "style_identifier": "text-99-paragraphstyle-Custom Style 99",
+                    "name": style.name,
+                    "style_identifier": style_id_name,
                 },
                 "override_count": 1,
-                "char_properties": {
-                    "font_color": {
-                        "model": "rgb",
-                        "r": style._font_color.r / 255,
-                        "g": style._font_color.g / 255,
-                        "b": style._font_color.b / 255,
-                        "a": 1.0,
-                        "rgbspace": "srgb",
-                    },
-                    "bold": style._is_bold,
-                    "italic": style._is_italic,
-                    "underline": underline,
-                    "strikethru": strikethru,
-                    "font_size": style._font_size,
-                    "font_name": style._font_name,
-                },
-                "para_properties": {
-                    "alignment": style.alignment.horizontal,
+                "cell_properties": {
+                    **color_attrs,
+                    "vertical_alignment": style.alignment.vertical,
                 },
             },
-            TSWPArchives.ParagraphStyleArchive,
-        )
-        text_style.super.parent.MergeFrom(
-            TSPMessages.Reference(identifier=table_model.body_text_style.identifier)
+            TSTArchives.CellStyleArchive,
         )
         stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
-        text_style.super.stylesheet.MergeFrom(
+        cell_style.super.stylesheet.MergeFrom(
             TSPMessages.Reference(identifier=stylesheet_id)
         )
         self.objects[stylesheet_id].styles.append(
-            TSPMessages.Reference(identifier=text_style_id)
+            TSPMessages.Reference(identifier=cell_style_id)
+        )
+        self.objects[stylesheet_id].identifier_to_style_map.append(
+            TSSArchives.StylesheetArchive.IdentifiedStyleEntry(
+                identifier=style_id_name,
+                style=TSPMessages.Reference(identifier=cell_style_id),
+            )
+        )
+        return cell_style_id
+
+    def text_style_object_id(self, cell_storage) -> int:
+        if cell_storage.text_style_id is None:
+            return None
+        entry = self._table_styles.lookup_value(
+            cell_storage.table_id, cell_storage.text_style_id
+        )
+        return entry.reference.identifier
+
+    def cell_style_object_id(self, cell_storage) -> int:
+        if cell_storage.cell_style_id is None:
+            return None
+        entry = self._table_styles.lookup_value(
+            cell_storage.table_id, cell_storage.cell_style_id
         )
-        return text_style_id
+        return entry.reference.identifier
+
+    def custom_style_name(self, current_styles: List[str]) -> Tuple[str, str]:
+        """Find custom styles in the current document and return the next
+        highest numbered style"""
+        stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
+        custom_styles = [
+            x for x in current_styles if re.fullmatch(r"Custom Style \d+", x)
+        ]
+        for style_entry in self.objects[stylesheet_id].identifier_to_style_map:
+            style_id = style_entry.style.identifier
+            style_name = getattr(self.objects[style_id].super, "name", "")
+            if re.fullmatch(r"Custom Style \d+", style_name):
+                custom_styles.append(style_name)
+
+        if len(custom_styles) > 0:
+            offset = len("Custom Style ")
+            custom_style_ids = [int(x[offset:]) for x in custom_styles]
+            return "Custom Style " + str(custom_style_ids[-1] + 1)
+        else:
+            return "Custom Style 1"
 
     def pack_cell_storage(  # noqa: C901
         self,
         table_id: int,
         data: List,
         row_num: int,
         col_num: int,
         formula_id=None,
         num_format_id=None,
     ) -> bytearray:
         """Create a storage buffer for a cell using v5 (modern) layout"""
         cell = data[row_num][col_num]
-        if cell._style is not None and cell._style._cell_style_updated:
-            if cell._storage.cell_style_id is None:
-                cell_style_id = self.add_cell_style(cell._table_id, cell._style)
-                cell._storage.cell_style_id = self._table_styles.lookup_key(
+        if cell._style is not None:
+            if cell.style._text_style_id is not None:
+                cell._storage.text_style_id = self._table_styles.lookup_key(
                     cell._table_id,
-                    TSPMessages.Reference(identifier=cell_style_id),
+                    TSPMessages.Reference(identifier=cell.style._text_style_id),
                 )
                 self.add_component_reference(
-                    cell_style_id,
-                    "DocumentStylesheet",
-                    self.objects[DOCUMENT_ID].stylesheet.identifier,
+                    cell.style._text_style_id,
+                    parent_id=self._table_styles.id(cell._table_id),
                 )
-            else:
-                # TODO: update existing styles
-                pass
-        if cell._style is not None and cell._style._text_style_updated:
-            if cell._storage.text_style_id is None:
-                text_style_id = self.add_text_style(cell._table_id, cell._style)
-                cell._storage.text_style_id = self._table_styles.lookup_key(
+
+            if cell.style._cell_style_id is not None:
+                cell._storage.cell_style_id = self._table_styles.lookup_key(
                     cell._table_id,
-                    TSPMessages.Reference(identifier=text_style_id),
+                    TSPMessages.Reference(identifier=cell.style._cell_style_id),
                 )
                 self.add_component_reference(
-                    text_style_id,
-                    "DocumentStylesheet",
-                    self.objects[DOCUMENT_ID].stylesheet.identifier,
+                    cell.style._cell_style_id,
+                    parent_id=self._table_styles.id(cell._table_id),
                 )
-            else:
-                # TODO: update existing styles
-                pass
 
         length = 12
         if isinstance(cell, NumberCell):
             flags = 1
             length += 16
             cell_type = TSTArchives.numberCellType
             value = pack_decimal128(cell.value)
@@ -1287,17 +1448,15 @@
             value = pack("<d", float(cell.value))
         elif isinstance(cell, DurationCell):
             flags = 2
             length += 8
             cell_type = TSTArchives.durationCellType
             value = value = pack("<d", float(cell.value.total_seconds()))
         elif isinstance(cell, EmptyCell):
-            if cell._style is not None and (
-                cell._style._cell_style_updated or cell._style._text_style_updated
-            ):
+            if cell._style is not None:
                 flags = 0
                 cell_type = TSTArchives.emptyCellValueType
                 value = b""
             else:
                 return None
         elif isinstance(cell, MergedCell):
             return None
@@ -1450,114 +1609,107 @@
                     "bullets": bullets,
                     "bullet_chars": bullet_chars,
                     "hyperlinks": hyperlinks,
                 }
 
         return None
 
-    def table_paragraph_style(self, cell_storage: object) -> object:
-        style = self.table_style(cell_storage.table_id, cell_storage.text_style_id)
-        if isinstance(style, TSWPArchives.ParagraphStyleArchive):
-            return style
+    def cell_text_style(self, cell_storage: object) -> object:
+        """Return the text style object for the cell or, if none
+        is defined, the default header, footer or body style"""
+        if cell_storage.text_style_id is not None:
+            style = self.table_style(cell_storage.table_id, cell_storage.text_style_id)
+            if isinstance(style, TSWPArchives.ParagraphStyleArchive):
+                return style
 
         table_model = self.objects[cell_storage.table_id]
         if cell_storage.row_num in range(0, table_model.number_of_header_rows):
-            return self.objects[table_model.header_row_text_style.identfier]
+            return self.objects[table_model.header_row_text_style.identifier]
         elif cell_storage.col_num in range(0, table_model.number_of_header_columns):
             return self.objects[table_model.header_column_text_style.identifier]
         elif table_model.number_of_footer_rows > 0:
             start_row_num = (
                 table_model.number_of_rows - table_model.number_of_footer_rows
             )
             if cell_storage.row_num in range(
                 start_row_num, table_model.number_of_header_rows
             ):
                 return self.objects[table_model.footer_row_text_style.identifier]
         return self.objects[table_model.body_text_style.identifier]
 
     def cell_alignment(self, cell_storage: object) -> Alignment:
-        if cell_storage.text_style_id is None:
-            horizontal = HorizontalJustification.LEFT
-        else:
-            cell_style = self.table_paragraph_style(cell_storage)
-            horizontal = HorizontalJustification(cell_style.para_properties.alignment)
+        cell_style = self.cell_text_style(cell_storage)
+        horizontal = HorizontalJustification(cell_style.para_properties.alignment)
 
         if cell_storage.cell_style_id is None:
             vertical = VerticalJustification.TOP
         else:
             cell_style = self.table_style(
                 cell_storage.table_id, cell_storage.cell_style_id
             )
             vertical = VerticalJustification(
                 cell_style.cell_properties.vertical_alignment
             )
         return Alignment(horizontal, vertical)
 
     def cell_bg_color(self, cell_storage: object) -> Union[Tuple, List[Tuple]]:
         if cell_storage.cell_style_id is None:
-            return RGB(0, 0, 0)
+            return None
 
         cell_style = self.table_style(cell_storage.table_id, cell_storage.cell_style_id)
         cell_properties = cell_style.cell_properties.cell_fill
 
         if cell_properties.HasField("color"):
             return rgb(cell_properties.color)
         elif cell_properties.HasField("gradient"):
             return [(rgb(s.color)) for s in cell_properties.gradient.stops]
 
-    def cell_text_style(self, cell_storage: object) -> object:
-        if cell_storage.text_style_id is None:
-            table_model = self.objects[cell_storage.table_id]
-            return self.objects[table_model.body_text_style.identifier]
-        else:
-            return self.table_paragraph_style(cell_storage)
-
     def char_property(self, style: object, field: str):
         """Return a char_property field from a style if present
         in the style, or from the parent if not"""
         if not style.char_properties.HasField(field):
             parent = self.objects[style.super.parent.identifier]
             return getattr(parent.char_properties, field)
         else:
             return getattr(style.char_properties, field)
 
-    def cell_is_bold(self, cell_storage: object) -> bool:
-        style = self.cell_text_style(cell_storage)
+    def cell_is_bold(self, obj: object) -> bool:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return self.char_property(style, "bold")
 
-    def cell_is_italic(self, cell_storage: object) -> bool:
-        style = self.cell_text_style(cell_storage)
+    def cell_is_italic(self, obj: object) -> bool:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return self.char_property(style, "bold")
 
-    def cell_is_underline(self, cell_storage: object) -> bool:
-        style = self.cell_text_style(cell_storage)
+    def cell_is_underline(self, obj: object) -> bool:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         underline = self.char_property(style, "underline")
         return underline != CharacterStyle.UnderlineType.kNoUnderline
 
-    def cell_is_strikethrough(self, cell_storage: object) -> bool:
-        style = self.cell_text_style(cell_storage)
+    def cell_is_strikethrough(self, obj: object) -> bool:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         strikethru = self.char_property(style, "strikethru")
         return strikethru != CharacterStyle.StrikethruType.kNoStrikethru
 
-    def cell_style_name(self, cell_storage: object) -> bool:
-        style = self.cell_text_style(cell_storage)
+    def cell_style_name(self, obj: object) -> bool:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return style.super.name
 
-    def cell_font_color(self, cell_storage: object) -> Tuple:
-        style = self.cell_text_style(cell_storage)
+    def cell_font_color(self, obj: object) -> Tuple:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return rgb(self.char_property(style, "font_color"))
 
-    def cell_font_size(self, cell_storage: object) -> float:
-        style = self.cell_text_style(cell_storage)
+    def cell_font_size(self, obj: object) -> float:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return self.char_property(style, "font_size")
 
-    def cell_font_name(self, cell_storage: object) -> str:
-        style = self.cell_text_style(cell_storage)
+    def cell_font_name(self, obj: object) -> str:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         font_name = self.char_property(style, "font_name")
-        return FONT_NAME_MAP[font_name]
+        return FONT_NAME_TO_FAMILY[font_name]
 
 
 def rgb(obj) -> RGB:
     """Convert a TSPArchives.Color into an RGB tuple"""
     return RGB(round(obj.r * 255), round(obj.g * 255), round(obj.b * 255))
```

### Comparing `numbers_parser-4.0.0/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.1.0/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.0.0/PKG-INFO` & `numbers_parser-4.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: numbers-parser
-Version: 4.0.0
-Summary: Read and write Apple Numbers spreadsheets
-Home-page: https://github.com/masaccio/numbers-parser
-License: MIT
-Author: Jon Connell
-Author-email: python@figsandfudge.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
-Requires-Dist: compact-json (>=1.1.3,<2.0.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: protobuf (>=4.21.1,<5.0.0)
-Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
-Requires-Dist: regex (>=2022.9.13,<2023.0.0)
-Requires-Dist: roman (>=3.3,<4.0)
-Project-URL: Documentation, https://github.com/masaccio/numbers-parser/blob/main/README.md
-Project-URL: Repository, https://github.com/masaccio/numbers-parser
-Description-Content-Type: text/markdown
-
 # numbers-parser
 
 [![build:](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml)
 [![build:](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml)
 [![codecov](https://codecov.io/gh/masaccio/numbers-parser/branch/main/graph/badge.svg?token=EKIUFGT05E)](https://codecov.io/gh/masaccio/numbers-parser)
 
 `numbers-parser` is a Python module for parsing [Apple Numbers](https://www.apple.com/numbers/)
@@ -38,15 +10,15 @@
 
 It supports and is tested against Python versions from 3.8 onwards. It is not compatible with earlier versions of Python.
 
 Formula evaluation relies on Numbers storing current values which should usually be the case. Formulas themselves rather than the computed values can optionally be extracted. [Style support](#styles) is somewhat limited, but has grown significantly as of version 4.0.
 
 ## API changes in version 4.0
 
-To better partition cell styles, the new cell property `style` contains all style information for a cell including background image data which was supported in earlier versions. Image information is now found in `cell.style.bg_image`. Using the deprecated methods `image_data` and `image_filename` will issue a `DeprecationWarning` if used.The legacy methods will be removed in a future version of numbers-parser.
+To better partition cell styles, background image data which was supported in earlier versions through the methods `image_data` and `image_filename` is now part of the new `cell_style` property. Using the deprecated methods `image_data` and `image_filename` will issue a `DeprecationWarning` if used.The legacy methods will be removed in a future version of numbers-parser.
 
 `NumberCell` cell types return [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html) types rather than `float`. These are created in a [decimal128](https://en.wikipedia.org/wiki/Decimal128_floating-point_format) context to preserve the precision used by Numbers. Previously, using float resulted in rounding errors in unpacking internal numbers.
 
 ## Installation
 
 ``` bash
 python3 -m pip install numbers-parser
@@ -201,37 +173,40 @@
 ``` python
 cell = table.cell(0, 0)
 (text, url) = cell.hyperlinks[0]
 ```
 
 ### Styles
 
-`numbers_parser` has very limited support for cell styles. Currently only cell backgrounds are supported.
-
-#### Cell background colour
-
-The `bg_color` cell property returns either a tuple of RGB values or, in the case of gradient backgrounds, a list of tuples with each colour in the gradient. If no background color is defined, `None` is returned.
-
-``` python
-rgb = table.cell("B1").bg_color
-print("B1 RGB =", rgb[0], rgb[1], rgb[2])
-```
+`numbers_parser` currently only supports paragraph styles and cell styles. The following paragraph styles are suppoprted:
 
-#### Cell text attributes
-
-Cell text fonts can be returned using a number of methods. Formatting changes within cells such as "This is **bold** text" are not supported.
-
-* `cell.style.name`: cell style (`str`)
-* `cell.style.is_bold`: `True` if the cell font is bold
-* `cell.style.is_italic`: `True` if the cell font is italic
-* `cell.style.is_underline`: `True` if the cell font is underline
-* `cell.style.is_strikethrough`: `True` if the cell font is strikethrough
-* `cell.style.font_color`: font color as a tuple of RGB values
-* `cell.style.font_size`: font size in points (`float`)
-* `cell.style.font_name`: font name (`str`)
+* font attributes: bold, italic, underline, strikethrough
+* font selection and size
+* text foreground color
+* horizontal and vertical alignment
+* cell background color
+
+Table styles that allow new tables to adopt a style across the whole table are not planned.
+
+#### Reading styles
+
+The cell method `style` returns a `Style` object containing all the style information for that cell. Cells with identical style settings contain references to a single style object.
+
+Cell text fonts can be returned using a number of methods.
+
+* `Cell.style.alignment`: the horizontal and vertical alignment of the cell as an `Alignment` names tuple
+* `Cell.style.bg_color`: cell background color as an `RGB` named tuple, or a list of `RGB` values for gradients
+* `Cell.style.bold`: `True` if the cell font is bold
+* `Cell.style.font_color`: font color as an `RGB` named tuple
+* `Cell.style.font_size`: font size in points (`float`)
+* `Cell.style.font_name`: font name (`str`)
+* `Cell.style.italic`: `True` if the cell font is italic
+* `Cell.style.name`: cell style (`str`)
+* `Cell.style.underline`: `True` if the cell font is underline
+* `Cell.style.strikethrough`: `True` if the cell font is strikethrough
 
 #### Cell images
 
 The methods `style.bg_image.filename` and `style.bg_image.data` return data about the image used for a cell's background, where set. If a cell has no background image, `style.bg_image`  is `None`.
 
 ``` python
 cell = table.cell("B1")
@@ -241,23 +216,23 @@
 
 ## Writing Numbers files
 
 Whilst support for writing numbers files has been stable since version 3.4.0, you are highly recommened not to overwrite working Numbers files and instead save data to a new file.
 
 ### Limitations
 
-Since version 3.4.0, adding tables and sheets is supported. Known limitations to write support are:
+Current limitations to write support are:
 
 * Creating cells of type `BulletedTextCell` is not supported
 * Formats cannot be defined for `DurationCell` or `DateCell`
 * New tables are inserted with a fixed offset below the last table in a worksheet which does not take into account title or caption size
 * New sheets insert tables with formats copied from the first table in the previous sheet rather than default table formats
-* Style cannot be saved.
+* Style editing is limited to paragraph styles.
 
-### Editing cells
+### Cell values
 
 `numbers-parser` will automatically empty rows and columns for any cell references that are out of range of the current table. The `write` method accepts the same cell numbering notation as `cell` plus an additional argument representing the new cell value. The type of the new value will be used to determine the cell type.
 
 ``` python
 doc = Document("old-sheet.numbers")
 sheets = doc.sheets
 tables = sheets[0].tables
@@ -286,19 +261,19 @@
 table.write(1, 1, 1000)
 table.write(1, 2, 2000)
 table.write(1, 3, 3000)
 
 doc.save("sheet.numbers")
 ```
 
-## Table geometries
+### Table geometries
 
 `numbers-parser` can query and change the position and size of tables. Changes made to a table's row height or column width is retained when files are saved.
 
-###  Row and column sizes
+####  Row and column sizes
 
 Row heights and column widths are queried and set using the `row_height` and `col_width` methods:
 
 ```python
 doc = Document("sheet.numbers")
 table = doc.sheets[0].tables[0]
 print(f"Table size is {table.height} x {table.width}")
@@ -306,38 +281,70 @@
 table.row_height(0, 40)
 print(f"Table row 1 height is now {table.row_height(0)}")
 print(f"Table column A width is {table.col_width(0)}")
 table.col_width(0, 200)
 print(f"Table column A width is {table.col_width(0)}")
 ```
 
-###  Header row and columns
+####  Header row and columns
 
 When new tables are created, `numbers-parser` follows the Numbers convention of creating a table with one row header and one column header. You can change the number of headers by modifying the appopriate property:
 
 ```python
 doc = Document("sheet.numbers")
 table = doc.sheets[0].tables[0]
 table.num_header_rows = 2
 table.num_header_cols = 0
 doc.save("saved.numbers")
 ```
 
 A zero header count will remove the headers from the table. Attempting to set a negative number of headers, or using more headers that rows or columns in the table will raise a `ValueError` exception.
 
-### Positioning tables
+#### Positioning tables
 
 By default, new tables are positioned at a fixed offset below the last table vertically in a sheet and on the left side of the sheet. Large table headers and captions may result in new tables overlapping existing ones. The `add_table` method takes optional coordinates for positioning a table. A table's height and coordinates can also be queried to help aligning new tables:
 
 ```python
 (x, y) = sheet.table[0].coordinates
 y += sheet.table[0].height + 200.0
 new_table = sheet.add_table("Offset Table", x, y)
 ```
 
+### Editing paragraph styles
+
+Cell text styles, known as paragraph styles, are those applied by the Text tab in Numbers Format pane. To simplify the API, when writing documents, it is not possible to make ad hoc changes to cells without assigning an existing style or creating a new one. This differs to the Numbers interface where cells can have modified styles on a per cell basis. Such styles are read correctly when reading Numbers files.
+
+Character styles, which allow formatting changes within cells such as "This is **bold** text" are not supported.
+
+Styles are created using the `Document`'s `add_style` method, and can be applied to cells either as part of a `write` or using `set_cell_style`:
+
+``` python
+red_text = doc.add_style(
+    name="Red Text",
+    font_name="Lucida Grande",
+    font_color=RGB(230, 25, 25),
+    font_size=14.0,
+    bold=True,
+    italic=True,
+    alignment=Alignment("right", "top"),
+)
+table.write("B2", "Red", style=red_text)
+table.set_cell_style("C2", red_text)
+```
+
+Cell styles can also be referred to by name in both `Table.write` and `Table.set_cell_style`. A `dict` of available styles is returned by `Document.styles`. This contains key value pairs of style names and `Style` objects. Any changes to `Style` objects in the document are written back such that those styles are changed for all cells that use them.
+
+``` python
+doc = Document("styles.numbers")
+styles = doc.styles
+styles["Title"].font_size = 20.0
+```
+
+Since `Style` objects are shared, changing `Cell.style.font_size` will have the effect of changing the font size for that style and will in turn affect the styles of all cells using that style.
+
 ## Command-line scripts
 
 When installed from [PyPI](https://pypi.org/project/numbers-parser/), a command-like script `cat-numbers` is installed in Python's scripts folder. This script dumps Numbers spreadsheets into Excel-compatible CSV format, iterating through all the spreadsheets passed on the command-line.
 
 ``` text
 usage: cat-numbers [-h] [-T | -S | -b] [-V] [--debug] [--formulas]
                    [--formatting] [-s SHEET] [-t TABLE] [document ...]
@@ -405,8 +412,7 @@
 
 Decimal128 conversion to and from byte storage was adapted from work done by the
 [SheetsJS project](https://github.com/SheetJS/sheetjs). SheetJS also helped greatly with some of the steps required to successfully save a Numbers spreadsheet.
 
 ## License
 
 All code in this repository is licensed under the [MIT License](https://github.com/masaccio/numbers-parser/blob/master/LICENSE.rst)
-
```

