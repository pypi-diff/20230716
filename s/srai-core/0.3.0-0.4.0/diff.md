# Comparing `tmp/srai-core-0.3.0.tar.gz` & `tmp/srai-core-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-core-0.3.0.tar", last modified: Sat Jul 15 08:26:33 2023, max compression
+gzip compressed data, was "srai-core-0.4.0.tar", last modified: Sun Jul 16 08:32:17 2023, max compression
```

## Comparing `srai-core-0.3.0.tar` & `srai-core-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 08:26:33.804980 srai-core-0.3.0/
--rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       24 2023-07-15 08:05:50.000000 srai-core-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      767 2023-07-15 08:26:33.805985 srai-core-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 07:25:20.000000 srai-core-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 08:26:33.807980 srai-core-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1221 2023-07-15 08:06:27.000000 srai-core-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:26:33.794984 srai-core-0.3.0/srai_core/
--rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.3.0/srai_core/__init__.py
--rw-rw-rw-   0        0        0      356 2023-07-15 07:48:15.000000 srai-core-0.3.0/srai_core/file_store_disk.py
--rw-rw-rw-   0        0        0     1238 2023-07-15 07:46:28.000000 srai-core-0.3.0/srai_core/jsondict_store.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:26:33.803981 srai-core-0.3.0/srai_core.egg-info/
--rw-rw-rw-   0        0        0      767 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:32:17.526181 srai-core-0.4.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       24 2023-07-15 08:05:50.000000 srai-core-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      767 2023-07-16 08:32:17.526181 srai-core-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 07:25:20.000000 srai-core-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-16 08:32:17.528174 srai-core-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-16 08:28:50.000000 srai-core-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:32:17.498175 srai-core-0.4.0/srai_core/
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.4.0/srai_core/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-07-16 08:31:22.000000 srai-core-0.4.0/srai_core/file_store.py
+-rw-rw-rw-   0        0        0      466 2023-07-16 08:28:25.000000 srai-core-0.4.0/srai_core/file_store_disk.py
+-rw-rw-rw-   0        0        0     1296 2023-07-16 08:31:12.000000 srai-core-0.4.0/srai_core/jsondict_store.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:32:17.525192 srai-core-0.4.0/srai_core.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 08:32:17.000000 srai-core-0.4.0/srai_core.egg-info/top_level.txt
```

### Comparing `srai-core-0.3.0/LICENSE.txt` & `srai-core-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srai-core-0.3.0/PKG-INFO` & `srai-core-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai-core
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library core functions used in other SRAI libraries.
 Home-page: https://github.com/southriverai/srai-core
 Download-URL: https://github.com/southriverai/srai-core/archive/v_01.tar.gz
 Author: Jaap Oosterbroek
 Author-email: jaap.oosterbroek@southriverai.com
 License: MIT
 Keywords: SRAI,TOOLS
```

### Comparing `srai-core-0.3.0/setup.py` & `srai-core-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,29 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="srai-core",
     packages=find_packages(),
-    version="0.3.0",
-    license='MIT',
+    version="0.4.0",
+    license="MIT",
     package_data={},
     python_requires=">=3.5",
     install_requires=requirements,
     author="Jaap Oosterbroek",
     author_email="jaap.oosterbroek@southriverai.com",
     description="A library core functions used in other SRAI libraries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/southriverai/srai-core",
-    download_url='https://github.com/southriverai/srai-core/archive/v_01.tar.gz',
-    keywords=['SRAI', 'TOOLS'],
+    download_url="https://github.com/southriverai/srai-core/archive/v_01.tar.gz",
+    keywords=["SRAI", "TOOLS"],
     classifiers=[
-        'Development Status :: 3 - Alpha', 
-        'Intended Audience :: Developers',      # Define that your audience are developers
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',   # Again, pick a license
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",  # Define that your audience are developers
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",  # Again, pick a license
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
 )
-
-
-
```

### Comparing `srai-core-0.3.0/srai_core/jsondict_store.py` & `srai-core-0.4.0/srai_core/jsondict_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import hashlib
 import json
 
-from srai_core.file_store_disk import FileStoreDisk
-class JsondictStore(FileStoreDisk):
-    #file store for 
+from srai_core.file_store import FileStore
 
-    def __init__(self, backing_store: FileStoreDisk) -> None:
+
+class JsondictStore:
+    # file store for
+
+    def __init__(self, backing_store: FileStore) -> None:
         self.backing_store = backing_store
 
     def sha256hexdigest(self, jsondict_key: dict) -> str:
         # convert a jsondict_key to a sha256 hash digest
         # jsondict_key is a dict of key value pairs
-        jsondict_key_bytes = json.dumps(jsondict_key).encode('utf-8')
+        jsondict_key_bytes = json.dumps(jsondict_key).encode("utf-8")
         return hashlib.sha256(jsondict_key_bytes).hexdigest()
 
     def exists(self, jsondict_key: dict) -> bool:
         key = self.sha256hexdigest(jsondict_key)
         return self.backing_store.exists(key)
 
     def read_jsondict(self, jsondict_key: dict) -> bool:
         key = self.sha256hexdigest(jsondict_key)
+        self.backing_store.download(key)
         path_file = self.backing_store.get_path_file(key)
-        with open(path_file, 'r') as file:
+        with open(path_file, "r") as file:
             return json.load(file)
 
     def write_jsondict(self, jsondict_key: dict, jsondict_value: dict) -> None:
         key = self.sha256hexdigest(jsondict_key)
         path_file = self.backing_store.get_path_file(key)
-        with open(path_file, 'r') as file:
+        with open(path_file, "r") as file:
             json.dump(jsondict_value, file)
+        self.backing_store.upload(key)
```

### Comparing `srai-core-0.3.0/srai_core.egg-info/PKG-INFO` & `srai-core-0.4.0/srai_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai-core
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library core functions used in other SRAI libraries.
 Home-page: https://github.com/southriverai/srai-core
 Download-URL: https://github.com/southriverai/srai-core/archive/v_01.tar.gz
 Author: Jaap Oosterbroek
 Author-email: jaap.oosterbroek@southriverai.com
 License: MIT
 Keywords: SRAI,TOOLS
```

