# Comparing `tmp/spycoprobe-1.0.1.tar.gz` & `tmp/spycoprobe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spycoprobe-1.0.1.tar", last modified: Thu Mar  9 09:16:39 2023, max compression
+gzip compressed data, was "spycoprobe-1.0.2.tar", last modified: Tue May  2 12:17:42 2023, max compression
```

## Comparing `spycoprobe-1.0.1.tar` & `spycoprobe-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 09:16:39.973006 spycoprobe-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-09 09:16:39.973006 spycoprobe-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 09:16:39.973006 spycoprobe-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 09:16:39.973006 spycoprobe-1.0.1/spycoprobe/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/spycoprobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/spycoprobe/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/spycoprobe/intelhex.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/spycoprobe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-09 09:16:27.000000 spycoprobe-1.0.1/spycoprobe/spycoprobe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 09:16:39.973006 spycoprobe-1.0.1/spycoprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-09 09:16:39.000000 spycoprobe-1.0.1/spycoprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-09 09:16:39.000000 spycoprobe-1.0.1/spycoprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 09:16:39.000000 spycoprobe-1.0.1/spycoprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-09 09:16:39.000000 spycoprobe-1.0.1/spycoprobe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-09 09:16:39.000000 spycoprobe-1.0.1/spycoprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-09 09:16:39.000000 spycoprobe-1.0.1/spycoprobe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:42.467054 spycoprobe-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 12:17:42.467054 spycoprobe-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:17:42.467054 spycoprobe-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:42.463054 spycoprobe-1.0.2/spycoprobe/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/spycoprobe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/spycoprobe/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/spycoprobe/intelhex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/spycoprobe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-02 12:17:24.000000 spycoprobe-1.0.2/spycoprobe/spycoprobe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:42.467054 spycoprobe-1.0.2/spycoprobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 12:17:42.000000 spycoprobe-1.0.2/spycoprobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-02 12:17:42.000000 spycoprobe-1.0.2/spycoprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:17:42.000000 spycoprobe-1.0.2/spycoprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 12:17:42.000000 spycoprobe-1.0.2/spycoprobe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 12:17:42.000000 spycoprobe-1.0.2/spycoprobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 12:17:42.000000 spycoprobe-1.0.2/spycoprobe.egg-info/top_level.txt
```

### Comparing `spycoprobe-1.0.1/LICENSE.txt` & `spycoprobe-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spycoprobe-1.0.1/PKG-INFO` & `spycoprobe-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spycoprobe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tool for controlling Spycoprobe SBW debugger
 Author: Kai Geissdoerfer
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Spycoprobe programmer
```

### Comparing `spycoprobe-1.0.1/setup.py` & `spycoprobe-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="spycoprobe",
-    version="1.0.1",
+    version="1.0.2",
     description="Tool for controlling Spycoprobe SBW debugger",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Kai Geissdoerfer",
     packages=["spycoprobe"],
     license="MIT",
     include_package_data=True,
```

### Comparing `spycoprobe-1.0.1/spycoprobe/cli.py` & `spycoprobe-1.0.2/spycoprobe/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from serial.tools import list_ports
 
 from spycoprobe.spycoprobe import SpycoProbe
 from spycoprobe.spycoprobe import INTERFACE_NAMES
 
 from spycoprobe.intelhex import IntelHex16bitReader
 from spycoprobe.protocol import REQUEST_MAX_DATA
+from spycoprobe.protocol import IOSetState
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"], obj={}))
 @click.option(
     "--device",
     "-d",
     type=click.Path(exists=True),
@@ -67,13 +68,43 @@
 @click.pass_context
 def halt(ctx):
     with SpycoProbe(ctx.obj["device"]) as probe:
         probe.start()
         probe.halt()
         probe.stop()
 
+
 @cli.command(short_help="Control target power supply")
 @click.option("--on/--off", required=True)
 @click.pass_context
 def target_power(ctx, on):
     with SpycoProbe(ctx.obj["device"]) as probe:
         probe.target_power(on)
+
+
+@cli.command(short_help="Control GPIO pin")
+@click.option("--pin-no", "-p", type=int, required=True, help="Pin number")
+@click.option(
+    "--state",
+    "-s",
+    type=click.Choice(["high", "1", "low", "0", "input"], case_sensitive=False),
+    required=True,
+    help="Pin state",
+)
+@click.pass_context
+def gpio_set(ctx, pin_no, state):
+    with SpycoProbe(ctx.obj["device"]) as probe:
+        if state in ["high", "1"]:
+            probe.gpio_set(pin_no, IOSetState.IOSET_OUT_HIGH)
+        elif state in ["low", "0"]:
+            probe.gpio_set(pin_no, IOSetState.IOSET_OUT_LOW)
+        else:
+            probe.gpio_set(pin_no, IOSetState.IOSET_IN)
+
+
+@cli.command(short_help="Read GPIO pin")
+@click.option("--pin-no", "-p", type=int, required=True, help="Pin number")
+@click.pass_context
+def gpio_get(ctx, pin_no):
+    with SpycoProbe(ctx.obj["device"]) as probe:
+        state = probe.gpio_get(pin_no)
+        click.echo(state)
```

### Comparing `spycoprobe-1.0.1/spycoprobe/intelhex.py` & `spycoprobe-1.0.2/spycoprobe/intelhex.py`

 * *Files identical despite different names*

### Comparing `spycoprobe-1.0.1/spycoprobe/spycoprobe.py` & `spycoprobe-1.0.2/spycoprobe/spycoprobe.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 import struct
 from typing import Union
 
 from spycoprobe.protocol import ReqType
 from spycoprobe.protocol import ReturnCode
 from spycoprobe.protocol import TargetPowerState
+from spycoprobe.protocol import IOSetState
 
 from spycoprobe.protocol import REQUEST_MAX_DATA
 from spycoprobe.protocol import RESPONSE_MAX_DATA
 
 
 INTERFACE_NAMES = ["Spycoprobe SBW", "Rioteeprobe SBW"]
 
@@ -72,14 +73,24 @@
         if state:
             pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_POWER, 1, 0x0, TargetPowerState.TARGET_POWER_ON)
         else:
             pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_POWER, 1, 0x0, TargetPowerState.TARGET_POWER_OFF)
         self._ser.write(pkt)
         self._recv_rsp()
 
+    def gpio_set(self, pin_no, state: IOSetState):
+        pkt = struct.pack(f"=BBI2H", ReqType.SBW_REQ_IOSET, 2, 0x0, pin_no, state)
+        self._ser.write(pkt)
+        self._recv_rsp()
+
+    def gpio_get(self, pin_no) -> bool:
+        pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_IOGET, 2, 0x0, pin_no)
+        self._ser.write(pkt)
+        return bool(self._recv_rsp()[0])
+
     def write_mem(self, addr, data: Union[int, np.ndarray]):
         """Write a word to NVM or RAM."""
         if hasattr(data, "__len__"):
             if len(data) > REQUEST_MAX_DATA:
                 raise ValueError("Data length exceeds request packet size")
             pkt = struct.pack(f"=BBI{len(data)}H", ReqType.SBW_REQ_WRITE, len(data), addr, *data)
         else:
```

### Comparing `spycoprobe-1.0.1/spycoprobe.egg-info/PKG-INFO` & `spycoprobe-1.0.2/spycoprobe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spycoprobe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tool for controlling Spycoprobe SBW debugger
 Author: Kai Geissdoerfer
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Spycoprobe programmer
```

