# Comparing `tmp/deltalake-redis-lock-0.0.1a5.tar.gz` & `tmp/deltalake-redis-lock-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake-redis-lock-0.0.1a5.tar", max compression
+gzip compressed data, was "deltalake-redis-lock-0.0.1a6.tar", max compression
```

## Comparing `deltalake-redis-lock-0.0.1a5.tar` & `deltalake-redis-lock-0.0.1a6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-07-14 15:51:34.636636 deltalake-redis-lock-0.0.1a5/LICENSE
--rw-r--r--   0        0        0     2628 2023-07-16 06:17:34.428847 deltalake-redis-lock-0.0.1a5/README.md
--rw-r--r--   0        0        0      594 2023-07-16 08:48:54.001478 deltalake-redis-lock-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 15:52:45.562904 deltalake-redis-lock-0.0.1a5/src/__init__.py
--rw-r--r--   0        0        0     3055 2023-07-15 14:28:54.444862 deltalake-redis-lock-0.0.1a5/src/deltalake_redis_lock.py
--rw-r--r--   0        0        0      126 2023-07-15 14:28:54.445676 deltalake-redis-lock-0.0.1a5/src/global_lock.py
--rw-r--r--   0        0        0     2135 2023-07-15 14:28:54.446711 deltalake-redis-lock-0.0.1a5/src/redis_lock_object_store.py
--rw-r--r--   0        0        0     3533 2023-07-16 08:49:23.725516 deltalake-redis-lock-0.0.1a5/setup.py
--rw-r--r--   0        0        0     3321 2023-07-16 08:49:23.725867 deltalake-redis-lock-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-14 15:51:34.636636 deltalake-redis-lock-0.0.1a6/LICENSE
+-rw-r--r--   0        0        0     2592 2023-07-16 09:04:06.785162 deltalake-redis-lock-0.0.1a6/README.md
+-rw-r--r--   0        0        0      594 2023-07-16 08:58:58.292361 deltalake-redis-lock-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 15:52:45.562904 deltalake-redis-lock-0.0.1a6/src/__init__.py
+-rw-r--r--   0        0        0     3051 2023-07-16 08:58:19.312467 deltalake-redis-lock-0.0.1a6/src/deltalake_redis_lock.py
+-rw-r--r--   0        0        0      122 2023-07-16 08:58:19.308691 deltalake-redis-lock-0.0.1a6/src/global_lock.py
+-rw-r--r--   0        0        0     2135 2023-07-15 14:28:54.446711 deltalake-redis-lock-0.0.1a6/src/redis_lock_object_store.py
+-rw-r--r--   0        0        0     3496 2023-07-16 09:04:41.918074 deltalake-redis-lock-0.0.1a6/setup.py
+-rw-r--r--   0        0        0     3285 2023-07-16 09:04:41.918368 deltalake-redis-lock-0.0.1a6/PKG-INFO
```

### Comparing `deltalake-redis-lock-0.0.1a5/LICENSE` & `deltalake-redis-lock-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `deltalake-redis-lock-0.0.1a5/README.md` & `deltalake-redis-lock-0.0.1a6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,10 +111,9 @@
 environment of the codebase, and do `unit/integration and load tests`.
 
 ```bash
 make build-container-image DOCKER_BUILD="buildx build --platform linux/amd64" CONTEXT=.
 ```
 
 ```bash
-make get-container-info-environment
 make run-container-tests type=unit
 ```
```

### Comparing `deltalake-redis-lock-0.0.1a5/pyproject.toml` & `deltalake-redis-lock-0.0.1a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltalake-redis-lock"
-version = "0.0.1-alpha.5"
+version = "0.0.1-alpha.6"
 description = "deltalake-redis-lock"
 authors = ["Simon Thelin"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/wrapbytes/deltalake-redis-lock"
 repository = "https://github.com/wrapbytes/deltalake-redis-lock"
 packages = [
```

### Comparing `deltalake-redis-lock-0.0.1a5/src/deltalake_redis_lock.py` & `deltalake-redis-lock-0.0.1a6/src/deltalake_redis_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pyarrow.fs as pa_fs
 from deltalake import DeltaTable, write_deltalake
 from deltalake._internal import DeltaError
 from pyarrow.lib import RecordBatchReader
 from redis.exceptions import LockError
 from redis.lock import Lock
 
-from src.global_lock import REDIS_LOCK
+from global_lock import REDIS_LOCK
 
 
 def write_redis_lock_deltalake(
     lock_table_name: str,
     table_or_uri: Union[str, Path, DeltaTable],
     data: Union[
         pd.DataFrame,
```

### Comparing `deltalake-redis-lock-0.0.1a5/src/redis_lock_object_store.py` & `deltalake-redis-lock-0.0.1a6/src/redis_lock_object_store.py`

 * *Files identical despite different names*

### Comparing `deltalake-redis-lock-0.0.1a5/setup.py` & `deltalake-redis-lock-0.0.1a6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['deltalake>=0.10.0,<0.11.0',
  'pandas==2.0.3',
  'pyarrow>=12.0.1,<13.0.0',
  'redis>=4.6.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'deltalake-redis-lock',
-    'version': '0.0.1a5',
+    'version': '0.0.1a6',
     'description': 'deltalake-redis-lock',
-    'long_description': '# deltalake-redis-lock\n\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/merge.yaml/badge.svg)\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/pr.yaml/badge.svg)\n\nA library creating an interface for a write lock for [delta-rs](https://pypi.org/project/deltalake/).\n\n## Library Usage\n\nWhen using this client, it can be used from multiple hosts. Below follow a minimal example\nto mimic this behaviour.\n\n### Redis Env Variables\n\nMake sure to set these `envs` before executing code.\n```bash\nREDIS_HOST=<host>\nREDIS_PORT=<port>  # default 6739\nREDIS_DB=<0>  # default 0\n```\n\n### Concurrent Write Example\n```python\n# run.py\nimport logging\nimport os\nimport string\nfrom random import choices\nfrom multiprocessing import Pool\n\nfrom pandas import DataFrame\n\nfrom deltalake_redis_lock import write_redis_lock_deltalake\n\ndef fake_worker(args):\n    df, table_name = args\n\n    logging.basicConfig(\n        level=logging.INFO,\n        format=\'%(asctime)s [%(levelname)s] %(message)s\',\n        datefmt=\'%Y-%m-%d %H:%M:%S\'\n    )\n\n    write_redis_lock_deltalake(\n        table_or_uri=f"{os.getcwd()}/{table_name}",\n        lock_table_name=table_name,\n        mode="append",\n        data=df,\n        overwrite_schema=True,\n    )\n\n\ndef define_datasets(_table_name: str) -> None:\n    df1 = DataFrame({"id": [1]})\n    df2 = DataFrame({"id": [2]})\n    df3 = DataFrame({"id": [3]})\n    df4 = DataFrame({"id": [4]})\n\n    datasets = [(df1, table_name), (df2, table_name), (df3, table_name), (df4, table_name)]\n\n    with Pool() as pool:\n        pool.map(fake_worker, datasets)\n\n\ndef generate_random_string(length):\n    return "".join(choices(string.ascii_lowercase, k=length))\n\n\nif __name__ == \'__main__\':\n    random_string = generate_random_string(3)\n    table_name = f"test_run_{random_string}"\n\n    define_datasets(_table_name=table_name)\n```\n\nThis can be exeucted with something like:\n\n```bash\nseq 2 | xargs -I{} -P 2 poetry run python run.py\n```\n\n## Setup From Scratch\n\n### Requirement\n\n* ^python3.9\n* poetry 1.1.13\n* make (GNU Make 3.81)\n\n### Setup\n\n```bash\nmake setup-environment\n```\n\nUpdate package\n```bash\nmake update\n```\n\n### Test\n\n```bash\nexport PYTHONPATH="${PYTHONPATH}:src"\nmake test type=unit\n```\n\n### Docker\n\nThe reason `docker` is used in the source code here, is to be able to build up an encapsulated\nenvironment of the codebase, and do `unit/integration and load tests`.\n\n```bash\nmake build-container-image DOCKER_BUILD="buildx build --platform linux/amd64" CONTEXT=.\n```\n\n```bash\nmake get-container-info-environment\nmake run-container-tests type=unit\n```\n',
+    'long_description': '# deltalake-redis-lock\n\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/merge.yaml/badge.svg)\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/pr.yaml/badge.svg)\n\nA library creating an interface for a write lock for [delta-rs](https://pypi.org/project/deltalake/).\n\n## Library Usage\n\nWhen using this client, it can be used from multiple hosts. Below follow a minimal example\nto mimic this behaviour.\n\n### Redis Env Variables\n\nMake sure to set these `envs` before executing code.\n```bash\nREDIS_HOST=<host>\nREDIS_PORT=<port>  # default 6739\nREDIS_DB=<0>  # default 0\n```\n\n### Concurrent Write Example\n```python\n# run.py\nimport logging\nimport os\nimport string\nfrom random import choices\nfrom multiprocessing import Pool\n\nfrom pandas import DataFrame\n\nfrom deltalake_redis_lock import write_redis_lock_deltalake\n\ndef fake_worker(args):\n    df, table_name = args\n\n    logging.basicConfig(\n        level=logging.INFO,\n        format=\'%(asctime)s [%(levelname)s] %(message)s\',\n        datefmt=\'%Y-%m-%d %H:%M:%S\'\n    )\n\n    write_redis_lock_deltalake(\n        table_or_uri=f"{os.getcwd()}/{table_name}",\n        lock_table_name=table_name,\n        mode="append",\n        data=df,\n        overwrite_schema=True,\n    )\n\n\ndef define_datasets(_table_name: str) -> None:\n    df1 = DataFrame({"id": [1]})\n    df2 = DataFrame({"id": [2]})\n    df3 = DataFrame({"id": [3]})\n    df4 = DataFrame({"id": [4]})\n\n    datasets = [(df1, table_name), (df2, table_name), (df3, table_name), (df4, table_name)]\n\n    with Pool() as pool:\n        pool.map(fake_worker, datasets)\n\n\ndef generate_random_string(length):\n    return "".join(choices(string.ascii_lowercase, k=length))\n\n\nif __name__ == \'__main__\':\n    random_string = generate_random_string(3)\n    table_name = f"test_run_{random_string}"\n\n    define_datasets(_table_name=table_name)\n```\n\nThis can be exeucted with something like:\n\n```bash\nseq 2 | xargs -I{} -P 2 poetry run python run.py\n```\n\n## Setup From Scratch\n\n### Requirement\n\n* ^python3.9\n* poetry 1.1.13\n* make (GNU Make 3.81)\n\n### Setup\n\n```bash\nmake setup-environment\n```\n\nUpdate package\n```bash\nmake update\n```\n\n### Test\n\n```bash\nexport PYTHONPATH="${PYTHONPATH}:src"\nmake test type=unit\n```\n\n### Docker\n\nThe reason `docker` is used in the source code here, is to be able to build up an encapsulated\nenvironment of the codebase, and do `unit/integration and load tests`.\n\n```bash\nmake build-container-image DOCKER_BUILD="buildx build --platform linux/amd64" CONTEXT=.\n```\n\n```bash\nmake run-container-tests type=unit\n```\n',
     'author': 'Simon Thelin',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/wrapbytes/deltalake-redis-lock',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `deltalake-redis-lock-0.0.1a5/PKG-INFO` & `deltalake-redis-lock-0.0.1a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltalake-redis-lock
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: deltalake-redis-lock
 Home-page: https://github.com/wrapbytes/deltalake-redis-lock
 License: MIT
 Author: Simon Thelin
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -130,11 +130,10 @@
 environment of the codebase, and do `unit/integration and load tests`.
 
 ```bash
 make build-container-image DOCKER_BUILD="buildx build --platform linux/amd64" CONTEXT=.
 ```
 
 ```bash
-make get-container-info-environment
 make run-container-tests type=unit
 ```
```

