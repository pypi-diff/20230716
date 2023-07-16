# Comparing `tmp/mmoran0032-0.1.0-py3-none-any.whl.zip` & `tmp/mmoran0032-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 1553 bytes, number of entries: 6
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-15 17:22 mmoran0032/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 16:48 mmoran0032/cli.py
--rw-r--r--  2.0 unx      633 b- defN 23-Jul-15 18:02 mmoran0032-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 18:02 mmoran0032-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-15 18:02 mmoran0032-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      457 b- defN 23-Jul-15 18:02 mmoran0032-0.1.0.dist-info/RECORD
-6 files, 1215 bytes uncompressed, 717 bytes compressed:  41.0%
+Zip file size: 2156 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-16 00:33 mmoran0032/__init__.py
+-rw-r--r--  2.0 unx      447 b- defN 23-Jul-16 00:28 mmoran0032/cli.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-16 00:36 mmoran0032-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 00:36 mmoran0032-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-16 00:36 mmoran0032-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-16 00:36 mmoran0032-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      557 b- defN 23-Jul-16 00:36 mmoran0032-1.0.0.dist-info/RECORD
+7 files, 2017 bytes uncompressed, 1158 bytes compressed:  42.6%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: mmoran0032/__init__.py
 Comment: 
 
 Filename: mmoran0032/cli.py
 Comment: 
 
-Filename: mmoran0032-0.1.0.dist-info/METADATA
+Filename: mmoran0032-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mmoran0032-0.1.0.dist-info/WHEEL
+Filename: mmoran0032-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mmoran0032-0.1.0.dist-info/top_level.txt
+Filename: mmoran0032-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mmoran0032-0.1.0.dist-info/RECORD
+Filename: mmoran0032-1.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: mmoran0032-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mmoran0032/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "1.0.0"
```

## mmoran0032/cli.py

```diff
@@ -0,0 +1,28 @@
+00000000: 6672 6f6d 2072 6963 6820 696d 706f 7274  from rich import
+00000010: 2070 7269 6e74 0a69 6d70 6f72 7420 7479   print.import ty
+00000020: 7065 720a 0a61 7070 203d 2074 7970 6572  per..app = typer
+00000030: 2e54 7970 6572 2829 0a0a 0a40 6170 702e  .Typer()...@app.
+00000040: 636f 6d6d 616e 6428 290a 6465 6620 6d61  command().def ma
+00000050: 696e 2829 202d 3e20 4e6f 6e65 3a0a 2020  in() -> None:.  
+00000060: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
+00000070: 2022 222c 0a20 2020 2020 2020 2022 4d69   "",.        "Mi
+00000080: 6b65 204d 6f72 616e 222c 0a20 2020 2020  ke Moran",.     
+00000090: 2020 2022 4461 7461 2053 6369 656e 7469     "Data Scienti
+000000a0: 7374 2061 7420 5b62 6f6c 6420 6772 6565  st at [bold gree
+000000b0: 6e5d 4475 6f20 5365 6375 7269 7479 5b2f  n]Duo Security[/
+000000c0: 626f 6c64 2067 7265 656e 5d22 2c0a 2020  bold green]",.  
+000000d0: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
+000000e0: 2020 2245 6d61 696c 203a 696e 636f 6d69    "Email :incomi
+000000f0: 6e67 5f65 6e76 656c 6f70 652d 656d 6f6a  ng_envelope-emoj
+00000100: 693a 2020 2020 2020 206d 696b 6540 6d6b  i:       mike@mk
+00000110: 6d72 6e2e 6465 7622 2c0a 2020 2020 2020  mrn.dev",.      
+00000120: 2020 2247 6974 6c61 6220 3a66 6f78 5f66    "Gitlab :fox_f
+00000130: 6163 652d 656d 6f6a 693a 2020 2020 2020  ace-emoji:      
+00000140: 406d 6d6f 7261 6e30 3033 3222 2c0a 2020  @mmoran0032",.  
+00000150: 2020 2020 2020 224d 6f73 7420 736f 6369        "Most soci
+00000160: 616c 733a 2020 406d 6d6f 7261 6e30 3033  als:  @mmoran003
+00000170: 3222 2c0a 2020 2020 2020 2020 2222 2c0a  2",.        "",.
+00000180: 2020 2020 2020 2020 7365 703d 225c 6e22          sep="\n"
+00000190: 2c0a 2020 2020 290a 0a0a 6966 205f 5f6e  ,.    )...if __n
+000001a0: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+000001b0: 5f5f 223a 0a20 2020 2061 7070 2829 0a    __":.    app().
```

## Comparing `mmoran0032-0.1.0.dist-info/METADATA` & `mmoran0032-1.0.0.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: mmoran0032
-Version: 0.1.0
+Version: 1.0.0
 Summary: whoami in Python
 Author-email: Mike Moran <mike@mkmrn.dev>
+Project-URL: homepage, https://mkmrn.dev
+Project-URL: repository, https://gitlab.com/mmoran0032/mmoran0032
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: rich
 Requires-Dist: typer[all]
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov (>=4.0.0) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.0.0) ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: wheel ; extra == 'dev'
 
 # mmoran0032
 
+![PyPI](https://img.shields.io/pypi/v/mmoran0032)
+
 `whoami` but for me and within Python for all to see.
```

