# Comparing `tmp/koai-1.0.8.6-cp38-cp38-macosx_13_0_arm64.whl.zip` & `tmp/koai-1.0.8.7-cp38-cp38-macosx_13_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 230994 bytes, number of entries: 20
--rw-r--r--  2.0 unx      211 b- defN 23-Mar-01 07:06 koai/__init__.py
+Zip file size: 230989 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      189 b- defN 23-Mar-01 07:35 koai/__init__.py
 -rw-r--r--  2.0 unx       70 b- defN 23-Mar-01 07:06 koai/benchmarks/__init__.py
 -rw-------  2.0 unx     5301 b- defN 23-Mar-01 07:06 koai/benchmarks/benchmarks.json
 -rw-r--r--  2.0 unx     4871 b- defN 23-Mar-01 07:06 koai/benchmarks/evaluation.py
 -rw-r--r--  2.0 unx    12075 b- defN 23-Mar-01 07:06 koai/benchmarks/finetune.py
 -rw-r--r--  2.0 unx    19540 b- defN 23-Mar-01 07:06 koai/benchmarks/finetune_utils.py
 -rw-r--r--  2.0 unx     5619 b- defN 23-Mar-01 07:06 koai/benchmarks/modeling_dp.py
 -rw-r--r--  2.0 unx     4018 b- defN 23-Mar-01 07:06 koai/benchmarks/modeling_re.py
 -rw-r--r--  2.0 unx     1677 b- defN 23-Mar-01 07:06 koai/benchmarks/postprocess.py
 -rw-r--r--  2.0 unx     3244 b- defN 23-Mar-01 07:06 koai/benchmarks/preprocess.py
 -rw-r--r--  2.0 unx     5046 b- defN 23-Mar-01 07:06 koai/benchmarks/trainer_qa.py
 -rw-r--r--  2.0 unx    12943 b- defN 23-Mar-01 07:06 koai/benchmarks/utils_qa.py
 -rw-r--r--  2.0 unx      130 b- defN 23-Mar-01 07:06 koai/utils/__init__.py
 -rw-r--r--  2.0 unx     3287 b- defN 23-Mar-01 07:06 koai/utils/iterable_dataset.py
--rwxr-xr-x  2.0 unx   537898 b- defN 23-Mar-01 07:23 koai/utils/rs_utils.cpython-38-darwin.so
+-rwxr-xr-x  2.0 unx   537898 b- defN 23-Mar-01 07:35 koai/utils/rs_utils.cpython-38-darwin.so
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 07:06 koai/utils/text.py
--rw-r--r--  2.0 unx     4945 b- defN 23-Mar-01 07:23 koai-1.0.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Mar-01 07:23 koai-1.0.8.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-01 07:23 koai-1.0.8.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1652 b- defN 23-Mar-01 07:23 koai-1.0.8.6.dist-info/RECORD
-20 files, 622640 bytes uncompressed, 228308 bytes compressed:  63.3%
+-rw-r--r--  2.0 unx     4945 b- defN 23-Mar-01 07:35 koai-1.0.8.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Mar-01 07:35 koai-1.0.8.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Mar-01 07:35 koai-1.0.8.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1652 b- defN 23-Mar-01 07:35 koai-1.0.8.7.dist-info/RECORD
+20 files, 622618 bytes uncompressed, 228303 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: koai/utils/rs_utils.cpython-38-darwin.so
 Comment: 
 
 Filename: koai/utils/text.py
 Comment: 
 
-Filename: koai-1.0.8.6.dist-info/METADATA
+Filename: koai-1.0.8.7.dist-info/METADATA
 Comment: 
 
-Filename: koai-1.0.8.6.dist-info/WHEEL
+Filename: koai-1.0.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: koai-1.0.8.6.dist-info/top_level.txt
+Filename: koai-1.0.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: koai-1.0.8.6.dist-info/RECORD
+Filename: koai-1.0.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## koai/__init__.py

```diff
@@ -1,7 +1,6 @@
 from . import benchmarks
-from . import models
 from .benchmarks import finetune, TaskInfo
 
 __version__ = "0.0.1.6"
 
 __all__ = ["benchmarks", "finetune", "TaskInfo"]  # more functions will be added soon...
```

## Comparing `koai-1.0.8.6.dist-info/METADATA` & `koai-1.0.8.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koai
-Version: 1.0.8.6
+Version: 1.0.8.7
 Summary: Korean AI Project
 Home-page: https://github.com/hkjeon13/koai
 Author: Eddie
 Author-email: hkjeo13@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `koai-1.0.8.6.dist-info/RECORD` & `koai-1.0.8.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-koai/__init__.py,sha256=XwXaNnoY7CnIyPyTMA53P18a0gjIYBea9uBrlfXSPGo,211
+koai/__init__.py,sha256=2L4conA-HsWVnV148QFh-RMKXfL81LpIl8NC2poz6FQ,189
 koai/benchmarks/__init__.py,sha256=tXSODJrQJzZ-5MZhx9j33q0Bk6m81u4oz-J9ceut8HI,70
 koai/benchmarks/benchmarks.json,sha256=KXfFA3Ds2GZbInXrqSfxMSng5xXCMqQTaT9XFWyo9lA,5301
 koai/benchmarks/evaluation.py,sha256=Ttw93dFAIcFM3XinwtRRz4l6jaQ7YWFIepgEqMA97SM,4871
 koai/benchmarks/finetune.py,sha256=-xQkWjUzs-b9Znjiye8TLs_IIyYzCPpzDfwNe-BHi00,12075
 koai/benchmarks/finetune_utils.py,sha256=0Hxei3Vsqw0stfLlD-MaFtCrqbEMTHjanZ0g3rYLjaY,19540
 koai/benchmarks/modeling_dp.py,sha256=2sK1m3DGEIu7yzpfxtmkeanr4D87PFed3EtSmPjegRA,5619
 koai/benchmarks/modeling_re.py,sha256=QrlmxuvjCwtgmjw8fjj9BGTOp9hZRn3PGBMTXBlOadE,4018
@@ -10,11 +10,11 @@
 koai/benchmarks/preprocess.py,sha256=8lHKq9jpoA2gU8xqp_TRqOVt2NtwLDUIi7gF4afmgXc,3244
 koai/benchmarks/trainer_qa.py,sha256=_of9922Jnaj4vagRn_giBlQ5Nb5NWzEP-7ojUWOTPg4,5046
 koai/benchmarks/utils_qa.py,sha256=mhtLb8JEGm33y98pCTna1gFNcfAmI7XTkqt-3LGOyp4,12943
 koai/utils/__init__.py,sha256=FnoF-QXHEeRRhGG89fwDkyOUJHqfo3ZgWNgd9JOSt-M,130
 koai/utils/iterable_dataset.py,sha256=eG1bPv-ZGA2H-oYuAcdvDWo1mnMvJofyZFyAislSnlM,3287
 koai/utils/rs_utils.cpython-38-darwin.so,sha256=ijd0lbkKFbJIntLP7ZGS1xs9mDt5f8HwNB_tb6H1i68,537898
 koai/utils/text.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-koai-1.0.8.6.dist-info/METADATA,sha256=hUtlGLWQggY5uD1qQl1cR9Rf7dIiFC6XV_jOF3sjxCg,4945
-koai-1.0.8.6.dist-info/WHEEL,sha256=RIgvgIy-UfMD-ojWOlkuaEp8Bs_a_uFRucDjIsS9GDM,108
-koai-1.0.8.6.dist-info/top_level.txt,sha256=aFsnS3NoYOQYbDIlsw0Mrr95espQ0EqQFgM5SosR1Tc,5
-koai-1.0.8.6.dist-info/RECORD,,
+koai-1.0.8.7.dist-info/METADATA,sha256=JrcJf37UEW9i2_GjZqOphtFkN0p-KOULTt5P1fgwra0,4945
+koai-1.0.8.7.dist-info/WHEEL,sha256=RIgvgIy-UfMD-ojWOlkuaEp8Bs_a_uFRucDjIsS9GDM,108
+koai-1.0.8.7.dist-info/top_level.txt,sha256=aFsnS3NoYOQYbDIlsw0Mrr95espQ0EqQFgM5SosR1Tc,5
+koai-1.0.8.7.dist-info/RECORD,,
```

