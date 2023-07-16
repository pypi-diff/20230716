# Comparing `tmp/pyle38-0.9.0.tar.gz` & `tmp/pyle38-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyle38-0.9.0.tar", max compression
+gzip compressed data, was "pyle38-0.9.1.tar", max compression
```

## Comparing `pyle38-0.9.0.tar` & `pyle38-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1060 2022-09-30 18:51:29.820356 pyle38-0.9.0/LICENSE
--rw-r--r--   0        0        0    33180 2022-12-22 13:13:38.657753 pyle38-0.9.0/README.md
--rw-r--r--   0        0        0       50 2023-03-08 15:49:03.864821 pyle38-0.9.0/pyle38/__init__.py
--rw-r--r--   0        0        0     5165 2023-03-08 14:46:34.154734 pyle38-0.9.0/pyle38/client.py
--rw-r--r--   0        0        0        0 2022-09-30 18:51:29.821959 pyle38-0.9.0/pyle38/commands/__init__.py
--rw-r--r--   0        0        0      497 2022-09-30 18:51:29.822263 pyle38-0.9.0/pyle38/commands/executable.py
--rw-r--r--   0        0        0     2799 2023-01-25 11:16:51.475573 pyle38-0.9.0/pyle38/commands/fset.py
--rw-r--r--   0        0        0     2392 2022-11-29 20:55:35.813492 pyle38-0.9.0/pyle38/commands/get.py
--rw-r--r--   0        0        0    13905 2022-11-27 21:42:43.534653 pyle38-0.9.0/pyle38/commands/intersects.py
--rw-r--r--   0        0        0    10097 2022-11-27 21:42:43.535457 pyle38-0.9.0/pyle38/commands/nearby.py
--rw-r--r--   0        0        0     4189 2022-11-27 21:42:43.536056 pyle38-0.9.0/pyle38/commands/scan.py
--rw-r--r--   0        0        0     3193 2022-11-27 21:54:29.398209 pyle38-0.9.0/pyle38/commands/search.py
--rw-r--r--   0        0        0     2875 2022-11-29 21:06:38.799270 pyle38-0.9.0/pyle38/commands/set.py
--rw-r--r--   0        0        0     1648 2022-09-30 18:51:29.824023 pyle38-0.9.0/pyle38/commands/setchan.py
--rw-r--r--   0        0        0     1900 2022-09-30 18:51:29.824229 pyle38-0.9.0/pyle38/commands/sethook.py
--rw-r--r--   0        0        0     1388 2022-12-22 12:36:17.987731 pyle38-0.9.0/pyle38/commands/whereable.py
--rw-r--r--   0        0        0    13644 2023-01-25 10:58:14.222702 pyle38-0.9.0/pyle38/commands/within.py
--rw-r--r--   0        0        0      247 2022-11-30 21:16:48.254334 pyle38-0.9.0/pyle38/errors.py
--rw-r--r--   0        0        0     4210 2022-09-30 18:51:29.824842 pyle38-0.9.0/pyle38/follower.py
--rw-r--r--   0        0        0     4014 2022-09-30 18:51:29.825040 pyle38-0.9.0/pyle38/leader.py
--rw-r--r--   0        0        0     2862 2022-09-30 18:51:29.825229 pyle38-0.9.0/pyle38/models.py
--rw-r--r--   0        0        0     1096 2022-11-30 21:18:15.510659 pyle38-0.9.0/pyle38/parse_response.py
--rw-r--r--   0        0        0     7525 2022-11-29 21:05:28.160622 pyle38-0.9.0/pyle38/responses.py
--rw-r--r--   0        0        0      846 2022-09-30 18:51:29.825799 pyle38-0.9.0/pyle38/tile38.py
--rw-r--r--   0        0        0      286 2022-09-30 18:51:29.825924 pyle38-0.9.0/pyle38/utils.py
--rw-r--r--   0        0        0     2695 2023-03-08 15:49:03.865076 pyle38-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    34138 1970-01-01 00:00:00.000000 pyle38-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2022-09-30 18:51:29.820356 pyle38-0.9.1/LICENSE
+-rw-r--r--   0        0        0    33180 2022-12-22 13:13:38.657753 pyle38-0.9.1/README.md
+-rw-r--r--   0        0        0       50 2023-03-24 08:37:03.586816 pyle38-0.9.1/pyle38/__init__.py
+-rw-r--r--   0        0        0     5165 2023-03-08 14:46:34.154734 pyle38-0.9.1/pyle38/client.py
+-rw-r--r--   0        0        0        0 2022-09-30 18:51:29.821959 pyle38-0.9.1/pyle38/commands/__init__.py
+-rw-r--r--   0        0        0      497 2022-09-30 18:51:29.822263 pyle38-0.9.1/pyle38/commands/executable.py
+-rw-r--r--   0        0        0     2799 2023-01-25 11:16:51.475573 pyle38-0.9.1/pyle38/commands/fset.py
+-rw-r--r--   0        0        0     2392 2022-11-29 20:55:35.813492 pyle38-0.9.1/pyle38/commands/get.py
+-rw-r--r--   0        0        0    13905 2022-11-27 21:42:43.534653 pyle38-0.9.1/pyle38/commands/intersects.py
+-rw-r--r--   0        0        0    10097 2022-11-27 21:42:43.535457 pyle38-0.9.1/pyle38/commands/nearby.py
+-rw-r--r--   0        0        0     4189 2022-11-27 21:42:43.536056 pyle38-0.9.1/pyle38/commands/scan.py
+-rw-r--r--   0        0        0     3193 2022-11-27 21:54:29.398209 pyle38-0.9.1/pyle38/commands/search.py
+-rw-r--r--   0        0        0     2875 2022-11-29 21:06:38.799270 pyle38-0.9.1/pyle38/commands/set.py
+-rw-r--r--   0        0        0     1648 2022-09-30 18:51:29.824023 pyle38-0.9.1/pyle38/commands/setchan.py
+-rw-r--r--   0        0        0     1900 2022-09-30 18:51:29.824229 pyle38-0.9.1/pyle38/commands/sethook.py
+-rw-r--r--   0        0        0     1388 2022-12-22 12:36:17.987731 pyle38-0.9.1/pyle38/commands/whereable.py
+-rw-r--r--   0        0        0    13644 2023-01-25 10:58:14.222702 pyle38-0.9.1/pyle38/commands/within.py
+-rw-r--r--   0        0        0      247 2022-11-30 21:16:48.254334 pyle38-0.9.1/pyle38/errors.py
+-rw-r--r--   0        0        0     4210 2022-09-30 18:51:29.824842 pyle38-0.9.1/pyle38/follower.py
+-rw-r--r--   0        0        0     4014 2022-09-30 18:51:29.825040 pyle38-0.9.1/pyle38/leader.py
+-rw-r--r--   0        0        0     2862 2022-09-30 18:51:29.825229 pyle38-0.9.1/pyle38/models.py
+-rw-r--r--   0        0        0     1096 2022-11-30 21:18:15.510659 pyle38-0.9.1/pyle38/parse_response.py
+-rw-r--r--   0        0        0     7525 2022-11-29 21:05:28.160622 pyle38-0.9.1/pyle38/responses.py
+-rw-r--r--   0        0        0      846 2022-09-30 18:51:29.825799 pyle38-0.9.1/pyle38/tile38.py
+-rw-r--r--   0        0        0      286 2022-09-30 18:51:29.825924 pyle38-0.9.1/pyle38/utils.py
+-rw-r--r--   0        0        0     2757 2023-03-24 08:37:03.587084 pyle38-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    34138 1970-01-01 00:00:00.000000 pyle38-0.9.1/PKG-INFO
```

### Comparing `pyle38-0.9.0/LICENSE` & `pyle38-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/README.md` & `pyle38-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/client.py` & `pyle38-0.9.1/pyle38/client.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/fset.py` & `pyle38-0.9.1/pyle38/commands/fset.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/get.py` & `pyle38-0.9.1/pyle38/commands/get.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/intersects.py` & `pyle38-0.9.1/pyle38/commands/intersects.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/nearby.py` & `pyle38-0.9.1/pyle38/commands/nearby.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/scan.py` & `pyle38-0.9.1/pyle38/commands/scan.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/search.py` & `pyle38-0.9.1/pyle38/commands/search.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/set.py` & `pyle38-0.9.1/pyle38/commands/set.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/setchan.py` & `pyle38-0.9.1/pyle38/commands/setchan.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/sethook.py` & `pyle38-0.9.1/pyle38/commands/sethook.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/whereable.py` & `pyle38-0.9.1/pyle38/commands/whereable.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/commands/within.py` & `pyle38-0.9.1/pyle38/commands/within.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/follower.py` & `pyle38-0.9.1/pyle38/follower.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/leader.py` & `pyle38-0.9.1/pyle38/leader.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/models.py` & `pyle38-0.9.1/pyle38/models.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/parse_response.py` & `pyle38-0.9.1/pyle38/parse_response.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/responses.py` & `pyle38-0.9.1/pyle38/responses.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyle38/tile38.py` & `pyle38-0.9.1/pyle38/tile38.py`

 * *Files identical despite different names*

### Comparing `pyle38-0.9.0/pyproject.toml` & `pyle38-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyle38"
-version = "0.9.0"
+version = "0.9.1"
 description = "Async python client for Tile38"
 authors = ["Benjamin Ramser <ahoi@iwpnd.pw>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iwpnd/pyle38"
 repository = "https://github.com/iwpnd/pyle38"
 keywords = ["tile38", "async", "client"]
@@ -18,29 +18,29 @@
     "License :: OSI Approved :: MIT License",
     "Typing :: Typed"]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.8.1"
-redis = "^4.3.4"
+redis = "^4.5.3"
 
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.3.21.5"
 pytest = "^7.2.2"
 pre-commit = ">=2.20,<4.0"
 black = "^23.1.0"
-pytest-asyncio = "^0.20.2"
+pytest-asyncio = ">=0.20.2,<0.22.0"
 gitlint = "^0.19.0"
 poethepoet = ">=0.16.4,<0.19.0"
 isort = "^5.10.1"
 pytest-cov = "^4.0.0"
 mypy = ">=0.991,<1.2"
 python-semantic-release = "^7.32.1"
-ruff = "^0.0.254"
+ruff = ">=0.0.254,<0.0.258"
 
 [tool.semantic_release]
 version_variable = [
     "pyle38/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 commit_subject = "ci: release v{version}"
@@ -99,13 +99,13 @@
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.poe.tasks]
 test       = "poetry run pytest -vv --asyncio-mode=auto -s tests/"
-test-cov   = "poetry run pytest -vv --asyncio-mode=auto -s --cov=pyle38 tests/"
+test-cov   = "poetry run pytest -vv --asyncio-mode=auto -s --cov=pyle38 tests/ --cov-report xml:/home/runner/coverage.xml"
 mypy       = "poetry run mypy --ignore-missing-imports --config-file pyproject.toml"
 lint       = "ruff ."
 up         = "docker-compose up"
 down       = "docker-compose down"
 publish    = "poetry run semantic-release publish"
```

### Comparing `pyle38-0.9.0/PKG-INFO` & `pyle38-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyle38
-Version: 0.9.0
+Version: 0.9.1
 Summary: Async python client for Tile38
 Home-page: https://github.com/iwpnd/pyle38
 License: MIT
 Keywords: tile38,async,client
 Author: Benjamin Ramser
 Author-email: ahoi@iwpnd.pw
 Requires-Python: >=3.10,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: pydantic (>=1.8.1,<2.0.0)
-Requires-Dist: redis (>=4.3.4,<5.0.0)
+Requires-Dist: redis (>=4.5.3,<5.0.0)
 Project-URL: Repository, https://github.com/iwpnd/pyle38
 Description-Content-Type: text/markdown
 
 <br  />
 <br  />
 <p align="center">
 <img  src=".github/img/pyle38.png" height="40%" width="40%" alt="Logo">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: pyle38 Version: 0.9.0 Summary: Async python client
+Metadata-Version: 2.1 Name: pyle38 Version: 0.9.1 Summary: Async python client
 for Tile38 Home-page: https://github.com/iwpnd/pyle38 License: MIT Keywords:
 tile38,async,client Author: Benjamin Ramser Author-email: ahoi@iwpnd.pw
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Database :: Front-Ends Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed Requires-Dist: pydantic (>=1.8.1,<2.0.0) Requires-
-Dist: redis (>=4.3.4,<5.0.0) Project-URL: Repository, https://github.com/iwpnd/
+Dist: redis (>=4.5.3,<5.0.0) Project-URL: Repository, https://github.com/iwpnd/
 pyle38 Description-Content-Type: text/markdown
 
                                     [Logo]
                    iwpnd.pw Â· Report_Bug Â· Request_Feature
 ## About The Project This is an asynchonous Python client for Tile38 that
 allows for fast and easy interaction with the worlds fastest in-memory
 geodatabase [Tile38](https://www.tile38.com). Check out my introductory blog
```

