# Comparing `tmp/jsonschema2md-0.4.0.tar.gz` & `tmp/jsonschema2md-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema2md-0.4.0.tar", max compression
+gzip compressed data, was "jsonschema2md-0.9.0.tar", max compression
```

## Comparing `jsonschema2md-0.4.0.tar` & `jsonschema2md-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11357 2022-03-04 17:37:10.655156 jsonschema2md-0.4.0/LICENSE
--rw-r--r--   0        0        0     2568 2022-03-04 17:37:10.655156 jsonschema2md-0.4.0/README.md
--rw-r--r--   0        0        0    10465 2022-03-04 17:37:10.655156 jsonschema2md-0.4.0/jsonschema2md.py
--rw-r--r--   0        0        0     1063 2022-03-04 17:37:10.655156 jsonschema2md-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3530 2022-03-04 17:37:18.939476 jsonschema2md-0.4.0/setup.py
--rw-r--r--   0        0        0     3728 2022-03-04 17:37:18.939832 jsonschema2md-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-16 09:36:27.977427 jsonschema2md-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2899 2023-07-16 09:36:27.977427 jsonschema2md-0.9.0/README.md
+-rw-r--r--   0        0        0    13524 2023-07-16 09:36:27.977427 jsonschema2md-0.9.0/jsonschema2md/__init__.py
+-rw-r--r--   0        0        0     1902 2023-07-16 09:38:24.962740 jsonschema2md-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 jsonschema2md-0.9.0/PKG-INFO
```

### Comparing `jsonschema2md-0.4.0/LICENSE` & `jsonschema2md-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema2md-0.4.0/README.md` & `jsonschema2md-0.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,73 @@
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
 
-
-*Convert JSON Schemas to simple, human-readable Markdown documentation.*
+_Convert JSON Schemas to simple, human-readable Markdown documentation._
 
 ---
 
 For example:
+
 ```json
 {
-    "$id": "https://example.com/person.schema.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "title": "Person",
-    "description": "JSON Schema for a person object.",
-    "type": "object",
-    "properties": {
-      "firstName": {
-        "type": "string",
-        "description": "The person's first name."
-      },
-      "lastName": {
-        "type": "string",
-        "description": "The person's last name."
-      }
+  "$id": "https://example.com/person.schema.json",
+  "$schema": "http://json-schema.org/draft-07/schema#",
+  "title": "Person",
+  "description": "JSON Schema for a person object.",
+  "type": "object",
+  "properties": {
+    "firstName": {
+      "type": "string",
+      "description": "The person's first name."
+    },
+    "lastName": {
+      "type": "string",
+      "description": "The person's last name."
     }
   }
+}
 ```
 
 will be converted to:
 
 > # Person
-> *JSON Schema for a person object.*
+>
+> _JSON Schema for a person object._
+>
 > ## Properties
 >
-> - **`firstName`** *(string)*: The person's first name.
-> - **`lastName`** *(string)*: The person's last name.
+> - **`firstName`** _(string)_: The person's first name.
+> - **`lastName`** _(string)_: The person's last name.
 
-See the [examples](https://github.com/RalfG/jsonschema2md/tree/master/examples)
+See the [examples](https://github.com/sbrunner/jsonschema2md/tree/master/examples)
 directory for more elaborate examples.
 
 ---
 
 ## Installation
 
 Install with pip
 
 ```sh
 pip install jsonschema2md
 ```
 
-
 ## Usage
 
 ### From the CLI
 
 ```sh
 jsonschema2md [OPTIONS] <input.json> <output.md>
 ```
 
-
 ### From Python
 
 ```python
 import json
 import jsonschema2md
 
 parser = jsonschema2md.Parser(
@@ -76,28 +75,49 @@
     show_examples="all",
 )
 with open("./examples/food.json", "r") as json_file:
     md_lines = parser.parse_schema(json.load(json_file))
 print(''.join(md_lines))
 ```
 
-
 ### Options
 
-- `examples_as_yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:
+- `examples-as-yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:
   `False`)
-- `show_examples`: Parse examples for only the main object, only properties, or all.
-(`str`, default `all`, options: `object`, `properties`, `all`)
+- `show-examples`: Parse examples for only the main object, only properties, or all.
+  (`str`, default `all`, options: `object`, `properties`, `all`)
+
+## pre-commit hook
+
+You can use the pre-commit hook with:
 
+```yaml
+repos:
+  - repo: https://github.com/sbrunner/jsonschema2md
+    rev: <version> # Use the ref you want to point at
+    hooks:
+      - id: jsonschema2md
+        files: schema.json
+        args:
+          - --pre-commit
+          - schema.json
+          - schema.md
+```
 
 ## Contributing
 
 Bugs, questions or suggestions? Feel free to post an issue in the
-[issue tracker](https://github.com/RalfG/jsonschema2md/issues/) or to make a pull
+[issue tracker](https://github.com/sbrunner/jsonschema2md/issues/) or to make a pull
 request! See
-[Contributing.md](https://github.com/RalfG/jsonschema2md/blob/master/CONTRIBUTING.md)
+[Contributing.md](https://github.com/sbrunner/jsonschema2md/blob/master/CONTRIBUTING.md)
 for more info.
 
+Install the pre-commit hooks:
+
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
 
 ## Changelog
 
-See [Changelog.md](https://github.com/RalfG/jsonschema2md/blob/master/CHANGELOG.md).
+See [Changelog.md](https://github.com/sbrunner/jsonschema2md/blob/master/CHANGELOG.md).
```

### Comparing `jsonschema2md-0.4.0/jsonschema2md.py` & `jsonschema2md-0.9.0/jsonschema2md/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Convert JSON Schema to Markdown documentation."""
 
 
-__author__ = "Ralf Gabriels"
-__email__ = "ralfg@hotmail.be"
+__author__ = "Stéphane Brunner"
+__email__ = "stephane.brunner@gmail.com"
 __license__ = "Apache-2.0"
 
 
 try:
     from importlib.metadata import version
 except ImportError:
     from importlib_metadata import version
 
+import argparse
 import io
 import json
 import re
-from typing import Dict, Optional, Sequence
+import subprocess  # nosec
+import sys
+from typing import Dict, List, Optional, Sequence, Union
 
-import click
 import yaml
 
-__version__ = version('jsonschema2md')
+__version__ = version("jsonschema2md")
 
 
 class Parser:
     """
     JSON Schema to Markdown parser.
 
     Examples
@@ -31,19 +33,15 @@
     >>> import jsonschema2md
     >>> parser = jsonschema2md.Parser()
     >>> md_lines = parser.parse_schema(json.load(input_json))
     """
 
     tab_size = 2
 
-    def __init__(
-        self,
-        examples_as_yaml: bool = False,
-        show_examples: str = "all"
-    ):
+    def __init__(self, examples_as_yaml: bool = False, show_examples: str = "all"):
         """
         Setup JSON Schema to Markdown parser.
 
         Parameters
         ----------
         examples_as_yaml : bool, default False
             Parse examples in YAML-format instead of JSON.
@@ -60,159 +58,197 @@
             self.show_examples = show_examples
         else:
             raise ValueError(
                 f"`show_examples` option should be one of "
                 f"`{valid_show_examples_options}`; `{show_examples}` was passed."
             )
 
-    def _construct_description_line(
-        self,
-        obj: Dict,
-        add_type: bool = False
-    ) -> Sequence[str]:
+    def _construct_description_line(self, obj: Dict, add_type: bool = False) -> Sequence[str]:
         """Construct description line of property, definition, or item."""
         description_line = []
 
         if "description" in obj:
             ending = "" if re.search(r"[.?!;]$", obj["description"]) else "."
             description_line.append(f"{obj['description']}{ending}")
         if add_type:
             if "type" in obj:
                 description_line.append(f"Must be of type *{obj['type']}*.")
         if "minimum" in obj:
             description_line.append(f"Minimum: `{obj['minimum']}`.")
+        if "exclusiveMinimum" in obj:
+            description_line.append(f"Exclusive minimum: `{obj['exclusiveMinimum']}`.")
         if "maximum" in obj:
             description_line.append(f"Maximum: `{obj['maximum']}`.")
+        if "exclusiveMaximum" in obj:
+            description_line.append(f"Exclusive maximum: `{obj['exclusiveMaximum']}`.")
+        if "minItems" in obj or "maxItems" in obj:
+            length_description = "Length must be "
+            if "minItems" in obj and "maxItems" not in obj:
+                length_description += f"at least {obj['minItems']}."
+            elif "maxItems" in obj and "minItems" not in obj:
+                length_description += f"at most {obj['maxItems']}."
+            elif obj["minItems"] == obj["maxItems"]:
+                length_description += f"equal to {obj['minItems']}."
+            else:
+                length_description += f"between {obj['minItems']} and {obj['maxItems']} (inclusive)."
+            description_line.append(length_description)
         if "enum" in obj:
-            description_line.append(f"Must be one of: `{obj['enum']}`.")
+            description_line.append(f"Must be one of: `{json.dumps(obj['enum'])}`.")
         if "additionalProperties" in obj:
             if obj["additionalProperties"]:
                 description_line.append("Can contain additional properties.")
             else:
                 description_line.append("Cannot contain additional properties.")
         if "$ref" in obj:
-            description_line.append(f"Refer to *{obj['$ref']}*.")
+            description_line.append(f"Refer to *[{obj['$ref']}](#{obj['$ref'][2:]})*.")
         if "default" in obj:
-            description_line.append(f"Default: `{obj['default']}`.")
+            description_line.append(f"Default: `{json.dumps(obj['default'])}`.")
 
         # Only add start colon if items were added
         if description_line:
             description_line.insert(0, ":")
 
         return description_line
 
-    def _construct_examples(
-        self,
-        obj: Dict,
-        indent_level: int = 0,
-        add_header: bool = True
-    ) -> Sequence[str]:
+    def _construct_examples(self, obj: Dict, indent_level: int = 0, add_header: bool = True) -> Sequence[str]:
         def dump_json_with_line_head(obj, line_head, **kwargs):
-            f = io.StringIO(json.dumps(obj, **kwargs))
-            result = [line_head + line for line in f.readlines()]
-            return ''.join(result)
+            result = [line_head + line for line in io.StringIO(json.dumps(obj, **kwargs)).readlines()]
+            return "".join(result)
 
         def dump_yaml_with_line_head(obj, line_head, **kwargs):
-            f = io.StringIO(yaml.dump(obj, **kwargs))
-            result = [line_head + line for line in f.readlines()]
-            return ''.join(result).rstrip()
+            result = [line_head + line for line in io.StringIO(yaml.dump(obj, **kwargs)).readlines()]
+            return "".join(result).rstrip()
 
         example_lines = []
         if "examples" in obj:
             example_indentation = " " * self.tab_size * (indent_level + 1)
             if add_header:
-                example_lines.append(f'\n{example_indentation}Examples:\n')
+                example_lines.append(f"\n{example_indentation}Examples:\n")
             for example in obj["examples"]:
                 if self.examples_as_yaml:
                     lang = "yaml"
                     dump_fn = dump_yaml_with_line_head
                 else:
                     lang = "json"
                     dump_fn = dump_json_with_line_head
-                example_str = dump_fn(
-                    example,
-                    line_head=example_indentation,
-                    indent=4
-                )
+                example_str = dump_fn(example, line_head=example_indentation, indent=4)
                 example_lines.append(
-                    f"{example_indentation}```{lang}\n"
-                    f"{example_str}\n"
-                    f"{example_indentation}```\n\n"
+                    f"{example_indentation}```{lang}\n{example_str}\n{example_indentation}```\n\n"
                 )
         return example_lines
 
     def _parse_object(
         self,
-        obj: Dict,
-        name: str,
+        obj: Union[Dict, List],
+        name: Optional[str],
         name_monospace: bool = True,
-        output_lines: Optional[str] = None,
+        output_lines: Optional[List[str]] = None,
         indent_level: int = 0,
+        path: Optional[List[str]] = None,
+        required: bool = False,
     ) -> Sequence[str]:
         """Parse JSON object and its items, definitions, and properties recursively."""
-        if not isinstance(obj, dict):
-            raise TypeError(
-                f"Non-object type found in properties list: `{name}: {obj}`."
-            )
 
         if not output_lines:
             output_lines = []
 
         indentation = " " * self.tab_size * indent_level
         indentation_items = " " * self.tab_size * (indent_level + 1)
 
+        if isinstance(obj, list):
+            output_lines.append(f"{indentation}- **{name}**:\n")
+
+            for element in obj:
+                output_lines = self._parse_object(
+                    element,
+                    None,
+                    name_monospace=False,
+                    output_lines=output_lines,
+                    indent_level=indent_level + 2,
+                )
+            return output_lines
+
+        if not isinstance(obj, dict):
+            raise TypeError(f"Non-object type found in properties list: `{name}: {obj}`.")
+
         # Construct full description line
         description_line_base = self._construct_description_line(obj)
-        description_line = list(map(lambda line: line.replace("\n\n", "<br>" + indentation_items), description_line_base))
+        description_line = list(
+            map(
+                lambda line: line.replace("\n\n", "<br>" + indentation_items),
+                description_line_base,
+            )
+        )
 
         # Add full line to output
         description_line = " ".join(description_line)
-        obj_type = f" *({obj['type']})*" if "type" in obj else ""
-        name_formatted = f"**`{name}`**" if name_monospace else f"**{name}**"
-        output_lines.append(
-            f"{indentation}- {name_formatted}{obj_type}{description_line}\n"
-        )
+        if name is None:
+            obj_type = f"*{obj['type']}*" if "type" in obj else ""
+            name_formatted = ""
+        else:
+            required_str = ", required" if required else ""
+            obj_type = f" *({obj['type']}{required_str})*" if "type" in obj else ""
+            name_formatted = f"**`{name}`**" if name_monospace else f"**{name}**"
+        anchor = f"<a id=\"{'/'.join(path)}\"></a>" if path else ""
+        output_lines.append(f"{indentation}- {anchor}{name_formatted}{obj_type}{description_line}\n")
+
+        # Recursively parse subschemas following schema composition keywords
+        schema_composition_keyword_map = {
+            "allOf": "All of",
+            "anyOf": "Any of",
+            "oneOf": "One of",
+        }
+        for key, label in schema_composition_keyword_map.items():
+            if key in obj:
+                output_lines.append(f"{indentation_items}- **{label}**\n")
+                for child_obj in obj[key]:
+                    output_lines = self._parse_object(
+                        child_obj,
+                        None,
+                        name_monospace=False,
+                        output_lines=output_lines,
+                        indent_level=indent_level + 2,
+                    )
 
         # Recursively add items and definitions
-        for name in ["items", "definitions"]:
-            if name in obj:
+        for property_name in ["items", "definitions"]:
+            if property_name in obj:
                 output_lines = self._parse_object(
-                    obj[name],
-                    name.capitalize(),
+                    obj[property_name],
+                    property_name.capitalize(),
                     name_monospace=False,
                     output_lines=output_lines,
-                    indent_level=indent_level + 1
+                    indent_level=indent_level + 1,
                 )
 
         # Recursively add additional child properties
         if "additionalProperties" in obj and isinstance(obj["additionalProperties"], dict):
             output_lines = self._parse_object(
                 obj["additionalProperties"],
                 "Additional Properties",
                 name_monospace=False,
                 output_lines=output_lines,
-                indent_level=indent_level + 1
+                indent_level=indent_level + 1,
             )
 
         # Recursively add child properties
-        for name in ["properties", "patternProperties"]:
-            if name in obj:
-                for property_name, property_obj in obj[name].items():
+        for property_name in ["properties", "patternProperties"]:
+            if property_name in obj:
+                for property_name, property_obj in obj[property_name].items():
                     output_lines = self._parse_object(
                         property_obj,
                         property_name,
                         output_lines=output_lines,
                         indent_level=indent_level + 1,
+                        required=property_name in obj.get("required", []),
                     )
 
         # Add examples
         if self.show_examples in ["all", "properties"]:
-            output_lines.extend(
-                self._construct_examples(obj, indent_level=indent_level)
-            )
+            output_lines.extend(self._construct_examples(obj, indent_level=indent_level))
 
         return output_lines
 
     def parse_schema(self, schema_object: Dict) -> Sequence[str]:
         """Parse JSON Schema object to markdown text."""
         output_lines = []
 
@@ -222,75 +258,86 @@
         else:
             output_lines.append("# JSON Schema\n\n")
         if "description" in schema_object:
             output_lines.append(f"*{schema_object['description']}*\n\n")
 
         # Add items
         if "items" in schema_object:
-            output_lines.append(f"## Items\n\n")
-            output_lines.extend(self._parse_object(
-                schema_object["items"],
-                "Items",
-                name_monospace=False
-            ))
+            output_lines.append("## Items\n\n")
+            output_lines.extend(self._parse_object(schema_object["items"], "Items", name_monospace=False))
 
         # Add additional properties
-        if "additionalProperties" in schema_object and isinstance(schema_object["additionalProperties"], dict):
-            output_lines.append(f"## Additional Properties\n\n")
-            output_lines.extend(self._parse_object(
-                schema_object["additionalProperties"],
-                "Additional Properties",
-                name_monospace=False
-            ))
+        if "additionalProperties" in schema_object and isinstance(
+            schema_object["additionalProperties"], dict
+        ):
+            output_lines.append("## Additional Properties\n\n")
+            output_lines.extend(
+                self._parse_object(
+                    schema_object["additionalProperties"],
+                    "Additional Properties",
+                    name_monospace=False,
+                )
+            )
 
         # Add pattern properties
         if "patternProperties" in schema_object:
-            output_lines.append(f"## Pattern Properties\n\n")
+            output_lines.append("## Pattern Properties\n\n")
             for obj_name, obj in schema_object["patternProperties"].items():
                 output_lines.extend(self._parse_object(obj, obj_name))
 
         # Add properties and definitions
         for name in ["properties", "definitions"]:
             if name in schema_object:
                 output_lines.append(f"## {name.capitalize()}\n\n")
                 for obj_name, obj in schema_object[name].items():
-                    output_lines.extend(self._parse_object(obj, obj_name))
+                    path = [name, obj_name] if name == "definitions" else []
+                    output_lines.extend(self._parse_object(obj, obj_name, path=path))
 
         # Add examples
         if "examples" in schema_object and self.show_examples in ["all", "object"]:
             output_lines.append("## Examples\n\n")
-            output_lines.extend(self._construct_examples(
-                schema_object, indent_level=0, add_header=False
-            ))
+            output_lines.extend(self._construct_examples(schema_object, indent_level=0, add_header=False))
 
         return output_lines
 
 
-@click.command()
-@click.version_option(version=__version__)
-@click.argument("input-json", type=click.File("rt"), metavar="<input.json>")
-@click.argument("output-markdown", type=click.File("wt"), metavar="<output.md>")
-@click.option(
-    "--examples-as-yaml",
-    type=bool,
-    default=False,
-    help="Parse examples in YAML-format instead of JSON."
-)
-@click.option(
-    "--show-examples",
-    type=click.Choice(['all', 'properties', 'object'], case_sensitive=False),
-    default='all',
-    help="Parse examples for only the main object, only properties, or all."
-)
-def main(input_json, output_markdown, examples_as_yaml, show_examples):
+def main():
     """Convert JSON Schema to Markdown documentation."""
-    parser = Parser(
-        examples_as_yaml=examples_as_yaml,
-        show_examples=show_examples
+
+    argparser = argparse.ArgumentParser("Convert JSON Schema to Markdown documentation.")
+    argparser.add_argument("--version", action="store_true", help="Show version and exit.")
+    argparser.add_argument(
+        "--pre-commit", action="store_true", help="Run as pre-commit hook after the generation."
+    )
+    argparser.add_argument(
+        "--examples-as-yaml", action="store_true", help="Parse examples in YAML-format instead of JSON."
     )
-    output_md = parser.parse_schema(json.load(input_json))
-    output_markdown.writelines(output_md)
-    click.secho("✔ Successfully parsed schema!", bold=True, fg="green")
+    argparser.add_argument(
+        "--show-examples",
+        choices=["all", "properties", "object"],
+        default="all",
+        help="Parse examples for only the main object, only properties, or all.",
+    )
+    argparser.add_argument("input_json", help="Input JSON file.")
+    argparser.add_argument("output_markdown", help="Output Markdown file.")
+
+    args = argparser.parse_args()
+
+    if args.version:
+        print(__version__)
+        sys.exit(0)
+
+    parser = Parser(examples_as_yaml=args.examples_as_yaml, show_examples=args.show_examples)
+    with open(args.input_json, encoding="utf-8") as input_json:
+        output_md = parser.parse_schema(json.load(input_json))
+
+    with open(args.output_markdown, "w", encoding="utf-8") as output_markdown:
+        output_markdown.writelines(output_md)
+
+    if args.pre_commit:
+        subprocess.run(  # pylint: disable=subprocess-run-check # nosec
+            ["pre-commit", "run", "--color=never", f"--files={args.output_markdown}"]
+        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jsonschema2md-0.4.0/setup.py` & `jsonschema2md-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,151 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-modules = \
-['jsonschema2md']
-install_requires = \
-['PyYAML>=5.1', 'click>=7']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=1,<2']}
-
-entry_points = \
-{'console_scripts': ['jsonschema2md = jsonschema2md:main']}
-
-setup_kwargs = {
-    'name': 'jsonschema2md',
-    'version': '0.4.0',
-    'description': 'Convert JSON Schema to human-readable Markdown documentation',
-    'long_description': '# jsonschema2md\n\n[![](https://flat.badgen.net/pypi/v/jsonschema2md?icon=pypi)](https://pypi.org/project/jsonschema2md)\n[![](https://flat.badgen.net/github/release/ralfg/jsonschema2md)](https://github.com/ralfg/jsonschema2md/releases)\n[![](https://flat.badgen.net/github/checks/ralfg/jsonschema2md/)](https://github.com/ralfg/jsonschema2md/actions)\n[![](https://flat.badgen.net/codecov/c/github/ralfg/jsonschema2md)](https://codecov.io/gh/RalfG/jsonschema2md)\n![](https://flat.badgen.net/github/last-commit/ralfg/jsonschema2md)\n![](https://flat.badgen.net/github/license/ralfg/jsonschema2md)\n\n\n*Convert JSON Schemas to simple, human-readable Markdown documentation.*\n\n---\n\nFor example:\n```json\n{\n    "$id": "https://example.com/person.schema.json",\n    "$schema": "http://json-schema.org/draft-07/schema#",\n    "title": "Person",\n    "description": "JSON Schema for a person object.",\n    "type": "object",\n    "properties": {\n      "firstName": {\n        "type": "string",\n        "description": "The person\'s first name."\n      },\n      "lastName": {\n        "type": "string",\n        "description": "The person\'s last name."\n      }\n    }\n  }\n```\n\nwill be converted to:\n\n> # Person\n> *JSON Schema for a person object.*\n> ## Properties\n>\n> - **`firstName`** *(string)*: The person\'s first name.\n> - **`lastName`** *(string)*: The person\'s last name.\n\nSee the [examples](https://github.com/RalfG/jsonschema2md/tree/master/examples)\ndirectory for more elaborate examples.\n\n---\n\n## Installation\n\nInstall with pip\n\n```sh\npip install jsonschema2md\n```\n\n\n## Usage\n\n### From the CLI\n\n```sh\njsonschema2md [OPTIONS] <input.json> <output.md>\n```\n\n\n### From Python\n\n```python\nimport json\nimport jsonschema2md\n\nparser = jsonschema2md.Parser(\n    examples_as_yaml=False,\n    show_examples="all",\n)\nwith open("./examples/food.json", "r") as json_file:\n    md_lines = parser.parse_schema(json.load(json_file))\nprint(\'\'.join(md_lines))\n```\n\n\n### Options\n\n- `examples_as_yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:\n  `False`)\n- `show_examples`: Parse examples for only the main object, only properties, or all.\n(`str`, default `all`, options: `object`, `properties`, `all`)\n\n\n## Contributing\n\nBugs, questions or suggestions? Feel free to post an issue in the\n[issue tracker](https://github.com/RalfG/jsonschema2md/issues/) or to make a pull\nrequest! See\n[Contributing.md](https://github.com/RalfG/jsonschema2md/blob/master/CONTRIBUTING.md)\nfor more info.\n\n\n## Changelog\n\nSee [Changelog.md](https://github.com/RalfG/jsonschema2md/blob/master/CHANGELOG.md).\n',
-    'author': 'Ralf Gabriels',
-    'author_email': 'ralfg@hotmail.be',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/RalfG/jsonschema2md',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
+Metadata-Version: 2.1
+Name: jsonschema2md
+Version: 0.9.0
+Summary: Convert JSON Schema to human-readable Markdown documentation
+Home-page: https://github.com/sbrunner/jsonschema2md
+License: Apache-2.0
+Keywords: JSON Schema,Markdown,Converter,Parser,Documentation
+Author: Ralf Gabriels
+Author-email: ralfg@hotmail.be
+Maintainer: Stéphane Brunner
+Maintainer-email: stephane.brunner@gmail.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Project-URL: Repository, https://github.com/sbrunner/jsonschema2md
+Description-Content-Type: text/markdown
+
+# jsonschema2md
+
+[![](https://flat.badgen.net/pypi/v/jsonschema2md?icon=pypi)](https://pypi.org/project/jsonschema2md)
+[![](https://flat.badgen.net/github/release/sbrunner/jsonschema2md)](https://github.com/sbrunner/jsonschema2md/releases)
+[![](https://flat.badgen.net/github/checks/sbrunner/jsonschema2md/)](https://github.com/sbrunner/jsonschema2md/actions)
+![](https://flat.badgen.net/github/last-commit/sbrunner/jsonschema2md)
+![](https://flat.badgen.net/github/license/sbrunner/jsonschema2md)
+
+_Convert JSON Schemas to simple, human-readable Markdown documentation._
+
+---
+
+For example:
+
+```json
+{
+  "$id": "https://example.com/person.schema.json",
+  "$schema": "http://json-schema.org/draft-07/schema#",
+  "title": "Person",
+  "description": "JSON Schema for a person object.",
+  "type": "object",
+  "properties": {
+    "firstName": {
+      "type": "string",
+      "description": "The person's first name."
+    },
+    "lastName": {
+      "type": "string",
+      "description": "The person's last name."
+    }
+  }
 }
+```
+
+will be converted to:
+
+> # Person
+>
+> _JSON Schema for a person object._
+>
+> ## Properties
+>
+> - **`firstName`** _(string)_: The person's first name.
+> - **`lastName`** _(string)_: The person's last name.
+
+See the [examples](https://github.com/sbrunner/jsonschema2md/tree/master/examples)
+directory for more elaborate examples.
+
+---
+
+## Installation
+
+Install with pip
+
+```sh
+pip install jsonschema2md
+```
+
+## Usage
+
+### From the CLI
+
+```sh
+jsonschema2md [OPTIONS] <input.json> <output.md>
+```
+
+### From Python
+
+```python
+import json
+import jsonschema2md
+
+parser = jsonschema2md.Parser(
+    examples_as_yaml=False,
+    show_examples="all",
+)
+with open("./examples/food.json", "r") as json_file:
+    md_lines = parser.parse_schema(json.load(json_file))
+print(''.join(md_lines))
+```
+
+### Options
+
+- `examples-as-yaml`: Parse examples in YAML-format instead of JSON. (`bool`, default:
+  `False`)
+- `show-examples`: Parse examples for only the main object, only properties, or all.
+  (`str`, default `all`, options: `object`, `properties`, `all`)
+
+## pre-commit hook
+
+You can use the pre-commit hook with:
+
+```yaml
+repos:
+  - repo: https://github.com/sbrunner/jsonschema2md
+    rev: <version> # Use the ref you want to point at
+    hooks:
+      - id: jsonschema2md
+        files: schema.json
+        args:
+          - --pre-commit
+          - schema.json
+          - schema.md
+```
+
+## Contributing
+
+Bugs, questions or suggestions? Feel free to post an issue in the
+[issue tracker](https://github.com/sbrunner/jsonschema2md/issues/) or to make a pull
+request! See
+[Contributing.md](https://github.com/sbrunner/jsonschema2md/blob/master/CONTRIBUTING.md)
+for more info.
+
+Install the pre-commit hooks:
+
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
+
+## Changelog
 
+See [Changelog.md](https://github.com/sbrunner/jsonschema2md/blob/master/CHANGELOG.md).
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

