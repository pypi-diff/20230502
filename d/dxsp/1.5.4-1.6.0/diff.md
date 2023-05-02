# Comparing `tmp/dxsp-1.5.4.tar.gz` & `tmp/dxsp-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.5.4.tar", max compression
+gzip compressed data, was "dxsp-1.6.0.tar", max compression
```

## Comparing `dxsp-1.5.4.tar` & `dxsp-1.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-01 20:09:39.184575 dxsp-1.5.4/LICENSE
--rw-r--r--   0        0        0     3225 2023-05-01 20:09:39.184575 dxsp-1.5.4/README.md
--rw-r--r--   0        0        0       38 2023-05-01 20:09:39.184575 dxsp-1.5.4/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-01 20:09:39.992581 dxsp-1.5.4/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-01 20:09:39.184575 dxsp-1.5.4/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-01 20:09:39.184575 dxsp-1.5.4/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-01 20:09:39.184575 dxsp-1.5.4/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-05-01 20:09:39.184575 dxsp-1.5.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0    29282 2023-05-01 20:09:39.184575 dxsp-1.5.4/dxsp/main.py
--rw-r--r--   0        0        0     1045 2023-05-01 20:09:39.992581 dxsp-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-02 06:34:10.479825 dxsp-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-05-02 06:34:10.479825 dxsp-1.6.0/README.md
+-rw-r--r--   0        0        0       38 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-02 06:34:11.219831 dxsp-1.6.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/config.py
+-rw-r--r--   0        0        0      564 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    29576 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/main.py
+-rw-r--r--   0        0        0     1045 2023-05-02 06:34:11.215831 dxsp-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.6.0/PKG-INFO
```

### Comparing `dxsp-1.5.4/LICENSE` & `dxsp-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.4/README.md` & `dxsp-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.4/dxsp/assets/blockchains.py` & `dxsp-1.6.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.4/dxsp/default_settings.toml` & `dxsp-1.6.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.4/dxsp/main.py` & `dxsp-1.6.0/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 if amount_trading_option == 1:
                     #buy or sell %p percentage DEFAULT OPTION
                     asset_out_amount = ((asset_out_balance)/
                                         (10 ** asset_out_decimals))*(float(quantity)/100)
                 if amount_trading_option == 2:
                     #SELL all token in case of sell order for example
                     asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals)
-                order = self.get_swap(
+                order = await self.get_swap(
                         asset_out_symbol,
                         asset_in_symbol,
                         asset_out_amount
                         )
                 if order:
                     return order['confirmation']
 
@@ -535,20 +535,27 @@
     async def get_token_balance(
                                 self,
                                 token
                             ):
         self.logger.debug("get_token_balance %s", token)
         try:
             token_address = await self.search_contract(token)
-            token_abi =  await self.get_abi(token_address)
+            if token_address is None:
+                raise ValueError(f"Token address not found for {token}")
+            token_abi = await self.get_abi(token_address)
+            if token_abi is None:
+                raise ValueError(f"ABI not found for {token_address}")
             token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
-            token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
-            self.logger.debug("token_address %s token_balance %s",token_address,token_balance)
+            token_balance = 0
+            try:
+                token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
+            except ValueError as e:
+                self.logger.warning("Invalid address %s for token %s: %s", self.wallet_address, token, e)
             # (ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
-            return 0 if token_balance <=0 or token_balance is None else token_balance
+            return 0 if token_balance <=0 else token_balance
         except Exception as e:
             self.logger.error("get_token_balance %s: %s",token, e)
             return 0
 
     async def get_basecoin_balance(
                                 self
                             ):
```

### Comparing `dxsp-1.5.4/pyproject.toml` & `dxsp-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.5.4"
+version = "1.6.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.5.4/PKG-INFO` & `dxsp-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.5.4
+Version: 1.6.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

