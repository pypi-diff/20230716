# Comparing `tmp/TPython-1.8.2-py2.py3-none-any.whl.zip` & `tmp/TPython-1.8.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8493 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       64 b- defN 23-May-12 17:15 tpy/__init__.py
+Zip file size: 8507 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      113 b- defN 23-Jul-16 07:35 tpy/__init__.py
 -rw-rw-rw-  2.0 fat       31 b- defN 23-Feb-20 17:02 tpy/__main__.py
 -rw-rw-rw-  2.0 fat     3961 b- defN 23-May-07 11:56 tpy/config.py
--rw-rw-rw-  2.0 fat      903 b- defN 23-May-07 11:40 tpy/jsonc.py
--rw-rw-rw-  2.0 fat    12054 b- defN 23-May-12 17:15 tpy/tpy.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2482 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       37 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      827 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/RECORD
-11 files, 21535 bytes uncompressed, 7107 bytes compressed:  67.0%
+-rw-rw-rw-  2.0 fat      894 b- defN 23-Jul-16 07:25 tpy/jsonc.py
+-rw-rw-rw-  2.0 fat    11852 b- defN 23-Jul-16 07:35 tpy/tpy.py
+-rw-rw-rw-  2.0 fat     1062 b- defN 23-Jul-16 07:41 TPython-1.8.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2468 b- defN 23-Jul-16 07:41 TPython-1.8.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-16 07:41 TPython-1.8.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       37 b- defN 23-Jul-16 07:41 TPython-1.8.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-16 07:41 TPython-1.8.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      828 b- defN 23-Jul-16 07:41 TPython-1.8.3.dist-info/RECORD
+11 files, 21360 bytes uncompressed, 7121 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tpy/jsonc.py
 Comment: 
 
 Filename: tpy/tpy.py
 Comment: 
 
-Filename: TPython-1.8.2.dist-info/LICENSE
+Filename: TPython-1.8.3.dist-info/LICENSE
 Comment: 
 
-Filename: TPython-1.8.2.dist-info/METADATA
+Filename: TPython-1.8.3.dist-info/METADATA
 Comment: 
 
-Filename: TPython-1.8.2.dist-info/WHEEL
+Filename: TPython-1.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: TPython-1.8.2.dist-info/entry_points.txt
+Filename: TPython-1.8.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: TPython-1.8.2.dist-info/top_level.txt
+Filename: TPython-1.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: TPython-1.8.2.dist-info/RECORD
+Filename: TPython-1.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpy/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .tpy import main
+from .jsonc import parse_file
 
-__all__ = ['main']
-VERSION = '1.8.2'
+__all__ = ['main', 'parse_file']
+__version__ = '1.8.3'
```

## tpy/jsonc.py

```diff
@@ -7,23 +7,23 @@
 class JSONCDecodeError(Exception):
     def __init__(self, msg: str) -> None:
         super().__init__(msg)
 
 # Parser
 def parse_file(file: str) -> dict:
     # Read the contents of the file into a string
-    with open(file, 'r') as f:
+    with open(file) as f:
         content:str = f.read()
 
     # Remove the comments from the string
     json_str: str = re.sub(r'(\/\/[^\n]*)|(/\*[\s\S]*?\*/)', '', content)
 
     # Check for broken comments
     tmp_list: List[str] = re.sub(r'"([^"]*)"', '', json_str).splitlines()
 
     for line_no, element in enumerate(tmp_list, 1):
         if '*/' in element:
             raise JSONCDecodeError(f"expected '/*' before '*/', line {line_no}")
         elif '/*' in element:
             raise JSONCDecodeError(f"expected '*/' after '/*', line {line_no}")
-    
+
     return json.loads(json_str)
```

## tpy/tpy.py

```diff
@@ -19,15 +19,15 @@
     sys.exit('Module not found: colorama')
 
 # Vars
 cell_number: int = 1
 err: bool = False
 ind: bool = False
 namespace: dict = {'__builtins__': __builtins__, '__name__': '__main__', '__doc__': 'Automatically created module for TPython interactive environment', '__package__': None, '__loader__': None, '__spec__': None, '__annotations__': {}}
-VERSION: str = '1.8.2'
+VERSION: str = '1.8.3'
 
 # Exception prettifier
 def exc() -> None:
     name, value = sys.exc_info()[0:2] # type: ignore
     name: str = name.__name__ # type: ignore
     top_bar = "----------------------------------------------------------------------" if os.get_terminal_size().columns > 70 else "-"*os.get_terminal_size().columns
     if name == 'SyntaxError':
@@ -95,18 +95,14 @@
             if pypi_version != VERSION:
                 print(f'{config["colors"]["update"]["text_color"]}Newer version of TPython is available: {config["colors"]["update"]["version_color"]}{pypi_version}')
         except urllib.error.URLError:
             pass
         return
     Thread(target=update_checker).run()
 
-# Entry point
-def main() -> None:
-    global cell_number, err, ind
-
     # Exit function
     def ext(crash_m: str = '', crash: bool = False) -> None:
         columns = os.get_terminal_size().columns
         success_m = 'Process Completed Successfully'
         if crash:
             if config['config']['crash_msg']:
                 msg = crash_m
@@ -117,43 +113,47 @@
             if config['config']['exit_msg']:
                 msg = success_m
                 for i in range((columns-len(success_m))//2):
                     msg = f'{config["colors"]["exit"]["success"]["padding_color"]}-{config["colors"]["exit"]["success"]["text_color"]}{msg}{config["colors"]["exit"]["success"]["padding_color"]}-'
                 print(f'{msg}')
             sys.exit()
 
-    try:
-        # Execute function
-        def execute(code: str, timeit_b: bool = False) -> None:
-            global err, cell_number
-            run = False
-            if timeit_b:
-                try:
-                    time = timeit(code, globals=namespace, number=1)
-                    print(f'{TNP_COLORS["time_text"]["text_color"]}Execution time: {TNP_COLORS["time_text"]["time_color"]}{time}')
-                except Exception:
-                    exc()
-                    err = True
-            else:
-                try:
-                    eval_return = eval(code, namespace)
-                    if eval_return != None:
-                        print(repr(eval_return))
-                    err = False
-                except:
-                    run = True
-                if run:
-                    try:
-                        exec(code, namespace)
-                        err = False
-                    except Exception:
-                        exc()
-                        err = True
-            cell_number += 1
+# Execute function
+def execute(code: str, timeit_b: bool = False, REPL = False) -> None:
+    global err, cell_number
+    run = False
+    if timeit_b:
+        try:
+            time = timeit(code, globals=namespace, number=1)
+            print(f'{TNP_COLORS["time_text"]["text_color"]}Execution time: {TNP_COLORS["time_text"]["time_color"]}{time}')
+        except Exception:
+            exc()
+            err = True
+    else:
+        try:
+            eval_return = eval(code, namespace)
+            if eval_return != None:
+                print(repr(eval_return))
+            err = False
+        except:
+            run = True
+        if run:
+            try:
+                exec(code, namespace)
+                err = False
+            except Exception:
+                exc()
+                err = True
+    cell_number += 1
+
+# Entry point
+def main() -> None:
+    global cell_number, err, ind
 
+    try:
         # Welcome message
         if config['config']['welcome_msg']:
             columns = os.get_terminal_size().columns
             msg = 'TPython'
             columns -= 7
             for i in range(columns//2):
                 msg = f'{config["colors"]["welcome"]["padding_color"]}-{config["colors"]["welcome"]["text_color"]}{msg}{config["colors"]["welcome"]["padding_color"]}-'
```

## Comparing `TPython-1.8.2.dist-info/LICENSE` & `TPython-1.8.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `TPython-1.8.2.dist-info/METADATA` & `TPython-1.8.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TPython
-Version: 1.8.2
+Version: 1.8.3
 Summary: A better python REPL
 Home-page: https://github.com/Techlord210/TPython
 Author: Techlord210
 Author-email: techlord210@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -49,15 +49,14 @@
 ```
 $ pip install TPython
 ```
 
 ## Dependencies
 ```
 colorama
-jsonc_parser
 ```
 
 ## **Usage**
 
 ### **Run**
 ```
 $ tpy
```

