# Comparing `tmp/empiric_network-1.6.5.tar.gz` & `tmp/empiric_network-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.6.5.tar", max compression
+gzip compressed data, was "empiric_network-1.6.6.tar", max compression
```

## Comparing `empiric_network-1.6.5.tar` & `empiric_network-1.6.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      284 2023-07-14 15:37:41.069850 empiric_network-1.6.5/README.md
--rw-r--r--   0        0        0        0 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/__init__.py
--rw-r--r--   0        0        0      193 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    14135 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4232 2023-07-14 15:37:41.069850 empiric_network-1.6.5/empiric/core/client.py
--rw-r--r--   0        0        0     2618 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/config.py
--rw-r--r--   0        0        0     3797 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/contract.py
--rw-r--r--   0        0        0     9972 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0    25441 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     8808 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     4177 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     2716 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2261 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/client.py
--rw-r--r--   0        0        0      354 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3826 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     3814 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3754 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3631 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      668 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-07-14 15:37:41.073850 empiric_network-1.6.5/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1016 2023-07-14 15:37:41.073850 empiric_network-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-07-16 09:13:07.883196 empiric_network-1.6.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    14135 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4257 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/client.py
+-rw-r--r--   0        0        0     2618 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/config.py
+-rw-r--r--   0        0        0     3919 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/contract.py
+-rw-r--r--   0        0        0     9972 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25441 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     8808 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     4177 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     2716 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2261 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      668 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1016 2023-07-16 09:13:07.883196 empiric_network-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.6/PKG-INFO
```

### Comparing `empiric_network-1.6.5/empiric/core/abis/oracle.py` & `empiric_network-1.6.6/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/abis/proxy.py` & `empiric_network-1.6.6/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/abis/publisher_registry.py` & `empiric_network-1.6.6/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/abis/randomness.py` & `empiric_network-1.6.6/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/abis/summary_stats.py` & `empiric_network-1.6.6/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/client.py` & `empiric_network-1.6.6/empiric/core/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Optional
 
 from empiric.core.abis import ORACLE_ABI, PUBLISHER_REGISTRY_ABI, SUMMARY_STATS_ABI
-from empiric.core.config import CONTRACT_ADDRESSES, NETWORKS, ContractAddresses
+from empiric.core.config import CONTRACT_ADDRESSES, NETWORKS, ContractAddresses, get_client_from_network
 from empiric.core.contract import Contract
 from empiric.core.mixins import (
     NonceMixin,
     OracleMixin,
     PublisherRegistryMixin,
     RandomnessMixin,
     TransactionMixin,
```

### Comparing `empiric_network-1.6.5/empiric/core/config.py` & `empiric_network-1.6.6/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/contract.py` & `empiric_network-1.6.6/empiric/core/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     return invoke_result
 
 
 async def wait_for_received(
     client,
     tx_hash,
-    check_interval=3,
+    check_interval=6,
 ) -> (int, TransactionStatus):
     # pylint: disable=too-many-branches
     """
     Awaits for transaction to get accepted or at least pending by polling its status
 
     :param client: Account client
     :param tx_hash: Transaction's hash
@@ -78,16 +78,20 @@
     """
     if check_interval <= 0:
         raise ValueError("check_interval has to bigger than 0.")
 
     first_run = True
     try:
         while True:
-            result = await client.get_transaction_receipt(tx_hash=tx_hash)
-            status = result.status
+            status = TransactionStatus.NOT_RECEIVED
+            try:
+                result = await client.get_transaction_receipt(tx_hash=tx_hash)
+                status = result.status
+            except:
+                continue
 
             if status in (
                 TransactionStatus.ACCEPTED_ON_L1,
                 TransactionStatus.ACCEPTED_ON_L2,
             ):
                 return result.block_number, status
             if status == TransactionStatus.PENDING:
```

### Comparing `empiric_network-1.6.5/empiric/core/entry.py` & `empiric_network-1.6.6/empiric/core/entry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/mixins/evm.py` & `empiric_network-1.6.6/empiric/core/mixins/evm.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/mixins/nonce.py` & `empiric_network-1.6.6/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/mixins/oracle.py` & `empiric_network-1.6.6/empiric/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.6.6/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/mixins/randomness.py` & `empiric_network-1.6.6/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/mixins/transactions.py` & `empiric_network-1.6.6/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/types.py` & `empiric_network-1.6.6/empiric/core/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/core/utils.py` & `empiric_network-1.6.6/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/assets.py` & `empiric_network-1.6.6/empiric/publisher/assets.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/client.py` & `empiric_network-1.6.6/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/cex.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/defillama.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/kaiko.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/okx.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.6.6/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/publisher/types.py` & `empiric_network-1.6.6/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/empiric/test/interface_consistency.py` & `empiric_network-1.6.6/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.5/pyproject.toml` & `empiric_network-1.6.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.6.5"
+version = "1.6.6"
 authors = ["Pragma <contact@pragmaoracle.com>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragmaoracle.com"
 repository = "https://github.com/Astraly-Labs/Pragma"
 documentation = "https://docs.pragmaoracle.com"
 classifiers = [
```

### Comparing `empiric_network-1.6.5/PKG-INFO` & `empiric_network-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.6.5
+Version: 1.6.6
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragmaoracle.com
 Author: Pragma
 Author-email: contact@pragmaoracle.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

