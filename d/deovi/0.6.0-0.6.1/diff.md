# Comparing `tmp/deovi-0.6.0.tar.gz` & `tmp/deovi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deovi-0.6.0.tar", last modified: Wed Jul 12 20:41:16 2023, max compression
+gzip compressed data, was "deovi-0.6.1.tar", last modified: Sun Jul 16 10:04:24 2023, max compression
```

## Comparing `deovi-0.6.0.tar` & `deovi-0.6.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1075 2022-09-12 23:01:15.000000 deovi-0.6.0/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      173 2022-09-12 23:01:15.000000 deovi-0.6.0/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-12 20:41:16.054276 deovi-0.6.0/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      979 2023-07-12 20:40:49.000000 deovi-0.6.0/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      686 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/cli/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/cli/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1940 2023-03-07 02:37:37.000000 deovi-0.6.0/deovi/cli/collect.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1860 2023-07-12 20:40:49.000000 deovi-0.6.0/deovi/cli/entrypoint.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1117 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/cli/job.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1751 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/cli/rename.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3794 2023-07-12 20:40:49.000000 deovi-0.6.0/deovi/cli/scrap.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      232 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/cli/version.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/collector/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      463 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/collector/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    13819 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/collector/collect.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6637 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/collector/storage.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1150 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/exceptions.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1128 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/logger.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/renamer/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    10871 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/jobs.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4685 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/renamer/printer.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4505 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/runner.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    11870 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/tasks.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5033 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/validators.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6193 2023-07-12 20:40:49.000000 deovi-0.6.0/deovi/scrapper.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4720 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/utils/checksum.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      717 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/utils/jsons.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3347 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/utils/tests.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      789 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       60 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/entry_points.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      234 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        6 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-03-04 01:42:58.000000 deovi-0.6.0/deovi.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1482 2023-07-12 20:41:16.058276 deovi-0.6.0/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-09-12 23:01:15.000000 deovi-0.6.0/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.481897 deovi-0.6.1/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1075 2022-09-12 23:01:15.000000 deovi-0.6.1/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      173 2022-09-12 23:01:15.000000 deovi-0.6.1/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-16 10:04:24.481897 deovi-0.6.1/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      979 2023-07-12 20:40:49.000000 deovi-0.6.1/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      686 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi/cli/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/cli/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1940 2023-03-07 02:37:37.000000 deovi-0.6.1/deovi/cli/collect.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1860 2023-07-12 20:40:49.000000 deovi-0.6.1/deovi/cli/entrypoint.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1117 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/cli/job.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1751 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/cli/rename.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4007 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/cli/scrap.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      232 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/cli/version.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi/collector/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      463 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/collector/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    13956 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/collector/collect.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6755 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/collector/storage.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1150 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/exceptions.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1128 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/logger.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.481897 deovi-0.6.1/deovi/renamer/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10871 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/jobs.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4685 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/renamer/printer.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4505 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/runner.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    11870 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/tasks.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5033 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/validators.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5999 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/scrapper.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.481897 deovi-0.6.1/deovi/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4720 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/utils/checksum.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      717 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/utils/jsons.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3347 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/utils/tests.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      789 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       60 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/entry_points.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      234 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        6 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-03-04 01:42:58.000000 deovi-0.6.1/deovi.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1482 2023-07-16 10:04:24.481897 deovi-0.6.1/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-09-12 23:01:15.000000 deovi-0.6.1/setup.py
```

### Comparing `deovi-0.6.0/LICENCE.txt` & `deovi-0.6.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/PKG-INFO` & `deovi-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deovi
-Version: 0.6.0
+Version: 0.6.1
 Summary: Utility to rename files and collect their filepaths
 Home-page: https://github.com/sveetch/deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `deovi-0.6.0/README.rst` & `deovi-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/__init__.py` & `deovi-0.6.1/deovi/__init__.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/cli/collect.py` & `deovi-0.6.1/deovi/cli/collect.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/cli/entrypoint.py` & `deovi-0.6.1/deovi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/cli/job.py` & `deovi-0.6.1/deovi/cli/job.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/cli/rename.py` & `deovi-0.6.1/deovi/cli/rename.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/cli/scrap.py` & `deovi-0.6.1/deovi/cli/scrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,24 @@
         help=(
             "If enabled, a file 'manifest.diff.txt' will be written along manifest "
             "file if there was a previous manifest file in destination directory and "
             "it got differences with the new one. This is not incremental, previous "
             "manifest difference file may be overwritten from a scrap job to another."
         ),
     )
+    @click.option(
+        "--dry",
+        is_flag=True,
+        help=(
+            "If enabled, everything is runned but nothing will be written or removed."
+        ),
+    )
     @click.pass_context
-    def scrap_command(context, tvid, destination, key, filekey, language, write_diff):
+    def scrap_command(context, tvid, destination, key, filekey, language, write_diff,
+                      dry):
         """
         Scrap TV show informations and poster image from TMDb API.
 
         Required arguments:
 
         TVID\n
             The TV Show ID from TMDb, it may looks like an integer ('14009').
@@ -108,15 +116,15 @@
         logger.info("TV ID: {}".format(tvid))
         logger.debug("Destination: {}".format(destination))
         logger.debug("Language: {}".format(language))
         logger.debug("API Key {}".format(
             "from file" if filekey else "from string",
         ))
 
-        connector = TmdbScrapper(key, language=language)
+        connector = TmdbScrapper(key, language=language, dry=dry)
 
         data, manifest, poster, diffs = connector.fetch_tv(
             destination,
             tvid,
             write_diff=write_diff,
         )
         logger.info("Title: {}".format(data["title"]))
```

### Comparing `deovi-0.6.0/deovi/collector/collect.py` & `deovi-0.6.1/deovi/collector/collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         self.file_storage_queue = []
 
         self.registry = {}
         self.stats = {
             "directories": 0,
             "files": 0,
             "size": 0,
+            "asset_storage": None,
         }
 
     def timestamp_to_isoformat(self, timestamp):
         """
         Return datetime formatted from given timestamp.
 
         Arguments:
@@ -396,10 +397,12 @@
 
         if self.registry and destination:
             with destination.open("w") as fp:
                 json.dump(self.registry, fp, indent=4, cls=ExtendedJsonEncoder)
                 self.log_info("Registry saved to: {}".format(str(destination)))
 
             # Proceed to copy queued files into storage dir
-            self.storage.store_assets(self.file_storage_queue)
+            container, stored = self.storage.store_assets(self.file_storage_queue)
+            if container:
+                self.stats["asset_storage"] = container
 
         return self.stats
```

### Comparing `deovi-0.6.0/deovi/collector/storage.py` & `deovi-0.6.1/deovi/collector/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,16 +161,18 @@
         asset, (first item is the source path).
 
         Arguments:
             assets (list): List of tuple ``(source, destination)`` where both items are
                 Path objects as returned from ``Collector.get_directory_asset()``.
 
         Returns:
-            list: List of stored file in their final destination.
+            tuple: The asset storage path and the list of stored files in their final
+            destination.
         """
+        container = None
         stored = []
 
         if len(assets) > 0:
             container = self.storage_path / self.storage_assets
 
             if not container.exists():
                 container.mkdir(parents=True, exist_ok=True)
@@ -181,8 +183,11 @@
                     self.log_warning(msg.format(source))
 
                 # Destination path should be a relative path (from base) which already
                 # include the assets directory
                 shutil.copy(source, self.storage_path / destination)
                 stored.append(self.storage_path / destination)
 
-        return stored
+        return (
+            container,
+            stored,
+        )
```

### Comparing `deovi-0.6.0/deovi/exceptions.py` & `deovi-0.6.1/deovi/exceptions.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/logger.py` & `deovi-0.6.1/deovi/logger.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/renamer/jobs.py` & `deovi-0.6.1/deovi/renamer/jobs.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/renamer/printer.py` & `deovi-0.6.1/deovi/renamer/printer.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/renamer/runner.py` & `deovi-0.6.1/deovi/renamer/runner.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/renamer/tasks.py` & `deovi-0.6.1/deovi/renamer/tasks.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/renamer/validators.py` & `deovi-0.6.1/deovi/renamer/validators.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/scrapper.py` & `deovi-0.6.1/deovi/scrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,19 @@
         api_key (string): Private key needed to use API.
 
     Keyword Arguments:
         language (string): Used language for payload content.
         poster_size (string): Size name as supported from TMDb API.
         poster_filename (string): Filename to use to write download poster image,
             without any extension.
+        dry (boolean): If enabled nothing will be written or removed.
     """
     def __init__(self, api_key, language="fr", poster_size="w780",
-                 poster_filename="cover"):
+                 poster_filename="cover", dry=False):
+        self.dry = dry
         self.poster_size = poster_size
         self.poster_filename = poster_filename
 
         # Set TMDb client options
         self.client = self.get_client(api_key, language)
 
         # Get some config attributes from API
@@ -115,20 +117,21 @@
             url.split("/")[-1]
         ).suffix
 
         destination = basefilepath.with_suffix(extension)
 
         # Go download the file
         with requests.get(url, stream=True) as r:
-            # Create destination directory if missing
-            if not basepath.exists():
-                basepath.mkdir(parents=True, exist_ok=True)
-            # Write file from stream
-            with open(destination, "wb") as f:
-                shutil.copyfileobj(r.raw, f)
+            if not self.dry:
+                # Create destination directory if missing
+                if not basepath.exists():
+                    basepath.mkdir(parents=True, exist_ok=True)
+                # Write file from stream
+                with open(destination, "wb") as f:
+                    shutil.copyfileobj(r.raw, f)
 
         return destination
 
     def write_manifest(self, sourcepath, data, write_diff=False):
         """
         Write given data to manifest and possibly create a log file about differences
         with previous manifest file if any.
@@ -136,22 +139,23 @@
         diff_lines = []
 
         # Write differences if any
         if sourcepath.exists():
             original = yaml.load(sourcepath.read_text(), Loader=yaml.FullLoader)
             diffs = DeepDiff(original, data)
             diff_lines = diffs.pretty().splitlines()
-            if write_diff and diff_lines:
+            if not self.dry and write_diff and diff_lines:
                 diffpath = sourcepath.with_suffix(".diff.txt")
                 diffpath.write_text("\n".join(diff_lines))
 
         # Write/overwrite manifest
-        sourcepath.write_text(
-            yaml.dump(data, Dumper=yaml.Dumper)
-        )
+        if not self.dry:
+            sourcepath.write_text(
+                yaml.dump(data, Dumper=yaml.Dumper)
+            )
 
         return diff_lines
 
     def fetch_tv(self, directory, tv_id, write_diff=False):
         """
         Get informations payload and medias for given TV ID.
 
@@ -174,23 +178,7 @@
 
         return (
             data,
             manifest,
             fetched_poster,
             diff,
         )
-
-
-if __name__ == "__main__":
-    API_KEY = "c8a1f464dca620cde9037eda3f105425"
-    connector = TmdbScrapper(API_KEY, language="fr")
-
-    print()
-    connector.fetch_tv(
-        Path("/home/emencia/Projects/Apps/deovi/dist/StarTrek_Strange-New-Worlds"),
-        "103516"
-    )
-    print()
-    connector.fetch_tv(
-        Path("/home/emencia/Projects/Apps/deovi/dist/Au dela du reel"),
-        "21567"
-    )
```

### Comparing `deovi-0.6.0/deovi/utils/checksum.py` & `deovi-0.6.1/deovi/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/utils/jsons.py` & `deovi-0.6.1/deovi/utils/jsons.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi/utils/tests.py` & `deovi-0.6.1/deovi/utils/tests.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/deovi.egg-info/PKG-INFO` & `deovi-0.6.1/deovi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deovi
-Version: 0.6.0
+Version: 0.6.1
 Summary: Utility to rename files and collect their filepaths
 Home-page: https://github.com/sveetch/deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `deovi-0.6.0/deovi.egg-info/SOURCES.txt` & `deovi-0.6.1/deovi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deovi-0.6.0/setup.cfg` & `deovi-0.6.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deovi
-version = 0.6.0
+version = 0.6.1
 description = Utility to rename files and collect their filepaths
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = sveetch@gmail.com
 url = https://github.com/sveetch/deovi
 license = MIT
```

