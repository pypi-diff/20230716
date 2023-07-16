# Comparing `tmp/unibox-0.1.4.tar.gz` & `tmp/unibox-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.4.tar", max compression
+gzip compressed data, was "unibox-0.1.4.3.tar", max compression
```

## Comparing `unibox-0.1.4.tar` & `unibox-0.1.4.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-07-14 02:03:31.604033 unibox-0.1.4/LICENSE
--rw-r--r--   0        0        0      733 2023-07-14 02:03:31.604033 unibox-0.1.4/README.md
--rw-r--r--   0        0        0      500 2023-07-14 02:03:31.604033 unibox-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       79 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/__init__.py
--rw-r--r--   0        0        0     3095 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/cli.py
--rw-r--r--   0        0        0        0 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/processing/__init__.py
--rw-r--r--   0        0        0     2095 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/processing/file_mover.py
--rw-r--r--   0        0        0     6268 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/utils/__init__.py
--rw-r--r--   0        0        0     3291 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/utils/uni_loader.py
--rw-r--r--   0        0        0     3759 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/utils/uni_logger.py
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 unibox-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-16 02:44:50.607468 unibox-0.1.4.3/LICENSE
+-rw-r--r--   0        0        0      733 2023-07-16 02:44:50.607468 unibox-0.1.4.3/README.md
+-rw-r--r--   0        0        0      578 2023-07-16 02:44:50.607468 unibox-0.1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      541 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/__init__.py
+-rw-r--r--   0        0        0     3095 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/cli.py
+-rw-r--r--   0        0        0        0 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/processing/converer.py
+-rw-r--r--   0        0        0     2095 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/processing/file_mover.py
+-rw-r--r--   0        0        0     6268 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/utils/__init__.py
+-rw-r--r--   0        0        0     3573 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/utils/uni_loader.py
+-rw-r--r--   0        0        0     3759 2023-07-16 02:44:50.607468 unibox-0.1.4.3/unibox/utils/uni_logger.py
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 unibox-0.1.4.3/PKG-INFO
```

### Comparing `unibox-0.1.4/LICENSE` & `unibox-0.1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.1.4/README.md` & `unibox-0.1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `unibox-0.1.4/unibox/cli.py` & `unibox-0.1.4.3/unibox/cli.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.4/unibox/processing/file_mover.py` & `unibox-0.1.4.3/unibox/processing/file_mover.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.4/unibox/processing/image_resizer.py` & `unibox-0.1.4.3/unibox/processing/image_resizer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.4/unibox/utils/uni_loader.py` & `unibox-0.1.4.3/unibox/utils/uni_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # Adding the _load_csv and _load_parquet methods to the UniLoader class
 
 from __future__ import annotations
 
-from pathlib import Path
-from typing import Callable
-import csv
 import json
 import tomli
 import pandas as pd
 from PIL import Image
+from pathlib import Path
 from omegaconf import OmegaConf
-import pyarrow.parquet as pq
 
 from .uni_logger import UniLogger
 
 
 class UniLoader:
     """A simple utility class for loading various file types.
     Data cleaning should be done in the class that uses this loader.
@@ -25,14 +22,15 @@
             self.logger = UniLogger(file_suffix="UniLoader")
         else:
             self.logger = logger
 
         # Mapping of file extensions to loader functions
         self.loaders = {
             '.json': self._load_json,
+            '.jsonl': self._load_jsonl,  # Added '.jsonl' to the loaders dictionary
             '.txt': self._load_txt,
             '.csv': self._load_csv,
             '.png': self._load_image,
             '.jpg': self._load_image,
             '.toml': self._load_toml,
             '.yaml': self._load_yaml,
             '.parquet': self._load_parquet,
@@ -62,14 +60,19 @@
             self.logger.log("ERROR", f'{file_type} LOAD ERROR at "{file_path}": {e}')
             return None
 
     def _load_json(self, file_path: Path, encoding):
         with open(file_path, "r", encoding=encoding) as f:
             return json.load(f)
 
+    def _load_jsonl(self, file_path: Path, encoding):
+        """Load data from a .jsonl file and return it as a list of dictionaries."""
+        with open(file_path, "r", encoding=encoding) as f:
+            return [json.loads(line) for line in f]
+
     def _load_txt(self, file_path: Path, encoding):
         with open(file_path, "r", encoding=encoding) as f:
             return f.readlines()
 
     def _load_csv(self, file_path: Path, encoding):
         return pd.read_csv(file_path, delimiter=',')
 
@@ -88,14 +91,14 @@
         return pd.read_parquet(file_path)
 
 
 if __name__ == "__main__":
     # Usage example
     logger = UniLogger("logs", file_suffix="data_loader")
     data_loader = UniLoader(logger)
-    json_data = data_loader.loads("example.json")
-    txt_data = data_loader.loads(Path("example.txt"))
+    json_data = data_loader.loads("example.json") # string
+    txt_data = data_loader.loads(Path("example.txt")) # path
     csv_data = data_loader.loads(Path("example.csv"))
     image_data = data_loader.loads(Path("example.png"))
     toml_data = data_loader.loads(Path("example.toml"))
     yaml_data = data_loader.loads(Path("example.yaml"))
     parquet_data = data_loader.loads(Path("example.parquet"))
```

### Comparing `unibox-0.1.4/unibox/utils/uni_logger.py` & `unibox-0.1.4.3/unibox/utils/uni_logger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.4/PKG-INFO` & `unibox-0.1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.1.4
+Version: 0.1.4.3
 Summary: one toolbox to rule'em all
 License: GPL-3.0
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.5,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pandas (>=1.1.5,<2.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
-Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: pyarrow (>=6.0.1,<7.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Unibox
 
 Unibox is a tool that aims to provide a unified interface for various common daily operations.
```

