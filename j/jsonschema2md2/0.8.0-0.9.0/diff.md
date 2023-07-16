# Comparing `tmp/jsonschema2md2-0.8.0.tar.gz` & `tmp/jsonschema2md2-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema2md2-0.8.0.tar", max compression
+gzip compressed data, was "jsonschema2md2-0.9.0.tar", max compression
```

## Comparing `jsonschema2md2-0.8.0.tar` & `jsonschema2md2-0.9.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-04-20 16:03:56.297427 jsonschema2md2-0.8.0/LICENSE
--rw-r--r--   0        0        0     2993 2023-04-20 16:03:56.297427 jsonschema2md2-0.8.0/README.md
--rw-r--r--   0        0        0    13526 2023-04-20 16:03:56.297427 jsonschema2md2-0.8.0/jsonschema2md2/__init__.py
--rw-r--r--   0        0        0     1940 2023-04-20 16:05:40.779130 jsonschema2md2-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4227 1970-01-01 00:00:00.000000 jsonschema2md2-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-16 09:36:27.977427 jsonschema2md2-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2899 2023-07-16 09:36:27.977427 jsonschema2md2-0.9.0/README.md
+-rw-r--r--   0        0        0    13527 2023-07-16 09:38:29.294790 jsonschema2md2-0.9.0/jsonschema2md2/__init__.py
+-rw-r--r--   0        0        0     1905 2023-07-16 09:38:34.966856 jsonschema2md2-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 jsonschema2md2-0.9.0/PKG-INFO
```

### Comparing `jsonschema2md2-0.8.0/LICENSE` & `jsonschema2md2-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema2md2-0.8.0/README.md` & `jsonschema2md2-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # jsonschema2md
 
 [![](https://flat.badgen.net/pypi/v/jsonschema2md?icon=pypi)](https://pypi.org/project/jsonschema2md)
-[![](https://flat.badgen.net/github/release/ralfg/jsonschema2md)](https://github.com/ralfg/jsonschema2md/releases)
-[![](https://flat.badgen.net/github/checks/ralfg/jsonschema2md/)](https://github.com/ralfg/jsonschema2md/actions)
-[![](https://flat.badgen.net/codecov/c/github/ralfg/jsonschema2md)](https://codecov.io/gh/RalfG/jsonschema2md)
-![](https://flat.badgen.net/github/last-commit/ralfg/jsonschema2md)
-![](https://flat.badgen.net/github/license/ralfg/jsonschema2md)
+[![](https://flat.badgen.net/github/release/sbrunner/jsonschema2md)](https://github.com/sbrunner/jsonschema2md/releases)
+[![](https://flat.badgen.net/github/checks/sbrunner/jsonschema2md/)](https://github.com/sbrunner/jsonschema2md/actions)
+![](https://flat.badgen.net/github/last-commit/sbrunner/jsonschema2md)
+![](https://flat.badgen.net/github/license/sbrunner/jsonschema2md)
 
 _Convert JSON Schemas to simple, human-readable Markdown documentation._
 
 ---
 
 For example:
 
@@ -40,15 +39,15 @@
 > _JSON Schema for a person object._
 >
 > ## Properties
 >
 > - **`firstName`** _(string)_: The person's first name.
 > - **`lastName`** _(string)_: The person's last name.
 
-See the [examples](https://github.com/RalfG/jsonschema2md/tree/master/examples)
+See the [examples](https://github.com/sbrunner/jsonschema2md/tree/master/examples)
 directory for more elaborate examples.
 
 ---
 
 ## Installation
 
 Install with pip
@@ -78,47 +77,47 @@
 with open("./examples/food.json", "r") as json_file:
     md_lines = parser.parse_schema(json.load(json_file))
 print(''.join(md_lines))
 ```
 
 ### Options
 
-- `examples_as_yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:
+- `examples-as-yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:
   `False`)
-- `show_examples`: Parse examples for only the main object, only properties, or all.
+- `show-examples`: Parse examples for only the main object, only properties, or all.
   (`str`, default `all`, options: `object`, `properties`, `all`)
 
 ## pre-commit hook
 
 You can use the pre-commit hook with:
 
 ```yaml
 repos:
-  - repo: https://github.com/sbrunner/jsonschema2md2
+  - repo: https://github.com/sbrunner/jsonschema2md
+    rev: <version> # Use the ref you want to point at
     hooks:
       - id: jsonschema2md
-        rev: <version> # Use the ref you want to point at
         files: schema.json
         args:
           - --pre-commit
           - schema.json
           - schema.md
 ```
 
 ## Contributing
 
 Bugs, questions or suggestions? Feel free to post an issue in the
-[issue tracker](https://github.com/sbrunner/jsonschema2md2/issues/) or to make a pull
+[issue tracker](https://github.com/sbrunner/jsonschema2md/issues/) or to make a pull
 request! See
-[Contributing.md](https://github.com/sbrunner/jsonschema2md2/blob/master/CONTRIBUTING.md)
+[Contributing.md](https://github.com/sbrunner/jsonschema2md/blob/master/CONTRIBUTING.md)
 for more info.
 
 Install the pre-commit hooks:
 
 ```bash
 pip install pre-commit
 pre-commit install --allow-missing-config
 ```
 
 ## Changelog
 
-See [Changelog.md](https://github.com/RalfG/jsonschema2md/blob/master/CHANGELOG.md).
+See [Changelog.md](https://github.com/sbrunner/jsonschema2md/blob/master/CHANGELOG.md).
```

### Comparing `jsonschema2md2-0.8.0/jsonschema2md2/__init__.py` & `jsonschema2md2-0.9.0/jsonschema2md2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 class Parser:
     """
     JSON Schema to Markdown parser.
 
     Examples
     --------
-    >>> import jsonschema2md
-    >>> parser = jsonschema2md.Parser()
+    >>> import jsonschema2md2
+    >>> parser = jsonschema2md2.Parser()
     >>> md_lines = parser.parse_schema(json.load(input_json))
     """
 
     tab_size = 2
 
     def __init__(self, examples_as_yaml: bool = False, show_examples: str = "all"):
         """
@@ -95,15 +95,14 @@
             description_line.append(f"Must be one of: `{json.dumps(obj['enum'])}`.")
         if "additionalProperties" in obj:
             if obj["additionalProperties"]:
                 description_line.append("Can contain additional properties.")
             else:
                 description_line.append("Cannot contain additional properties.")
         if "$ref" in obj:
-
             description_line.append(f"Refer to *[{obj['$ref']}](#{obj['$ref'][2:]})*.")
         if "default" in obj:
             description_line.append(f"Default: `{json.dumps(obj['default'])}`.")
 
         # Only add start colon if items were added
         if description_line:
             description_line.insert(0, ":")
```

### Comparing `jsonschema2md2-0.8.0/pyproject.toml` & `jsonschema2md2-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,45 +3,44 @@
 target-version = ['py37']
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "jsonschema2md2"
-version = "0.8.0"
+version = "0.9.0"
 description = "Convert JSON Schema to human-readable Markdown documentation"
 authors = ["Ralf Gabriels <ralfg@hotmail.be>", "Matt Graham <matthew.m.graham@gmail.com>"]
 maintainers = ["Stéphane Brunner <stephane.brunner@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-repository = "https://github.com/sbrunner/jsonschema2md2"
+repository = "https://github.com/sbrunner/jsonschema2md"
 keywords = ["JSON Schema", "Markdown", "Converter", "Parser", "Documentation"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Documentation",
     "Topic :: Software Development :: Documentation",
 ]
 
 [tool.poetry.scripts]
-jsonschema2md = 'jsonschema2md2:main'
+jsonschema2md2 = 'jsonschema2md2:main'
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
-importlib_metadata = { version = "6.1.0", python = "<3.8" }
 PyYAML = "6.0"
 
-[tool.poetry.dev-dependencies]
-prospector = { version = "1.9.0", extras = ["with_bandit", "with_mypy", "with_pyroma"] }
-pytest = "6.0.1"
-pytest-cov = "2.10.1"
-pydocstyle = "5.1.1"
+[tool.poetry.group.dev.dependencies]
+prospector = { version = "1.10.2", extras = ["with_bandit", "with_mypy", "with_pyroma"] }
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
+prospector-profile-duplicated = "0.1.0"
 
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
     "poetry-dynamic-versioning[plugin]>=0.19.0",
     "poetry-plugin-tweak-dependencies-version",
 ]
```

### Comparing `jsonschema2md2-0.8.0/PKG-INFO` & `jsonschema2md2-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: jsonschema2md2
-Version: 0.8.0
+Version: 0.9.0
 Summary: Convert JSON Schema to human-readable Markdown documentation
-Home-page: https://github.com/sbrunner/jsonschema2md2
+Home-page: https://github.com/sbrunner/jsonschema2md
 License: Apache-2.0
 Keywords: JSON Schema,Markdown,Converter,Parser,Documentation
 Author: Ralf Gabriels
 Author-email: ralfg@hotmail.be
 Maintainer: Stéphane Brunner
 Maintainer-email: stephane.brunner@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
@@ -15,30 +15,27 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: importlib_metadata (>=6.0.0,<7.0.0) ; python_version < "3.8"
-Project-URL: Repository, https://github.com/sbrunner/jsonschema2md2
+Project-URL: Repository, https://github.com/sbrunner/jsonschema2md
 Description-Content-Type: text/markdown
 
 # jsonschema2md
 
 [![](https://flat.badgen.net/pypi/v/jsonschema2md?icon=pypi)](https://pypi.org/project/jsonschema2md)
-[![](https://flat.badgen.net/github/release/ralfg/jsonschema2md)](https://github.com/ralfg/jsonschema2md/releases)
-[![](https://flat.badgen.net/github/checks/ralfg/jsonschema2md/)](https://github.com/ralfg/jsonschema2md/actions)
-[![](https://flat.badgen.net/codecov/c/github/ralfg/jsonschema2md)](https://codecov.io/gh/RalfG/jsonschema2md)
-![](https://flat.badgen.net/github/last-commit/ralfg/jsonschema2md)
-![](https://flat.badgen.net/github/license/ralfg/jsonschema2md)
+[![](https://flat.badgen.net/github/release/sbrunner/jsonschema2md)](https://github.com/sbrunner/jsonschema2md/releases)
+[![](https://flat.badgen.net/github/checks/sbrunner/jsonschema2md/)](https://github.com/sbrunner/jsonschema2md/actions)
+![](https://flat.badgen.net/github/last-commit/sbrunner/jsonschema2md)
+![](https://flat.badgen.net/github/license/sbrunner/jsonschema2md)
 
 _Convert JSON Schemas to simple, human-readable Markdown documentation._
 
 ---
 
 For example:
 
@@ -69,15 +66,15 @@
 > _JSON Schema for a person object._
 >
 > ## Properties
 >
 > - **`firstName`** _(string)_: The person's first name.
 > - **`lastName`** _(string)_: The person's last name.
 
-See the [examples](https://github.com/RalfG/jsonschema2md/tree/master/examples)
+See the [examples](https://github.com/sbrunner/jsonschema2md/tree/master/examples)
 directory for more elaborate examples.
 
 ---
 
 ## Installation
 
 Install with pip
@@ -107,48 +104,48 @@
 with open("./examples/food.json", "r") as json_file:
     md_lines = parser.parse_schema(json.load(json_file))
 print(''.join(md_lines))
 ```
 
 ### Options
 
-- `examples_as_yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:
+- `examples-as-yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:
   `False`)
-- `show_examples`: Parse examples for only the main object, only properties, or all.
+- `show-examples`: Parse examples for only the main object, only properties, or all.
   (`str`, default `all`, options: `object`, `properties`, `all`)
 
 ## pre-commit hook
 
 You can use the pre-commit hook with:
 
 ```yaml
 repos:
-  - repo: https://github.com/sbrunner/jsonschema2md2
+  - repo: https://github.com/sbrunner/jsonschema2md
+    rev: <version> # Use the ref you want to point at
     hooks:
       - id: jsonschema2md
-        rev: <version> # Use the ref you want to point at
         files: schema.json
         args:
           - --pre-commit
           - schema.json
           - schema.md
 ```
 
 ## Contributing
 
 Bugs, questions or suggestions? Feel free to post an issue in the
-[issue tracker](https://github.com/sbrunner/jsonschema2md2/issues/) or to make a pull
+[issue tracker](https://github.com/sbrunner/jsonschema2md/issues/) or to make a pull
 request! See
-[Contributing.md](https://github.com/sbrunner/jsonschema2md2/blob/master/CONTRIBUTING.md)
+[Contributing.md](https://github.com/sbrunner/jsonschema2md/blob/master/CONTRIBUTING.md)
 for more info.
 
 Install the pre-commit hooks:
 
 ```bash
 pip install pre-commit
 pre-commit install --allow-missing-config
 ```
 
 ## Changelog
 
-See [Changelog.md](https://github.com/RalfG/jsonschema2md/blob/master/CHANGELOG.md).
+See [Changelog.md](https://github.com/sbrunner/jsonschema2md/blob/master/CHANGELOG.md).
```

