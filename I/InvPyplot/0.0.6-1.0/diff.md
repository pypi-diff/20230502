# Comparing `tmp/InvPyplot-0.0.6.tar.gz` & `tmp/InvPyplot-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InvPyplot-0.0.6.tar", last modified: Tue May  2 16:59:37 2023, max compression
+gzip compressed data, was "InvPyplot-1.0.tar", last modified: Wed Apr 19 19:02:18 2023, max compression
```

## Comparing `InvPyplot-0.0.6.tar` & `InvPyplot-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:59:37.504541 InvPyplot-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:59:37.504541 InvPyplot-0.0.6/InvPyplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-02 16:59:37.000000 InvPyplot-0.0.6/InvPyplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 16:59:37.000000 InvPyplot-0.0.6/InvPyplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:59:37.000000 InvPyplot-0.0.6/InvPyplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 16:59:37.000000 InvPyplot-0.0.6/InvPyplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 16:59:37.000000 InvPyplot-0.0.6/InvPyplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 16:59:22.000000 InvPyplot-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-02 16:59:37.504541 InvPyplot-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-02 16:59:22.000000 InvPyplot-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    36338 2023-05-02 16:59:22.000000 InvPyplot-0.0.6/invplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-02 16:59:22.000000 InvPyplot-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:59:37.504541 InvPyplot-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 16:59:22.000000 InvPyplot-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:02:18.653283 InvPyplot-1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:02:18.649283 InvPyplot-1.0/InvPyplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-19 19:02:18.000000 InvPyplot-1.0/InvPyplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-19 19:02:18.000000 InvPyplot-1.0/InvPyplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:02:18.000000 InvPyplot-1.0/InvPyplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 19:02:18.000000 InvPyplot-1.0/InvPyplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 19:02:18.000000 InvPyplot-1.0/InvPyplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-19 19:02:04.000000 InvPyplot-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-19 19:02:18.649283 InvPyplot-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 19:02:04.000000 InvPyplot-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    36308 2023-04-19 19:02:04.000000 InvPyplot-1.0/invplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-19 19:02:04.000000 InvPyplot-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:02:18.653283 InvPyplot-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 19:02:04.000000 InvPyplot-1.0/setup.py
```

### Comparing `InvPyplot-0.0.6/InvPyplot.egg-info/PKG-INFO` & `InvPyplot-1.0/InvPyplot.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InvPyplot
-Version: 0.0.6
+Version: 1.0
 Summary: Python package enabling plotting of .inv files exported from Res2DInv in matplotlib
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,22 +21,22 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/RJbalikian/InvPyplot
-Project-URL: API Documentation, https://rjbalikian.github.io/InvPyplot/
 Keywords: Res2dInv,electrical,resistivity,geophysics,plot,inv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # InvPyplot
 Plot Res2DInv .inv files in matplotlib
 
-This package makes it easy to read and plot .inv files using customizations available through matplotlib.
+This package makes it easy to read and plot .inv files using the customization available through matplotlib.
+
+Read the docstrings for the autoplot and resinv_plot functions for how to customize.
 
-- API Documentation here: https://rjbalikian.github.io/InvPyplot/
```

### Comparing `InvPyplot-0.0.6/LICENSE` & `InvPyplot-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `InvPyplot-0.0.6/PKG-INFO` & `InvPyplot-1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InvPyplot
-Version: 0.0.6
+Version: 1.0
 Summary: Python package enabling plotting of .inv files exported from Res2DInv in matplotlib
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,22 +21,22 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/RJbalikian/InvPyplot
-Project-URL: API Documentation, https://rjbalikian.github.io/InvPyplot/
 Keywords: Res2dInv,electrical,resistivity,geophysics,plot,inv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # InvPyplot
 Plot Res2DInv .inv files in matplotlib
 
-This package makes it easy to read and plot .inv files using customizations available through matplotlib.
+This package makes it easy to read and plot .inv files using the customization available through matplotlib.
+
+Read the docstrings for the autoplot and resinv_plot functions for how to customize.
 
-- API Documentation here: https://rjbalikian.github.io/InvPyplot/
```

### Comparing `InvPyplot-0.0.6/invplot.py` & `InvPyplot-1.0/invplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy.interpolate
 import matplotlib
 
-def autoplot(inv_file, iteration, return_dict=False, **kwargs):
+def autoplot(inv_file, iteration, verbose=False, **kwargs):
     """Function to run all intermedaite functions and resinv_plot to simply read and plot everything in one call.
 
     Parameters
     ----------
     inv_file : str or pathlib.PurePath object
         Filepath to .inv file of interest. The .inv file should be one generated from Res2DInv.
     iteration : int or list or either str {':', 'all'}
         Integer or list of integers indicating which iteration of the .inv result to use for plotting. If list, all will be plotted separately. If ':' or 'all', will plot all iterations successively.
-    return_dict : bool, optional
-        Whether to return results as a dictionary, by default False
+    verbose : bool, optional
+        Whether to print results out to terminal along the way, by default False
     **kwargs
         Other keyword arguments may be read into autoplot. These are read in as **kwargs to either resinv_plot() or matplotlib.pyplot.imshow via the resinv_plot function. See documentation for resinv_plot for available parameters for resinv_plot.
 
     Returns
     -------
     inv_dict : dict
         Dictionary containing all input parameters and data generated along the way, including the output figures and axes
@@ -75,17 +75,15 @@
         axList.append(ax)
 
     inv_dict['iterationNo'] = iterIndList
     inv_dict['iterationInd'] = iterNoList
     inv_dict['fig'] = figList
     inv_dict['ax'] = axList
     
-    if return_dict:
-        return inv_dict
-    return
+    return inv_dict
 
 #Function that performs all the actual plotting
 def resinv_plot(inv_dict, colMap='nipy_spectral', cBarFormat ='%3.0f', cBarLabel='Resistivity (ohm-m)', cBarOrientation='horizontal', cMin=None, cMax=None, griddedFt=[False,False], griddedM=[False,False], title=None, normType='log', primaryUnit='m', showPoints=False,whichTicks='major', figsize=None, dpi=None, reverse=False, tight_layout=True, savefig=False, saveformat='png', imshow_kwargs=None, **kwargs):
     """Function to pull everything together and plot it nicely.
 
     It is recommended to use the autoplot function rather than resinv_plot directly, since using autoplot() incorporates all the setup needed to create the input dictionary keys/values correctly.
```

### Comparing `InvPyplot-0.0.6/pyproject.toml` & `InvPyplot-1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'InvPyplot'
 dynamic = ["readme"]
 license = {file = "LICENSE"}
-version="0.0.6"
+version="1.0"
 description = "Python package enabling plotting of .inv files exported from Res2DInv in matplotlib"
 keywords = ["Res2dInv", "electrical", "resistivity", "geophysics", "plot", 'inv']
 requires-python = ">=3.0"
 dependencies =  ["numpy", "pandas", "matplotlib", "scipy"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -18,8 +18,7 @@
 ]
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"]}
 
 [project.urls]
 "Homepage" = "https://github.com/RJbalikian/InvPyplot"
-"API Documentation" = "https://rjbalikian.github.io/InvPyplot/"
```

