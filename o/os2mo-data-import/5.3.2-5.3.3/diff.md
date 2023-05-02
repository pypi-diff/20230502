# Comparing `tmp/os2mo_data_import-5.3.2.tar.gz` & `tmp/os2mo_data_import-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2mo_data_import-5.3.2.tar", max compression
+gzip compressed data, was "os2mo_data_import-5.3.3.tar", max compression
```

## Comparing `os2mo_data_import-5.3.2.tar` & `os2mo_data_import-5.3.3.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0        0        0        0 2023-04-13 08:50:57.440809 os2mo_data_import-5.3.2/LICENSES/
--rw-r--r--   0        0        0    11696 2023-04-13 08:50:57.441809 os2mo_data_import-5.3.2/README.rst
--rw-r--r--   0        0        0       99 2023-04-13 08:50:57.441809 os2mo_data_import-5.3.2/kle/__init__.py
--rw-r--r--   0        0        0    13572 2023-04-13 08:50:57.441809 os2mo_data_import-5.3.2/kle/kle_import.py
--rw-r--r--   0        0        0     2261 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/kle/payloads.py
--rw-r--r--   0        0        0      332 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/__init__.py
--rw-r--r--   0        0        0     7243 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/mox_helper.py
--rw-r--r--   0        0        0    20756 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/mox_util.py
--rw-r--r--   0        0        0     2736 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/payloads.py
--rw-r--r--   0        0        0       40 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/mox_helpers/requirements.txt
--rw-r--r--   0        0        0      899 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/mox_helpers/utils.py
--rw-r--r--   0        0        0      397 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/__init__.py
--rw-r--r--   0        0        0     3799 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/caching_import.py
--rw-r--r--   0        0        0     1300 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/defaults.py
--rw-r--r--   0        0        0    19484 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/helpers.py
--rw-r--r--   0        0        0    22987 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/mora_data_types.py
--rw-r--r--   0        0        0    13436 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/mox_data_types.py
--rw-r--r--   0        0        0       99 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/tests/__init__.py
--rw-r--r--   0        0        0     1650 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/tests/test_utilities.py
--rw-r--r--   0        0        0    27431 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/utilities.py
--rw-r--r--   0        0        0      332 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/__init__.py
--rw-r--r--   0        0        0    30138 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/mora_helpers.py
--rw-r--r--   0        0        0       41 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/requirements.txt
--rw-r--r--   0        0        0     1169 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/settings.py
--rw-r--r--   0        0        0       99 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/tests/__init__.py
--rw-r--r--   0        0        0     3412 2023-04-13 08:50:57.446810 os2mo_data_import-5.3.2/os2mo_helpers/tests/test_morahelpers.py
--rw-r--r--   0        0        0     1080 2023-04-13 08:50:58.671979 os2mo_data_import-5.3.2/pyproject.toml
--rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.3.2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-01 08:05:41.162638 os2mo_data_import-5.3.3/LICENSES/
+-rw-r--r--   0        0        0    11696 2023-05-01 08:05:41.163638 os2mo_data_import-5.3.3/README.rst
+-rw-r--r--   0        0        0      332 2023-05-01 08:05:41.163638 os2mo_data_import-5.3.3/mox_helpers/__init__.py
+-rw-r--r--   0        0        0     7243 2023-05-01 08:05:41.164638 os2mo_data_import-5.3.3/mox_helpers/mox_helper.py
+-rw-r--r--   0        0        0    20756 2023-05-01 08:05:41.164638 os2mo_data_import-5.3.3/mox_helpers/mox_util.py
+-rw-r--r--   0        0        0     2736 2023-05-01 08:05:41.164638 os2mo_data_import-5.3.3/mox_helpers/payloads.py
+-rw-r--r--   0        0        0       40 2023-05-01 08:05:41.164638 os2mo_data_import-5.3.3/mox_helpers/requirements.txt
+-rw-r--r--   0        0        0      899 2023-05-01 08:05:41.164638 os2mo_data_import-5.3.3/mox_helpers/utils.py
+-rw-r--r--   0        0        0      397 2023-05-01 08:05:41.165638 os2mo_data_import-5.3.3/os2mo_data_import/__init__.py
+-rw-r--r--   0        0        0     3799 2023-05-01 08:05:41.165638 os2mo_data_import-5.3.3/os2mo_data_import/caching_import.py
+-rw-r--r--   0        0        0     1300 2023-05-01 08:05:41.165638 os2mo_data_import-5.3.3/os2mo_data_import/defaults.py
+-rw-r--r--   0        0        0    19484 2023-05-01 08:05:41.165638 os2mo_data_import-5.3.3/os2mo_data_import/helpers.py
+-rw-r--r--   0        0        0    22987 2023-05-01 08:05:41.166638 os2mo_data_import-5.3.3/os2mo_data_import/mora_data_types.py
+-rw-r--r--   0        0        0    13436 2023-05-01 08:05:41.166638 os2mo_data_import-5.3.3/os2mo_data_import/mox_data_types.py
+-rw-r--r--   0        0        0       99 2023-05-01 08:05:41.166638 os2mo_data_import-5.3.3/os2mo_data_import/tests/__init__.py
+-rw-r--r--   0        0        0     1650 2023-05-01 08:05:41.166638 os2mo_data_import-5.3.3/os2mo_data_import/tests/test_utilities.py
+-rw-r--r--   0        0        0    27431 2023-05-01 08:05:41.167639 os2mo_data_import-5.3.3/os2mo_data_import/utilities.py
+-rw-r--r--   0        0        0      332 2023-05-01 08:05:41.167639 os2mo_data_import-5.3.3/os2mo_helpers/__init__.py
+-rw-r--r--   0        0        0    30138 2023-05-01 08:05:41.167639 os2mo_data_import-5.3.3/os2mo_helpers/mora_helpers.py
+-rw-r--r--   0        0        0       41 2023-05-01 08:05:41.167639 os2mo_data_import-5.3.3/os2mo_helpers/requirements.txt
+-rw-r--r--   0        0        0     1169 2023-05-01 08:05:41.167639 os2mo_data_import-5.3.3/os2mo_helpers/settings.py
+-rw-r--r--   0        0        0       99 2023-05-01 08:05:41.168639 os2mo_data_import-5.3.3/os2mo_helpers/tests/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-01 08:05:41.168639 os2mo_data_import-5.3.3/os2mo_helpers/tests/test_morahelpers.py
+-rw-r--r--   0        0        0     1054 2023-05-01 08:05:42.796795 os2mo_data_import-5.3.3/pyproject.toml
+-rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.3.3/PKG-INFO
```

### Comparing `os2mo_data_import-5.3.2/README.rst` & `os2mo_data_import-5.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/kle/payloads.py` & `os2mo_data_import-5.3.3/mox_helpers/payloads.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,103 @@
 # SPDX-FileCopyrightText: 2023 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
-def _virkning(dato="1910-01-01 00:00:00"):
+def _virkning(dato=None):
+    if dato is None:
+        dato = "1910-01-01 00:00:00"
     virkning = {
         "from": dato,
         "to": "infinity",
         "aktoerref": "ddc99abd-c1b0-48c2-aef7-74fea841adae",
         "aktoertypekode": "Bruger",
     }
     return virkning
 
 
-def lora_facet(bvn, org="ddc99abd-c1b0-48c2-aef7-74fea841adae"):
+def lora_facet(bvn, org_uuid, description=None):
     attributter = {
         "facetegenskaber": [
             {
                 "brugervendtnoegle": bvn,
                 "virkning": _virkning(),
             }
         ]
     }
-    tilstande = {
-        "facetpubliceret": [{"publiceret": "Publiceret", "virkning": _virkning()}]
-    }
+    if description:
+        attributter["facetegenskaber"][0]["beskrivelse"] = description
+
     relationer = {
         "ansvarlig": [
-            {"objekttype": "organisation", "uuid": org, "virkning": _virkning()}
+            {"objekttype": "organisation", "uuid": org_uuid, "virkning": _virkning()}
         ]
     }
+    tilstande = {
+        "facetpubliceret": [{"publiceret": "Publiceret", "virkning": _virkning()}]
+    }
     facet = {
         "attributter": attributter,
-        "tilstande": tilstande,
         "relationer": relationer,
+        "tilstande": tilstande,
     }
     return facet
 
 
 def lora_klasse(
-    brugervendtnoegle,
-    beskrivelse,
-    titel,
-    dato,
-    facet,
-    ansvarlig,
-    omfang=None,
-    overklasse=None,
+    bvn,
+    title,
+    facet_uuid,
+    org_uuid,
+    org_unit_uuid=None,
+    description=None,
+    dato=None,
+    scope=None,
+    parent_uuid=None,
 ):
+    # NOTE: This is used from SD, and should be split out as a library?
     attributter = {
         "klasseegenskaber": [
             {
-                "brugervendtnoegle": brugervendtnoegle,
-                "beskrivelse": beskrivelse,
-                "titel": titel,
+                "brugervendtnoegle": bvn,
+                "titel": title,
                 "virkning": _virkning(dato),
             }
         ]
     }
+    if description:
+        attributter["klasseegenskaber"][0]["beskrivelse"] = description
+    if scope:
+        attributter["klasseegenskaber"][0]["omfang"] = scope
     tilstande = {
         "klassepubliceret": [{"publiceret": "Publiceret", "virkning": _virkning(dato)}]
     }
     relationer = {
-        "facet": [{"uuid": facet, "virkning": _virkning(dato), "objekttype": "Facet"}],
-        "overordnetklasse": [{"virkning": _virkning(dato), "objekttype": "Klasse"}],
+        "facet": [
+            {"uuid": facet_uuid, "virkning": _virkning(dato), "objekttype": "Facet"}
+        ],
+        "overordnetklasse": [
+            {"uuid": parent_uuid, "virkning": _virkning(dato), "objekttype": "Klasse"}
+        ],
         "ansvarlig": [
             {
-                "uuid": ansvarlig,
+                "uuid": org_uuid,
                 "virkning": _virkning(dato),
                 "objekttype": "Organisation",
             }
         ],
+        "ejer": [
+            {
+                "uuid": org_unit_uuid,
+                "virkning": _virkning(dato),
+                "objekttype": "OrganisationEnhed",
+            }
+        ],
     }
+    if parent_uuid is None:
+        del relationer["overordnetklasse"]
+    if org_unit_uuid is None:
+        del relationer["ejer"]
     klasse = {
         "attributter": attributter,
-        "tilstande": tilstande,
         "relationer": relationer,
+        "tilstande": tilstande,
     }
-    if overklasse is not None:
-        klasse["relationer"]["overordnetklasse"][0]["uuid"] = overklasse
-    else:
-        del klasse["relationer"]["overordnetklasse"]
-
-    if omfang:
-        attributter["klasseegenskaber"][0]["omfang"] = omfang
 
     return klasse
```

### Comparing `os2mo_data_import-5.3.2/mox_helpers/mox_helper.py` & `os2mo_data_import-5.3.3/mox_helpers/mox_helper.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/mox_helpers/mox_util.py` & `os2mo_data_import-5.3.3/mox_helpers/mox_util.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/mox_helpers/utils.py` & `os2mo_data_import-5.3.3/mox_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_data_import/caching_import.py` & `os2mo_data_import-5.3.3/os2mo_data_import/caching_import.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_data_import/defaults.py` & `os2mo_data_import-5.3.3/os2mo_data_import/defaults.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_data_import/helpers.py` & `os2mo_data_import-5.3.3/os2mo_data_import/helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_data_import/mora_data_types.py` & `os2mo_data_import-5.3.3/os2mo_data_import/mora_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_data_import/mox_data_types.py` & `os2mo_data_import-5.3.3/os2mo_data_import/mox_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_data_import/tests/test_utilities.py` & `os2mo_data_import-5.3.3/os2mo_data_import/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_data_import/utilities.py` & `os2mo_data_import-5.3.3/os2mo_data_import/utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_helpers/mora_helpers.py` & `os2mo_data_import-5.3.3/os2mo_helpers/mora_helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_helpers/settings.py` & `os2mo_data_import-5.3.3/os2mo_helpers/settings.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/os2mo_helpers/tests/test_morahelpers.py` & `os2mo_data_import-5.3.3/os2mo_helpers/tests/test_morahelpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.2/pyproject.toml` & `os2mo_data_import-5.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [tool.poetry]
 name = "os2mo_data_import"
-version = "5.3.2"
+version = "5.3.3"
 description = "A set of tools for OS2MO data import and export"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.rst"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo_data_import"
 keywords = ["os2mo", "dipex"]
 packages = [
     { include = "os2mo_data_import" },
     { include = "os2mo_helpers" },
     { include = "mox_helpers" },
-    { include = "kle" },
 ]
-
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.8.4"
 anytree = "^2.8.0"
 certifi = "^2022.12.7"
 chardet = "^5.1.0"
 click = "^8.1.3"
```

### Comparing `os2mo_data_import-5.3.2/PKG-INFO` & `os2mo_data_import-5.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2mo-data-import
-Version: 5.3.2
+Version: 5.3.3
 Summary: A set of tools for OS2MO data import and export
 Home-page: https://git.magenta.dk/rammearkitektur/os2mo_data_import
 License: MPL-2.0
 Keywords: os2mo,dipex
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
```

