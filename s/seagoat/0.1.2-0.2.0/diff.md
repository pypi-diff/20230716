# Comparing `tmp/seagoat-0.1.2.tar.gz` & `tmp/seagoat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.1.2.tar", max compression
+gzip compressed data, was "seagoat-0.2.0.tar", max compression
```

## Comparing `seagoat-0.1.2.tar` & `seagoat-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-11 18:39:34.444967 seagoat-0.1.2/LICENSE
--rw-r--r--   0        0        0      771 2023-07-11 13:40:38.554139 seagoat-0.1.2/README.md
--rw-r--r--   0        0        0     1217 2023-07-11 19:13:50.387003 seagoat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/__init__.py
--rw-r--r--   0        0        0     1583 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/cache.py
--rw-r--r--   0        0        0      196 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/common.py
--rw-r--r--   0        0        0     4477 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/engine.py
--rw-r--r--   0        0        0     3474 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/file.py
--rw-r--r--   0        0        0     1862 2023-07-11 19:13:50.387003 seagoat-0.1.2/seagoat/main.py
--rw-r--r--   0        0        0     2664 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/repository.py
--rw-r--r--   0        0        0     1626 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/result.py
--rw-r--r--   0        0        0     1876 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1208 2023-07-11 13:40:38.560806 seagoat-0.1.2/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 seagoat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-11 18:39:34.444967 seagoat-0.2.0/LICENSE
+-rw-r--r--   0        0        0      756 2023-07-16 13:37:20.559141 seagoat-0.2.0/README.md
+-rw-r--r--   0        0        0     1335 2023-07-16 13:37:35.452495 seagoat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 13:40:38.560806 seagoat-0.2.0/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/cache.py
+-rw-r--r--   0        0        0     2398 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-07-11 13:40:38.560806 seagoat-0.2.0/seagoat/common.py
+-rw-r--r--   0        0        0     4512 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/result.py
+-rw-r--r--   0        0        0     5058 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/server.py
+-rw-r--r--   0        0        0     1878 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1210 2023-07-16 13:37:20.562474 seagoat-0.2.0/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 seagoat-0.2.0/PKG-INFO
```

### Comparing `seagoat-0.1.2/LICENSE` & `seagoat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.1.2/README.md` & `seagoat-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 
 ### Manually testing
 
 To manually test this app against a code repository,
 you can use the following command:
 
 ```bash
-poetry run python seagoat/main.py ~/path/to/your/repository
+poetry run seagoat ~/path/to/your/repository
 ```
```

### Comparing `seagoat-0.1.2/pyproject.toml` & `seagoat-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.1.2"
+version = "0.2.0"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
-gt = "seagoat.main:seagoat"
-seagoat = "seagoat.main:seagoat"
+gt = "seagoat.cli:seagoat"
+seagoat = "seagoat.cli:seagoat"
+seagoat-server = "seagoat.server:cli"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 chromadb = "^0.3.26"
 gitpython = "^3.1.31"
 tqdm = "^4.65.0"
 appdirs = "^1.4.4"
 click = "^8.1.3"
 prompt-toolkit = "^3.0.38"
 blessed = "^1.20.0"
 pygments = "^2.15.1"
 ripgrepy = "^2.0.0"
 nest-asyncio = "^1.5.6"
+flask = "^2.3.2"
+requests = "^2.31.0"
 
 [virtualenvs]
 in-project = true
 create = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
@@ -34,14 +37,16 @@
 pre-commit = "^3.3.3"
 pyright = "^1.1.314"
 pytest-watch = "^4.2.0"
 freezegun = "^1.2.2"
 syrupy = "^4.0.4"
 pytest-ordering = "^0.6"
 pytest-asyncio = "^0.21.0"
+ipython = "^8.14.0"
+pytest-flask = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 venvPath = "."
```

### Comparing `seagoat-0.1.2/seagoat/cache.py` & `seagoat-0.2.0/seagoat/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import os
 import hashlib
-from pathlib import Path
+import os
 import pickle
-from typing import TypeVar, Generic
+from pathlib import Path
+from typing import Generic
+from typing import TypeVar
 
 import appdirs
 
 T = TypeVar("T")
 
 CACHE_FORMAT_VERSION = 15
```

### Comparing `seagoat-0.1.2/seagoat/engine.py` & `seagoat-0.2.0/seagoat/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
     This module allows you to use seagoat as a library
 """
-
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
+from functools import partial
 from itertools import chain
 from pathlib import Path
-from typing import Dict, List, Set
-from functools import partial
-from typing_extensions import TypedDict
+from typing import Dict
+from typing import List
+from typing import Set
 
-from tqdm import tqdm
 import nest_asyncio
+from tqdm import tqdm
+from typing_extensions import TypedDict
 
 from seagoat.cache import Cache
-from seagoat.repository import Repository
 from seagoat.file import File
-from seagoat.sources import ripgrep
+from seagoat.repository import Repository
 from seagoat.sources import chroma
+from seagoat.sources import ripgrep
 
 
 RepositoryData = TypedDict(
     "RepositoryData",
     {
         "last_analyzed_version_of_branch": Dict[str, str],
         "required_commits": Set[str],
```

### Comparing `seagoat-0.1.2/seagoat/file.py` & `seagoat-0.2.0/seagoat/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import time
 import hashlib
-from typing import List, Literal
+import time
+from typing import List
+from typing import Literal
 
 from chromadb.errors import Dict
 
 
 class File:
     def __init__(self, path: str, absolute_path: str):
         self.path = path
```

### Comparing `seagoat-0.1.2/seagoat/main.py` & `seagoat-0.2.0/seagoat/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,34 @@
-from functools import cache
 import os
 import sys
+from functools import cache
+
 import click
+import requests
 from pygments import highlight
-from pygments.lexers import get_lexer_for_filename
 from pygments.formatters import TerminalFormatter
-from pygments.lexers.javascript import JavascriptLexer, TypeScriptLexer
+from pygments.lexers import get_lexer_for_filename
+from pygments.lexers.javascript import JavascriptLexer
+from pygments.lexers.javascript import TypeScriptLexer
+
+from seagoat.server import get_server_info_file
+from seagoat.server import load_server_info
 
-from seagoat.engine import Engine
+
+def query_server(query, server_address):
+    response = requests.get(f"{server_address}/query/{query}")
+    try:
+        response.raise_for_status()
+    except requests.exceptions.HTTPError as err:
+        print("HTTP error occurred:")
+        print(f"Response code: {response.status_code}")
+        print(f"Error: {err}")
+        print(f"Response body: {response.text}")
+        raise
+    return response.json()["results"]
 
 
 @cache
 def get_highlighted_lines(file_name: str):
     with open(file_name, "r", encoding="utf-8") as source_code_file:
         code = source_code_file.read()
 
@@ -28,37 +45,33 @@
     result = highlight(code, lexer, TerminalFormatter())
 
     return result.splitlines()
 
 
 def print_result_line(result, line, color_enabled):
     if color_enabled:
-        highlighted_lines = get_highlighted_lines(str(result.full_path))
+        highlighted_lines = get_highlighted_lines(str(result["full_path"]))
         print(
-            f"{result.path}:{click.style(str(line), bold=True)}:{highlighted_lines[line - 1]}"
+            f"{result['path']}:{click.style(str(line), bold=True)}:{highlighted_lines[line - 1]}"
         )
     else:
-        print(f"{result.path}:{line}:{result.line_texts[line - 1]}")
+        print(f"{result['path']}:{line}:{result['line_texts'][line - 1]}")
 
 
 @click.command()
 @click.argument("query")
 @click.argument("repo_path", required=False, default=os.getcwd())
 @click.option("--no-color", is_flag=True)
 def seagoat(query, repo_path, no_color):
     """Query your codebase using vector embeddings"""
-    my_seagoat = Engine(repo_path)
-    my_seagoat.analyze_codebase()
-
-    my_seagoat.query(query)
-    my_seagoat.fetch_sync()
-    results = my_seagoat.get_results()
+    _, __, server_address = load_server_info(get_server_info_file(repo_path))
+    results = query_server(query, server_address)
 
     color_enabled = sys.stdout.isatty() and not no_color
     for result in results:
-        for line in result.get_lines(query):
-            print_result_line(result, line, color_enabled)
+        for result_line in result.get("lines", []):
+            print_result_line(result, result_line["line"], color_enabled)
 
 
 if __name__ == "__main__":
     # pylint: disable-next=no-value-for-parameter
     seagoat()
```

### Comparing `seagoat-0.1.2/seagoat/repository.py` & `seagoat-0.2.0/seagoat/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
-
 from git.repo import Repo
 from tqdm import tqdm
-from seagoat.cache import Cache
-from seagoat.common import SUPPORTED_FILE_TYPES, IGNORED_BRANCHES
 
+from seagoat.cache import Cache
+from seagoat.common import IGNORED_BRANCHES
+from seagoat.common import SUPPORTED_FILE_TYPES
 from seagoat.file import File
 
 
 class Repository:
     def __init__(self, path: str, cache: Cache) -> None:
         self._repo = Repo(path)
         self._cache = cache
```

### Comparing `seagoat-0.1.2/seagoat/result.py` & `seagoat-0.2.0/seagoat/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,20 @@
         if query.lower() in self.line_text.lower():
             return 1
         return 0
 
     def get_score(self, query: str) -> float:
         return self.vector_distance / (1 + self._get_number_of_exact_matches(query))
 
+    def to_json(self):
+        return {
+            "line": self.line,
+            "line_text": self.line_text,
+        }
+
 
 class Result:
     def __init__(self, path: str, full_path: Path) -> None:
         self.path: str = path
         self.full_path: Path = full_path
         self.lines: Set[ResultLine] = set()
         self.line_texts = self._read_lines()
@@ -47,7 +53,17 @@
                 set(
                     result_line.line
                     for result_line in self.lines
                     if result_line.get_score(query) <= best_score * 1.2
                 )
             )
         )
+
+    def to_json(self):
+        return {
+            "path": self.path,
+            "full_path": str(self.full_path),
+            "lines": [
+                line.to_json()
+                for line in sorted(self.lines, key=lambda item: item.line)
+            ],
+        }
```

### Comparing `seagoat-0.1.2/seagoat/sources/chroma.py` & `seagoat-0.2.0/seagoat/sources/chroma.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
+
 from chromadb import chromadb
 from chromadb.errors import IDAlreadyExistsError
+
 from seagoat.cache import Cache
 from seagoat.repository import Repository
 from seagoat.result import Result
 
 
 def initialize(repository: Repository):
     cache = Cache("chroma", Path(repository.path), {})
```

### Comparing `seagoat-0.1.2/seagoat/sources/ripgrep.py` & `seagoat-0.2.0/seagoat/sources/ripgrep.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pathlib import Path
+
 from ripgrepy import Ripgrepy
-from seagoat.repository import Repository
+
 from seagoat.common import SUPPORTED_FILE_TYPES
+from seagoat.repository import Repository
 from seagoat.result import Result
 
 
 def _fetch(query_text: str, path: str):
     files = {}
     for result in Ripgrepy(query_text, path).json().run().as_dict:
         result_data = result["data"]
```

### Comparing `seagoat-0.1.2/PKG-INFO` & `seagoat-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.1.2
+Version: 0.2.0
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: blessed (>=1.20.0,<2.0.0)
 Requires-Dist: chromadb (>=0.3.26,<0.4.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ripgrepy (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 -->
 
 <h1>
@@ -51,10 +53,10 @@
 
 ### Manually testing
 
 To manually test this app against a code repository,
 you can use the following command:
 
 ```bash
-poetry run python seagoat/main.py ~/path/to/your/repository
+poetry run seagoat ~/path/to/your/repository
 ```
```

