# Comparing `tmp/mtgpu-0.6.202210041316-py3-none-any.whl.zip` & `tmp/mtgpu-0.7.202305021026-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8046 bytes, number of entries: 14
--rw-rw-r--  2.0 unx     2290 b- defN 22-Oct-04 12:51 mt/gpu/__init__.py
--rw-rw-r--  2.0 unx     2717 b- defN 22-Oct-04 13:16 mt/gpu/arch.py
+Zip file size: 8278 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx     2510 b- defN 23-May-02 10:17 mt/gpu/__init__.py
+-rw-rw-r--  2.0 unx     3093 b- defN 23-May-02 10:16 mt/gpu/arch.py
 -rw-rw-r--  2.0 unx     1879 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_amd.py
 -rw-rw-r--  2.0 unx      245 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_cpu.py
 -rw-rw-r--  2.0 unx     1682 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_nvidia.py
 -rw-rw-r--  2.0 unx      462 b- defN 22-Oct-04 12:51 mt/gpu/arch_rpi.py
--rw-rw-r--  2.0 unx     2129 b- defN 22-Oct-04 12:52 mt/gpu/arch_tegra.py
--rw-rw-r--  2.0 unx      396 b- defN 22-Oct-04 13:16 mt/gpu/version.py
--rwxrwxr-x  2.0 unx       87 b- defN 22-Oct-04 13:16 mtgpu-0.6.202210041316.data/scripts/detect_machine
--rw-rw-r--  2.0 unx     1070 b- defN 22-Oct-04 13:16 mtgpu-0.6.202210041316.dist-info/LICENSE
--rw-rw-r--  2.0 unx      399 b- defN 22-Oct-04 13:16 mtgpu-0.6.202210041316.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Oct-04 13:16 mtgpu-0.6.202210041316.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 22-Oct-04 13:16 mtgpu-0.6.202210041316.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1149 b- defN 22-Oct-04 13:16 mtgpu-0.6.202210041316.dist-info/RECORD
-14 files, 14600 bytes uncompressed, 6128 bytes compressed:  58.0%
+-rw-rw-r--  2.0 unx     2358 b- defN 23-May-02 10:26 mt/gpu/arch_tegra.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-02 10:26 mt/gpu/version.py
+-rwxrwxr-x  2.0 unx       87 b- defN 23-May-02 10:27 mtgpu-0.7.202305021026.data/scripts/detect_machine
+-rw-rw-r--  2.0 unx     1070 b- defN 23-May-02 10:27 mtgpu-0.7.202305021026.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      399 b- defN 23-May-02 10:27 mtgpu-0.7.202305021026.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-02 10:27 mtgpu-0.7.202305021026.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-02 10:27 mtgpu-0.7.202305021026.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1149 b- defN 23-May-02 10:27 mtgpu-0.7.202305021026.dist-info/RECORD
+14 files, 15425 bytes uncompressed, 6360 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: mt/gpu/arch_tegra.py
 Comment: 
 
 Filename: mt/gpu/version.py
 Comment: 
 
-Filename: mtgpu-0.6.202210041316.data/scripts/detect_machine
+Filename: mtgpu-0.7.202305021026.data/scripts/detect_machine
 Comment: 
 
-Filename: mtgpu-0.6.202210041316.dist-info/LICENSE
+Filename: mtgpu-0.7.202305021026.dist-info/LICENSE
 Comment: 
 
-Filename: mtgpu-0.6.202210041316.dist-info/METADATA
+Filename: mtgpu-0.7.202305021026.dist-info/METADATA
 Comment: 
 
-Filename: mtgpu-0.6.202210041316.dist-info/WHEEL
+Filename: mtgpu-0.7.202305021026.dist-info/WHEEL
 Comment: 
 
-Filename: mtgpu-0.6.202210041316.dist-info/top_level.txt
+Filename: mtgpu-0.7.202305021026.dist-info/top_level.txt
 Comment: 
 
-Filename: mtgpu-0.6.202210041316.dist-info/RECORD
+Filename: mtgpu-0.7.202305021026.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/gpu/__init__.py

```diff
@@ -1,65 +1,84 @@
 from __future__ import absolute_import, division, print_function
 
 from .version import version as __version__
 from .arch import detect_machine
 
 
-__all__ = ['detect_machine', 'get_mem_info', 'sort_gpu_devices']
+__all__ = ["detect_machine", "get_mem_info", "sort_gpu_devices"]
 
 
 def get_mem_info(print_bars=False):
-    '''Returns a dictionary containing information about detected CPU/GPU devices and their memory usage, or None if the architecture is unknown.
+    """Returns a dictionary containing information about detected CPU/GPU devices and their memory usage, or None if the architecture is unknown.
 
     Parameters
     ----------
     print_bars : bool
         whether or not to print some bars
-    '''
+    """
     arch = detect_machine()
 
-    if arch == 'amd64-cpu':
+    if arch == "amd64-cpu":
         from .arch_amd64_cpu import get_mem_info_impl
+
         res = get_mem_info_impl()
-    elif arch == 'amd64-nvidia':
+    elif arch == "amd64-nvidia":
         from .arch_amd64_nvidia import get_mem_info_impl
-        res =  get_mem_info_impl()
-    elif arch == 'amd64-amd':
+
+        res = get_mem_info_impl()
+    elif arch == "amd64-amd":
         from .arch_amd64_amd import get_mem_info_impl
+
         res = get_mem_info_impl()
-    elif arch in ['arm64-rp3', 'arm64-rp4']:
+    elif arch in ["arm64-rp3", "arm64-rp4"]:
         from .arch_rpi import get_mem_info_impl
+
         res = get_mem_info_impl(arch)
-    elif arch in ['arm64-tx1', 'arm64-tx2', 'arm64-xnx']:
+    elif arch in ["arm64-tx1", "arm64-tx2", "arm64-xnx", "arm64-orin"]:
         from .arch_tegra import get_mem_info_impl
+
         res = get_mem_info_impl(arch)
-    elif arch == 'unknown':
+    elif arch == "unknown":
         res = None
 
     if print_bars and res:
         from tqdm import tqdm
-        MB = 1024*1024
 
-        is_cgpu = res.get('cpu_mem_shared_with_gpu', False)
+        MB = 1024 * 1024
 
-        cpu_desc = 'cpu_gpu' if is_cgpu else 'cpu'
-        cpu_bar = tqdm(desc=cpu_desc, total=res['cpu_mem_total']//MB, initial=res['cpu_mem_used']//MB, unit='MB', bar_format='{l_bar}{bar}|{n_fmt}/{total_fmt} {unit}')
+        is_cgpu = res.get("cpu_mem_shared_with_gpu", False)
+
+        cpu_desc = "cpu_gpu" if is_cgpu else "cpu"
+        cpu_bar = tqdm(
+            desc=cpu_desc,
+            total=res["cpu_mem_total"] // MB,
+            initial=res["cpu_mem_used"] // MB,
+            unit="MB",
+            bar_format="{l_bar}{bar}|{n_fmt}/{total_fmt} {unit}",
+        )
         cpu_bar.display()
         cpu_bar.close()
 
         if not is_cgpu:
-            for i, gpu in enumerate(res['gpus']):
-                gpu_desc = 'gpu {} ({})'.format(i, gpu['name'])
-                gpu_bar = tqdm(desc=gpu_desc, total=gpu['mem_total']//MB, initial=gpu['mem_used']//MB, unit='MB', bar_format='{l_bar}{bar}|{n_fmt}/{total_fmt} {unit}')
+            for i, gpu in enumerate(res["gpus"]):
+                gpu_desc = "gpu {} ({})".format(i, gpu["name"])
+                gpu_bar = tqdm(
+                    desc=gpu_desc,
+                    total=gpu["mem_total"] // MB,
+                    initial=gpu["mem_used"] // MB,
+                    unit="MB",
+                    bar_format="{l_bar}{bar}|{n_fmt}/{total_fmt} {unit}",
+                )
                 gpu_bar.display()
                 gpu_bar.close()
 
     return res
 
 
 def sort_gpu_devices():
-    '''Sorts the GPU devices in decreasing order of free memory. Only effective with CUDA hardare.'''
+    """Sorts the GPU devices in decreasing order of free memory. Only effective with CUDA hardare."""
 
     arch = detect_machine()
-    if arch == 'amd64-nvidia':
+    if arch == "amd64-nvidia":
         from .arch_amd64_nvidia import sort_cuda_devices
+
         return sort_cuda_devices()
```

## mt/gpu/arch.py

```diff
@@ -29,15 +29,40 @@
     - "amd64-amd" : and amd64 PC with AMDGPU card(s)
     """
     machine_type = uname().machine
 
     if machine_type == "aarch64":  # arm64
         tegra_chip_id_filepath = "/sys/module/tegra_fuse/parameters/tegra_chip_id"
 
-        if not _op.exists(tegra_chip_id_filepath):  # not a Tegra? maybe an RPi
+        if _op.exists(tegra_chip_id_filepath):  # Tegra TK1, TX1, TX2 or XNX
+
+            chip_id = _sp.check_output(["cat", tegra_chip_id_filepath]).decode().strip()
+            # We expect TK1 to respond '64', TX1 to respond '32', TX2 to respond '24'.
+            if chip_id == "64":
+                return "arm64-tk1"  # obsolete
+            if chip_id in ["32", "33"]:
+                return "arm64-tx1"
+            if chip_id == "25":
+                return "arm64-xnx"
+            if chip_id != "24":  # need to expand later
+                return "unknown"
+
+            # TX2
+            return "arm64-tx2"  # need to expand later
+
+        soc_id_filepath = "/sys/devices/soc0/soc.id"
+        if _op.exists(soc_id_filepath):  # Orin
+            soc_id = int(open(soc_id_filepath, "rt").read())
+            if soc_id == 35:
+                return "arm64-orin"
+
+            # assume orin for now until further notice
+            return "arm64-orin"
+
+        else:  # maybe an RPi
 
             rpi_model_filepath = "/sys/firmware/devicetree/base/model"
 
             if not _op.exists(rpi_model_filepath):
                 return "unknown"  # unknown aarch64
 
             rpi_model = _sp.check_output(["cat", rpi_model_filepath]).decode().strip()
@@ -49,29 +74,14 @@
                 return "arm64-rp3"
 
             if rpi_model.startswith("NVIDIA Jetson Xavier NX Developer Kit"):
                 return "arm64-xnx"
 
             return "unknown"  # unknown Raspberry Pi model
 
-        # Tegra
-        chip_id = _sp.check_output(["cat", tegra_chip_id_filepath]).decode().strip()
-        # We expect TK1 to respond '64', TX1 to respond '32', TX2 to respond '24'.
-        if chip_id == "64":
-            return "arm64-tk1"  # obsolete
-        if chip_id in ["32", "33"]:
-            return "arm64-tx1"
-        if chip_id == "25":
-            return "arm64-xnx"
-        if chip_id != "24":  # need to expand later
-            return "unknown"
-
-        # TX2
-        return "arm64-tx2"  # need to expand later
-
     if machine_type != "x86_64":
         return "unknown"  # need to expand later
 
     try:
         nvidia_smi = _sp.check_output(["which", "nvidia-smi"]).decode().strip()
         if nvidia_smi:
             return "amd64-nvidia"
```

## mt/gpu/arch_tegra.py

```diff
@@ -29,14 +29,15 @@
     "32.4.2": "4.4",
     "32.4.3": "4.4",
     "32.4.4": "4.4.1",
     "32.5": "4.5",
     "32.5.1": "4.5.1",
     "32.6.1": "4.6",
     "35.1": "5.0.2",
+    "34.0.1": "5.0",
 }
 
 
 def detect_l4t_version_range():
     kernel_version = uname().release
     if kernel_version.startswith("4.4.38"):
         return ["28.2.1", "28.2.1"]
@@ -48,14 +49,16 @@
         return ["31.0.1", "31.1"]
     if kernel_version.startswith("4.9.140"):
         return ["32.1", "32.4.4"]
     if kernel_version.startswith("4.9.201"):
         return ["32.5", "32.5.1"]
     if kernel_version.startswith("4.9.253-tegra"):
         return ["32.6.1"]
+    if kernel_version.startswith("5.10.65-tegra"):
+        return ["34.0.1"]
     if kernel_version.startswith("5.10.104-tegra"):
         return ["35.1"]
     return "unknown"
 
 
 def get_mem_info_impl(arch):
     res = {}
@@ -66,15 +69,19 @@
     res["cpu_mem_total"] = mem_info.total
     res["cpu_mem_shared_with_gpu"] = True
 
     gpu = {}
     gpu["mem_free"] = res["cpu_mem_free"]
     gpu["mem_used"] = res["cpu_mem_used"]
     gpu["mem_total"] = res["cpu_mem_total"]
-    gpu["name"] = arch2gpu.get(arch, "Unknown")
+    if arch == "arm64-orin":
+        name = open("/sys/firmware/devicetree/base/model", "rt").read()
+    else:
+        name = arch2gpu.get(arch, "Unknown")
+    gpu["name"] = name
     res["gpus"] = [gpu]
 
     l4t_version = detect_l4t_version_range()
     res["l4t"] = l4t_version
     if l4t_version != "unknown":
         jetpack_version = [version_l4t_to_jetpack[x] for x in l4t_version]
         res["jetpack"] = jetpack_version
```

## mt/gpu/version.py

```diff
@@ -1,11 +1,11 @@
-VERSION_YEAR = 2022
-VERSION_MONTH = int('10')
-VERSION_DAY = int('04')
-VERSION_HOUR = int('13')
-VERSION_MINUTE = int('16')
+VERSION_YEAR = 2023
+VERSION_MONTH = int('05')
+VERSION_DAY = int('02')
+VERSION_HOUR = int('10')
+VERSION_MINUTE = int('26')
 MAJOR_VERSION = 0
-MINOR_VERSION = 6
-PATCH_VERSION = 202210041316
-version_date = '2022/10/04 13:16'
+MINOR_VERSION = 7
+PATCH_VERSION = 202305021026
+version_date = '2023/05/02 10:26'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtgpu-0.6.202210041316.dist-info/LICENSE` & `mtgpu-0.7.202305021026.dist-info/LICENSE`

 * *Files identical despite different names*

