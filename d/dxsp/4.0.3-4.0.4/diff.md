# Comparing `tmp/dxsp-4.0.3.tar.gz` & `tmp/dxsp-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.0.3.tar", max compression
+gzip compressed data, was "dxsp-4.0.4.tar", max compression
```

## Comparing `dxsp-4.0.3.tar` & `dxsp-4.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-16 20:54:38.807265 dxsp-4.0.3/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-16 20:54:38.807265 dxsp-4.0.3/README.md
--rw-r--r--   0        0        0      115 2023-07-16 20:54:39.619277 dxsp-4.0.3/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-16 20:54:38.807265 dxsp-4.0.3/dxsp/config.py
--rw-r--r--   0        0        0    10529 2023-07-16 20:54:38.807265 dxsp-4.0.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5622 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1835 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1036 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4636 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6590 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1989 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-16 20:54:38.811266 dxsp-4.0.3/dxsp/utils/utils.py
--rw-r--r--   0        0        0     2327 2023-07-16 20:54:39.619277 dxsp-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 dxsp-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-16 20:59:31.981466 dxsp-4.0.4/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-16 20:59:31.981466 dxsp-4.0.4/README.md
+-rw-r--r--   0        0        0      115 2023-07-16 20:59:32.709483 dxsp-4.0.4/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/config.py
+-rw-r--r--   0        0        0    10529 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5622 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1835 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1036 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4728 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6590 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1989 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-16 20:59:31.985466 dxsp-4.0.4/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     2327 2023-07-16 20:59:32.709483 dxsp-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 dxsp-4.0.4/PKG-INFO
```

### Comparing `dxsp-4.0.3/LICENSE` & `dxsp-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/README.md` & `dxsp-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/dxsp/default_settings.toml` & `dxsp-4.0.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/dxsp/main.py` & `dxsp-4.0.4/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/dxsp/protocols/oneinch.py` & `dxsp-4.0.4/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/dxsp/protocols/uniswap.py` & `dxsp-4.0.4/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/dxsp/protocols/zerox.py` & `dxsp-4.0.4/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/dxsp/utils/account_utils.py` & `dxsp-4.0.4/dxsp/utils/account_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,31 @@
 
     def __init__(self, w3: Optional[Web3] = None):
         self.logger = logging.getLogger(name="DexSwap")
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
         self.account_number = (f"{str(self.w3.net.version)} - "
-                        f"{str(self.wallet_address[-8:])}")
+                        f"{str(self.wallet_address)[-8:]}")
         self.private_key = settings.dex_private_key
         self.trading_asset_address = self.w3.to_checksum_address(
         settings.trading_asset_address)
         self.contract_utils = ContractUtils(w3=self.w3)
 
     async def get_info(self):
-        return (f"ℹ️ {__class__.__name__} {__version__}\n"
-                f"💱 {await self.get_name()}\n"
-                f"🪪 {self.account_number}")
+        try:
+            return (f"ℹ️ {__package__.__name__} {__version__}\n"
+                    f"💱 {await self.get_name()}\n"
+                    f"🪪 {self.account_number}")
+        except Exception as error:
+            return error
 
     async def get_name(self):
         if settings.dex_router_contract_addr:
-            return settings.dex_router_contract_addr[-8:]
+            return str(settings.dex_router_contract_addr)[-8:]
 
     async def get_account_balance(self):
         account_balance = self.w3.eth.get_balance(
             self.w3.to_checksum_address(self.wallet_address))
         account_balance = self.w3.from_wei(account_balance, 'ether') or 0
         trading_asset_balance = await self.get_trading_asset_balance()
         return f"₿ {round(account_balance,5)}\n💵 {trading_asset_balance}"
```

### Comparing `dxsp-4.0.3/dxsp/utils/contract_utils.py` & `dxsp-4.0.4/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/dxsp/utils/explorer_utils.py` & `dxsp-4.0.4/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.3/pyproject.toml` & `dxsp-4.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.0.3"
+version = "4.0.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-4.0.3/PKG-INFO` & `dxsp-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.0.3
+Version: 4.0.4
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
-Metadata-Version: 2.1 Name: dxsp Version: 4.0.3 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.0.4 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

