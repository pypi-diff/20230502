# Comparing `tmp/mtgpu-0.7.202305021039-py3-none-any.whl.zip` & `tmp/mtgpu-0.7.202305021042-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8275 bytes, number of entries: 14
+Zip file size: 8290 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx     2510 b- defN 23-May-02 10:17 mt/gpu/__init__.py
 -rw-rw-r--  2.0 unx     3093 b- defN 23-May-02 10:39 mt/gpu/arch.py
 -rw-rw-r--  2.0 unx     1879 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_amd.py
 -rw-rw-r--  2.0 unx      245 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_cpu.py
 -rw-rw-r--  2.0 unx     1682 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_nvidia.py
 -rw-rw-r--  2.0 unx      462 b- defN 22-Oct-04 12:51 mt/gpu/arch_rpi.py
--rw-rw-r--  2.0 unx     2358 b- defN 23-May-02 10:26 mt/gpu/arch_tegra.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-02 10:39 mt/gpu/version.py
--rwxrwxr-x  2.0 unx       87 b- defN 23-May-02 10:39 mtgpu-0.7.202305021039.data/scripts/detect_machine
--rw-rw-r--  2.0 unx     1070 b- defN 23-May-02 10:39 mtgpu-0.7.202305021039.dist-info/LICENSE
--rw-rw-r--  2.0 unx      399 b- defN 23-May-02 10:39 mtgpu-0.7.202305021039.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 10:39 mtgpu-0.7.202305021039.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-02 10:39 mtgpu-0.7.202305021039.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1149 b- defN 23-May-02 10:39 mtgpu-0.7.202305021039.dist-info/RECORD
-14 files, 15425 bytes uncompressed, 6357 bytes compressed:  58.8%
+-rw-rw-r--  2.0 unx     2392 b- defN 23-May-02 10:42 mt/gpu/arch_tegra.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-02 10:42 mt/gpu/version.py
+-rwxrwxr-x  2.0 unx       87 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.data/scripts/detect_machine
+-rw-rw-r--  2.0 unx     1070 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      399 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1149 b- defN 23-May-02 10:43 mtgpu-0.7.202305021042.dist-info/RECORD
+14 files, 15459 bytes uncompressed, 6372 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: mt/gpu/arch_tegra.py
 Comment: 
 
 Filename: mt/gpu/version.py
 Comment: 
 
-Filename: mtgpu-0.7.202305021039.data/scripts/detect_machine
+Filename: mtgpu-0.7.202305021042.data/scripts/detect_machine
 Comment: 
 
-Filename: mtgpu-0.7.202305021039.dist-info/LICENSE
+Filename: mtgpu-0.7.202305021042.dist-info/LICENSE
 Comment: 
 
-Filename: mtgpu-0.7.202305021039.dist-info/METADATA
+Filename: mtgpu-0.7.202305021042.dist-info/METADATA
 Comment: 
 
-Filename: mtgpu-0.7.202305021039.dist-info/WHEEL
+Filename: mtgpu-0.7.202305021042.dist-info/WHEEL
 Comment: 
 
-Filename: mtgpu-0.7.202305021039.dist-info/top_level.txt
+Filename: mtgpu-0.7.202305021042.dist-info/top_level.txt
 Comment: 
 
-Filename: mtgpu-0.7.202305021039.dist-info/RECORD
+Filename: mtgpu-0.7.202305021042.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/gpu/arch_tegra.py

```diff
@@ -71,14 +71,15 @@
 
     gpu = {}
     gpu["mem_free"] = res["cpu_mem_free"]
     gpu["mem_used"] = res["cpu_mem_used"]
     gpu["mem_total"] = res["cpu_mem_total"]
     if arch == "arm64-orin":
         name = open("/sys/firmware/devicetree/base/model", "rt").read()
+        name = name.strip(chr(0))
     else:
         name = arch2gpu.get(arch, "Unknown")
     gpu["name"] = name
     res["gpus"] = [gpu]
 
     l4t_version = detect_l4t_version_range()
     res["l4t"] = l4t_version
```

## mt/gpu/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
 VERSION_DAY = int('02')
 VERSION_HOUR = int('10')
-VERSION_MINUTE = int('39')
+VERSION_MINUTE = int('42')
 MAJOR_VERSION = 0
 MINOR_VERSION = 7
-PATCH_VERSION = 202305021039
-version_date = '2023/05/02 10:39'
+PATCH_VERSION = 202305021042
+version_date = '2023/05/02 10:42'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtgpu-0.7.202305021039.dist-info/LICENSE` & `mtgpu-0.7.202305021042.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtgpu-0.7.202305021039.dist-info/RECORD` & `mtgpu-0.7.202305021042.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 mt/gpu/__init__.py,sha256=v5_zfaqe2WN2TNXqNieWg2UjcjVJ-b0uEt2l2XGm0Ek,2510
 mt/gpu/arch.py,sha256=dfbm41vRf4zX7HLZD3S_QvZtqT50HBe5wBkHG6gxdeQ,3093
 mt/gpu/arch_amd64_amd.py,sha256=tp7rkq9mtXK3_5u2Y93VCtHWnVtbv3uB9q0MIPrpXdg,1879
 mt/gpu/arch_amd64_cpu.py,sha256=wdavcOtmwgj0i6yWcdX1A3hzpwjOUJ1_9Yg3HcPJq6M,245
 mt/gpu/arch_amd64_nvidia.py,sha256=l5bZas2wik1FYFzK3GOyAPPZQ4Jwb9cY0dg4cliTZcQ,1682
 mt/gpu/arch_rpi.py,sha256=FHzifWhV1YijXMSN4PglMKuLD2bcnFOHVSYmWxZDg2g,462
-mt/gpu/arch_tegra.py,sha256=UyU5wOk4WVsOGQ_hREIKSu-oJrZBU90PctDgwNl_sqE,2358
-mt/gpu/version.py,sha256=Nb8geotoH-6YnTlprjyjVtXccD6IJ-IST5TSMDe0ASM,396
-mtgpu-0.7.202305021039.data/scripts/detect_machine,sha256=7lX1WIVJNSZqsGpnHwJIp6C2EFWl_Ow74cBNc9uZQ0w,87
-mtgpu-0.7.202305021039.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtgpu-0.7.202305021039.dist-info/METADATA,sha256=XSySNzMjz1PnjoFFIawW82ZUzbLaHbvyRUGoGCJH74Q,399
-mtgpu-0.7.202305021039.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtgpu-0.7.202305021039.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtgpu-0.7.202305021039.dist-info/RECORD,,
+mt/gpu/arch_tegra.py,sha256=ADj7pXO3vSjUoar9woRXeXuFhqGy7RH8HiYd3zgbNLk,2392
+mt/gpu/version.py,sha256=xgGt7zOHieShhshfmGoOR_hQOyteNjFrDC2bHr_AaPM,396
+mtgpu-0.7.202305021042.data/scripts/detect_machine,sha256=7lX1WIVJNSZqsGpnHwJIp6C2EFWl_Ow74cBNc9uZQ0w,87
+mtgpu-0.7.202305021042.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtgpu-0.7.202305021042.dist-info/METADATA,sha256=JcZ88-3zXQzxCRjxyjaqqbsAiQSpx8uTdTEszHrMOcQ,399
+mtgpu-0.7.202305021042.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtgpu-0.7.202305021042.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtgpu-0.7.202305021042.dist-info/RECORD,,
```

