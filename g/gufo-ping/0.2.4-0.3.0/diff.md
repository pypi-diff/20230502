# Comparing `tmp/gufo_ping-0.2.4.tar.gz` & `tmp/gufo_ping-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gufo_ping-0.2.4.tar", last modified: Thu Dec 29 08:17:53 2022, max compression
+gzip compressed data, was "gufo_ping-0.3.0.tar", last modified: Tue May  2 07:58:41 2023, max compression
```

## Comparing `gufo_ping-0.2.4.tar` & `gufo_ping-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:17:53.519091 gufo_ping-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2022-12-29 08:17:53.519091 gufo_ping-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2022-12-29 08:17:53.519091 gufo_ping-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      992 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:17:53.519091 gufo_ping-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:17:53.515092 gufo_ping-0.2.4/src/gufo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:17:53.519091 gufo_ping-0.2.4/src/gufo/ping/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/gufo/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/gufo/ping/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/gufo/ping/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/gufo/ping/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/gufo/ping/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:17:53.519091 gufo_ping-0.2.4/src/gufo_ping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2022-12-29 08:17:53.000000 gufo_ping-0.2.4/src/gufo_ping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2022-12-29 08:17:53.000000 gufo_ping-0.2.4/src/gufo_ping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 08:17:53.000000 gufo_ping-0.2.4/src/gufo_ping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 08:17:53.000000 gufo_ping-0.2.4/src/gufo_ping.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-29 08:17:53.000000 gufo_ping-0.2.4/src/gufo_ping.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/icmp.rs
--rw-r--r--   0 runner    (1001) docker     (123)      641 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/session.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2022-12-29 08:17:35.000000 gufo_ping-0.2.4/src/socket.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:41.455087 gufo_ping-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-02 07:58:41.455087 gufo_ping-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-02 07:58:41.455087 gufo_ping-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:41.451087 gufo_ping-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:41.447087 gufo_ping-0.3.0/src/gufo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:41.451087 gufo_ping-0.3.0/src/gufo/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/gufo/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/gufo/ping/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/gufo/ping/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/gufo/ping/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/gufo/ping/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:41.455087 gufo_ping-0.3.0/src/gufo_ping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-02 07:58:41.000000 gufo_ping-0.3.0/src/gufo_ping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-02 07:58:41.000000 gufo_ping-0.3.0/src/gufo_ping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:58:41.000000 gufo_ping-0.3.0/src/gufo_ping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:58:41.000000 gufo_ping-0.3.0/src/gufo_ping.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 07:58:41.000000 gufo_ping-0.3.0/src/gufo_ping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/icmp.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/session.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/src/socket.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:41.455087 gufo_ping-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/tests/test_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/tests/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-02 07:58:23.000000 gufo_ping-0.3.0/tests/test_socket.py
```

### Comparing `gufo_ping-0.2.4/Cargo.toml` & `gufo_ping-0.3.0/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 edition = "2021"
 name = "gufo_ping"
-version = "0.2.3"
+version = "0.3.0"
 
 # See more keys and their definitions 
 # at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 name = "gufo_ping"
 
 [dependencies]
 byteorder = "1.4"
 coarsetime = "0.1"
 internet-checksum = "0.2"
-pyo3 = {version = "0.17", features = ["extension-module"]}
+pyo3 = {version = "0.18", features = ["extension-module"]}
 rand = "0.8"
-socket2 = {version = "0.4", features = ["all"]}
+socket2 = {version = "0.5", features = ["all"]}
 
 [target.'cfg(target_os = "linux")'.dependencies]
 libc = "0.2"
 
 [profile.release]
 strip = "debuginfo"
```

### Comparing `gufo_ping-0.2.4/LICENSE.md` & `gufo_ping-0.3.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright &copy; 2022, Gufo Labs.
+Copyright &copy; 2022-2023, Gufo Labs.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `gufo_ping-0.2.4/PKG-INFO` & `gufo_ping-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gufo_ping
-Version: 0.2.4
+Version: 0.3.0
 Home-page: https://github.com/gufolabs/gufo_ping/
 Author: Gufo Labs
 License: BSD 3-Clause License
 Project-URL: Documentation, https://docs.gufolabs.com/gufo_ping/
 Project-URL: Source Code, https://github.com/gufolabs/gufo_ping/
 Project-URL: Bug Tracker, https://github.com/gufolabs/gufo_ping/issues
 Project-URL: Changelog, https://github.com/gufolabs/gufo_ping/blob/master/CHANGELOG.md
@@ -33,16 +33,17 @@
 # Gufo Ping
 
 *Gufo Ping is the accelerated Python asyncio IPv4/IPv6 ping implementation.*
 
 [![PyPi version](https://img.shields.io/pypi/v/gufo_ping.svg)](https://pypi.python.org/pypi/gufo_ping/)
 ![Python Versions](https://img.shields.io/pypi/pyversions/gufo_ping)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-![Build](https://img.shields.io/github/workflow/status/gufolabs/gufo_ping/Run%20Tests/master)
+![Build](https://img.shields.io/github/actions/workflow/status/gufolabs/gufo_ping/tests.yml?branch=master)
 ![Sponsors](https://img.shields.io/github/sponsors/gufolabs)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 
 ---
 
 **Documentation**: [https://docs.gufolabs.com/gufo_ping/](https://docs.gufolabs.com/gufo_ping/)
 
 **Source Code**: [https://github.com/gufolabs/gufo_ping/](https://github.com/gufolabs/gufo_ping/)
```

### Comparing `gufo_ping-0.2.4/README.md` & `gufo_ping-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Gufo Ping
 
 *Gufo Ping is the accelerated Python asyncio IPv4/IPv6 ping implementation.*
 
 [![PyPi version](https://img.shields.io/pypi/v/gufo_ping.svg)](https://pypi.python.org/pypi/gufo_ping/)
 ![Python Versions](https://img.shields.io/pypi/pyversions/gufo_ping)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-![Build](https://img.shields.io/github/workflow/status/gufolabs/gufo_ping/Run%20Tests/master)
+![Build](https://img.shields.io/github/actions/workflow/status/gufolabs/gufo_ping/tests.yml?branch=master)
 ![Sponsors](https://img.shields.io/github/sponsors/gufolabs)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 
 ---
 
 **Documentation**: [https://docs.gufolabs.com/gufo_ping/](https://docs.gufolabs.com/gufo_ping/)
 
 **Source Code**: [https://github.com/gufolabs/gufo_ping/](https://github.com/gufolabs/gufo_ping/)
```

### Comparing `gufo_ping-0.2.4/setup.cfg` & `gufo_ping-0.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,14 @@
 python_requires = >=3.8
 zip_safe = False
 include_package_data = True
 
 [options.packages.find]
 where = src
 
-[flake8]
-ignore = E203,W503
-
 [options.package_data]
 * = py.typed
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gufo_ping-0.2.4/setup.py` & `gufo_ping-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ---------------------------------------------------------------------
 # Gufo Ping: ICMPv4/ICMPv6 ping implementation
 # Python build
 # ---------------------------------------------------------------------
-# Copyright (C) 2022, Gufo Labs
+# Copyright (C) 2022-23, Gufo Labs
 # ---------------------------------------------------------------------
 
 # Python modules
 from typing import Optional, Sequence
 import os
 
 # Third-party modules
```

### Comparing `gufo_ping-0.2.4/src/gufo/ping/ping.py` & `gufo_ping-0.3.0/src/gufo/ping/socket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,212 +1,203 @@
 # ---------------------------------------------------------------------
-# Gufo Ping: Ping implementation
+# Gufo Ping: PingSocket implementation
 # ---------------------------------------------------------------------
-# Copyright (C) 2022, Gufo Labs
+# Copyright (C) 2022-23, Gufo Labs
 # ---------------------------------------------------------------------
 
+"""
+PingSocket implementation.
+
+Attributes:
+    IPv4: IPv4 address family.
+    IPv6: IPv6 address family.
+"""
+
 # Python modules
-from typing import Optional, Dict, Tuple, AsyncIterable
-import asyncio
-import itertools
-import random
-from time import perf_counter
+from asyncio import Future, get_running_loop, sleep
+from typing import Dict, Optional, cast
 
 # Gufo Labs modules
-from .socket import PingSocket
+from ._fast import SocketWrapper
+from .proto import SocketProto
 
+NS = 1_000_000_000.0
+IPv4 = 4
+IPv6 = 6
+MAX_TTL = 255
+MAX_TOS = 255
 
-class Ping(object):
+
+class PingSocket(object):
     """
-    High-performance asyncronous ICMPv4/ICMPv6 ping client.
+    Python API to Gufo Ping internals.
+
+    Python-side ICMP requests/reply dispatcher for the given address family.
+    Wraps Rust socket implementation.
 
     Args:
+        afi: Address Family. Either 4 or 6
         size: Set outgoing packet's size, including IP header.
+        src_addr: Optional source address of outgoing packets.
         ttl: Set outgoing packet's TTL.
             Use OS defaults when empty.
         tos: Set DSCP/TOS field to outgoing packets.
             Use OS defaults when empty.
         timeout: Default timeout in seconds.
         send_buffer_size: Send buffer size.
             Use OS defaults when empty.
         recv_buffer_size: Receive buffer size.
             Use OS defaults when empty.
         coarse: Use CLOCK_MONOTONIC_COARSE when set,
             fall back to CLOCK_MONOTONIC otherwise.
         accelerated: Enable platform-dependend accelerated
             socket processing.
-
-    Note:
-        Opening the Raw Socket may require super-user priveleges
-        or additional permissions. Refer to the operation system's
-        documentation for details.
-
-    Example:
-        Ping single packet.
-
-        ``` py
-        from gufo.ping import Ping
-
-        async def ping(address):
-            p = Ping()
-            rtt = await p.ping(address)
-            print(rtt)
-        ```
-
-        Ping multiple packets.
-
-        ``` py
-        from gufo.ping import Ping
-
-        async def ping(address):
-            p = Ping()
-            async for rtt in p.iter_rtt(address):
-                print(rtt)
-        ```
     """
 
-    request_id = itertools.count(random.randint(0, 0xFFFF))
-
     def __init__(
-        self,
+        self: "PingSocket",
+        afi: int = IPv4,
         size: int = 64,
+        src_addr: Optional[str] = None,
         ttl: Optional[int] = None,
         tos: Optional[int] = None,
         timeout: float = 1.0,
         send_buffer_size: Optional[int] = None,
         recv_buffer_size: Optional[int] = None,
         coarse: bool = False,
         accelerated: bool = True,
     ) -> None:
+        self.__force_del = False
+        if afi != IPv4 and afi != IPv6:
+            msg = f"afi must be {IPv4} or {IPv6}"
+            raise ValueError(msg)
+        # Check settings
+        if ttl is not None and (ttl < 1 or ttl > MAX_TTL):
+            msg = f"ttl must be in 0..{MAX_TTL} range"
+            raise ValueError(msg)
+        if tos is not None and (tos < 0 or tos > MAX_TOS):
+            msg = f"tos must be in 0..{MAX_TOS} range"
+            raise ValueError(msg)
+        #
         self.__size = size
-        self.__ttl = ttl
-        self.__tos = tos
+        # Create and initialize wrapped socket
+        self.__sock: SocketProto = cast(SocketProto, SocketWrapper(afi))
+        self.__sock.set_timeout(int(timeout * NS))
+        if src_addr:
+            self.__sock.bind(src_addr)
+        if ttl is not None:
+            self.__sock.set_ttl(ttl)
+        if tos is not None:
+            self.__sock.set_tos(tos)
+        if send_buffer_size is not None:
+            self.__sock.set_send_buffer_size(send_buffer_size)
+        if recv_buffer_size is not None:
+            self.__sock.set_recv_buffer_size(recv_buffer_size)
+        if coarse:
+            self.__sock.set_coarse(True)
+        if accelerated:
+            self.__sock.set_accelerated(True)
         self.__timeout = timeout
-        self.__send_buffer_size = send_buffer_size
-        self.__recv_buffer_size = recv_buffer_size
-        self.__coarse = coarse
-        self.__accelerated = accelerated
-        self.__sockets: Dict[int, PingSocket] = {}
-
-    @staticmethod
-    def __get_afi(address: str) -> int:
-        """
-        Get address family (AFI) for a given address.
+        self.__sock_fd = self.__sock.get_fd()
+        #  <addr>-<request id>-<seq> -> future
+        self.__sessions: Dict[str, Future[Optional[float]]] = {}
+        # Install response reader
+        self.__force_del = True
+        get_running_loop().add_reader(self.__sock_fd, self._on_read)
+        # Install deadline cleaner
+        self.__cleanup_task = get_running_loop().create_task(self._cleanup())
+
+    def __del__(self: "PingSocket") -> None:
+        """
+        Perform cleanup on delete.
+
+        * Cancel expiration task.
+        * Remove socket reader.
+        """
+        if not self.__force_del:
+            return
+        try:
+            # Unsubscribe reader
+            # get_running_loop() may raise Runtime Error
+            get_running_loop().remove_reader(self.__sock_fd)
+            # Stop cleanup task
+            if self.__cleanup_task is not None:
+                self.__cleanup_task.cancel()
+        except RuntimeError:  # pragma: no cover
+            pass  # Loop is already closed
 
-        Args:
-            address: Address to ping.
-
-        Returns:
-            * `4` for IPv4
-            * `6` for IPv6
-        """
-        if ":" in address:
-            return 6
-        return 4
-
-    def __get_socket(self, address: str) -> PingSocket:
+    def clean_ip(self: "PingSocket", addr: str) -> str:
         """
-        Get ping socket instance for specified address.
-        Initialize when necessary.
+        Normalize IP address to a stable form.
 
         Args:
-            address: Address to ping
+            addr: IP address
 
         Returns:
-            Initialized socket instance
-        """
-        afi = self.__get_afi(address)
-        sock = self.__sockets.get(afi)
-        if not sock:
-            sock = PingSocket(
-                afi=afi,
-                size=self.__size,
-                ttl=self.__ttl,
-                tos=self.__tos,
-                timeout=self.__timeout,
-                send_buffer_size=self.__send_buffer_size,
-                recv_buffer_size=self.__recv_buffer_size,
-                coarse=self.__coarse,
-                accelerated=self.__accelerated,
-            )
-            self.__sockets[afi] = sock
-        return sock
-
-    def __get_request_id(self) -> Tuple[int, int]:
+            Normalized address
         """
-        Generate ICMP request id and starting
-        sequence number.
-
-        Returns:
-            Tuple of (`request_id`, `sequence`)
-        """
-        request_id = next(self.request_id) & 0xFFFF
-        seq = random.randint(0, 0xFFFF)
-        return request_id, seq
+        return self.__sock.clean_ip(addr)
 
     async def ping(
-        self,
+        self: "PingSocket",
         addr: str,
         size: Optional[int] = None,
+        request_id: int = 0,
+        seq: int = 0,
     ) -> Optional[float]:
         """
-        Send ICMP echo request to the given address and await
-        for response or timeout.
+        Send ICMP echo request and await for result.
 
         Args:
-            addr: IPv4/IPv6 address to ping.
-            size: Packet's size, including IP headers. Use PingSocket
-                intialized defaults, when empty.
-
-        Returns:
-            * Round-trip time in seconds (as float) if success.
-            * None - if failed or timed out.
-        """
-        sock = self.__get_socket(addr)
-        request_id, seq = self.__get_request_id()
-        return await sock.ping(addr, size=size, request_id=request_id, seq=seq)
+            addr: Socket to ping.
+            size: Packet size in bytes, including IP header.
+            request_id: ICMP request id.
+            seq: ICMP sequental number.
+        """
+        if ":" in addr:
+            # Convert IPv6 address to compact form
+            addr = self.__sock.clean_ip(addr)
+        sid = f"{addr}-{request_id}-{seq}"
+        fut: Future[Optional[float]] = get_running_loop().create_future()
+        # Build and send the packet
+        try:
+            self.__sock.send(addr, request_id, seq, size or self.__size)
+        except OSError:
+            # Some kernels raise OSError (Network Unreachable)
+            # when cannot find the route. Treat them as losses.
+            fut.set_result(None)
+            return await fut
+        # Install future in the sessions
+        self.__sessions[sid] = fut
+        # Await response or timeout
+        return await fut
+
+    def _on_read(self: "PingSocket") -> None:
+        """Handle socket read event."""
+        # Get bulk read info from Rust side
+        seen = self.__sock.recv()
+        if seen is None:
+            return
+        # seen is the dict of sid -> rtt
+        for sid, rtt in seen.items():
+            # Find and pop the future in single call
+            fut = self.__sessions.pop(sid, None)
+            if fut:
+                # Pass rtt to the future, unblock await in `ping`
+                fut.set_result(float(rtt) / NS)
 
-    async def iter_rtt(
-        self,
-        addr: str,
-        *,
-        size: Optional[int] = None,
-        interval: Optional[float] = 1.0,
-        count: Optional[int] = None,
-    ) -> AsyncIterable[Optional[float]]:
-        """
-        Send echo request every `interval` seconds,
-        await and yield the result.
-
-        Args:
-            addr: Address to ping.
-            size: Packets' size, including IP headers. Use PingSocket
-                intialized defaults, when empty.
-            interval: Interval between requests, in seconds.
-            count: Stop after `count` requests, if set. Do not stop
-                otherwise.
-
-        Returns:
-            Yields for each attempt:
-
-            * Round-trip time in seconds (as float) if success.
-            * None - if failed or timed out.
-
-        """
-        sock = self.__get_socket(addr)
-        request_id, seq = self.__get_request_id()
-        t0 = 0.0
-        n = 0
+    async def _cleanup(self: "PingSocket") -> None:
+        """Check for expired sessions and close them."""
         while True:
-            if interval:
-                t0 = perf_counter()
-            yield await sock.ping(
-                addr, size=size, request_id=request_id, seq=seq
-            )
-            seq = (seq + 1) & 0xFFFF
-            if interval:
-                dt = perf_counter() - t0
-                if dt < interval:
-                    await asyncio.sleep(interval - dt)
-            n += 1
-            if count and n >= count:
-                break
+            # Wait for next cycle
+            await sleep(self.__timeout)
+            # Get a list of exired sids
+            expired = self.__sock.get_expired()
+            if not expired:
+                continue
+            # Iterate over expired sids
+            for sid in expired:
+                # Find and pop the future by single call
+                fut = self.__sessions.pop(sid, None)
+                if fut:
+                    # Pass None to indicate the timeout
+                    fut.set_result(None)
```

### Comparing `gufo_ping-0.2.4/src/gufo/ping/proto.py` & `gufo_ping-0.3.0/src/gufo/ping/proto.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,144 +1,161 @@
 # ---------------------------------------------------------------------
 # Gufo Ping: SocketProto
 # ---------------------------------------------------------------------
-# Copyright (C) 2022, Gufo Labs
+# Copyright (C) 2022-23, Gufo Labs
 # ---------------------------------------------------------------------
 
+"""SocketWrapper protocol definition."""
 
 # Python modules
-from typing import Optional, List, Dict, Protocol
+from typing import Dict, List, Optional, Protocol
 
 
 class SocketProto(Protocol):
     """
     SocketWrapper protocol.
 
     Socket wrapper is the [PyO3](https://pyo3.rs)-wrapped Rust code,
     implementing low-level details of the PingSocket.
     """
 
-    def __init__(self, afi: int) -> None:
+    def __init__(self: "SocketProto", afi: int) -> None:
         ...
 
-    def set_timeout(self, timeout: int) -> None:
+    def set_timeout(self: "SocketProto", timeout: int) -> None:
         """
         Set default ping timeout.
 
         Args:
             timeout: Ping timeout, in nanoseconds.
         """
         ...
 
-    def set_ttl(self, ttl: int) -> None:
+    def bind(self: "SocketProto", addr: str) -> None:
+        """
+        Bind to source address.
+
+        Args:
+            addr: Source Address
+        """
+
+    def set_ttl(self: "SocketProto", ttl: int) -> None:
         """
         Change outgoing packets' time-to-live field.
 
         Args:
             ttl: TTL value.
         """
         ...
 
-    def set_tos(self, tos: int) -> None:
+    def set_tos(self: "SocketProto", tos: int) -> None:
         """
         Change outgoing packets' ToS/DSCP field.
 
         Args:
             tos: ToS value.
         """
         ...
 
-    def set_coarse(self, ct: bool) -> None:
+    def set_coarse(self: "SocketProto", ct: bool) -> None:
         """
         Switch between the internal timer implemenetation.
 
         Args:
             ct: Use
 
                 * `CLOCK_MONOTONIC_COARSE` if True
                 * `CLOCK_MONOTONIC` if False
         """
         ...
 
-    def set_send_buffer_size(self, size: int) -> None:
+    def set_send_buffer_size(self: "SocketProto", size: int) -> None:
         """
-        Set outgoing socket's buffer size. If the requested
+        Set outgoing socket's buffer size.
+
+        If the requested
         size is too big, adjust to proper size.
 
         Args:
             size: Requested send buffer size, in bytes.
         """
         ...
 
-    def set_recv_buffer_size(self, size: int) -> None:
+    def set_recv_buffer_size(self: "SocketProto", size: int) -> None:
         """
-        Set incoming socket's buffer size. If the requested
+        Set incoming socket's buffer size.
+
+        If the requested
         size is too big, adjust to proper size.
 
         Args:
             size: Requested recv buffer size, in bytes.
         """
         ...
 
-    def set_accelerated(self, a: bool) -> None:
+    def set_accelerated(self: "SocketProto", a: bool) -> None:
         """
         Enable platform-dependend raw socket processing.
 
         Args:
             a: Enable or disable an acceleration.
                 * True - enable, when platform supports acceleration.
                 * False - disable the acceleration.
         """
 
-    def get_fd(self) -> int:  # @todo: Shold be FileDescriptorLike
+    def get_fd(
+        self: "SocketProto",
+    ) -> int:  # @todo: Shold be FileDescriptorLike
         """
         Get socket's file descriptor.
 
         Returns:
             file descriptor for open socket.
         """
         ...
 
-    def send(self, addr: str, request_id: int, seq: int, size: int) -> None:
+    def send(
+        self: "SocketProto", addr: str, request_id: int, seq: int, size: int
+    ) -> None:
         """
         Generate and send icmp request packet.
 
         Args:
             addr: Destination address.
             request_id: ICMP request id.
             seq: ICMP sequental number.
             size: Outgoing packet's size in bytes, including IP header.
         """
         ...
 
-    def recv(self) -> Optional[Dict[str, float]]:
+    def recv(self: "SocketProto") -> Optional[Dict[str, float]]:
         """
         Receive all awaiting packets.
 
         Returns:
             * `None` - when no packets received.
             * Dict of `session id` -> `rtt`,
                 where `session id` is the string of
                 <address>-<request_id>-<seq>,
                 and `rtt` - is the measured round-trip-time in nanoseconds.
         """
         ...
 
-    def get_expired(self) -> Optional[List[str]]:
+    def get_expired(self: "SocketProto") -> Optional[List[str]]:
         """
         Get list of sessions with expired timeouts.
 
         Returns:
             * `None` - when no sessions expired.
             * List of expired sessionn ids, where each session id
                 has the format: <address>-<request_id>-<seq>
         """
         ...
 
-    def clean_ip(self, addr: str) -> str:
+    def clean_ip(self: "SocketProto", addr: str) -> str:
         """
         Normalize IP address to a stable form.
 
         Args:
             addr: IP address
 
         Returns:
```

### Comparing `gufo_ping-0.2.4/src/gufo/ping/socket.py` & `gufo_ping-0.3.0/src/gufo/ping/ping.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,186 +1,271 @@
 # ---------------------------------------------------------------------
-# Gufo Ping: PingSocket implementation
+# Gufo Ping: Ping implementation
 # ---------------------------------------------------------------------
-# Copyright (C) 2022, Gufo Labs
+# Copyright (C) 2022-23, Gufo Labs
 # ---------------------------------------------------------------------
 
+"""Ping client implementation."""
+
 # Python modules
-from typing import Optional, Dict, cast
-from asyncio import Future, get_running_loop, sleep
+import asyncio
+import itertools
+import random
+from time import perf_counter
+from typing import AsyncIterable, Dict, Iterable, Optional, Tuple, Union
 
 # Gufo Labs modules
-from .proto import SocketProto
-from ._fast import SocketWrapper
-
-NS = 1_000_000_000.0
+from .socket import IPv4, IPv6, PingSocket
 
 
-class PingSocket(object):
+class Ping(object):
     """
-    Python-side ICMP requests/reply dispatcher for the given address family.
-    Wraps Rust socket implementation.
+    High-performance asyncronous ICMPv4/ICMPv6 ping client.
 
     Args:
-        afi: Address Family. Either 4 or 6
         size: Set outgoing packet's size, including IP header.
+        src_addr: Set source address for outgoing packets.
+            Depends upon address family. May be one of:
+            * None - detect source address automatically.
+            * str - containing source address for one address family.
+            * Iterable of strings, containing multiple addresses
+                which to be distributed among the address families.
+                First address for given address family will be used.
         ttl: Set outgoing packet's TTL.
             Use OS defaults when empty.
-        tos: Set DSCP/TOS field to outgoing packets.
+
+            !!! warning
+
+                This option is ignored on IPv6 socket due to
+                issue [#4](https://github.com/gufolabs/gufo_ping/issues/4)
+        tos: Set DSCP/TOS/TCLASS field to outgoing packets.
             Use OS defaults when empty.
+
+            !!! warning
+
+                This option is ignored on IPv6 socket due to
+                issue [#2](https://github.com/gufolabs/gufo_ping/issues/2)
         timeout: Default timeout in seconds.
         send_buffer_size: Send buffer size.
             Use OS defaults when empty.
         recv_buffer_size: Receive buffer size.
             Use OS defaults when empty.
         coarse: Use CLOCK_MONOTONIC_COARSE when set,
             fall back to CLOCK_MONOTONIC otherwise.
         accelerated: Enable platform-dependend accelerated
             socket processing.
+
+    Note:
+        Opening the Raw Socket may require super-user priveleges
+        or additional permissions. Refer to the operation system's
+        documentation for details.
+
+    Example:
+        Ping single packet.
+
+        ``` py
+        from gufo.ping import Ping
+
+        async def ping(address):
+            p = Ping()
+            rtt = await p.ping(address)
+            print(rtt)
+        ```
+
+        Ping multiple packets.
+
+        ``` py
+        from gufo.ping import Ping
+
+        async def ping(address):
+            p = Ping()
+            async for rtt in p.iter_rtt(address):
+                print(rtt)
+        ```
     """
 
+    request_id = itertools.count(random.randint(0, 0xFFFF))
+
     def __init__(
-        self,
-        afi: int = 4,
+        self: "Ping",
         size: int = 64,
+        src_addr: Union[None, str, Iterable[str]] = None,
         ttl: Optional[int] = None,
         tos: Optional[int] = None,
         timeout: float = 1.0,
         send_buffer_size: Optional[int] = None,
         recv_buffer_size: Optional[int] = None,
         coarse: bool = False,
         accelerated: bool = True,
-    ):
-        self.__force_del = False
-        if afi != 4 and afi != 6:
-            raise ValueError("afi must be 4 or 6")
-        # Check settings
-        if ttl is not None and (ttl < 1 or ttl > 255):
-            raise ValueError("ttl must be in 0..255 range")
-        if tos is not None and (tos < 0 or tos > 255):
-            raise ValueError("tos must be in 0..255 range")
-        #
+    ) -> None:
         self.__size = size
-        # Create and initialize wrapped socket
-        self.__sock: SocketProto = cast(SocketProto, SocketWrapper(afi))
-        self.__sock.set_timeout(int(timeout * NS))
-        if ttl is not None:
-            self.__sock.set_ttl(ttl)
-        if tos is not None:
-            self.__sock.set_tos(tos)
-        if send_buffer_size is not None:
-            self.__sock.set_send_buffer_size(send_buffer_size)
-        if recv_buffer_size is not None:
-            self.__sock.set_recv_buffer_size(recv_buffer_size)
-        if coarse:
-            self.__sock.set_coarse(True)
-        if accelerated:
-            self.__sock.set_accelerated(True)
+        self.__src_addr = self._get_src_addr(src_addr)
+        self.__ttl = ttl
+        self.__tos = tos
         self.__timeout = timeout
-        self.__sock_fd = self.__sock.get_fd()
-        #  <addr>-<request id>-<seq> -> future
-        self.__sessions: Dict[str, Future[Optional[float]]] = {}
-        # Install response reader
-        self.__force_del = True
-        get_running_loop().add_reader(self.__sock_fd, self.__on_read)
-        # Install deadline cleaner
-        self.__cleanup_task = get_running_loop().create_task(self.__cleanup())
-
-    def __del__(self) -> None:
-        """
-        Perform cleanup on delete:
-
-        * Cancel expiration task.
-        * Remove socket reader.
-        """
-        if not self.__force_del:
-            return
-        try:
-            # Unsubscribe reader
-            # get_running_loop() may raise Runtime Error
-            get_running_loop().remove_reader(self.__sock_fd)
-            # Stop cleanup task
-            if self.__cleanup_task is not None:
-                self.__cleanup_task.cancel()
-        except RuntimeError:  # pragma: no cover
-            pass  # Loop is already closed
+        self.__send_buffer_size = send_buffer_size
+        self.__recv_buffer_size = recv_buffer_size
+        self.__coarse = coarse
+        self.__accelerated = accelerated
+        self.__sockets: Dict[int, PingSocket] = {}
+
+    @staticmethod
+    def _get_afi(address: str) -> int:
+        """
+        Get address family (AFI) for a given address.
+
+        Args:
+            address: Address to ping.
+
+        Returns:
+            * `4` for IPv4
+            * `6` for IPv6
+        """
+        if ":" in address:
+            return IPv6
+        return IPv4
 
-    def clean_ip(self, addr: str) -> str:
+    @staticmethod
+    def _get_src_addr(addr: Union[None, str, Iterable[str]]) -> Dict[int, str]:
         """
-        Normalize IP address to a stable form.
+        Parse source addresses.
+
+        Parse source addresses and distribute them around address families.
 
         Args:
-            addr: IP address
+            addr: One of:
+                * None - detect source address automatically.
+                * str - containing source address for one address family.
+                * Iterable of strings, containing multiple addresses
+                    which to be distributed among the address families.
+                    First address for given address family will be used.
 
         Returns:
-            Normalized address
+            Dict of `address family` -> `source address`.
         """
-        return self.__sock.clean_ip(addr)
+        if not addr:
+            return {}
+        if isinstance(addr, str):
+            return {Ping._get_afi(addr): addr}
+        r: Dict[int, str] = {}
+        for a in addr:
+            afi = Ping._get_afi(a)
+            if afi not in r:
+                r[afi] = a
+        return r
+
+    def __get_socket(self: "Ping", address: str) -> PingSocket:
+        """
+        Get PingSocket instace.
+
+        Get ping socket instance for specified address.
+        Initialize when necessary.
+
+        Args:
+            address: Address to ping
+
+        Returns:
+            Initialized socket instance
+        """
+        afi = self._get_afi(address)
+        sock = self.__sockets.get(afi)
+        if not sock:
+            sock = PingSocket(
+                afi=afi,
+                size=self.__size,
+                src_addr=self.__src_addr.get(afi),
+                ttl=self.__ttl if afi == IPv4 else None,
+                tos=self.__tos if afi == IPv4 else None,
+                timeout=self.__timeout,
+                send_buffer_size=self.__send_buffer_size,
+                recv_buffer_size=self.__recv_buffer_size,
+                coarse=self.__coarse,
+                accelerated=self.__accelerated,
+            )
+            self.__sockets[afi] = sock
+        return sock
+
+    def __get_request_id(self: "Ping") -> Tuple[int, int]:
+        """
+        Get request id.
+
+        Generate ICMP request id and starting
+        sequence number.
+
+        Returns:
+            Tuple of (`request_id`, `sequence`)
+        """
+        request_id = next(self.request_id) & 0xFFFF
+        seq = random.randint(0, 0xFFFF)
+        return request_id, seq
 
     async def ping(
-        self,
+        self: "Ping",
         addr: str,
         size: Optional[int] = None,
-        request_id: int = 0,
-        seq: int = 0,
     ) -> Optional[float]:
         """
-        Send ICMP echo request and await for result.
+        Do ping probe.
+
+        Send ICMP echo request to the given address and await
+        for response or timeout.
 
         Args:
-            addr: Socket to ping.
-            size: Packet size in bytes, including IP header.
-            request_id: ICMP request id.
-            seq: ICMP sequental number.
-        """
-        if ":" in addr:
-            # Convert IPv6 address to compact form
-            addr = self.__sock.clean_ip(addr)
-        sid = f"{addr}-{request_id}-{seq}"
-        fut: Future[Optional[float]] = get_running_loop().create_future()
-        # Build and send the packet
-        try:
-            self.__sock.send(addr, request_id, seq, size or self.__size)
-        except OSError:
-            # Some kernels raise OSError (Network Unreachable)
-            # when cannot find the route. Treat them as losses.
-            fut.set_result(None)
-            return await fut
-        # Install future in the sessions
-        self.__sessions[sid] = fut
-        # Await response or timeout
-        return await fut
-
-    def __on_read(self) -> None:
-        """
-        Handle socket read event.
-        """
-        # Get bulk read info from Rust side
-        seen = self.__sock.recv()
-        if seen is None:
-            return
-        # seen is the dict of sid -> rtt
-        for sid, rtt in seen.items():
-            # Find and pop the future in single call
-            fut = self.__sessions.pop(sid, None)
-            if fut:
-                # Pass rtt to the future, unblock await in `ping`
-                fut.set_result(float(rtt) / NS)
+            addr: IPv4/IPv6 address to ping.
+            size: Packet's size, including IP headers. Use PingSocket
+                intialized defaults, when empty.
 
-    async def __cleanup(self) -> None:
+        Returns:
+            * Round-trip time in seconds (as float) if success.
+            * None - if failed or timed out.
         """
-        Check for expired sessions and close them.
+        sock = self.__get_socket(addr)
+        request_id, seq = self.__get_request_id()
+        return await sock.ping(addr, size=size, request_id=request_id, seq=seq)
+
+    async def iter_rtt(
+        self: "Ping",
+        addr: str,
+        *,
+        size: Optional[int] = None,
+        interval: Optional[float] = 1.0,
+        count: Optional[int] = None,
+    ) -> AsyncIterable[Optional[float]]:
+        """
+        Do the serie of ping probes.
+
+        Send echo request every `interval` seconds,
+        await and yield the result.
+
+        Args:
+            addr: Address to ping.
+            size: Packets' size, including IP headers. Use PingSocket
+                intialized defaults, when empty.
+            interval: Interval between requests, in seconds.
+            count: Stop after `count` requests, if set. Do not stop
+                otherwise.
+
+        Returns:
+            Yields for each attempt:
+
+            * Round-trip time in seconds (as float) if success.
+            * None - if failed or timed out.
+
         """
+        sock = self.__get_socket(addr)
+        request_id, seq = self.__get_request_id()
+        t0 = 0.0
+        n = 0
         while True:
-            # Wait for next cycle
-            await sleep(self.__timeout)
-            # Get a list of exired sids
-            expired = self.__sock.get_expired()
-            if not expired:
-                continue
-            # Iterate over expired sids
-            for sid in expired:
-                # Find and pop the future by single call
-                fut = self.__sessions.pop(sid, None)
-                if fut:
-                    # Pass None to indicate the timeout
-                    fut.set_result(None)
+            if interval:
+                t0 = perf_counter()
+            yield await sock.ping(
+                addr, size=size, request_id=request_id, seq=seq
+            )
+            seq = (seq + 1) & 0xFFFF
+            if interval:
+                dt = perf_counter() - t0
+                if dt < interval:
+                    await asyncio.sleep(interval - dt)
+            n += 1
+            if count and n >= count:
+                break
```

### Comparing `gufo_ping-0.2.4/src/gufo_ping.egg-info/PKG-INFO` & `gufo_ping-0.3.0/src/gufo_ping.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gufo-ping
-Version: 0.2.4
+Version: 0.3.0
 Home-page: https://github.com/gufolabs/gufo_ping/
 Author: Gufo Labs
 License: BSD 3-Clause License
 Project-URL: Documentation, https://docs.gufolabs.com/gufo_ping/
 Project-URL: Source Code, https://github.com/gufolabs/gufo_ping/
 Project-URL: Bug Tracker, https://github.com/gufolabs/gufo_ping/issues
 Project-URL: Changelog, https://github.com/gufolabs/gufo_ping/blob/master/CHANGELOG.md
@@ -33,16 +33,17 @@
 # Gufo Ping
 
 *Gufo Ping is the accelerated Python asyncio IPv4/IPv6 ping implementation.*
 
 [![PyPi version](https://img.shields.io/pypi/v/gufo_ping.svg)](https://pypi.python.org/pypi/gufo_ping/)
 ![Python Versions](https://img.shields.io/pypi/pyversions/gufo_ping)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-![Build](https://img.shields.io/github/workflow/status/gufolabs/gufo_ping/Run%20Tests/master)
+![Build](https://img.shields.io/github/actions/workflow/status/gufolabs/gufo_ping/tests.yml?branch=master)
 ![Sponsors](https://img.shields.io/github/sponsors/gufolabs)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 
 ---
 
 **Documentation**: [https://docs.gufolabs.com/gufo_ping/](https://docs.gufolabs.com/gufo_ping/)
 
 **Source Code**: [https://github.com/gufolabs/gufo_ping/](https://github.com/gufolabs/gufo_ping/)
```

### Comparing `gufo_ping-0.2.4/src/icmp.rs` & `gufo_ping-0.3.0/src/icmp.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // ---------------------------------------------------------------------
 // Gufo Ping: ICMP packet constructing and parsing
 // ---------------------------------------------------------------------
-// Copyright (C) 2022, Gufo Labs
+// Copyright (C) 2022-23, Gufo Labs
 // ---------------------------------------------------------------------
 
 use byteorder::{BigEndian, ByteOrder};
 use internet_checksum::checksum;
 use std::convert::TryFrom;
 use std::mem::MaybeUninit;
```

### Comparing `gufo_ping-0.2.4/src/lib.rs` & `gufo_ping-0.3.0/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // ---------------------------------------------------------------------
 // Gufo Ping: Module definition
 // ---------------------------------------------------------------------
-// Copyright (C) 2022, Gufo Labs
+// Copyright (C) 2022-23, Gufo Labs
 // ---------------------------------------------------------------------
 
 use pyo3::prelude::*;
 pub(crate) mod session;
 pub(crate) use session::Session;
 pub(crate) mod icmp;
 pub(crate) use icmp::IcmpPacket;
```

### Comparing `gufo_ping-0.2.4/src/session.rs` & `gufo_ping-0.3.0/src/session.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // ---------------------------------------------------------------------
 // Gufo Ping: Session implementation
 // ---------------------------------------------------------------------
-// Copyright (C) 2022, Gufo Labs
+// Copyright (C) 2022-23, Gufo Labs
 // ---------------------------------------------------------------------
 
 use std::cmp::Ordering;
 
 /// Ping probe state
 /// sid is a string of <addr>-<request id>-<seq>
 /// deeadline - is timeout deadline in nanoseconds
```

### Comparing `gufo_ping-0.2.4/src/socket.rs` & `gufo_ping-0.3.0/src/socket.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // ---------------------------------------------------------------------
 // Gufo Ping: SocketWrapper implementation
 // ---------------------------------------------------------------------
-// Copyright (C) 2022, Gufo Labs
+// Copyright (C) 2022-23, Gufo Labs
 // ---------------------------------------------------------------------
 
 use super::{IcmpPacket, Session};
 use coarsetime::Clock;
 use pyo3::{
     exceptions::{PyOSError, PyValueError},
     prelude::*,
@@ -18,39 +18,39 @@
 use std::net::{SocketAddrV4, SocketAddrV6};
 use std::os::unix::io::AsRawFd;
 use std::time::Instant;
 
 const MAX_SIZE: usize = 4096;
 const ICMP_SIZE: usize = 8;
 
-enum AFI {
+enum Afi {
     IPV4,
     IPV6,
 }
 
 struct Proto {
-    afi: AFI,
+    afi: Afi,
     domain: Domain,
     protocol: Protocol,
     ip_header_size: usize,
     icmp_request_type: u8,
     icmp_reply_type: u8,
 }
 
 static IPV4: Proto = Proto {
-    afi: AFI::IPV4,
+    afi: Afi::IPV4,
     domain: Domain::IPV4,
     protocol: Protocol::ICMPV4,
     ip_header_size: 20,
     icmp_request_type: 8,
     icmp_reply_type: 0,
 };
 
 static IPV6: Proto = Proto {
-    afi: AFI::IPV6,
+    afi: Afi::IPV6,
     domain: Domain::IPV6,
     protocol: Protocol::ICMPV6,
     ip_header_size: 0, // No IPv6 header is passed over socket
     icmp_request_type: 128,
     icmp_reply_type: 129,
 };
 
@@ -92,14 +92,23 @@
             timeout: 1_000_000_000,
             start: Instant::now(),
             coarse: false,
             buf: unsafe { MaybeUninit::uninit().assume_init() },
         })
     }
 
+    ///
+    fn bind(&mut self, addr: &str) -> PyResult<()> {
+        let src_addr: SockAddr = match self.proto.afi {
+            Afi::IPV4 => SocketAddrV4::new(addr.parse()?, 0).into(),
+            Afi::IPV6 => SocketAddrV6::new(addr.parse()?, 0, 0, 0).into(),
+        };
+        self.io.bind(&src_addr)?;
+        Ok(())
+    }
     /// Set default timeout, in nanoseconds
     fn set_timeout(&mut self, timeout: u64) -> PyResult<()> {
         self.timeout = timeout;
         Ok(())
     }
 
     /// Set default outgoing packets' TTL
@@ -159,25 +168,25 @@
     fn get_fd(&self) -> PyResult<i32> {
         Ok(self.io.as_raw_fd())
     }
 
     /// Normalize address
     fn clean_ip(&self, addr: String) -> PyResult<String> {
         Ok(match self.proto.afi {
-            AFI::IPV4 => SocketAddrV4::new(addr.parse()?, 0).ip().to_string(),
-            AFI::IPV6 => SocketAddrV6::new(addr.parse()?, 0, 0, 0).ip().to_string(),
+            Afi::IPV4 => SocketAddrV4::new(addr.parse()?, 0).ip().to_string(),
+            Afi::IPV6 => SocketAddrV6::new(addr.parse()?, 0, 0, 0).ip().to_string(),
         })
     }
 
     /// Send single ICMP echo request
     fn send(&mut self, addr: String, request_id: u16, seq: u16, size: usize) -> PyResult<()> {
         // Parse IP address
         let to_addr: SockAddr = match self.proto.afi {
-            AFI::IPV4 => SocketAddrV4::new(addr.parse()?, 0).into(),
-            AFI::IPV6 => SocketAddrV6::new(addr.parse()?, 0, 0, 0).into(),
+            Afi::IPV4 => SocketAddrV4::new(addr.parse()?, 0).into(),
+            Afi::IPV6 => SocketAddrV6::new(addr.parse()?, 0, 0, 0).into(),
         };
         // Get timestamp
         let ts = self.get_ts();
         let pkt = IcmpPacket::new(
             self.proto.icmp_request_type,
             request_id,
             seq,
@@ -215,16 +224,16 @@
                     let delay = if ts > pkt_ts {
                         ts - pkt_ts
                     } else {
                         1 // Minimal delay
                     };
                     // Convert SockAddr to printable form
                     let paddr = match self.proto.afi {
-                        AFI::IPV4 => addr.as_socket_ipv4().unwrap().ip().to_string(),
-                        AFI::IPV6 => addr.as_socket_ipv6().unwrap().ip().to_string(),
+                        Afi::IPV4 => addr.as_socket_ipv4().unwrap().ip().to_string(),
+                        Afi::IPV6 => addr.as_socket_ipv6().unwrap().ip().to_string(),
                     };
                     r.insert(pkt.get_sid(paddr.clone()), delay);
                     self.sessions
                         .remove(&Session::new(&pkt.get_sid(paddr), pkt_ts + self.timeout));
                 }
             }
         }
@@ -286,28 +295,28 @@
         fn op(code: u16, jt: u8, jf: u8, k: u32) -> sock_filter {
             sock_filter { code, jt, jf, k }
         }
 
         use libc::sock_filter;
 
         match self.proto.afi {
-            AFI::IPV4 => {
+            Afi::IPV4 => {
                 let filters = [
                     op(0x30, 0, 0, 0x00000014),                           // ldb [20]
                     op(0x15, 0, 5, self.proto.icmp_reply_type as u32),    // jne #0x0, drop
                     op(0x20, 0, 0, 0x0000001c),                           // ld [28]
                     op(0x15, 0, 3, (self.signature >> 32) as u32),        // jne #sig1, drop
                     op(0x20, 0, 0, 0x00000020),                           // ld [32]
                     op(0x15, 0, 1, (self.signature & 0xFFFFFFFF) as u32), // jne #sig2, drop
                     op(0x06, 0, 0, 0xffffffff),                           // ret #-1
                     op(0x06, 0, 0, 0000000000),                           // drop: ret #0
                 ];
                 self.io.attach_filter(&filters)?;
             }
-            AFI::IPV6 => {
+            Afi::IPV6 => {
                 let filters = [
                     op(0x30, 0, 0, 0x00000000),                           // ldb [0]
                     op(0x15, 0, 5, self.proto.icmp_reply_type as u32),    // jne #0x81, drop
                     op(0x20, 0, 0, 0x00000008),                           // ld [8]
                     op(0x15, 0, 3, (self.signature >> 32) as u32),        // jne #sig1, drop
                     op(0x20, 0, 0, 0x0000000c),                           // ld [12]
                     op(0x15, 0, 1, (self.signature & 0xFFFFFFFF) as u32), // jne #sig2, drop
```

