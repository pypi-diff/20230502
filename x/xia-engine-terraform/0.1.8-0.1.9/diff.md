# Comparing `tmp/xia_engine_terraform-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 221618 bytes, number of entries: 7
--rw-r--r--  2.0 unx      645 b- defN 23-May-01 11:52 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   596992 b- defN 23-May-01 11:55 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 11:55 xia_engine_terraform-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      724 b- defN 23-May-01 11:55 xia_engine_terraform-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 11:55 xia_engine_terraform-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-01 11:55 xia_engine_terraform-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 11:55 xia_engine_terraform-0.1.8.dist-info/RECORD
-7 files, 599279 bytes uncompressed, 220452 bytes compressed:  63.2%
+Zip file size: 222584 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-May-01 20:58 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   600576 b- defN 23-May-01 21:01 xia_engine_terraform/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 21:01 xia_engine_terraform-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      724 b- defN 23-May-01 21:01 xia_engine_terraform-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 21:01 xia_engine_terraform-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-01 21:01 xia_engine_terraform-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 21:01 xia_engine_terraform-0.1.9.dist-info/RECORD
+7 files, 602863 bytes uncompressed, 221418 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform-0.1.8.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.8.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.8.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.8.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.8.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "TerraformEngine", "TerraformConnectParam", "TerraformClient",
     "TerraformLocalEngine", "TerraformLocalConnectParam", "TerraformLocalClient",
     "ScwTerraformLocalEngine", "ScwTerraformLocalConnectParam",
     "TerraformConfigFactory"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_engine_terraform-0.1.8.dist-info/METADATA` & `xia_engine_terraform-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

