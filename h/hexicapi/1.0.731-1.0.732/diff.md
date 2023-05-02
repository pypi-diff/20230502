# Comparing `tmp/hexicapi-1.0.731.tar.gz` & `tmp/hexicapi-1.0.732.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexicapi-1.0.731.tar", last modified: Wed Nov 23 21:37:49 2022, max compression
+gzip compressed data, was "hexicapi-1.0.732.tar", last modified: Tue May  2 21:46:28 2023, max compression
```

## Comparing `hexicapi-1.0.731.tar` & `hexicapi-1.0.732.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-23 21:37:49.155989 hexicapi-1.0.731/
--rw-rw-rw-   0        0        0      360 2022-11-23 21:37:49.154993 hexicapi-1.0.731/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-23 21:37:49.131743 hexicapi-1.0.731/hexicapi/
--rw-rw-rw-   0        0        0      133 2022-02-20 04:22:49.000000 hexicapi-1.0.731/hexicapi/__init__.py
--rw-rw-rw-   0        0        0    12874 2022-11-15 14:39:30.000000 hexicapi-1.0.731/hexicapi/client.py
--rw-rw-rw-   0        0        0      607 2022-11-12 19:37:47.000000 hexicapi-1.0.731/hexicapi/encryption.py
--rw-rw-rw-   0        0        0     4170 2022-11-01 11:41:18.000000 hexicapi-1.0.731/hexicapi/redlogger.py
--rw-rw-rw-   0        0        0     8305 2022-11-22 17:34:54.000000 hexicapi-1.0.731/hexicapi/registrator.py
--rw-rw-rw-   0        0        0      398 2022-07-22 07:54:05.000000 hexicapi-1.0.731/hexicapi/save.py
--rw-rw-rw-   0        0        0    24294 2022-11-23 21:32:22.000000 hexicapi-1.0.731/hexicapi/server.py
--rw-rw-rw-   0        0        0     4300 2022-07-25 21:56:21.000000 hexicapi-1.0.731/hexicapi/socketMessage.py
--rw-rw-rw-   0        0        0      145 2022-11-23 21:34:20.000000 hexicapi-1.0.731/hexicapi/verinfo.py
-drwxrwxrwx   0        0        0        0 2022-11-23 21:37:49.148335 hexicapi-1.0.731/hexicapi.egg-info/
--rw-rw-rw-   0        0        0      360 2022-11-23 21:37:48.000000 hexicapi-1.0.731/hexicapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2022-11-23 21:37:48.000000 hexicapi-1.0.731/hexicapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-23 21:37:48.000000 hexicapi-1.0.731/hexicapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2022-11-23 21:37:48.000000 hexicapi-1.0.731/hexicapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-23 21:37:48.000000 hexicapi-1.0.731/hexicapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-23 21:37:49.156990 hexicapi-1.0.731/setup.cfg
--rw-rw-rw-   0        0        0      657 2022-11-23 21:37:37.000000 hexicapi-1.0.731/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:46:28.079982 hexicapi-1.0.732/
+-rw-rw-rw-   0        0        0      360 2023-05-02 21:46:28.070116 hexicapi-1.0.732/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 21:46:28.031237 hexicapi-1.0.732/hexicapi/
+-rw-rw-rw-   0        0        0      133 2022-02-20 04:22:49.000000 hexicapi-1.0.732/hexicapi/__init__.py
+-rw-rw-rw-   0        0        0    13098 2023-05-02 21:22:58.000000 hexicapi-1.0.732/hexicapi/client.py
+-rw-rw-rw-   0        0        0     1815 2023-05-02 21:43:10.000000 hexicapi-1.0.732/hexicapi/connectors.py
+-rw-rw-rw-   0        0        0      607 2022-11-12 19:37:47.000000 hexicapi-1.0.732/hexicapi/encryption.py
+-rw-rw-rw-   0        0        0     4170 2022-11-01 11:41:18.000000 hexicapi-1.0.732/hexicapi/redlogger.py
+-rw-rw-rw-   0        0        0     8305 2022-11-22 17:34:54.000000 hexicapi-1.0.732/hexicapi/registrator.py
+-rw-rw-rw-   0        0        0      398 2022-07-22 07:54:05.000000 hexicapi-1.0.732/hexicapi/save.py
+-rw-rw-rw-   0        0        0    24313 2023-05-02 20:16:09.000000 hexicapi-1.0.732/hexicapi/server.py
+-rw-rw-rw-   0        0        0     4409 2023-05-02 21:15:42.000000 hexicapi-1.0.732/hexicapi/socketMessage.py
+-rw-rw-rw-   0        0        0      145 2023-05-02 20:10:51.000000 hexicapi-1.0.732/hexicapi/verinfo.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:46:28.065615 hexicapi-1.0.732/hexicapi.egg-info/
+-rw-rw-rw-   0        0        0      360 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:46:28.081009 hexicapi-1.0.732/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-02 20:24:09.000000 hexicapi-1.0.732/setup.py
```

### Comparing `hexicapi-1.0.731/hexicapi/client.py` & `hexicapi-1.0.732/hexicapi/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 import traceback, pickle
+from typing import Type
 
 import colorama
 
 from hexicapi.socketMessage import *
 from hexicapi.encryption import *
 from hexicapi.save import save, load
 from hexicapi.verinfo import __version__
+from hexicapi.connectors import Connector, TCPConnector, AddressException
+
 BUFFER_SIZE = 1024
 FILE_SERVING_SIZE = 32768
 
-ip = "localhost"
-port = 81
+HOST = 'localhost:81'
 debug = False
 
 functions={ # print(list(functions)) - > shows all available functions
     'connecting':None,
     'connection_warning':None,
     'connection_fail':None,
     'connection_success':None,
@@ -221,19 +223,21 @@
 
     def __enter__(self) -> Client:
         return self
 
     def __exit__(self, *exceptions) -> None:
         self.disconnect()
 
-def run(app,username,password='',autoauth=True, silent=False):
-    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+def run(app: str, username: str, password: str = '', autoauth: bool = True, silent: bool = False, connector: Type[Connector] = TCPConnector):
+    s = connector()
     if not silent: calf('connecting', "The client was ran.")
     try:
-        s.connect((ip,port))
+        s.connect(HOST)
+    except AddressException:
+        calf('connection_fail', "Address malformed")
     except:
         calf('connection_fail', "Couldn't make a connection to the provided port and ip.")
         return
     if not silent: calf('connection_success', "Was able to connect to the server port and ip.")
     send_all(s, "clientGetID".encode("utf-8"))
     id_enc = recv_all(s, BUFFER_SIZE, skip=True).decode('utf-8')
     try:
@@ -258,15 +262,15 @@
         enc_public
     )
     enc_private, public_key = generate_keys()
     send_all(CLI(id, s), public_key, skip=True)
     recv_all(CLI(id, s), enc=enc_private)
     if not silent: calf('handshake', "Encryption handshake.")
 
-    cli = Client(ip, port, s, id, enc_private, enc_public, username, app)
+    cli = Client(*s.getsockname(), s, id, enc_private, enc_public, username, app)
 
     if autoauth:
         if not silent: calf('authenticating',"Autoauth was enabled.")
         cli.auth(password=password, silent=silent)
     cli.silent = silent
     return cli
```

### Comparing `hexicapi-1.0.731/hexicapi/encryption.py` & `hexicapi-1.0.732/hexicapi/encryption.py`

 * *Files identical despite different names*

### Comparing `hexicapi-1.0.731/hexicapi/redlogger.py` & `hexicapi-1.0.732/hexicapi/redlogger.py`

 * *Files identical despite different names*

### Comparing `hexicapi-1.0.731/hexicapi/registrator.py` & `hexicapi-1.0.732/hexicapi/registrator.py`

 * *Files identical despite different names*

### Comparing `hexicapi-1.0.731/hexicapi/server.py` & `hexicapi-1.0.732/hexicapi/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,14 +414,15 @@
     global die
     print('==READER : type help==')
     while not die:
         try: inp = input()
         except:
             if log: logg.reader("Detected an interruption.")
             stop()
+            break
         if inp == "ipbans":
             for ip in ipbans:
                 if ip[1]>=10:
                     t=time.time()-ip[2]
                     pre="seconds"
                     if t>60:
                         t=int(t/60)
```

### Comparing `hexicapi-1.0.731/hexicapi/socketMessage.py` & `hexicapi-1.0.732/hexicapi/socketMessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import socket, time
 import traceback
 
+from hexicapi.connectors import Connector
 from hexicapi.verinfo import __version__, __title__, __author__, __license__, __copyright__
 from hexicapi.encryption import *
 working = []
 record = []
 enc_private = None
 enc_public = None
 sock_msg_debug = False
@@ -26,15 +27,15 @@
     now = time.time()
     for item in record:
         if now-item[1] >= 10:
             if item[0] in working: working.remove(item[0])
             else: print(f'TRYING TO REMOVE {item[0]} in {working}')
             record.remove(item)
 def recv_all(client, packet_size=1024, skip=False, enc=None):
-    if isinstance(client, socket.socket):
+    if isinstance(client, Connector) or isinstance(client, socket.socket):
         the_socket = client
         client_id = client.getsockname()
     else:
         the_socket = client.socket
         client_id = client.id
     menc = enc or enc_private
     if sock_msg_debug: print(f"RECV on wait. waiting:{working} record:{record}")
@@ -72,15 +73,15 @@
         ))
         except: pass
     if sock_msg_debug_minimal: print(f"{the_socket.getsockname()[0]} : RECV : >{data}<")
     return data
 class data_not_bytes(Exception):
     pass
 def send_all(client, data, skip=False, enc=None):
-    if isinstance(client, socket.socket):
+    if isinstance(client, Connector) or isinstance(client, socket.socket):
         the_socket = client
         client_id = client.getsockname()
     else:
         the_socket = client.socket
         client_id = client.id
     menc = enc or enc_public
     if sock_msg_debug or sock_msg_debug_minimal: old_data = data
```

