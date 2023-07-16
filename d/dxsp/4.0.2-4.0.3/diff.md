# Comparing `tmp/dxsp-4.0.2.tar.gz` & `tmp/dxsp-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.0.2.tar", max compression
+gzip compressed data, was "dxsp-4.0.3.tar", max compression
```

## Comparing `dxsp-4.0.2.tar` & `dxsp-4.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-14 21:37:55.456406 dxsp-4.0.2/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-14 21:37:55.456406 dxsp-4.0.2/README.md
--rw-r--r--   0        0        0      115 2023-07-14 21:37:56.560520 dxsp-4.0.2/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/config.py
--rw-r--r--   0        0        0    10529 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5622 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1835 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1036 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4636 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6590 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1989 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-14 21:37:55.456406 dxsp-4.0.2/dxsp/utils/utils.py
--rw-r--r--   0        0        0     2328 2023-07-14 21:37:56.560520 dxsp-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 dxsp-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-16 20:54:38.807265 dxsp-4.0.3/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-16 20:54:38.807265 dxsp-4.0.3/README.md
+-rw-r--r--   0        0        0      115 2023-07-16 20:54:39.619277 dxsp-4.0.3/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-16 20:54:38.807265 dxsp-4.0.3/dxsp/config.py
+-rw-r--r--   0        0        0    10529 2023-07-16 20:54:38.807265 dxsp-4.0.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5622 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1835 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1036 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4636 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6590 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1989 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     2327 2023-07-16 20:54:39.619277 dxsp-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 dxsp-4.0.3/PKG-INFO
```

### Comparing `dxsp-4.0.2/LICENSE` & `dxsp-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/README.md` & `dxsp-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/default_settings.toml` & `dxsp-4.0.3/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/main.py` & `dxsp-4.0.3/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/protocols/oneinch.py` & `dxsp-4.0.3/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/protocols/uniswap.py` & `dxsp-4.0.3/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/protocols/zerox.py` & `dxsp-4.0.3/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/utils/account_utils.py` & `dxsp-4.0.3/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/utils/contract_utils.py` & `dxsp-4.0.3/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/dxsp/utils/explorer_utils.py` & `dxsp-4.0.3/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.2/pyproject.toml` & `dxsp-4.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.0.2"
+version = "4.0.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -23,15 +23,15 @@
 python = "^3.10"
 dynaconf = "^3.1.12"
 web3 = "^6.4.0"
 pycoingecko = "^3.1.0"
 uniswap-python = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
-python-semantic-release = "^7.34.3"
+python-semantic-release = "^8.0.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
```

### Comparing `dxsp-4.0.2/PKG-INFO` & `dxsp-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.0.2
+Version: 4.0.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.0.2 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.0.3 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

