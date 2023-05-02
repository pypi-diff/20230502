# Comparing `tmp/xdatasets-0.2.2.tar.gz` & `tmp/xdatasets-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdatasets-0.2.2.tar", last modified: Mon May  1 23:58:57 2023, max compression
+gzip compressed data, was "xdatasets-0.2.3.tar", last modified: Tue May  2 00:30:53 2023, max compression
```

## Comparing `xdatasets-0.2.2.tar` & `xdatasets-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:58:57.752591 xdatasets-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 23:58:54.000000 xdatasets-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-01 23:58:54.000000 xdatasets-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-01 23:58:54.000000 xdatasets-0.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 23:58:54.000000 xdatasets-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-01 23:58:54.000000 xdatasets-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 23:58:57.752591 xdatasets-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 23:58:54.000000 xdatasets-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 23:58:57.752591 xdatasets-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-01 23:58:54.000000 xdatasets-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:58:57.752591 xdatasets-0.2.2/xdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:58:57.752591 xdatasets-0.2.2/xdatasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:30:53.562669 xdatasets-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 00:30:49.000000 xdatasets-0.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-02 00:30:49.000000 xdatasets-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 00:30:49.000000 xdatasets-0.2.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-02 00:30:49.000000 xdatasets-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 00:30:49.000000 xdatasets-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-02 00:30:53.562669 xdatasets-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-02 00:30:49.000000 xdatasets-0.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-02 00:30:53.562669 xdatasets-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-02 00:30:49.000000 xdatasets-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:30:53.558669 xdatasets-0.2.3/xdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:30:53.562669 xdatasets-0.2.3/xdatasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/top_level.txt
```

### Comparing `xdatasets-0.2.2/CONTRIBUTING.rst` & `xdatasets-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/LICENSE` & `xdatasets-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/PKG-INFO` & `xdatasets-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.2
+Version: 0.2.3
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.2/README.rst` & `xdatasets-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/setup.py` & `xdatasets-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,10 +72,10 @@
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords=KEYWORDS,
     name=NAME,
     packages=find_packages(),
     extras_require={"dev": dev_requirements},
     url=URL,
-    version='0.2.2',
+    version='0.2.3',
     zip_safe=False,
 )
```

### Comparing `xdatasets-0.2.2/xdatasets/core.py` & `xdatasets-0.2.3/xdatasets/core.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/xdatasets/scripting.py` & `xdatasets-0.2.3/xdatasets/scripting.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/xdatasets/spatial.py` & `xdatasets-0.2.3/xdatasets/spatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Sequence, Tuple, Union, Dict, List, Optional
 
 from clisops.core.subset import subset_shape, subset_time, create_mask, shape_bbox_indexer, subset_gridpoint
 from clisops.core.average import average_shape
 import xarray as xr
 from tqdm import tqdm
 import logging
-import xagg as xa
+import xagg_no_xesmf_deps as xa
 import pandas as pd
 
 from .utils import HiddenPrints
 
 
 def bbox_ds(ds_copy, geom):
     indexer = shape_bbox_indexer(ds_copy, geom)
```

### Comparing `xdatasets-0.2.2/xdatasets/temporal.py` & `xdatasets-0.2.3/xdatasets/temporal.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/xdatasets/tutorial.py` & `xdatasets-0.2.3/xdatasets/tutorial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/xdatasets/utils.py` & `xdatasets-0.2.3/xdatasets/utils.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/xdatasets/validations.py` & `xdatasets-0.2.3/xdatasets/validations.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/xdatasets/workflows.py` & `xdatasets-0.2.3/xdatasets/workflows.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.2/xdatasets.egg-info/PKG-INFO` & `xdatasets-0.2.3/xdatasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.2
+Version: 0.2.3
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.2/xdatasets.egg-info/requires.txt` & `xdatasets-0.2.3/xdatasets.egg-info/requires.txt`

 * *Files identical despite different names*

