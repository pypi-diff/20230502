# Comparing `tmp/planetmint_transactions-0.8.0.tar.gz` & `tmp/planetmint_transactions-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint_transactions-0.8.0.tar", max compression
+gzip compressed data, was "planetmint_transactions-0.8.1.tar", max compression
```

## Comparing `planetmint_transactions-0.8.0.tar` & `planetmint_transactions-0.8.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    34523 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/LICENSE
--rw-r--r--   0        0        0       73 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/README.md
--rw-r--r--   0        0        0      693 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      831 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/__init__.py
--rw-r--r--   0        0        0     1932 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/crypto.py
--rw-r--r--   0        0        0     3427 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/exceptions.py
--rw-r--r--   0        0        0     5029 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/input.py
--rw-r--r--   0        0        0     1323 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/memoize.py
--rw-r--r--   0        0        0     8321 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/output.py
--rw-r--r--   0        0        0     2606 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/schema/README.md
--rw-r--r--   0        0        0     5231 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/schema/__init__.py
--rw-r--r--   0        0        0     3841 2023-04-05 13:28:43.053746 planetmint_transactions-0.8.0/transactions/common/schema/v1.0/transaction.yaml
--rw-r--r--   0        0        0      787 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v1.0/transaction_create.yaml
--rw-r--r--   0        0        0      778 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v1.0/transaction_transfer.yaml
--rw-r--r--   0        0        0     5070 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction.yaml
--rw-r--r--   0        0        0     1127 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml
--rw-r--r--   0        0        0      742 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_create.yaml
--rw-r--r--   0        0        0      778 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_transfer.yaml
--rw-r--r--   0        0        0     1674 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_validator_election.yaml
--rw-r--r--   0        0        0      843 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_vote.yaml
--rw-r--r--   0        0        0     4363 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction.yaml
--rw-r--r--   0        0        0     1233 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml
--rw-r--r--   0        0        0     1086 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_compose.yaml
--rw-r--r--   0        0        0      950 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_create.yaml
--rw-r--r--   0        0        0     1088 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_decompose.yaml
--rw-r--r--   0        0        0      933 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_transfer.yaml
--rw-r--r--   0        0        0     1780 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_validator_election.yaml
--rw-r--r--   0        0        0      843 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_vote.yaml
--rw-r--r--   0        0        0     1475 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/script.py
--rw-r--r--   0        0        0    33513 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/transaction.py
--rw-r--r--   0        0        0     2645 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/transaction_link.py
--rw-r--r--   0        0        0      332 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/transaction_mode_types.py
--rw-r--r--   0        0        0     7746 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/common/utils.py
--rw-r--r--   0        0        0        0 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/assets/__init__.py
--rw-r--r--   0        0        0     2872 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/assets/compose.py
--rw-r--r--   0        0        0     3280 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/assets/create.py
--rw-r--r--   0        0        0     3195 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/assets/decompose.py
--rw-r--r--   0        0        0     3873 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/assets/transfer.py
--rw-r--r--   0        0        0        0 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/elections/__init__.py
--rw-r--r--   0        0        0      529 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/elections/chain_migration_election.py
--rw-r--r--   0        0        0     2818 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/elections/election.py
--rw-r--r--   0        0        0      792 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/elections/validator_election.py
--rw-r--r--   0        0        0     1497 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/elections/validator_utils.py
--rw-r--r--   0        0        0     1410 2023-04-05 13:28:43.057746 planetmint_transactions-0.8.0/transactions/types/elections/vote.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 planetmint_transactions-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/LICENSE
+-rw-r--r--   0        0        0       73 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/README.md
+-rw-r--r--   0        0        0      693 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      953 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/__init__.py
+-rw-r--r--   0        0        0     1932 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/crypto.py
+-rw-r--r--   0        0        0     3427 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/exceptions.py
+-rw-r--r--   0        0        0     5029 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/input.py
+-rw-r--r--   0        0        0     1323 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/memoize.py
+-rw-r--r--   0        0        0     8319 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/output.py
+-rw-r--r--   0        0        0     2606 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/schema/README.md
+-rw-r--r--   0        0        0     5231 2023-05-02 09:05:46.099022 planetmint_transactions-0.8.1/transactions/common/schema/__init__.py
+-rw-r--r--   0        0        0     3841 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction.yaml
+-rw-r--r--   0        0        0      787 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_create.yaml
+-rw-r--r--   0        0        0      778 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_transfer.yaml
+-rw-r--r--   0        0        0     5070 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction.yaml
+-rw-r--r--   0        0        0     1127 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml
+-rw-r--r--   0        0        0      742 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_create.yaml
+-rw-r--r--   0        0        0      778 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_transfer.yaml
+-rw-r--r--   0        0        0     1674 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_validator_election.yaml
+-rw-r--r--   0        0        0      843 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_vote.yaml
+-rw-r--r--   0        0        0     4363 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction.yaml
+-rw-r--r--   0        0        0     1233 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml
+-rw-r--r--   0        0        0     1086 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_compose.yaml
+-rw-r--r--   0        0        0      950 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_create.yaml
+-rw-r--r--   0        0        0     1088 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_decompose.yaml
+-rw-r--r--   0        0        0      933 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_transfer.yaml
+-rw-r--r--   0        0        0     1780 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_validator_election.yaml
+-rw-r--r--   0        0        0      843 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_vote.yaml
+-rw-r--r--   0        0        0     1475 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/script.py
+-rw-r--r--   0        0        0    33738 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/transaction.py
+-rw-r--r--   0        0        0     2645 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/transaction_link.py
+-rw-r--r--   0        0        0      332 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/transaction_mode_types.py
+-rw-r--r--   0        0        0     7709 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/common/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/__init__.py
+-rw-r--r--   0        0        0     2865 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/compose.py
+-rw-r--r--   0        0        0     3280 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/create.py
+-rw-r--r--   0        0        0     3189 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/decompose.py
+-rw-r--r--   0        0        0     3867 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/assets/transfer.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/chain_migration_election.py
+-rw-r--r--   0        0        0     2817 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/election.py
+-rw-r--r--   0        0        0      792 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/validator_election.py
+-rw-r--r--   0        0        0     1485 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/validator_utils.py
+-rw-r--r--   0        0        0     1410 2023-05-02 09:05:46.103023 planetmint_transactions-0.8.1/transactions/types/elections/vote.py
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 planetmint_transactions-0.8.1/PKG-INFO
```

### Comparing `planetmint_transactions-0.8.0/LICENSE` & `planetmint_transactions-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/pyproject.toml` & `planetmint_transactions-0.8.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "planetmint-transactions"
-version = "0.8.0"
+version = "0.8.1"
 description = "Python implementation of the planetmint transactions spec"
 authors = ["Lorenz Herzberger <lorenzherzberger@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "transactions" }
 ]
```

### Comparing `planetmint_transactions-0.8.0/transactions/common/crypto.py` & `planetmint_transactions-0.8.1/transactions/common/crypto.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/exceptions.py` & `planetmint_transactions-0.8.1/transactions/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/input.py` & `planetmint_transactions-0.8.1/transactions/common/input.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/memoize.py` & `planetmint_transactions-0.8.1/transactions/common/memoize.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/output.py` & `planetmint_transactions-0.8.1/transactions/common/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         if not isinstance(amount, int):
             raise TypeError("`amount` must be a int")
         if amount < 1:
             raise AmountError("`amount` needs to be greater than zero")
         if not isinstance(public_keys, list):
             raise TypeError("`public_keys` must be an instance of list")
         if len(public_keys) == 0:
-            raise ValueError("`public_keys` needs to contain at least one" "owner")
+            raise ValueError("`public_keys` needs to contain at least one owner")
         elif len(public_keys) == 1 and not isinstance(public_keys[0], list):
             if isinstance(public_keys[0], Fulfillment):
                 ffill = public_keys[0]
             else:
                 ffill = Ed25519Sha256(public_key=base58.b58decode(public_keys[0]))
             return cls(ffill, public_keys, amount=amount)
         else:
```

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/README.md` & `planetmint_transactions-0.8.1/transactions/common/schema/README.md`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/__init__.py` & `planetmint_transactions-0.8.1/transactions/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v1.0/transaction.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v1.0/transaction_create.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_create.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v1.0/transaction_transfer.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v1.0/transaction_transfer.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_chain_migration_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_create.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_create.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_transfer.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_transfer.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_validator_election.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_validator_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v2.0/transaction_vote.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v2.0/transaction_vote.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_chain_migration_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_compose.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_compose.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_create.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_create.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_decompose.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_decompose.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_transfer.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_transfer.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_validator_election.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_validator_election.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/schema/v3.0/transaction_vote.yaml` & `planetmint_transactions-0.8.1/transactions/common/schema/v3.0/transaction_vote.yaml`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/script.py` & `planetmint_transactions-0.8.1/transactions/common/script.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/transaction.py` & `planetmint_transactions-0.8.1/transactions/common/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,18 @@
     TRANSFER: str = TRANSFER
     VALIDATOR_ELECTION: str = VALIDATOR_ELECTION
     CHAIN_MIGRATION_ELECTION: str = CHAIN_MIGRATION_ELECTION
     VOTE: str = VOTE
     COMPOSE: str = COMPOSE
     DECOMPOSE: str = DECOMPOSE
     ALLOWED_OPERATIONS: tuple[str, ...] = (CREATE, TRANSFER, COMPOSE, DECOMPOSE)
-    ASSETS: str = ASSETS
-    METADATA: str = METADATA
+    __ASSETS__: str = ASSETS
+    __METADATA__: str = METADATA
     DATA: str = DATA
-    VERSION: str = "3.0"
+    __VERSION__: str = "3.0"
 
     def __init__(
         self,
         operation,
         assets,
         inputs=None,
         outputs=None,
@@ -166,19 +166,19 @@
                         )
                     )
 
         elif operation == self.TRANSFER:
             if not version or version != "2.0":
                 if not (isinstance(assets, list) and "id" in assets[0]):
                     raise TypeError(
-                        ("`assets` must be a list of dicts holding an `id` property " "for 'TRANSFER' Transactions")
+                        ("`assets` must be a list of dicts holding an `id` property for 'TRANSFER' Transactions")
                     )
             else:
                 if not (isinstance(assets, dict) and "id" in assets):
-                    raise TypeError(("`asset` must be a dict holding an `id` property " "for 'TRANSFER' Transactions"))
+                    raise TypeError(("`asset` must be a dict holding an `id` property for 'TRANSFER' Transactions"))
 
         if outputs and not isinstance(outputs, list):
             raise TypeError("`outputs` must be a list instance or None")
 
         if inputs and not isinstance(inputs, list):
             raise TypeError("`inputs` must be a list instance or None")
 
@@ -190,15 +190,15 @@
 
         if script is not None and not isinstance(script, Script):
             raise TypeError("`script` must be a dict or None")
 
         if script is not None and not script.validate():
             raise ValueError("`script` input to output validation failed")
 
-        self.version = version if version is not None else Transaction.VERSION
+        self.version = version if version is not None else Transaction.__VERSION__
         self.operation = operation
         self.assets = assets
         self.inputs = inputs or []
         self.outputs = outputs or []
         self.metadata = metadata
         self.script = script
         self._id = hash_id
@@ -447,15 +447,15 @@
             key_pairs (dict): The keys to sign the Transaction with.
         """
         if isinstance(input_.fulfillment, Ed25519Sha256):
             return cls._sign_ed25519_signature_fulfillment(input_, message, key_pairs)
         elif isinstance(input_.fulfillment, ThresholdSha256):
             return cls._sign_threshold_signature_fulfillment(input_, message, key_pairs)
         else:
-            raise ValueError("Fulfillment couldn't be matched to " "Cryptocondition fulfillment type.")
+            raise ValueError("Fulfillment couldn't be matched to crypto condition fulfillment type.")
 
     @classmethod
     def _sign_ed25519_signature_fulfillment(cls, input_: Input, message: str, key_pairs: dict) -> Input:
         """Signs a Ed25519Fulfillment.
 
         Args:
             input_ (:class:`~transactions.common.transaction.
@@ -547,15 +547,18 @@
         if self.operation == self.CREATE:
             # NOTE: Since in the case of a `CREATE`-transaction we do not have
             #       to check for outputs, we're just submitting dummy
             #       values to the actual method. This simplifies it's logic
             #       greatly, as we do not have to check against `None` values.
             return self._inputs_valid(["dummyvalue" for _ in self.inputs])
         elif self.operation in [self.TRANSFER, self.COMPOSE, self.DECOMPOSE]:
-            return self._inputs_valid([output.fulfillment.condition_uri for output in outputs])
+            conditions = []
+            for i in range(len(outputs)):
+                conditions.append(outputs[i].fulfillment.condition_uri)
+            return self._inputs_valid(conditions)
         elif self.operation == self.VALIDATOR_ELECTION:
             return self._inputs_valid(["dummyvalue" for _ in self.inputs])
         elif self.operation == self.CHAIN_MIGRATION_ELECTION:
             return self._inputs_valid(["dummyvalue" for _ in self.inputs])
         else:
             allowed_ops = ", ".join(self.__class__.ALLOWED_OPERATIONS)
             raise TypeError("`operation` must be one of {}".format(allowed_ops))
@@ -572,15 +575,15 @@
                 Outputs to check the Inputs against.
 
         Returns:
             bool: If all Outputs are valid.
         """
 
         if len(self.inputs) != len(output_condition_uris):
-            raise ValueError("Inputs and " "output_condition_uris must have the same count")
+            raise ValueError("Inputs and output_condition_uris must have the same count")
 
         tx_dict = self.tx_dict if self.tx_dict else self.to_dict()
         tx_dict = Transaction._remove_signatures(tx_dict)
         tx_dict["id"] = None
         tx_serialized = Transaction._to_str(tx_dict)
 
         def validate(i, output_condition_uri=None):
@@ -759,15 +762,15 @@
         if not isinstance(transactions, list):
             transactions = [transactions]
 
         asset_ids = Transaction.get_asset_ids(transactions)
 
         # check that all the transactions have the same asset id
         if len(asset_ids) > 1:
-            raise AssetIdMismatch(("All inputs of all transactions passed" " need to have the same asset id"))
+            raise AssetIdMismatch(("All inputs of all transactions passed need to have the same asset id"))
         return asset_ids.pop()
 
     @staticmethod
     def validate_id(tx_body: dict):
         """Validate the transaction ID of a transaction
 
         Args:
@@ -783,15 +786,15 @@
             raise InvalidHash("No transaction id found!")
 
         tx_body["id"] = None
 
         tx_body_serialized = Transaction._to_str(tx_body)
         valid_tx_id = Transaction._to_hash(tx_body_serialized)
         if proposed_tx_id != valid_tx_id:
-            err_msg = "The transaction's id '{}' isn't equal to " "the hash of its body, i.e. it's not valid."
+            err_msg = "The transaction's id '{}' isn't equal to the hash of its body, i.e. it's not valid."
             raise InvalidHash(err_msg.format(proposed_tx_id))
         return True
 
     @classmethod
     @memoize_from_dict
     def from_dict(cls, tx: dict, skip_schema_validation=True):
         """Transforms a Python dictionary to a Transaction object.
@@ -799,51 +802,55 @@
         Args:
             tx_body (dict): The Transaction to be transformed.
 
         Returns:
             :class:`~transactions.common.transaction.Transaction`
         """
         operation = tx.get("operation", Transaction.CREATE) if isinstance(tx, dict) else Transaction.CREATE
-        cls = Transaction.resolve_class(operation)
+        tx_object = Transaction.resolve_class(operation)
+        if not tx_object:
+            from transactions.common.exceptions import SchemaValidationError
 
-        id = None
+            raise SchemaValidationError("Operation type does not exist.")
+
+        tx_id = None
         try:
-            id = tx["id"]
+            tx_id = tx["id"]
         except KeyError:
-            id = None
+            tx_id = None
         asset_tag = Transaction.get_assets_tag(tx["version"])
         asset_obj = Transaction.get_asset_obj(tx)
         local_dict = {
             "inputs": tx["inputs"],
             "outputs": tx["outputs"],
             "operation": operation,
             "metadata": tx["metadata"],
             asset_tag: asset_obj,
             "version": tx["version"],
-            "id": id,
+            "id": tx_id,
         }
 
         try:
             script_ = tx["script"]
             script_dict = {"script": script_}
         except KeyError:
             script_ = None
             pass
         else:
             local_dict = {**local_dict, **script_dict}
 
         if not skip_schema_validation:
-            cls.validate_id(local_dict)
-            cls.validate_schema(local_dict)
+            tx_object.validate_id(local_dict)
+            tx_object.validate_schema(local_dict)
 
         inputs = [Input.from_dict(input_) for input_ in tx["inputs"]]
         outputs = [Output.from_dict(output) for output in tx["outputs"]]
         asset_obj = Transaction.get_asset_obj(tx)
         script_ = Script.from_dict(script_) if script_ else None
-        return cls(
+        return tx_object(
             tx["operation"],
             asset_obj,
             inputs,
             outputs,
             tx["metadata"],
             tx["version"],
             hash_id=tx["id"],
@@ -853,19 +860,18 @@
 
     type_registry: dict[type, type] = {}
 
     @staticmethod
     def register_type(tx_type, tx_class):
         Transaction.type_registry[tx_type] = tx_class
 
+    @staticmethod
     def resolve_class(operation):
         """For the given `tx` based on the `operation` key return its implementation class"""
-
-        create_txn_class = Transaction.type_registry.get(Transaction.CREATE)
-        return Transaction.type_registry.get(operation, create_txn_class)
+        return Transaction.type_registry.get(operation)
 
     @classmethod
     def validate_schema(cls, tx):
         validate_transaction_schema(tx)
 
     # NOTE: only used for CREATE transactions
     @classmethod
@@ -873,15 +879,15 @@
         inputs = []
         outputs = []
 
         # generate_outputs
         for recipient in recipients:
             if not isinstance(recipient, tuple) or len(recipient) != 2:
                 raise ValueError(
-                    ("Each `recipient` in the list must be a" " tuple of `([<list of public keys>]," " <amount>)`")
+                    ("Each `recipient` in the list must be a tuple of `([<list of public keys>], <amount>)`")
                 )
             pub_keys, amount = recipient
             outputs.append(Output.generate(pub_keys, amount))
 
         # generate inputs
         inputs.append(Input.generate(tx_signers))
```

### Comparing `planetmint_transactions-0.8.0/transactions/common/transaction_link.py` & `planetmint_transactions-0.8.1/transactions/common/transaction_link.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/common/utils.py` & `planetmint_transactions-0.8.1/transactions/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import base58
 import base64
 import time
 import re
 import rapidjson
 from typing import Callable
 
-# from planetmint.config import Config
 from transactions.common.exceptions import ValidationError
 from planetmint_cryptoconditions import ThresholdSha256, Ed25519Sha256, Fulfillment
 from transactions.common.exceptions import ThresholdTooDeep
 from planetmint_cryptoconditions.exceptions import UnsupportedTypeError
 
 VALID_LANGUAGES = (
     "danish",
@@ -167,15 +166,15 @@
 
      Returns:
          None: validation successful
 
      Raises:
          ValidationError: will raise exception in case of regex match.
     """
-    if re.search(r"^[$]|\.|\x00", key):
+    if re.search(r"^([$]|\.|\x00)", key):
         error_str = (
             'Invalid key name "{}" in {} object. The '
             "key name cannot contain characters "
             '".", "$" or null characters'
         ).format(key, obj_name)
         raise ValidationError(error_str)
```

### Comparing `planetmint_transactions-0.8.0/transactions/types/assets/compose.py` & `planetmint_transactions-0.8.1/transactions/types/assets/compose.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         if len(input_tx_ids) < len(asset_ids):
             raise ValueError("there must be at least one input per consumed asset")
 
         outputs = []
         for recipient in recipients:
             if not isinstance(recipient, tuple) or len(recipient) != 2:
                 raise ValueError(
-                    ("Each `recipient` in the list must be a" " tuple of `([<list of public keys>]," " <amount>)`")
+                    ("Each `recipient` in the list must be a tuple of `([<list of public keys>],<amount>)`")
                 )
             pub_keys, amount = recipient
             outputs.append(Output.generate(pub_keys, amount))
 
         if len(outputs) != 1:
             raise ValueError("compose transactions only allow a single ouptut")
```

### Comparing `planetmint_transactions-0.8.0/transactions/types/assets/create.py` & `planetmint_transactions-0.8.1/transactions/types/assets/create.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/types/assets/decompose.py` & `planetmint_transactions-0.8.1/transactions/types/assets/decompose.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             raise ValueError("decompose must create at least one new `asset`")
 
         outputs = []
         recipient_pub_keys = []
         for recipient in recipients:
             if not isinstance(recipient, tuple) or len(recipient) != 2:
                 raise ValueError(
-                    ("Each `recipient` in the list must be a" " tuple of `([<list of public keys>]," " <amount>)`")
+                    ("Each `recipient` in the list must be a tuple of `([<list of public keys>], <amount>)`")
                 )
             pub_keys, amount = recipient
             if len(pub_keys) != 1:
                 raise ValueError("decompose transactions only allow for one recipient")
             recipient_pub_keys.append(pub_keys[0])
             outputs.append(Output.generate(pub_keys, amount))
```

### Comparing `planetmint_transactions-0.8.0/transactions/types/assets/transfer.py` & `planetmint_transactions-0.8.1/transactions/types/assets/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         if len(recipients) == 0:
             raise ValueError("`recipients` list cannot be empty")
 
         outputs = []
         for recipient in recipients:
             if not isinstance(recipient, tuple) or len(recipient) != 2:
                 raise ValueError(
-                    ("Each `recipient` in the list must be a" " tuple of `([<list of public keys>]," " <amount>)`")
+                    ("Each `recipient` in the list must be a tuple of `([<list of public keys>], <amount>)`")
                 )
             pub_keys, amount = recipient
             outputs.append(Output.generate(pub_keys, amount))
 
         if not isinstance(asset_ids, list):
             raise TypeError("`asset_ids` must be a list of strings")
```

### Comparing `planetmint_transactions-0.8.0/transactions/types/elections/chain_migration_election.py` & `planetmint_transactions-0.8.1/transactions/types/elections/chain_migration_election.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/types/elections/election.py` & `planetmint_transactions-0.8.1/transactions/types/elections/election.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ONGOING: str = "ongoing"
     CONCLUDED: str = "concluded"
     INCONCLUSIVE: str = "inconclusive"
     # Vote ratio to approve an election
     ELECTION_THRESHOLD = 2 / 3
 
     @classmethod
-    def validate_election(self, tx_signers, recipients, assets, metadata):
+    def validate_election(cls, tx_signers, recipients, assets, metadata):
         if not isinstance(tx_signers, list):
             raise TypeError("`tx_signers` must be a list instance")
         if not isinstance(recipients, list):
             raise TypeError("`recipients` must be a list instance")
         if len(tx_signers) == 0:
             raise ValueError("`tx_signers` list cannot be empty")
         if len(recipients) == 0:
```

### Comparing `planetmint_transactions-0.8.0/transactions/types/elections/validator_election.py` & `planetmint_transactions-0.8.1/transactions/types/elections/validator_election.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/transactions/types/elections/validator_utils.py` & `planetmint_transactions-0.8.1/transactions/types/elections/validator_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     except binascii.Error:
         raise InvalidPublicKey("Invalid `type` specified for public key `value`")
 
 
 def get_public_key_decoder(pk):
     encoding = pk["type"]
-    decoder = base64.b64decode
+    decoder = None
 
     if encoding == "ed25519-base16":
         decoder = base64.b16decode
     elif encoding == "ed25519-base32":
         decoder = base64.b32decode
     elif encoding == "ed25519-base64":
         decoder = base64.b64decode
```

### Comparing `planetmint_transactions-0.8.0/transactions/types/elections/vote.py` & `planetmint_transactions-0.8.1/transactions/types/elections/vote.py`

 * *Files identical despite different names*

### Comparing `planetmint_transactions-0.8.0/PKG-INFO` & `planetmint_transactions-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint-transactions
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python implementation of the planetmint transactions spec
 Author: Lorenz Herzberger
 Author-email: lorenzherzberger@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

