# Comparing `tmp/float_table-0.1.3.tar.gz` & `tmp/float_table-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "float_table-0.1.3.tar", max compression
+gzip compressed data, was "float_table-0.1.4.tar", max compression
```

## Comparing `float_table-0.1.3.tar` & `float_table-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.3/README.md
--rw-r--r--   0        0        0      165 2023-07-16 20:27:07.444635 float_table-0.1.3/float_table/__init__.py
--rw-r--r--   0        0        0     2868 2023-07-16 20:27:33.264856 float_table-0.1.3/float_table/fmt.py
--rw-r--r--   0        0        0      824 2023-07-16 20:27:39.833965 float_table-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2626 2023-07-16 20:27:33.270808 float_table-0.1.3/tests/test.py
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.4/README.md
+-rw-r--r--   0        0        0      165 2023-07-16 20:27:07.444635 float_table-0.1.4/float_table/__init__.py
+-rw-r--r--   0        0        0     2910 2023-07-16 21:39:45.016397 float_table-0.1.4/float_table/fmt.py
+-rw-r--r--   0        0        0      824 2023-07-16 21:40:10.951129 float_table-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2763 2023-07-16 21:39:25.227350 float_table-0.1.4/tests/test.py
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.4/PKG-INFO
```

### Comparing `float_table-0.1.3/float_table/fmt.py` & `float_table-0.1.4/float_table/fmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 
 def determine_eng_exponent(column):
     """
     Determine the common engineering notation exponent for a numeric column.
     """
     max_abs_val = max(abs(column))
+    if max_abs_val == 0:
+        return 0
     exponent = 3 * math.floor(
         math.log10(max_abs_val) / 3
     )  # Choose the exponent based on the maximum absolute value
     return exponent
 
 
 def find_decimal(x):
```

### Comparing `float_table-0.1.3/pyproject.toml` & `float_table-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "float-table"
-version = "0.1.3"
+version = "0.1.4"
 homepage = "https://github.com/tadamcz/float-table"
 description = "Top-level package for float-table."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `float_table-0.1.3/tests/test.py` & `float_table-0.1.4/tests/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,14 +48,20 @@
 
 
 def test_exponent(num_column):
     exponent = determine_eng_exponent(num_column)
     assert exponent % 3 == 0
 
 
+def test_all_zeros():
+    num_column = pd.Series([0, 0, 0])
+    exponent = determine_eng_exponent(num_column)
+    assert exponent == 0
+
+
 @pytest.mark.parametrize("sig_figs", [1, 4, 8])
 def test_numbers_correct(num_column, sig_figs):
     # The most obvious way to test this (using Python's 'g' formatter),
     # fails on edge cases: this is because round() applies "round half to even" whereas
     # 'g' format applies "round half away from zero".
     # This is a dumb hack to avoid integers that end in 5
     num_column = num_column.apply(lambda x: x + 0.0000001)
```

### Comparing `float_table-0.1.3/PKG-INFO` & `float_table-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: float-table
-Version: 0.1.3
+Version: 0.1.4
 Summary: Top-level package for float-table.
 Home-page: https://github.com/tadamcz/float-table
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

