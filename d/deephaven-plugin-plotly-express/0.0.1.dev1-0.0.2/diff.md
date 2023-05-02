# Comparing `tmp/deephaven-plugin-plotly-express-0.0.1.dev1.tar.gz` & `tmp/deephaven-plugin-plotly-express-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-plotly-express-0.0.1.dev1.tar", last modified: Fri Apr 14 22:57:47 2023, max compression
+gzip compressed data, was "deephaven-plugin-plotly-express-0.0.2.tar", last modified: Tue May  2 17:45:17 2023, max compression
```

## Comparing `deephaven-plugin-plotly-express-0.0.1.dev1.tar` & `deephaven-plugin-plotly-express-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.174360 deephaven-plugin-plotly-express-0.0.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-14 22:57:47.174360 deephaven-plugin-plotly-express-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-14 22:57:47.178360 deephaven-plugin-plotly-express-0.0.1.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.166360 deephaven-plugin-plotly-express-0.0.1.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.166360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.166360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.166360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.170360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/DataMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/data_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/json_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.170360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/custom_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.174360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/_private_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/area.py
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/financial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/hierarchial.py
--rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.174360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/preprocess/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.174360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 22:57:35.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/shared/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:47.174360 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-14 22:57:47.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 22:57:47.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:57:47.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 22:57:47.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 22:57:47.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 22:57:47.000000 deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.347500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/DataMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/data_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/json_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.347500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/custom_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.347500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/_private_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/financial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/hierarchial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/LICENSE` & `deephaven-plugin-plotly-express-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.1.dev1
+Version: 0.0.2
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/README.md` & `deephaven-plugin-plotly-express-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/setup.cfg` & `deephaven-plugin-plotly-express-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/__init__.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .deephaven_figure import DeephavenFigure, export_figure
 
 from .plots import area, bar, frequency_bar, timeline, histogram, _ecdf, box, \
     violin, strip, ohlc, candlestick, treemap, sunburst, icicle, funnel, \
     funnel_area, line, line_polar, line_ternary, line_3d, scatter, scatter_3d, \
     scatter_polar, scatter_ternary, pie, layer
 
-__version__ = "0.0.1.dev1"
+__version__ = "0.0.2"
 
 NAME = "deephaven.plot.express.DeephavenFigure"
 
 
 class DeephavenFigureType(ObjectType):
     @property
     def name(self) -> str:
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/DataMapping.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/DataMapping.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/data_mapping.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/data_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "error_x": "error_x/array",
     "error_x_minus": "error_x/arrayminus",
     "error_y": "error_y/array",
     "error_y_minus": "error_y/arrayminus",
     "error_z": "error_z/array",
     "error_z_minus": "error_z/arrayminus",
     "x_diff": "x",
+    "size": "marker/size",
 }
 
 # override these data columns with different names
 OVERRIDES = {
     "names": "labels",
     "x_start": "base",
 }
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/data_mapping/json_conversion.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/json_conversion.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,25 +73,26 @@
             self: DeephavenFigure,
             fig: Figure = None,
             call: Callable = None,
             call_args: dict[any] = None,
             data_mappings: list[DataMapping] = None,
             has_template: str = None,
             has_color: bool = False,
-            trace_generator: Generator[dict[str, any]] = None
+            trace_generator: Generator[dict[str, any]] = None,
+            has_subplots: bool = False
     ):
         """
         Initialize a DeephavenFigure
 
         :param fig: The underlying plotly fig
         :param call_args: The arguments that were used to call px
         :param call: The (usually) px drawing function
         :param data_mappings:A list of data mappings from table column to
         corresponding plotly variable
-        :param template: A template that is used
+        :param has_template: If a template is used
         :param has_color: True if color was manually applied via
         discrete_color_sequence
         :param trace_generator: A generator for modifications to traces
         """
         # keep track of function that called this and it's args
         self.fig = fig
         self.call = call
@@ -102,14 +103,16 @@
             has_arg(call_args, "template")
 
         self.has_color = has_color if has_color else \
             has_arg(call_args, has_color_args)
 
         self._data_mappings = data_mappings if data_mappings else []
 
+        self.has_subplots = has_subplots
+
     def copy_mappings(
             self: DeephavenFigure,
             offset: int = 0
     ) -> list[DataMapping]:
         """
         Copy all DataMappings within this figure, adding a specific offset
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/custom_draw.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/custom_draw.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,19 +42,19 @@
                             close=data_frame[close]))
 
     return go.Figure(data=data)
 
 
 def draw_ohlc(
         data_frame: DataFrame,
-        x_finance: str,
-        open: str,
-        high: str,
-        low: str,
-        close: str
+        x_finance: str | list[str],
+        open: str | list[str],
+        high: str | list[str],
+        low: str | list[str],
+        close: str | list[str],
 ) -> Figure:
     """
     Create a plotly OHLC chart.
 
     :param data_frame: The data frame to draw with
     :param x_finance: The name of the column containing x-axis values
     :param open: The name of the column containing open values
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/deephaven_figure/generate.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,43 +60,48 @@
     # px can handle multiple colors in wide mode, but not if new data is added
     # need separate keys for line and scatter color as they are written to
     # different locations
     "color_discrete_sequence_line": "line_color",
     "color_discrete_sequence_marker": "marker_color",
     "increasing_color_sequence": "increasing_line_color",
     "decreasing_color_sequence": "decreasing_line_color",
+    "size_sequence": "marker_size"
 }
 
 # these args should always be converted to a list and only passed to custom
 # args
 CUSTOM_LIST_ARGS = {
     "log_x", "range_x",
     "log_y", "range_y",
-    "xaxis_title_sequence", "yaxis_title_sequence",
+    "xaxis_titles", "yaxis_titles",
     "x_diff"
 }
 CUSTOM_LIST_ARGS.update(AXIS_SEQUENCE_ARGS)
 
 # any custom args should be specified here to prevent them from being passed
 # to plotly express
 # Note that table is not here because it is pulled off and converted to a
 # pandas data frame separately
 CUSTOM_ARGS = {
-    "callback",
     "bargap",
+    "marginal",
+    "marginal_x",
+    "marginal_y"
     #"rangemode"
 }
 
-ERROR_UPDATE_MAP = {
+# these are columns that are "attached" sequentially to the traces
+ATTACHED_UPDATE_MAP = {
     "error_x": "error_x_array",
     "error_x_minus": "error_x_arrayminus",
     "error_y": "error_y_array",
     "error_y_minus": "error_y_arrayminus",
     "error_z": "error_z_array",
-    "error_z_minus": "error_z_arrayminus"
+    "error_z_minus": "error_z_arrayminus",
+    "size": "marker_size"
 }
 
 
 def col_null_mapping(
         table: Table, cols: set[str]
 ) -> Generator[tuple[str, str]]:
     """
@@ -188,15 +193,15 @@
                 new_call_args[arg.removesuffix('_scene')] = val
             elif arg.startswith("range_"):
                 # range is a special case as ranges are a list
                 # None can be specified for no range within a list of ranges
                 custom_call_args[arg] = val if \
                     (isinstance(val[0], list) or val[0] is None) else [val]
             elif any([arg in mappable for mappable in
-                      [ERROR_UPDATE_MAP, SEQUENCE_ARGS_MAP, CUSTOM_LIST_ARGS]]):
+                      [ATTACHED_UPDATE_MAP, SEQUENCE_ARGS_MAP, CUSTOM_LIST_ARGS]]):
                 # some of these args should always be lists, so the check is
                 # redundant, but useful if a single valid value is passed
                 custom_call_args[arg] = val if isinstance(val, list) else [val]
             elif arg in DATA_LIST_ARGS:
                 new_call_args[arg] = val if isinstance(val, list) else [val]
             else:
                 new_call_args[arg] = val
@@ -215,19 +220,19 @@
     :returns: Generated dict
     """
     bottom = True
     for num in count(start=1):
         update = {
             "anchor": "free" if num >= 2 else "y",
             "overlaying": "x" if num >= 2 else None,
-            "side": "bottom" if bottom else "top",
+            "side": "bottom" if bottom else "top"
         }
         # only update the title if there is an axis arg
         if update_titles:
-            update["title"] = {"text": f"X Values {num}"}
+            update["title"] = None #{"text": f"X Values {num}"}
         yield update
         bottom = not bottom
 
 
 def base_y_axis_generator(
     update_titles: bool = False
 ) -> Generator[dict]:
@@ -239,19 +244,19 @@
     :returns: Generated dict
     """
     left = True
     for num in count(start=1):
         update = {
             "anchor": "free" if num >= 2 else "x",
             "overlaying": "y" if num >= 2 else None,
-            "side": "left" if left else "right",
+            "side": "left" if left else "right"
         }
         # only update the title if there is an axis arg
         if update_titles:
-            update["title"] = {"text": f"Y Values {num}"}
+            update["title"] = None #{"text": f"Y Values {num}"}
         yield update
         left = not left
 
 
 def key_val_generator(  # this can handle log, range, title, domain (once calculated)
         key: str,
         vals: list[any]
@@ -284,29 +289,29 @@
 
     for new_axis in cycle(new_axes):
         # don't number the first axis as it's already created without numbering
         new_axis = "" if new_axis == 1 else new_axis
         yield f"{var}axis", f"{var}{new_axis}"
 
 
-def new_error_generator(
+def attached_generator(
         arg: str,
-        error_cols: list[str]
+        attached_cols: list[str]
 ) -> Generator[tuple[str, list]]:
     """
     Generate key, value pairs for error bar updates. If an error column is
     None, then there is no error bar drawn for the corresponding trace.
 
     :param arg: The error bar to map to an update
-    :param error_cols: A list of error columns to determine what the value
+    :param attached_cols: A list of error columns to determine what the value
     should be
     :returns: Generates a list of key, value pairs of (error update, value)
     """
-    for error_col in cycle(error_cols):
-        yield ERROR_UPDATE_MAP[arg], [] if error_col else None
+    for error_col in cycle(attached_cols):
+        yield ATTACHED_UPDATE_MAP[arg], [] if error_col else None
 
 
 def update_traces(
         fig: Figure,
         generator: Generator[dict],
         step: int = 1,
 ) -> None:
@@ -517,16 +522,16 @@
                     y_axis_generators.append(key_val_generator("domain", [y_domain]))
                 else:
                     y_axis_generators.append(position_generator(x_domain))
                     last_y_axis = max(val)
                     last_x_axis = max(1, last_x_axis)
                     x_axis_generators.append(key_val_generator("domain", [x_domain]))
 
-            elif arg in ERROR_UPDATE_MAP:
-                trace_generators.append(new_error_generator(arg, val))
+            elif arg in ATTACHED_UPDATE_MAP:
+                trace_generators.append(attached_generator(arg, val))
 
             elif arg in SEQUENCE_ARGS_MAP:
                 trace_generators.append(sequence_generator(arg, val))
 
             elif arg == "log_x":
                 last_x_axis = max(1, last_x_axis)
                 x_axis_generators.append(log_generator(val))
@@ -571,30 +576,27 @@
 
 
 def generate_figure(
         draw: Callable,
         call_args: dict[str, any],
         start_index: int = 0,
         trace_generator: Generator[dict] = None,
-        allow_callback: bool = True
 ) -> DeephavenFigure:
     """
     Generate a figure using a plotly express function as well as any args that
     should be used
 
     :param draw: The plotly express function to use to generate the figure
     :param call_args: Call arguments to use, either passing to plotly express
     or handled separately
     :param start_index: Optional argument. Only needed if there are existing
     traces that this figure is being added to. In that case, the data mapping
     needs to start at the end of the existing traces.
     :param trace_generator: Optional, if provided then only use this trace
     generator and return (as layout should already be created)
-    :param allow_callback: Optional, set to False to disable the callback if
-    more processing is needed before this figure is "done"
     :return: a Deephaven figure
     """
     table = call_args.pop("table")
 
     filtered_call_args, custom_call_args = split_args(call_args)
 
     data_cols = get_data_cols(filtered_call_args)
@@ -607,29 +609,23 @@
     px_fig = draw(data_frame=data_frame, **filtered_call_args)
 
     trace_generator = handle_custom_args(px_fig,
                                          custom_call_args,
                                          step=1,
                                          trace_generator=trace_generator)
 
-    # allow either returning a new fig or not from callback
-    new_fig = None
-    if allow_callback:
-        new_fig = custom_call_args['callback'](px_fig)
-    new_fig = new_fig if new_fig else px_fig
-
     data_mapping = create_data_mapping(
         data_cols,
         custom_call_args,
         table,
         start_index
     )
 
     dh_fig = DeephavenFigure(
-        new_fig,
+        px_fig,
         call_args=call_args,
         call=draw,
         data_mappings=[data_mapping],
         trace_generator=trace_generator
     )
 
     return dh_fig
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/area.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/area.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,72 @@
+from functools import partial
 from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args
+from ._private_utils import default_callback, validate_common_args, unsafe_figure_update_wrapper
 from ..deephaven_figure import generate_figure, DeephavenFigure
 
 
 def area(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
         pattern_shape_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
         xaxis_sequence: list[str] = None,
         yaxis_sequence: list[str] = None,
-        yaxis_title_sequence: list[str] = None,
-        xaxis_title_sequence: list[str] = None,
         markers: bool = False,
         # todo: groupnorm in engine
         groupnorm: str = None,
         log_x: bool | list[bool] = False,
         log_y: bool | list[bool] = False,
         range_x: list[int] | list[list[int]] = None,
         range_y: list[int] | list[list[int]] = None,
+        yaxis_titles: list[str] = None,
+        xaxis_titles: list[str] = None,
         line_shape: str = 'linear',
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns an area chart
 
     :param table: A table to pull data from.
     :param x: A column or list of columns that contain x-axis values.
     :param y: A column or list of columns that contain y-axis values.
+    :param size: A column or list of columns that contain size values.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
-    :param symbol_sequence: A list of symbols to sequentially apply to the
-    series. The symbols loop, so if there are more series than symbols, symbols
-    will be reused.
     :param pattern_shape_sequence: A list of patterns to sequentially apply
     to the series. The patterns loop, so if there are more series than
     patterns, patterns will be reused.
+    :param symbol_sequence: A list of symbols to sequentially apply to the
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
     :param xaxis_sequence: A list of x axes to assign series to. Odd numbers
     starting with 1 are created on the bottom x axis and even numbers starting
     with 2 are created on the top x axis. Axes are created up
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
     :param yaxis_sequence: A list of y axes to assign series to. Odd numbers
     starting with 1 are created on the left y axis and even numbers starting
     with 2 are created on the top y axis. Axes are created up
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
-    :param yaxis_title_sequence: A list of titles to sequentially apply to the
-    y axes. The titles do not loop.
-    :param xaxis_title_sequence: A list of titles to sequentially apply to the
-    x axes. The titles do not loop.
     :param markers: True to draw markers on the line, False to not. Default
     False
     :param groupnorm: Default None. 'fraction' to plot the fraction out of
     the total value of all points at that x value, 'percent' to take the
     fraction and multiply by 100. Note that if multiple y axes are
     specified, the groupnorm is taken per axis.
     :param log_x: Default False. A boolean or list of booleans that specify if
@@ -73,27 +76,42 @@
     the corresponding axis is a log axis or not. The booleans loop, so if there
     are more series than booleans, booleans will be reused.
     :param range_x: A list of two numbers or a list of lists of two numbers
     that specify the range of the x axes. None can be specified for no range
     The ranges loop, so if there are more axes than ranges, ranges will
     be reused.
     :param range_y: A list of two numbers or a list of lists of two numbers
-     that specify the range of the x axes. None can be specified for no range
+    that specify the range of the x axes. None can be specified for no range
     The ranges loop, so if there are more axes than ranges, ranges will
     be reused.
+    :param yaxis_titles: A list of titles to sequentially apply to the
+    y axes. The titles do not loop.
+    :param xaxis_titles: A list of titles to sequentially apply to the
+    x axes. The titles do not loop.
     :param line_shape: The line shape for all lines created. One of 'linear',
     'spline', 'vhv', 'hvh', 'vh', 'hv'. Default 'linear'
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the area chart
     """
     args = locals()
+
+    validate_common_args(args)
+
     args["pattern_shape_sequence_area"] = args.pop("pattern_shape_sequence")
     args["color_discrete_sequence_marker"] = args["color_discrete_sequence"]
     args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
 
-    validate_common_args(args)
-
-    return generate_figure(draw=px.area, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.area, call_args=args)
+    )
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/bar.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/bar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args, preprocess_and_layer
+from ._private_utils import default_callback, validate_common_args, preprocess_and_layer, unsafe_figure_update_wrapper
 from ..deephaven_figure import generate_figure, DeephavenFigure
 from ..preprocess import preprocess_timeline, preprocess_frequency_bar
 
 
 def bar(
         table: Table = None,
         x: str | list[str] = None,
@@ -25,15 +25,15 @@
         log_x: bool = False,
         log_y: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
         text_auto: bool | str = False,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a bar chart
 
     :param table: A table to pull data from.
     :param x: A column or list of columns that contain x-axis values.
     :param y: A column or list of columns that contain y-axis values.
@@ -82,26 +82,36 @@
     that specify the range of the x axes. None can be specified for no range
     The ranges loop, so if there are more axes than ranges, ranges will
     be reused.
     :param text_auto: Default False. If True, display the value at each bar.
     If a string, specifies a plotly texttemplate.
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the bar chart
     """
     args = locals()
     args["pattern_shape_sequence_bar"] = args.pop("pattern_shape_sequence")
     args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.bar, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.bar, call_args=args)
+    )
 
 
 def _bar_polar(
         table: Table = None,
         r: str = None,
         theta: str = None,
         color_discrete_sequence: list[str] = None,
@@ -111,15 +121,15 @@
         direction: str = 'clockwise',
         start_angle: int = 90,
         range_r: list[int] = None,
         range_theta: list[int] = None,
         log_r: bool = False,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     # todo: not yet implemented
     if isinstance(table, Table):
         args = locals()
         args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
         validate_common_args(args)
@@ -135,15 +145,15 @@
         color_discrete_sequence: list[str] = None,
         pattern_shape_sequence: list[str] = None,
         opacity: float = None,
         range_x: list[int] = None,
         range_y: list[int] = None,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ):
     """
     Returns a timeline (otherwise known as a gantt chart)
 
     :param table: A table to pull data from.
     :param x_start: A column that contains starting x-axis values.
     :param x_end: A column that contains ending x-axis values.
@@ -156,27 +166,37 @@
     patterns, patterns will be reused.
     :param opacity: Opacity to apply to all points. 0 is completely transparent
     and 1 is completely opaque.
     :param range_x: A list of two numbers that specify the range of the x axis.
     :param range_y: A list of two numbers that specify the range of the y axis.
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the timeline chart
     """
     # TODO: add resource column?
     table, x_diff = preprocess_timeline(table, x_start, x_end, y)
     args = locals()
     args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.timeline, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.timeline, call_args=args)
+    )
 
 
 def frequency_bar(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
@@ -186,15 +206,15 @@
         log_x: bool = False,
         log_y: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
         text_auto: bool | str = False,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ):
     """
     Returns a bar chart that contains the counts of the specified columns
 
     :param table: A table to pull data from.
     :param x: A column name or list of columns that contain x-axis values.
     Only one of x or y can be specified. If x is specified, the bars are drawn
@@ -219,27 +239,37 @@
     axis or not.
     :param range_x: A list of two numbers that specify the range of the x axis.
     :param range_y: A list of two numbers that specify the range of the y axis.
     :param text_auto: Default False. If True, display the value at each bar.
     If a string, specifies a plotly texttemplate.
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the bar chart
     """
 
     if x and y:
         raise ValueError("Cannot specify both x and y")
 
     args = locals()
     args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
     args["pattern_shape_sequence_bar"] = args.pop("pattern_shape_sequence")
 
     validate_common_args(args)
 
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
     create_layered = partial(preprocess_and_layer,
                              preprocess_frequency_bar,
                              px.bar, args, list_var_axis_name="value")
 
-    return create_layered("x") if x else create_layered("y", orientation="h")
+    return update_wrapper(
+        create_layered("x") if x else create_layered("y", orientation="h")
+    )
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/distribution.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/scatter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,331 +1,371 @@
+import json
 from functools import partial
 from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args, preprocess_and_layer
+from .distribution import attach_marginals, get_marg_args
+from ._private_utils import default_callback, validate_common_args, remap_scene_args, unsafe_figure_update_wrapper
 from ..deephaven_figure import generate_figure, DeephavenFigure
-from ..preprocess import preprocess_ecdf, create_hist_tables, preprocess_violin
 
 
-def violin(
+def scatter(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
+        error_x: str | list[str] = None,
+        error_x_minus: str | list[str] = None,
+        error_y: str | list[str] = None,
+        error_y_minus: str | list[str] = None,
+        size: str | list[str] = None,
+        # labels: dict[str, str] = None
         color_discrete_sequence: list[str] = None,
-        violinmode: str = 'group',
-        log_x: bool = False,
-        log_y: bool = False,
-        range_x: list[int] = None,
-        range_y: list[int] = None,
-        points: bool | str = 'outliers',
-        box: bool = False,
+        symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
+        xaxis_sequence: list[int] = None,
+        yaxis_sequence: list[int] = None,
+        opacity: float = None,
+        marginal_x: str = None,
+        marginal_y: str = None,
+        log_x: bool | list[bool] = False,
+        log_y: bool | list[bool] = False,
+        range_x: list[int] | list[list[int]] = None,
+        range_y: list[int] | list[list[int]] = None,
+        yaxis_titles: list[str] = None,
+        xaxis_titles: list[str] = None,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
-    Returns a violin chart
+    Returns a scatter chart
 
     :param table: A table to pull data from.
-    :param x: A column name or list of columns that contain x-axis values.
-    Only one of x or y can be specified. If x is specified, the violins are
-    drawn horizontally.
-    :param y: A column name or list of columns that contain y-axis values.
-    Only one of x or y can be specified. If y is specified, the violins are
-    drawn vertically.
+    :param x: A column or list of columns that contain x-axis values.
+    :param y: A column or list of columns that contain y-axis values.
+    :param error_x: A column or list of columns with x error bar
+    values. These form the error bars in both the positive and negative
+    direction if error_x_minus is not specified, and the error bars in only the
+    positive direction if error_x_minus is specified. None can be used to
+    specify no error bars on the corresponding series.
+    :param error_x_minus: A column or list of columns with x error
+    bar values. These form the error bars in the negative direction, and are
+    ignored if error_x is not specified.
+    :param size: A column or list of columns that contain size values.
+    :param error_y: A column or list of columns with x error bar
+    values. These form the error bars in both the positive and negative
+    direction if error_y_minus is not specified, and the error bars in only the
+    positive direction if error_y_minus is specified. None can be used to
+    specify no error bars on the corresponding series.
+    :param error_y_minus: A column or list of columns with x error
+    bar values. These form the error bars in the negative direction, and are
+    ignored if error_y is not specified.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
-    :param violinmode: Default 'group', which draws the violins next
-    to each other and 'overlay' which draws them on top of each other.
-    :param log_x: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param log_y: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param range_x: A list of two numbers that specify the range of the x axis.
-    :param range_y: A list of two numbers that specify the range of the y axis.
-    :param points: Default 'outliers', which draws points outside the whiskers.
-    'suspectedoutliers' draws points below 4*Q1-3*Q3 and above 4*Q3-3*Q1.
-    'all' draws all points and False draws no points.
-    :param box: Default False. Draw boxes inside the violin if True.
+    :param symbol_sequence: A list of symbols to sequentially apply to the
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
+    :param xaxis_sequence: A list of x axes to assign series to. Odd numbers
+    starting with 1 are created on the bottom x axis and even numbers starting
+    with 2 are created on the top x axis. Axes are created up
+    to the maximum number specified. The axes loop, so if there are more series
+    than axes, axes will be reused.
+    :param yaxis_sequence: A list of y axes to assign series to. Odd numbers
+    starting with 1 are created on the left y axis and even numbers starting
+    with 2 are created on the top y axis. Axes are created up
+    to the maximum number specified. The axes loop, so if there are more series
+    than axes, axes will be reused.
+    :param opacity: Opacity to apply to all points. 0 is completely transparent
+    and 1 is completely opaque.
+    :param marginal_x: The type of x-axis marginal; histogram, violin, rug, box
+    :param marginal_y: The type of y-axis marginal; histogram, violin, rug, box
+    :param log_x: Default False. A boolean or list of booleans that specify if
+    the corresponding axis is a log axis or not. The booleans loop, so if there
+    are more series than booleans, booleans will be reused.
+    :param log_y: Default False. A boolean or list of booleans that specify if
+    the corresponding axis is a log axis or not. The booleans loop, so if there
+    are more series than booleans, booleans will be reused.
+    :param range_x: A list of two numbers or a list of lists of two numbers
+    that specify the range of the x axes. None can be specified for no range
+    The ranges loop, so if there are more axes than ranges, ranges will
+    be reused.
+    :param range_y: A list of two numbers or a list of lists of two numbers
+    that specify the range of the x axes. None can be specified for no range
+    The ranges loop, so if there are more axes than ranges, ranges will
+    be reused.
+    :param yaxis_titles: A list of titles to sequentially apply to the
+    y axes. The titles do not loop.
+    :param xaxis_titles: A list of titles to sequentially apply to the
+    x axes. The titles do not loop.
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
-    :return: A DeephavenFigure that contains the violin chart
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
+    :return: A DeephavenFigure that contains the scatter chart
     """
-    if x and y:
-        raise ValueError("Cannot specify both x and y")
-
+    render_mode = "webgl"
     args = locals()
-    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
     validate_common_args(args)
 
-    create_layered = partial(preprocess_and_layer,
-                             preprocess_violin,
-                             px.violin, args,
-                             list_val_axis_name="value")
+    marg_data, marg_style = get_marg_args(args)
+    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
+
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
 
-    return create_layered("x") if x else create_layered("y")
+    return update_wrapper(
+        attach_marginals(
+            generate_figure(draw=px.scatter, call_args=args),
+            marg_data,
+            marg_style,
+            marginal_x=marginal_x, marginal_y=marginal_y,
+        )
+    )
 
 
-def box(
+def scatter_3d(
         table: Table = None,
-        x: str | list[str] = None,
-        y: str | list[str] = None,
+        x: str = None,
+        y: str = None,
+        z: str = None,
+        error_x: str | list[str] = None,
+        error_x_minus: str | list[str] = None,
+        error_y: str | list[str] = None,
+        error_y_minus: str | list[str] = None,
+        error_z: str | list[str] = None,
+        error_z_minus: str | list[str] = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
-        boxmode: str = 'group',
+        symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
+        opacity: float = None,
         log_x: bool = False,
         log_y: bool = False,
+        log_z: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
-        points: bool | str = 'outliers',
-        notched: bool = False,
+        range_z: list[int] = None,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
-    Returns a box chart
+    Returns a 3D scatter chart
 
     :param table: A table to pull data from.
-    :param x: A column name or list of columns that contain x-axis values.
-    Only one of x or y can be specified. If x is specified, the violins are
-    drawn horizontally.
-    :param y: A column name or list of columns that contain y-axis values.
-    Only one of x or y can be specified. If y is specified, the violins are
-    drawn vertically.
+    :param x: A column that contains x-axis values.
+    :param y: A column that contains y-axis values.
+    :param z: A column that contains z-axis values.
+    :param error_x: A column with x error bar values. These form the error
+    bars in both the positive and negative direction if error_x_minus is not
+    specified, and the error bars in only the positive direction if
+    error_x_minus is specified.
+    :param error_x_minus: A column with x error bar values. These form
+    the error bars in the negative direction, and are ignored if error_x is not
+    specified.
+    :param error_y: A column with x error bar values. These form the error
+    bars in both the positive and negative direction if error_z_minus is not
+    specified, and the error bars in only the positive direction if
+    error_x_minus is specified.
+    :param error_y_minus: A column with y error bar values. These form
+    the error bars in the negative direction, and are ignored if error_x is not
+    specified.
+    :param error_z: A column with x error bar values. These form the error
+    bars in both the positive and negative direction if error_z_minus is not
+    specified, and the error bars in only the positive direction if
+    error_x_minus is specified.
+    :param error_z_minus: A column with z error bar values. These form
+    the error bars in the negative direction, and are ignored if error_x is not
+    specified.
+    :param size: A column or list of columns that contain size values.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
-    :param boxmode: Default 'group', which draws the violins next
-    to each other and 'overlay' which draws them on top of each other.
+    :param symbol_sequence: A list of symbols to sequentially apply to the
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
+    :param opacity: Opacity to apply to all points. 0 is completely transparent
+    and 1 is completely opaque.
     :param log_x: A boolean that specifies if the corresponding axis is a log
     axis or not.
     :param log_y: A boolean that specifies if the corresponding axis is a log
     axis or not.
+    :param log_z: A boolean that specifies if the corresponding axis is a log
+    axis or not.
     :param range_x: A list of two numbers that specify the range of the x axis.
     :param range_y: A list of two numbers that specify the range of the y axis.
-    :param points: Default 'outliers', which draws points outside the whiskers.
-    'suspectedoutliers' draws points below 4*Q1-3*Q3 and above 4*Q3-3*Q1.
-    'all' draws all points and False draws no points.
-    :param notched: Default False, if True boxes are drawn with notches
-    :param title: The title of the chart
+    :param range_z: A list of two numbers that specify the range of the z axis.
+    :param title: The title of the chart.
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
-    :return: A DeephavenFigure that contains the box chart
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
+    :return: A DeephavenFigure that contains the 3D scatter chart
     """
-    if x and y:
-        raise ValueError("Cannot specify both x and y")
-
     args = locals()
-    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
     validate_common_args(args)
 
-    create_layered = partial(preprocess_and_layer,
-                             preprocess_violin,
-                             px.box, args,
-                             list_val_axis_name="value")
+    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
+
+    remap_scene_args(args)
+
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
 
-    return create_layered("x") if x else create_layered("y")
+    return update_wrapper(
+        generate_figure(draw=px.scatter_3d, call_args=args)
+    )
 
 
-def strip(
+def scatter_polar(
         table: Table = None,
-        x: str | list[str] = None,
-        y: str | list[str] = None,
+        r: str = None,
+        theta: str = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
-        stripmode: bool | str = 'group',
-        log_x: bool = False,
-        log_y: bool = False,
-        range_x: list[int] = None,
-        range_y: list[int] = None,
+        symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
+        opacity: float = None,
+        direction: str = 'clockwise',
+        start_angle: int = 90,
+        range_r: list[int] = None,
+        range_theta: list[int] = None,
+        log_r: bool = False,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
-    Returns a strip chart
+    Returns a polar scatter chart
 
     :param table: A table to pull data from.
-    :param x: A column name or list of columns that contain x-axis values.
-    Only one of x or y can be specified. If x is specified, the violins are
-    drawn horizontally.
-    :param y: A column name or list of columns that contain y-axis values.
-    Only one of x or y can be specified. If y is specified, the violins are
-    drawn vertically.
+    :param r: A column that contains r values.
+    :param theta: A column that contains theta values.
+    :param size: A column or list of columns that contain size values.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
-    :param stripmode: Default 'group', which draws the violins next
-    to each other and 'overlay' which draws them on top of each other.
-    :param log_x: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param log_y: A boolean that specifies if the corresponding axis is a log
+    :param symbol_sequence: A list of symbols to sequentially apply to the
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
+    :param opacity: Opacity to apply to all points. 0 is completely transparent
+    and 1 is completely opaque.
+    :param direction: Which direction points are drawn. Default clockwise.
+    :param start_angle: Sets start angle. Default 90.
+    :param range_r: A list of two numbers that specify the range of r.
+    :param range_theta: A list of two numbers that specify the range of theta.
+    :param log_r: A boolean that specifies if the corresponding axis is a log
     axis or not.
-    :param range_x: A list of two numbers that specify the range of the x axis.
-    :param range_y: A list of two numbers that specify the range of the y axis.
-    :param title: The title of the chart
+    :param title: The title of the chart.
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
-    :return: A DeephavenFigure that contains the strip chart
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
+    :return: A DeephavenFigure that contains the polar scatter chart
     """
-    if x and y:
-        raise ValueError("Cannot specify both x and y")
-
-    args = locals()
-    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
-
-    validate_common_args(args)
-
-    create_layered = partial(preprocess_and_layer,
-                             preprocess_violin,
-                             px.strip, args,
-                             list_val_axis_name="value")
-
-    return create_layered("x") if x else create_layered("y")
-
-
-def _ecdf(
-        table: Table = None,
-        x: str | list[str] = None,
-        y: str | list[str] = None,
-        markers: bool = False,
-        lines: bool = True,
-        color_discrete_sequence: list[str] = None,
-        line_dash_sequence: list[str] = None,
-        symbol_sequence: list[str] = None,
-        opacity: float = None,
-        ecdfnorm: str = 'probability',
-        ecdfmode: str = 'standard',
-        log_x: bool = False,
-        log_y: bool = False,
-        range_x: list[int] = None,
-        range_y: list[int] = None,
-        title: str = None,
-        template: str = None,
-        callback: Callable = default_callback
-) -> DeephavenFigure:
-    line_shape = "hv"
-    # rangemode = "tozero"
-
+    render_mode = "webgl"
     args = locals()
 
     validate_common_args(args)
 
     args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
-    args.pop("lines")
-    args.pop("ecdfnorm")
-    args.pop("ecdfmode")
-
-    create_layered = partial(preprocess_and_layer,
-                             preprocess_ecdf,
-                             px.line, args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
 
-    return create_layered("x") if x else create_layered("y", orientation="h")
+    return update_wrapper(
+        generate_figure(draw=px.scatter_polar, call_args=args)
+    )
 
 
-def histogram(
+def scatter_ternary(
         table: Table = None,
-        x: str | list[str] = None,
-        y: str | list[str] = None,
+        a: str = None,
+        b: str = None,
+        c: str = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
-        pattern_shape_sequence: list[str] = None,
+        symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
         opacity: float = None,
-        barmode: str = 'relative',
-        # barnorm: str = None,
-        # histnorm: str = None,
-        log_x: bool = False,
-        log_y: bool = False,
-        range_x: list[int] = None,
-        range_y: list[int] = None,
-        range_bins: list[int] = None,
-        histfunc: str = 'count',
-        # cumulative: bool = False,
-        nbins: int = 10,
-        text_auto: bool | str = False,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
-    Returns a histogram
+    Returns a ternary scatter chart
 
     :param table: A table to pull data from.
-    :param x: A column name or list of columns that contain x-axis values.
-    Only one of x or y can be specified. If x is specified, the bars are drawn
-    vertically.
-    :param y: A column name or list of columns that contain y-axis values.
-    Only one of x or y can be specified. If x is specified, the bars are drawn
-    horizontally.
+    :param a: A column that contains a-axis values.
+    :param b: A column that contains b-axis values.
+    :param c: A column that contains c-axis values.
+    :param size: A column or list of columns that contain size values.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
-    :param pattern_shape_sequence: A list of patterns to sequentially apply
-    to the series. The patterns loop, so if there are more series than
-    patterns, patterns will be reused.
+    :param symbol_sequence: A list of symbols to sequentially apply to the
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
     :param opacity: Opacity to apply to all points. 0 is completely transparent
     and 1 is completely opaque.
-    :param barmode: Default 'relative'. If 'relative', bars are stacked. If
-    'overlay', bars are drawn on top of each other. If 'group', bars are drawn
-    next to each other.
-    :param log_x: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param log_y: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param range_x: A list of two numbers that specify the range of the x axis.
-    :param range_y: A list of two numbers that specify the range of the y axis.
-    :param range_bins: A list of two numbers that specify the range of data
-    that is used.
-    :param histfunc: The function to use when aggregating within bins. One of
-    'avg', 'count', 'count_distinct', 'max', 'median', 'min', 'std', 'sum',
-    or 'var'
-    :param nbins: Default 10. The number of bins to use.
-    :param text_auto: Default False. If True, display the value at each bar.
-    If a string, specifies a plotly texttemplate.
-    :param title: The title of the chart
+    :param title: The title of the chart.
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
-    :return: A DeephavenFigure that contains the histogram
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
+    :return: A DeephavenFigure that contains the ternary scatter chart
     """
-    bargap = 0
     args = locals()
     validate_common_args(args)
 
-    # remove arguments not used in bar
-    args.pop("nbins")
-    args.pop("histfunc")
-    args.pop("range_bins")
-
     args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
-    args["pattern_shape_sequence_bar"] = args.pop("pattern_shape_sequence")
 
-    preprocessor = partial(
-        create_hist_tables,
-        nbins=nbins,
-        range_bins=range_bins,
-        histfunc=histfunc
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
     )
 
-    create_layered = partial(
-        preprocess_and_layer,
-        preprocessor, px.bar, args,
-        str_val_axis_name=histfunc,
-        list_val_axis_name=histfunc,
-        skip_layer=True,
+    return update_wrapper(
+        generate_figure(draw=px.scatter_ternary, call_args=args)
     )
 
-    return create_layered("x") if x else create_layered("y", orientation="h")
+
+def _scatter_matrix():
+    # todo: not yet implemented
+    pass
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/financial.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/financial.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from functools import partial
 from typing import Callable
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args
+from ._private_utils import default_callback, validate_common_args, unsafe_figure_update_wrapper
 from ..deephaven_figure import generate_figure, draw_ohlc, draw_candlestick, DeephavenFigure
 
 
 def ohlc(
         table: Table = None,
         x: str = None,
         open: str = None,
         high: str = None,
         low: str = None,
         close: str = None,
         increasing_color_sequence: list[str] = None,
         decreasing_color_sequence: list[str] = None,
         xaxis_sequence: list[int] = None,
         yaxis_sequence: list[int] = None,
-        yaxis_title_sequence: list[str] = None,
-        xaxis_title_sequence: list[str] = None,
-        callback: Callable = default_callback
+        yaxis_titles: list[str] = None,
+        xaxis_titles: list[str] = None,
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns an ohlc chart
 
     :param table: A table to pull data from.
     :param x: The column containing x-axis data
     :param open: The column containing the open data
@@ -42,48 +43,58 @@
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
     :param yaxis_sequence: A list of y axes to assign series to. Odd numbers
     starting with 1 are created on the left y axis and even numbers starting
     with 2 are created on the top y axis. Axes are created up
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
-    :param yaxis_title_sequence: A list of titles to sequentially apply to the
+    :param yaxis_titles: A list of titles to sequentially apply to the
     y axes. The titles do not loop.
-    :param xaxis_title_sequence: A list of titles to sequentially apply to the
+    :param xaxis_titles: A list of titles to sequentially apply to the
     x axes. The titles do not loop.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the ohlc chart
     """
 
     # todo: range slider
     #   fig.update(layout_xaxis_rangeslider_visible=False)
     args = locals()
     args["x_finance"] = args.pop("x")
 
     validate_common_args(args)
 
-    return generate_figure(draw=draw_ohlc, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=draw_ohlc, call_args=args)
+    )
 
 
 def candlestick(
         table: Table = None,
         x: str = None,
         open: str = None,
         high: str = None,
         low: str = None,
         close: str = None,
         increasing_color_sequence: list[str] = None,
         decreasing_color_sequence: list[str] = None,
         xaxis_sequence: list[int] = None,
         yaxis_sequence: list[int] = None,
-        yaxis_title_sequence: list[str] = None,
-        xaxis_title_sequence: list[str] = None,
-        callback: Callable = default_callback
+        yaxis_titles: list[str] = None,
+        xaxis_titles: list[str] = None,
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a candlestick chart
 
     :param table: A table to pull data from.
     :param x: The column containing x-axis data
     :param open: The column containing the open data
@@ -102,22 +113,33 @@
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
     :param yaxis_sequence: A list of y axes to assign series to. Odd numbers
     starting with 1 are created on the left y axis and even numbers starting
     with 2 are created on the top y axis. Axes are created up
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
-    :param yaxis_title_sequence: A list of titles to sequentially apply to the
+    :param yaxis_titles: A list of titles to sequentially apply to the
     y axes. The titles do not loop.
-    :param xaxis_title_sequence: A list of titles to sequentially apply to the
+    :param xaxis_titles: A list of titles to sequentially apply to the
     x axes. The titles do not loop.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the candlestick chart
     """
     args = locals()
-    args["x_finance"] = args.pop("x")
 
     validate_common_args(args)
 
-    return generate_figure(draw=draw_candlestick, call_args=args)
+    args["x_finance"] = args.pop("x")
+
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=draw_candlestick, call_args=args)
+    )
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/hierarchial.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/hierarchial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from functools import partial
 from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args
+from ._private_utils import default_callback, validate_common_args, unsafe_figure_update_wrapper
 from ..deephaven_figure import generate_figure, DeephavenFigure
 from ..preprocess import preprocess_aggregate
 
 
 def treemap(
         table: Table = None,
         names: str = None,
@@ -16,15 +17,15 @@
         parents: str = None,
         ids: str = None,
         # path: str = None,
         title: str = None,
         template: str = None,
         branchvalues: str = None,
         maxdepth: int = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ):
     """
     Returns a treemap chart
 
     :param table: A table to pull data from.
     :param names: The column containing names of the sections
     :param values: The column containing values of the sections
@@ -33,38 +34,48 @@
     must be unique. Values are used for ids if ids are not specified.
     :param title: The title of the chart
     :param template: The template for the chart.
     :param branchvalues: Set to 'total' to take the value at a level to include
     all descendants and 'remainder' to the value as the remainder after
     subtracting leaf values.
     :param maxdepth: Sets the total number of visible levels. Set to -1 to
-     render all levels.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    render all levels.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the treemap chart
     """
     args = locals()
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.treemap, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.treemap, call_args=args)
+    )
 
 
 def sunburst(
         table: Table = None,
         names: str = None,
         values: str = None,
         parents: str = None,
         ids: str = None,
         title: str = None,
         template: str = None,
         branchvalues: str = None,
         maxdepth: int = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ):
     """
     Returns a sunburst chart
 
     :param table: A table to pull data from.
     :param names: The column containing names of the sections
     :param values: The column containing values of the sections
@@ -73,38 +84,48 @@
     must be unique. Values are used for ids if ids are not specified.
     :param title: The title of the chart
     :param template: The template for the chart.
     :param branchvalues: Set to 'total' to take the value at a level to include
     all descendants and 'remainder' to the value as the remainder after
     subtracting leaf values.
     :param maxdepth: Sets the total number of visible levels. Set to -1 to
-     render all levels.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    render all levels.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the sunburst chart
     """
     args = locals()
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.sunburst, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.sunburst, call_args=args)
+    )
 
 
 def icicle(
         table: Table = None,
         names: str = None,
         values: str = None,
         parents: str = None,
         ids: str = None,
         title: str = None,
         template: str = None,
         branchvalues: str = None,
         maxdepth: int = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ):
     """
     Returns a icicle chart
 
     :param table: A table to pull data from.
     :param names: The column containing names of the sections
     :param values: The column containing values of the sections
@@ -113,25 +134,35 @@
     must be unique. Values are used for ids if ids are not specified.
     :param title: The title of the chart
     :param template: The template for the chart.
     :param branchvalues: Set to 'total' to take the value at a level to include
     all descendants and 'remainder' to the value as the remainder after
     subtracting leaf values.
     :param maxdepth: Sets the total number of visible levels. Set to -1 to
-     render all levels.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    render all levels.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the icicle chart
     """
     args = locals()
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.icicle, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.icicle, call_args=args)
+    )
 
 
 def funnel(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
@@ -139,15 +170,15 @@
         orientation: str = None,
         log_x: bool = False,
         log_y: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a funnel chart
 
     :param table: A table to pull data from.
     :param x: A column that contains x-axis values.
     :param y: A column that contains y-axis values.
@@ -161,36 +192,46 @@
     axis or not.
     :param log_y: A boolean that specifies if the corresponding axis is a log
     axis or not.
     :param range_x: A list of two numbers that specify the range of the x axis.
     :param range_y: A list of two numbers that specify the range of the y axis.
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the funnel chart
     """
     args = locals()
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.funnel, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.funnel, call_args=args)
+    )
 
 
 def funnel_area(
         table: Table = None,
         names: str = None,
         values: str = None,
         color_discrete_sequence: list[str] = None,
         title: str = None,
         template: str = None,
         opacity: float = None,
         aggregate: bool = True,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ):
     """
     Returns a funnel area chart
 
     :param table: A table to pull data from.
     :param names: The column containing names of the pie slices
     :param values: The column containing values of the pie slices
@@ -199,25 +240,35 @@
     colors will be reused.
     :param title: The title of the chart
     :param template: The template for the chart.
     :param opacity: Opacity to apply to all points. 0 is completely transparent
     and 1 is completely opaque.
     :param aggregate: Default True, aggregate the table names by total values. Can
     be set to False if the table is already aggregated by name.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the funnel area chart
     """
 
     args = locals()
 
     validate_common_args(args)
 
     if aggregate:
         args["table"] = preprocess_aggregate(table, names, values)
 
     args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
     args.pop("aggregate")
 
-    return generate_figure(draw=px.funnel_area, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.funnel_area, call_args=args)
+    )
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/line.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/line.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,45 @@
+from functools import partial
 from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args, remap_scene_args
+from ._private_utils import default_callback, validate_common_args, remap_scene_args, unsafe_figure_update_wrapper
 from ..deephaven_figure import generate_figure, DeephavenFigure
 
 
 # TODO: support line_shape as a list?
 def line(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
         error_x: str | list[str] = None,
         error_x_minus: str | list[str] = None,
         error_y: str | list[str] = None,
         error_y_minus: str | list[str] = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
         line_dash_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
         xaxis_sequence: list[str] = None,
         yaxis_sequence: list[str] = None,
-        yaxis_title_sequence: list[str] = None,
-        xaxis_title_sequence: list[str] = None,
         markers: bool = False,
         log_x: bool | list[bool] = False,
         log_y: bool | list[bool] = False,
         range_x: list[int] | list[list[int]] = None,
         range_y: list[int] | list[list[int]] = None,
+        yaxis_titles: list[str] = None,
+        xaxis_titles: list[str] = None,
         line_shape: str = 'linear',
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a line chart
 
     :param table: A table to pull data from.
     :param x: A column or list of columns that contain x-axis values.
     :param y: A column or list of columns that contain y-axis values.
@@ -52,93 +55,110 @@
     values. These form the error bars in both the positive and negative
     direction if error_y_minus is not specified, and the error bars in only the
     positive direction if error_y_minus is specified. None can be used to
     specify no error bars on the corresponding series.
     :param error_y_minus: A column or list of columns with x error
     bar values. These form the error bars in the negative direction, and are
     ignored if error_y is not specified.
+    :param size: A column or list of columns that contain size values.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
     :param line_dash_sequence: A list of line dashes to sequentially apply to
     the series. The dashes loop, so if there are more series than dashes,
     dashes will be reused.
     :param symbol_sequence: A list of symbols to sequentially apply to the
-    series. The symbols loop, so if there are more series than symbols, symbols
-    will be reused.
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
     :param xaxis_sequence: A list of x axes to assign series to. Odd numbers
     starting with 1 are created on the bottom x axis and even numbers starting
     with 2 are created on the top x axis. Axes are created up
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
     :param yaxis_sequence: A list of y axes to assign series to. Odd numbers
     starting with 1 are created on the left y axis and even numbers starting
     with 2 are created on the top y axis. Axes are created up
     to the maximum number specified. The axes loop, so if there are more series
     than axes, axes will be reused.
-    :param yaxis_title_sequence: A list of titles to sequentially apply to the
-    y axes. The titles do not loop.
-    :param xaxis_title_sequence: A list of titles to sequentially apply to the
-    x axes. The titles do not loop.
     :param markers: True to draw markers on the line, False to not. Default
     False
     :param log_x: Default False. A boolean or list of booleans that specify if
     the corresponding axis is a log axis or not. The booleans loop, so if there
     are more series than booleans, booleans will be reused.
     :param log_y: Default False. A boolean or list of booleans that specify if
     the corresponding axis is a log axis or not. The booleans loop, so if there
     are more series than booleans, booleans will be reused.
     :param range_x: A list of two numbers or a list of lists of two numbers
     that specify the range of the x axes. None can be specified for no range
     The ranges loop, so if there are more axes than ranges, ranges will
     be reused.
     :param range_y: A list of two numbers or a list of lists of two numbers
-     that specify the range of the x axes. None can be specified for no range
+    that specify the range of the x axes. None can be specified for no range
     The ranges loop, so if there are more axes than ranges, ranges will
     be reused.
+    :param yaxis_titles: A list of titles to sequentially apply to the
+    y axes. The titles do not loop.
+    :param xaxis_titles: A list of titles to sequentially apply to the
+    x axes. The titles do not loop.
     :param line_shape: The line shape for all lines created. One of 'linear',
     'spline', 'vhv', 'hvh', 'vh', 'hv'. Default 'linear'
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the line chart
     """
     args = locals()
-    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.line, call_args=args)
+    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
+
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.line, call_args=args)
+    )
 
 
 def line_3d(
         table: Table = None,
         x: str = None,
         y: str = None,
         z: str = None,
         error_x: str | list[str] = None,
         error_x_minus: str | list[str] = None,
         error_y: str | list[str] = None,
         error_y_minus: str | list[str] = None,
         error_z: str | list[str] = None,
         error_z_minus: str | list[str] = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
         markers: bool = False,
         log_x: bool = False,
         log_y: bool = False,
         log_z: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
         range_z: list[int] = None,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a 3D line chart
 
     :param table: A table to pull data from.
     :param x: A column that contains x-axis values.
     :param y: A column that contains y-axis values.
@@ -146,14 +166,15 @@
     :param error_x: A column with x error bar values. These form the error
     bars in both the positive and negative direction if error_x_minus is not
     specified, and the error bars in only the positive direction if
     error_x_minus is specified.
     :param error_x_minus: A column with x error bar values. These form
     the error bars in the negative direction, and are ignored if error_x is not
     specified.
+    :param size: A column or list of columns that contain size values.
     :param error_y: A column with x error bar values. These form the error
     bars in both the positive and negative direction if error_z_minus is not
     specified, and the error bars in only the positive direction if
     error_x_minus is specified.
     :param error_y_minus: A column with y error bar values. These form
     the error bars in the negative direction, and are ignored if error_x is not
     specified.
@@ -164,137 +185,184 @@
     :param error_z_minus: A column with z error bar values. These form
     the error bars in the negative direction, and are ignored if error_x is not
     specified.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
     :param symbol_sequence: A list of symbols to sequentially apply to the
-    series. The symbols loop, so if there are more series than symbols, symbols
-    will be reused.
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
     :param markers: True to draw markers on the line, False to not. Default
     False
     :param log_x: A boolean that specifies if the corresponding axis is a log
     axis or not.
     :param log_y: A boolean that specifies if the corresponding axis is a log
     axis or not.
     :param log_z: A boolean that specifies if the corresponding axis is a log
     axis or not.
     :param range_x: A list of two numbers that specify the range of the x axis.
     :param range_y: A list of two numbers that specify the range of the y axis.
     :param range_z: A list of two numbers that specify the range of the z axis.
     :param title: The title of the chart.
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the 3D line chart
     """
     args = locals()
+
+    validate_common_args(args)
+
     args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
 
     remap_scene_args(args)
 
-    validate_common_args(args)
-
-    return generate_figure(draw=px.line_3d, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.line_3d, call_args=args)
+    )
 
 
 def line_polar(
         table: Table = None,
         r: str = None,
         theta: str = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
         markers: bool = False,
         direction: str = 'clockwise',
         start_angle: int = 90,
         line_close: bool = False,
         line_shape: str = 'linear',
         range_r: list[int] = None,
         range_theta: list[int] = None,
         log_r: bool = False,
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback,
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a polar scatter chart
 
     :param table: A table to pull data from.
     :param r: A column that contains r values.
     :param theta: A column that contains theta values.
+    :param size: A column or list of columns that contain size values.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
     :param symbol_sequence: A list of symbols to sequentially apply to the
-    series. The symbols loop, so if there are more series than symbols, symbols
-    will be reused.
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
     :param markers: True to draw markers on the line, False to not. Default
     False
     :param direction: Which direction points are drawn. Default clockwise.
     :param start_angle: Sets start angle. Default 90.
     :param line_close: True draw a line between first and last point, False to
     not. Default False
     :param line_shape: The line shape for all lines created. One of 'linear',
     'spline'. Default 'linear'
     :param range_r: A list of two numbers that specify the range of r.
     :param range_theta: A list of two numbers that specify the range of theta.
     :param log_r: A boolean that specifies if the corresponding axis is a log
     axis or not.
     :param title: The title of the chart.
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the polar scatter chart
     """
     args = locals()
     args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.line_polar, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.line_polar, call_args=args)
+    )
 
 
 def line_ternary(
         table: Table = None,
         a: str = None,
         b: str = None,
         c: str = None,
+        size: str | list[str] = None,
         color_discrete_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
+        size_sequence: list[int] = None,
         markers: bool = False,
         line_shape: str = 'linear',
         title: str = None,
         template: str = None,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a ternary line chart
 
     :param table: A table to pull data from.
     :param a: A column that contains a-axis values.
     :param b: A column that contains b-axis values.
     :param c: A column that contains c-axis values.
+    :param size: A column or list of columns that contain size values.
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
     :param symbol_sequence: A list of symbols to sequentially apply to the
-    series. The symbols loop, so if there are more series than symbols, symbols
-    will be reused.
+    markers in the series. The symbols loop, so if there are more series than
+    symbols, symbols will be reused.
+    :param size_sequence: A list of sizes to sequentially apply to the
+    markers in the series. The sizes loop, so if there are more series than
+    symbols, sizes will be reused. This is overriden is "size" is specified.
     :param markers: True to draw markers on the line, False to not. Default
     False
     :param line_shape: The line shape for all lines created. One of 'linear',
     'spline'. Default 'linear'
     :param title: The title of the chart.
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the ternary line chart
     """
     args = locals()
-    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
 
     validate_common_args(args)
 
-    return generate_figure(draw=px.line_ternary, call_args=args)
+    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
+
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.line_ternary, call_args=args)
+    )
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/plots/pie.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/pie.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,65 @@
+from functools import partial
 from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args
+from ._private_utils import default_callback, validate_common_args, unsafe_figure_update_wrapper
 from ..deephaven_figure import generate_figure, DeephavenFigure
 from ..preprocess import preprocess_aggregate
 
 
 def pie(
         table: Table = None,
         names: str = None,
         values: str = None,
         color_discrete_sequence: list[str] = None,
         title: str = None,
         template: str = None,
         opacity: float = None,
         hole: float = None,
         aggregate: bool = True,
-        callback: Callable = default_callback
+        unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Returns a pie chart
 
     :param table: A table to pull data from.
     :param names: The column containing names of the pie slices
     :param values: The column containing values of the pie slices
     :param color_discrete_sequence: A list of colors to sequentially apply to
     the series. The colors loop, so if there are more series than colors,
     colors will be reused.
     :param title: The title of the chart
     :param template: The template for the chart.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
-    :param opacity: Opacity to apply to all points. 0 is completely transparent
-    and 1 is completely opaque.
     :param hole: Fraction of the radius to cut out of the center of the pie.
     :param aggregate: Default True, aggregate the table names by total values. Can
     be set to False if the table is already aggregated by name.
-    :param callback: A callback function that takes a figure as an argument and
-    returns a figure. Used to add any custom changes to the underlying plotly
-    figure. Note that the existing data traces should not be removed.
+    :param unsafe_update_figure: An update function that takes a plotly figure
+    as an argument and optionally returns a plotly figure. If a figure is not
+    returned, the plotly figure passed will be assumed to be the return value.
+    Used to add any custom changes to the underlying plotly figure. Note that
+    the existing data traces should not be removed. This may lead to unexpected
+    behavior if traces are modified in a way that break data mappings.
     :return: A DeephavenFigure that contains the pie chart
     """
     args = locals()
 
     validate_common_args(args)
 
     if aggregate:
         args["table"] = preprocess_aggregate(table, names, values)
 
     args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
     args.pop("aggregate")
 
-    return generate_figure(draw=px.pie, call_args=args)
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
+    )
+
+    return update_wrapper(
+        generate_figure(draw=px.pie, call_args=args)
+    )
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/preprocess/preprocess.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
     :param nbins: The number of bins, shared between all histograms
     :param range_bins: The range that the bins are drawn over. If none, the range
     will be over all data
     :param histfunc: The function to aggregate values within each bin
     :return: A tuple containing (the new counts table,
     the column of the midpoint, the columns that contain counts)
     """
+    columns = list(set(columns))
+
     range_table = create_range_table(table, columns, nbins, range_bins)
     bin_counts = new_table([
         long_col("RangeIndex", [i for i in range(nbins)])
     ])
 
     count_cols = []
 
@@ -217,32 +219,32 @@
                             f"{y}"])
     return new_table, "Time_Diff"
 
 
 def preprocess_violin(
         table: Table,
         column: str
-) -> tuple[Table, str, str]:
+) -> tuple[Table, str, None]:
     """
     Preprocess the violin (or box or strip) params into an appropriate table
     For each column, the data needs to be reshaped so that there is a column
-    that contains the column name, and a column that contains the value
+    that contains the column value.
 
     :param table: The table to pull data from
     :param column: The column to use for violin data
-    :return: A tuple of new_table, column names, and column values
+    :return: A tuple of new_table, column values, and None
     """
-    col_names, col_vals = "category", f"{column}",
     # also used for box and strip
     new_table = table.view([
-        f"{col_names} = `{column}`",
-        f"{col_vals} = {column}"
+        f"{column} = {column}"
     ])
-
-    return new_table, col_names, col_vals
+    # The names are None as a third tuple value is required for
+    # preprocess_and_layer but putting the names in the figure
+    # breaks violinmode=overlay
+    return new_table, column, None
 
 
 def preprocess_ecdf(
         table,
         column
 ):
     col_dup = f"{column}_2"
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven/plot/express/shared/shared.py` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/shared.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.1.dev1
+Version: 0.0.2
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.1.dev1/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt` & `deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt`

 * *Files identical despite different names*

