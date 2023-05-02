# Comparing `tmp/ovtp-1.0.4.3.tar.gz` & `tmp/ovtp-1.0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovtp-1.0.4.3.tar", last modified: Sat Dec  3 02:03:54 2022, max compression
+gzip compressed data, was "ovtp-1.0.5.0.tar", last modified: Tue May  2 18:07:21 2023, max compression
```

## Comparing `ovtp-1.0.4.3.tar` & `ovtp-1.0.5.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-12-03 02:03:54.486305 ovtp-1.0.4.3/
--rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-10-24 22:47:16.000000 ovtp-1.0.4.3/LICENSE.txt
--rw-r--r--   0 jok4r      (501) staff       (20)     6735 2022-12-03 02:03:54.486361 ovtp-1.0.4.3/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)     5420 2022-10-24 22:47:16.000000 ovtp-1.0.4.3/README.md
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-12-03 02:03:54.482848 ovtp-1.0.4.3/ovtp/
--rw-r--r--   0 jok4r      (501) staff       (20)       42 2022-08-01 18:29:36.000000 ovtp-1.0.4.3/ovtp/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)      351 2022-08-01 18:29:19.000000 ovtp-1.0.4.3/ovtp/__main__.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-12-03 02:03:54.484622 ovtp-1.0.4.3/ovtp/client/
--rw-r--r--   0 jok4r      (501) staff       (20)       89 2022-08-01 22:18:27.000000 ovtp-1.0.4.3/ovtp/client/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)      173 2022-08-01 22:18:27.000000 ovtp-1.0.4.3/ovtp/client/config.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1019 2022-08-01 18:29:05.000000 ovtp-1.0.4.3/ovtp/client/main.py
--rwxr-xr-x   0 jok4r      (501) staff       (20)    19359 2022-12-03 02:03:17.000000 ovtp-1.0.4.3/ovtp/client/ovtp_client.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-12-03 02:03:54.485875 ovtp-1.0.4.3/ovtp/server/
--rw-r--r--   0 jok4r      (501) staff       (20)      190 2022-08-01 22:18:27.000000 ovtp-1.0.4.3/ovtp/server/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1116 2022-08-01 22:18:27.000000 ovtp-1.0.4.3/ovtp/server/add_auth_keys.py
--rw-r--r--   0 jok4r      (501) staff       (20)      846 2022-11-20 20:43:32.000000 ovtp-1.0.4.3/ovtp/server/config.py
--rw-r--r--   0 jok4r      (501) staff       (20)      386 2022-08-01 22:18:27.000000 ovtp-1.0.4.3/ovtp/server/keys_conv.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1226 2022-10-24 22:47:16.000000 ovtp-1.0.4.3/ovtp/server/main.py
--rwxr-xr-x   0 jok4r      (501) staff       (20)    21691 2022-11-21 02:21:11.000000 ovtp-1.0.4.3/ovtp/server/ovtp_server.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-12-03 02:03:54.483790 ovtp-1.0.4.3/ovtp.egg-info/
--rw-r--r--   0 jok4r      (501) staff       (20)        2 2022-08-02 02:52:00.000000 ovtp-1.0.4.3/ovtp.egg-info/.gitignore
--rw-r--r--   0 jok4r      (501) staff       (20)     6735 2022-12-03 02:03:54.000000 ovtp-1.0.4.3/ovtp.egg-info/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)      478 2022-12-03 02:03:54.000000 ovtp-1.0.4.3/ovtp.egg-info/SOURCES.txt
--rw-r--r--   0 jok4r      (501) staff       (20)        1 2022-12-03 02:03:54.000000 ovtp-1.0.4.3/ovtp.egg-info/dependency_links.txt
--rw-r--r--   0 jok4r      (501) staff       (20)       42 2022-12-03 02:03:54.000000 ovtp-1.0.4.3/ovtp.egg-info/requires.txt
--rw-r--r--   0 jok4r      (501) staff       (20)        5 2022-12-03 02:03:54.000000 ovtp-1.0.4.3/ovtp.egg-info/top_level.txt
--rw-r--r--   0 jok4r      (501) staff       (20)      411 2022-12-03 02:03:54.486582 ovtp-1.0.4.3/setup.cfg
--rw-r--r--   0 jok4r      (501) staff       (20)       38 2022-07-31 23:53:24.000000 ovtp-1.0.4.3/setup.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.826962 ovtp-1.0.5.0/
+-rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-10-24 22:47:16.000000 ovtp-1.0.5.0/LICENSE.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-02 18:07:21.827014 ovtp-1.0.5.0/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)     5420 2022-10-24 22:47:16.000000 ovtp-1.0.5.0/README.md
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.823017 ovtp-1.0.5.0/ovtp/
+-rw-r--r--   0 jok4r      (501) staff       (20)       42 2022-08-01 18:29:36.000000 ovtp-1.0.5.0/ovtp/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      351 2022-08-01 18:29:19.000000 ovtp-1.0.5.0/ovtp/__main__.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.825005 ovtp-1.0.5.0/ovtp/client/
+-rw-r--r--   0 jok4r      (501) staff       (20)       89 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/client/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      173 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/client/config.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1019 2022-08-01 18:29:05.000000 ovtp-1.0.5.0/ovtp/client/main.py
+-rwxr-xr-x   0 jok4r      (501) staff       (20)    19825 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/client/ovtp_client.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.826519 ovtp-1.0.5.0/ovtp/server/
+-rw-r--r--   0 jok4r      (501) staff       (20)      222 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1116 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/server/add_auth_keys.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      846 2022-11-20 20:43:32.000000 ovtp-1.0.5.0/ovtp/server/config.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.826815 ovtp-1.0.5.0/ovtp/server/func/
+-rw-r--r--   0 jok4r      (501) staff       (20)       32 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/func/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1586 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/func/check_key.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      386 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/server/keys_conv.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1226 2022-10-24 22:47:16.000000 ovtp-1.0.5.0/ovtp/server/main.py
+-rwxr-xr-x   0 jok4r      (501) staff       (20)    21649 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/ovtp_server.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      216 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/saved_key.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.824111 ovtp-1.0.5.0/ovtp.egg-info/
+-rw-r--r--   0 jok4r      (501) staff       (20)        2 2022-08-02 02:52:00.000000 ovtp-1.0.5.0/ovtp.egg-info/.gitignore
+-rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)      562 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/SOURCES.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)        1 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/dependency_links.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)       42 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/requires.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)        5 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/top_level.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)      411 2023-05-02 18:07:21.827233 ovtp-1.0.5.0/setup.cfg
+-rw-r--r--   0 jok4r      (501) staff       (20)       38 2022-07-31 23:53:24.000000 ovtp-1.0.5.0/setup.py
```

### Comparing `ovtp-1.0.4.3/LICENSE.txt` & `ovtp-1.0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.4.3/PKG-INFO` & `ovtp-1.0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovtp
-Version: 1.0.4.3
+Version: 1.0.5.0
 Summary: Over Transfer Protocol
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `ovtp-1.0.4.3/README.md` & `ovtp-1.0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.4.3/ovtp/client/main.py` & `ovtp-1.0.5.0/ovtp/client/main.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.4.3/ovtp/client/ovtp_client.py` & `ovtp-1.0.5.0/ovtp/client/ovtp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import rsa
 import pathlib
 import ovcrypt
 import asyncio
 import oe_common
 import ov_aes_cipher
 import json
+import base64
 from ovtp.client import cfg
 
 
 script_run = True
 
 
 class OvtpClient:
@@ -354,14 +355,25 @@
             return rcv_data
 
     def send_message_sync(self, message, timeout=2, retries=0):
         return self.loop.run_until_complete(
             self.send_message(message, timeout, retries)
         )
 
+    async def send_add_temp_auth_key(self, key: bytes, remote_address: str):
+        await self.check_connection()
+        data = json.dumps({'temp_key': key.decode(), 'remote_address': remote_address}).encode()
+        response = await self.send_data(
+            self.server_address,
+            data=data,
+            data_type='add_tmp_ak'
+        )
+        print(f"Add temp auth key response: {response}")
+        return response
+
     async def send_message(self, message, timeout=2, retries=0):
         await self.check_connection()
         try:
             rcv = await self.send_data(self.server_address, data=message.encode(), timeout=timeout, retries=retries)
         except ConnectionResetError:
             if not retries:
                 raise
@@ -437,15 +449,15 @@
         # rcv_data = await self.reader.read(4096)
         rcv_data = (await self.read_with_prefix(timeout=timeout, retries=retries))[0]
         # print(f'Encoded: {rcv_data}, len: {len(base64.b64decode(rcv_data))}')
         if data_type not in ['public_key', 'auth_req'] and self.server_public_key:
             # print(f'Decrypted: {aes.decrypt(rcv_data)}')
             if len(rcv_data) > 0:
                 rcv_data = self.aes.decrypt(rcv_data)
-                if data_type == 'message' and rcv_data == b'Sign ok':
+                if data_type in ['message', 'add_tmp_ak'] and rcv_data == b'Sign ok':
                     sign_data = rcv_data  # Xz why
                     rcv_data = self.aes.decrypt((await self.read_with_prefix(timeout=timeout, retries=retries))[0])
                 elif rcv_data == b'Sign error':
                     rcv_data = json.dumps({'status': False, 'description': 'Sign error'}).encode()
                 rcv_data = oe_common.fix_block_encoding_errors(rcv_data)
             else:
                 await self.close_connection()
```

### Comparing `ovtp-1.0.4.3/ovtp/server/add_auth_keys.py` & `ovtp-1.0.5.0/ovtp/server/add_auth_keys.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.4.3/ovtp/server/config.py` & `ovtp-1.0.5.0/ovtp/server/config.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.4.3/ovtp/server/main.py` & `ovtp-1.0.5.0/ovtp/server/main.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.4.3/ovtp/server/ovtp_server.py` & `ovtp-1.0.5.0/ovtp/server/ovtp_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,54 +2,28 @@
 import os
 import rsa
 import pathlib
 import ovcrypt
 import asyncio
 import ov_aes_cipher
 import oe_common
-from ovtp.server import cfg, short_key_to_full, get_short_rsa_key
+from datetime import datetime, timedelta
+from ovtp.server import cfg, SavedKey, func
 
 
 class OvtpServer:
     class Handler:
         def __init__(self, server, reader, writer):
             self.server = server
             self.reader = reader
             self.writer = writer
             self.new_message_timeout = 30
             self.aes = None
             self.cr = ovcrypt.OvCrypt()
 
-        def check_key_is_master(self, key):
-            auth_keys_path = os.path.join(cfg['auth_keys_dir'], 'authorized_keys')
-            os.makedirs(cfg['auth_keys_dir'], exist_ok=True)
-            # oe_common.check_create_dir(auth_keys_path)
-            saved_master_keys = []
-            if os.path.isfile(auth_keys_path):
-                with open(auth_keys_path, 'rb') as f:
-                    for line in f:
-                        if self.server.debug:
-                            print(f'found saved rsa key: {line}')
-                        saved_master_keys.append(rsa.PublicKey.load_pkcs1(short_key_to_full(line)))
-            if key not in saved_master_keys:
-                master_keys = self.cr.get_master_keys()
-                for m_key in master_keys:
-                    if m_key not in saved_master_keys:
-                        saved_master_keys.append(m_key)
-                with open(auth_keys_path, 'wb') as f:
-                    f.write(b'\n'.join([get_short_rsa_key(rsa.PublicKey.save_pkcs1(k).replace(b'\n', b'')) for k in
-                                        saved_master_keys]))
-            if key in saved_master_keys:
-                if self.server.debug:
-                    print(f'Key found in master keys: {key}')
-                return True, True
-            if self.server.verbose:
-                print('Key not found in master keys')
-            return False, 'no_key'
-
         @staticmethod
         def unpad_ov_header(s):
             return bytes(s).rstrip(b'\x00')
 
         async def parse_header(self, read_bytes):
             length = int.from_bytes(await asyncio.wait_for(self.reader.read(read_bytes), timeout=30), byteorder='big')
             if length > 0:
@@ -172,28 +146,39 @@
                         # print(f'prefix: {prefix}')
                         pk_data = b''
                         if prefix != b'':
                             msg_len = int(prefix[:-3])
                             # print(f'Receiving {msg_len} bytes')
                             pk_data = await asyncio.wait_for(self.reader.readexactly(msg_len), timeout=5)
                         # print(f'received: {pk_data}')
-                        self.server.saved_keys[address] = self.cr.Key(rsa.PublicKey.load_pkcs1(
-                            pk_data))
+                        self.server.saved_keys[address] = SavedKey(
+                            rsa.PublicKey.load_pkcs1(pk_data),
+                            datetime.now() + timedelta(minutes=5)
+                        )
                         # self.writer.write(rsa.PublicKey.save_pkcs1(self.cr.public_key))
                         await self.write_with_prefix(rsa.PublicKey.save_pkcs1(self.cr.public_key))
                         break
                     elif data_type == b'auth_req':
                         prefix = (await asyncio.wait_for(self.reader.readline(), timeout=5)).rstrip()
                         pk_data = b''
                         if prefix != b'':
                             msg_len = int(prefix[:-3])
                             # print(f'Receiving {msg_len} bytes')
                             pk_data = await asyncio.wait_for(self.reader.readexactly(msg_len), timeout=5)
                         if self.server.debug:
                             print(f'pk_data: {pk_data}')
+                        if address not in self.server.saved_keys:
+                            print(f'Auth attempt from {address} that is not in saved keys')
+                            await self.write_with_prefix(b'Req failed')
+                            break
+                        key = self.server.temp_keys.get(address[0])
+                        if key and key.expire < datetime.now():
+                            print("Key is expired")
+                            await self.write_with_prefix(b'Key is expired')
+                            break
                         v_string = oe_common.get_rnd_string(100).encode()
                         self.server.saved_keys[address].verification_string = v_string
                         # self.writer.write(rsa.encrypt(v_string, self.server.saved_keys[address].key))
                         await self.write_with_prefix(rsa.encrypt(v_string, self.server.saved_keys[address].key))
                         if self.server.debug:
                             print(f'generated string: {v_string}')
                         r = await self.read_with_prefix()
@@ -349,21 +334,33 @@
                     dec_data = oe_common.fix_block_encoding_errors(data)
                     if self.server.debug or self.server.verbose:
                         print('message:', dec_data)
                     status, description = self.server.callback(True, dec_data)
                     d = json.dumps({'status': status, 'description': description}).encode()
                     await self.write_with_prefix(self.aes.encrypt(d))
                     self.new_message_timeout = cfg['new_message_timeout'] * 60
+                elif data_type == b'add_tmp_ak':
+                    data = json.loads((b''.join(data_parts)).decode())
+                    temp_key = data['temp_key'].encode()
+                    remote_address = data['remote_address']
+
+                    self.server.temp_keys[remote_address] = SavedKey(
+                        rsa.PublicKey.load_pkcs1(temp_key),
+                        datetime.now() + timedelta(minutes=5)
+                    )
+                    send_data = json.dumps({'status': 'OK', 'description': 'Temp key added'}).encode()
+                    await self.write_with_prefix(self.aes.encrypt(send_data))
+                    print("Temp key added")
                 elif data_type == b'auth_resp':
                     data = b''.join(data_parts)
                     del data_parts
                     if self.server.debug:
                         print(f'auth resp is: {data}')
                     if data == self.server.saved_keys[address].verification_string:
-                        status, response = self.check_key_is_master(self.server.saved_keys[address].key)
+                        status, response = func.check_key(self, self.server.saved_keys[address], address)
                         if status:
                             # self.writer.write(aes.encrypt('auth successful'.encode()))
                             await self.write_with_prefix(self.aes.encrypt('auth successful'.encode()))
                             self.server.saved_keys[address].auth = True
                         else:
                             if self.server.verbose:
                                 print(f'Auth failed: {response}')
@@ -378,14 +375,15 @@
                 if self.server.debug:
                     print(f'End of packet {address}')
 
     def __init__(self, callback, verbose=None, debug=None):
         self.server = None
         self.callback = callback
         self.saved_keys = {}
+        self.temp_keys = {}
         self.verbose = verbose
         self.debug = debug
 
     async def run_packet_handler(self, reader, writer):
         handler = self.Handler(self, reader, writer)
         await handler.handle_packet()
```

### Comparing `ovtp-1.0.4.3/ovtp.egg-info/PKG-INFO` & `ovtp-1.0.5.0/ovtp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovtp
-Version: 1.0.4.3
+Version: 1.0.5.0
 Summary: Over Transfer Protocol
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

