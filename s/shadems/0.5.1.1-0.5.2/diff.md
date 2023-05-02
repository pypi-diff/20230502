# Comparing `tmp/shadems-0.5.1.1.tar.gz` & `tmp/shadems-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadems-0.5.1.1.tar", last modified: Tue Sep 27 20:41:17 2022, max compression
+gzip compressed data, was "shadems-0.5.2.tar", max compression
```

## Comparing `shadems-0.5.1.1.tar` & `shadems-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:41:17.272594 shadems-0.5.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    15945 2022-09-27 20:41:17.272594 shadems-0.5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15283 2022-09-27 20:41:08.000000 shadems-0.5.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:41:17.268594 shadems-0.5.1.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      109 2022-09-27 20:41:08.000000 shadems-0.5.1.1/bin/shadems
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:41:17.272594 shadems-0.5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-09-27 20:41:08.000000 shadems-0.5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:41:17.272594 shadems-0.5.1.1/shade_ms/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20832 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8415 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19026 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/data_mappers.py
--rw-r--r--   0 runner    (1001) docker     (121)    26277 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/data_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)     6787 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/ds_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)    26242 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     8045 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/ms_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:41:17.272594 shadems-0.5.1.1/shade_ms/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-09-27 20:41:08.000000 shadems-0.5.1.1/shade_ms/tests/test_dask_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:41:17.272594 shadems-0.5.1.1/shadems.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15945 2022-09-27 20:41:17.000000 shadems-0.5.1.1/shadems.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-27 20:41:17.000000 shadems-0.5.1.1/shadems.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:41:17.000000 shadems-0.5.1.1/shadems.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-27 20:41:17.000000 shadems-0.5.1.1/shadems.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-27 20:41:17.000000 shadems-0.5.1.1/shadems.egg-info/top_level.txt
+-rw-r--r--   0        0        0    15283 2023-05-02 09:42:52.194320 shadems-0.5.2/README.md
+-rwxr-xr-x   0        0        0      109 2023-05-02 09:42:52.194320 shadems-0.5.2/bin/shadems
+-rw-r--r--   0        0        0     1663 2023-05-02 09:42:52.222319 shadems-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1092 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/__init__.py
+-rw-r--r--   0        0        0    20832 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/__main__.py
+-rw-r--r--   0        0        0     8415 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/dask_utils.py
+-rw-r--r--   0        0        0    19026 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/data_mappers.py
+-rw-r--r--   0        0        0    27196 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/data_plots.py
+-rw-r--r--   0        0        0     6787 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/ds_ext.py
+-rw-r--r--   0        0        0    26242 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/main.py
+-rw-r--r--   0        0        0     8564 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/ms_info.py
+-rw-r--r--   0        0        0      528 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/Makefile
+-rw-r--r--   0        0        0      711 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/__init__.py
+-rwxr-xr-x   0        0        0     7568 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/check-shadems-functionality.sh
+-rw-r--r--   0        0        0     3537 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/test_dask_utils.py
+-rw-r--r--   0        0        0    16827 1970-01-01 00:00:00.000000 shadems-0.5.2/PKG-INFO
```

### Comparing `shadems-0.5.1.1/PKG-INFO` & `shadems-0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: shadems
-Version: 0.5.1.1
-Summary: Rapid Measurement Set plotting with dask-ms and datashader
-Home-page: https://github.com/ratt-ru/shadeMS
-Author: Ian Heywood & RATT
-Author-email: ian.heywood@physics.ox.ac.uk
-License: GNU GPL v2
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-
 # shadems
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/shadems.svg)](https://pypi.python.org/pypi/shadems/)
 
 `shadems` is a tool for plotting interferometric visibilities or associated metadata from CASA format Measurement Sets. 
 The primary goal is rapid visualisation of the many billions of data points produced by a typical observation
```

### Comparing `shadems-0.5.1.1/README.md` & `shadems-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: shadems
+Version: 0.5.2
+Summary: Rapid Measurement Set plotting with dask-ms and datashader
+Home-page: https://github.com/ratt-ru/shadeMS
+License: GPL-2.0-only
+Keywords: Astronomy,Visualisation,Packaging
+Author: Ian Heywood & RATT
+Author-email: ian.heywood@physics.ox.ac.uk
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Provides-Extra: testing
+Requires-Dist: cmasher (>=1.6.3,<2.0.0)
+Requires-Dist: dask-ms[xarray] (>=0.2.15,<0.3.0)
+Requires-Dist: dask[array] (==2022.9.1)
+Requires-Dist: datashader
+Requires-Dist: future-fstrings (>=1.2.0,<2.0.0)
+Requires-Dist: holoviews (>=1.14.9,<2.0.0)
+Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
+Requires-Dist: numpy (==1.23.5)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: pytest (>=7.2.2,<8.0.0) ; extra == "testing"
+Requires-Dist: pytest-flake8 (>=1.1.1,<2.0.0) ; extra == "testing"
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Repository, https://github.com/ratt-ru/shadeMS
+Description-Content-Type: text/markdown
+
 # shadems
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/shadems.svg)](https://pypi.python.org/pypi/shadems/)
 
 `shadems` is a tool for plotting interferometric visibilities or associated metadata from CASA format Measurement Sets. 
 The primary goal is rapid visualisation of the many billions of data points produced by a typical observation 
@@ -305,7 +342,8 @@
                         Use -j0 to auto-set this to half the available cores
                         (36 on this system). This is not necessarily faster,
                         as they might all end up contending for disk I/O. This
                         might also work against dask-ms's own intrinsic
                         parallelism. You have been advised.
   --profile             Enable dask profiling output
 ```
+
```

### Comparing `shadems-0.5.1.1/shade_ms/__init__.py` & `shadems-0.5.2/shade_ms/__init__.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.1.1/shade_ms/__main__.py` & `shadems-0.5.2/shade_ms/__main__.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.1.1/shade_ms/dask_utils.py` & `shadems-0.5.2/shade_ms/dask_utils.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.1.1/shade_ms/data_mappers.py` & `shadems-0.5.2/shade_ms/data_mappers.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.1.1/shade_ms/data_plots.py` & `shadems-0.5.2/shade_ms/data_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,23 +147,29 @@
 
             # number of rows in dataframe
             nrows0 = output_rows.setdefault(dataframe_key, 0)
 
             # always read flags -- easier that way
             flag = group.FLAG if not noflags else None
             flag_row = group.FLAG_ROW if not noflags else None
-
-            a1 = da.minimum(group.ANTENNA1.data, group.ANTENNA2.data)
-            a2 = da.maximum(group.ANTENNA1.data, group.ANTENNA2.data)
-            baselines = msinfo.baseline_number(a1, a2)
-
+            if not iter_baseline:
+                # if group by then these are attributes, not data arrays
+                a1 = da.minimum(group.ANTENNA1.data, group.ANTENNA2.data)
+                a2 = da.maximum(group.ANTENNA1.data, group.ANTENNA2.data)
+                baselines = msinfo.baseline_number(a1, a2)
+            else:
+                baselines = None
             freqs = chan_freqs[ddid]
             chans = xarray.DataArray(range(len(freqs)), dims=("chan",))
             wavel = freq_to_wavel(freqs)
-            extras = dict(chans=chans, freqs=freqs, wavel=wavel, rows=group.row, baselines=baselines)
+            extras = dict(chans=chans,
+                          freqs=freqs,
+                          wavel=wavel,
+                          rows=group.row,
+                          baselines=baselines if [baselines] else np.array([baseline]))
 
             nchan = len(group.chan)
             if flag is not None:
                 flag = flag[dict(chan=chanslice)]
                 nchan = flag.shape[1]
             shape = (len(group.row), nchan)
 
@@ -464,38 +470,51 @@
         img = datashader.transfer_functions.dynspread(img, options.spread_thr, max_px=options.spread_pix)
         log.info(f": spreading ({options.spread_thr} {options.spread_pix})")
     rgb = holoviews.RGB(holoviews.operation.datashader.shade.uint32_to_uint8_xr(img))
 
     log.debug('done')
 
     # Set plot limits based on data extent or user values for axis labels
-
-    xmin, xmax = bounds[xaxis]
-    ymin, ymax = bounds[yaxis]
-
+    limits = {
+        "xmin": bounds[xaxis][0],
+        "xmax": bounds[xaxis][1],
+        "ymin": bounds[yaxis][0],
+        "ymax": bounds[yaxis][1]
+    }
     log.debug('rendering image')
 
     fig = pylab.figure(figsize=(figx, figy))
     ax = fig.add_subplot(111, facecolor=bgcol)
 
     for funcname, args, kwargs in extra_markup:
         getattr(ax, funcname)(*args, **kwargs)
-
-    ax.imshow(X=rgb.data, extent=[xmin, xmax, ymin, ymax],
-              aspect='auto', origin='lower', interpolation='nearest')
+    
+    # any 1D arrays like freq and WAVEL that is dask arrays at this point needs
+    # compute called
+    compute_arrays = dict(filter(lambda x: isinstance(x[1], da.Array), limits.items()))
+    limits.update(dict(zip(compute_arrays.keys(), da.compute(*compute_arrays.values()))))
+
+    ax.imshow(X=rgb.data, 
+              extent=[limits['xmin'], 
+                      limits['xmax'],
+                      limits['ymin'],
+                      limits['ymax']],
+              aspect='auto',
+              origin='lower',
+              interpolation='nearest')
 
     ax.set_title("\n".join(textwrap.wrap(title, 90)), loc='center', fontdict=dict(fontsize=options.fontsize))
     ax.set_xlabel(xlabel, fontdict=dict(fontsize=options.fontsize))
     ax.set_ylabel(ylabel, fontdict=dict(fontsize=options.fontsize))
     # ax.plot(xmin,ymin,'.',alpha=0.0)
     # ax.plot(xmax,ymax,'.',alpha=0.0)
 
-    dx, dy = xmax - xmin, ymax - ymin
-    ax.set_xlim([xmin - dx/100, xmax + dx/100])
-    ax.set_ylim([ymin - dy/100, ymax + dy/100])
+    dx, dy = limits['xmax'] - limits['xmin'], limits['ymax'] - limits['ymin']
+    ax.set_xlim([limits['xmin'] - dx/100, limits['xmax'] + dx/100])
+    ax.set_ylim([limits['ymin'] - dy/100, limits['ymax'] + dy/100])
 
     def decimate_list(x, maxel):
         """Helper function to reduce a list to < given max number of elements, dividing it by decimal factors of 2 and 5"""
         factors = 2, 5, 10
         base = divisor = 1
         while len(x)//divisor > maxel:
             for fac in factors:
```

### Comparing `shadems-0.5.1.1/shade_ms/ds_ext.py` & `shadems-0.5.2/shade_ms/ds_ext.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.1.1/shade_ms/main.py` & `shadems-0.5.2/shade_ms/main.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.1.1/shade_ms/ms_info.py` & `shadems-0.5.2/shade_ms/ms_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,50 @@
-from MSUtils.msutils import STOKES_TYPES
 from casacore.tables import table
 import re
 import daskms
 import math
 import numpy as np
 from collections import OrderedDict
 
+STOKES_TYPES = {
+    0  : "Undefined",
+    1  : "I",
+    2  : "Q",
+    3  : "U",
+    4  : "V",
+    5  : "RR",
+    6  : "RL",
+    7  : "LR",
+    8  : "LL",
+    9  : "XX",
+    10 : "XY",
+    11 : "YX",
+    12 : "YY",
+    13 : "RX",
+    14 : "RY",
+    15 : "LX",
+    16 : "LY",
+    17 : "XR",
+    18 : "XL",
+    19 : "YR",
+    20 : "YL",
+    21 : "PP",
+    22 : "PQ",
+    23 : "QP",
+    24 : "QQ",
+    25 : "RCircular",
+    26 : "LCircular",
+    27 : "Linear",
+    28 : "Ptotal",
+    29 : "Plinear",
+    30 : "PFtotal",
+    31 : "PFlinear",
+    32 : "Pangle",
+}
+
 class NamedList(object):
     """Holds a list of names (e.g. field names), and provides common indexing and subset operations"""
 
     def __init__(self, label, names, numbers=None):
         self.label = label
         self.names = names
         self.numbers = numbers or range(len(self.names))
```

### Comparing `shadems-0.5.1.1/shade_ms/tests/test_dask_utils.py` & `shadems-0.5.2/shade_ms/tests/test_dask_utils.py`

 * *Files identical despite different names*

