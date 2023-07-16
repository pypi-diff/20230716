# Comparing `tmp/python2verilog-0.0.1.tar.gz` & `tmp/python2verilog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python2verilog-0.0.1.tar", last modified: Thu Jul 13 19:41:18 2023, max compression
+gzip compressed data, was "python2verilog-0.0.2.tar", last modified: Sun Jul 16 07:08:58 2023, max compression
```

## Comparing `python2verilog-0.0.1.tar` & `python2verilog-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:41:18.363170 python2verilog-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-13 19:41:18.363170 python2verilog-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-13 19:41:03.000000 python2verilog-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-13 19:41:03.000000 python2verilog-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:41:18.359169 python2verilog-0.0.1/python2verilog/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 19:41:03.000000 python2verilog-0.0.1/python2verilog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:41:18.363170 python2verilog-0.0.1/python2verilog/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 19:41:03.000000 python2verilog-0.0.1/python2verilog/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-13 19:41:03.000000 python2verilog-0.0.1/python2verilog/backend/ast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:41:18.363170 python2verilog-0.0.1/python2verilog/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 19:41:03.000000 python2verilog-0.0.1/python2verilog/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-07-13 19:41:03.000000 python2verilog-0.0.1/python2verilog/frontend/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-13 19:41:03.000000 python2verilog-0.0.1/python2verilog/frontend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:41:18.363170 python2verilog-0.0.1/python2verilog/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:41:03.000000 python2verilog-0.0.1/python2verilog/optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:41:18.363170 python2verilog-0.0.1/python2verilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-13 19:41:18.000000 python2verilog-0.0.1/python2verilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-13 19:41:18.000000 python2verilog-0.0.1/python2verilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:41:18.000000 python2verilog-0.0.1/python2verilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:41:18.000000 python2verilog-0.0.1/python2verilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:41:18.363170 python2verilog-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-16 07:08:58.059761 python2verilog-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-16 07:08:41.000000 python2verilog-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-16 07:08:41.000000 python2verilog-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.055761 python2verilog-0.0.2/python2verilog/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15689 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/generator2ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/optimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.055761 python2verilog-0.0.2/python2verilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 07:08:58.059761 python2verilog-0.0.2/setup.cfg
```

### Comparing `python2verilog-0.0.1/PKG-INFO` & `python2verilog-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
@@ -27,45 +27,104 @@
 **Warning**: Variables must be unique, i.e. variables do not have block scope, e.g. the following modifies global `i`:
 
 ```python
 for i in range(10):
     pass
 ```
 
-## Doing Your Own Conversion
-`python3 tests/parsers/new_generator.py <name>` to create new test case and prepare template Python file.
+## Sample Usage
+`pip install python2verilog`
 
-`python3 -m pytest --verbose` to run tests / generate the module, testbench, visualizations, dumps, and expected/actual outputs.
+### Basic usage
+`python3 -m python2verilog.convert generator.py`
+`python3 -m python2verilog.convert generator.py -c "(1, 2, 3, 4)"`
+
+### More Complex Usage
+
+## Testing
+
+### Requirements
+
+Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
+
+Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
+
+Python: `python3 -m pip install -r tests/requirements.txt`
+
+### Creating New Test
+
+To create a new test case and set up configs, run `python3 tests/frontend/new_generator.py <name>`.
+
+### Running Tests
+
+To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
+Those files will be stored in `tests/frontend/data/generator/<name>/`.
 
 ## Tested Generations
-The outputs of the Python script tests can be found [here](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
 
-Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md).
+The outputs of the Python script tests can be found [as a github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
 
-I recommend [EDA Playground](https://edaplayground.com/) or [Icarus Verilog](https://github.com/steveicarus/iverilog) for testing the verilog code. Refer to the [github action](.github/workflows/python-package.yml) to see how to setup testing with Icarus Verilog.
+Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md), more up-to-date ones can be found in the artifact.
 
 ## For Developers
+
 Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
 
 Architecture is based on [LLVM](https://llvm.org/).
 
 To setup pre-commit, run `pre-commit install`.
 
 ### Epics
 
-- Create a Verilog AST representation (lots of samples online) to better optimize (mostly end statements)
-- Add `valid` signal and then generate testbenches that test multiple cases
+- Support arrays
 
 ## Docs
 
 - Generate `.html` docs: `bash docs/generate.sh`
 - Live docs: `python3 -m pydoc -b`
 
 ## Random Planning, Design, and Notes
 
+### Potential API
+
+```python
+import python2verilog as p2v
+import ast
+
+func = ast.parse(code).body[0]
+
+ir = p2v.from_python_get_ir(func.body) # returns an ir node for the root of the body
+
+# Optimization passes
+ir = p2v.optimizations.replace_single_item_cases(ir)
+ir = p2v.optimizations.remove_nesting(ir)
+ir = p2v.optimizations.combine_statements(ir)
+for i in dir(p2v.optimizations): # Do one pass of every optimization
+  item = getattr(pv2.optimizations, i)
+    if callable(item):
+      ir = item(ir)
+
+verilog = p2v.Verilog()
+verilog.from_python_do_setup(func) # module I/O is dependent on Python
+verilog.from_ir_fill_body(ir) # fills the body
+
+# whether has valid or done signal,
+# whether initialization is always happening or only on start,
+# verilog sim name
+verilog.config(has_valid=True, has_done=True, lazy_start=True, verilog_sim="iverilog")
+
+with open(f"{verilog.get_module_name()}.sv", mode="w") as module:
+  module.write(verilog.get_module())
+with open(f"{verilog.get_module_name()}_tb.sv", mode="w") as tb:
+  tb.write(verilog.get_testbench())
+
+print(verilog.get_verilog_run_cmd())
+assert verilog.test_outputs() # checks if verilog and python output same
+```
+
 ### Rectangle Filled
 
 ```python
 def draw_rectangle(s_x, s_y, height, width) -> tuple[int, int]:
     for i0 in range(0, width):
         for i1 in range(0, height):
             yield (s_x + i1, s_y + i0)
```

### Comparing `python2verilog-0.0.1/README.md` & `python2verilog-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -15,45 +15,104 @@
 **Warning**: Variables must be unique, i.e. variables do not have block scope, e.g. the following modifies global `i`:
 
 ```python
 for i in range(10):
     pass
 ```
 
-## Doing Your Own Conversion
-`python3 tests/parsers/new_generator.py <name>` to create new test case and prepare template Python file.
+## Sample Usage
+`pip install python2verilog`
 
-`python3 -m pytest --verbose` to run tests / generate the module, testbench, visualizations, dumps, and expected/actual outputs.
+### Basic usage
+`python3 -m python2verilog.convert generator.py`
+`python3 -m python2verilog.convert generator.py -c "(1, 2, 3, 4)"`
+
+### More Complex Usage
+
+## Testing
+
+### Requirements
+
+Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
+
+Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
+
+Python: `python3 -m pip install -r tests/requirements.txt`
+
+### Creating New Test
+
+To create a new test case and set up configs, run `python3 tests/frontend/new_generator.py <name>`.
+
+### Running Tests
+
+To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
+Those files will be stored in `tests/frontend/data/generator/<name>/`.
 
 ## Tested Generations
-The outputs of the Python script tests can be found [here](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
 
-Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md).
+The outputs of the Python script tests can be found [as a github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
 
-I recommend [EDA Playground](https://edaplayground.com/) or [Icarus Verilog](https://github.com/steveicarus/iverilog) for testing the verilog code. Refer to the [github action](.github/workflows/python-package.yml) to see how to setup testing with Icarus Verilog.
+Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md), more up-to-date ones can be found in the artifact.
 
 ## For Developers
+
 Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
 
 Architecture is based on [LLVM](https://llvm.org/).
 
 To setup pre-commit, run `pre-commit install`.
 
 ### Epics
 
-- Create a Verilog AST representation (lots of samples online) to better optimize (mostly end statements)
-- Add `valid` signal and then generate testbenches that test multiple cases
+- Support arrays
 
 ## Docs
 
 - Generate `.html` docs: `bash docs/generate.sh`
 - Live docs: `python3 -m pydoc -b`
 
 ## Random Planning, Design, and Notes
 
+### Potential API
+
+```python
+import python2verilog as p2v
+import ast
+
+func = ast.parse(code).body[0]
+
+ir = p2v.from_python_get_ir(func.body) # returns an ir node for the root of the body
+
+# Optimization passes
+ir = p2v.optimizations.replace_single_item_cases(ir)
+ir = p2v.optimizations.remove_nesting(ir)
+ir = p2v.optimizations.combine_statements(ir)
+for i in dir(p2v.optimizations): # Do one pass of every optimization
+  item = getattr(pv2.optimizations, i)
+    if callable(item):
+      ir = item(ir)
+
+verilog = p2v.Verilog()
+verilog.from_python_do_setup(func) # module I/O is dependent on Python
+verilog.from_ir_fill_body(ir) # fills the body
+
+# whether has valid or done signal,
+# whether initialization is always happening or only on start,
+# verilog sim name
+verilog.config(has_valid=True, has_done=True, lazy_start=True, verilog_sim="iverilog")
+
+with open(f"{verilog.get_module_name()}.sv", mode="w") as module:
+  module.write(verilog.get_module())
+with open(f"{verilog.get_module_name()}_tb.sv", mode="w") as tb:
+  tb.write(verilog.get_testbench())
+
+print(verilog.get_verilog_run_cmd())
+assert verilog.test_outputs() # checks if verilog and python output same
+```
+
 ### Rectangle Filled
 
 ```python
 def draw_rectangle(s_x, s_y, height, width) -> tuple[int, int]:
     for i0 in range(0, width):
         for i1 in range(0, height):
             yield (s_x + i1, s_y + i0)
```

### Comparing `python2verilog-0.0.1/pyproject.toml` & `python2verilog-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python2verilog"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Kerry Wang", email = "kerrywang369@gmail.com" }]
 description = "Converts a subset of python generator functions into synthesizable sequential SystemVerilog"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `python2verilog-0.0.1/python2verilog/frontend/generator.py` & `python2verilog-0.0.2/python2verilog/frontend/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     def stringify_always_block():
         """
         always @(posedge _clock) begin
         end
         """
         return (Lines(["always @(posedge _clock) begin"]), Lines(["end"]))
 
+    def __str__(self):
+        return self.generate_verilog().to_string()
+
     def generate_verilog(self, indent: int = 0):
         """
         Generates the verilog (does the most work, calls other functions)
         """
         stmt_lines = self.parse_statements(
             self.root.body, prefix="", end_stmts=Lines(["_done = 1;"])
         )
@@ -119,14 +122,15 @@
         end_lines += "endmodule"
         return (start_lines, end_lines)
 
     def __init__(self, root: ast.FunctionDef):
         """
         Initializes the parser, does quick setup work
         """
+        assert isinstance(root, ast.FunctionDef)
         self.name = root.name
         self.yield_vars = self.generate_return_vars(root.returns, "")
         self.unique_name_counter = 0
         self.global_vars: dict[str, str] = {}
         self.root = root
 
     def parse_for(self, node: ast.For, prefix: str = ""):
@@ -407,16 +411,18 @@
             operator = ">"
         elif isinstance(node.ops[0], ast.GtE):
             operator = ">="
         else:
             raise TypeError(
                 "Error: unknown operator", type(node.ops[0]), ast.dump(node.ops[0])
             )
-        return f"{self.parse_expression(node.left)} {operator} \
-            {self.parse_expression(node.comparators[0])}"
+        return (
+            f"{self.parse_expression(node.left)} {operator}"
+            f" {self.parse_expression(node.comparators[0])}"
+        )
 
     def parse_while(self, node: ast.While, prefix: str = ""):
         """
         Converts while loop to a while-true-if-break loop
         """
         conditional = (
             Lines(
```

### Comparing `python2verilog-0.0.1/python2verilog/frontend/utils.py` & `python2verilog-0.0.2/python2verilog/frontend/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
 
     @staticmethod
     def assert_no_newline(stringable: any):
         """
         Asserts no newline character in str(stringable)
         """
-        assert str(stringable).find("\n") == -1, "Lines should not contain \\n"
+        assert str(stringable).find("\n") == -1, "Newline in Lines: " + str(stringable)
 
     def __init__(self, data: list[str] | str = None):
         if data is None:
             self.lines = []
         elif isinstance(data, str):
             self.assert_no_newline(data)
             self.lines = [data]
```

### Comparing `python2verilog-0.0.1/python2verilog.egg-info/PKG-INFO` & `python2verilog-0.0.2/python2verilog.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
@@ -27,45 +27,104 @@
 **Warning**: Variables must be unique, i.e. variables do not have block scope, e.g. the following modifies global `i`:
 
 ```python
 for i in range(10):
     pass
 ```
 
-## Doing Your Own Conversion
-`python3 tests/parsers/new_generator.py <name>` to create new test case and prepare template Python file.
+## Sample Usage
+`pip install python2verilog`
 
-`python3 -m pytest --verbose` to run tests / generate the module, testbench, visualizations, dumps, and expected/actual outputs.
+### Basic usage
+`python3 -m python2verilog.convert generator.py`
+`python3 -m python2verilog.convert generator.py -c "(1, 2, 3, 4)"`
+
+### More Complex Usage
+
+## Testing
+
+### Requirements
+
+Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
+
+Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
+
+Python: `python3 -m pip install -r tests/requirements.txt`
+
+### Creating New Test
+
+To create a new test case and set up configs, run `python3 tests/frontend/new_generator.py <name>`.
+
+### Running Tests
+
+To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
+Those files will be stored in `tests/frontend/data/generator/<name>/`.
 
 ## Tested Generations
-The outputs of the Python script tests can be found [here](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
 
-Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md).
+The outputs of the Python script tests can be found [as a github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
 
-I recommend [EDA Playground](https://edaplayground.com/) or [Icarus Verilog](https://github.com/steveicarus/iverilog) for testing the verilog code. Refer to the [github action](.github/workflows/python-package.yml) to see how to setup testing with Icarus Verilog.
+Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md), more up-to-date ones can be found in the artifact.
 
 ## For Developers
+
 Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
 
 Architecture is based on [LLVM](https://llvm.org/).
 
 To setup pre-commit, run `pre-commit install`.
 
 ### Epics
 
-- Create a Verilog AST representation (lots of samples online) to better optimize (mostly end statements)
-- Add `valid` signal and then generate testbenches that test multiple cases
+- Support arrays
 
 ## Docs
 
 - Generate `.html` docs: `bash docs/generate.sh`
 - Live docs: `python3 -m pydoc -b`
 
 ## Random Planning, Design, and Notes
 
+### Potential API
+
+```python
+import python2verilog as p2v
+import ast
+
+func = ast.parse(code).body[0]
+
+ir = p2v.from_python_get_ir(func.body) # returns an ir node for the root of the body
+
+# Optimization passes
+ir = p2v.optimizations.replace_single_item_cases(ir)
+ir = p2v.optimizations.remove_nesting(ir)
+ir = p2v.optimizations.combine_statements(ir)
+for i in dir(p2v.optimizations): # Do one pass of every optimization
+  item = getattr(pv2.optimizations, i)
+    if callable(item):
+      ir = item(ir)
+
+verilog = p2v.Verilog()
+verilog.from_python_do_setup(func) # module I/O is dependent on Python
+verilog.from_ir_fill_body(ir) # fills the body
+
+# whether has valid or done signal,
+# whether initialization is always happening or only on start,
+# verilog sim name
+verilog.config(has_valid=True, has_done=True, lazy_start=True, verilog_sim="iverilog")
+
+with open(f"{verilog.get_module_name()}.sv", mode="w") as module:
+  module.write(verilog.get_module())
+with open(f"{verilog.get_module_name()}_tb.sv", mode="w") as tb:
+  tb.write(verilog.get_testbench())
+
+print(verilog.get_verilog_run_cmd())
+assert verilog.test_outputs() # checks if verilog and python output same
+```
+
 ### Rectangle Filled
 
 ```python
 def draw_rectangle(s_x, s_y, height, width) -> tuple[int, int]:
     for i0 in range(0, width):
         for i1 in range(0, height):
             yield (s_x + i1, s_y + i0)
```

