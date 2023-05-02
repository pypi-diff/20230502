# Comparing `tmp/pymodaq_femto-0.2.0.tar.gz` & `tmp/pymodaq_femto-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_femto-0.2.0.tar", last modified: Tue May 31 13:02:19 2022, max compression
+gzip compressed data, was "pymodaq_femto-0.2.1.tar", last modified: Tue May  2 10:39:10 2023, max compression
```

## Comparing `pymodaq_femto-0.2.0.tar` & `pymodaq_femto-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:02:19.022283 pymodaq_femto-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-05-31 13:02:19.022283 pymodaq_femto-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-05-31 13:02:19.022283 pymodaq_femto-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:02:19.018283 pymodaq_femto-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:02:19.018283 pymodaq_femto-0.2.0/src/pymodaq_femto/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14260 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/graphics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/materials.py
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/pnps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:02:19.022283 pymodaq_femto-0.2.0/src/pymodaq_femto/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    11329 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/resources/load_settings.png
--rw-r--r--   0 runner    (1001) docker     (121)    11258 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/resources/save_settings.png
--rw-r--r--   0 runner    (1001) docker     (121)    94151 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/retriever.py
--rw-r--r--   0 runner    (1001) docker     (121)    23392 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:02:19.022283 pymodaq_femto-0.2.0/src/pymodaq_femto/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-05-31 13:02:10.000000 pymodaq_femto-0.2.0/src/pymodaq_femto/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:02:19.018283 pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-05-31 13:02:18.000000 pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-31 13:02:18.000000 pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 13:02:18.000000 pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-05-31 13:02:18.000000 pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-31 13:02:18.000000 pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-31 13:02:18.000000 pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-02 10:39:10.980780 pymodaq_femto-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.972779 pymodaq_femto-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/pnps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/resources/load_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/resources/save_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95147 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/raw_scans/
+-rw-r--r--   0 runner    (1001) docker     (123)  1554195 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/raw_scans/example_measured_dscan_to_convert.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/top_level.txt
```

### Comparing `pymodaq_femto-0.2.0/LICENSE` & `pymodaq_femto-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/PKG-INFO` & `pymodaq_femto-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pymodaq_femto
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyMoDAQ extension for femtosecond laser pulse characterization
 Home-page: http://pymodaq.cnrs.fr
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CeCILL-B
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: <3.9,>=3.6
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `pymodaq_femto-0.2.0/setup.cfg` & `pymodaq_femto-0.2.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Software Development :: User Interfaces
 
 [options]
 py_module = pymodaq_femto
 python_requires = >=3.6, <3.9
 install_requires = 
-	pymodaq
+	pymodaq<4.0
 	matplotlib
+	pypret_pymodaq
+	pyqt5
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 
 [options.packages.find]
 where = src
```

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/__init__.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/graphics.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/graphics.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/materials.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/materials.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/pnps.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/pnps.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/resources/load_settings.png` & `pymodaq_femto-0.2.1/src/pymodaq_femto/resources/load_settings.png`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/resources/save_settings.png` & `pymodaq_femto-0.2.1/src/pymodaq_femto/resources/save_settings.png`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/retriever.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from collections import OrderedDict
 from pypret import FourierTransform, Pulse, PNPS, lib, MeshData, random_gaussian
 from pypret.frequencies import om2wl, wl2om, convert
 import scipy
 import importlib
 from scipy.fftpack import next_fast_len
 from pymodaq.daq_utils.h5modules import H5BrowserUtil, H5Saver
+from pymodaq.daq_utils.h5utils import get_h5_data_from_node
 from pyqtgraph.graphicsItems.GradientEditorItem import Gradients
 from pymodaq_femto import _PNPS_CLASSES
 from pypret.retrieval.retriever import _RETRIEVER_CLASSES
 import warnings
 import math, os
 import inspect
 import pymodaq_femto.materials
@@ -367,15 +368,15 @@
                             "readonly": False,
                             "tip": "Scaling to go from the Trace wavelength values to wavelength in meters",
                         },
                         {
                             "title": "Parameter scaling",
                             "name": "param_scaling",
                             "type": "float",
-                            "value": 1e-6,
+                            "value": 1,
                             "readonly": False,
                             "tip": "Scaling to go from the trace parameter values to delay in seconds, insertion in m (dscan) "
                                    "or phase in rad (miips)",
                         },
                     ],
                 },
                 {
@@ -802,14 +803,16 @@
             name="propagation_settings", type="group", children=self.prop_param
         )
         self.pulse_settings = Parameter.create(
             name="pulse_settings", type="group", children=self.pulse_prop
         )
         self.prop_settings.sigTreeStateChanged.connect(self.prop_settings_changed)
 
+        self.resources_dir = os.path.abspath(os.path.dirname(__file__)) + "\\resources"
+
         self.setupUI()
         self.create_menu(self.mainwindow.menuBar())
         self.simulator = None
         self.data_in = None
         self.ft = None
         self.retriever = None
         self.pnps = None
@@ -887,15 +890,15 @@
 
         self.ui.dock_retrieved_data = Dock("Retrieved Data")
         self.dockarea.addDock(
             self.ui.dock_retrieved_data, "below", self.ui.dock_retriever
         )
 
         self.ui.dock_propagation = Dock("Propagation")
-        self.dockarea.addDock(self.ui.dock_propagation, "below", self.ui.dock_retriever)
+        self.dockarea.addDock(self.ui.dock_propagation, "below", self.ui.dock_retrieved_data)
 
         self.ui.dock_processed.raiseDock()
 
         # ######################################################
         #  setup settings in dock
         self.settings_tree = ParameterTree()
         self.settings_tree.setMinimumWidth(300)
@@ -904,15 +907,15 @@
 
         # setup toolbar
         self.toolbar = QtWidgets.QToolBar()
         self.mainwindow.addToolBar(self.toolbar)
 
         if self.dashboard is not None:
             if self.dashboard.scan_module is not None:
-                self.load_last_scan_action = gutils.QAction(
+                self.load_last_scan_action = QAction(
                     QIcon(QPixmap(":/icons/Icon_Library/Open_2D.png")),
                     "Load last 2D scan",
                 )
                 self.toolbar.addAction(self.load_last_scan_action)
                 self.toolbar.addSeparator()
                 self.load_last_scan_action.triggered.connect(self.load_last_scan)
 
@@ -934,20 +937,21 @@
             "Load Data from Simulation",
         )
 
         self.save_data_action = QAction(
             QIcon(QPixmap(":/icons/Icon_Library/Save.png")), "Save Data"
         )
 
+
         self.save_settings_action = QAction(
-            QIcon(QPixmap("resources/save_settings.png")),
+            QIcon(QPixmap(os.path.join(self.resources_dir, 'save_settings.png'))),
             "Save current settings",
         )
         self.recall_settings_action = QAction(
-            QIcon(QPixmap("resources/load_settings.png")),
+            QIcon(QPixmap(os.path.join(self.resources_dir, 'load_settings.png'))),
             "Recall saved settings",
         )
 
         self.load_trace_in_action.triggered.connect(self.load_trace_in)
         self.load_spectrum_in_action.triggered.connect(self.load_spectrum_in)
         self.gen_trace_in_action.triggered.connect(self.open_simulator)
         self.load_from_simulation_action.triggered.connect(self.load_from_simulator)
@@ -1367,15 +1371,16 @@
         else:
             data, fname, node_path = browse_data(
                 ret_all=True,
                 message="Select the node corresponding to the" "Fundamental Spectrum",
             )
             if fname != "":
                 h5file = self.h5browse.open_file(fname)
-                data, axes, nav_axes, is_spread = self.h5browse.get_h5_data(node_path)
+                node = self.h5browse.get_node(node_path)
+                data, axes, nav_axes, is_spread = get_h5_data_from_node(node)
                 self.h5browse.close_file()
             else:
                 return
 
         if self.data_in is None:
             self.data_in = DataIn(source="experimental")
 
@@ -1419,15 +1424,16 @@
         self.settings.child("processing", "grid_settings", "wl0").setValue(wl0 * 1e9)
         self.state.append("spectrum_loaded")
 
     def load_trace_in(self, fname=None, node_path=None):
         try:
             if fname is not None and node_path is not None:
                 h5file = self.h5browse.open_file(fname)
-                data, axes, nav_axes, is_spread = self.h5browse.get_h5_data(node_path)
+                node = self.h5browse.get_node(node_path)
+                data, axes, nav_axes, is_spread = get_h5_data_from_node(node)
                 self.h5browse.close_file()
             else:
                 data, fname, node_path = browse_data(
                     ret_all=True,
                     message="Select the node corresponding to the"
                             "Characterization Trace",
                 )
@@ -1462,15 +1468,16 @@
             units=[unit, "m"],
         )
 
         return self.data_in["trace_in"]
 
     def get_axes_from_trace_node(self, fname, node_path):
         h5file = self.h5browse.open_file(fname)
-        data, axes, nav_axes, is_spread = self.h5browse.get_h5_data(node_path)
+        node = self.h5browse.get_node(node_path)
+        data, axes, nav_axes, is_spread = get_h5_data_from_node(node)
         self.h5browse.close_file()
         return axes["x_axis"], axes["nav_00"]
 
     def get_pulse_in(self):
 
         self.data_in["pulse_in"] = pulse_from_spectrum(
             self.data_in["raw_spectrum"]["x_axis"]["data"],
@@ -1639,15 +1646,15 @@
             return
         self.ui.dock_processed.raiseDock()
 
         self.generate_ft_grid()
         if len(np.unique(self.ft.w)) == 1:
             popup_message(
                 "Error",
-                "Frequency axis only has one point. Check time resolution and Npoints.",
+                "Frequency axis only has one point. Please check that i) the correct method and NL process are selected, ii) the grid settings in 'Processing' are correct. In particular, check that 'Time resolution (fs)' makes sense - typically it should be on the order of 1 fs for a standard femtosecond laser pulse.",
             )
             return
 
         method = self.settings.child("algo", "method").value()
         nlprocess = self.settings.child("algo", "nlprocess").value()
         wl0 = self.settings.child("data_in_info", "trace_in_info", "wl0").value() * 1e-9
         spectrum = self.data_in["raw_spectrum"]["data"]
@@ -1726,15 +1733,19 @@
                 self.settings.child("algo", "miips_parameter", "step").value(),
             )
         else:
             self.pnps = PNPS(self.data_in["pulse_in"], method, nlprocess)
 
         self.state.append("spectrum_processed")
         self.pulse_canvas.figure.clf()
-        PulsePlot(self.data_in["pulse_in"], self.pulse_canvas.figure)
+
+        try:
+            PulsePlot(self.data_in["pulse_in"], self.pulse_canvas.figure)
+        except ValueError:
+            popup_message("Error", "The wavelength axis of the processed spectrum seems to be wrong. Please check that i) the correct method and NL methods are selected, ii) the grid settings in 'Processing' are correct. In particular, check that 'Time resolution (fs)' makes sense - typically it is on the order of 1 fs for a standard femtosecond laser pulse.")
         self.pulse_canvas.draw()
 
     def process_trace(self):
         if "trace_loaded" not in self.state:
             popup_message("Error", "Please load a trace first!")
             return
         if "spectrum_processed" not in self.state:
@@ -2088,33 +2099,33 @@
 
         except Exception as e:
             pass
 
         h5saver.close_file()
 
     def save_settings_to_file(self):
-        path_to_file = 'resources/retriever_settings.h5'
+        path_to_file = os.path.join(self.resources_dir, 'retriever_settings.h5')
 
         msg = QtWidgets.QMessageBox()
         msg.setWindowTitle('Save settings to file')
 
         if os.path.exists(path_to_file):
             msg.setText('Do you want to overwrite the file with the current settings?')
         else:
             msg.setText('Should I save the current settings to file?')
         msg.setStandardButtons(QtWidgets.QMessageBox.Save | QtWidgets.QMessageBox.Cancel)
         msg.setDefaultButton(QtWidgets.QMessageBox.Save)
         msg.setIcon(QtWidgets.QMessageBox.Question)
         answer = msg.exec_()
 
         if answer == QtWidgets.QMessageBox.Save:
-            self.save_data('resources/retriever_settings.h5')
+            self.save_data(path_to_file)
 
     def recall_settings_from_file(self):
-        path_to_file = 'resources/retriever_settings.h5'
+        path_to_file = os.path.join(self.resources_dir, 'retriever_settings.h5')
 
         if not os.path.exists(path_to_file):
             popup_message("Error", "Did not find a file with saved settings.")
         else:
             h5file = self.h5browse.open_file(path_to_file)
             fund_data, fund_axes, fund_nav_axes, is_spread = self.h5browse.get_h5_data('/PyMoDAQFemtoAnalysis/DataIn/FunSpectrum/Data')
             trace_data, trace_axes, trace_nav_axes, is_spread = self.h5browse.get_h5_data('/PyMoDAQFemtoAnalysis/DataIn/NLTrace/Data')
```

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/simulation.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/simulation.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,57 +6,68 @@
 """
 
 import pypret
 from pymodaq.daq_utils.h5modules import H5SaverBase
 import os
 
 
-class DScanCustomSaver(H5SaverBase):
+class PyMoDAQFemtoCustomSaver(H5SaverBase):
     def add_exp_trace(self, node, trace, wl, label="Wavelength", units="m"):
         traceToSave = dict(data=trace, x_axis=dict(data=wl, label=label, units=units))
         det = self.get_set_group(node, "DSCAN_Measurement", title='DScan')
         self.set_attr(det, 'type', 'detector')
         # det = self.add_det_group(node, title='DScan')
         self.add_data(det, traceToSave, title='DScan trace')
 
-    def add_exp_insertion(self, node, insertion, label="Insertion", units="m"):
-        ax = self.add_navigation_axis(insertion, node, axis='x_axis', title=label)
+    def add_exp_parameter(self, node, parameter, label="Parameter", units="p.u."):
+        ax = self.add_navigation_axis(parameter, node, axis='x_axis', title=label)
         self.set_attr(ax, "label", label)
         self.set_attr(ax, "units", units)
         self.set_attr(ax, "nav_index", 0)
 
     def add_exp_fundamental(self, node, spectrum, wl, label="Wavelength", units="m"):
         spectrumToSave = dict(data=spectrum, x_axis=dict(data=wl, label=label, units=units))
         # det = self.add_det_group(node, title='Fundamental')
         det = self.get_set_group(node, "Fundamental_spectrum", title='Fundamental')
         self.add_data(det, spectrumToSave, title='Fundamental spectrum')
 
 
 if __name__ == '__main__':
     from pathlib import Path
+    saver = PyMoDAQFemtoCustomSaver()
 
-    path_root = Path(__file__).parent.parent.parent.parent
-    pathToLoad = path_root.joinpath("data/dscan_bank/")
-    pathToSave = path_root.joinpath("data/dscan_bank_pymodaq/")
+    # # One particular implementation of saved data
+    path_root = Path(__file__).parent
+    pathToLoad = path_root.joinpath("raw_scans/")
+    pathToSave = path_root.joinpath("converted_scans/")
     if not pathToSave.is_dir():
         pathToSave.mkdir()
 
-    saver = DScanCustomSaver()
-
-    fileIndex = 6
     # Load data
-    fileName = "measured_dscan_" + str(fileIndex) + ".h5"
+    fileName = "example_measured_dscan_to_convert.h5"
     pulse_from_spectrum, retrieved_pulse, measured_dscan, retrieved_dscan, raw_spectrum, folder = pypret.load(
         str(pathToLoad.joinpath(fileName)))
+    parameter_axis = measured_dscan.axes[0]
+    spectrum_trace_axis = measured_dscan.axes[1]
+    spectrum_fundamental_intensity = raw_spectrum.intensity
+    spectrum_fundamental_axis_wavelength = raw_spectrum.wl
+    trace_data = measured_dscan.data
+
+    # # template to use:
+    # trace_data = my_experimental_data_trace_as_2D_numpy_array
+    # parameter_axis = my_experimental_parameter_as_numpy_array
+    # spectrum_trace_axis = my_experimental_trace_wavelength_axis_as_numpy_array
+    # spectrum_fundamental_intensity = my_experimental_fundamental_spectrum_as_numpy_array
+    # spectrum_fundamental_axis_wavelength = my_experimental_fundamental_spectrum_wavelength_axis_as_numpy_array
 
     # Open file and create scan node
     saver.init_file(addhoc_file_path=str(pathToSave.joinpath(fileName)), update_h5=True)
     scannode = saver.add_scan_group()
     scannode.set_attr('scan_type', "Scan1D")
 
     # Add all data
-    saver.add_exp_insertion(scannode, measured_dscan.axes[0])
-    saver.add_exp_trace(scannode, measured_dscan.data, measured_dscan.axes[1])
-    saver.add_exp_fundamental(scannode, raw_spectrum.intensity, raw_spectrum.wl)
+    saver.add_exp_parameter(scannode, parameter_axis, label='Insertion', units='m')
+    saver.add_exp_trace(scannode, trace_data, spectrum_trace_axis)
+    saver.add_exp_fundamental(scannode, spectrum_fundamental_intensity, spectrum_fundamental_axis_wavelength)
     saver.close_file()
     pass
```

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto/viewers.py` & `pymodaq_femto-0.2.1/src/pymodaq_femto/viewers.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/PKG-INFO` & `pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pymodaq-femto
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyMoDAQ extension for femtosecond laser pulse characterization
 Home-page: http://pymodaq.cnrs.fr
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CeCILL-B
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: <3.9,>=3.6
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `pymodaq_femto-0.2.0/src/pymodaq_femto.egg-info/SOURCES.txt` & `pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 src/pymodaq_femto.egg-info/SOURCES.txt
 src/pymodaq_femto.egg-info/dependency_links.txt
 src/pymodaq_femto.egg-info/entry_points.txt
 src/pymodaq_femto.egg-info/requires.txt
 src/pymodaq_femto.egg-info/top_level.txt
 src/pymodaq_femto/resources/load_settings.png
 src/pymodaq_femto/resources/save_settings.png
-src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py
+src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py
+src/pymodaq_femto/utils/raw_scans/example_measured_dscan_to_convert.h5
```

