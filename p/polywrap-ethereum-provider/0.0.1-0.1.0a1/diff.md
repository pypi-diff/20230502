# Comparing `tmp/polywrap_ethereum_provider-0.0.1.tar.gz` & `tmp/polywrap_ethereum_provider-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_ethereum_provider-0.0.1.tar", max compression
+gzip compressed data, was "polywrap_ethereum_provider-0.1.0a1.tar", max compression
```

## Comparing `polywrap_ethereum_provider-0.0.1.tar` & `polywrap_ethereum_provider-0.1.0a1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     3017 2023-04-14 00:08:26.322250 polywrap_ethereum_provider-0.0.1/polywrap_ethereum_provider/__init__.py
--rw-r--r--   0        0        0     1862 2023-04-14 00:08:26.322250 polywrap_ethereum_provider-0.0.1/polywrap_ethereum_provider/connection.py
--rw-r--r--   0        0        0     3147 2023-04-14 00:08:26.326250 polywrap_ethereum_provider-0.0.1/polywrap_ethereum_provider/connections.py
--rw-r--r--   0        0        0      559 2023-04-11 15:28:55.628769 polywrap_ethereum_provider-0.0.1/polywrap_ethereum_provider/networks.py
--rw-r--r--   0        0        0      519 2023-04-11 16:00:10.761474 polywrap_ethereum_provider-0.0.1/polywrap_ethereum_provider/wrap/types.py
--rw-r--r--   0        0        0     1095 2023-04-14 00:08:12.815084 polywrap_ethereum_provider-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.0.1/setup.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6850 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/connection.py
+-rw-r--r--   0        0        0     2837 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/connections.py
+-rw-r--r--   0        0        0     1451 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/networks.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/py.typed
+-rw-r--r--   0        0        0     1509 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a1/PKG-INFO
```

### Comparing `polywrap_ethereum_provider-0.0.1/polywrap_ethereum_provider/connection.py` & `polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/connection.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,54 @@
-from dataclasses import dataclass
-from web3 import Web3
-from eth_account.signers.local import LocalAccount
-from typing import Optional, Union, cast
-
-from polywrap_ethereum_provider.networks import KnownNetwork, get_network_name
-
-EthereumProvider = str | Web3.HTTPProvider
+"""This module contains a connection class for an EVM network."""
+from typing import Optional, Tuple
 
+from web3 import Web3
+from web3.providers.base import JSONBaseProvider
 
-@dataclass(slots=True, kw_only=True)
-class ConnectionConfig:
-    provider: EthereumProvider
-    signer: Optional[LocalAccount]
+from polywrap_ethereum_provider.networks import KnownNetwork
 
 
 class Connection:
-    provider: Web3.HTTPProvider
-    signer: Optional[LocalAccount]
+    """Defines a connection to an EVM network."""
 
-    def __init__(self, config: ConnectionConfig):
-        self.set_provider(config.provider)
+    __slots__: Tuple[str, str] = ("_provider", "_signer")
 
-        if config.signer:
-            self.set_signer(config.signer)
-
-    def set_provider(self, provider: EthereumProvider):
-        if isinstance(provider, str):
-            self.provider = Web3.HTTPProvider(provider)
-        else:
-            self.provider = provider
-
-    def set_signer(self, signer: LocalAccount):
-        self.signer = signer
-
-    def get_provider(self) -> Web3.HTTPProvider:
-        return self.provider
-    
-    def get_signer(self) -> LocalAccount:
-        if not self.signer:
-            raise RuntimeError("Signer not found")
-        return self.signer
-
-    @staticmethod
-    def from_node(node: str):
-        config = ConnectionConfig(provider=node, signer=None)
-        return Connection(config=config)
-
-    @staticmethod
-    def from_network(network: Union[KnownNetwork, int]):
-        network_name = (
-            get_network_name(network)
-            if isinstance(network, int)
-            else cast(str, network)
-        )
-        if not network_name:
-            raise RuntimeError(f"Network: {str(network)} not found")
+    _provider: JSONBaseProvider
+    _signer: Optional[str]  # Private key
 
+    def __init__(self, provider: JSONBaseProvider | str, signer: Optional[str]):
+        """Initialize a connection to an EVM network."""
+        self._provider = Web3.HTTPProvider(provider) if isinstance(provider, str) else provider
+        self._signer = signer
+
+    @property
+    def provider(self) -> JSONBaseProvider:
+        """EVM network provider."""
+        return self._provider
+
+    @property
+    def signer(self) -> str:
+        """Private key for signing transactions."""
+        if not self._signer:
+            raise ValueError(f"signer is not set for {self}")
+        return self._signer
+
+    @classmethod
+    def from_node(cls, node: str, signer: Optional[str] = None):
+        """Create a connection from a node URL."""
+        return cls(provider=node, signer=signer)
+
+    @classmethod
+    def from_network(cls, network: KnownNetwork, signer: Optional[str] = None):
+        """Create a connection from a known network."""
         provider = (
-            f"https://{network_name}.infura.io/v3/1a8e6a8ab1df44ccb77d3e954082c5d4"
+            f"https://{network.name}.infura.io/v3/1a8e6a8ab1df44ccb77d3e954082c5d4"
         )
-        config = ConnectionConfig(provider=provider, signer=None)
-        return Connection(config=config)
+        return cls(provider=provider, signer=signer)
+
+    def __str__(self) -> str:
+        """String representation of the connection."""
+        return f"Connection: {self.provider}"
+
+    def has_signer(self) -> bool:
+        """Returns true if the connection has a signer."""
+        return self._signer is not None
```

### Comparing `polywrap_ethereum_provider-0.0.1/pyproject.toml` & `polywrap_ethereum_provider-0.1.0a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,77 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-name = "polywrap_ethereum-provider"
-version = "0.0.1"
+name = "polywrap-ethereum-provider"
+version = "0.1.0a1"
 description = "Ethereum provider in python"
 authors = ["Cesar <cesar@polywrap.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "6.1.0"
 eth_account = "0.8.0"
-polywrap-plugin = "0.1.0a28"
+polywrap-plugin = "0.1.0a29"
+polywrap-core = "^0.1.0a29"
+polywrap-msgpack = "^0.1.0a29"
+polywrap-manifest = "^0.1.0a29"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
 pydocstyle = "^6.1.1"
-polywrap-client = "0.1.0a28"
-polywrap-client-config-builder = "0.1.0a28"
+polywrap-client = "0.1.0a29"
+polywrap-client-config-builder = "0.1.0a29"
+polywrap-uri-resolvers = "^0.1.0a29"
+
+[tool.poetry.group.dev.dependencies]
+eth-tester = "^0.8.0b3"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
+exclude = [
+    "polywrap_ethereum_provider/wrap"
+]
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportShadowedImports = false
+exclude = [
+    "**/wrap/"
+]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = [
-    "tests"
+    "tests",
 ]
 
 [tool.pylint]
 disable = [
     "too-many-return-statements",
+    "invalid-name",
+    "unused-argument",
+    "unused-variable",
 ]
-ignore = [
-    "tests/"
+ignore-paths = [
+    "polywrap_ethereum_provider/wrap"
 ]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
+skip = ["polywrap_ethereum_provider/wrap"]
 
 [tool.pydocstyle]
 # default
```

