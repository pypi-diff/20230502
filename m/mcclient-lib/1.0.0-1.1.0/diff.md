# Comparing `tmp/mcclient-lib-1.0.0.tar.gz` & `tmp/mcclient-lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcclient-lib-1.0.0.tar", last modified: Thu Apr 27 15:53:53 2023, max compression
+gzip compressed data, was "mcclient-lib-1.1.0.tar", last modified: Tue May  2 14:23:00 2023, max compression
```

## Comparing `mcclient-lib-1.0.0.tar` & `mcclient-lib-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.681413 mcclient-lib-1.0.0/
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1090 2023-02-17 12:34:30.000000 mcclient-lib-1.0.0/LICENSE
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3698 2023-04-27 15:53:53.678483 mcclient-lib-1.0.0/PKG-INFO
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3266 2023-04-25 18:09:46.000000 mcclient-lib-1.0.0/README.md
-drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.227221 mcclient-lib-1.0.0/mcclient/
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      196 2023-04-26 19:07:22.000000 mcclient-lib-1.0.0/mcclient/__init__.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1590 2023-04-27 14:48:51.000000 mcclient-lib-1.0.0/mcclient/address.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2835 2023-04-27 14:52:51.000000 mcclient-lib-1.0.0/mcclient/base_client.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1763 2023-04-27 14:54:50.000000 mcclient-lib-1.0.0/mcclient/bedrock_slp.py
-drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.324435 mcclient-lib-1.0.0/mcclient/encoding/
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-01-27 20:41:53.000000 mcclient-lib-1.0.0/mcclient/encoding/__init__.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1246 2023-04-26 20:35:05.000000 mcclient-lib-1.0.0/mcclient/encoding/packet.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      751 2023-04-26 20:24:04.000000 mcclient-lib-1.0.0/mcclient/encoding/varint.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3486 2023-04-27 14:56:04.000000 mcclient-lib-1.0.0/mcclient/query_client.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     7222 2023-04-27 15:19:29.000000 mcclient-lib-1.0.0/mcclient/response.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2062 2023-04-27 14:59:01.000000 mcclient-lib-1.0.0/mcclient/slp.py
-drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.464600 mcclient-lib-1.0.0/mcclient_lib.egg-info/
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3698 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      611 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        1 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)       24 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/requires.txt
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        9 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/top_level.txt
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      861 2023-04-27 15:19:55.000000 mcclient-lib-1.0.0/pyproject.toml
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)       38 2023-04-27 15:53:53.682388 mcclient-lib-1.0.0/setup.cfg
-drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.650164 mcclient-lib-1.0.0/tests/
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      421 2023-04-26 20:25:33.000000 mcclient-lib-1.0.0/tests/test_address.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1497 2023-04-26 18:55:31.000000 mcclient-lib-1.0.0/tests/test_bedrock.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      753 2023-04-26 20:33:35.000000 mcclient-lib-1.0.0/tests/test_encoding.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1038 2023-04-26 18:53:32.000000 mcclient-lib-1.0.0/tests/test_formatting_removal.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1343 2023-04-26 18:52:08.000000 mcclient-lib-1.0.0/tests/test_legacy_slp.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     4257 2023-04-26 18:56:39.000000 mcclient-lib-1.0.0/tests/test_query.py
--rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2019 2023-04-26 20:35:54.000000 mcclient-lib-1.0.0/tests/test_slp.py
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-05-02 14:23:00.120646 mcclient-lib-1.1.0/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1090 2023-02-17 12:34:30.000000 mcclient-lib-1.1.0/LICENSE
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3698 2023-05-02 14:23:00.116739 mcclient-lib-1.1.0/PKG-INFO
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3266 2023-05-02 12:42:21.000000 mcclient-lib-1.1.0/README.md
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-05-02 14:22:59.663914 mcclient-lib-1.1.0/mcclient/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      199 2023-05-02 13:10:04.000000 mcclient-lib-1.1.0/mcclient/__init__.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1459 2023-05-02 14:13:27.000000 mcclient-lib-1.1.0/mcclient/address.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2835 2023-04-27 14:52:51.000000 mcclient-lib-1.1.0/mcclient/base_client.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1620 2023-05-02 14:13:55.000000 mcclient-lib-1.1.0/mcclient/bedrock_client.py
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-05-02 14:22:59.763085 mcclient-lib-1.1.0/mcclient/encoding/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-01-27 20:41:53.000000 mcclient-lib-1.1.0/mcclient/encoding/__init__.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1246 2023-04-26 20:35:05.000000 mcclient-lib-1.1.0/mcclient/encoding/packet.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      751 2023-04-26 20:24:04.000000 mcclient-lib-1.1.0/mcclient/encoding/varint.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3486 2023-04-27 14:56:04.000000 mcclient-lib-1.1.0/mcclient/query_client.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     7222 2023-04-27 15:19:29.000000 mcclient-lib-1.1.0/mcclient/response.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2062 2023-04-27 14:59:01.000000 mcclient-lib-1.1.0/mcclient/slp.py
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-05-02 14:22:59.906884 mcclient-lib-1.1.0/mcclient_lib.egg-info/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3698 2023-05-02 14:22:59.000000 mcclient-lib-1.1.0/mcclient_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      614 2023-05-02 14:22:59.000000 mcclient-lib-1.1.0/mcclient_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        1 2023-05-02 14:22:59.000000 mcclient-lib-1.1.0/mcclient_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)       24 2023-05-02 14:22:59.000000 mcclient-lib-1.1.0/mcclient_lib.egg-info/requires.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        9 2023-05-02 14:22:59.000000 mcclient-lib-1.1.0/mcclient_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      861 2023-05-02 14:17:02.000000 mcclient-lib-1.1.0/pyproject.toml
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)       38 2023-05-02 14:23:00.121621 mcclient-lib-1.1.0/setup.cfg
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-05-02 14:23:00.088385 mcclient-lib-1.1.0/tests/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      421 2023-04-26 20:25:33.000000 mcclient-lib-1.1.0/tests/test_address.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1497 2023-04-26 18:55:31.000000 mcclient-lib-1.1.0/tests/test_bedrock.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      753 2023-04-26 20:33:35.000000 mcclient-lib-1.1.0/tests/test_encoding.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1038 2023-04-26 18:53:32.000000 mcclient-lib-1.1.0/tests/test_formatting_removal.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1343 2023-04-26 18:52:08.000000 mcclient-lib-1.1.0/tests/test_legacy_slp.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     4257 2023-04-26 18:56:39.000000 mcclient-lib-1.1.0/tests/test_query.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2019 2023-04-26 20:35:54.000000 mcclient-lib-1.1.0/tests/test_slp.py
```

### Comparing `mcclient-lib-1.0.0/LICENSE` & `mcclient-lib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/PKG-INFO` & `mcclient-lib-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcclient-lib
-Version: 1.0.0
+Version: 1.1.0
 Summary: A lightweight Minecraft client for querying the status data of a Minecraft server.
 Author-email: Sch8ill <noreply@noreply.com>
 Project-URL: Bug Tracker, https://github.com/Sch8ill/MCClient-lib/issues
 Project-URL: Homepage, https://github.com/Sch8ill/MCClient-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mcclient-lib-1.0.0/README.md` & `mcclient-lib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/mcclient/address.py` & `mcclient-lib-1.1.0/mcclient/address.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import ipaddress
 
 import dns.resolver
 
+MINECRAFT_SRV_PREFIX = "_minecraft._tcp."
 
 class Address:
     addr: str
-    proto: str
     is_ip: bool
 
-    def __init__(self, addr: str, proto: str = "tcp"):
+    def __init__(self, addr: str):
         self.addr = addr
-        self.proto = proto
         self.is_ip = self._ip_check(self.addr)
 
     def get_host(self, srv: bool = True) -> tuple[str, int]:
         if self.is_ip:
             return self.addr, -1
 
         else:
             return self._resolve_hostname(self.addr, srv)
 
     def _resolve_hostname(self, hostname: str, srv: bool) -> tuple[str, int]:
         host = self._resolve_a_record(hostname)
         if srv:
             try:
-                srv_record = self._mc_srv_lookup(hostname, self.proto)
+                srv_record = self._mc_srv_lookup(hostname)
                 return host, srv_record[1]
 
             except Exception:
                 pass
 
         return host, -1  # -1 = no srv port
 
     @staticmethod
-    def _mc_srv_lookup(hostname: str, proto: str) -> tuple[str, int]:
-        srv_prefix = f"_minecraft._{proto}."
-        # only use the first srv record returned
-        srv_record = dns.resolver.resolve(srv_prefix + hostname, "SRV")[0]
+    def _mc_srv_lookup(hostname: str) -> tuple[str, int]:
+        srv_record = dns.resolver.resolve(MINECRAFT_SRV_PREFIX + hostname, "SRV")[0]
         host = str(srv_record.target).rstrip(".")
         port = int(srv_record.port)
         return host, port
 
     @staticmethod
     def _resolve_a_record(hostname: str) -> str:
         record = dns.resolver.resolve(hostname, "A")[0]
```

### Comparing `mcclient-lib-1.0.0/mcclient/base_client.py` & `mcclient-lib-1.1.0/mcclient/base_client.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/mcclient/bedrock_slp.py` & `mcclient-lib-1.1.0/mcclient/bedrock_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,24 @@
 
 class BedrockSLPClient:
     host: str
     port: int
     hostname: str
     sock: socket.socket
 
-    def __init__(self, host: str, port: int = DEFAULT_BEDROCK_PORT, timeout: int = DEFAULT_TIMEOUT, srv: bool = True):
+    def __init__(self, host: str, port: int = DEFAULT_BEDROCK_PORT, timeout: int = DEFAULT_TIMEOUT):
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.port = port
+        self.hostname = host
         self.sock.settimeout(timeout)
-        self.get_host(host, port, srv)
+        self.get_host(host)
 
-    def get_host(self, hostname: str, port: int, srv: bool) -> None:
+    def get_host(self, hostname: str) -> None:
         addr = Address(hostname)
-        self.host, srv_port = addr.get_host(srv)
-        self.hostname = hostname
-        if srv_port == -1:
-            self.port = port
-
-        else:
-            self.port = srv_port
+        self.host, _ = addr.get_host(False)
 
     def get_status(self) -> BedrockResponse:
         raw_res = self._request_status()
         res = self._parse_res(raw_res)
         return BedrockResponse(self.hostname, self.port, res)
 
     def _request_status(self) -> bytes:
```

### Comparing `mcclient-lib-1.0.0/mcclient/encoding/packet.py` & `mcclient-lib-1.1.0/mcclient/encoding/packet.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/mcclient/encoding/varint.py` & `mcclient-lib-1.1.0/mcclient/encoding/varint.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/mcclient/query_client.py` & `mcclient-lib-1.1.0/mcclient/query_client.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/mcclient/response.py` & `mcclient-lib-1.1.0/mcclient/response.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/mcclient/slp.py` & `mcclient-lib-1.1.0/mcclient/slp.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/mcclient_lib.egg-info/PKG-INFO` & `mcclient-lib-1.1.0/mcclient_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcclient-lib
-Version: 1.0.0
+Version: 1.1.0
 Summary: A lightweight Minecraft client for querying the status data of a Minecraft server.
 Author-email: Sch8ill <noreply@noreply.com>
 Project-URL: Bug Tracker, https://github.com/Sch8ill/MCClient-lib/issues
 Project-URL: Homepage, https://github.com/Sch8ill/MCClient-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mcclient-lib-1.0.0/mcclient_lib.egg-info/SOURCES.txt` & `mcclient-lib-1.1.0/mcclient_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 mcclient/__init__.py
 mcclient/address.py
 mcclient/base_client.py
-mcclient/bedrock_slp.py
+mcclient/bedrock_client.py
 mcclient/query_client.py
 mcclient/response.py
 mcclient/slp.py
 mcclient/encoding/__init__.py
 mcclient/encoding/packet.py
 mcclient/encoding/varint.py
 mcclient_lib.egg-info/PKG-INFO
```

### Comparing `mcclient-lib-1.0.0/pyproject.toml` & `mcclient-lib-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dependencies = [
   "dnspython<2.4.0,>=2.2.1",
 ]
 description = "A lightweight Minecraft client for querying the status data of a Minecraft server."
 name = "mcclient-lib"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.0.0"
+version = "1.1.0"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/Sch8ill/MCClient-lib/issues"
 "Homepage" = "https://github.com/Sch8ill/MCClient-lib"
 
 [tool.pytest.ini_options]
 addopts = "--cov=mcclient --ignore=examples"
```

### Comparing `mcclient-lib-1.0.0/tests/test_bedrock.py` & `mcclient-lib-1.1.0/tests/test_bedrock.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/tests/test_encoding.py` & `mcclient-lib-1.1.0/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/tests/test_formatting_removal.py` & `mcclient-lib-1.1.0/tests/test_formatting_removal.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/tests/test_legacy_slp.py` & `mcclient-lib-1.1.0/tests/test_legacy_slp.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/tests/test_query.py` & `mcclient-lib-1.1.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-1.0.0/tests/test_slp.py` & `mcclient-lib-1.1.0/tests/test_slp.py`

 * *Files identical despite different names*

