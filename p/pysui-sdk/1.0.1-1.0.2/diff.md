# Comparing `tmp/pysui-sdk-1.0.1.tar.gz` & `tmp/pysui-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysui-sdk-1.0.1.tar", last modified: Tue May  2 06:40:41 2023, max compression
+gzip compressed data, was "pysui-sdk-1.0.2.tar", last modified: Tue May  2 08:16:39 2023, max compression
```

## Comparing `pysui-sdk-1.0.1.tar` & `pysui-sdk-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 06:40:41.990542 pysui-sdk-1.0.1/
--rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 06:40:41.990438 pysui-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 guomaoye   (501) staff       (20)     2475 2023-05-02 05:40:59.000000 pysui-sdk-1.0.1/README.md
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 06:40:41.989716 pysui-sdk-1.0.1/pysui_sdk/
--rw-r--r--   0 guomaoye   (501) staff       (20)       85 2023-05-02 05:04:49.000000 pysui-sdk-1.0.1/pysui_sdk/__init__.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1428 2023-05-02 05:04:49.000000 pysui-sdk-1.0.1/pysui_sdk/models.py
--rw-r--r--   0 guomaoye   (501) staff       (20)    11083 2023-05-02 05:05:47.000000 pysui-sdk-1.0.1/pysui_sdk/provider.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1900 2023-05-02 05:04:49.000000 pysui-sdk-1.0.1/pysui_sdk/rpc_tx_data_serializer.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1258 2023-05-02 05:04:49.000000 pysui-sdk-1.0.1/pysui_sdk/signer.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     2160 2023-05-02 06:23:16.000000 pysui-sdk-1.0.1/pysui_sdk/signer_with_provider.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1517 2023-05-02 05:04:49.000000 pysui-sdk-1.0.1/pysui_sdk/wallet.py
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 06:40:41.990256 pysui-sdk-1.0.1/pysui_sdk.egg-info/
--rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 06:40:41.000000 pysui-sdk-1.0.1/pysui_sdk.egg-info/PKG-INFO
--rw-r--r--   0 guomaoye   (501) staff       (20)      356 2023-05-02 06:40:41.000000 pysui-sdk-1.0.1/pysui_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)        1 2023-05-02 06:40:41.000000 pysui-sdk-1.0.1/pysui_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       13 2023-05-02 06:40:41.000000 pysui-sdk-1.0.1/pysui_sdk.egg-info/requires.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       10 2023-05-02 06:40:41.000000 pysui-sdk-1.0.1/pysui_sdk.egg-info/top_level.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       38 2023-05-02 06:40:41.990576 pysui-sdk-1.0.1/setup.cfg
--rw-r--r--   0 guomaoye   (501) staff       (20)      409 2023-05-02 06:40:26.000000 pysui-sdk-1.0.1/setup.py
+drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 08:16:39.703226 pysui-sdk-1.0.2/
+-rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 08:16:39.703117 pysui-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 guomaoye   (501) staff       (20)     2587 2023-05-02 08:16:18.000000 pysui-sdk-1.0.2/README.md
+drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 08:16:39.702389 pysui-sdk-1.0.2/pysui_sdk/
+-rw-r--r--   0 guomaoye   (501) staff       (20)       85 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/__init__.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1428 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/models.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)    11096 2023-05-02 08:15:58.000000 pysui-sdk-1.0.2/pysui_sdk/provider.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1900 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/rpc_tx_data_serializer.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1258 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/signer.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     2492 2023-05-02 06:50:24.000000 pysui-sdk-1.0.2/pysui_sdk/signer_with_provider.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1517 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/wallet.py
+drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 08:16:39.702959 pysui-sdk-1.0.2/pysui_sdk.egg-info/
+-rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 guomaoye   (501) staff       (20)      356 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)        1 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)       13 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/requires.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)       10 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/top_level.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)       38 2023-05-02 08:16:39.703264 pysui-sdk-1.0.2/setup.cfg
+-rw-r--r--   0 guomaoye   (501) staff       (20)      409 2023-05-02 08:15:58.000000 pysui-sdk-1.0.2/setup.py
```

### Comparing `pysui-sdk-1.0.1/README.md` & `pysui-sdk-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-
 Python SDK to interact with Sui Blockchain 
 
+forked from georgelombardi97/sui_python_sdk
+
+remove some api witch has not include in sui json api list
+
+add more json api
+
+fix signing transactions signature method 
+
 Supports creating wallets, fetching data, signing transactions 
 # Install
 ``
 pip install pysui-sdk
 ``
 
 Todo: 
 - Better type checking
 - Use objects instead of json or dict models 
 - More functions & helpers   
 - Add more examples 
-- Add support for Secp256k1 Signing (only ed25519 now)
 - Add websocket support & event subscription 
 - Add support for publishing move packages 
 
 # How to Use 
 ### Import required objects
 
 ```python
```

### Comparing `pysui-sdk-1.0.1/pysui_sdk/models.py` & `pysui-sdk-1.0.2/pysui_sdk/models.py`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.1/pysui_sdk/provider.py` & `pysui-sdk-1.0.2/pysui_sdk/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     def get_move_function_arg_types(self, package_id: str, module_name: str, function_name: str):
         return self.send_request_to_rpc(method="sui_getMoveFunctionArgTypes",
                                         params=[package_id, module_name, function_name])
 
     def get_check_point(self, check_point_id: str = "1000"):
         return self.send_request_to_rpc(method="sui_getCheckpoint", params=[check_point_id])
 
-    def get_check_points(self, cursor: str, limit: int = 10, order: bool = False):
+    def get_check_points(self, cursor: str = None, limit: int = 10, order: bool = False):
         return self.send_request_to_rpc(method="sui_getCheckpoints", params=[cursor, limit, order])
 
     def get_events(self, tx_digest: str):
         return self.send_request_to_rpc(method="sui_getEvents", params=[tx_digest])
 
     def get_latest_checkpoint_sequence_number(self):
         return self.send_request_to_rpc(method="sui_getLatestCheckpointSequenceNumber")
@@ -178,31 +178,31 @@
                 "showContent": True,
                 "showBcs": False,
                 "showStorageRebate": True
             }
         return self.send_request_to_rpc(method="sui_tryMultiGetPastObjects", params=[object_ids, options])
 
     # optional paging cursor, object_id
-    def get_all_coins(self, address: str, cursor: str = '', limit: int = 10):
+    def get_all_coins(self, address: str, cursor: str = None, limit: int = 10):
         return self.send_request_to_rpc(method="suix_getAllCoins", params=[address, cursor, limit])
 
     def get_coin_metadata(self, coin_type: str):
         return self.send_request_to_rpc(method="suix_getCoinMetadata", params=[coin_type])
 
-    def get_coins(self, address: str, coin_type: str = '0x2::sui::SUI', cursor: str = '', limit: int = 10):
+    def get_coins(self, address: str, coin_type: str = '0x2::sui::SUI', cursor: str = None, limit: int = 10):
         return self.send_request_to_rpc(method="suix_getCoins", params=[address, coin_type, cursor, limit])
 
     # example epoch="5000"
     def get_committee_info(self, epoch: str = None):
         return self.send_request_to_rpc(method="suix_getCommitteeInfo", params=[epoch])
 
     def get_dynamic_field_object(self, parent_object_id: str, dynamic_field_name: str):
         return self.send_request_to_rpc(method="suix_getDynamicFieldObject", params=[parent_object_id, dynamic_field_name])
 
-    def get_dynamic_fields(self, parent_object_id: str, cursor: str = '', limit: int = 10):
+    def get_dynamic_fields(self, parent_object_id: str, cursor: str = None, limit: int = 10):
         return self.send_request_to_rpc(method="suix_getDynamicFields", params=[parent_object_id, cursor, limit])
 
     # def get_objects_owned_by_object(self, object_id: str):
     #     return self.send_request_to_rpc(method="sui_getObjectsOwnedByObject", params=[object_id])
 
     # def get_objects_owned_by_address(self, addr: str):
     #     return self.send_request_to_rpc(method="suix_getBalance", params=[addr])
```

### Comparing `pysui-sdk-1.0.1/pysui_sdk/rpc_tx_data_serializer.py` & `pysui-sdk-1.0.2/pysui_sdk/rpc_tx_data_serializer.py`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.1/pysui_sdk/signer.py` & `pysui-sdk-1.0.2/pysui_sdk/signer.py`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.1/pysui_sdk/signer_with_provider.py` & `pysui-sdk-1.0.2/pysui_sdk/signer_with_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,14 +40,19 @@
         res = self.serializer.new_move_call(
             signer_addr=self.signer_wallet.get_address(),
             tx=tx_move_call)
         tx_bytes = res["result"]["txBytes"]
 
         res = self.provider.get_dry_run_transaction_block(tx_bytes)
         dry_run_status_map = res['result']['effects']['status']
+        # check can execute by dry run but not real run, may fail by blow reason
+        # 1, gas budget( solve: incr your gas budget)
+        # 2, function limit , some nft one account can only mint once ( solve: check is it has mint before)
+        # 3, no enough sui gas to execute the transaction
+        # etc... see error msg
         if dry_run_status_map['status'] == 'failure':
             raise Exception(dry_run_status_map['error'])
 
         return self.sign_and_execute_transaction(tx_bytes)
 
     def _fetch_and_update_rpc_version(self):
         rpc_version_res = self.provider.get_rpc_version()
```

### Comparing `pysui-sdk-1.0.1/pysui_sdk/wallet.py` & `pysui-sdk-1.0.2/pysui_sdk/wallet.py`

 * *Files identical despite different names*

