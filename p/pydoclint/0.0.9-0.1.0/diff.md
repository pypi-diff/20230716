# Comparing `tmp/pydoclint-0.0.9.tar.gz` & `tmp/pydoclint-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.9.tar", last modified: Mon Jun 12 08:31:16 2023, max compression
+gzip compressed data, was "pydoclint-0.1.0.tar", last modified: Sun Jul 16 00:19:47 2023, max compression
```

## Comparing `pydoclint-0.0.9.tar` & `pydoclint-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.967443 pydoclint-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-12 08:31:07.000000 pydoclint-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-06-12 08:31:16.967443 pydoclint-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-12 08:31:07.000000 pydoclint-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.963443 pydoclint-0.0.9/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.967443 pydoclint-0.0.9/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.963443 pydoclint-0.0.9/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-12 08:31:16.967443 pydoclint-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 08:31:07.000000 pydoclint-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.967443 pydoclint-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    33175 2023-06-12 08:31:07.000000 pydoclint-0.0.9/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-12 08:31:07.000000 pydoclint-0.0.9/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-16 00:19:32.000000 pydoclint-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-07-16 00:19:47.940734 pydoclint-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-07-16 00:19:32.000000 pydoclint-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/return_anno.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/return_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23893 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-16 00:19:47.940734 pydoclint-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-16 00:19:32.000000 pydoclint-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-16 00:19:32.000000 pydoclint-0.1.0/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-07-16 00:19:32.000000 pydoclint-0.1.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-16 00:19:32.000000 pydoclint-0.1.0/tests/test_parse_config.py
```

### Comparing `pydoclint-0.0.9/LICENSE` & `pydoclint-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.9/PKG-INFO` & `pydoclint-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -175,14 +175,15 @@
 
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
+| `DOC203` | Return type(s) in the docstring not consistent with the return annotation                            |
 
 Note on `DOC201`: Methods with `@property` as its last decorator do not need to
 have a return section.
 
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
 | Code     | Explanation                                                                                             |
```

### Comparing `pydoclint-0.0.9/README.md` & `pydoclint-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
 
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
+| `DOC203` | Return type(s) in the docstring not consistent with the return annotation                            |
 
 Note on `DOC201`: Methods with `@property` as its last decorator do not need to
 have a return section.
 
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
 | Code     | Explanation                                                                                             |
```

### Comparing `pydoclint-0.0.9/pydoclint/flake8_entry.py` & `pydoclint-0.1.0/pydoclint/flake8_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,25 @@
             parse_from_config=True,
             help=(
                 'If False, a return section is not needed in docstring if'
                 ' the function body does not have a "return" statement and'
                 ' the return type annotation is "-> None".'
             ),
         )
+        parser.add_option(
+            '-crt',
+            '--check-return-types',
+            action='store',
+            default='True',
+            parse_from_config=True,
+            help=(
+                'If True, check that the type(s) in the docstring return section and'
+                ' the return annotation in the function signature are consistent'
+            ),
+        )
 
     @classmethod
     def parse_options(cls, options):  # noqa: D102
         cls.type_hints_in_signature = options.type_hints_in_signature
         cls.type_hints_in_docstring = options.type_hints_in_docstring
         cls.check_arg_order = options.check_arg_order
         cls.skip_checking_short_docstrings = (
```

### Comparing `pydoclint-0.0.9/pydoclint/main.py` & `pydoclint-0.1.0/pydoclint/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 def validateStyleValue(
         context: click.Context,
         param: click.Parameter,
         value: Optional[str],
 ) -> Optional[str]:
     """Validate the value of the 'style' option"""
     if value not in {'numpy', 'google'}:
-        raise click.BadParameter('"--style" must be "numpy" or "google"')
+        raise click.BadParameter(
+            '"--style" must be "numpy", "google", or "sphinx"'
+        )
 
     return value
 
 
 @click.command(
     context_settings={'help_option_names': ['-h', '--help']},
     help='Pydoclint, a linter for Python docstring styles',
@@ -123,14 +125,25 @@
     default=False,
     help=(
         'If False, a return section is not needed in docstring if'
         ' the function body does not have a "return" statement and'
         ' the return type annotation is "-> None".'
     ),
 )
+@click.option(
+    '-crt',
+    '--check-return-types',
+    type=bool,
+    show_default=True,
+    default=True,
+    help=(
+        'If True, check that the type(s) in the docstring return section and'
+        ' the return annotation in the function signature are consistent'
+    ),
+)
 @click.argument(
     'paths',
     nargs=-1,
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=True,
@@ -168,14 +181,15 @@
         paths: Tuple[str, ...],
         type_hints_in_signature: bool,
         type_hints_in_docstring: bool,
         check_arg_order: bool,
         skip_checking_short_docstrings: bool,
         skip_checking_raises: bool,
         allow_init_docstring: bool,
+        check_return_types: bool,
         require_return_section_when_returning_none: bool,
         config: Optional[str],  # don't remove it b/c it's required by `click`
 ) -> None:
     """Command-line entry point of pydoclint"""
     ctx.ensure_object(dict)
 
     if paths and src is not None:
@@ -200,14 +214,15 @@
         paths=paths,
         typeHintsInSignature=type_hints_in_signature,
         typeHintsInDocstring=type_hints_in_docstring,
         checkArgOrder=check_arg_order,
         skipCheckingShortDocstrings=skip_checking_short_docstrings,
         skipCheckingRaises=skip_checking_raises,
         allowInitDocstring=allow_init_docstring,
+        checkReturnTypes=check_return_types,
         requireReturnSectionWhenReturningNone=require_return_section_when_returning_none,
     )
 
     violationCounter: int = 0
     if len(violationsInAllFiles) > 0:
         counter = 0
         for filename, violationsInThisFile in violationsInAllFiles.items():
@@ -255,14 +270,15 @@
         style: str = 'numpy',
         typeHintsInSignature: bool = True,
         typeHintsInDocstring: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
+        checkReturnTypes: bool = True,
         requireReturnSectionWhenReturningNone: bool = False,
         quiet: bool = False,
         exclude: str = '',
 ) -> Dict[str, List[Violation]]:
     filenames: List[Path] = []
 
     if not quiet:
@@ -296,14 +312,15 @@
             style=style,
             typeHintsInSignature=typeHintsInSignature,
             typeHintsInDocstring=typeHintsInDocstring,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
             allowInitDocstring=allowInitDocstring,
+            checkReturnTypes=checkReturnTypes,
             requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
         )
         allViolations[filename.as_posix()] = violationsInThisFile
 
     return allViolations
 
 
@@ -312,28 +329,30 @@
         style: str = 'numpy',
         typeHintsInSignature: bool = True,
         typeHintsInDocstring: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
+        checkReturnTypes: bool = True,
         requireReturnSectionWhenReturningNone: bool = False,
 ) -> List[Violation]:
     with open(filename, encoding='utf8') as fp:
         src: str = ''.join(fp.readlines())
 
     tree: ast.Module = ast.parse(src)
     visitor = Visitor(
         style=style,
         typeHintsInSignature=typeHintsInSignature,
         typeHintsInDocstring=typeHintsInDocstring,
         checkArgOrder=checkArgOrder,
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
         skipCheckingRaises=skipCheckingRaises,
         allowInitDocstring=allowInitDocstring,
+        checkReturnTypes=checkReturnTypes,
         requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
     )
     visitor.visit(tree)
     return visitor.violations
 
 
 if __name__ == '__main__':
```

### Comparing `pydoclint-0.0.9/pydoclint/parse_config.py` & `pydoclint-0.1.0/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.9/pydoclint/utils/annotation.py` & `pydoclint-0.1.0/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.9/pydoclint/utils/arg.py` & `pydoclint-0.1.0/pydoclint/utils/arg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ast
 from typing import List, Optional, Set
 
 from docstring_parser.common import DocstringParam
 from numpydoc.docscrape import Parameter
 
 from pydoclint.utils.annotation import unparseAnnotation
+from pydoclint.utils.generic import stripQuotes
 
 
 class Arg:
     """
     A class to hold function input/return arguments.
 
     This class also defines some essential behaviors of an argument, such
@@ -46,15 +47,15 @@
 
         return self.typeHint < other.typeHint
 
     def __le__(self, other: 'Arg') -> bool:
         return self < other or self == other
 
     def __hash__(self) -> int:
-        return hash((self.name, self._stripQuotes(self.typeHint)))
+        return hash((self.name, stripQuotes(self.typeHint)))
 
     def nameEquals(self, other: 'Arg') -> bool:
         """More lenient equality: only compare names"""
         return self.name == other.name
 
     def hasTypeHint(self) -> bool:
         """Check whether this arg has type hint"""
@@ -87,19 +88,15 @@
 
     @classmethod
     def _str(cls, typeName: Optional[str]) -> str:
         return '' if typeName is None else typeName
 
     @classmethod
     def _eq(cls, str1: str, str2: str) -> bool:
-        return cls._stripQuotes(str1) == cls._stripQuotes(str2)
-
-    @classmethod
-    def _stripQuotes(cls, string: str) -> str:
-        return string.replace('"', '').replace("'", '')
+        return stripQuotes(str1) == stripQuotes(str2)
 
 
 class ArgList:
     """
     A class to hold a list of `Arg` objects.
 
     This class also defines some behaviors of an argument list, such as
@@ -219,23 +216,18 @@
         return set(self.infoList) - set(other.infoList)
 
     def noTypeHints(self) -> bool:
         """Check whether none of the args have type hints"""
         return not self.hasTypeHintInAnyArg()
 
     def hasTypeHintInAnyArg(self) -> bool:
-        """
-        Check whether any arg has a type hint.
-
-        Start arguments (such as `*args` or `**kwargs`) are excluded because
-        they don't need to have type hints.
-        """
-        return any(_.hasTypeHint() for _ in self.infoList if _.notStarArg())
+        """Check whether any arg has a type hint"""
+        return any(_.hasTypeHint() for _ in self.infoList)
 
     def hasTypeHintInAllArgs(self) -> bool:
         """
         Check whether all args have a type hint.
 
-        Start arguments (such as `*args` or `**kwargs`) are excluded because
+        Star arguments (such as `*args` or `**kwargs`) are excluded because
         they don't need to have type hints.
         """
         return all(_.hasTypeHint() for _ in self.infoList if _.notStarArg())
```

### Comparing `pydoclint-0.0.9/pydoclint/utils/astTypes.py` & `pydoclint-0.1.0/pydoclint/utils/astTypes.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.9/pydoclint/utils/generic.py` & `pydoclint-0.1.0/pydoclint/utils/generic.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     )
 
 
 def getFunctionId(node: FuncOrAsyncFuncDef) -> Tuple[int, int, str]:
     """
     Get unique identifier of a function def. We also need line and
     column number because different function can have identical names.
+
+    Note: this function is no longer used by the actual code, but it is
+    still used in unit tests. That's why we did not remove it.
     """
     return node.lineno, node.col_offset, node.name
 
 
 def detectMethodType(node: ast.FunctionDef) -> MethodType:
     """
     Detect whether the function def is an instance method,
@@ -72,14 +75,27 @@
 
             if decorator.id == 'staticmethod':
                 return MethodType.STATIC_METHOD
 
     return MethodType.INSTANCE_METHOD
 
 
+def checkIsAbstractMethod(node: ast.FunctionDef) -> bool:
+    """Check whether `node` is an abstract method"""
+    if len(node.decorator_list) == 0:
+        return False
+
+    for decorator in node.decorator_list:
+        if isinstance(decorator, ast.Name):
+            if decorator.id == 'abstractmethod':
+                return True
+
+    return False
+
+
 def getDocstring(node: ClassOrFunctionDef) -> str:
     """Get docstring from a class definition or a function definition"""
     docstring_: Optional[str] = ast.get_docstring(node)
     return '' if docstring_ is None else docstring_
 
 
 def generateMsgPrefix(
@@ -138,7 +154,12 @@
 def stringStartsWith(string: str, substrings: Tuple[str, ...]) -> bool:
     """Check whether the string starts with any of the substrings"""
     for substring in substrings:
         if string.startswith(substring):
             return True
 
     return False
+
+
+def stripQuotes(string: Optional[str]) -> Optional[str]:
+    """Strip quote (both double and single quote) from the given string"""
+    return None if string is None else string.replace('"', '').replace("'", '')
```

### Comparing `pydoclint-0.0.9/pydoclint/utils/unparser.py` & `pydoclint-0.1.0/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.9/pydoclint/utils/violation.py` & `pydoclint-0.1.0/pydoclint/utils/violation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import types
+from copy import deepcopy
 from typing import Tuple
 
 from pydoclint.utils.internal_error import InternalError
 
 VIOLATION_CODES = types.MappingProxyType({
     1: 'Potential formatting errors in docstring. Error message:',
 
@@ -19,14 +20,15 @@
     108: 'The option `--type-hints-in-signature` is `False` but there are type hints in the signature',
     109: 'The option `--type-hints-in-docstring` is `True` but there are no type hints in the docstring arg list',
     110: 'The option `--type-hints-in-docstring` is `True` but not all args in the docstring arg list have type hints',
     111: 'The option `--type-hints-in-docstring` is `False` but there are type hints in the docstring arg list',
 
     201: 'does not have a return section in docstring',
     202: 'has a return section in docstring, but there are no return statements or annotations',
+    203: 'return type(s) in docstring not consistent with the return annotation.',
 
     301: '__init__() should not have a docstring; please combine it with the docstring of the class',
     302: 'The class docstring does not need a "Returns" section, because __init__() cannot return anything',
     303: 'The __init__() docstring does not need a "Returns" section, because it cannot return anything',
     304: 'Class docstring has an argument/parameter section; please put it in the __init__() docstring',
     305: 'Class docstring has a "Raises" section; please put it in the __init__() docstring',
     306: 'The class docstring does not need a "Yields" section, because __init__() cannot yield anything',
@@ -76,7 +78,13 @@
         return f'{self.line}: {self.__str__()}'
 
     def getInfoForFlake8(self) -> Tuple[int, int, str]:
         """Get the violation info for flake8"""
         colOffset: int = 0  # we don't need column offset to locate the issue
         msg = f'{self.fullErrorCode} {self.msg}'  # no colon b/c that would cause 'yesqa' issues
         return self.line, colOffset, msg
+
+    def appendMoreMsg(self, moreMsg: str) -> 'Violation':
+        """Append more error message, and return a new Violation object"""
+        new = deepcopy(self)
+        new.msg += moreMsg
+        return new
```

### Comparing `pydoclint-0.0.9/pydoclint/utils/walk.py` & `pydoclint-0.1.0/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.9/pydoclint/visitor.py` & `pydoclint-0.1.0/pydoclint/visitor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import ast
 from typing import List, Optional, Set
 
+from pydoclint.utils.annotation import unparseAnnotation
 from pydoclint.utils.arg import Arg, ArgList
 from pydoclint.utils.astTypes import FuncOrAsyncFuncDef
 from pydoclint.utils.doc import Doc
 from pydoclint.utils.generic import (
+    checkIsAbstractMethod,
     collectFuncArgs,
     detectMethodType,
     generateMsgPrefix,
     getDocstring,
     isPropertyMethod,
+    stripQuotes,
 )
 from pydoclint.utils.internal_error import InternalError
 from pydoclint.utils.method_type import MethodType
+from pydoclint.utils.return_anno import ReturnAnnotation
+from pydoclint.utils.return_arg import ReturnArg
 from pydoclint.utils.return_yield_raise import (
     hasGeneratorAsReturnAnnotation,
     hasIteratorOrIterableAsReturnAnnotation,
     hasRaiseStatements,
     hasReturnAnnotation,
     hasReturnStatements,
     hasYieldStatements,
@@ -33,23 +38,25 @@
             style: str = 'numpy',
             typeHintsInSignature: bool = True,
             typeHintsInDocstring: bool = True,
             checkArgOrder: bool = True,
             skipCheckingShortDocstrings: bool = True,
             skipCheckingRaises: bool = False,
             allowInitDocstring: bool = False,
+            checkReturnTypes: bool = True,
             requireReturnSectionWhenReturningNone: bool = False,
     ) -> None:
         self.style: str = style
         self.typeHintsInSignature: bool = typeHintsInSignature
         self.typeHintsInDocstring: bool = typeHintsInDocstring
         self.checkArgOrder: bool = checkArgOrder
         self.skipCheckingShortDocstrings: bool = skipCheckingShortDocstrings
         self.skipCheckingRaises: bool = skipCheckingRaises
         self.allowInitDocstring: bool = allowInitDocstring
+        self.checkReturnTypes: bool = checkReturnTypes
         self.requireReturnSectionWhenReturningNone: bool = (
             requireReturnSectionWhenReturningNone
         )
 
         self.parent: Optional[ast.AST] = None  # keep track of parent node
         self.violations: List[Violation] = []
 
@@ -67,14 +74,16 @@
 
         isClassConstructor: bool = node.name == '__init__' and isinstance(
             parent_, ast.ClassDef
         )
 
         docstring: str = getDocstring(node)
 
+        self.isAbstractMethod = checkIsAbstractMethod(node)
+
         if isClassConstructor:
             docstring = self._checkClassConstructorDocstrings(
                 node=node,
                 parent_=parent_,
                 initDocstring=docstring,
             )
 
@@ -404,26 +413,27 @@
                         msgPrefix=msgPrefix,
                         msgPostfix=' '.join(msgPostfixParts),
                     )
                 )
 
         return violations
 
-    def checkReturns(
+    def checkReturns(  # noqa: C901
             self,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
             doc: Doc,
     ) -> List[Violation]:
         """Check return statement & return type annotation of this function"""
         lineNum: int = node.lineno
         msgPrefix = generateMsgPrefix(node, parent, appendColon=False)
 
         v201 = Violation(code=201, line=lineNum, msgPrefix=msgPrefix)
         v202 = Violation(code=202, line=lineNum, msgPrefix=msgPrefix)
+        v203 = Violation(code=203, line=lineNum, msgPrefix=msgPrefix)
 
         hasReturnStmt: bool = hasReturnStatements(node)
         hasReturnAnno: bool = hasReturnAnnotation(node)
         hasGenAsRetAnno: bool = hasGeneratorAsReturnAnnotation(node)
         onlyHasYieldStmt: bool = hasYieldStatements(node) and not hasReturnStmt
         hasIterAsRetAnno: bool = hasIteratorOrIterableAsReturnAnnotation(node)
 
@@ -445,14 +455,106 @@
                     violations.append(v201)
                 elif not isReturnAnnotationNone(node):
                     violations.append(v201)
 
         if docstringHasReturnSection and not (hasReturnStmt or hasReturnAnno):
             violations.append(v202)
 
+        if self.checkReturnTypes:
+            if hasReturnAnno:
+                returnAnno = ReturnAnnotation(unparseAnnotation(node.returns))
+            else:
+                returnAnno = ReturnAnnotation(annotation=None)
+
+            if docstringHasReturnSection:
+                returnSec: List[ReturnArg] = doc.returnSection
+            else:
+                returnSec = []
+
+            if (
+                returnSec == []  # no return section in docstring
+                and returnAnno.annotation == 'None'  # `-> None` in signature
+                and not self.requireReturnSectionWhenReturningNone
+            ):
+                return violations  # no need to check return type hints at all
+
+            if returnSec == [] and hasGenAsRetAnno:
+                # This is because if the return annotation is `Generator[...]`,
+                # we don't need a "Returns" section. (Instead, we need a
+                # "Yields" section in the docstring.) Therefore, we don't need
+                # to check for DOC203 violations.
+                return violations
+
+            if self.style == 'numpy':
+                # If the return annotation is a tuple (such as Tuple[int, str]),
+                # we consider both in the docstring to be a valid style:
+                #
+                # Option 1:
+                # >    Returns
+                # >    -------
+                # >    Tuple[int, str]
+                # >        ...
+                #
+                # Option 2:
+                # >    Returns
+                # >    -------
+                # >    int
+                # >        ...
+                # >    str
+                # >        ...
+                #
+                #  This is why we are comparing both the decomposed annotation
+                #  types and the original annotation type
+                returnAnnoItems: List[str] = returnAnno.decompose()
+                returnAnnoInList: List[str] = returnAnno.putAnnotationInList()
+
+                returnSecTypes: List[str] = [
+                    stripQuotes(_.argType) for _ in returnSec
+                ]
+
+                if returnAnnoInList != returnSecTypes:
+                    if len(returnAnnoItems) != len(returnSec):
+                        msg = f'Return annotation has {len(returnAnnoItems)}'
+                        msg += ' type(s); docstring return section has'
+                        msg += f' {len(returnSec)} type(s).'
+                        violations.append(v203.appendMoreMsg(moreMsg=msg))
+                    else:
+                        if returnSecTypes != returnAnnoItems:
+                            msg1 = (
+                                f'Return annotation types: {returnAnnoItems}; '
+                            )
+                            msg2 = f'docstring return section types: {returnSecTypes}'
+                            violations.append(v203.appendMoreMsg(msg1 + msg2))
+
+            else:  # Google style
+                # The Google docstring style does not allow (or at least does
+                # not encourage) splitting tuple return types (such as
+                # Tuple[int, str, bool]) into individual types (int, str, and
+                # bool).
+                # Therefore, in Google-style docstrings, people should always
+                # use one compound style for tuples.
+
+                if len(returnSec) > 0:
+                    retArgType = stripQuotes(returnSec[0].argType)
+                    if returnAnno.annotation is None:
+                        msg = 'Return annotation has 0 type(s); docstring'
+                        msg += ' return section has 1 type(s).'
+                        violations.append(v203.appendMoreMsg(moreMsg=msg))
+                    elif retArgType != returnAnno.annotation:
+                        msg = 'Return annotation types: '
+                        msg += str([returnAnno.annotation]) + '; '
+                        msg += 'docstring return section types: '
+                        msg += str([retArgType])
+                        violations.append(v203.appendMoreMsg(moreMsg=msg))
+                else:
+                    if bool(returnAnno.annotation):  # not empty str or not None
+                        msg = 'Return annotation has 1 type(s); docstring'
+                        msg += ' return section has 0 type(s).'
+                        violations.append(v203.appendMoreMsg(moreMsg=msg))
+
         return violations
 
     @classmethod
     def checkReturnsAndYieldsInClassConstructor(
             cls,
             parent: ast.ClassDef,
             doc: Doc,
@@ -475,17 +577,16 @@
                     line=parent.lineno,
                     msgPrefix=f'Class `{parent.name}`:',
                 )
             )
 
         return violations
 
-    @classmethod
     def checkYields(
-            cls,
+            self,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
             doc: Doc,
     ) -> List[Violation]:
         """Check violations on 'yield' statements or 'Generator' annotation"""
         violations: List[Violation] = []
 
@@ -506,21 +607,21 @@
                 violations.append(v401)
 
             if hasYieldStmt:
                 violations.append(v402)
 
         if docstringHasYieldsSection:
             if not hasYieldStmt and not hasGenAsRetAnno:
-                violations.append(v403)
+                if not self.isAbstractMethod:
+                    violations.append(v403)
 
         return violations
 
-    @classmethod
     def checkRaises(
-            cls,
+            self,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
             doc: Doc,
     ) -> List[Violation]:
         """Check violations on 'raise' statements"""
         violations: List[Violation] = []
 
@@ -533,10 +634,11 @@
         docstringHasRaisesSection: bool = doc.hasRaisesSection
         hasRaiseStmt: bool = hasRaiseStatements(node)
 
         if hasRaiseStmt and not docstringHasRaisesSection:
             violations.append(v501)
 
         if not hasRaiseStmt and docstringHasRaisesSection:
-            violations.append(v502)
+            if not self.isAbstractMethod:
+                violations.append(v502)
 
         return violations
```

### Comparing `pydoclint-0.0.9/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.1.0/pydoclint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -175,14 +175,15 @@
 
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
+| `DOC203` | Return type(s) in the docstring not consistent with the return annotation                            |
 
 Note on `DOC201`: Methods with `@property` as its last decorator do not need to
 have a return section.
 
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
 | Code     | Explanation                                                                                             |
```

### Comparing `pydoclint-0.0.9/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.1.0/pydoclint.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,13 +18,16 @@
 pydoclint/utils/annotation.py
 pydoclint/utils/arg.py
 pydoclint/utils/astTypes.py
 pydoclint/utils/doc.py
 pydoclint/utils/generic.py
 pydoclint/utils/internal_error.py
 pydoclint/utils/method_type.py
+pydoclint/utils/return_anno.py
+pydoclint/utils/return_arg.py
 pydoclint/utils/return_yield_raise.py
 pydoclint/utils/unparser.py
 pydoclint/utils/violation.py
 pydoclint/utils/walk.py
+tests/test_generic.py
 tests/test_main.py
 tests/test_parse_config.py
```

### Comparing `pydoclint-0.0.9/setup.cfg` & `pydoclint-0.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.9
+version = 0.1.0
 description = A Python docstring linter that checks arguments, returns, yields, and raises sections
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.0.9/tests/test_main.py` & `pydoclint-0.1.0/tests/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,82 +105,151 @@
 }
 
 
 @pytest.mark.parametrize(
     'style, filename, checkArgOrder',
     list(
         itertools.product(
-            ['numpy', 'google'],
+            ['numpy', 'google', 'sphinx'],
             ['function.py', 'classmethod.py', 'method.py', 'staticmethod.py'],
             [True, False],
         ),
     ),
 )
 def testArguments(
         style: str,
         filename: str,
-        checkArgOrder: str,
+        checkArgOrder: bool,
 ) -> None:
     expectedViolations: List[str] = expectedViolationsLookup[checkArgOrder]
 
     expectedViolationsCopy = copy.deepcopy(expectedViolations)
     if filename == 'function.py':
         _tweakViolationMsgForFunctions(expectedViolationsCopy)
 
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/args/{filename}',
         checkArgOrder=checkArgOrder,
+        checkReturnTypes=False,  # because this test only checks arguments
         style=style,
     )
     assert list(map(str, violations)) == expectedViolationsCopy
 
 
 @pytest.mark.parametrize(
     'style, filename',
     list(
         itertools.product(
-            ['numpy', 'google'],
+            ['numpy', 'google', 'sphinx'],
             ['function.py', 'classmethod.py', 'method.py', 'staticmethod.py'],
         ),
     ),
 )
 def testReturns(style: str, filename: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/returns/{filename}',
-        skipCheckingShortDocstrings=False,
+        skipCheckingShortDocstrings=True,
         requireReturnSectionWhenReturningNone=True,
         style=style,
     )
 
     expectedViolations: List[str] = [
-        'DOC201: Method `MyClass.func1_3` does not have a return section in '
-        'docstring ',
-        'DOC201: Method `MyClass.func1_5` does not have a return section in '
-        'docstring ',
         'DOC201: Method `MyClass.func1_6` does not have a return section in '
         'docstring ',
+        'DOC203: Method `MyClass.func1_6` return type(s) in docstring not consistent with '
+        'the return annotation. Return annotation has 1 type(s); docstring '
+        'return section has 0 type(s).',
         'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
         'function signature. ',
         'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
         'function arguments. (Or could be other formatting issues: '
         'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
         'the docstring: [arg2: float, arg3: str]. Arguments in the docstring but not '
         'in the function signature: [arg1: int].',
-        'DOC201: Function `func52` does not have a return section in docstring ',
+        'DOC203: Method `MyClass.func2` return type(s) in docstring not consistent with the '
+        "return annotation. Return annotation types: ['int | list[float]']; docstring "
+        "return section types: ['int']",
+        'DOC203: Method `MyClass.func4` return type(s) in docstring not consistent with the '
+        "return annotation. Return annotation types: ['int']; docstring return "
+        "section types: ['float']",
         'DOC202: Method `MyClass.func6` has a return section in docstring, but there '
         'are no return statements or annotations ',
+        'DOC203: Method `MyClass.func6` return type(s) in docstring not consistent with the '
+        'return annotation. Return annotation has 0 type(s); docstring return section '
+        'has 1 type(s).',
+        'DOC203: Method `MyClass.func62` return type(s) in docstring not consistent with the '
+        "return annotation. Return annotation types: ['float']; docstring return "
+        "section types: ['int']",
+        'DOC203: Method `MyClass.func7` return type(s) in docstring not consistent with the '
+        'return annotation. Return annotation has 0 type(s); docstring return section '
+        'has 1 type(s).',
     ]
 
+    if style == 'google':
+        expectedViolations.append(
+            'DOC203: Method `MyClass.func82` return type(s) in docstring not consistent with '
+            "the return annotation. Return annotation types: ['Tuple[int, bool]']; "
+            "docstring return section types: ['int']"
+        )
+
+    if style == 'sphinx':
+        expectedViolations.append(
+            'DOC203: Method `MyClass.func82` return type(s) in docstring not consistent with '
+            "the return annotation. Return annotation types: ['Tuple[int, bool]']; "
+            "docstring return section types: ['bool']"
+        )
+
+    expectedViolations.extend([
+        'DOC202: Method `MyClass.func101` has a return section in docstring, but '
+        'there are no return statements or annotations ',
+        'DOC203: Method `MyClass.func101` return type(s) in docstring not consistent '
+        'with the return annotation. Return annotation has 0 type(s); docstring '
+        'return section has 1 type(s).',
+        'DOC201: Function `inner101` does not have a return section in docstring ',
+        'DOC203: Function `inner101` return type(s) in docstring not consistent with '
+        'the return annotation. Return annotation has 1 type(s); docstring return '
+        'section has 0 type(s).',
+    ])
+
     expectedViolationsCopy = copy.deepcopy(expectedViolations)
     if filename == 'function.py':
         _tweakViolationMsgForFunctions(expectedViolationsCopy)
 
     assert list(map(str, violations)) == expectedViolationsCopy
 
 
+@pytest.mark.parametrize(
+    'style, require',
+    list(
+        itertools.product(
+            ['numpy', 'google', 'sphinx'],
+            [True, False],
+        ),
+    ),
+)
+def testReturns_returningNone(style: str, require: bool) -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / f'{style}/returning_none/cases.py',
+        skipCheckingShortDocstrings=True,
+        requireReturnSectionWhenReturningNone=require,
+        style=style,
+    )
+    expectedViolationsCopy = (
+        [
+            'DOC201: Function `func` does not have a return section in docstring ',
+            'DOC203: Function `func` return type(s) in docstring not consistent with the '
+            'return annotation. Return annotation has 1 type(s); docstring return section '
+            'has 0 type(s).',
+        ]
+        if require
+        else []
+    )
+    assert list(map(str, violations)) == expectedViolationsCopy
+
+
 def _tweakViolationMsgForFunctions(expectedViolationsCopy: List[str]) -> None:
     for i in range(len(expectedViolationsCopy)):
         expectedViolationsCopy[i] = expectedViolationsCopy[i].replace(
             'Method `MyClass.', 'Function `'
         )
 
 
@@ -192,15 +261,14 @@
     'DOC107: Function `func3`: The option `--type-hints-in-signature` is `True` '
     'but not all args in the signature have type hints ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
-    'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 expected_skipCheckingShortDocstrings_False = [
     'DOC101: Function `func1`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC106: Function `func1`: The option `--type-hints-in-signature` is `True` '
     'but there are no type hints in the signature ',
@@ -209,68 +277,76 @@
     'DOC109: Function `func1`: The option `--type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func1`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
     'function signature but not in the docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func1` does not have a return section in docstring ',
+    'DOC203: Function `func1` return type(s) in docstring not consistent with the '
+    'return annotation. Return annotation has 1 type(s); docstring return section '
+    'has 0 type(s).',
     'DOC101: Function `func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC106: Function `func2`: The option `--type-hints-in-signature` is `True` '
     'but there are no type hints in the signature ',
     'DOC107: Function `func2`: The option `--type-hints-in-signature` is `True` '
     'but not all args in the signature have type hints ',
     'DOC109: Function `func2`: The option `--type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func2`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
     'function signature but not in the docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func2` does not have a return section in docstring ',
+    'DOC203: Function `func2` return type(s) in docstring not consistent with the '
+    'return annotation. Return annotation has 1 type(s); docstring return section '
+    'has 0 type(s).',
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC106: Function `func3`: The option `--type-hints-in-signature` is `True` '
     'but there are no type hints in the signature ',
     'DOC107: Function `func3`: The option `--type-hints-in-signature` is `True` '
     'but not all args in the signature have type hints ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
     'function signature but not in the docstring: [arg1: , arg2: , arg3: ]. '
     'Arguments in the docstring but not in the function signature: [var1: int, '
     'var2: str].',
-    'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 
 @pytest.mark.parametrize(
     'style, skipCheckingShortDocstrings, expected',
     [
         ('numpy', True, expected_skipCheckingShortDocstrings_True),
         ('numpy', False, expected_skipCheckingShortDocstrings_False),
         ('google', True, expected_skipCheckingShortDocstrings_True),
         ('google', False, expected_skipCheckingShortDocstrings_False),
+        ('sphinx', True, expected_skipCheckingShortDocstrings_True),
+        ('sphinx', False, expected_skipCheckingShortDocstrings_False),
     ],
 )
 def testSkipCheckingShortDocstrings(
         style: str,
         skipCheckingShortDocstrings: bool,
         expected: List[str],
 ) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/short_docstrings/cases.py',
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
+        checkReturnTypes=True,
         style=style,
     )
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize(
     'style',
-    ['numpy', 'google'],
+    ['numpy', 'google', 'sphinx'],
 )
 def testInit(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/init/init.py',
         style=style,
     )
     expected = [
@@ -291,15 +367,15 @@
         'because __init__() cannot return anything ',
     ]
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize(
     'style',
-    ['numpy', 'google'],
+    ['numpy', 'google', 'sphinx'],
 )
 def testAllowInitDocstring(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/allow_init_docstring/cases.py',
         style=style,
         allowInitDocstring=True,
     )
@@ -324,18 +400,19 @@
         'because __init__() cannot yield anything ',
         'DOC403: Method `D.__init__` has a "Yields" section in the docstring, but '
         'there are no "yield" statements or a Generator return annotation ',
     ]
     assert list(map(str, violations)) == expected
 
 
-@pytest.mark.parametrize('style', ['numpy', 'google'])
+@pytest.mark.parametrize('style', ['numpy', 'google', 'sphinx'])
 def testYields(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/yields/cases.py',
+        checkReturnTypes=False,
         style=style,
     )
     expected = [
         'DOC401: Method `A.method1` returns a Generator, but the docstring does not '
         'have a "Yields" section ',
         'DOC402: Method `A.method1` has "yield" statements, but the docstring does '
         'not have a "Yields" section ',
@@ -354,47 +431,61 @@
         'DOC402: Method `A.method8c` has "yield" statements, but the docstring does '
         'not have a "Yields" section ',
         'DOC402: Method `A.method8d` has "yield" statements, but the docstring does '
         'not have a "Yields" section ',
         'DOC201: Method `A.zipLists2` does not have a return section in docstring ',
         'DOC403: Method `A.zipLists2` has a "Yields" section in the docstring, but '
         'there are no "yield" statements or a Generator return annotation ',
+        'DOC402: Function `inner9b` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
+        'DOC201: Method `A.method9c` does not have a return section in docstring ',
+        'DOC403: Method `A.method9c` has a "Yields" section in the docstring, but '
+        'there are no "yield" statements or a Generator return annotation ',
+        'DOC402: Method `A.method9d` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
+        'DOC402: Function `inner9d` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
     ]
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize(
     'style, skipRaisesCheck',
     itertools.product(
-        ['numpy', 'google'],
+        ['numpy', 'google', 'sphinx'],
         [False, True],
     ),
 )
 def testRaises(style: str, skipRaisesCheck: bool) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/raises/cases.py',
         skipCheckingRaises=skipRaisesCheck,
         typeHintsInSignature=False,
         typeHintsInDocstring=False,
+        checkReturnTypes=False,
         style=style,
     )
     expected0 = [
         'DOC501: Method `B.func1` has "raise" statements, but the docstring does not '
         'have a "Raises" section ',
         'DOC502: Method `B.func5` has a "Raises" section in the docstring, but there '
         'are not "raise" statements in the body ',
         'DOC502: Method `B.func7` has a "Raises" section in the docstring, but there '
         'are not "raise" statements in the body ',
+        'DOC502: Method `B.func9a` has a "Raises" section in the docstring, but there '
+        'are not "raise" statements in the body ',
+        'DOC501: Function `inner9a` has "raise" statements, but the docstring does '
+        'not have a "Raises" section ',
     ]
     expected1 = []
     expected = expected1 if skipRaisesCheck else expected0
     assert list(map(str, violations)) == expected
 
 
-@pytest.mark.parametrize('style', ['numpy', 'google'])
+@pytest.mark.parametrize('style', ['numpy', 'google', 'sphinx'])
 def testStarsInArgumentList(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/star_args/cases.py',
         style=style,
     )
     expected = [
         'DOC110: Function `func2`: The option `--type-hints-in-docstring` is `True` '
@@ -424,26 +515,48 @@
         'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [**kwargs: , *args: , arg1: float, arg2: str]. Arguments in the '
         'docstring but not in the function signature: [arg1: int, arg2: dict].',
     ]
     assert list(map(str, violations)) == expected
 
 
+@pytest.mark.parametrize('style', ['numpy', 'google', 'sphinx'])
+def testStarsInArgumentList2(style: str) -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / f'{style}/star_args/cases2.py',
+        typeHintsInSignature=True,
+        typeHintsInDocstring=False,
+        allowInitDocstring=True,
+        style=style,
+    )
+    expected = []
+    assert list(map(str, violations)) == expected
+
+
 def testParsingErrors_google() -> None:
     violations = _checkFile(
         filename=DATA_DIR / 'google/parsing_errors/cases.py',
         style='google',
     )
     expected = [
         'DOC001: Function/method `__init__`: Potential formatting errors in '
         "docstring. Error message: Expected a colon in 'arg1'."
     ]
     assert list(map(str, violations)) == expected
 
 
+def testParsingErrors_sphinx() -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / 'sphinx/parsing_errors/cases.py',
+        style='sphinx',
+    )
+    expected = []  # not sure how to craft docstrings with parsing errors yet
+    assert list(map(str, violations)) == expected
+
+
 def testParsingErrors_numpy() -> None:
     violations = _checkFile(
         filename=DATA_DIR / 'numpy/parsing_errors/cases.py',
         typeHintsInDocstring=False,
         typeHintsInSignature=False,
         style='numpy',
     )
@@ -455,25 +568,26 @@
     ]
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize(
     'style, rrs',
     itertools.product(
-        ['numpy', 'google'],
+        ['numpy', 'google', 'sphinx'],
         [False, True],
     ),
 )
 def testNoReturnSection(
         style: str,
         rrs: bool,
 ) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/no_return_section/cases.py',
         style=style,
+        checkReturnTypes=False,
         requireReturnSectionWhenReturningNone=rrs,
     )
     expected_lookup = {
         True: [
             'DOC201: Function `func1` does not have a return section in docstring ',
             'DOC201: Function `func2` does not have a return section in docstring ',
             'DOC201: Function `func3` does not have a return section in docstring ',
@@ -488,30 +602,67 @@
         ],
     }
     assert list(map(str, violations)) == expected_lookup[rrs]
 
 
 @pytest.mark.parametrize(
     'style',
-    ['numpy', 'google'],
+    ['numpy', 'google', 'sphinx'],
 )
 def testPropertyMethod(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/property_method/cases.py',
         style=style,
         skipCheckingShortDocstrings=True,
     )
     expected = []
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize(
+    'style, checkReturnTypes',
+    itertools.product(
+        ['numpy', 'google', 'sphinx'],
+        [False, True],
+    ),
+)
+def testAbstractMethod(style: str, checkReturnTypes: bool) -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / f'{style}/abstract_method/cases.py',
+        checkReturnTypes=checkReturnTypes,
+        style=style,
+    )
+    if checkReturnTypes:
+        expected = [
+            'DOC201: Method `AbstractClass.another_abstract_method` does not have a '
+            'return section in docstring ',
+            'DOC203: Method `AbstractClass.another_abstract_method` return type(s) in '
+            'docstring not consistent with the return annotation. Return annotation has 1 '
+            'type(s); docstring return section has 0 type(s).',
+            'DOC201: Method `AbstractClass.third_abstract_method` does not have a return '
+            'section in docstring ',
+            'DOC203: Method `AbstractClass.third_abstract_method` return type(s) in '
+            'docstring not consistent with the return annotation. Return annotation has 1 '
+            'type(s); docstring return section has 0 type(s).',
+        ]
+    else:
+        expected = [
+            'DOC201: Method `AbstractClass.another_abstract_method` does not have a '
+            'return section in docstring ',
+            'DOC201: Method `AbstractClass.third_abstract_method` does not have a return '
+            'section in docstring ',
+        ]
+
+    assert list(map(str, violations)) == expected
+
+
+@pytest.mark.parametrize(
     'style, typeHintsInDocstring, typeHintsInSignature',
     itertools.product(
-        ['numpy', 'google'],
+        ['numpy', 'google', 'sphinx'],
         [False, True],
         [False, True],
     ),
 )
 def testTypeHintChecking(
         style: str,
         typeHintsInDocstring: bool,
```

### Comparing `pydoclint-0.0.9/tests/test_parse_config.py` & `pydoclint-0.1.0/tests/test_parse_config.py`

 * *Files identical despite different names*

