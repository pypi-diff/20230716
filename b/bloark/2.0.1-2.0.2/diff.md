# Comparing `tmp/bloark-2.0.1.tar.gz` & `tmp/bloark-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloark-2.0.1.tar", max compression
+gzip compressed data, was "bloark-2.0.2.tar", max compression
```

## Comparing `bloark-2.0.1.tar` & `bloark-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 bloark-2.0.1/LICENSE
--rw-r--r--   0        0        0     1542 2023-07-15 23:37:34.226075 bloark-2.0.1/README.md
--rw-r--r--   0        0        0      137 2023-07-16 05:13:51.246446 bloark-2.0.1/bloark/__init__.py
--rw-r--r--   0        0        0    17991 2023-07-16 05:13:23.187997 bloark-2.0.1/bloark/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 bloark-2.0.1/bloark/builder_helpers.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 bloark-2.0.1/bloark/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 bloark-2.0.1/bloark/logger_init.py
--rw-r--r--   0        0        0    11486 2023-07-16 05:48:42.766541 bloark-2.0.1/bloark/modifier.py
--rw-r--r--   0        0        0     8460 2023-07-16 05:13:23.191780 bloark-2.0.1/bloark/reader.py
--rw-r--r--   0        0        0     6702 2023-07-16 06:04:39.261316 bloark-2.0.1/bloark/utils.py
--rw-r--r--   0        0        0     5234 2023-07-16 05:25:20.174851 bloark-2.0.1/bloark/warehouse.py
--rw-r--r--   0        0        0      980 2023-07-16 06:11:44.354513 bloark-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2617 1970-01-01 00:00:00.000000 bloark-2.0.1/setup.py
--rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 bloark-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 bloark-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1542 2023-07-15 23:37:34.226075 bloark-2.0.2/README.md
+-rw-r--r--   0        0        0      137 2023-07-16 19:42:54.285250 bloark-2.0.2/bloark/__init__.py
+-rw-r--r--   0        0        0    17991 2023-07-16 05:13:23.187997 bloark-2.0.2/bloark/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 bloark-2.0.2/bloark/builder_helpers.py
+-rw-r--r--   0        0        0     2977 2023-07-16 21:18:37.433442 bloark-2.0.2/bloark/decorators.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 bloark-2.0.2/bloark/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 bloark-2.0.2/bloark/logger_init.py
+-rw-r--r--   0        0        0    16600 2023-07-16 21:23:43.884492 bloark-2.0.2/bloark/modifier.py
+-rw-r--r--   0        0        0     8978 2023-07-16 21:36:29.042415 bloark-2.0.2/bloark/reader.py
+-rw-r--r--   0        0        0     7755 2023-07-16 20:23:09.560453 bloark-2.0.2/bloark/utils.py
+-rw-r--r--   0        0        0     5234 2023-07-16 05:25:20.174851 bloark-2.0.2/bloark/warehouse.py
+-rw-r--r--   0        0        0      979 2023-07-16 21:27:28.980983 bloark-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 bloark-2.0.2/setup.py
+-rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 bloark-2.0.2/PKG-INFO
```

### Comparing `bloark-2.0.1/LICENSE` & `bloark-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bloark-2.0.1/README.md` & `bloark-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bloark-2.0.1/bloark/builder.py` & `bloark-2.0.2/bloark/builder.py`

 * *Files identical despite different names*

### Comparing `bloark-2.0.1/bloark/logger.py` & `bloark-2.0.2/bloark/logger.py`

 * *Files identical despite different names*

### Comparing `bloark-2.0.1/bloark/logger_init.py` & `bloark-2.0.2/bloark/logger_init.py`

 * *Files identical despite different names*

### Comparing `bloark-2.0.1/bloark/reader.py` & `bloark-2.0.2/bloark/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from typing import List, Tuple, Union
 import time
 import uuid
 
 from py7zr import py7zr
 
 from .logger_init import _init_logger_main_process, _init_logger_sub_process, _init_logger_multiprocessing
-from .utils import get_file_list, prepare_output_dir, get_curr_version, cleanup_dir, read_line_in_file, parse_schema
+from .utils import get_file_list, prepare_output_dir, get_curr_version, cleanup_dir, read_line_in_file, parse_schema, \
+    decompress_zstd
 
 _DEFAULT_NUM_PROC = 1
 _DEFAULT_LOG_LEVEL = logging.INFO
 
 
 class Reader:
     """
@@ -83,37 +84,44 @@
     def _worker_initializer(self, q):
         """
         Initialize the worker process.
         """
         # Initialize the logger within the sub-process.
         _init_logger_sub_process(q, log_level=self.log_level)
 
-    def _decompress_executor(self, file_path: str) -> List[str]:
+    def _decompress_executor(self, file_path: str, temporarily: bool = False) -> List[str]:
         """
         Decompress the file.
         """
-        # Initialize temporary directory.
-        temp_dir = os.path.join(self.output_dir, 'temp')
-        os.makedirs(temp_dir, exist_ok=True)
+        # Initialize output directory.
+        output_dir = os.path.join(self.output_dir, 'temp') if temporarily else self.output_dir
+        os.makedirs(output_dir, exist_ok=True)
 
         archive_filename = os.path.basename(file_path)
         random_id = uuid.uuid4().hex
-        decompressed_dir_path = os.path.join(temp_dir, random_id)
-        os.makedirs(decompressed_dir_path, exist_ok=True)
+        decompressed_dir_path = os.path.join(output_dir, random_id) if temporarily else output_dir
+        if temporarily:
+            os.makedirs(decompressed_dir_path, exist_ok=True)
 
         logging.debug(f'Decompressing [{archive_filename}]...')
 
         try:
-            with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
-                start_time = time.time()
-                z.extractall(path=decompressed_dir_path)
-                end_time = time.time()
-                execution_duration = (end_time - start_time) / 60
-                logging.debug(f'Decompression took {execution_duration:.2f} min. ({archive_filename})')
-            decompressed_files = get_file_list(decompressed_dir_path)
+            start_time = time.time()
+            if file_path.endswith('.7z'):
+                with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
+                    z.extractall(path=decompressed_dir_path)
+                decompressed_files = get_file_list(decompressed_dir_path)
+            elif file_path.endswith('.zst'):
+                decompress_zstd(file_path, os.path.join(decompressed_dir_path, archive_filename[:-4]))
+                decompressed_files = [os.path.join(decompressed_dir_path, archive_filename[:-4])]
+            else:
+                decompressed_files = []
+            end_time = time.time()
+            execution_duration = (end_time - start_time) / 60
+            logging.debug(f'Decompression took {execution_duration:.2f} min. ({archive_filename})')
             return decompressed_files
 
         except Exception as e:
             logging.critical(f'Failed to decompress [{archive_filename}] for this reason: {e}')
             return []
 
     def decompress(self):
@@ -228,15 +236,15 @@
         # Prepare the temporary directory for glimpse.
         glimpse_temp_dir = os.path.join(os.getcwd(), '.glimpse')
         os.makedirs(glimpse_temp_dir, exist_ok=True)
 
         logging.info(f'Decompressing...')
 
         # Decompress the file.
-        decompressed_files = self._decompress_executor(glimpse_path)
+        decompressed_files = self._decompress_executor(file_path=glimpse_path, temporarily=True)
         if not decompressed_files:
             logging.error(f'Failed to decompress the file: {glimpse_path}')
             return None, None
 
         decompressed_path = decompressed_files[0]
         first_block_text = read_line_in_file(decompressed_path, 0).rstrip('\n')
```

### Comparing `bloark-2.0.1/bloark/warehouse.py` & `bloark-2.0.2/bloark/warehouse.py`

 * *Files identical despite different names*

### Comparing `bloark-2.0.1/pyproject.toml` & `bloark-2.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "bloark"
-version = "2.0.1"
-description = "Blocks Architecture (BloArk): An unified tool for processing revision-based data efficiently."
+version = "2.0.2"
+description = "Blocks Architecture (BloArk): A unified tool for processing revision-based data efficiently."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "bloark" },
 ]
 homepage = "https://bloark.lingxi.li/"
```

### Comparing `bloark-2.0.1/setup.py` & `bloark-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
  'zstandard>=0.21.0,<0.22.0']
 
 entry_points = \
 {'console_scripts': ['benchmark = tests.benchmark:main']}
 
 setup_kwargs = {
     'name': 'bloark',
-    'version': '2.0.1',
-    'description': 'Blocks Architecture (BloArk): An unified tool for processing revision-based data efficiently.',
+    'version': '2.0.2',
+    'description': 'Blocks Architecture (BloArk): A unified tool for processing revision-based data efficiently.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/b4d5d2b0-860c-4d73-02f0-104d77223800/Ultra" alt="BloArk" />\n\n# Blocks Architecture (BloArk)\n\nBlocks Architecture (BloArk) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install bloark\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bloark.lingxi.li/',
     'packages': packages,
```

### Comparing `bloark-2.0.1/PKG-INFO` & `bloark-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bloark
-Version: 2.0.1
-Summary: Blocks Architecture (BloArk): An unified tool for processing revision-based data efficiently.
+Version: 2.0.2
+Summary: Blocks Architecture (BloArk): A unified tool for processing revision-based data efficiently.
 Home-page: https://bloark.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

