# Comparing `tmp/horde_model_reference-0.0.3-py3-none-any.whl.zip` & `tmp/horde_model_reference-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,33 @@
-Zip file size: 43100 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 18:31 embeddings/hypernetworks/add_hypernetworks_here.txt
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 18:31 embeddings/lora/add_loras_here.txt
--rw-rw-rw-  2.0 fat      880 b- defN 23-May-01 18:31 legacy/README.md
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 18:31 legacy/__init__.py
--rw-rw-rw-  2.0 fat    13833 b- defN 23-May-01 20:04 legacy/add_to_legacy_sd.py
--rw-rw-rw-  2.0 fat     1478 b- defN 23-May-01 18:58 legacy/convert_all_legacy_dbs.py
--rw-rw-rw-  2.0 fat     1573 b- defN 23-May-01 22:40 legacy/download_live_legacy_dbs.py
--rw-rw-rw-  2.0 fat     3332 b- defN 23-May-01 22:51 legacy/validate_sd.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 19:47 legacy/classes/__init__.py
--rw-rw-rw-  2.0 fat    31531 b- defN 23-May-01 22:13 legacy/classes/legacy_converters.py
--rw-rw-rw-  2.0 fat     1953 b- defN 23-May-01 20:35 legacy/classes/raw_legacy_model_database_records.py
--rw-rw-rw-  2.0 fat     4349 b- defN 23-May-01 22:27 legacy/classes/staging_model_database_records.py
--rw-rw-rw-  2.0 fat     1432 b- defN 23-May-01 18:31 showcase/README.md
--rw-rw-rw-  2.0 fat    35184 b- defN 23-May-01 23:16 horde_model_reference-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    44129 b- defN 23-May-01 23:16 horde_model_reference-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 23:16 horde_model_reference-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       27 b- defN 23-May-01 23:16 horde_model_reference-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1598 b- defN 23-May-01 23:16 horde_model_reference-0.0.3.dist-info/RECORD
-18 files, 141391 bytes uncompressed, 40432 bytes compressed:  71.4%
+Zip file size: 90430 bytes, number of entries: 31
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 23:35 horde_model_reference/__init__.py
+-rw-rw-rw-  2.0 fat     1119 b- defN 23-May-01 23:35 horde_model_reference/blip.json
+-rw-rw-rw-  2.0 fat     2543 b- defN 23-May-01 23:35 horde_model_reference/clip.json
+-rw-rw-rw-  2.0 fat      674 b- defN 23-May-01 23:35 horde_model_reference/codeformer.json
+-rw-rw-rw-  2.0 fat    11395 b- defN 23-May-01 23:35 horde_model_reference/controlnet.json
+-rw-rw-rw-  2.0 fat     4228 b- defN 23-May-01 23:35 horde_model_reference/esrgan.json
+-rw-rw-rw-  2.0 fat     1356 b- defN 23-May-01 23:35 horde_model_reference/gfpgan.json
+-rw-rw-rw-  2.0 fat     2229 b- defN 23-May-01 23:35 horde_model_reference/meta_consts.py
+-rw-rw-rw-  2.0 fat     6015 b- defN 23-May-01 23:35 horde_model_reference/model_reference_records.py
+-rw-rw-rw-  2.0 fat     3675 b- defN 23-May-01 23:35 horde_model_reference/path_consts.py
+-rw-rw-rw-  2.0 fat     1327 b- defN 23-May-01 23:35 horde_model_reference/safety_checker.json
+-rw-rw-rw-  2.0 fat   264121 b- defN 23-May-01 23:35 horde_model_reference/stable_diffusion.json
+-rw-rw-rw-  2.0 fat      500 b- defN 23-May-01 23:35 horde_model_reference/util.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 23:35 horde_model_reference/embeddings/hypernetworks/add_hypernetworks_here.txt
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 23:35 horde_model_reference/embeddings/lora/add_loras_here.txt
+-rw-rw-rw-  2.0 fat      880 b- defN 23-May-01 23:35 horde_model_reference/legacy/README.md
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 23:35 horde_model_reference/legacy/__init__.py
+-rw-rw-rw-  2.0 fat    13833 b- defN 23-May-01 23:35 horde_model_reference/legacy/add_to_legacy_sd.py
+-rw-rw-rw-  2.0 fat     1478 b- defN 23-May-01 23:35 horde_model_reference/legacy/convert_all_legacy_dbs.py
+-rw-rw-rw-  2.0 fat     1573 b- defN 23-May-01 23:35 horde_model_reference/legacy/download_live_legacy_dbs.py
+-rw-rw-rw-  2.0 fat     3332 b- defN 23-May-01 23:35 horde_model_reference/legacy/validate_sd.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-01 23:35 horde_model_reference/legacy/classes/__init__.py
+-rw-rw-rw-  2.0 fat    31531 b- defN 23-May-01 23:35 horde_model_reference/legacy/classes/legacy_converters.py
+-rw-rw-rw-  2.0 fat     1953 b- defN 23-May-01 23:35 horde_model_reference/legacy/classes/raw_legacy_model_database_records.py
+-rw-rw-rw-  2.0 fat     4349 b- defN 23-May-01 23:35 horde_model_reference/legacy/classes/staging_model_database_records.py
+-rw-rw-rw-  2.0 fat     1432 b- defN 23-May-01 23:35 horde_model_reference/showcase/README.md
+-rw-rw-rw-  2.0 fat    35184 b- defN 23-May-01 23:36 horde_model_reference-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    44129 b- defN 23-May-01 23:36 horde_model_reference-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 23:36 horde_model_reference-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-May-01 23:36 horde_model_reference-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3091 b- defN 23-May-01 23:36 horde_model_reference-0.0.7.dist-info/RECORD
+31 files, 442061 bytes uncompressed, 85266 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -1,55 +1,94 @@
-Filename: embeddings/hypernetworks/add_hypernetworks_here.txt
+Filename: horde_model_reference/__init__.py
 Comment: 
 
-Filename: embeddings/lora/add_loras_here.txt
+Filename: horde_model_reference/blip.json
 Comment: 
 
-Filename: legacy/README.md
+Filename: horde_model_reference/clip.json
 Comment: 
 
-Filename: legacy/__init__.py
+Filename: horde_model_reference/codeformer.json
 Comment: 
 
-Filename: legacy/add_to_legacy_sd.py
+Filename: horde_model_reference/controlnet.json
 Comment: 
 
-Filename: legacy/convert_all_legacy_dbs.py
+Filename: horde_model_reference/esrgan.json
 Comment: 
 
-Filename: legacy/download_live_legacy_dbs.py
+Filename: horde_model_reference/gfpgan.json
 Comment: 
 
-Filename: legacy/validate_sd.py
+Filename: horde_model_reference/meta_consts.py
 Comment: 
 
-Filename: legacy/classes/__init__.py
+Filename: horde_model_reference/model_reference_records.py
 Comment: 
 
-Filename: legacy/classes/legacy_converters.py
+Filename: horde_model_reference/path_consts.py
 Comment: 
 
-Filename: legacy/classes/raw_legacy_model_database_records.py
+Filename: horde_model_reference/safety_checker.json
 Comment: 
 
-Filename: legacy/classes/staging_model_database_records.py
+Filename: horde_model_reference/stable_diffusion.json
 Comment: 
 
-Filename: showcase/README.md
+Filename: horde_model_reference/util.py
 Comment: 
 
-Filename: horde_model_reference-0.0.3.dist-info/LICENSE
+Filename: horde_model_reference/embeddings/hypernetworks/add_hypernetworks_here.txt
 Comment: 
 
-Filename: horde_model_reference-0.0.3.dist-info/METADATA
+Filename: horde_model_reference/embeddings/lora/add_loras_here.txt
 Comment: 
 
-Filename: horde_model_reference-0.0.3.dist-info/WHEEL
+Filename: horde_model_reference/legacy/README.md
 Comment: 
 
-Filename: horde_model_reference-0.0.3.dist-info/top_level.txt
+Filename: horde_model_reference/legacy/__init__.py
 Comment: 
 
-Filename: horde_model_reference-0.0.3.dist-info/RECORD
+Filename: horde_model_reference/legacy/add_to_legacy_sd.py
+Comment: 
+
+Filename: horde_model_reference/legacy/convert_all_legacy_dbs.py
+Comment: 
+
+Filename: horde_model_reference/legacy/download_live_legacy_dbs.py
+Comment: 
+
+Filename: horde_model_reference/legacy/validate_sd.py
+Comment: 
+
+Filename: horde_model_reference/legacy/classes/__init__.py
+Comment: 
+
+Filename: horde_model_reference/legacy/classes/legacy_converters.py
+Comment: 
+
+Filename: horde_model_reference/legacy/classes/raw_legacy_model_database_records.py
+Comment: 
+
+Filename: horde_model_reference/legacy/classes/staging_model_database_records.py
+Comment: 
+
+Filename: horde_model_reference/showcase/README.md
+Comment: 
+
+Filename: horde_model_reference-0.0.7.dist-info/LICENSE
+Comment: 
+
+Filename: horde_model_reference-0.0.7.dist-info/METADATA
+Comment: 
+
+Filename: horde_model_reference-0.0.7.dist-info/WHEEL
+Comment: 
+
+Filename: horde_model_reference-0.0.7.dist-info/top_level.txt
+Comment: 
+
+Filename: horde_model_reference-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `legacy/README.md` & `horde_model_reference/legacy/README.md`

 * *Files identical despite different names*

## Comparing `legacy/add_to_legacy_sd.py` & `horde_model_reference/legacy/add_to_legacy_sd.py`

 * *Files identical despite different names*

## Comparing `legacy/convert_all_legacy_dbs.py` & `horde_model_reference/legacy/convert_all_legacy_dbs.py`

 * *Files identical despite different names*

## Comparing `legacy/download_live_legacy_dbs.py` & `horde_model_reference/legacy/download_live_legacy_dbs.py`

 * *Files identical despite different names*

## Comparing `legacy/validate_sd.py` & `horde_model_reference/legacy/validate_sd.py`

 * *Files identical despite different names*

## Comparing `legacy/classes/legacy_converters.py` & `horde_model_reference/legacy/classes/legacy_converters.py`

 * *Files identical despite different names*

## Comparing `legacy/classes/raw_legacy_model_database_records.py` & `horde_model_reference/legacy/classes/raw_legacy_model_database_records.py`

 * *Files identical despite different names*

## Comparing `legacy/classes/staging_model_database_records.py` & `horde_model_reference/legacy/classes/staging_model_database_records.py`

 * *Files identical despite different names*

## Comparing `showcase/README.md` & `horde_model_reference/showcase/README.md`

 * *Files identical despite different names*

## Comparing `horde_model_reference-0.0.3.dist-info/LICENSE` & `horde_model_reference-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `horde_model_reference-0.0.3.dist-info/METADATA` & `horde_model_reference-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde-model-reference
-Version: 0.0.3
+Version: 0.0.7
 Summary: A helper library providing a way to work with the lists of diffusion models, utility models, and any other related files required for AI-Horde.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>, Jug <jugdev@proton.me>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -705,15 +705,15 @@
 ## Python library
 This repo is also a python library!
 ### General info
 You can install this module through pip:
 ```
 python -m pip install horde_model_reference
 ```
-This library has a number of python classes which may assist you in working with the model reference. The following paths may be of interest:
+This library has a number of python classes which may assist you in working with the model reference. The following files may be of interest:
 - horde_model_reference\model_reference_records.py
   - Contains pydantic definitions, and some meta information, for all record types.
 - horde_model_reference\meta_consts.py
   - Contains many commonly used strings, enums, and certain useful dict lookups.
 - horde_model_reference\path_consts.py
   - Contains certain potentially useful paths, path constructors and folder/file name information relevant to the package.
 ## Horde Moderators/Support Staff
```

