# Comparing `tmp/mtgpu-0.7.202305021042-py3-none-any.whl.zip` & `tmp/mtgpu-0.7.202305021336-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8290 bytes, number of entries: 14
+Zip file size: 8298 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx     2510 b- defN 23-May-02 10:17 mt/gpu/__init__.py
 -rw-rw-r--  2.0 unx     3093 b- defN 23-May-02 10:39 mt/gpu/arch.py
 -rw-rw-r--  2.0 unx     1879 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_amd.py
 -rw-rw-r--  2.0 unx      245 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_cpu.py
 -rw-rw-r--  2.0 unx     1682 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_nvidia.py
 -rw-rw-r--  2.0 unx      462 b- defN 22-Oct-04 12:51 mt/gpu/arch_rpi.py
--rw-rw-r--  2.0 unx     2392 b- defN 23-May-02 10:42 mt/gpu/arch_tegra.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-02 10:42 mt/gpu/version.py
--rwxrwxr-x  2.0 unx       87 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.data/scripts/detect_machine
--rw-rw-r--  2.0 unx     1070 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/LICENSE
--rw-rw-r--  2.0 unx      399 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1149 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/RECORD
-14 files, 15459 bytes uncompressed, 6372 bytes compressed:  58.8%
+-rw-rw-r--  2.0 unx     2425 b- defN 23-May-02 13:36 mt/gpu/arch_tegra.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-02 13:36 mt/gpu/version.py
+-rwxrwxr-x  2.0 unx       87 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.data/scripts/detect_machine
+-rw-rw-r--  2.0 unx     1070 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      399 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1149 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/RECORD
+14 files, 15492 bytes uncompressed, 6380 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: mt/gpu/arch_tegra.py
 Comment: 
 
 Filename: mt/gpu/version.py
 Comment: 
 
-Filename: mtgpu-0.7.202305021042.data/scripts/detect_machine
+Filename: mtgpu-0.7.202305021336.data/scripts/detect_machine
 Comment: 
 
-Filename: mtgpu-0.7.202305021042.dist-info/LICENSE
+Filename: mtgpu-0.7.202305021336.dist-info/LICENSE
 Comment: 
 
-Filename: mtgpu-0.7.202305021042.dist-info/METADATA
+Filename: mtgpu-0.7.202305021336.dist-info/METADATA
 Comment: 
 
-Filename: mtgpu-0.7.202305021042.dist-info/WHEEL
+Filename: mtgpu-0.7.202305021336.dist-info/WHEEL
 Comment: 
 
-Filename: mtgpu-0.7.202305021042.dist-info/top_level.txt
+Filename: mtgpu-0.7.202305021336.dist-info/top_level.txt
 Comment: 
 
-Filename: mtgpu-0.7.202305021042.dist-info/RECORD
+Filename: mtgpu-0.7.202305021336.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/gpu/arch_tegra.py

```diff
@@ -28,16 +28,17 @@
     "32.3.1": "4.3",
     "32.4.2": "4.4",
     "32.4.3": "4.4",
     "32.4.4": "4.4.1",
     "32.5": "4.5",
     "32.5.1": "4.5.1",
     "32.6.1": "4.6",
-    "35.1": "5.0.2",
     "34.0.1": "5.0",
+    "35.1": "5.0.2",
+    "35.3.1": "5.1.1",
 }
 
 
 def detect_l4t_version_range():
     kernel_version = uname().release
     if kernel_version.startswith("4.4.38"):
         return ["28.2.1", "28.2.1"]
@@ -52,15 +53,15 @@
     if kernel_version.startswith("4.9.201"):
         return ["32.5", "32.5.1"]
     if kernel_version.startswith("4.9.253-tegra"):
         return ["32.6.1"]
     if kernel_version.startswith("5.10.65-tegra"):
         return ["34.0.1"]
     if kernel_version.startswith("5.10.104-tegra"):
-        return ["35.1"]
+        return ["35.1", "35.3.1"]
     return "unknown"
 
 
 def get_mem_info_impl(arch):
     res = {}
 
     mem_info = _pu.virtual_memory()
```

## mt/gpu/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
 VERSION_DAY = int('02')
-VERSION_HOUR = int('10')
-VERSION_MINUTE = int('42')
+VERSION_HOUR = int('13')
+VERSION_MINUTE = int('36')
 MAJOR_VERSION = 0
 MINOR_VERSION = 7
-PATCH_VERSION = 202305021042
-version_date = '2023/05/02 10:42'
+PATCH_VERSION = 202305021336
+version_date = '2023/05/02 13:36'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtgpu-0.7.202305021042.dist-info/LICENSE` & `mtgpu-0.7.202305021336.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtgpu-0.7.202305021042.dist-info/RECORD` & `mtgpu-0.7.202305021336.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 mt/gpu/__init__.py,sha256=v5_zfaqe2WN2TNXqNieWg2UjcjVJ-b0uEt2l2XGm0Ek,2510
 mt/gpu/arch.py,sha256=dfbm41vRf4zX7HLZD3S_QvZtqT50HBe5wBkHG6gxdeQ,3093
 mt/gpu/arch_amd64_amd.py,sha256=tp7rkq9mtXK3_5u2Y93VCtHWnVtbv3uB9q0MIPrpXdg,1879
 mt/gpu/arch_amd64_cpu.py,sha256=wdavcOtmwgj0i6yWcdX1A3hzpwjOUJ1_9Yg3HcPJq6M,245
 mt/gpu/arch_amd64_nvidia.py,sha256=l5bZas2wik1FYFzK3GOyAPPZQ4Jwb9cY0dg4cliTZcQ,1682
 mt/gpu/arch_rpi.py,sha256=FHzifWhV1YijXMSN4PglMKuLD2bcnFOHVSYmWxZDg2g,462
-mt/gpu/arch_tegra.py,sha256=ADj7pXO3vSjUoar9woRXeXuFhqGy7RH8HiYd3zgbNLk,2392
-mt/gpu/version.py,sha256=xgGt7zOHieShhshfmGoOR_hQOyteNjFrDC2bHr_AaPM,396
-mtgpu-0.7.202305021042.data/scripts/detect_machine,sha256=7lX1WIVJNSZqsGpnHwJIp6C2EFWl_Ow74cBNc9uZQ0w,87
-mtgpu-0.7.202305021042.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtgpu-0.7.202305021042.dist-info/METADATA,sha256=JcZ88-3zXQzxCRjxyjaqqbsAiQSpx8uTdTEszHrMOcQ,399
-mtgpu-0.7.202305021042.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtgpu-0.7.202305021042.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtgpu-0.7.202305021042.dist-info/RECORD,,
+mt/gpu/arch_tegra.py,sha256=blQVFk7g5VcqzNNR0MqaIxzNzoJrLnyd0Twjw92RiCs,2425
+mt/gpu/version.py,sha256=i8kLhmp_Y2xtOmM_auOldZWWLOr134qsobwyA9BSdQk,396
+mtgpu-0.7.202305021336.data/scripts/detect_machine,sha256=7lX1WIVJNSZqsGpnHwJIp6C2EFWl_Ow74cBNc9uZQ0w,87
+mtgpu-0.7.202305021336.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtgpu-0.7.202305021336.dist-info/METADATA,sha256=O7n0RQ_AUDxfaIBV5q6JSyKvZ3gsUObpXXMMteMit5s,399
+mtgpu-0.7.202305021336.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtgpu-0.7.202305021336.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtgpu-0.7.202305021336.dist-info/RECORD,,
```

