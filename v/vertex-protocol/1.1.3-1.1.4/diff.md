# Comparing `tmp/vertex_protocol-1.1.3.tar.gz` & `tmp/vertex_protocol-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-1.1.3.tar", max compression
+gzip compressed data, was "vertex_protocol-1.1.4.tar", max compression
```

## Comparing `vertex_protocol-1.1.3.tar` & `vertex_protocol-1.1.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     3337 2023-06-20 02:41:13.736585 vertex_protocol-1.1.3/README.md
--rw-r--r--   0        0        0     1664 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     6634 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     3404 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10101 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4782 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2964 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     3193 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2554 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     8264 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    11702 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    16980 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     4723 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    21812 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     8410 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    18858 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1013 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
--rw-r--r--   0        0        0      993 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0      908 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.test.json
--rw-r--r--   0        0        0      426 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1189 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2484 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     4636 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2747 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    18498 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    11206 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     5739 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    18440 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     3429 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0     9841 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    11233 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0     2979 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5625 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    12117 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      341 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5301 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0       99 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/enum.py
--rw-r--r--   0        0        0     1136 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0      927 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     2089 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      863 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      503 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3337 2023-07-16 02:48:38.444834 vertex_protocol-1.1.4/README.md
+-rw-r--r--   0        0        0     1664 2023-07-16 02:48:38.444834 vertex_protocol-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     6634 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     3404 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10101 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4782 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2964 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     3669 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2554 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     8786 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    13215 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    17205 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     5677 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    19201 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     6291 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    16739 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1013 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
+-rw-r--r--   0        0        0      993 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      908 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0      426 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1189 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2484 2023-07-16 02:48:38.448834 vertex_protocol-1.1.4/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     4636 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2914 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    18498 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    11206 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     5739 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    18440 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     3429 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0     9841 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    11793 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0     3077 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5656 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    12832 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      341 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5301 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0      927 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     2089 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      863 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      503 2023-07-16 02:48:38.452834 vertex_protocol-1.1.4/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.4/PKG-INFO
```

### Comparing `vertex_protocol-1.1.3/README.md` & `vertex_protocol-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/pyproject.toml` & `vertex_protocol-1.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vertex-protocol"
-version = "1.1.3"
+version = "1.1.4"
 description = "Vertex Protocol SDK"
 authors = ["Jeury Mejia <jeury@vertexprotocol.com>"]
 homepage = "https://vertexprotocol.com/"
 maintainers = [
   "Frank Jia <frank@vertexprotocol.com>",
   "Clark Oh-Willeke <clark@vertexprotocol.com>"
 ]
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/base.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/market/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/market/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/spot/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-1.1.4/vertex_protocol/client/apis/subaccount/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from vertex_protocol.engine_client.types.query import (
     FeeRatesData,
     QuerySubaccountInfoTx,
     SubaccountInfoData,
 )
 from vertex_protocol.indexer_client.types.query import (
     IndexerLinkedSignerRateLimitData,
+    IndexerReferralCodeData,
     IndexerTokenRewardsData,
 )
 
 
 class SubaccountQueryAPI(VertexBaseAPI):
     """
     Provides functionalities for querying data related to subaccounts in the Vertex Protocol.
@@ -73,7 +74,19 @@
         Args:
             subaccount (str): Unique identifier for the subaccount.
 
         Returns:
             IndexerLinkedSignerRateLimitData: A data class object containing information about the current linked signer and their rate limits for the queried subaccount.
         """
         return self.context.indexer_client.get_linked_signer_rate_limits(subaccount)
+
+    def get_referral_code(self, subaccount: str) -> IndexerReferralCodeData:
+        """
+        Query the referral code for the specified wallet from the indexer.
+
+        Args:
+            subaccount (str): Unique identifier for the subaccount.
+
+        Returns:
+            IndexerReferralCodeData: A data class object containing the wallet's referral code.
+        """
+        return self.context.indexer_client.get_referral_code(subaccount)
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/client/context.py` & `vertex_protocol-1.1.4/vertex_protocol/client/context.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/contracts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 from web3 import Web3
 from web3.types import TxParams
 from web3.contract import Contract
 from web3.contract.contract import ContractFunction
 from eth_account.signers.local import LocalAccount
 from vertex_protocol.contracts.loader import load_abi
 from vertex_protocol.contracts.types import DepositCollateralParams, VertexAbiName
-from vertex_protocol.utils.bytes32 import subaccount_name_to_bytes12, zero_address
+from vertex_protocol.utils.bytes32 import (
+    hex_to_bytes32,
+    str_to_hex,
+    subaccount_name_to_bytes12,
+    zero_address,
+)
 from vertex_protocol.utils.exceptions import InvalidProductId
 from vertex_protocol.contracts.types import *
 
 
 class VertexContractsContext(BaseModel):
     """
     Holds the context for various Vertex contracts.
@@ -104,22 +109,33 @@
 
             signer (LocalAccount): The account that will sign the deposit transaction.
 
         Returns:
             str: The transaction hash of the deposit operation.
         """
         params = DepositCollateralParams.parse_obj(params)
-        return self.execute(
-            self.endpoint.functions.depositCollateral(
-                subaccount_name_to_bytes12(params.subaccount_name),
-                params.product_id,
-                params.amount,
-            ),
-            signer,
-        )
+        if params.referral_code is not None and params.referral_code.strip():
+            return self.execute(
+                self.endpoint.functions.depositCollateralWithReferral(
+                    subaccount_name_to_bytes12(params.subaccount_name),
+                    params.product_id,
+                    params.amount,
+                    params.referral_code,
+                ),
+                signer,
+            )
+        else:
+            return self.execute(
+                self.endpoint.functions.depositCollateral(
+                    subaccount_name_to_bytes12(params.subaccount_name),
+                    params.product_id,
+                    params.amount,
+                ),
+                signer,
+            )
 
     def approve_allowance(self, erc20: Contract, amount: int, signer: LocalAccount):
         """
         Approves a specified amount of allowance for the ERC20 token contract.
 
         Args:
             erc20 (Contract): The ERC20 token contract.
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8974358974358975%*

 * *Differences: {'insert': "[(4, OrderedDict([('anonymous', False), ('inputs', [OrderedDict([('indexed', False), "*

 * *           "('internalType', 'address'), ('name', 'invitee'), ('type', 'address')]), "*

 * *           "OrderedDict([('indexed', False), ('internalType', 'bytes32'), ('name', "*

 * *           "'referralCode'), ('type', 'bytes32')])]), ('name', 'UserReferral'), ('type', "*

 * *           "'event')])), (7, OrderedDict([('inputs', [OrderedDict([('internalType', 'bytes12'), "*

 * *           "('name', 'subaccountName'), ('type', 'by […]*

```diff
@@ -59,14 +59,33 @@
     {
         "anonymous": false,
         "inputs": [],
         "name": "SubmitTransactions",
         "type": "event"
     },
     {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "invitee",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes32",
+                "name": "referralCode",
+                "type": "bytes32"
+            }
+        ],
+        "name": "UserReferral",
+        "type": "event"
+    },
+    {
         "inputs": [],
         "name": "clearinghouse",
         "outputs": [
             {
                 "internalType": "contract IClearinghouse",
                 "name": "",
                 "type": "address"
@@ -97,14 +116,42 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "bytes12",
+                "name": "subaccountName",
+                "type": "bytes12"
+            },
+            {
+                "internalType": "uint32",
+                "name": "productId",
+                "type": "uint32"
+            },
+            {
+                "internalType": "uint128",
+                "name": "amount",
+                "type": "uint128"
+            },
+            {
+                "internalType": "string",
+                "name": "referralCode",
+                "type": "string"
+            }
+        ],
+        "name": "depositCollateralWithReferral",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "uint32",
                 "name": "count",
                 "type": "uint32"
             }
         ],
         "name": "executeSlowModeTransactions",
         "outputs": [],
@@ -387,14 +434,33 @@
         ],
         "name": "processSlowModeTransaction",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "name": "referralCodes",
+        "outputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "renounceOwnership",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
@@ -493,14 +559,27 @@
                 "type": "uint64"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "slowModeFees",
+        "outputs": [
+            {
+                "internalType": "int128",
+                "name": "",
+                "type": "int128"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint64",
                 "name": "",
                 "type": "uint64"
             }
         ],
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9572222222222223%*

 * *Differences: {'12': "{'name': 'getInsurance', 'outputs': {0: {'internalType': 'int128', 'type': 'int128', "*

 * *       "delete: ['components']}}}",*

 * * '13': "{'name': 'getMaxHealthGroup', 'outputs': {0: {'internalType': 'uint32', 'type': "*

 * *       "'uint32'}}}",*

 * * 'insert': "[(5, OrderedDict([('inputs', [OrderedDict([('components', "*

 * *           "[OrderedDict([('internalType', 'bytes32'), ('name', 'subaccount'), ('type', "*

 * *           "'bytes32')])]), ('internalType', 'struct IEndpoint.ClaimSequencerFees'), ('name', "*

 * *            […]*

```diff
@@ -153,14 +153,39 @@
     },
     {
         "inputs": [
             {
                 "components": [
                     {
                         "internalType": "bytes32",
+                        "name": "subaccount",
+                        "type": "bytes32"
+                    }
+                ],
+                "internalType": "struct IEndpoint.ClaimSequencerFees",
+                "name": "tx",
+                "type": "tuple"
+            },
+            {
+                "internalType": "int128[]",
+                "name": "fees",
+                "type": "int128[]"
+            }
+        ],
+        "name": "claimSequencerFees",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "components": [
+                    {
+                        "internalType": "bytes32",
                         "name": "sender",
                         "type": "bytes32"
                     },
                     {
                         "internalType": "uint32",
                         "name": "productId",
                         "type": "uint32"
@@ -274,45 +299,33 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getHealthGroups",
+        "name": "getInsurance",
         "outputs": [
             {
-                "components": [
-                    {
-                        "internalType": "uint32",
-                        "name": "spotId",
-                        "type": "uint32"
-                    },
-                    {
-                        "internalType": "uint32",
-                        "name": "perpId",
-                        "type": "uint32"
-                    }
-                ],
-                "internalType": "struct IClearinghouseState.HealthGroup[]",
+                "internalType": "int128",
                 "name": "",
-                "type": "tuple[]"
+                "type": "int128"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getInsurance",
+        "name": "getMaxHealthGroup",
         "outputs": [
             {
-                "internalType": "int128",
+                "internalType": "uint32",
                 "name": "",
-                "type": "int128"
+                "type": "uint32"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {'insert': "[(2, OrderedDict([('anonymous', False), ('inputs', [OrderedDict([('indexed', False), "*

 * *           "('internalType', 'address'), ('name', 'invitee'), ('type', 'address')]), "*

 * *           "OrderedDict([('indexed', False), ('internalType', 'bytes32'), ('name', "*

 * *           "'referralCode'), ('type', 'bytes32')])]), ('name', 'UserReferral'), ('type', "*

 * *           "'event')])), (4, OrderedDict([('inputs', [OrderedDict([('internalType', 'bytes12'), "*

 * *           "('name', 'subaccountName'), ('type', 'by […]*

```diff
@@ -27,14 +27,33 @@
     {
         "anonymous": false,
         "inputs": [],
         "name": "SubmitTransactions",
         "type": "event"
     },
     {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "invitee",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes32",
+                "name": "referralCode",
+                "type": "bytes32"
+            }
+        ],
+        "name": "UserReferral",
+        "type": "event"
+    },
+    {
         "inputs": [
             {
                 "internalType": "bytes12",
                 "name": "subaccountName",
                 "type": "bytes12"
             },
             {
@@ -52,14 +71,42 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "bytes12",
+                "name": "subaccountName",
+                "type": "bytes12"
+            },
+            {
+                "internalType": "uint32",
+                "name": "productId",
+                "type": "uint32"
+            },
+            {
+                "internalType": "uint128",
+                "name": "amount",
+                "type": "uint128"
+            },
+            {
+                "internalType": "string",
+                "name": "referralCode",
+                "type": "string"
+            }
+        ],
+        "name": "depositCollateralWithReferral",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "address",
                 "name": "sender",
                 "type": "address"
             }
         ],
         "name": "getNonce",
         "outputs": [
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'delete': '[5, 4, 3, 2, 1]'}*

```diff
@@ -9,145 +9,14 @@
                 "type": "uint32"
             }
         ],
         "name": "AddProduct",
         "type": "event"
     },
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "subaccount",
-                "type": "bytes32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "lpAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "baseAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "quoteAmount",
-                "type": "int128"
-            }
-        ],
-        "name": "BurnLp",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "subaccount",
-                "type": "bytes32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "lpAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "baseAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "quoteAmount",
-                "type": "int128"
-            }
-        ],
-        "name": "MintLp",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            }
-        ],
-        "name": "ProductUpdate",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "subaccount",
-                "type": "bytes32"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "amount",
-                "type": "int128"
-            }
-        ],
-        "name": "SettlePnl",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "amountSocialized",
-                "type": "int128"
-            }
-        ],
-        "name": "SocializeProduct",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "components": [
                     {
                         "internalType": "uint32",
                         "name": "productId",
                         "type": "uint32"
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7647058823529411%*

 * *Differences: {'delete': '[4, 3, 2, 1]'}*

```diff
@@ -9,120 +9,14 @@
                 "type": "uint32"
             }
         ],
         "name": "AddProduct",
         "type": "event"
     },
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "subaccount",
-                "type": "bytes32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "lpAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "baseAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "quoteAmount",
-                "type": "int128"
-            }
-        ],
-        "name": "BurnLp",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "subaccount",
-                "type": "bytes32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "lpAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "baseAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "quoteAmount",
-                "type": "int128"
-            }
-        ],
-        "name": "MintLp",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            }
-        ],
-        "name": "ProductUpdate",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "amountSocialized",
-                "type": "int128"
-            }
-        ],
-        "name": "SocializeProduct",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "components": [
                     {
                         "internalType": "uint32",
                         "name": "productId",
                         "type": "uint32"
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': '[4, 3, 2, 1]'}*

```diff
@@ -9,120 +9,14 @@
                 "type": "uint32"
             }
         ],
         "name": "AddProduct",
         "type": "event"
     },
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "subaccount",
-                "type": "bytes32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "lpAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "baseAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "quoteAmount",
-                "type": "int128"
-            }
-        ],
-        "name": "BurnLp",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "subaccount",
-                "type": "bytes32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "lpAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "baseAmount",
-                "type": "int128"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "quoteAmount",
-                "type": "int128"
-            }
-        ],
-        "name": "MintLp",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            }
-        ],
-        "name": "ProductUpdate",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "uint32",
-                "name": "productId",
-                "type": "uint32"
-            },
-            {
-                "indexed": false,
-                "internalType": "int128",
-                "name": "amountSocialized",
-                "type": "int128"
-            }
-        ],
-        "name": "SocializeProduct",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "components": [
                     {
                         "internalType": "uint32",
                         "name": "productId",
                         "type": "uint32"
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.test.json` & `vertex_protocol-1.1.4/vertex_protocol/contracts/deployments/deployment.test.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-1.1.4/vertex_protocol/contracts/eip712/domain.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-1.1.4/vertex_protocol/contracts/eip712/sign.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/types.py` & `vertex_protocol-1.1.4/vertex_protocol/contracts/eip712/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/loader.py` & `vertex_protocol-1.1.4/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/contracts/types.py` & `vertex_protocol-1.1.4/vertex_protocol/contracts/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from pydantic import AnyUrl, Field
 from vertex_protocol.utils.enum import StrEnum
 
 from vertex_protocol.utils.model import VertexBaseModel
 
 
 class VertexNetwork(StrEnum):
@@ -32,20 +33,27 @@
 
 class VertexDeployment(VertexBaseModel):
     """
     Class representing deployment data for Vertex protocol contracts.
 
     Attributes:
         node_url (AnyUrl): The URL of the node.
+
         quote_addr (str): The address of the quote contract.
+
         querier_addr (str): The address of the querier contract.
+
         fee_calculator_addr (str): The address of the fee calculator contract.
+
         clearinghouse_addr (str): The address of the clearinghouse contract.
+
         endpoint_addr (str): The address of the endpoint contract.
+
         spot_engine_addr (str): The address of the spot engine contract.
+
         perp_engine_addr (str): The address of the perpetual engine contract.
     """
 
     node_url: AnyUrl = Field(alias="nodeUrl")
     quote_addr: str = Field(alias="quote")
     querier_addr: str = Field(alias="querier")
     fee_calculator_addr: str = Field(alias="feeCalculator")
@@ -61,19 +69,22 @@
 
     Attributes:
         subaccount_name (str): The name of the subaccount.
 
         product_id (int): The ID of the spot product to deposit collateral for.
 
         amount (int): The amount of collateral to be deposited.
+
+        referral_code (Optional[str]): Use this to indicate you were referred by existing member.
     """
 
     subaccount_name: str
     product_id: int
     amount: int
+    referral_code: Optional[str]
 
 
 class VertexExecuteType(StrEnum):
     """
     Enumeration of possible actions to execute in Vertex.
     """
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/engine_client/execute.py` & `vertex_protocol-1.1.4/vertex_protocol/engine_client/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/engine_client/query.py` & `vertex_protocol-1.1.4/vertex_protocol/engine_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/engine_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-1.1.4/vertex_protocol/engine_client/types/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-1.1.4/vertex_protocol/engine_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-1.1.4/vertex_protocol/engine_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/indexer_client/query.py` & `vertex_protocol-1.1.4/vertex_protocol/indexer_client/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     IndexerCandlesticksData,
     IndexerEventsParams,
     IndexerEventsData,
     IndexerFundingRateParams,
     IndexerFundingRateData,
     IndexerHistoricalOrdersByDigestParams,
     IndexerHistoricalOrdersData,
+    IndexerReferralCodeData,
+    IndexerReferralCodeParams,
     IndexerSubaccountHistoricalOrdersParams,
     IndexerLinkedSignerRateLimitData,
     IndexerLinkedSignerRateLimitParams,
     IndexerLiquidationFeedData,
     IndexerLiquidationFeedParams,
     IndexerMakerStatisticsData,
     IndexerMakerStatisticsParams,
@@ -312,7 +314,22 @@
         Returns:
             IndexerLinkedSignerRateLimitData: The rate limits for the linked signer of the specified subaccount.
         """
         return ensure_data_type(
             self.query(IndexerLinkedSignerRateLimitParams(subaccount=subaccount)).data,
             IndexerLinkedSignerRateLimitData,
         )
+
+    def get_referral_code(self, subaccount: str) -> IndexerReferralCodeData:
+        """
+        Retrieves the referral code for a given address.
+
+        Args:
+            subaccount (str): Unique identifier for the subaccount.
+
+        Returns:
+            IndexerReferralCodeData: The referral code for the specific address.
+        """
+        return ensure_data_type(
+            self.query(IndexerReferralCodeParams(subaccount=subaccount)).data,
+            IndexerReferralCodeData,
+        )
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/indexer_client/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,41 +31,44 @@
     "IndexerFundingRateParams",
     "IndexerPerpPricesParams",
     "IndexerOraclePricesParams",
     "IndexerTokenRewardsParams",
     "IndexerMakerStatisticsParams",
     "IndexerLiquidationFeedParams",
     "IndexerLinkedSignerRateLimitParams",
+    "IndexerReferralCodeParams",
     "IndexerParams",
     "IndexerHistoricalOrdersRequest",
     "IndexerMatchesRequest",
     "IndexerEventsRequest",
     "IndexerSubaccountSummaryRequest",
     "IndexerProductSnapshotsRequest",
     "IndexerCandlesticksRequest",
     "IndexerFundingRateRequest",
     "IndexerPerpPricesRequest",
     "IndexerOraclePricesRequest",
     "IndexerTokenRewardsRequest",
     "IndexerMakerStatisticsRequest",
     "IndexerLiquidationFeedRequest",
     "IndexerLinkedSignerRateLimitRequest",
+    "IndexerReferralCodeRequest",
     "IndexerRequest",
     "IndexerHistoricalOrdersData",
     "IndexerMatchesData",
     "IndexerEventsData",
     "IndexerSubaccountSummaryData",
     "IndexerProductSnapshotsData",
     "IndexerCandlesticksData",
     "IndexerFundingRateData",
     "IndexerPerpPricesData",
     "IndexerOraclePricesData",
     "IndexerTokenRewardsData",
     "IndexerMakerStatisticsData",
     "IndexerLinkedSignerRateLimitData",
+    "IndexerReferralCodeData",
     "IndexerLiquidationFeedData",
     "IndexerResponseData",
     "IndexerResponse",
     "IndexerEventType",
     "IndexerCandlesticksGranularity",
     "IndexerBaseModel",
     "IndexerBaseOrder",
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-1.1.4/vertex_protocol/indexer_client/types/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,15 @@
     uptime: int
     maker_volume: str
     taker_volume: str
     maker_fee: str
     taker_fee: str
     maker_tokens: str
     taker_tokens: str
+    taker_referral_tokens: str
     rebates: str
 
 
 class IndexerGlobalRewards(VertexBaseModel):
     product_id: int
     reward_coefficient: str
     q_scores: str
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-1.1.4/vertex_protocol/indexer_client/types/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     FUNDING_RATE = "funding_rate"
     PERP_PRICES = "price"
     ORACLE_PRICES = "oracle_price"
     REWARDS = "rewards"
     MAKER_STATISTICS = "maker_statistics"
     LIQUIDATION_FEED = "liquidation_feed"
     LINKED_SIGNER_RATE_LIMIT = "linked_signer_rate_limit"
+    REFERRAL_CODE = "referral_code"
 
 
 class IndexerBaseParams(VertexBaseModel):
     """
     Base parameters for the indexer queries.
     """
 
@@ -188,14 +189,22 @@
     """
     Parameters for querying linked signer rate limits.
     """
 
     subaccount: str
 
 
+class IndexerReferralCodeParams(VertexBaseModel):
+    """
+    Parameters for querying a referral code.
+    """
+
+    subaccount: str
+
+
 IndexerParams = Union[
     IndexerSubaccountHistoricalOrdersParams,
     IndexerHistoricalOrdersByDigestParams,
     IndexerMatchesParams,
     IndexerEventsParams,
     IndexerSubaccountSummaryParams,
     IndexerProductSnapshotsParams,
@@ -203,14 +212,15 @@
     IndexerFundingRateParams,
     IndexerPerpPricesParams,
     IndexerOraclePricesParams,
     IndexerTokenRewardsParams,
     IndexerMakerStatisticsParams,
     IndexerLiquidationFeedParams,
     IndexerLinkedSignerRateLimitParams,
+    IndexerReferralCodeParams,
 ]
 
 
 class IndexerHistoricalOrdersRequest(VertexBaseModel):
     """
     Request object for querying historical orders.
     """
@@ -312,28 +322,37 @@
     """
     Request object for querying linked signer rate limits.
     """
 
     linked_signer_rate_limit: IndexerLinkedSignerRateLimitParams
 
 
+class IndexerReferralCodeRequest(VertexBaseModel):
+    """
+    Request object for querying a referral code.
+    """
+
+    referral_code: IndexerReferralCodeParams
+
+
 IndexerRequest = Union[
     IndexerHistoricalOrdersRequest,
     IndexerMatchesRequest,
     IndexerEventsRequest,
     IndexerSubaccountSummaryRequest,
     IndexerProductSnapshotsRequest,
     IndexerCandlesticksRequest,
     IndexerFundingRateRequest,
     IndexerPerpPricesRequest,
     IndexerOraclePricesRequest,
     IndexerTokenRewardsRequest,
     IndexerMakerStatisticsRequest,
     IndexerLiquidationFeedRequest,
     IndexerLinkedSignerRateLimitRequest,
+    IndexerReferralCodeRequest,
 ]
 
 
 class IndexerHistoricalOrdersData(VertexBaseModel):
     """
     Data object for historical orders.
     """
@@ -416,14 +435,15 @@
 class IndexerTokenRewardsData(VertexBaseModel):
     """
     Data object for token rewards.
     """
 
     rewards: list[IndexerTokenReward]
     update_time: str
+    total_referrals: str
 
 
 class IndexerMakerStatisticsData(VertexBaseModel):
     """
     Data object for maker statistics.
     """
 
@@ -438,14 +458,22 @@
 
     remaining_tx: str
     total_tx_limit: str
     wait_time: int
     signer: str
 
 
+class IndexerReferralCodeData(VertexBaseModel):
+    """
+    Data object for referral codes.
+    """
+
+    referral_code: str
+
+
 IndexerLiquidationFeedData = list[IndexerLiquidatableAccount]
 
 
 IndexerResponseData = Union[
     IndexerHistoricalOrdersData,
     IndexerMatchesData,
     IndexerEventsData,
@@ -454,14 +482,15 @@
     IndexerCandlesticksData,
     IndexerFundingRateData,
     IndexerPerpPricesData,
     IndexerOraclePricesData,
     IndexerTokenRewardsData,
     IndexerMakerStatisticsData,
     IndexerLinkedSignerRateLimitData,
+    IndexerReferralCodeData,
     IndexerLiquidationFeedData,
 ]
 
 
 class IndexerResponse(VertexBaseModel):
     """
     Represents the response returned by the indexer.
@@ -530,11 +559,15 @@
             IndexerLiquidationFeedRequest,
             IndexerQueryType.LIQUIDATION_FEED.value,
         ),
         IndexerLinkedSignerRateLimitParams: (
             IndexerLinkedSignerRateLimitRequest,
             IndexerQueryType.LINKED_SIGNER_RATE_LIMIT.value,
         ),
+        IndexerReferralCodeParams: (
+            IndexerReferralCodeRequest,
+            IndexerQueryType.REFERRAL_CODE.value,
+        ),
     }
 
     RequestClass, field_name = indexer_request_mapping[type(params)]
     return RequestClass(**{field_name: params})
```

### Comparing `vertex_protocol-1.1.3/vertex_protocol/utils/__init__.py` & `vertex_protocol-1.1.4/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/utils/bytes32.py` & `vertex_protocol-1.1.4/vertex_protocol/utils/bytes32.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/utils/exceptions.py` & `vertex_protocol-1.1.4/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/utils/expiration.py` & `vertex_protocol-1.1.4/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/utils/math.py` & `vertex_protocol-1.1.4/vertex_protocol/utils/math.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/utils/model.py` & `vertex_protocol-1.1.4/vertex_protocol/utils/model.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/vertex_protocol/utils/nonce.py` & `vertex_protocol-1.1.4/vertex_protocol/utils/nonce.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.3/PKG-INFO` & `vertex_protocol-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 1.1.3
+Version: 1.1.4
 Summary: Vertex Protocol SDK
 Home-page: https://vertexprotocol.com/
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
 Maintainer: Frank Jia
 Maintainer-email: frank@vertexprotocol.com
```

