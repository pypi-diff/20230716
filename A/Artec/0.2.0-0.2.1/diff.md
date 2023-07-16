# Comparing `tmp/Artec-0.2.0.tar.gz` & `tmp/Artec-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Artec-0.2.0.tar", last modified: Sat Jul  8 14:32:21 2023, max compression
+gzip compressed data, was "Artec-0.2.1.tar", last modified: Sun Jul 16 20:31:22 2023, max compression
```

## Comparing `Artec-0.2.0.tar` & `Artec-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:32:21.092156 Artec-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:32:21.088155 Artec-0.2.0/Artec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-08 14:32:21.000000 Artec-0.2.0/Artec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-08 14:32:21.000000 Artec-0.2.0/Artec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:32:21.000000 Artec-0.2.0/Artec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-08 14:32:21.000000 Artec-0.2.0/Artec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 14:32:21.000000 Artec-0.2.0/Artec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-08 14:32:11.000000 Artec-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-08 14:32:21.092156 Artec-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-08 14:32:11.000000 Artec-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:32:21.092156 Artec-0.2.0/artec/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-08 14:32:11.000000 Artec-0.2.0/artec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-08 14:32:11.000000 Artec-0.2.0/artec/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-08 14:32:11.000000 Artec-0.2.0/artec/boiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 14:32:11.000000 Artec-0.2.0/artec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-08 14:32:11.000000 Artec-0.2.0/artec/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-08 14:32:11.000000 Artec-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:32:21.092156 Artec-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:32:11.000000 Artec-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:32:21.092156 Artec-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-08 14:32:11.000000 Artec-0.2.0/test/test_boiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-08 14:32:11.000000 Artec-0.2.0/test/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/Artec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-16 20:31:11.000000 Artec-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-16 20:31:22.537473 Artec-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-16 20:31:11.000000 Artec-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/artec/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-16 20:31:11.000000 Artec-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:31:22.537473 Artec-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:31:11.000000 Artec-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-16 20:31:11.000000 Artec-0.2.1/test/test_boiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-16 20:31:11.000000 Artec-0.2.1/test/test_parser.py
```

### Comparing `Artec-0.2.0/LICENSE` & `Artec-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Artec-0.2.0/artec/argparser.py` & `Artec-0.2.1/artec/argparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class list_templates(_VersionAction):
     def __call__(self, parser: ArgumentParser, *args, **kwargs) -> None:
         formatter = parser._get_formatter()
         formatter.add_text(
             "Available templates\n\n"
-            + "\n".join([f"> {key.title()}\t" for key, value in templates.items()])
+            + "\n".join([f"> {key.title()}\t" for key in templates.keys()])
         )
         parser._print_message(formatter.format_help(), sys.stdout)
         parser.exit()
 
 
 class Parser(ArgumentParser):
     def __init__(self, appVersion):
@@ -26,40 +26,43 @@
         epilog = "Examples:\n\tartec -h\n\tartec -o dest\
             \n\tartec -o dest -t python \n\tartec -o dest -s structure.json \n\tartec -o dest -s structure.json -v"
         super().__init__(
             prog, usage, description, epilog, formatter_class=RawTextHelpFormatter
         )
 
     def setup(self):
-        self.add_argument(
-            "-o",
-            "--output-directory",
-            dest="target",
-            help="Target output path where the structure will be created",
-            type=str,
-            required=True,
-        )
-
-        self.add_argument(
+        group = self.add_mutually_exclusive_group()
+        
+        group.add_argument(
             "-s",
             "--source-file",
             dest="source",
             help="Source JSON file containing structure to be created",
             type=str,
             required=False,
         )
-        self.add_argument(
+
+        group.add_argument(
             "-t",
             "--template",
             dest="template",
             help="Uses ready-made templates.",
             required=False,
         )
 
         self.add_argument(
+            "-o",
+            "--output-directory",
+            dest="target",
+            help="Target output path where the structure will be created",
+            type=str,
+            required=True,
+        )
+
+        self.add_argument(
             "-ls",
             "--list-template",
             help="lists all ready-made templates.",
             action=list_templates,
         )
 
 
@@ -76,15 +79,14 @@
             "-V",
             "--version",
             help="Display current version of Artec",
             action="version",
             version=f"{self.prog} {self.appVersion}",
         )
 
-
 def main_args(appVersion) -> Namespace:
     parser = Parser(appVersion)
     parser.setup()
     return parser.parse_args()
 
 
 if __name__ == "__main__":
```

### Comparing `Artec-0.2.0/artec/boiler.py` & `Artec-0.2.1/artec/boiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from .templates import templates, static_list
 
 
 class boiler_builder:
     def __init__(self, source=None, target=None, verbose=False, template=None) -> None:
         self.verbose = verbose
         self.target = target
-        self.template = template
-        if self.template is None:
+        if template is None:
             self.structure = self._source(source)
         else:
             self.structure = self._source_temp(template.lower())
 
     def _source_temp(self, template) -> list[dict[str, str]]:
         try:
             if template in templates:
@@ -28,37 +27,37 @@
 
         except InValidTemplate:
             structure = templates["python"].format(self.target)
         return structure
 
     def _source(self, source) -> list[dict[str, str]]:
         try:
+            if source is None : 
+                raise NoSource(self.verbose)
             if os.path.isfile(source) and source.endswith(".json"):
                 with open(source, "rt", encoding="utf-8") as file_data:
                     structure = static_list(json.load(file_data)).format(self.target)
             else:
                 raise NotJsonFile(self.verbose)
 
         except Exception as e:
-            if not hasattr(e, "errno"):
-                NoSource(self.verbose)
 
             structure = templates["python"].format(self.target)
         return structure
 
     def build(self):
         print("> Creating folder structure: {}\n".format(self.target))
 
         for entry in self.structure:
             for _type, name in entry.items():
                 try:
                     joined = Path(os.path.join(self.target, name))
-                    if _type == "folder":
+                    if "folder" in _type :
                         self._make_folder(joined)
-                    elif _type == "file":
+                    elif "file" in _type :
                         self._make_file(joined)
                     else:
                         raise NotValidJson(self.verbose)
                     print("Created: %s" % joined)
                 except Exception:
                     exit("> Fatal error - exiting...")
```

### Comparing `Artec-0.2.0/artec/exceptions.py` & `Artec-0.2.1/artec/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,31 +4,33 @@
         self.errno = 101
         if not verbose:
             return
         print("> Provided Source isn't valid JSON file")
         print("> Reverting to default structure")
 
 
-class NoSource:
+class NoSource(ValueError):
     def __init__(self, verbose: bool) -> None:
+        super().__init__("> No Source Provided")
+        self.errno = 102
         if not verbose:
             return
         print("> No Source Provided")
         print("> Using default structure")
 
 
 class NotValidJson(KeyError):
     def __init__(self, verbose: bool) -> None:
         super().__init__("> Provided Json file format is incorrect")
-        self.errno = 102
+        self.errno = 103
         if not verbose:
             return
         print("> Provided Json file format is incorrect")
 
 
 class InValidTemplate(KeyError):
     def __init__(self, verbose: bool) -> None:
         super().__init__("> Provided Template argument is invalid")
-        self.errno = 103
+        self.errno = 104
         if not verbose:
             return
         print("> Provided Template argument is invalid")
```

### Comparing `Artec-0.2.0/artec/templates.py` & `Artec-0.2.1/artec/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         {"file": "{}/__init__.py"},
         {"folder": "test"},
         {"file": "test/__init__.py"},
         {"file": "README.md"},
         {"file": "LICENSE"},
         {"file": "setup.py"},
         {"file": "setup.cfg"},
-        {"file": "pyproject.toml"},
+        {"file": "pyproject.toml"}
     ]
 )
 
 NODE_JS = static_list(
     [
         {"folder": "src"},
         {"folder": "src/api"},
```

### Comparing `Artec-0.2.0/pyproject.toml` & `Artec-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+include = ["artec*"]
+exclude = ["img*"]
+
 [project]
 name = "Artec"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="HushmKun", email="HushmKun@outlook.com" },
   { name="Link-", email="bsm.dgdy@gmail.com" },
 ]
 description = "Creates a configurable python project template in a given directory."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `Artec-0.2.0/test/test_boiler.py` & `Artec-0.2.1/test/test_boiler.py`

 * *Files identical despite different names*

### Comparing `Artec-0.2.0/test/test_parser.py` & `Artec-0.2.1/test/test_parser.py`

 * *Files identical despite different names*

