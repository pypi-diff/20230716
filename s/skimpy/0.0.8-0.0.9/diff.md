# Comparing `tmp/skimpy-0.0.8.tar.gz` & `tmp/skimpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skimpy-0.0.8.tar", max compression
+gzip compressed data, was "skimpy-0.0.9.tar", max compression
```

## Comparing `skimpy-0.0.8.tar` & `skimpy-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-01-15 19:35:02.874107 skimpy-0.0.8/LICENSE.md
--rw-r--r--   0        0        0    29418 2023-01-15 19:35:02.874107 skimpy-0.0.8/README.md
--rw-r--r--   0        0        0     2013 2023-01-15 19:35:14.082198 skimpy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    26145 2023-01-15 19:35:02.878107 skimpy-0.0.8/src/skimpy/__init__.py
--rw-r--r--   0        0        0      548 2023-01-15 19:35:02.878107 skimpy-0.0.8/src/skimpy/__main__.py
--rw-r--r--   0        0        0        0 2023-01-15 19:35:02.878107 skimpy-0.0.8/src/skimpy/py.typed
--rw-r--r--   0        0        0    30750 1970-01-01 00:00:00.000000 skimpy-0.0.8/setup.py
--rw-r--r--   0        0        0    30647 1970-01-01 00:00:00.000000 skimpy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-07-16 10:40:38.768602 skimpy-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0    28974 2023-07-16 10:40:38.768602 skimpy-0.0.9/README.md
+-rw-r--r--   0        0        0     2010 2023-07-16 10:40:53.725047 skimpy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    27894 2023-07-16 10:40:38.772602 skimpy-0.0.9/src/skimpy/__init__.py
+-rw-r--r--   0        0        0      548 2023-07-16 10:40:38.772602 skimpy-0.0.9/src/skimpy/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-16 10:40:38.772602 skimpy-0.0.9/src/skimpy/py.typed
+-rw-r--r--   0        0        0    30203 1970-01-01 00:00:00.000000 skimpy-0.0.9/PKG-INFO
```

### Comparing `skimpy-0.0.8/LICENSE.md` & `skimpy-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skimpy-0.0.8/README.md` & `skimpy-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 [![Tests](https://github.com/aeturrell/skimpy/workflows/Tests/badge.svg)](https://github.com/aeturrell/skimpy/actions?workflow=Tests)
 [![Codecov](https://codecov.io/gh/aeturrell/skimpy/branch/main/graph/badge.svg)](https://codecov.io/gh/aeturrell/skimpy)
 [![Downloads](https://static.pepy.tech/badge/skimpy)](https://pepy.tech/project/skimpy)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/aeturrell/7bf183c559dc1d15ab7e7aaac39ea0ed/skimpy_demo.ipynb)
 
-[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
+![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
+![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
+![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
 
 [![Soure](https://img.shields.io/badge/source%20code-github-lightgrey?style=for-the-badge)](https://github.com/aeturrell/skimpy)
 
 **skimpy** is a light weight tool that provides
 summary statistics about variables in data frames within the console or your interactive Python window.
 Think of it as a super-charged version of `df.describe()`.
 [You can find the documentation here](https://aeturrell.github.io/skimpy/).
@@ -128,30 +128,24 @@
 Now let's clean these—by default what we get back is in _snake case_:
 
 ```python
 clean_df = clean_columns(messy_df)
 print(list(clean_df.columns))
 ```
 
-<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="color: #008080; text-decoration-color: #008080; font-weight: bold">4</span> column names have been cleaned
-</pre>
-
 <pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">'bs_lncs_n_edbn'</span>, <span style="color: #008000; text-decoration-color: #008000">'nin_hao_wo_shi_zhong_guo_ren'</span>, <span style="color: #008000; text-decoration-color: #008000">'this_is_a_test'</span>, <span style="color: #008000; text-decoration-color: #008000">'uber_uber_german_umlaut'</span><span style="font-weight: bold">]</span>
 </pre>
 
 Other naming conventions are available, for example _camel case_:
 
 ```python
 clean_df = clean_columns(messy_df, case="camel")
 print(list(clean_df.columns))
 ```
 
-<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="color: #008080; text-decoration-color: #008080; font-weight: bold">4</span> column names have been cleaned
-</pre>
-
 <pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">'bsLncsNEdbn'</span>, <span style="color: #008000; text-decoration-color: #008000">'ninHaoWoShiZhongGuoRen'</span>, <span style="color: #008000; text-decoration-color: #008000">'thisIsATest'</span>, <span style="color: #008000; text-decoration-color: #008000">'uberUberGermanUmlaut'</span><span style="font-weight: bold">]</span>
 </pre>
 
 ## Requirements
 
 You can find a full list of requirements in the [pyproject.toml](https://github.com/aeturrell/skimpy/blob/main/pyproject.toml) file. The
 main requirements are:
@@ -168,18 +162,18 @@
 
 <pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">python &gt;=<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3.8</span>,&lt;<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">4.0</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>
 </pre>
 
 <pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">click ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">8.1</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3</span>
 </pre>
 
-<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">rich &gt;=<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">10.9</span>,&lt;<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">13.0</span>
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">rich &gt;=<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">10.9</span>,&lt;<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">14.0</span>
 </pre>
 
-<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">pandas ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1.3</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2</span>
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">pandas ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.0</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3</span>
 </pre>
 
 <pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">Pygments ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.10</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>
 </pre>
 
 <pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">typeguard ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.12</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1</span>
 </pre>
```

### Comparing `skimpy-0.0.8/pyproject.toml` & `skimpy-0.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skimpy"
-version = "0.0.8"
+version = "0.0.9"
 description = "skimpy"
 authors = ["Arthur Turrell"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://aeturrell.github.io/skimpy/"
 repository = "https://github.com/aeturrell/skimpy"
 documentation = "https://aeturrell.github.io/skimpy/"
@@ -17,48 +17,48 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/aeturrell/skimpy/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
 click = "^8.1.3"
-rich = ">=10.9,<13.0"
-pandas = "^1.3.2"
+rich = ">=10.9,<14.0"
+pandas = "^2.0.3"
 Pygments = "^2.10.0"
 typeguard = "^2.12.1"
 jupyter = "^1.0.0"
 ipykernel = "^6.7.0"
 numpy = "^1.22.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.1"
-coverage = {extras = ["toml"], version = "^6.5"}
+pytest = "^7.2.2"
+coverage = {extras = ["toml"], version = "^7.2"}
 safety = "^2.3.5"
-mypy = "^0.982"
+mypy = "^1.4"
 typeguard = "^2.12.1"
-xdoctest = {extras = ["colors"], version = "^1.0.0"}
-pre-commit = "^2.16.0"
+xdoctest = {extras = ["colors"], version = "^1.1.1"}
+pre-commit = "^3.3.1"
 flake8 = "^5.0.4"
 flake8-bandit = "^4.1.1"
-flake8-bugbear = "^22.9.23"
-flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.3"
-pep8-naming = "^0.13.2"
+flake8-bugbear = "^23.3.12"
+flake8-docstrings = "^1.7.0"
+flake8-rst-docstrings = "^0.3.0"
+pep8-naming = "^0.13.3"
 darglint = "^1.8.1"
-reorder-python-imports = "^3.8.5"
-pre-commit-hooks = "^4.0.1"
+reorder-python-imports = "^3.9.0"
+pre-commit-hooks = "^4.4.0"
 Pygments = "^2.9.0"
-autopep8 = "^1.7.0"
+autopep8 = "^2.0.0"
 nox = "^2022.11.21"
 jupyter = "^1.0.0"
-jupyterlab = "^3.5.1"
-matplotlib = "^3.6.2"
+jupyterlab = "^3.6.3"
+matplotlib = "^3.7.1"
 nbstripout = "^0.6.1"
-black = "^22.10.0"
-jupyter-book = "^0.13.1"
+black = "^22.12.0"
+jupyter-book = "^0.15.1"
 furo = "^2022.9.29"
 ghp-import = "^2.1.0"
 
 [tool.poetry.scripts]
 skimpy = "skimpy.__main__:main"
 
 [tool.coverage.paths]
```

### Comparing `skimpy-0.0.8/src/skimpy/__init__.py` & `skimpy-0.0.9/src/skimpy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """skimpy provides summary statistics about variables in pandas data frames."""
 import re
 from collections import defaultdict
-from dataclasses import MISSING
 from itertools import chain
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from unicodedata import normalize
 
@@ -76,14 +75,19 @@
     for col in loop_types:
         if col[1] == "string":
             data_type = "string"
         elif col[1] == "integer":
             data_type = "int"
         elif col[1] == "floating":
             data_type = "float64"
+        elif col[1] == "timedelta64":
+            print("issue1")
+            data_type = "timedelta64[ns]"
+        elif col[1] == "timedelta64[ns]":
+            data_type = "timedelta64[ns]"
         elif col[1] == "datetime64":
             data_type = "datetime64[ns]"
         elif col[1] == "categorical":
             data_type = "category"
         elif col[1] == "boolean":
             data_type = "bool"
         else:
@@ -104,14 +108,28 @@
     """
     for col in df.select_dtypes("number"):
         df[col] = df[col].apply(lambda x: float(f'{float(f"{x:.2g}"):g}'))
     return df
 
 
 @typechecked
+def _round_series(s: pd.Series) -> pd.Series:
+    """Rounds numerical series to 2 s.f.
+
+    Args:
+        s (pd.Series): Input series
+
+    Returns:
+        pd.Series: Series with numbers rounded to 2 s.f.
+    """
+    s = s.apply(lambda x: float(f'{float(f"{x:.2g}"):g}'))
+    return s
+
+
+@typechecked
 def _map_row_positions_to_text_style(types_to_property: dict, df: pd.DataFrame) -> dict:
     """Maps positions in summary dataframe (eg row) to a Rich text property.
 
     :param types_to_property: Datatype, datetime, mapping to Rich text property
     :type types_to_property: dict
     :param df: Dataframe to map positions in
     :type df: pd.DataFrame
@@ -200,15 +218,15 @@
         string (str): colour to render strings in
         bool (str): colour to render bools in
         object (str): colour to render objects in
 
     Returns:
         rich.table.Table: instance of Table from the rich package
     """
-    str_limit: int = 20  # For longer strings, limit chars shown.
+    COL_STR_LEN_LIMIT: int = 20  # For longer strings, limit chars shown.
     df = df.reset_index().rename(columns={"index": "column_name"})
     table = Table(show_footer=False, expand=True, title=table_name, show_header=True)
     # generate dict of types to colours
     datatype_colours = {
         "number": number,
         "category": category,
         "datetime": datetime,
@@ -235,19 +253,19 @@
         [
             str(s).rstrip("0").rstrip(".") if ("." and type(s) == float) else s
             for s in row
         ]
         for row in rows
     ]
     for col in df.columns:
-        table.add_column(str(col), overflow="fold")
+        table.add_column(str(col), overflow="fold", max_width=COL_STR_LEN_LIMIT)
     for row in rows:
         row = [
             Text(
-                str(item)[:str_limit],
+                str(item),
                 style=pos_to_colour[i],
                 justify=pos_to_justification[i],
             )
             for i, item in enumerate(row)
         ]
         table.add_row(*list(row))
     return table
@@ -306,22 +324,22 @@
         pd.DataFrame: A dataframe of summary statistics, with a number of rows
         determined by number of columns of xf
     """
     count_nans_vec = xf.isna().sum()
     data_dict = {
         MISSING_COL: count_nans_vec,
         COMPLETE_COL: 100 * count_nans_vec / xf.shape[0],
-        NUM_COL_MEAN: xf.mean(),
-        "sd": xf.std(),
+        NUM_COL_MEAN: _round_series(xf.mean()),
+        "sd": _round_series(xf.std()),
     }
     display_quantiles_as_pct = 100
     quantiles_dict = dict(
         zip(
             ["p" + str(int(x * display_quantiles_as_pct)) for x in QUANTILES],
-            [xf.quantile(x) for x in QUANTILES],
+            [_round_series(xf.quantile(x)) for x in QUANTILES],
         )
     )
     data_dict.update(quantiles_dict)
     # Create histogram using unicode block elements
     # https://en.wikipedia.org/wiki/Block_Elements
     hist_series = pd.concat(
         [_create_unicode_hist(xf[col].dropna()) for col in xf.columns], axis=0
@@ -366,15 +384,15 @@
 
     Returns:
         pd.DataFrame: A dataframe of summary statistics, with a number of rows
         determined by number of columns of xf
     """
     data_dict = {
         "true": xf.sum(),
-        "true rate": xf.sum() / xf.shape[0],
+        "true rate": _round_series(xf.sum() / xf.shape[0]),
     }
     hist_series = pd.concat(
         [_create_unicode_hist(xf[col].dropna()) for col in xf.columns], axis=0
     )
     data_dict.update({"hist": hist_series})
     summary_df = pd.DataFrame(data_dict)
     return summary_df
@@ -391,22 +409,24 @@
         pd.DataFrame: A dataframe of summary statistics, with a number of rows
         determined by number of columns of xf
     """
     count_nans_vec = xf.isna().sum()
     data_dict = {
         MISSING_COL: count_nans_vec,
         COMPLETE_COL: 100 * count_nans_vec / xf.shape[0],
-        "words per row": pd.Series(
-            dict(
-                zip(
-                    xf.columns,
-                    [
-                        xf[xf.columns[0]].str.count(" ").add(1).sum() / len(xf)
-                        for col in xf.columns
-                    ],
+        "words per row": _round_series(
+            pd.Series(
+                dict(
+                    zip(
+                        xf.columns,
+                        [
+                            xf[xf.columns[0]].str.count(" ").add(1).sum() / len(xf)
+                            for col in xf.columns
+                        ],
+                    )
                 )
             )
         ),
         "total words": pd.Series(
             dict(
                 zip(
                     xf.columns,
@@ -419,14 +439,38 @@
         ),
     }
     summary_df = pd.DataFrame(data_dict)
     return summary_df
 
 
 @typechecked
+def _timedelta_variable_summary_table(xf: pd.DataFrame) -> pd.DataFrame:
+    """Summarise dataframe columns that have timedelta type. (NB not object type).
+
+    Args:
+        xf (pd.DataFrame):  Dataframe with columns of only timedelta types
+
+    Returns:
+        pd.DataFrame: A dataframe of summary statistics, with a number of rows
+        determined by number of columns of xf
+    """
+    count_nans_vec = xf.isna().sum()
+    # NB: timedelta doesn't play nicely with rounding
+    data_dict = {
+        MISSING_COL: count_nans_vec,
+        COMPLETE_COL: 100 * count_nans_vec / xf.shape[0],
+        NUM_COL_MEAN: xf.mean(),
+        "median": xf.min(),
+        "max": xf.max(),
+    }
+    summary_df = pd.DataFrame(data_dict)
+    return summary_df
+
+
+@typechecked
 def _datetime_variable_summary_table(xf: pd.DataFrame) -> pd.DataFrame:
     """Summarise dataframe columns that have datetime type.
 
     Args:
         xf (pd.DataFrame): A dataframe with only datetime columns
 
     Returns:
@@ -465,15 +509,15 @@
 
 @typechecked
 def skim(
     df_in: pd.DataFrame, header_style: str = "bold cyan", **colour_kwargs: str
 ) -> None:
     """Skim a data frame and return statistics.
 
-    skim is an alternative to pandas.DataFrame.summary(), quickly providing
+    skim is an alternative to pandas.DataFrame.describe(), quickly providing
     an overview of a data frame. It produces a different set of summary
     functions based on the types of columns in the dataframe. You may get
     better results from ensuring that you set the datatypes in your dataframe
     you want before running skim.
     The colour_kwargs (str) are defined in _dataframe_to_rich_table.
 
     Args:
@@ -536,24 +580,27 @@
     # Summaries of cols of specific types
     types_funcs_dict = {
         "number": _numeric_variable_summary_table,
         "category": _category_variable_summary_table,
         "datetime": _datetime_variable_summary_table,
         "string": _string_variable_summary_table,
         "bool": _bool_variable_summary_table,
+        "timedelta64[ns]": _timedelta_variable_summary_table,
     }
     list_of_tabs = []
     for col_type, summary_func in types_funcs_dict.items():
-        xf = df.select_dtypes(col_type)
+        if col_type == "number":
+            # timedelta and datetime are technically integers, so exclude these
+            xf = df.select_dtypes(col_type, exclude=["datetime", "timedelta"])
+        else:
+            xf = df.select_dtypes(col_type)
         if not xf.empty:
             sum_df = summary_func(xf)
             list_of_tabs.append(
-                _dataframe_to_rich_table(
-                    col_type, _round_dataframe(sum_df)  # , **colour_kwargs
-                )
+                _dataframe_to_rich_table(col_type, sum_df)  # , **colour_kwargs
             )
     # Put all of the info together
     grid = Table.grid(expand=True)
     tables_list = [dat_sum_table, types_sum_table]
     if "category" in df.dtypes.astype(str).to_list():
         tables_list.append(cat_sum_table)
     grid.add_row(Columns(tables_list))
@@ -634,15 +681,14 @@
     df = df.rename(columns=lambda col: _convert_case(col, case))
     df.columns = _rename_duplicates(df.columns, case)
     # Count the number of changed column names
     new_columns = df.columns.astype(str).tolist()
     cleaned = [
         1 if new_columns[i] != orig_columns[i] else 0 for i in range(len(orig_columns))
     ]
-    print(f"{sum(cleaned)} column names have been cleaned")
     return df
 
 
 @typechecked
 def _convert_case(name: Any, case: str) -> Any:
     """Convert case style of a column name.
 
@@ -809,8 +855,11 @@
     df["text"] = df["text"].astype("string")
     # add a datetime column
     df["date"] = pd.date_range("2018-01-01", periods=len_df, freq="M")
     df["date_no_freq"] = rng.choice(
         (pd.to_datetime(pd.Series(["01/01/2022", "03/04/2023", "01/05/1992"]))), len_df
     )
     df.loc[[3, 12, 0], "date_no_freq"] = pd.NaT
+    timedelta_array = rng.multinomial(40, [1 / 7] * 5, len_df).ravel()
+    df["time diff"] = pd.Series([pd.Timedelta(x, "d") for x in timedelta_array])
+    df.loc[[22, 1, 13, 65, 120], "time diff"] = pd.NaT
     return df
```

### Comparing `skimpy-0.0.8/src/skimpy/__main__.py` & `skimpy-0.0.9/src/skimpy/__main__.py`

 * *Files identical despite different names*

### Comparing `skimpy-0.0.8/setup.py` & `skimpy-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,305 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: skimpy
+Version: 0.0.9
+Summary: skimpy
+Home-page: https://aeturrell.github.io/skimpy/
+License: MIT
+Author: Arthur Turrell
+Requires-Python: >=3.8,<4.0.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: Pygments (>=2.10.0,<3.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: ipykernel (>=6.7.0,<7.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: numpy (>=1.22.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: rich (>=10.9,<14.0)
+Requires-Dist: typeguard (>=2.12.1,<3.0.0)
+Project-URL: Changelog, https://github.com/aeturrell/skimpy/releases
+Project-URL: Documentation, https://aeturrell.github.io/skimpy/
+Project-URL: Repository, https://github.com/aeturrell/skimpy
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Skimpy
 
-packages = \
-['skimpy']
+A light weight tool for creating summary statistics from dataframes.
+![png](docs/logo.png)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pygments>=2.10.0,<3.0.0',
- 'click>=8.1.3,<9.0.0',
- 'ipykernel>=6.7.0,<7.0.0',
- 'jupyter>=1.0.0,<2.0.0',
- 'numpy>=1.22.2,<2.0.0',
- 'pandas>=1.3.2,<2.0.0',
- 'rich>=10.9,<13.0',
- 'typeguard>=2.12.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['skimpy = skimpy.__main__:main']}
-
-setup_kwargs = {
-    'name': 'skimpy',
-    'version': '0.0.8',
-    'description': 'skimpy',
-    'long_description': '# Skimpy\n\nA light weight tool for creating summary statistics from dataframes.\n![png](docs/logo.png)\n\n[![PyPI](https://img.shields.io/pypi/v/skimpy.svg)](https://pypi.org/project/skimpy/)\n[![Status](https://img.shields.io/pypi/status/skimpy.svg)](https://pypi.org/project/skimpy/)\n[![Python Version](https://img.shields.io/pypi/pyversions/skimpy)](https://pypi.org/project/skimpy)\n[![License](https://img.shields.io/pypi/l/skimpy)](https://opensource.org/licenses/MIT)\n[![Read the documentation at https://aeturrell.github.io/skimpy/](https://img.shields.io/badge/docs-passing-brightgreen)](https://aeturrell.github.io/skimpy/)\n[![Tests](https://github.com/aeturrell/skimpy/workflows/Tests/badge.svg)](https://github.com/aeturrell/skimpy/actions?workflow=Tests)\n[![Codecov](https://codecov.io/gh/aeturrell/skimpy/branch/main/graph/badge.svg)](https://codecov.io/gh/aeturrell/skimpy)\n[![Downloads](https://static.pepy.tech/badge/skimpy)](https://pepy.tech/project/skimpy)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/aeturrell/7bf183c559dc1d15ab7e7aaac39ea0ed/skimpy_demo.ipynb)\n\n[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n\n[![Soure](https://img.shields.io/badge/source%20code-github-lightgrey?style=for-the-badge)](https://github.com/aeturrell/skimpy)\n\n**skimpy** is a light weight tool that provides\nsummary statistics about variables in data frames within the console or your interactive Python window.\nThink of it as a super-charged version of `df.describe()`.\n[You can find the documentation here](https://aeturrell.github.io/skimpy/).\n\n## Quickstart\n\n_skim_ a dataframe and produce summary statistics within the console\nusing:\n\n```python\nfrom skimpy import skim\n\nskim(df)\n```\n\nwhere `df` is a dataframe.\n\nIf you need to a dataset to try _skimpy_ out on, you can use the\nbuilt-in test dataframe:\n\n```python\nfrom skimpy import skim, generate_test_data\n\ndf = generate_test_data()\nskim(df)\n```\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">╭──────────────────────────────────────────────── skimpy summary ─────────────────────────────────────────────────╮\n│ <span style="font-style: italic">         Data Summary         </span> <span style="font-style: italic">      Data Types       </span> <span style="font-style: italic">       Categories        </span>                                │\n│ ┏━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┓ ┏━━━━━━━━━━━━━┳━━━━━━━┓ ┏━━━━━━━━━━━━━━━━━━━━━━━┓                                │\n│ ┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> dataframe         </span>┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Values </span>┃ ┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Column Type </span>┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Count </span>┃ ┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Categorical Variables </span>┃                                │\n│ ┡━━━━━━━━━━━━━━━━━━━╇━━━━━━━━┩ ┡━━━━━━━━━━━━━╇━━━━━━━┩ ┡━━━━━━━━━━━━━━━━━━━━━━━┩                                │\n│ │ Number of rows    │ 1000   │ │ float64     │ 3     │ │ class                 │                                │\n│ │ Number of columns │ 10     │ │ category    │ 2     │ │ location              │                                │\n│ └───────────────────┴────────┘ │ datetime64  │ 2     │ └───────────────────────┘                                │\n│                                │ int64       │ 1     │                                                          │\n│                                │ bool        │ 1     │                                                          │\n│                                │ string      │ 1     │                                                          │\n│                                └─────────────┴───────┘                                                          │\n│ <span style="font-style: italic">                                                    number                                                    </span>  │\n│ ┏━━━━━━━━━━━━━━━━━━┳━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓  │\n│ ┃<span style="font-weight: bold"> column_name      </span>┃<span style="font-weight: bold"> NA    </span>┃<span style="font-weight: bold"> NA %    </span>┃<span style="font-weight: bold"> mean     </span>┃<span style="font-weight: bold"> sd     </span>┃<span style="font-weight: bold"> p0         </span>┃<span style="font-weight: bold"> p25      </span>┃<span style="font-weight: bold"> p75    </span>┃<span style="font-weight: bold"> p100   </span>┃<span style="font-weight: bold"> hist    </span>┃  │\n│ ┡━━━━━━━━━━━━━━━━━━╇━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">length          </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">      0</span> │ <span style="color: #008080; text-decoration-color: #008080">     0.5</span> │ <span style="color: #008080; text-decoration-color: #008080">  0.36</span> │ <span style="color: #008080; text-decoration-color: #008080">   1.6e-06</span> │ <span style="color: #008080; text-decoration-color: #008080">    0.13</span> │ <span style="color: #008080; text-decoration-color: #008080">  0.86</span> │ <span style="color: #008080; text-decoration-color: #008080">     1</span> │ <span style="color: #008000; text-decoration-color: #008000">█▃▃▃▄█ </span> │  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">width           </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">      0</span> │ <span style="color: #008080; text-decoration-color: #008080">       2</span> │ <span style="color: #008080; text-decoration-color: #008080">   1.9</span> │ <span style="color: #008080; text-decoration-color: #008080">    0.0021</span> │ <span style="color: #008080; text-decoration-color: #008080">     0.6</span> │ <span style="color: #008080; text-decoration-color: #008080">     3</span> │ <span style="color: #008080; text-decoration-color: #008080">    14</span> │ <span style="color: #008000; text-decoration-color: #008000">  █▃▁  </span> │  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">depth           </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">      0</span> │ <span style="color: #008080; text-decoration-color: #008080">      10</span> │ <span style="color: #008080; text-decoration-color: #008080">   3.2</span> │ <span style="color: #008080; text-decoration-color: #008080">         2</span> │ <span style="color: #008080; text-decoration-color: #008080">       8</span> │ <span style="color: #008080; text-decoration-color: #008080">    12</span> │ <span style="color: #008080; text-decoration-color: #008080">    20</span> │ <span style="color: #008000; text-decoration-color: #008000">▁▄█▆▃▁ </span> │  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">rnd             </span> │ <span style="color: #008080; text-decoration-color: #008080">  120</span> │ <span style="color: #008080; text-decoration-color: #008080">     12</span> │ <span style="color: #008080; text-decoration-color: #008080">   -0.02</span> │ <span style="color: #008080; text-decoration-color: #008080">     1</span> │ <span style="color: #008080; text-decoration-color: #008080">      -2.8</span> │ <span style="color: #008080; text-decoration-color: #008080">   -0.74</span> │ <span style="color: #008080; text-decoration-color: #008080">  0.66</span> │ <span style="color: #008080; text-decoration-color: #008080">   3.7</span> │ <span style="color: #008000; text-decoration-color: #008000"> ▁▄█▅▁ </span> │  │\n│ └──────────────────┴───────┴─────────┴──────────┴────────┴────────────┴──────────┴────────┴────────┴─────────┘  │\n│ <span style="font-style: italic">                                                   category                                                   </span>  │\n│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┓  │\n│ ┃<span style="font-weight: bold"> column_name                      </span>┃<span style="font-weight: bold"> NA        </span>┃<span style="font-weight: bold"> NA %           </span>┃<span style="font-weight: bold"> ordered               </span>┃<span style="font-weight: bold"> unique             </span>┃  │\n│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━┩  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">class                           </span> │ <span style="color: #008080; text-decoration-color: #008080">        0</span> │ <span style="color: #008080; text-decoration-color: #008080">             0</span> │ <span style="color: #00d7ff; text-decoration-color: #00d7ff">False                </span> │ <span style="color: #008080; text-decoration-color: #008080">                 2</span> │  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">location                        </span> │ <span style="color: #008080; text-decoration-color: #008080">        1</span> │ <span style="color: #008080; text-decoration-color: #008080">           0.1</span> │ <span style="color: #00d7ff; text-decoration-color: #00d7ff">False                </span> │ <span style="color: #008080; text-decoration-color: #008080">                 5</span> │  │\n│ └──────────────────────────────────┴───────────┴────────────────┴───────────────────────┴────────────────────┘  │\n│ <span style="font-style: italic">                                                   datetime                                                   </span>  │\n│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━┓  │\n│ ┃<span style="font-weight: bold"> column_name             </span>┃<span style="font-weight: bold"> NA    </span>┃<span style="font-weight: bold"> NA %      </span>┃<span style="font-weight: bold"> first               </span>┃<span style="font-weight: bold"> last                </span>┃<span style="font-weight: bold"> frequency        </span>┃  │\n│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━╇━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━┩  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">date                   </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">        0</span> │ <span style="color: #800000; text-decoration-color: #800000">    2018-01-31     </span> │ <span style="color: #800000; text-decoration-color: #800000">    2101-04-30     </span> │ <span style="color: #af87ff; text-decoration-color: #af87ff">M               </span> │  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">date_no_freq           </span> │ <span style="color: #008080; text-decoration-color: #008080">    3</span> │ <span style="color: #008080; text-decoration-color: #008080">      0.3</span> │ <span style="color: #800000; text-decoration-color: #800000">    1992-01-05     </span> │ <span style="color: #800000; text-decoration-color: #800000">    2023-03-04     </span> │ <span style="color: #af87ff; text-decoration-color: #af87ff">None            </span> │  │\n│ └─────────────────────────┴───────┴───────────┴─────────────────────┴─────────────────────┴──────────────────┘  │\n│ <span style="font-style: italic">                                                    string                                                    </span>  │\n│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┓  │\n│ ┃<span style="font-weight: bold"> column_name               </span>┃<span style="font-weight: bold"> NA      </span>┃<span style="font-weight: bold"> NA %       </span>┃<span style="font-weight: bold"> words per row                </span>┃<span style="font-weight: bold"> total words              </span>┃  │\n│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━┩  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">text                     </span> │ <span style="color: #008080; text-decoration-color: #008080">      6</span> │ <span style="color: #008080; text-decoration-color: #008080">       0.6</span> │ <span style="color: #008080; text-decoration-color: #008080">                         5.8</span> │ <span style="color: #008080; text-decoration-color: #008080">                    5800</span> │  │\n│ └───────────────────────────┴─────────┴────────────┴──────────────────────────────┴──────────────────────────┘  │\n│ <span style="font-style: italic">                                                     bool                                                     </span>  │\n│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┓  │\n│ ┃<span style="font-weight: bold"> column_name                        </span>┃<span style="font-weight: bold"> true            </span>┃<span style="font-weight: bold"> true rate                     </span>┃<span style="font-weight: bold"> hist                </span>┃  │\n│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━┩  │\n│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">booly_col                         </span> │ <span style="color: #008080; text-decoration-color: #008080">            520</span> │ <span style="color: #008080; text-decoration-color: #008080">                         0.52</span> │ <span style="color: #008000; text-decoration-color: #008000">      █    █       </span> │  │\n│ └────────────────────────────────────┴─────────────────┴───────────────────────────────┴─────────────────────┘  │\n╰────────────────────────────────────────────────────── End ──────────────────────────────────────────────────────╯\n</pre>\n\nIt is recommended that you set your datatypes before using _skimpy_ (for example converting any text columns to pandas string datatype), as this will produce richer statistical summaries. However, the _skim_ function will try and guess what the datatypes of your columns are.\n\n**skimpy** also comes with a `clean_columns` function as a convenience. This slugifies column names. For example,\n\n```python\nimport pandas as pd\nfrom rich import print\nfrom skimpy import clean_columns\n\ncolumns = [\n    "bs lncs;n edbn ",\n    "Nín hǎo. Wǒ shì zhōng guó rén",\n    "___This is a test___",\n    "ÜBER Über German Umlaut",\n]\nmessy_df = pd.DataFrame(columns=columns, index=[0], data=[range(len(columns))])\nprint("Column names:")\nprint(list(messy_df.columns))\n```\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">Column names:\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">\'bs lncs;n edbn \'</span>, <span style="color: #008000; text-decoration-color: #008000">\'Nín hǎo. Wǒ shì zhōng guó rén\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'___This is a test___\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'ÜBER Über German Umlaut\'</span><span style="font-weight: bold">]</span>\n</pre>\n\nNow let\'s clean these—by default what we get back is in _snake case_:\n\n```python\nclean_df = clean_columns(messy_df)\nprint(list(clean_df.columns))\n```\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace"><span style="color: #008080; text-decoration-color: #008080; font-weight: bold">4</span> column names have been cleaned\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">\'bs_lncs_n_edbn\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'nin_hao_wo_shi_zhong_guo_ren\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'this_is_a_test\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'uber_uber_german_umlaut\'</span><span style="font-weight: bold">]</span>\n</pre>\n\nOther naming conventions are available, for example _camel case_:\n\n```python\nclean_df = clean_columns(messy_df, case="camel")\nprint(list(clean_df.columns))\n```\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace"><span style="color: #008080; text-decoration-color: #008080; font-weight: bold">4</span> column names have been cleaned\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">\'bsLncsNEdbn\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'ninHaoWoShiZhongGuoRen\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'thisIsATest\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'uberUberGermanUmlaut\'</span><span style="font-weight: bold">]</span>\n</pre>\n\n## Requirements\n\nYou can find a full list of requirements in the [pyproject.toml](https://github.com/aeturrell/skimpy/blob/main/pyproject.toml) file. The\nmain requirements are:\n\n```python\nimport toml\nfrom pathlib import Path\n\nconfig = toml.load(Path("../pyproject.toml"))\ndict_main_deps = config["tool"]["poetry"]["dependencies"]\nfor key, value in dict_main_deps.items():\n    print(f"{key} {value}")\n```\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">python &gt;=<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3.8</span>,&lt;<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">4.0</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">click ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">8.1</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">rich &gt;=<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">10.9</span>,&lt;<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">13.0</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">pandas ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1.3</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">Pygments ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.10</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">typeguard ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.12</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">jupyter ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1.0</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">ipykernel ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">6.7</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>\n</pre>\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">numpy ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1.22</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2</span>\n</pre>\n\nYou can try this package out right now in your browser using this\n[Google Colab notebook](https://colab.research.google.com/gist/aeturrell/7bf183c559dc1d15ab7e7aaac39ea0ed/skimpy_demo.ipynb)\n(requires a Google account). Note that the Google Colab notebook uses the latest package released on PyPI (rather than the development release).\n\n## Installation\n\nYou can install the latest release of _skimpy_ via\n[pip](https://pip.pypa.io/) from [PyPI](https://pypi.org/):\n\n```bash\n$ pip install skimpy\n```\n\nTo install the development version from git, use:\n\n```bash\n$ pip install git+https://github.com/aeturrell/skimpy.git\n```\n\nFor development, see {ref}`contributing`.\n\n## Usage\n\nThis package is mostly designed to be used within an interactive console\nsession or Jupyter notebook\n\n```python\nfrom skimpy import skim\n\nskim(df)\n```\n\nHowever, you can also use it on the command line:\n\n```bash\n$ skimpy file.csv\n```\n\n## Features\n\n- Support for boolean, numeric, datetime, string, and category\n  datatypes\n- Command line interface in addition to interactive console\n  functionality\n- Light weight, with results printed to terminal using the\n  [rich](https://github.com/willmcgugan/rich) package.\n- Rounds numerical output to 2 significant figures\n\n## Citing Skimpy\n\n```text\n@misc{aeturrell_2022_skimpy,\n  author       = {Arthur Turrell},\n  title        = {Skimpy: v0.0.7},\n  month        = oct,\n  year         = 2022,\n  version      = {0.0.7},\n  url          = {https://github.com/aeturrell/skimpy}\n}\n```\n\nUsing **Skimpy** in your paper? Let us know by raising an issue beginning with "citation" and we\'ll add it to this page.\n\n## Contributing\n\nContributions are very welcome. To learn more, see the page on {ref}`contributing`.\n\nNote that you will need [Make](https://www.gnu.org/software/make/) installed to build the docs automatically\n\n## License\n\nDistributed under the terms of the [MIT license](https://opensource.org/licenses/MIT), _skimpy_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems, please [file an issue](https://github.com/aeturrell/skimpy/issues) along with a detailed description.\n\n## Credits\n\nThis project was generated from [\\@cjolowicz](https://github.com/cjolowicz)\\\'s [Hypermodern Python Cookiecutter](https://github.com/cjolowicz/cookiecutter-hypermodern-python) template.\n\nskimpy was inspired by the R package [skimr](https://docs.ropensci.org/skimr/articles/skimr.html) and by exploratory Python packages including [pandas_profiling](https://pandas-profiling.github.io/pandas-profiling) and [dataprep](https://dataprep.ai/), from which the `clean_columns` function comes.\n\nThe package is built with [poetry](https://python-poetry.org/), while the documentation is built with [Jupyter Book](https://jupyterbook.org). Tests are run with [nox](https://nox.thea.codes/en/stable/).\n',
-    'author': 'Arthur Turrell',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://aeturrell.github.io/skimpy/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0.0',
+[![PyPI](https://img.shields.io/pypi/v/skimpy.svg)](https://pypi.org/project/skimpy/)
+[![Status](https://img.shields.io/pypi/status/skimpy.svg)](https://pypi.org/project/skimpy/)
+[![Python Version](https://img.shields.io/pypi/pyversions/skimpy)](https://pypi.org/project/skimpy)
+[![License](https://img.shields.io/pypi/l/skimpy)](https://opensource.org/licenses/MIT)
+[![Read the documentation at https://aeturrell.github.io/skimpy/](https://img.shields.io/badge/docs-passing-brightgreen)](https://aeturrell.github.io/skimpy/)
+[![Tests](https://github.com/aeturrell/skimpy/workflows/Tests/badge.svg)](https://github.com/aeturrell/skimpy/actions?workflow=Tests)
+[![Codecov](https://codecov.io/gh/aeturrell/skimpy/branch/main/graph/badge.svg)](https://codecov.io/gh/aeturrell/skimpy)
+[![Downloads](https://static.pepy.tech/badge/skimpy)](https://pepy.tech/project/skimpy)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/aeturrell/7bf183c559dc1d15ab7e7aaac39ea0ed/skimpy_demo.ipynb)
+
+![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
+![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
+![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
+
+[![Soure](https://img.shields.io/badge/source%20code-github-lightgrey?style=for-the-badge)](https://github.com/aeturrell/skimpy)
+
+**skimpy** is a light weight tool that provides
+summary statistics about variables in data frames within the console or your interactive Python window.
+Think of it as a super-charged version of `df.describe()`.
+[You can find the documentation here](https://aeturrell.github.io/skimpy/).
+
+## Quickstart
+
+_skim_ a dataframe and produce summary statistics within the console
+using:
+
+```python
+from skimpy import skim
+
+skim(df)
+```
+
+where `df` is a dataframe.
+
+If you need to a dataset to try _skimpy_ out on, you can use the
+built-in test dataframe:
+
+```python
+from skimpy import skim, generate_test_data
+
+df = generate_test_data()
+skim(df)
+```
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">╭──────────────────────────────────────────────── skimpy summary ─────────────────────────────────────────────────╮
+│ <span style="font-style: italic">         Data Summary         </span> <span style="font-style: italic">      Data Types       </span> <span style="font-style: italic">       Categories        </span>                                │
+│ ┏━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┓ ┏━━━━━━━━━━━━━┳━━━━━━━┓ ┏━━━━━━━━━━━━━━━━━━━━━━━┓                                │
+│ ┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> dataframe         </span>┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Values </span>┃ ┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Column Type </span>┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Count </span>┃ ┃<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Categorical Variables </span>┃                                │
+│ ┡━━━━━━━━━━━━━━━━━━━╇━━━━━━━━┩ ┡━━━━━━━━━━━━━╇━━━━━━━┩ ┡━━━━━━━━━━━━━━━━━━━━━━━┩                                │
+│ │ Number of rows    │ 1000   │ │ float64     │ 3     │ │ class                 │                                │
+│ │ Number of columns │ 10     │ │ category    │ 2     │ │ location              │                                │
+│ └───────────────────┴────────┘ │ datetime64  │ 2     │ └───────────────────────┘                                │
+│                                │ int64       │ 1     │                                                          │
+│                                │ bool        │ 1     │                                                          │
+│                                │ string      │ 1     │                                                          │
+│                                └─────────────┴───────┘                                                          │
+│ <span style="font-style: italic">                                                    number                                                    </span>  │
+│ ┏━━━━━━━━━━━━━━━━━━┳━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓  │
+│ ┃<span style="font-weight: bold"> column_name      </span>┃<span style="font-weight: bold"> NA    </span>┃<span style="font-weight: bold"> NA %    </span>┃<span style="font-weight: bold"> mean     </span>┃<span style="font-weight: bold"> sd     </span>┃<span style="font-weight: bold"> p0         </span>┃<span style="font-weight: bold"> p25      </span>┃<span style="font-weight: bold"> p75    </span>┃<span style="font-weight: bold"> p100   </span>┃<span style="font-weight: bold"> hist    </span>┃  │
+│ ┡━━━━━━━━━━━━━━━━━━╇━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">length          </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">      0</span> │ <span style="color: #008080; text-decoration-color: #008080">     0.5</span> │ <span style="color: #008080; text-decoration-color: #008080">  0.36</span> │ <span style="color: #008080; text-decoration-color: #008080">   1.6e-06</span> │ <span style="color: #008080; text-decoration-color: #008080">    0.13</span> │ <span style="color: #008080; text-decoration-color: #008080">  0.86</span> │ <span style="color: #008080; text-decoration-color: #008080">     1</span> │ <span style="color: #008000; text-decoration-color: #008000">█▃▃▃▄█ </span> │  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">width           </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">      0</span> │ <span style="color: #008080; text-decoration-color: #008080">       2</span> │ <span style="color: #008080; text-decoration-color: #008080">   1.9</span> │ <span style="color: #008080; text-decoration-color: #008080">    0.0021</span> │ <span style="color: #008080; text-decoration-color: #008080">     0.6</span> │ <span style="color: #008080; text-decoration-color: #008080">     3</span> │ <span style="color: #008080; text-decoration-color: #008080">    14</span> │ <span style="color: #008000; text-decoration-color: #008000">  █▃▁  </span> │  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">depth           </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">      0</span> │ <span style="color: #008080; text-decoration-color: #008080">      10</span> │ <span style="color: #008080; text-decoration-color: #008080">   3.2</span> │ <span style="color: #008080; text-decoration-color: #008080">         2</span> │ <span style="color: #008080; text-decoration-color: #008080">       8</span> │ <span style="color: #008080; text-decoration-color: #008080">    12</span> │ <span style="color: #008080; text-decoration-color: #008080">    20</span> │ <span style="color: #008000; text-decoration-color: #008000">▁▄█▆▃▁ </span> │  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">rnd             </span> │ <span style="color: #008080; text-decoration-color: #008080">  120</span> │ <span style="color: #008080; text-decoration-color: #008080">     12</span> │ <span style="color: #008080; text-decoration-color: #008080">   -0.02</span> │ <span style="color: #008080; text-decoration-color: #008080">     1</span> │ <span style="color: #008080; text-decoration-color: #008080">      -2.8</span> │ <span style="color: #008080; text-decoration-color: #008080">   -0.74</span> │ <span style="color: #008080; text-decoration-color: #008080">  0.66</span> │ <span style="color: #008080; text-decoration-color: #008080">   3.7</span> │ <span style="color: #008000; text-decoration-color: #008000"> ▁▄█▅▁ </span> │  │
+│ └──────────────────┴───────┴─────────┴──────────┴────────┴────────────┴──────────┴────────┴────────┴─────────┘  │
+│ <span style="font-style: italic">                                                   category                                                   </span>  │
+│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┓  │
+│ ┃<span style="font-weight: bold"> column_name                      </span>┃<span style="font-weight: bold"> NA        </span>┃<span style="font-weight: bold"> NA %           </span>┃<span style="font-weight: bold"> ordered               </span>┃<span style="font-weight: bold"> unique             </span>┃  │
+│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━┩  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">class                           </span> │ <span style="color: #008080; text-decoration-color: #008080">        0</span> │ <span style="color: #008080; text-decoration-color: #008080">             0</span> │ <span style="color: #00d7ff; text-decoration-color: #00d7ff">False                </span> │ <span style="color: #008080; text-decoration-color: #008080">                 2</span> │  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">location                        </span> │ <span style="color: #008080; text-decoration-color: #008080">        1</span> │ <span style="color: #008080; text-decoration-color: #008080">           0.1</span> │ <span style="color: #00d7ff; text-decoration-color: #00d7ff">False                </span> │ <span style="color: #008080; text-decoration-color: #008080">                 5</span> │  │
+│ └──────────────────────────────────┴───────────┴────────────────┴───────────────────────┴────────────────────┘  │
+│ <span style="font-style: italic">                                                   datetime                                                   </span>  │
+│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━┓  │
+│ ┃<span style="font-weight: bold"> column_name             </span>┃<span style="font-weight: bold"> NA    </span>┃<span style="font-weight: bold"> NA %      </span>┃<span style="font-weight: bold"> first               </span>┃<span style="font-weight: bold"> last                </span>┃<span style="font-weight: bold"> frequency        </span>┃  │
+│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━╇━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━┩  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">date                   </span> │ <span style="color: #008080; text-decoration-color: #008080">    0</span> │ <span style="color: #008080; text-decoration-color: #008080">        0</span> │ <span style="color: #800000; text-decoration-color: #800000">    2018-01-31     </span> │ <span style="color: #800000; text-decoration-color: #800000">    2101-04-30     </span> │ <span style="color: #af87ff; text-decoration-color: #af87ff">M               </span> │  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">date_no_freq           </span> │ <span style="color: #008080; text-decoration-color: #008080">    3</span> │ <span style="color: #008080; text-decoration-color: #008080">      0.3</span> │ <span style="color: #800000; text-decoration-color: #800000">    1992-01-05     </span> │ <span style="color: #800000; text-decoration-color: #800000">    2023-03-04     </span> │ <span style="color: #af87ff; text-decoration-color: #af87ff">None            </span> │  │
+│ └─────────────────────────┴───────┴───────────┴─────────────────────┴─────────────────────┴──────────────────┘  │
+│ <span style="font-style: italic">                                                    string                                                    </span>  │
+│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┓  │
+│ ┃<span style="font-weight: bold"> column_name               </span>┃<span style="font-weight: bold"> NA      </span>┃<span style="font-weight: bold"> NA %       </span>┃<span style="font-weight: bold"> words per row                </span>┃<span style="font-weight: bold"> total words              </span>┃  │
+│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━┩  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">text                     </span> │ <span style="color: #008080; text-decoration-color: #008080">      6</span> │ <span style="color: #008080; text-decoration-color: #008080">       0.6</span> │ <span style="color: #008080; text-decoration-color: #008080">                         5.8</span> │ <span style="color: #008080; text-decoration-color: #008080">                    5800</span> │  │
+│ └───────────────────────────┴─────────┴────────────┴──────────────────────────────┴──────────────────────────┘  │
+│ <span style="font-style: italic">                                                     bool                                                     </span>  │
+│ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┓  │
+│ ┃<span style="font-weight: bold"> column_name                        </span>┃<span style="font-weight: bold"> true            </span>┃<span style="font-weight: bold"> true rate                     </span>┃<span style="font-weight: bold"> hist                </span>┃  │
+│ ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━┩  │
+│ │ <span style="color: #af87ff; text-decoration-color: #af87ff">booly_col                         </span> │ <span style="color: #008080; text-decoration-color: #008080">            520</span> │ <span style="color: #008080; text-decoration-color: #008080">                         0.52</span> │ <span style="color: #008000; text-decoration-color: #008000">      █    █       </span> │  │
+│ └────────────────────────────────────┴─────────────────┴───────────────────────────────┴─────────────────────┘  │
+╰────────────────────────────────────────────────────── End ──────────────────────────────────────────────────────╯
+</pre>
+
+It is recommended that you set your datatypes before using _skimpy_ (for example converting any text columns to pandas string datatype), as this will produce richer statistical summaries. However, the _skim_ function will try and guess what the datatypes of your columns are.
+
+**skimpy** also comes with a `clean_columns` function as a convenience. This slugifies column names. For example,
+
+```python
+import pandas as pd
+from rich import print
+from skimpy import clean_columns
+
+columns = [
+    "bs lncs;n edbn ",
+    "Nín hǎo. Wǒ shì zhōng guó rén",
+    "___This is a test___",
+    "ÜBER Über German Umlaut",
+]
+messy_df = pd.DataFrame(columns=columns, index=[0], data=[range(len(columns))])
+print("Column names:")
+print(list(messy_df.columns))
+```
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">Column names:
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">'bs lncs;n edbn '</span>, <span style="color: #008000; text-decoration-color: #008000">'Nín hǎo. Wǒ shì zhōng guó rén'</span>, <span style="color: #008000; text-decoration-color: #008000">'___This is a test___'</span>, <span style="color: #008000; text-decoration-color: #008000">'ÜBER Über German Umlaut'</span><span style="font-weight: bold">]</span>
+</pre>
+
+Now let's clean these—by default what we get back is in _snake case_:
+
+```python
+clean_df = clean_columns(messy_df)
+print(list(clean_df.columns))
+```
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">'bs_lncs_n_edbn'</span>, <span style="color: #008000; text-decoration-color: #008000">'nin_hao_wo_shi_zhong_guo_ren'</span>, <span style="color: #008000; text-decoration-color: #008000">'this_is_a_test'</span>, <span style="color: #008000; text-decoration-color: #008000">'uber_uber_german_umlaut'</span><span style="font-weight: bold">]</span>
+</pre>
+
+Other naming conventions are available, for example _camel case_:
+
+```python
+clean_df = clean_columns(messy_df, case="camel")
+print(list(clean_df.columns))
+```
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="font-weight: bold">[</span><span style="color: #008000; text-decoration-color: #008000">'bsLncsNEdbn'</span>, <span style="color: #008000; text-decoration-color: #008000">'ninHaoWoShiZhongGuoRen'</span>, <span style="color: #008000; text-decoration-color: #008000">'thisIsATest'</span>, <span style="color: #008000; text-decoration-color: #008000">'uberUberGermanUmlaut'</span><span style="font-weight: bold">]</span>
+</pre>
+
+## Requirements
+
+You can find a full list of requirements in the [pyproject.toml](https://github.com/aeturrell/skimpy/blob/main/pyproject.toml) file. The
+main requirements are:
+
+```python
+import toml
+from pathlib import Path
+
+config = toml.load(Path("../pyproject.toml"))
+dict_main_deps = config["tool"]["poetry"]["dependencies"]
+for key, value in dict_main_deps.items():
+    print(f"{key} {value}")
+```
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">python &gt;=<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3.8</span>,&lt;<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">4.0</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">click ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">8.1</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">rich &gt;=<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">10.9</span>,&lt;<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">14.0</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">pandas ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.0</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">3</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">Pygments ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.10</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">typeguard ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2.12</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">jupyter ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1.0</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">ipykernel ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">6.7</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">0</span>
+</pre>
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">numpy ^<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">1.22</span>.<span style="color: #008080; text-decoration-color: #008080; font-weight: bold">2</span>
+</pre>
+
+You can try this package out right now in your browser using this
+[Google Colab notebook](https://colab.research.google.com/gist/aeturrell/7bf183c559dc1d15ab7e7aaac39ea0ed/skimpy_demo.ipynb)
+(requires a Google account). Note that the Google Colab notebook uses the latest package released on PyPI (rather than the development release).
+
+## Installation
+
+You can install the latest release of _skimpy_ via
+[pip](https://pip.pypa.io/) from [PyPI](https://pypi.org/):
+
+```bash
+$ pip install skimpy
+```
+
+To install the development version from git, use:
+
+```bash
+$ pip install git+https://github.com/aeturrell/skimpy.git
+```
+
+For development, see {ref}`contributing`.
+
+## Usage
+
+This package is mostly designed to be used within an interactive console
+session or Jupyter notebook
+
+```python
+from skimpy import skim
+
+skim(df)
+```
+
+However, you can also use it on the command line:
+
+```bash
+$ skimpy file.csv
+```
+
+## Features
+
+- Support for boolean, numeric, datetime, string, and category
+  datatypes
+- Command line interface in addition to interactive console
+  functionality
+- Light weight, with results printed to terminal using the
+  [rich](https://github.com/willmcgugan/rich) package.
+- Rounds numerical output to 2 significant figures
+
+## Citing Skimpy
+
+```text
+@misc{aeturrell_2022_skimpy,
+  author       = {Arthur Turrell},
+  title        = {Skimpy: v0.0.7},
+  month        = oct,
+  year         = 2022,
+  version      = {0.0.7},
+  url          = {https://github.com/aeturrell/skimpy}
 }
+```
+
+Using **Skimpy** in your paper? Let us know by raising an issue beginning with "citation" and we'll add it to this page.
+
+## Contributing
+
+Contributions are very welcome. To learn more, see the page on {ref}`contributing`.
+
+Note that you will need [Make](https://www.gnu.org/software/make/) installed to build the docs automatically
+
+## License
+
+Distributed under the terms of the [MIT license](https://opensource.org/licenses/MIT), _skimpy_ is free and open source software.
+
+## Issues
+
+If you encounter any problems, please [file an issue](https://github.com/aeturrell/skimpy/issues) along with a detailed description.
+
+## Credits
+
+This project was generated from [\@cjolowicz](https://github.com/cjolowicz)\'s [Hypermodern Python Cookiecutter](https://github.com/cjolowicz/cookiecutter-hypermodern-python) template.
+
+skimpy was inspired by the R package [skimr](https://docs.ropensci.org/skimr/articles/skimr.html) and by exploratory Python packages including [pandas_profiling](https://pandas-profiling.github.io/pandas-profiling) and [dataprep](https://dataprep.ai/), from which the `clean_columns` function comes.
 
+The package is built with [poetry](https://python-poetry.org/), while the documentation is built with [Jupyter Book](https://jupyterbook.org). Tests are run with [nox](https://nox.thea.codes/en/stable/).
 
-setup(**setup_kwargs)
```

