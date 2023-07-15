# Comparing `tmp/index_503-2.3.1.tar.gz` & `tmp/index_503-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-2.3.1.tar", max compression
+gzip compressed data, was "index_503-2.4.0.tar", max compression
```

## Comparing `index_503-2.3.1.tar` & `index_503-2.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-06-02 12:45:22.064540 index_503-2.3.1/LICENSE
--rw-r--r--   0        0        0     4447 2023-06-02 12:45:22.064540 index_503-2.3.1/README.md
--rw-r--r--   0        0        0     2299 2023-06-02 12:45:22.840554 index_503-2.3.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-02 12:45:22.800553 index_503-2.3.1/src/index_503/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/cache.py
--rw-r--r--   0        0        0     1336 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/file.py
--rw-r--r--   0        0        0     6936 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/py.typed
--rw-r--r--   0        0        0     1513 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/util.py
--rw-r--r--   0        0        0     5152 2023-06-02 12:45:22.064540 index_503-2.3.1/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     5712 1970-01-01 00:00:00.000000 index_503-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-15 22:32:48.404777 index_503-2.4.0/LICENSE
+-rw-r--r--   0        0        0     3915 2023-07-15 22:32:48.404777 index_503-2.4.0/README.md
+-rw-r--r--   0        0        0     2299 2023-07-15 22:32:49.336846 index_503-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-15 22:32:49.300844 index_503-2.4.0/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1147 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/cache.py
+-rw-r--r--   0        0        0     1336 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/file.py
+-rw-r--r--   0        0        0     5936 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/main.py
+-rw-r--r--   0        0        0      540 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/py.typed
+-rw-r--r--   0        0        0     1513 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/util.py
+-rw-r--r--   0        0        0     5152 2023-07-15 22:32:48.408778 index_503-2.4.0/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 index_503-2.4.0/PKG-INFO
```

### Comparing `index_503-2.3.1/LICENSE` & `index_503-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-2.3.1/README.md` & `index_503-2.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
 
 For run time installs
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
 
 ## Known issues
 
-If you see `Discarding https://wheels.koston.org/musllinux-index/intelhex-2.3.0-py2.py3-none-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4 (from https://wheels.koston.org/musllinux-index/intelhex/): Requested IntelHex>=2.2.1 from https://wheels.koston.org/musllinux-index/intelhex-2.3.0-py2.py3-none-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4 (from pymysensors==0.24.0->-r requirements_and.txt (line 1853)) has inconsistent Name: expected 'IntelHex', but metadata has 'intelhex'` upgrade pip as its fixed via https://github.com/pypa/pip/pull/12044
+This only works with pip 23.2 or later due to https://github.com/pypa/pip/issues/12038
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install index-503`
```

#### html2text {}

```diff
@@ -8,23 +8,14 @@
 disturbing the original directory. Running this again will replace the original
 index and delete the old index in an atomic manner. A lock will be held in the
 parent directory to prevent concurrent executions. ## Example For image builds
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https:/
 /wheels.koston.org/musllinux-index/" -r requirements.txt` For run time installs
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url
 "https://wheels.koston.org/musllinux-index/" -r requirements.txt` ## Known
-issues If you see `Discarding https://wheels.koston.org/musllinux-index/
-intelhex-2.3.0-py2.py3-none-
-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4
-(from https://wheels.koston.org/musllinux-index/intelhex/): Requested
-IntelHex>=2.2.1 from https://wheels.koston.org/musllinux-index/intelhex-2.3.0-
-py2.py3-none-
-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4
-(from pymysensors==0.24.0->-r requirements_and.txt (line 1853)) has
-inconsistent Name: expected 'IntelHex', but metadata has 'intelhex'` upgrade
-pip as its fixed via https://github.com/pypa/pip/pull/12044 ## Installation
-Install this via pip (or your favourite package manager): `pip install index-
-503` ## Credits This package was created with [Copier](https://
-copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
-github.com/browniebroke/pypackage-template) project template. This project
-borrows heavily from Dominic Davis-Foster's simple503 https://github.com/repo-
-helper/simple503
+issues This only works with pip 23.2 or later due to https://github.com/pypa/
+pip/issues/12038 ## Installation Install this via pip (or your favourite
+package manager): `pip install index-503` ## Credits This package was created
+with [Copier](https://copier.readthedocs.io/) and the [browniebroke/pypackage-
+template](https://github.com/browniebroke/pypackage-template) project template.
+This project borrows heavily from Dominic Davis-Foster's simple503 https://
+github.com/repo-helper/simple503
```

### Comparing `index_503-2.3.1/pyproject.toml` & `index_503-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "2.3.1"
+version = "2.4.0"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-2.3.1/src/index_503/cache.py` & `index_503-2.4.0/src/index_503/cache.py`

 * *Files identical despite different names*

### Comparing `index_503-2.3.1/src/index_503/file.py` & `index_503-2.4.0/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-2.3.1/src/index_503/index.py` & `index_503-2.4.0/src/index_503/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from typing import Dict, List, Set
 
 from natsort import natsorted
 from yarl import URL
 
 from .cache import IndexCache
 from .file import write_utf8_file
-from .metadata import repair_metadata_file
 from .page_generator import generate_index, generate_project_page
 from .util import canonicalize_name, exclusive_lock
 from .wheel_file import WheelFile
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -120,39 +119,17 @@
             canonical_name = wheel_file_obj.canonical_name
             metadata_name = wheel_file_obj.metadata_name
             projects[metadata_name].append(wheel_file_obj)
             canonical_name_to_metadata_name[canonical_name] = metadata_name
             os.symlink(wheel_file_symlink_target, target_file)
 
         self.cache.remove_stale_keys(all_wheel_files)
-        self.repair_metadata_files(
-            new_wheel_file_objects,
-            wheel_file_name_to_metadata_path,
-            canonical_name_to_metadata_name,
-        )
         self.generate_index_pages(temp_dir_path, projects)
         self.cache.write_to_new(temp_dir_path)
 
-    def repair_metadata_files(
-        self,
-        new_wheel_file_objects: List[WheelFile],
-        wheel_file_name_to_metadata_path: Dict[str, Path],
-        canonical_name_to_metadata_name: Dict[str, str],
-    ) -> None:
-        """Repair the metadata files."""
-        # Now fix all the metadata files and update the sha256 hash + cache
-        raw_cache = self.cache.cache
-        for wheel_file_obj in new_wheel_file_objects:
-            wheel_file_name = wheel_file_obj.filename
-            metadata_path = wheel_file_name_to_metadata_path[wheel_file_name]
-
-            if repair_metadata_file(metadata_path, canonical_name_to_metadata_name):
-                wheel_file_obj.update_metadata(metadata_path)
-                raw_cache[wheel_file_name] = wheel_file_obj.as_dict()
-
     def generate_index_pages(
         self, temp_dir_path: Path, projects: Dict[str, List[WheelFile]]
     ) -> None:
         """Generate the index pages."""
         index_content = str(generate_index(projects.keys()))
         write_utf8_file(temp_dir_path.joinpath("index.html"), index_content)
         project_base_url = URL("../")
```

### Comparing `index_503-2.3.1/src/index_503/page_generator.py` & `index_503-2.4.0/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-2.3.1/src/index_503/util.py` & `index_503-2.4.0/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-2.3.1/src/index_503/wheel_file.py` & `index_503-2.4.0/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-2.3.1/PKG-INFO` & `index_503-2.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 2.3.1
+Version: 2.4.0
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -81,15 +81,15 @@
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
 
 For run time installs
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
 
 ## Known issues
 
-If you see `Discarding https://wheels.koston.org/musllinux-index/intelhex-2.3.0-py2.py3-none-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4 (from https://wheels.koston.org/musllinux-index/intelhex/): Requested IntelHex>=2.2.1 from https://wheels.koston.org/musllinux-index/intelhex-2.3.0-py2.py3-none-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4 (from pymysensors==0.24.0->-r requirements_and.txt (line 1853)) has inconsistent Name: expected 'IntelHex', but metadata has 'intelhex'` upgrade pip as its fixed via https://github.com/pypa/pip/pull/12044
+This only works with pip 23.2 or later due to https://github.com/pypa/pip/issues/12038
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install index-503`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: index-503 Version: 2.3.1 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 2.4.0 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -25,23 +25,14 @@
 disturbing the original directory. Running this again will replace the original
 index and delete the old index in an atomic manner. A lock will be held in the
 parent directory to prevent concurrent executions. ## Example For image builds
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https:/
 /wheels.koston.org/musllinux-index/" -r requirements.txt` For run time installs
 `pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url
 "https://wheels.koston.org/musllinux-index/" -r requirements.txt` ## Known
-issues If you see `Discarding https://wheels.koston.org/musllinux-index/
-intelhex-2.3.0-py2.py3-none-
-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4
-(from https://wheels.koston.org/musllinux-index/intelhex/): Requested
-IntelHex>=2.2.1 from https://wheels.koston.org/musllinux-index/intelhex-2.3.0-
-py2.py3-none-
-any.whl#sha256=87cc5225657524ec6361354be928adfd56bcf2a3dcc646c40f8f094c39c07db4
-(from pymysensors==0.24.0->-r requirements_and.txt (line 1853)) has
-inconsistent Name: expected 'IntelHex', but metadata has 'intelhex'` upgrade
-pip as its fixed via https://github.com/pypa/pip/pull/12044 ## Installation
-Install this via pip (or your favourite package manager): `pip install index-
-503` ## Credits This package was created with [Copier](https://
-copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
-github.com/browniebroke/pypackage-template) project template. This project
-borrows heavily from Dominic Davis-Foster's simple503 https://github.com/repo-
-helper/simple503
+issues This only works with pip 23.2 or later due to https://github.com/pypa/
+pip/issues/12038 ## Installation Install this via pip (or your favourite
+package manager): `pip install index-503` ## Credits This package was created
+with [Copier](https://copier.readthedocs.io/) and the [browniebroke/pypackage-
+template](https://github.com/browniebroke/pypackage-template) project template.
+This project borrows heavily from Dominic Davis-Foster's simple503 https://
+github.com/repo-helper/simple503
```

