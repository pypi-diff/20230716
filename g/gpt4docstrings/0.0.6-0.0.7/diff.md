# Comparing `tmp/gpt4docstrings-0.0.6.tar.gz` & `tmp/gpt4docstrings-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4docstrings-0.0.6.tar", max compression
+gzip compressed data, was "gpt4docstrings-0.0.7.tar", max compression
```

## Comparing `gpt4docstrings-0.0.6.tar` & `gpt4docstrings-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1076 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/LICENSE
--rw-r--r--   0        0        0     2830 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/README.md
--rw-r--r--   0        0        0     2036 2023-07-05 20:16:48.007518 gpt4docstrings-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       83 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/src/gpt4docstrings/__init__.py
--rw-r--r--   0        0        0       75 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/src/gpt4docstrings/__main__.py
--rw-r--r--   0        0        0     1376 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/src/gpt4docstrings/cli.py
--rw-r--r--   0        0        0       67 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/src/gpt4docstrings/docstrings_generators/__init__.py
--rw-r--r--   0        0        0     3420 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
--rw-r--r--   0        0        0     4149 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/src/gpt4docstrings/generate_docstrings.py
--rw-r--r--   0        0        0     1591 2023-07-05 20:16:33.795302 gpt4docstrings-0.0.6/src/gpt4docstrings/utils.py
--rw-r--r--   0        0        0     3867 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2813 2023-07-16 00:25:44.885929 gpt4docstrings-0.0.7/README.md
+-rw-r--r--   0        0        0     2076 2023-07-16 00:25:44.885929 gpt4docstrings-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/__main__.py
+-rw-r--r--   0        0        0     1804 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/ascii_title.py
+-rw-r--r--   0        0        0     1765 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/cli.py
+-rw-r--r--   0        0        0       67 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/docstrings_generators/__init__.py
+-rw-r--r--   0        0        0     5357 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
+-rw-r--r--   0        0        0     7170 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/generate_docstrings.py
+-rw-r--r--   0        0        0     2604 2023-07-16 00:25:29.665900 gpt4docstrings-0.0.7/src/gpt4docstrings/utils.py
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.7/PKG-INFO
```

### Comparing `gpt4docstrings-0.0.6/LICENSE` & `gpt4docstrings-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.6/README.md` & `gpt4docstrings-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -68,10 +68,10 @@
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [file an issue]: https://github.com/MichaelisTrofficus/gpt4docstrings/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
-[license]: https://github.com/MichaelisTrofficus/gpt4docstrings/blob/main/LICENSE
-[contributor guide]: https://github.com/MichaelisTrofficus/gpt4docstrings/blob/main/CONTRIBUTING.md
-[command-line reference]: https://gpt4docstrings.readthedocs.io/en/latest/usage.html
+[license]: https://gpt4docstrings.readthedocs.io/en/latest/license.html
+[contributor guide]: https://gpt4docstrings.readthedocs.io/en/latest/contributing.html#
+[command-line reference]: https://gpt4docstrings.readthedocs.io/en/latest/use_as_cli.html
```

### Comparing `gpt4docstrings-0.0.6/pyproject.toml` & `gpt4docstrings-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt4docstrings"
-version = "0.0.6"
+version = "0.0.7"
 description = "gpt4docstrings"
 authors = ["Miguel Otero Pedrido <miguel.otero.pedrido.1993@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 repository = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 documentation = "https://gpt4docstrings.readthedocs.io"
@@ -18,14 +18,16 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 click = ">=8.0.1"
 redbaron = "^0.9.2"
 openai = "^0.27.8"
 docformatter = "^1.7.3"
 pytest-mock = "^3.11.1"
+tabulate = "^0.9.0"
+colorama = "^0.4.6"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `gpt4docstrings-0.0.6/src/gpt4docstrings/cli.py` & `gpt4docstrings-0.0.7/src/gpt4docstrings/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,21 @@
     "-m",
     "--model",
     type=click.STRING,
     default="gpt-3.5-turbo",
     help="The model to be used by `gpt4docstrings`. By default, `gpt-3.5-turbo`.",
 )
 @click.option(
+    "-s",
+    "--style",
+    type=click.STRING,
+    default="google",
+    help="Docstring style, which must be one of 'google', 'reStructuredText', 'epytext', 'numpy'",
+)
+@click.option(
     "-k",
     "--api_key",
     type=click.STRING,
     default="",
     help="OpenAI's API key. If not provided, `gpt4docstrings` will try to access `OPENAI_API_KEY` environment variable.",
 )
 @click.option(
@@ -29,14 +36,21 @@
         writable=False,
         readable=True,
         resolve_path=True,
     ),
     default=(),
     help="Exclude PATHs of files and/or directories. Multiple `-e/--exclude` invocations supported.",
 )
+@click.option(
+    "-v",
+    "--verbose",
+    type=click.INT,
+    default=0,
+    help="Verbosity parameter. Defaults to 0.",
+)
 @click.help_option("-h", "--help")
 @click.argument(
     "paths",
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=True,
@@ -52,10 +66,12 @@
     if not paths:
         paths = (os.path.abspath(os.getcwd()),)
 
     docstrings_generator = gpt4docstrings.GPT4Docstrings(
         paths=paths,
         excluded=kwargs["exclude"],
         model=kwargs["model"],
+        docstring_style=kwargs["style"],
         api_key=kwargs["api_key"],
+        verbose=kwargs["verbose"],
     )
     docstrings_generator.generate_docstrings()
```

### Comparing `gpt4docstrings-0.0.6/PKG-INFO` & `gpt4docstrings-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: gpt4docstrings
-Version: 0.0.6
+Version: 0.0.7
 Summary: gpt4docstrings
 Home-page: https://github.com/MichaelisTrofficus/gpt4docstrings
 License: MIT
 Author: Miguel Otero Pedrido
 Author-email: miguel.otero.pedrido.1993@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: docformatter (>=1.7.3,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
 Requires-Dist: redbaron (>=0.9.2,<0.10.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Changelog, https://github.com/MichaelisTrofficus/gpt4docstrings/releases
 Project-URL: Documentation, https://gpt4docstrings.readthedocs.io
 Project-URL: Repository, https://github.com/MichaelisTrofficus/gpt4docstrings
 Description-Content-Type: text/markdown
 
 # gpt4docstrings
 
@@ -93,11 +95,11 @@
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [file an issue]: https://github.com/MichaelisTrofficus/gpt4docstrings/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
-[license]: https://github.com/MichaelisTrofficus/gpt4docstrings/blob/main/LICENSE
-[contributor guide]: https://github.com/MichaelisTrofficus/gpt4docstrings/blob/main/CONTRIBUTING.md
-[command-line reference]: https://gpt4docstrings.readthedocs.io/en/latest/usage.html
+[license]: https://gpt4docstrings.readthedocs.io/en/latest/license.html
+[contributor guide]: https://gpt4docstrings.readthedocs.io/en/latest/contributing.html#
+[command-line reference]: https://gpt4docstrings.readthedocs.io/en/latest/use_as_cli.html
```

