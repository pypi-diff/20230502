# Comparing `tmp/xdatasets-0.2.0.tar.gz` & `tmp/xdatasets-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdatasets-0.2.0.tar", last modified: Tue Mar 21 15:23:28 2023, max compression
+gzip compressed data, was "xdatasets-0.2.2.tar", last modified: Mon May  1 23:58:57 2023, max compression
```

## Comparing `xdatasets-0.2.0.tar` & `xdatasets-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:23:28.238359 xdatasets-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-21 15:23:21.000000 xdatasets-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-21 15:23:21.000000 xdatasets-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-21 15:23:21.000000 xdatasets-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-21 15:23:21.000000 xdatasets-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-21 15:23:21.000000 xdatasets-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-21 15:23:28.238359 xdatasets-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-21 15:23:21.000000 xdatasets-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-21 15:23:28.238359 xdatasets-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-21 15:23:21.000000 xdatasets-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:23:28.238359 xdatasets-0.2.0/xdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-21 15:23:21.000000 xdatasets-0.2.0/xdatasets/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:23:28.238359 xdatasets-0.2.0/xdatasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-21 15:23:28.000000 xdatasets-0.2.0/xdatasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-21 15:23:28.000000 xdatasets-0.2.0/xdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:23:28.000000 xdatasets-0.2.0/xdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:23:28.000000 xdatasets-0.2.0/xdatasets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-21 15:23:28.000000 xdatasets-0.2.0/xdatasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-21 15:23:28.000000 xdatasets-0.2.0/xdatasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:58:57.752591 xdatasets-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 23:58:54.000000 xdatasets-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-01 23:58:54.000000 xdatasets-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-01 23:58:54.000000 xdatasets-0.2.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 23:58:54.000000 xdatasets-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-01 23:58:54.000000 xdatasets-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 23:58:57.752591 xdatasets-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 23:58:54.000000 xdatasets-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 23:58:57.752591 xdatasets-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-01 23:58:54.000000 xdatasets-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:58:57.752591 xdatasets-0.2.2/xdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-01 23:58:54.000000 xdatasets-0.2.2/xdatasets/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:58:57.752591 xdatasets-0.2.2/xdatasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 23:58:57.000000 xdatasets-0.2.2/xdatasets.egg-info/top_level.txt
```

### Comparing `xdatasets-0.2.0/CONTRIBUTING.rst` & `xdatasets-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.0/LICENSE` & `xdatasets-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.0/PKG-INFO` & `xdatasets-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.0
+Version: 0.2.2
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.0/README.rst` & `xdatasets-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.0/setup.py` & `xdatasets-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 NAME = "xdatasets"
 DESCRIPTION = "Easy acess to earth observation datasets with xarray."
 URL = "https://github.com/hydrologie/xdatasets'"
 AUTHOR = "Sebastien Langlois"
 AUTHOR_EMAIL = "sebastien.langlois62@gmail.com"
 REQUIRES_PYTHON = ">=3.8.0"
-VERSION = "0.2.0"
 LICENSE = "MIT license"
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
@@ -29,17 +28,20 @@
     "jsonpickle",
     "numba",
     "numpy>=1.16",
     "pandas>=0.23",
     "pint>=0.10",
     "pyyaml",
     "s3fs>=2022.7.0",
+    "geopandas",
+    "tqdm",
     "scipy>=1.2",
     "xarray>=0.17",
-    "zarr>=2.11.1"
+    "zarr>=2.11.1",
+    "xagg-no-xesmf-deps"
 ]
 
 
 dev_requirements = []
 with open("requirements_dev.txt") as dev:
     for dependency in dev.readlines():
         dev_requirements.append(dependency)
@@ -70,10 +72,10 @@
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords=KEYWORDS,
     name=NAME,
     packages=find_packages(),
     extras_require={"dev": dev_requirements},
     url=URL,
-    version=VERSION,
+    version='0.2.2',
     zip_safe=False,
 )
```

### Comparing `xdatasets-0.2.0/xdatasets/core.py` & `xdatasets-0.2.2/xdatasets/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,32 +101,32 @@
         pangeo-forge:recipe_hash:  f2b6c75f28693bbae820161d5b71ebdb9d740dcdde0666...
         pangeo-forge:version:      0.9.4
         
     """
 
     def __init__(self,
                  datasets: Union[str, List[str], Dict[str, Union[str, List[str]]]],
-                 space: Dict[str, Union[str, List[str]]],
-                 time=dict(),
+                 space: Dict[str, Union[str, List[str]]] = dict(),
+                 time: Dict[str, Union[str, List[str]]] = dict(),
                  catalog_path: str = url_path
                  )-> None:
 
         self.catalog = intake.open_catalog(catalog_path)
         self.datasets = datasets
         self.space = self._resolve_space_params(**space)
         self.time = self._resolve_time_params(**time)
         
         self.load_query(datasets=self.datasets,
                         space=self.space,
                         time=self.time)
         
 
     def _resolve_space_params(self,
-                              clip: str, 
-                              geometry: Union[Dict[str, tuple], gpd.GeoDataFrame],
+                              clip: str = None, 
+                              geometry: Union[Dict[str, tuple], gpd.GeoDataFrame] = None,
                               averaging: Optional[bool] = False,
                               unique_id: Optional[str] = None
                               )-> Dict:
         
         
         """ 
         Resolves and validates user-provided space params
@@ -160,15 +160,15 @@
                 'unique_id': unique_id}
 
         return args
 
     def _resolve_time_params(self,
                              timestep: Optional[str] = None, 
                              aggregation: Optional[Dict[str, Union[Callable[..., Any], List[Callable[..., Any]]]]] = None,
-                             start: Optional[bool] = False,
+                             start: Optional[bool] = None,
                              end: Optional[str] = None,
                              timezone: Optional[str] = None,
                              ) -> Dict:
         
         
         """ 
         Resolves and validates user-provided time params
@@ -225,29 +225,32 @@
         elif isinstance(datasets, dict):
             datasets_name = list(datasets.keys())
 
         # Load data for each dataset
         dsets = []
         for dataset_name in datasets_name:
             data = None
+            kwargs = {}
             try:
                 variables_name = self.datasets[dataset_name]['variables']
+                if isinstance(variables_name, str):
+                    variables_name = [variables_name]
             except:
                 variables_name = None
                 pass
             try:
-                data = self.datasets[dataset_name]['data']
+                kwargs = {k:v for k,v in self.datasets[dataset_name].items() if k not in ['variables']}
             except:
                 pass
 
             ds_one = self._process_one_dataset(dataset_name=dataset_name,
                                                variables=variables_name,
                                                space=space,
                                                time=time,
-                                               data=data
+                                               **kwargs
                                                )
             dsets.append(ds_one)
             
         try:
             # Try naively merging datasets into single dataset
             ds = xr.merge(dsets)
             ds = ds
@@ -294,35 +297,31 @@
         elif dataset_category in ['hydrology']:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=RuntimeWarning)
                 ds = hydrometric_request(dataset_name,
                                          variables,
                                          space,
                                          time,
-                                         self.catalog)
+                                         self.catalog,
+                                         **kwargs)
                 
         elif dataset_category in ['user-provided']:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=RuntimeWarning)
                 ds = user_provided_dataset(dataset_name,
                                           variables,
                                           space,
                                           time,
                                           data)
         
         
         return ds
     
     def bbox_clip(self, ds):
+        """
+        """
         return ds.where(~ds.isnull(), drop=True)
-
-    def plot(self,
-             variables=None):
-
-        variables = ['t2m', 'tp']
-
-        return self.data[variables].hvplot(x='time', grid=True, subplots=True, shared_axes=False, by='geom', legend=True).cols(1)
```

### Comparing `xdatasets-0.2.0/xdatasets/scripting.py` & `xdatasets-0.2.2/xdatasets/scripting.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.0/xdatasets/spatial.py` & `xdatasets-0.2.2/xdatasets/spatial.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from typing import Sequence, Tuple, Union, Dict, List, Optional
 
-from clisops.core.subset import subset_shape, subset_time, create_mask, shape_bbox_indexer, create_weight_masks, subset_gridpoint
+from clisops.core.subset import subset_shape, subset_time, create_mask, shape_bbox_indexer, subset_gridpoint
 from clisops.core.average import average_shape
 import xarray as xr
 from tqdm import tqdm
 import logging
+import xagg as xa
+import pandas as pd
 
+from .utils import HiddenPrints
 
-def get_weight_masks(da, geom):
-    mask = create_weight_masks(da,
-            poly=geom)
-    da['weights'] = mask.squeeze()
-    da = da.where(da.weights>0, drop=True)
-    return da
 
 def bbox_ds(ds_copy, geom):
     indexer = shape_bbox_indexer(ds_copy, geom)
     da = ds_copy.isel(indexer)
     da = da.chunk({'latitude':-1, 'longitude':-1})
     return da
 
@@ -26,14 +23,35 @@
                  dataset_name
                  ):
     logging.info(f"Spatial operations: processing bbox with {dataset_name}")
     indexer = shape_bbox_indexer(ds, space['geometry'])
     ds_copy = ds.isel(indexer).copy()
     return ds_copy
     
+def create_weights_mask(da, poly):
+    
+    weightmap = xa.pixel_overlaps(da, poly, subset_bbox=True)
+
+    pixels = pd.DataFrame(index=weightmap.agg['pix_idxs'][0],
+                          data=list(map(list, weightmap.agg['coords'][0])),
+                          columns=['latitude','longitude']
+                         )
+
+    weights = pd.DataFrame(index=weightmap.agg['pix_idxs'][0],
+                 data=weightmap.agg['rel_area'][0][0].tolist(),
+                 columns=['weights'])
+
+
+    df = pd.merge(pixels, weights, left_index=True, right_index=True)
+    return df.set_index(['latitude', 'longitude']).to_xarray()
+
+def aggregate(ds_in, ds_weights):
+    return (ds_in*ds_weights.weights).sum(['latitude','longitude'], min_count=1)
+
+
 
 def clip_by_polygon(ds,
                     space,
                     dataset_name
                     ):
     indexer = shape_bbox_indexer(ds, space['geometry'])
     ds_copy = ds.isel(indexer).copy()
@@ -44,19 +62,25 @@
         item = row[space['unique_id']] if space['unique_id'] != None and space['unique_id'] in row else idx
         pbar.set_description(f"Spatial operations: processing polygon {item} with {dataset_name}")
 
         geom = space['geometry'].iloc[[idx]]
         da = bbox_ds(ds_copy, geom)
 
         # Average data array over shape
-        if space['averaging'] is True:            
-            da = average_shape(da, shape=geom)
+            #da = average_shape(da, shape=geom)
+        with HiddenPrints():
+            ds_weights  = create_weights_mask(da.isel(time=0), geom)
+        if space['averaging'] is True:   
+            da = aggregate(da, ds_weights)
         else:
-            da = get_weight_masks(da, geom)
+            da = xr.merge([da, ds_weights])
+            da = da.where(da.weights.notnull(), drop=True)
+        da = da.expand_dims({"geom": geom.index.values})
         arrays.append(da)
+
     data = xr.concat(arrays, dim='geom')
 
     if 'unique_id' in space:
         try:
             data = data.swap_dims({"geom": space["unique_id"]})
             data = data.drop('geom')
```

### Comparing `xdatasets-0.2.0/xdatasets/tutorial.py` & `xdatasets-0.2.2/xdatasets/tutorial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.0/xdatasets/utils.py` & `xdatasets-0.2.2/xdatasets/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import time
 from functools import reduce
+import os, sys
 
 catalog_path = 'https://raw.githubusercontent.com/hydrocloudservices/catalogs/main/catalogs/main.yaml'
 
 def open_dataset(
     name,
     catalog,
     **kws,
@@ -41,8 +42,18 @@
 
     if data.describe()['driver'][0] == 'geopandasfile':
         data =  data.read()
     elif data.describe()['driver'][0] == 'zarr':
         data = data.to_dask() 
     else:
         raise NotImplementedError(f'Dataset {name} is not available. Please request further datasets to our github issues pages')
-    return data  
+    return data  
+
+
+class HiddenPrints:
+    def __enter__(self):
+        self._original_stdout = sys.stdout
+        sys.stdout = open(os.devnull, 'w')
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        sys.stdout.close()
+        sys.stdout = self._original_stdout
```

### Comparing `xdatasets-0.2.0/xdatasets/validations.py` & `xdatasets-0.2.2/xdatasets/validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def _validate_space_params(clip: str, 
                             geometry: Union[Dict[str, tuple], gpd.GeoDataFrame],
                             averaging: bool = False,
                             unique_id: Optional[str] = None):
 
-    _clip_available_methods = ['bbox', 'point', 'polygon']
+    _clip_available_methods = ['bbox', 'point', 'polygon', None]
     
     if clip not in _clip_available_methods:
         raise ValueError(f"clip value '{clip}' is not one of {_clip_available_methods}")
         
     if not isinstance(averaging, bool):
         raise ValueError(f"averaging value '{averaging}' should be a boolean")
```

### Comparing `xdatasets-0.2.0/xdatasets.egg-info/PKG-INFO` & `xdatasets-0.2.2/xdatasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.0
+Version: 0.2.2
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.0/xdatasets.egg-info/requires.txt` & `xdatasets-0.2.2/xdatasets.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 jsonpickle
 numba
 numpy>=1.16
 pandas>=0.23
 pint>=0.10
 pyyaml
 s3fs>=2022.7.0
+geopandas
+tqdm
 scipy>=1.2
 xarray>=0.17
 zarr>=2.11.1
+xagg-no-xesmf-deps
 
 [dev]
 black
 bump2version
 coverage
 flake8
 flake8-rst-docstrings
```

