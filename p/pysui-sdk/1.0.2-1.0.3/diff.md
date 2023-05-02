# Comparing `tmp/pysui-sdk-1.0.2.tar.gz` & `tmp/pysui-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysui-sdk-1.0.2.tar", last modified: Tue May  2 08:16:39 2023, max compression
+gzip compressed data, was "pysui-sdk-1.0.3.tar", last modified: Tue May  2 10:31:21 2023, max compression
```

## Comparing `pysui-sdk-1.0.2.tar` & `pysui-sdk-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 08:16:39.703226 pysui-sdk-1.0.2/
--rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 08:16:39.703117 pysui-sdk-1.0.2/PKG-INFO
--rw-r--r--   0 guomaoye   (501) staff       (20)     2587 2023-05-02 08:16:18.000000 pysui-sdk-1.0.2/README.md
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 08:16:39.702389 pysui-sdk-1.0.2/pysui_sdk/
--rw-r--r--   0 guomaoye   (501) staff       (20)       85 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/__init__.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1428 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/models.py
--rw-r--r--   0 guomaoye   (501) staff       (20)    11096 2023-05-02 08:15:58.000000 pysui-sdk-1.0.2/pysui_sdk/provider.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1900 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/rpc_tx_data_serializer.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1258 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/signer.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     2492 2023-05-02 06:50:24.000000 pysui-sdk-1.0.2/pysui_sdk/signer_with_provider.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1517 2023-05-02 05:04:49.000000 pysui-sdk-1.0.2/pysui_sdk/wallet.py
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 08:16:39.702959 pysui-sdk-1.0.2/pysui_sdk.egg-info/
--rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/PKG-INFO
--rw-r--r--   0 guomaoye   (501) staff       (20)      356 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)        1 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       13 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/requires.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       10 2023-05-02 08:16:39.000000 pysui-sdk-1.0.2/pysui_sdk.egg-info/top_level.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       38 2023-05-02 08:16:39.703264 pysui-sdk-1.0.2/setup.cfg
--rw-r--r--   0 guomaoye   (501) staff       (20)      409 2023-05-02 08:15:58.000000 pysui-sdk-1.0.2/setup.py
+drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 10:31:21.636467 pysui-sdk-1.0.3/
+-rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 10:31:21.636360 pysui-sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 guomaoye   (501) staff       (20)     2587 2023-05-02 08:16:18.000000 pysui-sdk-1.0.3/README.md
+drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 10:31:21.635573 pysui-sdk-1.0.3/pysui_sdk/
+-rw-r--r--   0 guomaoye   (501) staff       (20)       85 2023-05-02 05:04:49.000000 pysui-sdk-1.0.3/pysui_sdk/__init__.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1428 2023-05-02 05:04:49.000000 pysui-sdk-1.0.3/pysui_sdk/models.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)    11743 2023-05-02 10:30:41.000000 pysui-sdk-1.0.3/pysui_sdk/provider.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1900 2023-05-02 05:04:49.000000 pysui-sdk-1.0.3/pysui_sdk/rpc_tx_data_serializer.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1258 2023-05-02 05:04:49.000000 pysui-sdk-1.0.3/pysui_sdk/signer.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     2492 2023-05-02 08:48:54.000000 pysui-sdk-1.0.3/pysui_sdk/signer_with_provider.py
+-rw-r--r--   0 guomaoye   (501) staff       (20)     1517 2023-05-02 05:04:49.000000 pysui-sdk-1.0.3/pysui_sdk/wallet.py
+drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-02 10:31:21.636194 pysui-sdk-1.0.3/pysui_sdk.egg-info/
+-rw-r--r--   0 guomaoye   (501) staff       (20)      299 2023-05-02 10:31:21.000000 pysui-sdk-1.0.3/pysui_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 guomaoye   (501) staff       (20)      356 2023-05-02 10:31:21.000000 pysui-sdk-1.0.3/pysui_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)        1 2023-05-02 10:31:21.000000 pysui-sdk-1.0.3/pysui_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)       13 2023-05-02 10:31:21.000000 pysui-sdk-1.0.3/pysui_sdk.egg-info/requires.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)       10 2023-05-02 10:31:21.000000 pysui-sdk-1.0.3/pysui_sdk.egg-info/top_level.txt
+-rw-r--r--   0 guomaoye   (501) staff       (20)       38 2023-05-02 10:31:21.636510 pysui-sdk-1.0.3/setup.cfg
+-rw-r--r--   0 guomaoye   (501) staff       (20)      409 2023-05-02 10:31:13.000000 pysui-sdk-1.0.3/setup.py
```

### Comparing `pysui-sdk-1.0.2/README.md` & `pysui-sdk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.2/pysui_sdk/models.py` & `pysui-sdk-1.0.3/pysui_sdk/models.py`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.2/pysui_sdk/provider.py` & `pysui-sdk-1.0.3/pysui_sdk/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,31 @@
 
     def get_dynamic_field_object(self, parent_object_id: str, dynamic_field_name: str):
         return self.send_request_to_rpc(method="suix_getDynamicFieldObject", params=[parent_object_id, dynamic_field_name])
 
     def get_dynamic_fields(self, parent_object_id: str, cursor: str = None, limit: int = 10):
         return self.send_request_to_rpc(method="suix_getDynamicFields", params=[parent_object_id, cursor, limit])
 
+    def split_coins(self, address: str, coin_object_id: str, split_amount: list[str], gas=None, gas_budget="100000"):
+        return self.send_request_to_rpc(method="unsafe_splitCoin", params=[
+            address,
+            coin_object_id,
+            split_amount,
+            gas,
+            gas_budget
+        ])
+
+    def transfer_objects(self, address: str, transfer_object_id: str, recipient: str, gas=None, gas_budget="100000"):
+        return self.send_request_to_rpc(method="unsafe_transferObject", params=[
+            address,
+            transfer_object_id,
+            gas,
+            gas_budget,
+            recipient
+        ])
     # def get_objects_owned_by_object(self, object_id: str):
     #     return self.send_request_to_rpc(method="sui_getObjectsOwnedByObject", params=[object_id])
 
     # def get_objects_owned_by_address(self, addr: str):
     #     return self.send_request_to_rpc(method="suix_getBalance", params=[addr])
 
     # def get_transactions(self,
```

### Comparing `pysui-sdk-1.0.2/pysui_sdk/rpc_tx_data_serializer.py` & `pysui-sdk-1.0.3/pysui_sdk/rpc_tx_data_serializer.py`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.2/pysui_sdk/signer.py` & `pysui-sdk-1.0.3/pysui_sdk/signer.py`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.2/pysui_sdk/signer_with_provider.py` & `pysui-sdk-1.0.3/pysui_sdk/signer_with_provider.py`

 * *Files identical despite different names*

### Comparing `pysui-sdk-1.0.2/pysui_sdk/wallet.py` & `pysui-sdk-1.0.3/pysui_sdk/wallet.py`

 * *Files identical despite different names*

