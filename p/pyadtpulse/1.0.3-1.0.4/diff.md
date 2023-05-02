# Comparing `tmp/pyadtpulse-1.0.3-py3-none-any.whl.zip` & `tmp/pyadtpulse-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 21418 bytes, number of entries: 11
 -rw-r--r--  2.0 unx    34446 b- defN 23-Apr-29 06:07 pyadtpulse/__init__.py
 -rw-r--r--  2.0 unx     1609 b- defN 23-Mar-28 16:07 pyadtpulse/const.py
 -rw-r--r--  2.0 unx    24957 b- defN 23-Apr-29 06:07 pyadtpulse/site.py
 -rw-r--r--  2.0 unx     4803 b- defN 23-Mar-28 16:07 pyadtpulse/util.py
 -rw-r--r--  2.0 unx     5847 b- defN 23-Apr-29 06:07 pyadtpulse/zones.py
--rw-r--r--  2.0 unx      581 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3680 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 03:34 pyadtpulse-1.0.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      875 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/RECORD
+-rw-r--r--  2.0 unx      581 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3680 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 03:34 pyadtpulse-1.0.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      875 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/RECORD
 11 files, 76902 bytes uncompressed, 19944 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pyadtpulse/util.py
 Comment: 
 
 Filename: pyadtpulse/zones.py
 Comment: 
 
-Filename: pyadtpulse-1.0.3.dist-info/LICENSE.md
+Filename: pyadtpulse-1.0.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyadtpulse-1.0.3.dist-info/METADATA
+Filename: pyadtpulse-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pyadtpulse-1.0.3.dist-info/WHEEL
+Filename: pyadtpulse-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyadtpulse-1.0.3.dist-info/top_level.txt
+Filename: pyadtpulse-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyadtpulse-1.0.3.dist-info/zip-safe
+Filename: pyadtpulse-1.0.4.dist-info/zip-safe
 Comment: 
 
-Filename: pyadtpulse-1.0.3.dist-info/RECORD
+Filename: pyadtpulse-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyadtpulse-1.0.3.dist-info/LICENSE.md` & `pyadtpulse-1.0.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyadtpulse-1.0.3.dist-info/METADATA` & `pyadtpulse-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyadtpulse
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python interface for ADT Pulse security systems
 Home-page: https://github.com/rsnodgrass/pyadtpulse
 Author: 
 Author-email: 
 License: Apache Software License
 Keywords: security system,adt,home automation,security alarm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: aiohttp (>=3.8.1)
-Requires-Dist: uvloop (==0.16.0)
+Requires-Dist: uvloop (>=0.17.0)
 
 # pyadtpulse - Python interface for ADT Pulse
 
 Python client interface to the ADT Pulse security system.
 
 [![PyPi](https://img.shields.io/pypi/v/pyadtpulse.svg)](https://pypi.python.org/pypi/pyadtpulse)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

## Comparing `pyadtpulse-1.0.3.dist-info/RECORD` & `pyadtpulse-1.0.4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pyadtpulse/__init__.py,sha256=b5xr7SUiaZV2a6F7LpnKHgwbjpRU-3-_eHfEqYAXfGE,34446
 pyadtpulse/const.py,sha256=q3xJ93olyh9pNKvywARCwsu9qnr-E8O3SkD8Z4BEGBw,1609
 pyadtpulse/site.py,sha256=L5fb9tXag8JQPPNVSOr-PNTYy5pJPVtdSPV2lmqnYoU,24957
 pyadtpulse/util.py,sha256=aTsrbEWoYkaAxnN0pU_ZoQ6eqyWTx-4_Ukihq8wwb88,4803
 pyadtpulse/zones.py,sha256=6EADUsVXp0n-0WEEhjHzBoOd8bPZcqtl2TZvEfikaZM,5847
-pyadtpulse-1.0.3.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
-pyadtpulse-1.0.3.dist-info/METADATA,sha256=gdZjc3eEq-HUUDNxyn9iHqEcd8iNdTWQRh-Yj-l2ZcI,3680
-pyadtpulse-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyadtpulse-1.0.3.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
-pyadtpulse-1.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pyadtpulse-1.0.3.dist-info/RECORD,,
+pyadtpulse-1.0.4.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
+pyadtpulse-1.0.4.dist-info/METADATA,sha256=a5WUTd06XE00yvl96ThLPaDVEw_Bc7Ca_ITeQZKVaLI,3680
+pyadtpulse-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyadtpulse-1.0.4.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
+pyadtpulse-1.0.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyadtpulse-1.0.4.dist-info/RECORD,,
```

