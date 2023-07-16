# Comparing `tmp/arctix-0.0.0a14.tar.gz` & `tmp/arctix-0.0.0a19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.0a14.tar", max compression
+gzip compressed data, was "arctix-0.0.0a19.tar", max compression
```

## Comparing `arctix-0.0.0a14.tar` & `arctix-0.0.0a19.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1501 2023-07-13 07:01:44.098384 arctix-0.0.0a14/LICENSE
--rw-r--r--   0        0        0     2019 2023-07-13 07:01:44.098384 arctix-0.0.0a14/README.md
--rw-r--r--   0        0        0     3923 2023-07-13 07:01:44.098384 arctix-0.0.0a14/pyproject.toml
--rw-r--r--   0        0        0      325 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/__init__.py
--rw-r--r--   0        0        0    16123 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/formatter.py
--rw-r--r--   0        0        0    14512 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/summarizer.py
--rw-r--r--   0        0        0        0 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0     3140 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/utils/format.py
--rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 arctix-0.0.0a14/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-15 07:41:24.239477 arctix-0.0.0a19/LICENSE
+-rw-r--r--   0        0        0     2019 2023-07-15 07:41:24.239477 arctix-0.0.0a19/README.md
+-rw-r--r--   0        0        0     4016 2023-07-15 07:41:24.239477 arctix-0.0.0a19/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/__init__.py
+-rw-r--r--   0        0        0     3323 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/_torch.py
+-rw-r--r--   0        0        0    16277 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/formatter.py
+-rw-r--r--   0        0        0    18379 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/summarizer.py
+-rw-r--r--   0        0        0      228 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/testing.py
+-rw-r--r--   0        0        0        0 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/utils/format.py
+-rw-r--r--   0        0        0      669 2023-07-15 07:41:24.239477 arctix-0.0.0a19/src/arctix/utils/imports.py
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 arctix-0.0.0a19/PKG-INFO
```

### Comparing `arctix-0.0.0a14/LICENSE` & `arctix-0.0.0a19/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a14/README.md` & `arctix-0.0.0a19/README.md`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a14/pyproject.toml` & `arctix-0.0.0a19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.0a14"
+version = "0.0.0a19"
 description = "A library to get a text summary of nested objects"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
 keywords = []
 license = "BSD-3-Clause"
@@ -25,31 +25,35 @@
     { include = "arctix", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
 python = "^3.9"
 
+# Optional dependencies
+torch = { version = ">=1.10,<3.0", optional = true}
+
 [tool.poetry.extras]
+all = ["torch"]
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1"
 mkdocstrings = "^0.22"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3"
+black = "^23.7"
 coverage = { extras = ["toml"], version = "^7.2" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
 pre-commit = "^3.3"
 pygments = "^2.15"
 pylint = "^2.17"
 pytest = "^7.4"
 pytest-cov = "^4.1"
 pytest-timeout = "^2.1"
-ruff = ">=0.0.277,<1.0"
+ruff = ">=0.0.278,<1.0"
 xdoctest = "^1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
```

### Comparing `arctix-0.0.0a14/src/arctix/formatter.py` & `arctix-0.0.0a19/src/arctix/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,17 +268,18 @@
             if length > self._max_items:
                 s = f"{s}\n..."
             s = f"(length={length:,})\n{s}"
         return str_indent(f"{typ} {s}", num_spaces=self._num_spaces)
 
     def load_state_dict(self, state: dict) -> None:
         self._max_items = state["max_items"]
+        self._num_spaces = state["num_spaces"]
 
     def state_dict(self) -> dict:
-        return {"max_items": self._max_items}
+        return {"max_items": self._max_items, "num_spaces": self._num_spaces}
 
     def get_max_items(self) -> int:
         r"""Gets the maximum number of items to show.
 
         Returns:
         -------
             int: The maximum number of items to show.
@@ -424,17 +425,18 @@
                 num_spaces=self._num_spaces,
             )
             s = f"\n{s}\n..." if length > self._max_items else f"\n{s}"
         return str_indent(f"{typ} (length={length:,}){s}", num_spaces=self._num_spaces)
 
     def load_state_dict(self, state: dict) -> None:
         self._max_items = state["max_items"]
+        self._num_spaces = state["num_spaces"]
 
     def state_dict(self) -> dict:
-        return {"max_items": self._max_items}
+        return {"max_items": self._max_items, "num_spaces": self._num_spaces}
 
     def get_max_items(self) -> int:
         r"""Gets the maximum number of items to show.
 
         Returns:
         -------
             int: The maximum number of items to show.
@@ -497,15 +499,15 @@
         return self._num_spaces
 
     def set_num_spaces(self, num_spaces: int) -> None:
         r"""Set the number of spaces for indentation.
 
         Args:
         ----
-            max_characters (int): Specifies the number of spaces for
+            num_spaces (int): Specifies the number of spaces for
                 indentation.
 
         Raises:
         ------
             TypeError if ``num_spaces`` is not an integer.
             TValueError if ``num_spaces`` is not a positive integer.
```

### Comparing `arctix-0.0.0a14/src/arctix/summarizer.py` & `arctix-0.0.0a19/src/arctix/summarizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -174,18 +174,15 @@
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> from arctix import Summarizer
             >>> from arctix.formatter import MappingFormatter
-            >>> from collections import defaultdict
-            >>> Summarizer.add_formatter(defaultdict, MappingFormatter())
-            >>> # To overwrite an existing formatter
-            >>> Summarizer.add_formatter(defaultdict, MappingFormatter(), exist_ok=True)
+            >>> Summarizer.add_formatter(dict, MappingFormatter(), exist_ok=True)
         """
         if data_type in cls.registry and not exist_ok:
             raise RuntimeError(
                 f"A formatter ({cls.registry[data_type]}) is already registered for the data "
                 f"type {data_type}. Please use `exist_ok=True` if you want to overwrite the "
                 "formatter for this type"
             )
@@ -270,26 +267,24 @@
             Summarizer(
               (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'object'>): DefaultFormatter(max_characters=10)
               (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.defaultdict'>): MappingFormatter(max_items=5, num_spaces=2)
             )
             >>> Summarizer.load_state_dict({object: {"max_characters": -1}})
             >>> summarizer
             Summarizer(
               (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'object'>): DefaultFormatter(max_characters=-1)
               (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.defaultdict'>): MappingFormatter(max_items=5, num_spaces=2)
             )
         """
         for data_type, formatter in cls.registry.items():
             if (s := state.get(data_type)) is not None:
                 formatter.load_state_dict(s)
 
     @classmethod
@@ -333,44 +328,138 @@
             Summarizer(
               (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'object'>): DefaultFormatter(max_characters=10)
               (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.defaultdict'>): MappingFormatter(max_items=5, num_spaces=2)
             )
             >>> Summarizer.set_max_characters(-1)
             >>> summarizer
             Summarizer(
               (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
               (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
               (<class 'object'>): DefaultFormatter(max_characters=-1)
               (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.defaultdict'>): MappingFormatter(max_items=5, num_spaces=2)
             )
         """
         for formatter in cls.registry.values():
             if hasattr(formatter, "set_max_characters"):
                 formatter.set_max_characters(max_characters)
 
+    @classmethod
+    def set_max_items(cls, max_items: int) -> None:
+        r"""Set the maximum number of items for the compatible formatter
+        to the specified value.
+
+        To be updated, the formatters need to implement the method
+        ``set_max_items``.
+
+        Args:
+        ----
+            max_items (int): Specifies the maximum number of items to
+                show.
+
+        Example usage:
+
+        .. code-block:: pycon
+
+            >>> from arctix import Summarizer
+            >>> Summarizer.set_max_items(10)
+            >>> summarizer = Summarizer()
+            >>> summarizer
+            Summarizer(
+              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=10, num_spaces=2)
+              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=10, num_spaces=2)
+              (<class 'dict'>): MappingFormatter(max_items=10, num_spaces=2)
+              (<class 'list'>): SequenceFormatter(max_items=10, num_spaces=2)
+              (<class 'object'>): DefaultFormatter(max_characters=-1)
+              (<class 'tuple'>): SequenceFormatter(max_items=10, num_spaces=2)
+            )
+            >>> Summarizer.set_max_items(5)
+            >>> summarizer
+            Summarizer(
+              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
+              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
+              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
+              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
+              (<class 'object'>): DefaultFormatter(max_characters=-1)
+              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
+            )
+        """
+        for formatter in cls.registry.values():
+            if hasattr(formatter, "set_max_items"):
+                formatter.set_max_items(max_items)
+
+    @classmethod
+    def set_num_spaces(cls, num_spaces: int) -> None:
+        r"""Set the maximum of items for the compatible formatter to the
+        specified value.
+
+        To be updated, the formatters need to implement the method
+        ``set_num_spaces``.
+
+        Args:
+        ----
+            num_spaces (int): Specifies the number of spaces for
+                indentation.
+
+        Example usage:
+
+        .. code-block:: pycon
+
+            >>> from arctix import Summarizer
+            >>> Summarizer.set_num_spaces(4)
+            >>> summarizer = Summarizer()
+            >>> summarizer
+            Summarizer(
+              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=4)
+              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=4)
+              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=4)
+              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=4)
+              (<class 'object'>): DefaultFormatter(max_characters=-1)
+              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=4)
+            )
+            >>> Summarizer.set_num_spaces(2)
+            >>> summarizer
+            Summarizer(
+              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
+              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
+              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
+              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
+              (<class 'object'>): DefaultFormatter(max_characters=-1)
+              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
+            )
+        """
+        for formatter in cls.registry.values():
+            if hasattr(formatter, "set_num_spaces"):
+                formatter.set_num_spaces(num_spaces)
+
 
-def set_summarizer_options(max_characters: int | None = None) -> None:
+def set_summarizer_options(
+    max_characters: int | None = None, max_items: int | None = None, num_spaces: int | None = None
+) -> None:
     r"""Set the ``Summarizer`` options.
 
     Note: It is recommended to use ``summarizer_options`` rather than
     this function.
 
     Args:
     ----
         max_characters (int or None, optional): Specifies the maximum
-            number of characters to show. If ``None``, all the
-            characters are shown. Default: ``None``
+            number of characters to show. If ``None``, the maximum
+            number of characters is unchanged. Default: ``None``
+        max_items (int or None, optional): Specifies the maximum
+            number of items to show. If ``None``, the maximum
+            number of items is unchanged. Default: ``None``
+        num_spaces (int or None, optional): Specifies the number of
+            spaces for indentation. If ``None``, the number of  spaces
+            for indentation is unchanged.  Default: ``None``
 
     Example usage:
 
     .. code-block:: pycon
 
         >>> from arctix import set_summarizer_options, summary
         >>> print(summary("abcdefghijklmnopqrstuvwxyz"))
@@ -380,14 +469,18 @@
         <class 'str'> abcdefghij...
         >>> set_summarizer_options(max_characters=-1)
         >>> print(summary("abcdefghijklmnopqrstuvwxyz"))
         <class 'str'> abcdefghijklmnopqrstuvwxyz
     """
     if max_characters is not None:
         Summarizer.set_max_characters(max_characters)
+    if max_items is not None:
+        Summarizer.set_max_items(max_items)
+    if num_spaces is not None:
+        Summarizer.set_num_spaces(num_spaces)
 
 
 @contextmanager
 def summarizer_options(**kwargs) -> None:
     r"""Context manager that temporarily changes the summarizer options.
 
     Accepted arguments are same as ``set_summarizer_options``.
```

### Comparing `arctix-0.0.0a14/src/arctix/utils/format.py` & `arctix-0.0.0a19/src/arctix/utils/format.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,33 +6,43 @@
 from typing import Any
 
 
 def str_indent(original: Any, num_spaces: int = 2) -> str:
     r"""Add indentations if the original string is a multi-lines string.
 
     Args:
+    ----
         original: Specifies the original string. If the inputis not a
             string, it will be converted to a string with the function
             ``str``.
         num_spaces (int, optional): Specifies the number of spaces
             used for the indentation. Default: ``2``.
 
     Returns:
+    -------
         str: The indented string.
 
+    Raises:
+    ------
+        RuntimeError if num_spaces is not a positive integer.
+
     Example usage:
 
     .. code-block:: pycon
 
         >>> from arctix.utils.format import str_indent
         >>> print(str_indent("string1\nstring2\n  string3", 4))
         string1
         string2
           string3
     """
+    if num_spaces < 0:
+        raise RuntimeError(
+            f"Incorrect num_spaces. Expected a positive integer but received {num_spaces}"
+        )
     formatted_str = str(original).split("\n")
     if len(formatted_str) == 1:  # single line
         return formatted_str[0]
     first = formatted_str.pop(0)
     formatted_str = "\n".join([(num_spaces * " ") + line for line in formatted_str])
     return first + "\n" + formatted_str
```

### Comparing `arctix-0.0.0a14/PKG-INFO` & `arctix-0.0.0a19/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arctix
-Version: 0.0.0a14
+Version: 0.0.0a19
 Summary: A library to get a text summary of nested objects
 Home-page: https://github.com/durandtibo/arctix
 License: BSD-3-Clause
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Provides-Extra: all
+Requires-Dist: torch (>=1.10,<3.0) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/arctix
 Description-Content-Type: text/markdown
 
 # arctix
 
 <p align="center">
     <a href="https://github.com/durandtibo/arctix/actions">
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.0a14 Summary: A library to get
+Metadata-Version: 2.1 Name: arctix Version: 0.0.0a19 Summary: A library to get
 a text summary of nested objects Home-page: https://github.com/durandtibo/
 arctix License: BSD-3-Clause Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Project-URL: Repository, https://
-github.com/durandtibo/arctix Description-Content-Type: text/markdown # arctix
+Engineering :: Artificial Intelligence Provides-Extra: all Requires-Dist: torch
+(>=1.10,<3.0) ; extra == "all" Project-URL: Repository, https://github.com/
+durandtibo/arctix Description-Content-Type: text/markdown # arctix
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  61b8574ea18ecf106dce/maintainability] [https://api.codeclimate.com/v1/badges/
                      61b8574ea18ecf106dce/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
```

