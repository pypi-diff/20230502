# Comparing `tmp/unisci-1.4.3.tar.gz` & `tmp/unisci-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.4.3.tar", last modified: Sun Apr 30 23:16:17 2023, max compression
+gzip compressed data, was "unisci-1.4.4.tar", last modified: Tue May  2 02:21:07 2023, max compression
```

## Comparing `unisci-1.4.3.tar` & `unisci-1.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 23:16:17.651911 unisci-1.4.3/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.3/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.3/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-30 23:16:17.651594 unisci-1.4.3/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.3/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-30 23:16:17.652007 unisci-1.4.3/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-04-30 23:14:16.000000 unisci-1.4.3/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 23:16:17.643470 unisci-1.4.3/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-30 23:14:22.000000 unisci-1.4.3/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1507 2023-04-30 23:14:01.000000 unisci-1.4.3/unisci/_conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.3/unisci/_error.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.3/unisci/constants.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 23:16:17.646829 unisci-1.4.3/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.3/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.3/unisci/formulas/_validation.py
--rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.3/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1842 2023-04-30 22:59:28.000000 unisci-1.4.3/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 23:16:17.650844 unisci-1.4.3/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.3/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.4.3/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.3/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    38865 2023-04-30 22:56:45.000000 unisci-1.4.3/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 23:16:17.645635 unisci-1.4.3/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-30 23:16:17.000000 unisci-1.4.3/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-04-30 23:16:17.000000 unisci-1.4.3/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-30 23:16:17.000000 unisci-1.4.3/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-04-30 23:16:17.000000 unisci-1.4.3/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-30 23:16:17.000000 unisci-1.4.3/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.938977 unisci-1.4.4/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.4/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.4/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:21:07.938662 unisci-1.4.4/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.4/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-02 02:21:07.939069 unisci-1.4.4/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-01 22:47:51.000000 unisci-1.4.4/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.932860 unisci-1.4.4/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-01 22:47:55.000000 unisci-1.4.4/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.4.4/unisci/_conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.4/unisci/_error.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.4/unisci/constants.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.935131 unisci-1.4.4/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.4/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.4/unisci/formulas/_validation.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.4/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1842 2023-04-30 22:59:28.000000 unisci-1.4.4/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.938266 unisci-1.4.4/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.4/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.4.4/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.4/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    38865 2023-04-30 22:56:45.000000 unisci-1.4.4/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.934302 unisci-1.4.4/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.4.3/LICENSE` & `unisci-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/PKG-INFO` & `unisci-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.3
+Version: 1.4.4
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.3/README.md` & `unisci-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/setup.py` & `unisci-1.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.4.3',
+    version='1.4.4',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.4.3/unisci/_conversion_factors.py` & `unisci-1.4.4/unisci/_conversion_factors.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # for time conversions
 CONVERT_TO_SECONDS = {
     's': 1,
     'min': 60,
     'hr': 3600,
     'dy': 3600 * 24,
     'wk': 3600 * 24 * 7,
-    'yr': 3600 * 24 * 7 * 365.25
+    'yr': 3600 * 24 * 365.25
 }
 
 # for volume conversions
 CONVERT_TO_LITERS = {
     'L': 1,
     'c.': 0.2366,
     'pt.': 0.2366 * 2,
```

### Comparing `unisci-1.4.3/unisci/_error.py` & `unisci-1.4.4/unisci/_error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci/formulas/_validation.py` & `unisci-1.4.4/unisci/formulas/_validation.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci/formulas/chemistry.py` & `unisci-1.4.4/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci/metric.py` & `unisci-1.4.4/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci/periodic/periodic-table-lookup.json` & `unisci-1.4.4/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci/periodic/periodic-table-numbers.json` & `unisci-1.4.4/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci/periodic/periodic-table-symbols.json` & `unisci-1.4.4/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci/types.py` & `unisci-1.4.4/unisci/types.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.3/unisci.egg-info/PKG-INFO` & `unisci-1.4.4/unisci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.3
+Version: 1.4.4
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.3/unisci.egg-info/SOURCES.txt` & `unisci-1.4.4/unisci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

