# Comparing `tmp/sbcoyote-1.4.0.tar.gz` & `tmp/sbcoyote-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbcoyote-1.4.0.tar", max compression
+gzip compressed data, was "sbcoyote-1.4.2.tar", max compression
```

## Comparing `sbcoyote-1.4.0.tar` & `sbcoyote-1.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.4.0/LICENSE
--rw-r--r--   0        0        0     1835 2023-04-17 19:01:31.262321 sbcoyote-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    10373 2023-04-07 19:29:33.141010 sbcoyote-1.4.0/README.md
--rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.4.0/rkviewer/__init__.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.4.0/rkviewer/canvas/__init__.py
--rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.4.0/rkviewer/canvas/canvas.py
--rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.4.0/rkviewer/canvas/data.py
--rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.4.0/rkviewer/canvas/elements.py
--rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.4.0/rkviewer/canvas/geometry.py
--rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.4.0/rkviewer/canvas/overlays.py
--rw-r--r--   0        0        0     1731 2021-09-10 21:55:36.695255 sbcoyote-1.4.0/rkviewer/canvas/state.py
--rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.4.0/rkviewer/canvas/utils.py
--rw-r--r--   0        0        0    18996 2023-04-11 18:08:06.351143 sbcoyote-1.4.0/rkviewer/config.py
--rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.4.0/rkviewer/controller.py
--rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.4.0/rkviewer/events.py
--rw-r--r--   0        0        0    98431 2023-04-14 18:57:17.020026 sbcoyote-1.4.0/rkviewer/forms.py
--rw-r--r--   0        0        0    94813 2023-04-12 23:20:38.517372 sbcoyote-1.4.0/rkviewer/iodine.py
--rw-r--r--   0        0        0     3329 2023-04-14 20:43:22.448825 sbcoyote-1.4.0/rkviewer/json/.default-settings.json
--rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.4.0/rkviewer/json/dark-settings.json
--rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.4.0/rkviewer/json/settings.json
--rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.4.0/rkviewer/main.py
--rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.4.0/rkviewer/mvc.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.4.0/rkviewer/plugin/__init__.py
--rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.4.0/rkviewer/plugin/api.py
--rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.4.0/rkviewer/plugin/canvas.py
--rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.4.0/rkviewer/plugin/classes.py
--rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.4.0/rkviewer/plugin/events.py
--rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.4.0/rkviewer/plugin_manage.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.4.0/rkviewer/resources/__init__.py
--rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.4.0/rkviewer/resources/AlignBottom_XP.png
--rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.4.0/rkviewer/resources/alignHorizCenter_XP.png
--rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.4.0/rkviewer/resources/alignHorizEqually_XP.png
--rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.4.0/rkviewer/resources/alignLeft_XP.png
--rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.4.0/rkviewer/resources/alignOnGrid_XP.png
--rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.4.0/rkviewer/resources/alignRight_XP.png
--rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.4.0/rkviewer/resources/alignTop_XP.png
--rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.4.0/rkviewer/resources/alignVertCenter_XP.png
--rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.4.0/rkviewer/resources/alignVertEqually_XP.png
--rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.4.0/rkviewer/resources/info-2-16.png
--rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.4.0/rkviewer/utils.py
--rw-r--r--   0        0        0    47660 2023-04-17 19:01:36.166032 sbcoyote-1.4.0/rkviewer/view.py
--rw-r--r--   0        0        0     8420 2023-04-10 20:09:02.114349 sbcoyote-1.4.0/rkviewer_plugins/addReaction.py
--rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.4.0/rkviewer_plugins/align_circle.py
--rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.4.0/rkviewer_plugins/arrow_designer.py
--rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.4.0/rkviewer_plugins/exportAntimony.py
--rw-r--r--   0        0        0    67844 2023-04-14 22:49:04.000455 sbcoyote-1.4.0/rkviewer_plugins/exportSBML.py
--rw-r--r--   0        0        0   154343 2023-04-17 17:29:27.368209 sbcoyote-1.4.0/rkviewer_plugins/importSBML.py
--rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.4.0/rkviewer_plugins/modelMetrics.py
--rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.4.0/rkviewer_plugins/networkX.py
--rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.4.0/rkviewer_plugins/randomNetwork.py
--rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.4.0/rkviewer_plugins/structuralAnalysis.py
--rw-r--r--   0        0        0    11928 1970-01-01 00:00:00.000000 sbcoyote-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1826 2023-05-02 21:40:04.275319 sbcoyote-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0    10368 2023-05-02 21:32:36.743811 sbcoyote-1.4.2/README.md
+-rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.4.2/rkviewer/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.4.2/rkviewer/canvas/__init__.py
+-rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.4.2/rkviewer/canvas/canvas.py
+-rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.4.2/rkviewer/canvas/data.py
+-rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.4.2/rkviewer/canvas/elements.py
+-rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.4.2/rkviewer/canvas/geometry.py
+-rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.4.2/rkviewer/canvas/overlays.py
+-rw-r--r--   0        0        0     1731 2021-09-10 21:55:36.695255 sbcoyote-1.4.2/rkviewer/canvas/state.py
+-rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.4.2/rkviewer/canvas/utils.py
+-rw-r--r--   0        0        0    18996 2023-04-11 18:08:06.351143 sbcoyote-1.4.2/rkviewer/config.py
+-rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.4.2/rkviewer/controller.py
+-rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.4.2/rkviewer/events.py
+-rw-r--r--   0        0        0    98431 2023-04-14 18:57:17.020026 sbcoyote-1.4.2/rkviewer/forms.py
+-rw-r--r--   0        0        0    94813 2023-04-12 23:20:38.517372 sbcoyote-1.4.2/rkviewer/iodine.py
+-rw-r--r--   0        0        0     3329 2023-04-14 20:43:22.448825 sbcoyote-1.4.2/rkviewer/json/.default-settings.json
+-rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.4.2/rkviewer/json/dark-settings.json
+-rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.4.2/rkviewer/json/settings.json
+-rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.4.2/rkviewer/main.py
+-rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.4.2/rkviewer/mvc.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.4.2/rkviewer/plugin/__init__.py
+-rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.4.2/rkviewer/plugin/api.py
+-rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.4.2/rkviewer/plugin/canvas.py
+-rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.4.2/rkviewer/plugin/classes.py
+-rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.4.2/rkviewer/plugin/events.py
+-rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.4.2/rkviewer/plugin_manage.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.4.2/rkviewer/resources/__init__.py
+-rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.4.2/rkviewer/resources/AlignBottom_XP.png
+-rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.4.2/rkviewer/resources/alignHorizCenter_XP.png
+-rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.4.2/rkviewer/resources/alignHorizEqually_XP.png
+-rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.4.2/rkviewer/resources/alignLeft_XP.png
+-rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.4.2/rkviewer/resources/alignOnGrid_XP.png
+-rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.4.2/rkviewer/resources/alignRight_XP.png
+-rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.4.2/rkviewer/resources/alignTop_XP.png
+-rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.4.2/rkviewer/resources/alignVertCenter_XP.png
+-rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.4.2/rkviewer/resources/alignVertEqually_XP.png
+-rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.4.2/rkviewer/resources/info-2-16.png
+-rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.4.2/rkviewer/utils.py
+-rw-r--r--   0        0        0    47660 2023-05-02 21:40:08.024102 sbcoyote-1.4.2/rkviewer/view.py
+-rw-r--r--   0        0        0     8420 2023-04-10 20:09:02.114349 sbcoyote-1.4.2/rkviewer_plugins/addReaction.py
+-rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.4.2/rkviewer_plugins/align_circle.py
+-rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.4.2/rkviewer_plugins/arrow_designer.py
+-rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.4.2/rkviewer_plugins/exportAntimony.py
+-rw-r--r--   0        0        0    70514 2023-05-02 17:16:00.570787 sbcoyote-1.4.2/rkviewer_plugins/exportSBML.py
+-rw-r--r--   0        0        0   156402 2023-05-02 21:09:10.632510 sbcoyote-1.4.2/rkviewer_plugins/importSBML.py
+-rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.4.2/rkviewer_plugins/modelMetrics.py
+-rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.4.2/rkviewer_plugins/networkX.py
+-rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.4.2/rkviewer_plugins/randomNetwork.py
+-rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.4.2/rkviewer_plugins/structuralAnalysis.py
+-rw-r--r--   0        0        0    11909 1970-01-01 00:00:00.000000 sbcoyote-1.4.2/PKG-INFO
```

### Comparing `sbcoyote-1.4.0/LICENSE` & `sbcoyote-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/pyproject.toml` & `sbcoyote-1.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SBcoyote"
-version = "1.4.0"
+version = "1.4.2"
 description = "SBcoyote: An Extensible Python Based Reaction Editor and Viewer."
 readme = "README.md"
 authors = ["Jin Xu and Gary Geng et al <jxu2019@uw.edu>"]
 packages = [
     #{ include = "*" }
     { include = "rkviewer"},
     { include = "rkviewer_plugins"},
@@ -16,37 +16,37 @@
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
 
     'Operating System :: Microsoft :: Windows',
     'Operating System :: MacOS',
     'Operating System :: POSIX :: Linux',
 
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 
     'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1, <3.11"
+python = ">=3.8, <3.11"
 wxPython = "^4.1.1"
 sortedcontainers = "^2.3.0"
 marshmallow = "^3.11.1"
 commentjson = "^0.9.0"
 dataclasses = { version = "^0.8", python = "~3.6" }
 marshmallow-polyfield = "^5.10"
 wheel = "*"
 requests = "*"
 traitlets = "*"
 networkx = { version = "^2.5.1" }
 simplesbml = { version = "^2.2.0"}
 python-libsbml = { version = "^5.18.0" }
 pandas = { version = "^1.3.0" }
+SBMLDiagrams = { version = ">=1.3.4"}
 tellurium = { version = "^2.2.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^3.5.4"
 sphinx-rtd-theme = "^0.5.2"
 sphinx-autodoc-typehints = "^1.12.0"
 pylint = "^2.8.2"
```

### Comparing `sbcoyote-1.4.0/README.md` & `sbcoyote-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ## Citing
 
 If you are using any of the code, please cite the article (https://arxiv.org/abs/2302.09151). 
 
 ## Installing SBcoyote
 
-* Install Python 3.7, 3.8, 3.9 or 3.10 if not already in the system.
+* Install Python 3.8, 3.9 or 3.10 if not already in the system.
 * Go to the command line and type `pip install SBcoyote`.
 * If wxPython doesn't get installed automatically, please try to install wxPython 4.1.1 or 4.2.0 manually referring to https://wxpython.org/pages/downloads/index.html. Note wxPython 4.1.1 does not work with Python 3.10. 
 * To run the application, simply type in the command line `SBcoyote`.
 
 ## Documentation
 
 The full documentation can be found at: https://sys-bio.github.io/SBcoyote/
```

### Comparing `sbcoyote-1.4.0/rkviewer/canvas/canvas.py` & `sbcoyote-1.4.2/rkviewer/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/canvas/data.py` & `sbcoyote-1.4.2/rkviewer/canvas/data.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/canvas/elements.py` & `sbcoyote-1.4.2/rkviewer/canvas/elements.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/canvas/geometry.py` & `sbcoyote-1.4.2/rkviewer/canvas/geometry.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/canvas/overlays.py` & `sbcoyote-1.4.2/rkviewer/canvas/overlays.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/canvas/state.py` & `sbcoyote-1.4.2/rkviewer/canvas/state.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/canvas/utils.py` & `sbcoyote-1.4.2/rkviewer/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/config.py` & `sbcoyote-1.4.2/rkviewer/config.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/controller.py` & `sbcoyote-1.4.2/rkviewer/controller.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/events.py` & `sbcoyote-1.4.2/rkviewer/events.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/forms.py` & `sbcoyote-1.4.2/rkviewer/forms.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/iodine.py` & `sbcoyote-1.4.2/rkviewer/iodine.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/json/.default-settings.json` & `sbcoyote-1.4.2/rkviewer/json/.default-settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/json/dark-settings.json` & `sbcoyote-1.4.2/rkviewer/json/dark-settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/json/settings.json` & `sbcoyote-1.4.2/rkviewer/json/settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/main.py` & `sbcoyote-1.4.2/rkviewer/main.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/mvc.py` & `sbcoyote-1.4.2/rkviewer/mvc.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/plugin/api.py` & `sbcoyote-1.4.2/rkviewer/plugin/api.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/plugin/canvas.py` & `sbcoyote-1.4.2/rkviewer/plugin/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/plugin/classes.py` & `sbcoyote-1.4.2/rkviewer/plugin/classes.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/plugin_manage.py` & `sbcoyote-1.4.2/rkviewer/plugin_manage.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/resources/alignRight_XP.png` & `sbcoyote-1.4.2/rkviewer/resources/alignRight_XP.png`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/utils.py` & `sbcoyote-1.4.2/rkviewer/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer/view.py` & `sbcoyote-1.4.2/rkviewer/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,15 +701,15 @@
         self.Bind(wx.EVT_MENU, callback, item)
         self.menu_events.append((callback, item))
         return item
 
     def onAboutDlg(self, event):
         info = wx.adv.AboutDialogInfo()
         info.SetName("SBcoyote")
-        info.SetVersion("1.4.0")
+        info.SetVersion("1.4.2")
         info.SetCopyright("(c) 2023 UW Sauro Lab")
         info.SetDescription("An Extensible Python-Based Reaction Editor and Viewer.")
         info.SetWebSite("https://github.com/sys-bio/SBcoyote",
                         "Home Page")  # TODO update home page?
         info.SetDevelopers(["Jin Xu", "Gary Geng", "Nhan D. Nguyen", "Carmen Perena-Corte","Claire Samuels", "Herbert M. Sauro"])# TODO update authors
         info.SetLicense("MIT")
```

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/addReaction.py` & `sbcoyote-1.4.2/rkviewer_plugins/addReaction.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/align_circle.py` & `sbcoyote-1.4.2/rkviewer_plugins/align_circle.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/arrow_designer.py` & `sbcoyote-1.4.2/rkviewer_plugins/arrow_designer.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/exportAntimony.py` & `sbcoyote-1.4.2/rkviewer_plugins/exportAntimony.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/exportSBML.py` & `sbcoyote-1.4.2/rkviewer_plugins/exportSBML.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Export the network on canvas to an SBML string as save it as a file.
-Version 1.0.7: Author: Jin Xu (2023)
+Version 1.0.8: Author: Jin Xu (2023)
 """
 
 
 # pylint: disable=maybe-no-member
 
 from inspect import Parameter
 import wx
@@ -17,15 +17,15 @@
 import re # to process kinetic_law string
 from rkviewer.config import get_theme
 
 class ExportSBML(WindowedPlugin):
     metadata = PluginMetadata(
         name='ExportSBML',
         author='Jin Xu',
-        version='1.0.7',
+        version='1.0.8',
         short_desc='Export SBML.',
         long_desc='Export the SBML String from the network on canvas and save it to a file.',
         category=PluginCategory.MODELS
     )
 
 
     def create_window(self, dialog):
@@ -189,15 +189,59 @@
             allNodes = api.get_nodes(netIn)
             
             allReactions = api.get_reactions(netIn)
             allcompartments = api.get_compartments(netIn)
             #print("allNodes:", allNodes)
             #print("allReactions:", allReactions)
             #print("allcompartments:", allcompartments)
-            numCompartments = len(allcompartments)      
+            numCompartments = len(allcompartments) 
+            #The following code calculates the size of the network
+            pos = [allNodes[0].position.x + 2.*allNodes[0].size.x, #double comes from the text position
+                    allNodes[0].position.y + 2.*allNodes[0].size.y]
+            for node in allNodes:
+                if (node.position.x + 2.*node.size.x) > pos[0]:
+                    pos[0] = node.position.x + 2.*node.size.x
+                if (node.position.y + 2.*node.size.y) > pos[1]:
+                    pos[1] = node.position.y + 2.*node.size.y
+            for comp in allcompartments:
+                if comp.id != "_compartment_default_":
+                    comp_fill_color = [comp.fill_color.r, comp.fill_color.g, comp.fill_color.b]
+                    comp_border_color = [comp.border_color.r, comp.border_color.g, comp.border_color.b]
+                    if comp_fill_color != [255, 255, 255] or comp_border_color != [255, 255, 255]:
+                        if (comp.position.x + comp.size.x) > pos[0]:
+                            pos[0] = comp.position.x + comp.size.x
+                        if (comp.position.y + comp.size.y) > pos[1]:
+                            pos[1] = comp.position.y + comp.size.y
+            for rxn in allReactions:
+                if rxn.center_pos.x > pos[0]:
+                    pos[0] = rxn.center_pos.x
+                if rxn.center_pos.y > pos[1]:
+                    pos[1] = rxn.center_pos.y
+                idx = rxn.index
+                handle_pos = api.get_reaction_center_handle(netIn, idx)
+                if handle_pos.x > pos[0]:
+                    pos[0] = handle_pos.x
+                if handle_pos.y > pos[1]:
+                    pos[1] = handle_pos.y
+                src = rxn.sources
+                tgt = rxn.targets
+                for i in range(len(src)):
+                    handle_pos = api.get_reaction_node_handle(netIn, idx, src[i],is_source=True)
+                    if handle_pos.x > pos[0]:
+                        pos[0] = handle_pos.x
+                    if handle_pos.y > pos[1]:
+                        pos[1] = handle_pos.y
+                for i in range(len(tgt)):
+                    handle_pos = api.get_reaction_node_handle(netIn, idx, tgt[i],is_source=False)
+                    if handle_pos.x > pos[0]:
+                        pos[0] = handle_pos.x
+                    if handle_pos.y > pos[1]:
+                        pos[1] = handle_pos.y    
+            cal_layout_size = [pos[0] + 100., pos[1] + 100.]
+            
     #######################################
 
             # Creates an SBMLNamespaces object with the given SBML level, version
             # package name, package version.
             # 
             # (NOTE) By default, the name of package (i.e. "layout") will be used
             # if the argument for the prefix is missing or empty. Thus the argument
@@ -253,15 +297,15 @@
                         species.setName(spec_name)
                         species.setSBOTerm(spec_SBO)
                         comp_idx = allNodes[i].comp_idx
                         if comp_idx != -1:
                             comp_id = allcompartments[comp_idx].id 
                             species.setCompartment(comp_id)  
                         else:
-                           species.setCompartment("_compartment_default_") #why "_compartment_default_"
+                            species.setCompartment("_compartment_default_") #why "_compartment_default_"
                         species.setInitialConcentration(allNodes[i].concentration)	
                         species.setHasOnlySubstanceUnits(False)
                         species.setBoundaryCondition(False)
                         species.setConstant(False)             
                         if allNodes[i].floating_node == False:
                             species.setBoundaryCondition(True)
                             species.setConstant(True)   
@@ -419,16 +463,21 @@
             #
             layout = mplugin.createLayout()
             layout.setId("SBcoyote_layout")
             def_canvas_width = get_theme('real_canvas_width')
             def_canvas_height = get_theme('real_canvas_height')
             #layout_width = 10000 - 20
             #layout_height = 6200 - 20
-            layout_width = def_canvas_width - 20.
-            layout_height = def_canvas_height - 20.
+            try:
+                layout_width = cal_layout_size[0]
+                layout_height = cal_layout_size[1]
+            except:
+                layout_width = def_canvas_width - 20.
+                layout_height = def_canvas_height - 20.
+
             layout.setDimensions(Dimensions(layoutns, layout_width, layout_height))
             # random network (40+800x, 40+800y)
 
             #create the CompartmentGlyph and SpeciesGlyphs
             if numCompartments != 0:
                 for i in range(numCompartments):   
                     comp_id=allcompartments[i].id
```

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/importSBML.py` & `sbcoyote-1.4.2/rkviewer_plugins/importSBML.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Import an SBML string from a file and visualize it to a network on canvas.
-Version 1.1.7: Author: Jin Xu (2023)
+Version 1.1.8: Author: Jin Xu (2023)
 """
 
 
 # pylint: disable=maybe-no-member
 
 from ast import Num
 from inspect import Parameter
@@ -19,20 +19,21 @@
 import os
 import simplesbml # does not have to import in the main.py too
 from libsbml import *
 import math
 import random as _random
 import pandas as pd
 from rkviewer.config import get_theme
+import SBMLDiagrams
 
 class IMPORTSBML(WindowedPlugin):
     metadata = PluginMetadata(
         name='ImportSBML',
         author='Jin Xu',
-        version='1.1.7',
+        version='1.1.8',
         short_desc='Import SBML.',
         long_desc='Import an SBML String from a file and visualize it as a network on canvas.',
         category=PluginCategory.MODELS
     )
 
     def create_window(self, dialog):
         """
@@ -198,16 +199,22 @@
                 #     if showDialogues:
                 #         wx.MessageBox("There is no layout information, so positions are randomly assigned.", "Message", wx.OK | wx.ICON_INFORMATION)
                 # else:
                 #def_canvas_width = 10000.
                 #def_canvas_height = 6200.
                 def_canvas_width = get_theme('real_canvas_width')
                 def_canvas_height = get_theme('real_canvas_height')
-                def_comp_width = def_canvas_width - 20.
-                def_comp_height = def_canvas_height - 20.
+                #def_comp_width = def_canvas_width - 20.
+                #def_comp_height = def_canvas_height - 20.
+                def_comp_width = SBMLDiagrams.load(sbmlStr).getNetworkBottomRightCorner().x + 100.
+                def_comp_height = SBMLDiagrams.load(sbmlStr).getNetworkBottomRightCorner().y + 100.
+                if SBMLDiagrams.load(sbmlStr).getNetworkTopLeftCorner().x < 0:
+                    def_comp_width -= SBMLDiagrams.load(sbmlStr).getNetworkTopLeftCorner().x
+                if SBMLDiagrams.load(sbmlStr).getNetworkTopLeftCorner().y < 0:
+                    def_comp_height -= SBMLDiagrams.load(sbmlStr).getNetworkTopLeftCorner().y
                 if mplugin is not None:
                     layout = mplugin.getLayout(0)
                     # if layout is None:
                     #     if showDialogues:
                     #         wx.MessageBox("There is no layout information, so positions are randomly assigned.", "Message", wx.OK | wx.ICON_INFORMATION)
                     # else:
                     try:
@@ -356,15 +363,15 @@
 
                             #rct_specGlyph_temp_list = []
                             #prd_specGlyph_temp_list = []
                             rct_specGlyph_handles_temp_list = []
                             prd_specGlyph_handles_temp_list = []  
                             mod_specGlyph_temp_list = []
 
-                            center_handle = []
+                            center_handle = [[],[]]
 
                             for j in range(numSpecRefGlyphs):
                                 alignment_name = TextAlignment.CENTER
                                 position_name = TextPosition.IN_NODE
                                 specRefGlyph = reactionGlyph.getSpeciesReferenceGlyph(j)
                                 specRefGlyph_id = specRefGlyph.getId()
                                 curve = specRefGlyph.getCurve() 
@@ -573,27 +580,32 @@
                                     spec_text_alignment_list.append(alignment_name)
                                     spec_text_position_list.append(position_name)
                                     spec_concentration_list.append(concentration)
 
                               
                                 if role == "substrate" or role == "sidesubstrate": #it is a rct
                                     #the center handle is supposed to be from the reactant
-                                    if center_handle == []:
-                                        center_handle.append(center_handle_candidate)
+                                    if center_handle[0] == []:
+                                        center_handle[0] = center_handle_candidate
                                     #rct_specGlyph_temp_list.append(specGlyph_id)
                                     rct_specGlyph_handles_temp_list.append([specGlyph_id,spec_handle,specRefGlyph_id,spec_lineend_pos])
                                 elif role == "product" or role == "sideproduct": #it is a prd
                                     #prd_specGlyph_temp_list.append(specGlyph_id)
+                                    if center_handle[1] == []:
+                                        center_handle[1] = center_handle_candidate
                                     prd_specGlyph_handles_temp_list.append([specGlyph_id,spec_handle,specRefGlyph_id,spec_lineend_pos])
                                 elif role == "modifier" or role == 'activator': #it is a modifier
                                     mod_specGlyph_temp_list.append(specGlyph_id)
                             #rct_specGlyph_list.append(rct_specGlyph_temp_list)
                             #prd_specGlyph_list.append(prd_specGlyph_temp_list)
                             try:
-                                reaction_center_handle_list.append(center_handle[0])
+                                if center_handle[0] != []:
+                                    reaction_center_handle_list.append(center_handle[0])
+                                else:
+                                    reaction_center_handle_list.append(center_handle[1])
                             except:
                                 #raise Exception("Can not find center handle information to process.")
                                 reaction_center_handle_list.append([])
                             rct_specGlyph_handle_list.append(rct_specGlyph_handles_temp_list)
                             prd_specGlyph_handle_list.append(prd_specGlyph_handles_temp_list)    
                             mod_specGlyph_list.append(mod_specGlyph_temp_list)
                          
@@ -1221,19 +1233,32 @@
                     for i in range(numComps):
                         temp_id = Comps_ids[i]
                         
                         vol= model.getCompartmentVolume(i)
                         if math.isnan(vol):
                             vol = 1.
                         if temp_id == "_compartment_default_":
-                            api.add_compartment(net_index, id=temp_id, volume = vol,
-                            size=Vec2(def_comp_width,def_comp_height), position=Vec2(10,10),
-                            fill_color = api.Color(255, 255, 255, 0), #the last digit for transparent
-                            border_color = api.Color(255, 255, 255, 0),
-                            border_width = comp_border_width)
+                            if len(comp_id_list) != 0:
+                                dimension = [def_comp_width, def_comp_height]
+                                position = [10, 10]                  
+                                for j in range(numCompGlyphs):
+                                    if comp_id_list[j] == temp_id:
+                                        dimension = comp_dimension_list[j]
+                                        position = comp_position_list[j]
+                                api.add_compartment(net_index, id=temp_id, volume = vol,
+                                size=Vec2(dimension[0],dimension[1]), position=Vec2(position[0],position[1]),
+                                fill_color = api.Color(255, 255, 255, 0), #the last digit for transparent
+                                border_color = api.Color(255, 255, 255, 0),
+                                border_width = comp_border_width)  
+                            else:
+                                api.add_compartment(net_index, id=temp_id, volume = vol,
+                                size=Vec2(def_comp_width,def_comp_height), position=Vec2(10,10),
+                                fill_color = api.Color(255, 255, 255, 0), #the last digit for transparent
+                                border_color = api.Color(255, 255, 255, 0),
+                                border_width = comp_border_width)
                         else:
                             if len(comp_id_list) != 0:
                             #if mplugin is not None:                    
                                 for j in range(numCompGlyphs):
                                     if comp_id_list[j] == temp_id:
                                         dimension = comp_dimension_list[j]
                                         position = comp_position_list[j]
@@ -1393,15 +1418,18 @@
                                     id_list.append(temp_id)
                                     nodeIdx_list.append(nodeIdx_temp)
                                     nodeIdx_specGlyph_alias_list.append([nodeIdx_temp,tempGlyph_id])
                                 
                                 comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
                                 for xx in range(numComps):
                                     if comp_id == Comps_ids[xx]:
-                                        api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_temp, comp_index=xx) 
+                                        try:
+                                            api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_temp, comp_index=xx)
+                                        except:
+                                            pass 
                                 for k in range(numCompGlyphs):
                                     if len(comp_id_list) !=0 and comp_id == comp_id_list[k]:
                                         comp_node_list[k].append(nodeIdx_temp)
                         for j in range(numBoundaryNodes):
                             if temp_id == BoundaryNodes_ids[j]:
                                 if temp_id not in id_list:
                                     flag_local = 0
@@ -2004,24 +2032,24 @@
                                 api.update_reaction(net_index, idx, 
                                 center_pos = Vec2(center_position[0],center_position[1]), 
                                 handle_positions=handles_Vec2, 
                                 fill_color=api.Color(reaction_line_color[0],reaction_line_color[1],reaction_line_color[2],reaction_line_color[3]))
 
 
                 else: # there is no layout information, assign position randomly and size as default
-                
+                    
                     comp_id_list = Comps_ids
 
                     for i in range(numComps):
                         temp_id = Comps_ids[i]
                         vol= model.getCompartmentVolume(i)
                         if math.isnan(vol):
                             vol = 1.
-                        dimension = [def_comp_width,def_comp_height]
-                        position = [10,10]
+                        dimension = [800 + 100, 800 + 100]
+                        position = [40,40]
 
                         api.add_compartment(net_index, id=temp_id, volume = vol,
                         size=Vec2(dimension[0],dimension[1]),position=Vec2(position[0],position[1]),
                         fill_color = api.Color(comp_fill_color[0],comp_fill_color[1],comp_fill_color[2],comp_fill_color[3]),
                         border_color = api.Color(comp_border_color[0],comp_border_color[1],comp_border_color[2],comp_border_color[3]),
                         border_width = comp_border_width)
```

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/modelMetrics.py` & `sbcoyote-1.4.2/rkviewer_plugins/modelMetrics.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/networkX.py` & `sbcoyote-1.4.2/rkviewer_plugins/networkX.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/randomNetwork.py` & `sbcoyote-1.4.2/rkviewer_plugins/randomNetwork.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/rkviewer_plugins/structuralAnalysis.py` & `sbcoyote-1.4.2/rkviewer_plugins/structuralAnalysis.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.0/PKG-INFO` & `sbcoyote-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: sbcoyote
-Version: 1.4.0
+Version: 1.4.2
 Summary: SBcoyote: An Extensible Python Based Reaction Editor and Viewer.
 Author: Jin Xu and Gary Geng et al
 Author-email: jxu2019@uw.edu
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: simulation
+Requires-Dist: SBMLDiagrams (>=1.3.4)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
 Requires-Dist: dataclasses (>=0.8,<0.9) ; python_version >= "3.6" and python_version < "3.7"
 Requires-Dist: marshmallow (>=3.11.1,<4.0.0)
 Requires-Dist: marshmallow-polyfield (>=5.10,<6.0)
 Requires-Dist: networkx (>=2.5.1,<3.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: python-libsbml (>=5.18.0,<6.0.0)
@@ -51,15 +51,15 @@
 
 ## Citing
 
 If you are using any of the code, please cite the article (https://arxiv.org/abs/2302.09151). 
 
 ## Installing SBcoyote
 
-* Install Python 3.7, 3.8, 3.9 or 3.10 if not already in the system.
+* Install Python 3.8, 3.9 or 3.10 if not already in the system.
 * Go to the command line and type `pip install SBcoyote`.
 * If wxPython doesn't get installed automatically, please try to install wxPython 4.1.1 or 4.2.0 manually referring to https://wxpython.org/pages/downloads/index.html. Note wxPython 4.1.1 does not work with Python 3.10. 
 * To run the application, simply type in the command line `SBcoyote`.
 
 ## Documentation
 
 The full documentation can be found at: https://sys-bio.github.io/SBcoyote/
```

