# Comparing `tmp/pyaprilaire-0.6.0b1.tar.gz` & `tmp/pyaprilaire-0.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaprilaire-0.6.0b1.tar", last modified: Wed Apr 26 00:23:50 2023, max compression
+gzip compressed data, was "pyaprilaire-0.6.0b2.tar", last modified: Tue May  2 00:18:26 2023, max compression
```

## Comparing `pyaprilaire-0.6.0b1.tar` & `pyaprilaire-0.6.0b2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.258863 pyaprilaire-0.6.0b1/pyaprilaire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26633 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/socket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/tests/test_socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.690633 pyaprilaire-0.6.0b2/pyaprilaire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/tests/test_socket_client.py
```

### Comparing `pyaprilaire-0.6.0b1/LICENSE` & `pyaprilaire-0.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b1/PKG-INFO` & `pyaprilaire-0.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b1
+Version: 0.6.0b2
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b1/README.md` & `pyaprilaire-0.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b1/pyaprilaire/client.py` & `pyaprilaire-0.6.0b2/pyaprilaire/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,24 +250,28 @@
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 3,
                 data={"dehumidification_setpoint": dehumidification_setpoint},
             )
         )
 
+        await self.read_dehumidification_setpoint()
+
     async def set_humidification_setpoint(self, humidification_setpoint: int):
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 4,
                 data={"humidification_setpoint": humidification_setpoint},
             )
         )
 
+        await self.read_humidification_setpoint()
+
     async def set_fresh_air(self, mode: int, event: int):
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 5,
                 data={"fresh_air_mode": mode, "fresh_air_event": event},
```

### Comparing `pyaprilaire-0.6.0b1/pyaprilaire/const.py` & `pyaprilaire-0.6.0b2/pyaprilaire/const.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b1/pyaprilaire/mock_server.py` & `pyaprilaire-0.6.0b2/pyaprilaire/mock_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -535,43 +535,19 @@
                             )
                         )
                     elif packet.attribute == 3:
                         self.dehumidification_setpoint = packet.data[
                             "dehumidification_setpoint"
                         ]
                         self.dehumidification_status = 2
-
-                        self.packet_queue.put_nowait(
-                            Packet(
-                                Action.COS,
-                                FunctionalDomain.CONTROL,
-                                3,
-                                sequence=self._get_sequence(),
-                                data={
-                                    "dehumidification_setpoint": self.dehumidification_setpoint
-                                },
-                            )
-                        )
                     elif packet.attribute == 4:
                         self.humidification_setpoint = packet.data[
                             "humidification_setpoint"
                         ]
                         self.humidification_status = 2
-
-                        self.packet_queue.put_nowait(
-                            Packet(
-                                Action.COS,
-                                FunctionalDomain.CONTROL,
-                                4,
-                                sequence=self._get_sequence(),
-                                data={
-                                    "humidification_setpoint": self.humidification_setpoint
-                                },
-                            )
-                        )
                     elif packet.attribute == 5:
                         self.fresh_air_mode = packet.data["fresh_air_mode"]
                         self.fresh_air_event = packet.data["fresh_air_event"]
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
```

### Comparing `pyaprilaire-0.6.0b1/pyaprilaire/packet.py` & `pyaprilaire-0.6.0b2/pyaprilaire/packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b1/pyaprilaire/socket_client.py` & `pyaprilaire-0.6.0b2/pyaprilaire/socket_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b1/pyaprilaire.egg-info/PKG-INFO` & `pyaprilaire-0.6.0b2/pyaprilaire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b1
+Version: 0.6.0b2
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b1/pyproject.toml` & `pyaprilaire-0.6.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaprilaire"
-version = "0.6.0b1"
+version = "0.6.0b2"
 readme = "README.md"
 dependencies = [
     "crc >= 4"
 ]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "coverage"]
 
 [tool.bumpver]
-current_version = "0.6.0b1"
+current_version = "0.6.0b2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyaprilaire-0.6.0b1/tests/test_client.py` & `pyaprilaire-0.6.0b2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b1/tests/test_packet.py` & `pyaprilaire-0.6.0b2/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b1/tests/test_socket_client.py` & `pyaprilaire-0.6.0b2/tests/test_socket_client.py`

 * *Files identical despite different names*

