# Comparing `tmp/voir-0.2.5.tar.gz` & `tmp/voir-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voir-0.2.5.tar", max compression
+gzip compressed data, was "voir-0.2.6.tar", max compression
```

## Comparing `voir-0.2.5.tar` & `voir-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0      803 2023-04-01 02:24:23.438577 voir-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      139 2023-03-23 16:47:14.434366 voir-0.2.5/voir/__init__.py
--rw-r--r--   0        0        0       61 2023-03-20 20:01:11.843872 voir-0.2.5/voir/__main__.py
--rw-r--r--   0        0        0     7819 2023-03-23 16:47:14.434629 voir-0.2.5/voir/argparse_ext.py
--rw-r--r--   0        0        0      759 2023-03-23 16:47:14.434905 voir-0.2.5/voir/cli.py
--rw-r--r--   0        0        0     1809 2023-03-25 15:52:21.103341 voir-0.2.5/voir/helpers.py
--rw-r--r--   0        0        0      399 2023-03-23 16:47:14.435425 voir-0.2.5/voir/instruments/__init__.py
--rw-r--r--   0        0        0     3292 2023-03-23 16:47:14.435688 voir-0.2.5/voir/instruments/dash.py
--rw-r--r--   0        0        0     6163 2023-03-28 03:32:19.138921 voir-0.2.5/voir/instruments/gpu.py
--rw-r--r--   0        0        0      884 2023-03-23 16:47:14.436583 voir-0.2.5/voir/instruments/log.py
--rw-r--r--   0        0        0      818 2023-04-01 02:22:45.030632 voir-0.2.5/voir/instruments/manage.py
--rw-r--r--   0        0        0     5981 2023-03-25 16:19:36.879569 voir-0.2.5/voir/instruments/metric.py
--rw-r--r--   0        0        0      382 2023-03-28 03:32:37.110995 voir-0.2.5/voir/instruments/utils.py
--rw-r--r--   0        0        0     6334 2023-03-23 16:47:14.437785 voir-0.2.5/voir/overseer.py
--rw-r--r--   0        0        0     9970 2023-03-23 16:47:14.438176 voir-0.2.5/voir/phase.py
--rw-r--r--   0        0        0     6183 2023-03-23 16:47:14.438522 voir-0.2.5/voir/proc.py
--rw-r--r--   0        0        0     1667 2023-03-23 16:47:14.438784 voir-0.2.5/voir/run.py
--rw-r--r--   0        0        0     1306 2023-03-23 16:47:14.439124 voir-0.2.5/voir/scriptutils.py
--rw-r--r--   0        0        0     3060 2023-03-23 16:47:14.439374 voir-0.2.5/voir/smuggle.py
--rw-r--r--   0        0        0     1720 2023-03-23 16:47:14.439677 voir-0.2.5/voir/tools.py
--rw-r--r--   0        0        0       18 2023-04-01 02:24:23.464813 voir-0.2.5/voir/version.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 voir-0.2.5/setup.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 voir-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      803 2023-05-02 17:56:23.440533 voir-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-03-23 16:47:14.434366 voir-0.2.6/voir/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-20 20:01:11.843872 voir-0.2.6/voir/__main__.py
+-rw-r--r--   0        0        0     7819 2023-03-23 16:47:14.434629 voir-0.2.6/voir/argparse_ext.py
+-rw-r--r--   0        0        0      759 2023-03-23 16:47:14.434905 voir-0.2.6/voir/cli.py
+-rw-r--r--   0        0        0      107 2023-05-02 17:55:30.856401 voir-0.2.6/voir/errors.py
+-rw-r--r--   0        0        0     1809 2023-03-25 15:52:21.103341 voir-0.2.6/voir/helpers.py
+-rw-r--r--   0        0        0      399 2023-03-23 16:47:14.435425 voir-0.2.6/voir/instruments/__init__.py
+-rw-r--r--   0        0        0     3292 2023-03-23 16:47:14.435688 voir-0.2.6/voir/instruments/dash.py
+-rw-r--r--   0        0        0     3609 2023-05-02 17:55:30.856567 voir-0.2.6/voir/instruments/gpu/__init__.py
+-rw-r--r--   0        0        0     2244 2023-05-02 17:55:30.856670 voir-0.2.6/voir/instruments/gpu/cuda.py
+-rw-r--r--   0        0        0     5854 2023-05-02 17:55:30.856783 voir-0.2.6/voir/instruments/gpu/rocm.py
+-rw-r--r--   0        0        0      884 2023-03-23 16:47:14.436583 voir-0.2.6/voir/instruments/log.py
+-rw-r--r--   0        0        0      818 2023-04-01 02:22:45.030632 voir-0.2.6/voir/instruments/manage.py
+-rw-r--r--   0        0        0     5981 2023-03-25 16:19:36.879569 voir-0.2.6/voir/instruments/metric.py
+-rw-r--r--   0        0        0      382 2023-03-28 03:32:37.110995 voir-0.2.6/voir/instruments/utils.py
+-rw-r--r--   0        0        0     6334 2023-03-23 16:47:14.437785 voir-0.2.6/voir/overseer.py
+-rw-r--r--   0        0        0     9968 2023-05-02 17:55:30.857303 voir-0.2.6/voir/phase.py
+-rw-r--r--   0        0        0     6183 2023-05-02 17:53:58.153830 voir-0.2.6/voir/proc.py
+-rw-r--r--   0        0        0     1667 2023-03-23 16:47:14.438784 voir-0.2.6/voir/run.py
+-rw-r--r--   0        0        0     1306 2023-03-23 16:47:14.439124 voir-0.2.6/voir/scriptutils.py
+-rw-r--r--   0        0        0     3060 2023-03-23 16:47:14.439374 voir-0.2.6/voir/smuggle.py
+-rw-r--r--   0        0        0     1720 2023-03-23 16:47:14.439677 voir-0.2.6/voir/tools.py
+-rw-r--r--   0        0        0       18 2023-05-02 17:56:23.466397 voir-0.2.6/voir/version.py
+-rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 voir-0.2.6/setup.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 voir-0.2.6/PKG-INFO
```

### Comparing `voir-0.2.5/pyproject.toml` & `voir-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voir"
-version = "0.2.5"
+version = "0.2.6"
 description = "Instrument, extend and visualize your programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ptera = "^1.4.1"
```

### Comparing `voir-0.2.5/voir/argparse_ext.py` & `voir-0.2.6/voir/argparse_ext.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/cli.py` & `voir-0.2.6/voir/cli.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/helpers.py` & `voir-0.2.6/voir/helpers.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/instruments/dash.py` & `voir-0.2.6/voir/instruments/dash.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/instruments/gpu.py` & `voir-0.2.6/voir/instruments/gpu/rocm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,232 +1,216 @@
-import json
 import os
-import shutil
-import subprocess
-import sys
-import time
-from threading import Thread
-
-from ..tools import instrument_definition
-from .utils import Monitor as Monitor2
-
-nvml_available = None
-
-
-def nvlm_init():
-    global nvml_available
-
-    if nvml_available is None:
-        from pynvml import nvmlInit
-        from pynvml.nvml import (
-            NVMLError_DriverNotLoaded,
-            NVMLError_LibraryNotFound,
-        )
 
-        nvml_available = False
-        try:
-            nvmlInit()
-            nvml_available = True
-        except NVMLError_LibraryNotFound:
-            pass
-        except NVMLError_DriverNotLoaded:
-            pass
-
-    return nvml_available
-
-
-def get_cuda_info():
-    from pynvml.smi import nvidia_smi
-
-    nvml_available = nvlm_init()
-
-    def fix_num(n):
-        if n == "N/A":
-            n = None
-        return n
-
-    def parse_gpu(gpu, gid):
-        mem = gpu["fb_memory_usage"]
-        used = fix_num(mem["used"])
-        total = fix_num(mem["total"])
-        compute = fix_num(gpu["utilization"]["gpu_util"])
-        if compute:
-            compute /= 100
-        return {
-            "device": gid,
-            "product": gpu["product_name"],
-            "memory": {
-                "used": used,
-                "total": total,
-            },
-            "utilization": {
-                "compute": compute,
-                "memory": total and used and (used / total),
-            },
-            "temperature": fix_num(gpu["temperature"]["gpu_temp"]),
-            "power": fix_num(gpu["power_readings"]["power_draw"]),
-            "selection_variable": "CUDA_VISIBLE_DEVICES",
-        }
+from ...errors import NotAvailable
 
-    if not nvml_available:
-        return {}
+IMPORT_ERROR = None
+try:
+    import sys
 
-    nvsmi = nvidia_smi.getInstance()
+    sys.path.append("/opt/rocm/libexec/rocm_smi/")
+    import rsmiBindings as rsmi
 
-    to_query = [
-        "gpu_name",
-        "memory.free",
-        "memory.used",
-        "memory.total",
-        "temperature.gpu",
-        "utilization.gpu",
-        "utilization.memory",
-        "power.draw",
-    ]
-    results = nvsmi.DeviceQuery(",".join(to_query))
-
-    if not results or "gpu" not in results:
-        return {}
-
-    gpus = results["gpu"]
-    if not isinstance(gpus, list):
-        gpus = [gpus]
-
-    return {str(i): parse_gpu(g, i) for i, g in enumerate(gpus)}
-
-
-def _get_info(requires, command, parse_function):
-    if not shutil.which(requires):
-        return None
-    proc_results = subprocess.run(
-        command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
-    )
+except ImportError as err:
+    IMPORT_ERROR = err
+
+
+def rsmi_ret_ok(my_ret, device=None, metric=None, silent=False):
+    """Returns true if RSMI call status is 0 (success)
+
+    If status is not 0, error logs are written to the debug log and false is returned
+
+    @param device: DRM device identifier
+    @param my_ret: Return of RSMI call (rocm_smi_lib API)
+    @param metric: Parameter of GPU currently being analyzed
+    """
+    if my_ret != rsmi.rsmi_status_t.RSMI_STATUS_SUCCESS:
+        err_str = rsmi.c_char_p()
+        rsmi.rocmsmi.rsmi_status_string(my_ret, rsmi.byref(err_str))
+
+        returnString = ""
+        if device is not None:
+            returnString += "%s GPU[%s]:" % (my_ret, device)
+        if metric is not None:
+            returnString += " %s: " % (metric)
+        returnString += "%s\t" % (err_str.value.decode())
+
+        raise RuntimeError(returnString)
+        return False
+    return True
+
+
+def is_driver_initialized():
+    """Returns true if amdgpu is found in the list of initialized modules"""
+    import subprocess
+
+    driverInitialized = ""
     try:
-        return parse_function(json.loads(proc_results.stdout))
-    except json.JSONDecodeError:
-        print(f"There was a problem with {requires}:")
-        print("=" * 80)
-        print(proc_results.stderr, file=sys.stderr)
-        print("=" * 80)
-        return None
-
-
-def get_rocm_info():
-    return _get_info("rocm-smi", "rocm-smi -a --showmeminfo vram --json", parse_rocm)
-
-
-def parse_rocm(info):
-    def parse_gpu(gpu, gid):
-        used = int(gpu["VRAM Total Used Memory (B)"])
-        total = int(gpu["VRAM Total Memory (B)"])
-        return {
-            "device": gid,
-            "product": "ROCm Device",
-            "memory": {
-                "used": used // (1024**2),
-                "total": total // (1024**2),
-            },
-            "utilization": {
-                "compute": float(gpu["GPU use (%)"]) / 100,
-                "memory": used / total,
-            },
-            "temperature": float(gpu["Temperature (Sensor edge) (C)"]),
-            "power": float(gpu["Average Graphics Package Power (W)"]),
-            "selection_variable": "ROCR_VISIBLE_DEVICES",
-        }
+        driverInitialized = str(
+            subprocess.check_output(
+                "cat /sys/module/amdgpu/initstate |grep live", shell=True
+            )
+        )
+    except subprocess.CalledProcessError:
+        pass
+    if len(driverInitialized) > 0:
+        return True
+    return False
 
-    results = {}
-    for k, v in info.items():
-        x, y, cnum = k.partition("card")
-        if x != "" or y != "card":
-            continue
-        results[cnum] = parse_gpu(v, cnum)
-
-    return results
-
-
-def get_gpu_info(arch=None):
-    if arch is None:
-        cuda = get_cuda_info()
-        rocm = get_rocm_info()
-        if cuda and rocm:
-            raise Exception(
-                "Milabench found both CUDA and ROCM-compatible GPUs and does not"
-                " know which kind to use. Please set $MILABENCH_GPU_ARCH to 'cuda',"
-                " 'rocm' or 'cpu'."
+
+def initialize_rsmi():
+    """initializes rocmsmi if the amdgpu driver is initialized"""
+    # Check if amdgpu is initialized before initializing rsmi
+    if is_driver_initialized() is True:
+        ret_init = rsmi.rocmsmi.rsmi_init(0)
+        if ret_init != 0:
+            raise NotAvailable(
+                "ROCm SMI returned %s (the expected value is 0)", ret_init
             )
-        elif cuda:
-            arch = "cuda"
-            results = cuda
-        elif rocm:
-            arch = "rocm"
-            results = rocm
-        else:
-            arch = "cpu"
-            results = {}
-
-    elif arch == "cuda":
-        results = get_cuda_info()
-    elif arch == "rocm":
-        results = get_rocm_info()
-    elif arch == "cpu":
-        results = {}
     else:
-        raise ValueError(
-            "Could not infer the gpu architecture because both cuda "
-            "and rocm-compatible gpus were found. Please specify "
-            "arch in ('cuda', 'rocm', 'cpu')"
-        )
+        raise NotAvailable("Driver not initialized (amdgpu not found in modules)")
+
+
+def list_devices():
+    """Returns a list of GPU devices"""
+
+    numberOfDevices = rsmi.c_uint32(0)
+    ret = rsmi.rocmsmi.rsmi_num_monitor_devices(rsmi.byref(numberOfDevices))
+
+    if rsmi_ret_ok(ret):
+        deviceList = list(range(numberOfDevices.value))
+        return deviceList
+    else:
+        exit(ret)
+
 
-    return {"arch": arch, "gpus": results}
+def get_gpu_use(device):
+    """Return the current GPU usage as a percentage"""
+    percent = rsmi.c_uint32()
 
+    ret = rsmi.rocmsmi.rsmi_dev_busy_percent_get(device, rsmi.byref(percent))
 
-class Monitor(Thread):
-    # Keeping this class temporarily to avoid a breakage in milabench
+    if rsmi_ret_ok(ret, device, "GPU Utilization "):
+        return percent.value
 
-    def __init__(self, ov, delay, func):
-        super().__init__(daemon=True)
-        self.ov = ov
-        self.stopped = False
-        self.delay = delay
-        self.func = func
+    return -1
 
-    def run(self):
-        while not self.stopped:
-            time.sleep(self.delay)
-            self.func()
 
-    def stop(self):
-        self.stopped = True
+def get_mem_info(device, memType="vram"):
+    """Return the specified memory usage for the specified device
 
+    @param device: DRM device identifier
+    @param type: [vram|vis_vram|gtt] Memory type to return
+    """
+    memType = memType.upper()
+    if memType not in rsmi.memory_type_l:
+        raise RuntimeError("Invalid memory type %s" % (memType))
 
-@instrument_definition
-def gpu_monitor(ov, poll_interval=10, arch=None):
-    yield ov.phases.load_script
+    memoryUse = rsmi.c_uint64()
+    memoryTot = rsmi.c_uint64()
+    memUsed = None
+    memTotal = None
 
-    visible = os.environ.get("CUDA_VISIBLE_DEVICES", None) or os.environ.get(
-        "ROCR_VISIBLE_DEVICES", None
+    ret = rsmi.rocmsmi.rsmi_dev_memory_usage_get(
+        device, rsmi.memory_type_l.index(memType), rsmi.byref(memoryUse)
     )
-    if visible:
-        ours = visible.split(",")
-    else:
-        ours = [str(x) for x in range(100)]
+    if rsmi_ret_ok(ret, device, memType):
+        memUsed = memoryUse.value
+
+    ret = rsmi.rocmsmi.rsmi_dev_memory_total_get(
+        device, rsmi.memory_type_l.index(memType), rsmi.byref(memoryTot)
+    )
+    if rsmi_ret_ok(ret, device, memType + " total"):
+        memTotal = memoryTot.value
+    return (memUsed, memTotal)
+
+
+def get_temp(device, sensor):
+    """Display the current temperature from a given device's sensor
+
+    @param device: DRM device identifier
+    @param sensor: Temperature sensor identifier
+    """
+    temp = rsmi.c_int64(0)
+    metric = rsmi.rsmi_temperature_metric_t.RSMI_TEMP_CURRENT
+    ret = rsmi.rocmsmi.rsmi_dev_temp_metric_get(
+        rsmi.c_uint32(device),
+        rsmi.temp_type_lst.index(sensor),
+        metric,
+        rsmi.byref(temp),
+    )
+    if rsmi_ret_ok(ret, device, sensor, True):
+        return temp.value / 1000
+    return "N/A"
+
+
+def get_power(device):
+    """Return the current power level of a given device
+
+    @param device: DRM device identifier
+    """
+    power = rsmi.c_uint32()
+    ret = rsmi.rocmsmi.rsmi_dev_power_ave_get(device, 0, rsmi.byref(power))
+    if rsmi_ret_ok(ret, device, "power"):
+        return power.value / 1000000
+    return "N/A"
+
+
+def get_product_name(device):
+    series = rsmi.create_string_buffer(256)
+
+    rsmi.rocmsmi.rsmi_dev_name_get(device, series, 256)
+
+    series = series.value.decode()
+
+    return series
+
+
+def is_installed():
+    return IMPORT_ERROR is None
+
+
+def get_arch():
+    return "rocm"
 
-    def monitor():
-        data = {
-            gpu["device"]: {
-                "memory": [gpu["memory"]["used"], gpu["memory"]["total"]],
-                "load": gpu["utilization"]["compute"],
-                "temperature": gpu["temperature"],
-            }
-            for gpu in get_gpu_info(arch)["gpus"].values()
-            if str(gpu["device"]) in ours
+
+def get_visible_devices():
+    return os.environ.get("ROCR_VISIBLE_DEVICES", None)
+
+
+class DeviceSMI:
+    def __init__(self) -> None:
+        if IMPORT_ERROR is not None:
+            raise IMPORT_ERROR
+
+        initialize_rsmi()
+        self.devices = list_devices()
+
+    def get_gpu_info(self, device):
+        util = get_gpu_use(device)
+        used, total = get_mem_info(device)
+        temp = get_temp(device, "edge")
+        power = get_power(device)
+
+        return {
+            "device": device,
+            "product": get_product_name(device),
+            "memory": {
+                "used": used // (1024**2),
+                "total": total // (1024**2),
+            },
+            "utilization": {
+                "compute": float(util) / 100,
+                "memory": used / total,
+            },
+            "temperature": temp,
+            "power": power,
+            "selection_variable": "ROCR_VISIBLE_DEVICES",
         }
-        ov.give(task="main", gpudata=data)
 
-    monitor_thread = Monitor2(poll_interval, monitor)
-    monitor_thread.start()
-    try:
-        yield ov.phases.run_script
-    finally:
-        monitor_thread.stop()
-        monitor()
+    def get_gpus_info(self):
+        gpus = dict()
+        for device in self.devices:
+            gpus[device] = self.get_gpu_info(device)
+        return gpus
+
+    def close(self):
+        pass
```

### Comparing `voir-0.2.5/voir/instruments/log.py` & `voir-0.2.6/voir/instruments/log.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/instruments/manage.py` & `voir-0.2.6/voir/instruments/manage.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/instruments/metric.py` & `voir-0.2.6/voir/instruments/metric.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/overseer.py` & `voir-0.2.6/voir/overseer.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/phase.py` & `voir-0.2.6/voir/phase.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
     def on_overseer_error(self, e):
         pass
 
     def on_stop(self, value):
         self.status = "stopped"
         for entries in self.plan.values():
-            for (_, __, gen, ___) in entries:
+            for _, __, gen, ___ in entries:
                 try:
                     gen.throw(StopProgram(value))
                 except (StopProgram, StopIteration):
                     pass
                 except BaseException as exc:
                     self.on_overseer_error(exc)
                     pass
```

### Comparing `voir-0.2.5/voir/proc.py` & `voir-0.2.6/voir/proc.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/run.py` & `voir-0.2.6/voir/run.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/scriptutils.py` & `voir-0.2.6/voir/scriptutils.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/smuggle.py` & `voir-0.2.6/voir/smuggle.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/voir/tools.py` & `voir-0.2.6/voir/tools.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.5/setup.py` & `voir-0.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['voir', 'voir.instruments']
+['voir', 'voir.instruments', 'voir.instruments.gpu']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['giving>=0.4.2,<0.5.0',
  'omegaconf>=2.3.0,<3.0.0',
@@ -16,15 +16,15 @@
  'rich>=13.3.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['voir = voir.cli:main']}
 
 setup_kwargs = {
     'name': 'voir',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'Instrument, extend and visualize your programs',
     'long_description': 'None',
     'author': 'Olivier Breuleux',
     'author_email': 'breuleux@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `voir-0.2.5/PKG-INFO` & `voir-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voir
-Version: 0.2.5
+Version: 0.2.6
 Summary: Instrument, extend and visualize your programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

