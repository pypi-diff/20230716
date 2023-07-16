# Comparing `tmp/float_table-0.1.0.tar.gz` & `tmp/float_table-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "float_table-0.1.0.tar", max compression
+gzip compressed data, was "float_table-0.1.1.tar", max compression
```

## Comparing `float_table-0.1.0.tar` & `float_table-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        4 2023-07-16 18:29:37.605123 float_table-0.1.0/README.md
--rw-r--r--   0        0        0      111 2023-07-16 16:20:05.485577 float_table-0.1.0/float_table/__init__.py
--rw-r--r--   0        0        0     2615 2023-07-16 18:26:40.631012 float_table-0.1.0/float_table/fmt.py
--rw-r--r--   0        0        0      833 2023-07-16 18:28:56.819225 float_table-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1955 2023-07-16 18:26:40.634724 float_table-0.1.0/tests/test.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 float_table-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.1/README.md
+-rw-r--r--   0        0        0      111 2023-07-16 16:20:05.485577 float_table-0.1.1/float_table/__init__.py
+-rw-r--r--   0        0        0     2615 2023-07-16 19:15:13.862085 float_table-0.1.1/float_table/fmt.py
+-rw-r--r--   0        0        0      833 2023-07-16 19:42:42.165695 float_table-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2320 2023-07-16 19:42:06.993525 float_table-0.1.1/tests/test.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 float_table-0.1.1/PKG-INFO
```

### Comparing `float_table-0.1.0/float_table/fmt.py` & `float_table-0.1.1/float_table/fmt.py`

 * *Files identical despite different names*

### Comparing `float_table-0.1.0/pyproject.toml` & `float_table-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool]
 [tool.poetry]
 name = "float-table"
-version = "0.1.0"
-homepage = "https://github.com/tadamcz/float_table"
+version = "0.1.1"
+homepage = "https://github.com/tadamcz/float-table"
 description = "Top-level package for float-table."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
 ]
```

### Comparing `float_table-0.1.0/tests/test.py` & `float_table-0.1.1/tests/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import numpy as np
 import pandas as pd
 import pytest
-import sigfig
 
 from float_table.fmt import pad_decimal, determine_eng_exponent, format_column
 
 
 @pytest.fixture(params=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9], ids=lambda x: f"seed={x}")
 def num_column(request):
-    n = 3
+    n = 1000
     np.random.seed(request.param)
 
     def base_floats():
         # Generate floats spanning 12 orders of magnitude
         return np.random.rand(n) * 10.0 ** np.random.randint(-6, 6, n)
 
     positive_floats = base_floats()
@@ -51,16 +50,22 @@
 def test_exponent(num_column):
     exponent = determine_eng_exponent(num_column)
     assert exponent % 3 == 0
 
 
 @pytest.mark.parametrize("sig_figs", [1, 4, 8])
 def test_numbers_correct(num_column, sig_figs):
+    # The most obvious way to test this (using Python's 'g' formatter),
+    # fails on edge cases: this is because round() applies "round half to even" whereas
+    # 'g' format applies "round half away from zero".
+    # This is a dumb hack to avoid integers that end in 5
+    num_column = num_column.apply(lambda x: x + 0.0000001)
+
     actual = format_column(num_column, sig_figs)
+    actual = actual.apply(lambda x: float(x.replace(" ", "")))
+
+    g_rounder = "{:." + str(sig_figs) + "g}"
+    expected = num_column.apply(lambda x: float(g_rounder.format(x)))
 
-    # Use the sigfig library to check (our code does not use sigfig)
-    expected = num_column.apply(lambda x: sigfig.round(x, sig_figs, output_type=str))
-    actual = actual.apply(lambda x: x.replace(" ", ""))
-
-    expected = expected.astype(float)
-    actual = actual.astype(float)
-    assert (actual == expected).all()
+    for i in range(len(actual)):
+        msg = f"For '{num_column.iloc[i]}', got '{actual.iloc[i]}', expected '{expected.iloc[i]}'"
+        assert actual.iloc[i] == expected.iloc[i], msg
```

### Comparing `float_table-0.1.0/PKG-INFO` & `float_table-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: float-table
-Version: 0.1.0
+Version: 0.1.1
 Summary: Top-level package for float-table.
-Home-page: https://github.com/tadamcz/float_table
+Home-page: https://github.com/tadamcz/float-table
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

