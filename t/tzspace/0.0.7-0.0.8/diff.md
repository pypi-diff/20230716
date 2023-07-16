# Comparing `tmp/tzspace-0.0.7.tar.gz` & `tmp/tzspace-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzspace-0.0.7.tar", last modified: Thu Jul 13 11:09:41 2023, max compression
+gzip compressed data, was "tzspace-0.0.8.tar", last modified: Sun Jul 16 03:19:23 2023, max compression
```

## Comparing `tzspace-0.0.7.tar` & `tzspace-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.056719 tzspace-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 tzspace-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      466 2023-07-13 11:09:41.056719 tzspace-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    13928 2023-07-13 11:08:24.000000 tzspace-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.024780 tzspace-0.0.7/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.7/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.026769 tzspace-0.0.7/ior/config/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.7/ior/config/__init__.py
--rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.7/ior/config/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.036264 tzspace-0.0.7/ior/config/contracts/
--rw-rw-rw-   0        0        0    90537 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/Certificate.json
--rw-rw-rw-   0        0        0    29114 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/Exchange.json
--rw-rw-rw-   0        0        0    26608 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/PermissionControl.json
--rw-rw-rw-   0        0        0    29186 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/RoleControl.json
--rw-rw-rw-   0        0        0    71651 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/StoredNFT.json
--rw-rw-rw-   0        0        0    35700 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/TZContractTemplate.json
--rw-rw-rw-   0        0        0    38166 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/TZTemplateControl.json
-drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.044922 tzspace-0.0.7/ior/core/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.7/ior/core/__init__.py
--rw-rw-rw-   0        0        0     6399 2023-07-13 09:58:58.000000 tzspace-0.0.7/ior/core/certificate_service.py
--rw-rw-rw-   0        0        0     1709 2023-07-13 09:56:40.000000 tzspace-0.0.7/ior/core/exchange_service.py
--rw-rw-rw-   0        0        0     3750 2023-07-13 10:37:45.000000 tzspace-0.0.7/ior/core/permission_control_service.py
--rw-rw-rw-   0        0        0     5524 2023-07-13 10:25:47.000000 tzspace-0.0.7/ior/core/role_control_service.py
--rw-rw-rw-   0        0        0     1739 2023-07-08 15:05:36.000000 tzspace-0.0.7/ior/core/stored_nft_service.py
--rw-rw-rw-   0        0        0     5628 2023-07-08 15:05:44.000000 tzspace-0.0.7/ior/core/tz_contract_template_service.py
--rw-rw-rw-   0        0        0     5856 2023-07-08 15:05:49.000000 tzspace-0.0.7/ior/core/tz_template_control_service.py
--rw-rw-rw-   0        0        0     1537 2023-07-13 08:41:23.000000 tzspace-0.0.7/ior/iorconfig.py
--rw-rw-rw-   0        0        0     2777 2023-07-13 10:50:06.000000 tzspace-0.0.7/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.049566 tzspace-0.0.7/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.7/ior/util/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.7/ior/util/certificate_utils.py
--rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.7/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     3582 2023-04-02 12:43:26.000000 tzspace-0.0.7/ior/util/web3_utils.py
--rw-rw-rw-   0        0        0       42 2023-07-13 11:09:41.056719 tzspace-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-07-13 11:09:36.000000 tzspace-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.054637 tzspace-0.0.7/tzspace.egg-info/
--rw-rw-rw-   0        0        0      466 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.228762 tzspace-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 tzspace-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      466 2023-07-16 03:19:23.227405 tzspace-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    24612 2023-07-15 13:32:36.000000 tzspace-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.171002 tzspace-0.0.8/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.8/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.174661 tzspace-0.0.8/ior/config/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.8/ior/config/__init__.py
+-rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.8/ior/config/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.189252 tzspace-0.0.8/ior/config/contracts/
+-rw-rw-rw-   0        0        0    90537 2023-03-26 16:06:07.000000 tzspace-0.0.8/ior/config/contracts/Certificate.json
+-rw-rw-rw-   0        0        0    29114 2023-03-26 16:06:07.000000 tzspace-0.0.8/ior/config/contracts/Exchange.json
+-rw-rw-rw-   0        0        0    26608 2023-03-26 16:06:07.000000 tzspace-0.0.8/ior/config/contracts/PermissionControl.json
+-rw-rw-rw-   0        0        0    29186 2023-03-26 16:06:07.000000 tzspace-0.0.8/ior/config/contracts/RoleControl.json
+-rw-rw-rw-   0        0        0    71651 2023-03-26 16:06:07.000000 tzspace-0.0.8/ior/config/contracts/StoredNFT.json
+-rw-rw-rw-   0        0        0    35700 2023-03-26 16:06:07.000000 tzspace-0.0.8/ior/config/contracts/TZContractTemplate.json
+-rw-rw-rw-   0        0        0    38166 2023-03-26 16:06:07.000000 tzspace-0.0.8/ior/config/contracts/TZTemplateControl.json
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.207595 tzspace-0.0.8/ior/core/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.8/ior/core/__init__.py
+-rw-rw-rw-   0        0        0     9209 2023-07-15 13:27:56.000000 tzspace-0.0.8/ior/core/certificate_service.py
+-rw-rw-rw-   0        0        0     1756 2023-07-14 16:33:46.000000 tzspace-0.0.8/ior/core/exchange_service.py
+-rw-rw-rw-   0        0        0     5937 2023-07-15 05:02:58.000000 tzspace-0.0.8/ior/core/permission_control_service.py
+-rw-rw-rw-   0        0        0     6819 2023-07-15 13:04:22.000000 tzspace-0.0.8/ior/core/role_control_service.py
+-rw-rw-rw-   0        0        0     1739 2023-07-13 14:34:22.000000 tzspace-0.0.8/ior/core/stored_nft_service.py
+-rw-rw-rw-   0        0        0     5604 2023-07-14 19:08:28.000000 tzspace-0.0.8/ior/core/tz_contract_template_service.py
+-rw-rw-rw-   0        0        0     5617 2023-07-14 18:37:46.000000 tzspace-0.0.8/ior/core/tz_template_control_service.py
+-rw-rw-rw-   0        0        0     4502 2023-07-15 13:18:38.000000 tzspace-0.0.8/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.214837 tzspace-0.0.8/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.8/ior/util/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.8/ior/util/certificate_utils.py
+-rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.8/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     4164 2023-07-15 03:48:36.000000 tzspace-0.0.8/ior/util/web3_utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 03:19:23.228762 tzspace-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-07-16 03:18:57.000000 tzspace-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.218983 tzspace-0.0.8/test/
+-rw-rw-rw-   0        0        0     1949 2023-07-15 13:28:24.000000 tzspace-0.0.8/test/test_cert.py
+-rw-rw-rw-   0        0        0     2588 2023-07-15 12:59:16.000000 tzspace-0.0.8/test/test_role.py
+-rw-rw-rw-   0        0        0     1877 2023-07-15 03:46:16.000000 tzspace-0.0.8/test/test_template.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:19:23.225286 tzspace-0.0.8/tzspace.egg-info/
+-rw-rw-rw-   0        0        0      466 2023-07-16 03:19:22.000000 tzspace-0.0.8/tzspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-07-16 03:19:23.000000 tzspace-0.0.8/tzspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 03:19:22.000000 tzspace-0.0.8/tzspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-16 03:19:22.000000 tzspace-0.0.8/tzspace.egg-info/top_level.txt
```

### Comparing `tzspace-0.0.7/LICENSE` & `tzspace-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/consts.py` & `tzspace-0.0.8/ior/config/consts.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/contracts/Certificate.json` & `tzspace-0.0.8/ior/config/contracts/Certificate.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/contracts/Exchange.json` & `tzspace-0.0.8/ior/config/contracts/Exchange.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/contracts/PermissionControl.json` & `tzspace-0.0.8/ior/config/contracts/PermissionControl.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/contracts/RoleControl.json` & `tzspace-0.0.8/ior/config/contracts/RoleControl.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/contracts/StoredNFT.json` & `tzspace-0.0.8/ior/config/contracts/StoredNFT.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/contracts/TZContractTemplate.json` & `tzspace-0.0.8/ior/config/contracts/TZContractTemplate.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/config/contracts/TZTemplateControl.json` & `tzspace-0.0.8/ior/config/contracts/TZTemplateControl.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/core/certificate_service.py` & `tzspace-0.0.8/ior/core/certificate_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,211 @@
 
 from ..config.consts import certificate_path
-from ..util.web3_utils import get_abi, contract_instance, func_send_raw_transaction, contract_functions
-from hexbytes import (
-    HexBytes,
-)
-
+from ..util.web3_utils import get_abi, contract_instance, func_send_raw_transaction, contract_functions, \
+    contract_events
+from hexbytes import HexBytes
+import traceback
+
+def error_handler(func):
+    def execute(self,*args,**kwargs):
+        try:
+            return func(self,*args,**kwargs),0
+        except:
+            msg = traceback.format_exc()
+            if self.config.is_print:
+                print(msg)
+            return f'error:{msg}',1
+    return execute
 
 class CertificateService(object):
+    @classmethod
+    def deploy_instance(cls, w3, config, public_key: str, private_key: str):
+        abi,bytecode = get_abi_bytecode(certificate_path)
+        receipt = func_send_raw_transaction(w3.eth.contract(abi=abi, bytecode=bytecode).constructor()
+            , w3, public_key, private_key, config.timeout, config.poll_latency)
+
+        if config.is_print:
+            print(receipt)
+        return receipt.contractAddress
+
     def __init__(self, w3, config, address):
         self.w3 = w3
         self.config = config
         self.address = address
         self.abi = get_abi(certificate_path)
-        self.certificate_contract_instance = contract_instance(self.w3, address, self.abi)
+        self.contract_instance = contract_instance(self.w3, address, self.abi)
 
     @property
     def functions(self):
-        if not self.certificate_contract_instance:
+        if not self.contract_instance:
             raise RuntimeError("合约获取失败【certificate_contract】")
-        return contract_functions(self.certificate_contract_instance)
+        return contract_functions(self.contract_instance)
 
     def token_id_mapping_item(self, key):
         """
         合约属性 mapping(uint256 => uint256) public tokenIdMapping
         :param key:
         :return:
         """
         res = self.functions.tokenIdMapping(key).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
+        return res
 
     def recreations_item(self, key):
         """
         合约属性 mapping(uint256 => DataTypes.AuthorizeData) public recreations
         :param key:
         :return:
         """
         res = self.functions.recreations(key).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
+        return res
+
+    def process_receipt_for(self,event,receipt,key):
+        logs = event.process_receipt(receipt)
+        if self.config.is_print:
+            print(receipt)
+        key = logs[0]['args'][key]
+        return receipt, key
+
+
+    def approve(self, to, token_id, public_key, private_key):
+        func = self.functions.approve(to, token_id)
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
+
+    def set_approve_for_all(self, operator, approved, public_key, private_key):
+        func = self.functions.setApprovalForAll(operator, approved)
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
     def mint(self, to: str, public_key: str, private_key: str):
         """
         合约方法 mint(address to) 【继承】
         方法返回 无
         :param to:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.mint(to)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        block: HexBytes = receipt.get("blockHash")
-        transaction: HexBytes = receipt.get("transactionHash")
-        return block.hex(), transaction.hex(), receipt
+        return self.process_receipt_for(contract_events(self.contract_instance).Transfer(),receipt,'tokenId')
+
+    def safeTransferFrom(self, fromAddr: str, toAddr: str, tokenId: int, public_key: str, private_key: str):
+        """
+        合约方法 mint(address to) 【继承】
+        方法返回 无
+        :param to:
+        :param public_key:
+        :param private_key:
+        :return:
+        """
+        func = self.functions.safeTransferFrom(fromAddr,toAddr,tokenId)
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
+
 
     def bind_option(self, option, public_key, private_key):
         """
         合约方法 bindOption(address option_)
         合约返回 无
         :param option:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.bindOption(option)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        block: HexBytes = receipt.get("blockHash")
-        transaction: HexBytes = receipt.get("transactionHash")
-        return block.hex(), transaction.hex()
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
     def set_authorize_approval(self, token_id, operator, approved, public_key, private_key):
         """
         合约方法 setAuthorizeApproval(uint256 tokenId, address operator, bool approved)
         合约返回 无
         :param token_id:
         :param operator:
         :param approved:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.setAuthorizeApproval(token_id, operator, approved)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
     def is_authorize_approved(self, token_id: int, operator: str) -> bool:
         """
         合约方法 isAuthorizeApproved(uint256 tokenId, address operator)
         合约返回 bool
         :param token_id:
         :param operator:
         :return:
         """
         res = self.functions.isAuthorizeApproved(token_id, operator).call()
+        if self.config.is_print:
+            print(res)
         return res
 
     def authorize(self, to: str, original_token_id: int, public_key: str, private_key: str):
         """
         合约方法 authorize(address to, uint256 originalTokenId)
         合约返回 uint256 tokenId
         :param to:
         :param original_token_id:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.authorize(to, original_token_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        return receipt
+        return self.process_receipt_for(contract_events(self.contract_instance).Transfer(),receipt,'tokenId')
 
     def create_option(self, to, original_token_id, price, effect_date, public_key, private_key):
         func = self.functions.createOption(to, original_token_id, price, effect_date)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        return receipt
+        return self.process_receipt_for(contract_events(self.contract_instance).Transfer(),receipt,'tokenId')
 
     def authorize_option(self, to, original_token_id, option_token_id, public_key, private_key):
         func = self.functions.authorizeOption(to, original_token_id, option_token_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        return receipt
+        return self.process_receipt_for(contract_events(self.contract_instance).Transfer(),receipt,'tokenId')
 
     def recreate(self, to, ref_token_ids, public_key, private_key):
         func = self.functions.recreate(to, ref_token_ids)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        return receipt
+        return self.process_receipt_for(contract_events(self.contract_instance).Transfer(),receipt,'tokenId')
 
     def recreate_in_chain(self, to, certificates, ref_token_ids, public_key, private_key):
         func = self.functions.recreateInChain(to, certificates, ref_token_ids)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        return receipt
+        return self.process_receipt_for(contract_events(self.contract_instance).Transfer(),receipt,'tokenId')
 
     def recreate_cross_chain(self, to, chain_ids, certificates, ref_token_ids, public_key, private_key):
         func = self.functions.recreateCrossChain(to, chain_ids, certificates, ref_token_ids)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
-        return receipt
+        return self.process_receipt_for(contract_events(self.contract_instance).Transfer(),receipt,'tokenId')
 
     def update_token_id_mapping(self, token_id, original_token_id, public_key, private_key):
         func = self.functions.updateTokenIdMapping(token_id, original_token_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        if self.config.is_print:
+            print(receipt)
         return receipt
 
     def token_uri(self, token_id):
         res = self.functions.tokenURI(token_id).call()
+        if self.config.is_print:
+            print(res)
         return res
```

### Comparing `tzspace-0.0.7/ior/core/exchange_service.py` & `tzspace-0.0.8/ior/core/exchange_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 
 class ExchangeService(object):
 
     def __init__(self, w3, config):
         self.w3 = w3
         self.config = config
         self.abi = get_abi(exchange_path)
-        self.exchange_contract_instance = contract_instance(self.w3, self.config.contract_addresses['TZExchange'], self.abi)
+        self.contract_instance = contract_instance(self.w3, self.config.contract_addresses['TZExchange'], self.abi)
 
     @property
     def functions(self):
-        if not self.exchange_contract_instance:
+        if not self.contract_instance:
             raise RuntimeError("合约获取失败【exchange_contract】")
-        return contract_functions(self.exchange_contract_instance)
+        return contract_functions(self.contract_instance)
 
     def exchange(self, cert_address: str, token_id: int, from_address: str, to_address: str, price: int, public_key: str,
                  private_key: str):
         func = self.functions.exchange(cert_address, token_id, from_address, to_address, price)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        #print(receipt)
+        if self.config.is_print:
+            print(receipt)
         return receipt
 
     def exchange_with_feed(self, cert_address: str, token_id: int, from_address: str, to_address: str, price: int,
                            fee: int, feeds: list[str], percents: list[int], public_key: str, private_key: str):
         func = self.functions.exchangeWithFeed(cert_address, token_id, from_address, to_address, price, fee, feeds,
                                                percents)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        #print(receipt)
+        if self.config.is_print:
+            print(receipt)
         return receipt
```

### Comparing `tzspace-0.0.7/ior/core/role_control_service.py` & `tzspace-0.0.8/ior/core/role_control_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,91 @@
 from ..config.consts import role_control_path
-from ..util.web3_utils import get_abi, contract_instance, func_send_raw_transaction, contract_functions
+from ..util.web3_utils import get_abi, contract_instance, func_send_raw_transaction, contract_functions, keccak256
+import traceback
 
+def error_handler(func):
+    def execute(self,*args,**kwargs):
+        try:
+            return func(self,*args,**kwargs),0
+        except:
+            msg = traceback.format_exc()
+            if self.config.is_print:
+                print(msg)
+            return f'error:{msg}',1
+    return execute
 
 class RoleControlService(object):
-    def __init__(self, w3, config):
+    @classmethod
+    def deploy_instance(cls, w3, config, public_key: str, private_key: str):
+        abi,bytecode = get_abi_bytecode(role_control_path)
+        receipt = func_send_raw_transaction(w3.eth.contract(abi=abi, bytecode=bytecode).constructor()
+            , w3, public_key, private_key, config.timeout, config.poll_latency)
+
+        if config.is_print:
+            print(receipt)
+        return receipt.contractAddress
+
+
+    def __init__(self, w3, config, address=None):
         self.w3 = w3
         self.config = config
         self.abi = get_abi(role_control_path)
-        self.role_control_contract_instance = contract_instance(self.w3, self.config.contract_addresses['RoleControl'], self.abi)
+
+        if address is None:
+            self.address = self.config.contract_addresses['RoleControl']
+        else:
+            self.address = address
+        self.contract_instance = contract_instance(self.w3, self.address, self.abi) 
 
     @property
     def functions(self):
-        if not self.role_control_contract_instance:
+        if not self.contract_instance:
             raise RuntimeError("合约获取失败【role_control_contract】")
-        return contract_functions(self.role_control_contract_instance)
+        return contract_functions(self.contract_instance)
 
+
+    
     def roles_item(self, key):
         """
         合约属性 mapping(bytes32 => TzRoleData) public roles
         :param key:
         :return:
         """
         res = self.functions.roles(key).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
         return res
 
-
+    @error_handler
     def grant_role(self, role_name: str, to: str, public_key: str, private_key: str):
 
-        role_name_bytes = f"0x{role_name.encode().hex()}"
+        role_name_bytes = keccak256(role_name)
         func = self.functions.grantRole(role_name_bytes, to)
-        receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
+    @error_handler
     def revoke_role(self, role_name: str, to: str, public_key: str, private_key: str):
 
-        role_name_bytes = f"0x{role_name.encode().hex()}"
+        role_name_bytes = keccak256(role_name)
         func = self.functions.revokeRole(role_name_bytes, to)
-        receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
     def has_role(self, role_name: str, to: str):
 
-        role_name_bytes = f"0x{role_name.encode().hex()}"
+        role_name_bytes = keccak256(role_name)
         res = self.functions.hasRole(role_name_bytes,to).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
         return res
 
     def add_role(self, role_name: str, admin_role: str, permission_role: str, permissions: list[str],
                  permission_contract_addrs: list[str], public_key: str, private_key: str):
         """
         合约方法 addRole(bytes32 roleName, bytes32 adminRole, bytes32 permissionRole,
                             bytes32[] calldata permissions, address[] calldata permissionContractAddrs)
@@ -58,65 +95,73 @@
         :param permission_role:
         :param permissions:
         :param permission_contract_addrs:
         :param public_key:
         :param private_key:
         :return:
         """
-        role_name_bytes = f"0x{role_name.encode().hex()}"
-        admin_role_bytes = f"0x{admin_role.encode().hex()}"
-        permission_role_bytes = f"0x{permission_role.encode().hex()}"
-        permissions_bytes = [f"0x{p.encode().hex()}" for p in permissions]
+        role_name_bytes = keccak256(role_name)
+        admin_role_bytes = keccak256(admin_role)
+        permission_role_bytes = keccak256(permission_role)
+        permissions_bytes = [keccak256(p) for p in permissions]
         func = self.functions.addRole(role_name_bytes, admin_role_bytes, permission_role_bytes, permissions_bytes,
                                       permission_contract_addrs)
-        receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
-    def add_permission(self, role_name, permissions, permission_contract_addrs, public_key, private_key):
+    def add_permission(self, role_name: str, permissions: list[str], permission_contract_addrs: list[str],
+                public_key: str, private_key: str):
         """
         合约方法 addPermission(bytes32 roleName, bytes32[] calldata permissions, address[] calldata permissionContractAddrs)
         合约返回 无
         :param role_name:
         :param permissions:
         :param permission_contract_addrs:
         :param public_key:
         :param private_key:
         :return:
         """
-        role_name_bytes = f"0x{role_name.encode().hex()}"
-        permissions_bytes = [p.encode().hex() for p in permissions]
+        role_name_bytes = keccak256(role_name)
+        permissions_bytes = [keccak256(p) for p in permissions]
         func = self.functions.addPermission(role_name_bytes, permissions_bytes, permission_contract_addrs)
-        receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
-    def del_permission(self, role_name, permissions, public_key, private_key):
+    def del_permission(self, role_name: str, permissions: list[str], public_key: str, private_key: str):
         """
         合约方法 delPermission(bytes32 roleName, bytes32[] calldata permissions)
         合约返回 无
         :param role_name:
         :param permissions:
         :param public_key:
         :param private_key:
         :return:
         """
-        role_name_bytes = f"0x{role_name.encode().hex()}"
-        permissions_bytes = [p.encode().hex() for p in permissions]
+        role_name_bytes = keccak256(role_name)
+        permissions_bytes = [keccak256(p) for p in permissions]
         func = self.functions.delPermission(role_name_bytes, permissions_bytes)
-        receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
+        if self.config.is_print:
+            print(receipt)
+        return receipt
 
-    def check_permission(self, role_name, permission_name, data_hash, operations) -> bool:
+    def check_permission(self, role_name: str, permission_name: str, data: str, operations: int) -> bool:
         """
         合约方法 checkPermission(bytes32 roleName, bytes32 permissionName, bytes32 dataHash, uint32 operations)
         合约返回 bool
         :param role_name:
         :param permission_name:
-        :param data_hash:
+        :param data:
         :param operations:
         :return:
         """
-        role_name_bytes = f"0x{role_name.encode().hex()}"
-        permission_name_bytes = f"0x{permission_name.encode().hex()}"
-        data_hash_bytes = f"0x{data_hash.encode().hex()}"
-        res = self.functions.checkPermission(role_name_bytes, permission_name_bytes, data_hash_bytes, operations).call()
-        print(res)
+        role_name_bytes = keccak256(role_name)
+        permission_name_bytes = keccak256(permission_name)
+        data_bytes = keccak256(data)
+        res = self.functions.checkPermission(role_name_bytes, permission_name_bytes, data_bytes, operations).call()
+        if self.config.is_print:
+            print(res)
         return res
```

### Comparing `tzspace-0.0.7/ior/core/stored_nft_service.py` & `tzspace-0.0.8/ior/core/stored_nft_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/core/tz_contract_template_service.py` & `tzspace-0.0.8/ior/core/tz_contract_template_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 
 class TZContractTemplateService(object):
     def __init__(self, w3, config, address):
         self.w3 = w3
         self.config = config
         self.abi = get_abi(tz_contract_template_path)
-        self.tz_contract_template_contract_instance = contract_instance(self.w3, address, self.abi)
+        self.contract_instance = contract_instance(self.w3, address, self.abi)
 
     @property
     def functions(self):
-        if not self.tz_contract_template_contract_instance:
+        if not self.contract_instance:
             raise RuntimeError("合约获取失败【tz_contract_template_contract】")
-        return contract_functions(self.tz_contract_template_contract_instance)
+        return contract_functions(self.contract_instance)
 
     def create_instance(self, hash_value: str, end_time: int, user: str, public_key: str, private_key: str):
         """
         合约方法 createInstance(bytes32 hash, uint256 endTime, address user)
         合约返回 uint256 insId
         :param hash_value:
         :param end_time:
@@ -28,113 +28,112 @@
         :param public_key:
         :param private_key:
         :return:
         """
         hash_bytes = f"{hash_value.encode().hex()}"
         func = self.functions.createInstance(hash_bytes, end_time, user)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        print(receipt)
+        if self.config.is_print:
+            print(receipt)
         return receipt
 
+    def process_receipt_for(self,event,receipt,key):
+        logs = event.process_receipt(receipt)
+        if self.config.is_print:
+            print(logs)
+        key = logs[0]['args'][key]
+        return receipt, key
+
     def init(self, ins_id: int, signatories: list[str], payer: str, payees: list[str],
              share_ratios: list[int], public_key: str, private_key: str):
         """
         合约方法 init(uint256 insId, address[] calldata signatories, address payer, address[] calldata payees, uint256[] calldata shareRatios)
         合约事件 insId, ins.owner, ins.endTime, ins.hash, ins.status
         :param ins_id:
         :param signatories:
         :param payer:
         :param payees:
         :param share_ratios:
         :param public_key:
         :param private_key:
         :return:
-        """
+        """        
         func = self.functions.init(ins_id, signatories, payer, payees, share_ratios)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_contract_template_contract_instance). \
-            TzContractStateChanged().process_receipt(receipt, errors=DISCARD)
-        res = logs[0]['args']
-        print(res)
+        return self.process_receipt_for(contract_events(self.contract_instance).TzContractStateChanged(),receipt,'state')
 
     def start(self, ins_id: int, public_key: str, private_key: str):
         """
         合约方法 start(uint256 insId)
         合约事件 insId, ins.owner, ins.endTime, ins.hash, ins.status
         :param ins_id:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.start(ins_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_contract_template_contract_instance). \
-            TzContractStateChanged().process_receipt(receipt, errors=DISCARD)
-        res = logs[0]['args']
-        print(res)
+        return self.process_receipt_for(contract_events(self.contract_instance).TzContractStateChanged(),receipt,'state')
 
     def sign(self, ins_id: int, public_key: str, private_key: str):
         """
         合约方法 sign(uint256 insId)
         合约事件 insId, ins.owner, ins.endTime, ins.hash, ins.status, _msgSender()
         :param ins_id:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.sign(ins_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_contract_template_contract_instance). \
-            TzContractSigned().process_receipt(receipt, errors=DISCARD)
-        res = logs[0]['args']
-        print(res)
+        return self.process_receipt_for(contract_events(self.contract_instance).TzContractSigned(),receipt,'state')
 
     def end(self, ins_id: int, public_key: str, private_key: str):
         """
         合约方法 end(uint256 insId)
         合约事件 insId, ins.owner, ins.endTime, ins.hash, ins.status
         :param ins_id:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.end(ins_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_contract_template_contract_instance). \
-            TzContractStateChanged().process_receipt(receipt, errors=DISCARD)
-        res = logs[0]['args']
-        print(res)
+        return self.process_receipt_for(contract_events(self.contract_instance).TzContractStateChanged(),receipt,'state')
 
     def can_pay(self, ins_id: int, addr: str) -> bool:
         """
         合约方法 canPay(uint256 insId,address addr)
         合约返回 bool
         :param ins_id:
         :param addr:
         :return:
         """
         res = self.functions.canPay(ins_id, addr).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
         return res
 
     def get_payees(self, ins_id: int) -> list[str]:
         """
         合约方法 getPayees(uint256 insId)
         合约返回 bytes32[] memory
         :param ins_id:
         :return:
         """
         res = self.functions.getPayees(ins_id).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
         return res
 
     def get_ratio(self, ins_id: int, payee: str) -> int:
         """
         合约方法 getRatio(uint256 insId,address payee)
         合约返回 uint256
         :param ins_id:
         :param payee:
         :return:
         """
         res = self.functions.getRatio(ins_id, payee).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
         return res
```

### Comparing `tzspace-0.0.7/ior/core/tz_template_control_service.py` & `tzspace-0.0.8/ior/core/tz_template_control_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,92 +6,93 @@
 
 
 class TZTemplateControlService(object):
     def __init__(self, w3, config):
         self.w3 = w3
         self.config = config
         self.abi = get_abi(tz_template_control_path)
-        self.tz_template_control_contract_instance = contract_instance(self.w3, self.config.contract_addresses['TZTemplateControl'], self.abi)
+        self.contract_instance = contract_instance(self.w3, self.config.contract_addresses['TZTemplateControl'], self.abi)
 
     @property
     def functions(self):
-        if not self.tz_template_control_contract_instance:
+        if not self.contract_instance:
             raise RuntimeError("合约获取失败【tz_template_control_contract】")
-        return contract_functions(self.tz_template_control_contract_instance)
+        return contract_functions(self.contract_instance)
 
     def indexes_item(self, key):
         """
         合约属性 mapping(address => uint256) public indexes
         :param key:
         :return:
         """
         res = self.functions.indexes(key).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
+        return res
 
     def get_template(self, template_id: int):
         """
         合约方法 getTemplate(uint256 templateId)
         合约放回 (ins.template, ins.name, ins.category, ins.owner, ins.ratio, ins.status)
         :param template_id:
         :return:
         """
         res = self.functions.getTemplate(template_id).call()
-        print(res)
+        if self.config.is_print:
+            print(res)
         return res
 
+    def process_receipt_for(self,event,receipt,key):
+        logs = event.process_receipt(receipt)
+        if self.config.is_print:
+            print(logs)
+        key = logs[0]['args'][key]
+        return receipt, key
+
     def register(self, template: str, category: int, name: str, ratio: int, public_key: str, private_key: str) -> int:
         """
         合约方法 register(address template, uint256 category, bytes32 name, uint256 ratio)
         事件返回 TzTemplateRegistered(templateId,ins.owner,ins.template,ins.category)
         :param template:
         :param category:
         :param name:
         :param ratio:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.register(template, category, name, ratio)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_template_control_contract_instance). \
-            TzTemplateRegistered().process_receipt(receipt, errors=DISCARD)
-        print(logs)
-        return logs[0]['args']['templateId']
+        return self.process_receipt_for(contract_events(self.contract_instance).TzTemplateInstanceCreated(),receipt,'templateId')
 
     def start(self, template_id: int, public_key: str, private_key: str):
         """
         合约方法 end(uint256 templateId)
         事件返回 TzTemplateStateChanged(templateId, ins.owner, ins.status)
         :param template_id:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.start(template_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_template_control_contract_instance). \
-            TzTemplateStateChanged().process_receipt(receipt, errors=DISCARD)
-        print(logs)
-        return logs[0]['args']['ins.status']
+        return self.process_receipt_for(contract_events(self.contract_instance).TzTemplateStateChanged(),receipt,'state')
 
     def end(self, template_id: int, public_key: str, private_key: str):
         """
         合约方法 end(uint256 templateId)
         事件返回 TzTemplateStateChanged(templateId, ins.owner, ins.status)
         :param template_id:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.end(template_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_template_control_contract_instance). \
-            TzTemplateStateChanged().process_receipt(receipt, errors=DISCARD)
-        print(logs)
-        return logs[0]['args']['ins.status']
+        return self.process_receipt_for(contract_events(self.contract_instance).TzTemplateStateChanged(),receipt,'state')
 
     def request_template(self, template_id: int, hash_value: str, end_time: int, public_key: str,
                          private_key: str) -> int:
         """
         合约方法 requestTemplate(uint256 templateId, bytes32 hash, uint256 endTime)
         事件返回 TzTemplateInstanceCreated(templateId, ins.template, instanceId, _msgSender(), endTime, hash)
         :param template_id:
@@ -100,19 +101,16 @@
         :param public_key:
         :param private_key:
         :return:
         """
         hash_bytes = f"{hash_value.encode().hex()}"
         func = self.functions.requestTemplate(template_id, hash_bytes, end_time)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_template_control_contract_instance). \
-            TzTemplateInstanceCreated().process_receipt(receipt, errors=DISCARD)
-        print(logs)
-        return logs[0]['args']['instanceId']
-
+        return self.process_receipt_for(contract_events(self.contract_instance).TzTemplateInstanceCreated(),receipt,'instanceId')
+        
     def pay(self, template_id: int, instance_id: int, token: str, total_income: int, public_key: str,
             private_key: str) -> dict:
         """
         合约方法 pay(uint256 templateId,uint256 instanceId,address token,uint256 totalIncome)
         事件返回 CommissionPaid(templateId, instanceId, ins.template, _msgSender(), token, totalIncome)
         :param template_id:
         :param instance_id:
@@ -120,11 +118,10 @@
         :param total_income:
         :param public_key:
         :param private_key:
         :return:
         """
         func = self.functions.pay(template_id, instance_id, token, total_income)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
-        logs = contract_events(self.tz_template_control_contract_instance). \
-            CommissionPaid().process_receipt(receipt, errors=DISCARD)
-        print(logs)
-        return logs[0]['args']
+        if self.config.is_print:
+            print(receipt)
+        return receipt
```

### Comparing `tzspace-0.0.7/ior/util/certificate_utils.py` & `tzspace-0.0.8/ior/util/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/util/result_utils.py` & `tzspace-0.0.8/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.7/ior/util/web3_utils.py` & `tzspace-0.0.8/ior/util/web3_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,25 @@
         w3.middleware_onion.inject(web3.middleware.geth_poa_middleware, layer=0)
     if is_print:
         print(f"连接状态 => {w3.is_connected()}")
         print(f"最近一个块 => {w3.eth.get_block('latest')}")
         print(f"版本 => {w3.client_version}")
     return w3
 
+def to_address(data):
+    return Web3.to_checksum_address(data)
+
+def to_hex(data):
+    return Web3.to_hex(data)
+
+def to_text(data):
+    return Web3.to_text(data)
+
+def keccak256(data: str):
+    return Web3.keccak(text=data)
 
 def get_abi(filename: str):
     """
     从文件里获取abi
     :param filename:
     :return:
     """
@@ -42,14 +53,27 @@
         obj = json.load(f)
         if not obj:
             raise IOError(f"{filename}文件非法")
         if 'abi' not in obj:
             raise IOError(f"{filename}文件不包含abi")
         return obj['abi']
 
+def get_abi_bytecode(filename: str):
+    """
+    从文件里获取abi
+    :param filename:
+    :return:
+    """
+    with open(filename, 'r', encoding='utf-8')as f:
+        obj = json.load(f)
+        if not obj:
+            raise IOError(f"{filename}文件非法")
+        if 'abi' not in obj:
+            raise IOError(f"{filename}文件不包含abi")
+        return obj['abi'],obj['bytecode']
 
 def contract_instance(w3: Web3, address: str, abi) -> Contract:
     """
     获取合约
     :param w3:
     :param address:
     :param abi:
@@ -89,15 +113,15 @@
     :return:
     """
     # 1. 配置gasPrice为0，则提示{'code': -32000, 'message': 'transaction underpriced'} 交易定价过低
     # 2. 注释gasPrice配置,则提示baseFeePerGas
     # 3. 配置baseFeePerGas: w3.eth.get_block("latest").get("baseFeePerGas") 依然报错
     # 4. 配置gasPrice:w3.eth.gas_price
     tx = func.build_transaction({
-        "gasPrice": w3.eth.gas_price,
+        "gasPrice": 0, #w3.eth.gas_price,
         # 'gas': 50000,
         "from": public_key,
         "nonce": w3.eth.get_transaction_count(public_key)
     })
     signed_txn = w3.eth.account.sign_transaction(tx, private_key=private_key)
     tx_hash = w3.eth.send_raw_transaction(signed_txn.rawTransaction)
     receipt = w3.eth.wait_for_transaction_receipt(tx_hash, timeout=timeout, poll_latency=poll_latency)
@@ -107,11 +131,10 @@
 def create_account(w3):
     """
     创建账户
     :param w3:
     :return:
     """
     acc = w3.eth.account.create()
-    key = acc.key.hex()
-    address = acc.address
-    print(f"private = {key}， public = {address}")
-    return key, address
+    pk = acc.key.hex()
+    pub = acc.address
+    return pub,pk
```

### Comparing `tzspace-0.0.7/setup.py` & `tzspace-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 #with open("README.MD", "r") as fh:
 #  long_description = fh.read()
 
 long_description = "https://github.com/tzspace-ior/tzspacesdk/README.MD"
 setuptools.setup(
   name="tzspace",
-  version="0.0.7",
+  version="0.0.8",
   author="Jie Guan",
   author_email="jguanisme@163.com",
   description="tzspace sdk for ior standard",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/tzspace-ior/tzspacesdk",
   packages=setuptools.find_packages(),
```

### Comparing `tzspace-0.0.7/tzspace.egg-info/SOURCES.txt` & `tzspace-0.0.8/tzspace.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 ior/__init__.py
-ior/iorconfig.py
 ior/iorsdk.py
 ior/config/__init__.py
 ior/config/consts.py
 ior/config/contracts/Certificate.json
 ior/config/contracts/Exchange.json
 ior/config/contracts/PermissionControl.json
 ior/config/contracts/RoleControl.json
@@ -22,11 +21,14 @@
 ior/core/stored_nft_service.py
 ior/core/tz_contract_template_service.py
 ior/core/tz_template_control_service.py
 ior/util/__init__.py
 ior/util/certificate_utils.py
 ior/util/result_utils.py
 ior/util/web3_utils.py
+test/test_cert.py
+test/test_role.py
+test/test_template.py
 tzspace.egg-info/PKG-INFO
 tzspace.egg-info/SOURCES.txt
 tzspace.egg-info/dependency_links.txt
 tzspace.egg-info/top_level.txt
```

