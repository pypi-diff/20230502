# Comparing `tmp/qudi_hira_analysis-1.4.2.tar.gz` & `tmp/qudi_hira_analysis-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qudi_hira_analysis-1.4.2.tar", max compression
+gzip compressed data, was "qudi_hira_analysis-1.4.3.tar", max compression
```

## Comparing `qudi_hira_analysis-1.4.2.tar` & `qudi_hira_analysis-1.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1090 2023-03-04 13:38:16.100952 qudi_hira_analysis-1.4.2/LICENSE
--rw-r--r--   0        0        0      899 2023-04-17 14:19:29.352143 qudi_hira_analysis-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      176 2023-03-05 20:29:56.471910 qudi_hira_analysis-1.4.2/qudi_hira_analysis/__init__.py
--rw-r--r--   0        0        0    11607 2023-04-17 14:18:57.003451 qudi_hira_analysis-1.4.2/qudi_hira_analysis/analysis_logic.py
--rw-r--r--   0        0        0    13217 2023-04-17 14:25:42.292519 qudi_hira_analysis-1.4.2/qudi_hira_analysis/data_handler.py
--rw-r--r--   0        0        0        0 2023-03-05 20:20:55.998728 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/__init__.py
--rw-r--r--   0        0        0     1992 2023-01-10 21:18:35.126407 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/antibunchingmethods.py
--rw-r--r--   0        0        0    25064 2023-01-10 21:18:35.126407 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/decaylikemethods.py
--rw-r--r--   0        0        0    41794 2023-03-05 20:29:56.434172 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
--rw-r--r--   0        0        0    23695 2023-03-05 20:29:56.418510 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/generalmethods.py
--rw-r--r--   0        0        0     5998 2023-03-05 20:29:56.434172 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
--rw-r--r--   0        0        0    10849 2023-03-05 20:29:56.418510 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/linearmethods.py
--rw-r--r--   0        0        0    42414 2023-03-05 20:29:56.402925 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
--rw-r--r--   0        0        0    16836 2023-03-05 20:29:56.449756 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
--rw-r--r--   0        0        0   108340 2023-04-03 12:15:20.198945 qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/sinemethods.py
--rw-r--r--   0        0        0     1854 2023-03-09 22:52:17.007898 qudi_hira_analysis-1.4.2/qudi_hira_analysis/helper_functions.py
--rw-r--r--   0        0        0    13112 2023-04-17 14:27:20.868766 qudi_hira_analysis-1.4.2/qudi_hira_analysis/io_handler.py
--rw-r--r--   0        0        0     6960 2023-03-10 00:23:25.520105 qudi_hira_analysis-1.4.2/qudi_hira_analysis/measurement_dataclass.py
--rw-r--r--   0        0        0    19138 2023-04-17 14:03:20.837890 qudi_hira_analysis-1.4.2/qudi_hira_analysis/qudi_fit_logic.py
--rw-r--r--   0        0        0    12219 2023-04-14 20:12:36.860860 qudi_hira_analysis-1.4.2/README.md
--rw-r--r--   0        0        0    13165 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.2/setup.py
--rw-r--r--   0        0        0    12891 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-03-04 13:38:16.100952 qudi_hira_analysis-1.4.3/LICENSE
+-rw-r--r--   0        0        0      899 2023-05-02 13:27:57.641266 qudi_hira_analysis-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-03-05 20:29:56.471910 qudi_hira_analysis-1.4.3/qudi_hira_analysis/__init__.py
+-rw-r--r--   0        0        0    11607 2023-04-17 14:18:57.003451 qudi_hira_analysis-1.4.3/qudi_hira_analysis/analysis_logic.py
+-rw-r--r--   0        0        0    14024 2023-05-02 13:20:52.265183 qudi_hira_analysis-1.4.3/qudi_hira_analysis/data_handler.py
+-rw-r--r--   0        0        0        0 2023-03-05 20:20:55.998728 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/__init__.py
+-rw-r--r--   0        0        0     1992 2023-01-10 21:18:35.126407 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/antibunchingmethods.py
+-rw-r--r--   0        0        0    25064 2023-01-10 21:18:35.126407 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/decaylikemethods.py
+-rw-r--r--   0        0        0    41794 2023-03-05 20:29:56.434172 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
+-rw-r--r--   0        0        0    23695 2023-03-05 20:29:56.418510 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/generalmethods.py
+-rw-r--r--   0        0        0     5998 2023-03-05 20:29:56.434172 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
+-rw-r--r--   0        0        0    10849 2023-03-05 20:29:56.418510 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/linearmethods.py
+-rw-r--r--   0        0        0    42414 2023-03-05 20:29:56.402925 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
+-rw-r--r--   0        0        0    16836 2023-03-05 20:29:56.449756 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
+-rw-r--r--   0        0        0   108340 2023-04-03 12:15:20.198945 qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/sinemethods.py
+-rw-r--r--   0        0        0     1854 2023-03-09 22:52:17.007898 qudi_hira_analysis-1.4.3/qudi_hira_analysis/helper_functions.py
+-rw-r--r--   0        0        0    13799 2023-05-02 13:20:52.260179 qudi_hira_analysis-1.4.3/qudi_hira_analysis/io_handler.py
+-rw-r--r--   0        0        0     6960 2023-03-10 00:23:25.520105 qudi_hira_analysis-1.4.3/qudi_hira_analysis/measurement_dataclass.py
+-rw-r--r--   0        0        0    19138 2023-04-17 14:03:20.837890 qudi_hira_analysis-1.4.3/qudi_hira_analysis/qudi_fit_logic.py
+-rw-r--r--   0        0        0    13666 2023-05-02 13:24:16.673723 qudi_hira_analysis-1.4.3/README.md
+-rw-r--r--   0        0        0    14612 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.3/setup.py
+-rw-r--r--   0        0        0    14285 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.3/PKG-INFO
```

### Comparing `qudi_hira_analysis-1.4.2/LICENSE` & `qudi_hira_analysis-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/pyproject.toml` & `qudi_hira_analysis-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qudi-hira-analysis"
-version = "1.4.2"
+version = "1.4.3"
 repository = "https://github.com/dineshpinto/qudi-hira-analysis"
 homepage = "https://github.com/dineshpinto/qudi-hira-analysis"
 keywords = ["python", "qubit", "analysis", "nv centers", "photon timetrace"]
 description = "A Python toolkit to analzye photon timetrace data from qubit sensors"
 authors = ["dineshpinto <annual.fallout_0z@icloud.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/analysis_logic.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/analysis_logic.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/data_handler.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/data_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import datetime
 import logging
 import os
 from pathlib import Path
 from typing import List, TYPE_CHECKING, Callable
 
+import pySPM
+
 from qudi_hira_analysis.analysis_logic import AnalysisLogic
 from qudi_hira_analysis.io_handler import IOHandler
 from qudi_hira_analysis.measurement_dataclass import RawTimetrace, PulsedMeasurement, PulsedMeasurementDataclass, \
     LaserPulses, MeasurementDataclass
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -28,34 +30,46 @@
         super().__init__(**kwargs)
 
         # Create callables used in measurement dataclasses
         self.default_qudi_loader: (Callable[[Path], pd.DataFrame], Callable[[Path], dict]) = (
             self.read_into_dataframe,
             self.read_qudi_parameters
         )
-        self.confocal_qudi_loader: (Callable[[Path, ...], np.ndarray], Callable[[Path], dict]) = (
+        self.confocal_qudi_loader: (Callable[[Path], np.ndarray], Callable[[Path], dict]) = (
             self.read_confocal_into_dataframe,
             self.read_qudi_parameters
         )
-        self.pixelscanner_qudi_loader: (Callable[[Path, ...], np.ndarray], Callable[[Path], dict]) = (
+        self.pixelscanner_qudi_loader: (Callable[[Path], (pySPM.SPM_image, pySPM.SPM_image)], Callable[[Path], dict]) = (
             self.read_pixelscanner_data,
             self.read_qudi_parameters
         )
-        self.trace_qudi_loader: (Callable[[Path, ...], np.ndarray], Callable[[Path], dict]) = (
+        self.trace_qudi_loader: (Callable[[Path], np.ndarray], Callable[[Path], dict]) = (
             self.read_into_ndarray_transposed,
             self.read_qudi_parameters
         )
         self.nanonis_loader: (Callable[[Path], pd.DataFrame], Callable[[Path], dict]) = (
             self.read_nanonis_data,
             self.read_nanonis_parameters
         )
+        self.nanonis_spm_loader: (Callable[[Path], pySPM.SXM], None) = (
+            self.read_nanonis_spm_data,
+            None
+        )
+        self.bruker_spm_loader: (Callable[[Path], pySPM.Bruker], None) = (
+            self.read_bruker_spm_data,
+            None
+        )
         self.temperature_loader: (Callable[[Path], pd.DataFrame], None) = (
             self.read_lakeshore_data,
             None
         )
+        self.pys_loader: (Callable[[Path], dict], None) = (
+            self.read_pys,
+            None
+        )
         self.pressure_loader: (Callable[[Path], pd.DataFrame], None) = (
             self.read_pfeiffer_data,
             None
         )
 
 
 class DataHandler(DataLoader, AnalysisLogic):
@@ -253,25 +267,35 @@
     def __load_standard_measurements_into_dataclass(
             self,
             measurement_str: str,
             extension: str
     ) -> dict[str: MeasurementDataclass]:
         measurement_list: dict[str: MeasurementDataclass] = {}
 
+        # Try and infer measurement type
         if measurement_str.lower() == "temperature-monitoring":
             loaders = self.temperature_loader
             extension = ".xls"
             exclude_str = None
         elif measurement_str.lower() == "pressure-monitoring":
             loaders = self.pressure_loader
             extension = ".txt"
             exclude_str = None
         elif measurement_str == "frq-sweep":
             loaders = self.nanonis_loader
             exclude_str = None
+        elif extension == ".sxm":
+            loaders = self.nanonis_spm_loader
+            exclude_str = None
+        elif extension == ".pys":
+            loaders = self.pys_loader
+            exclude_str = None
+        elif extension == ".001":
+            loaders = self.bruker_spm_loader
+            exclude_str = None
         else:
             loaders = self.default_qudi_loader
             exclude_str = None
 
         for filepath in self.get_measurement_filepaths(measurement_str, extension, exclude_str):
             timestamp = datetime.datetime.fromtimestamp(os.path.getmtime(filepath))
             ts = datetime.datetime.strftime(timestamp, self.timestamp_format_str)
```

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/antibunchingmethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/antibunchingmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/decaylikemethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/decaylikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/gaussianlikemethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/gaussianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/generalmethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/generalmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/linearmethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/linearmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/poissonianlikemethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/poissonianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/fitmethods/sinemethods.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/fitmethods/sinemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/helper_functions.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/io_handler.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/io_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from functools import wraps
 from pathlib import Path
 from typing import Callable
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import pySPM
 
 
 class IOHandler:
     """ Handle all read and write operations. """
 
     def __init__(self, base_read_path: Path = None, base_write_path: Path = None):
         super().__init__()
@@ -134,17 +135,19 @@
 
     @add_base_read_path
     def read_into_ndarray_transposed(self, filepath: Path, **kwargs) -> np.ndarray:
         return np.genfromtxt(filepath, **kwargs).T
 
     @add_base_read_path
     @check_extension(".pys")
-    def read_pys(self, filepath: Path) -> np.ndarray:
+    def read_pys(self, filepath: Path) -> dict:
         """ Loads raw pys data files. Wraps around numpy.load. """
-        return np.load(str(filepath), encoding="bytes", allow_pickle=True)
+        byte_dict = np.load(str(filepath), encoding="bytes", allow_pickle=True)
+        # Convert byte string keys to normal strings
+        return {key.decode('utf8'): byte_dict.get(key) for key in byte_dict.keys()}
 
     @add_base_read_path
     @check_extension(".pkl")
     def read_pkl(self, filepath: Path) -> dict:
         """ Loads processed pickle files for plotting/further analysis. """
         with open(filepath, 'rb') as f:
             file = pickle.load(f)
@@ -189,14 +192,26 @@
                         pass
                     if "Oscillation Control>" in label:
                         label = label.replace("Oscillation Control>", "")
                     parameters[label] = value
         return parameters
 
     @add_base_read_path
+    @check_extension(".sxm")
+    def read_nanonis_spm_data(self, filepath: Path) -> pySPM.SXM:
+        """ Read a Nanonis SPM data file. """
+        return pySPM.SXM(filepath)
+
+    @add_base_read_path
+    @check_extension(".001")
+    def read_bruker_spm_data(self, filepath: Path) -> pySPM.Bruker:
+        """ Read a Bruker SPM data file. """
+        return pySPM.Bruker(filepath)
+
+    @add_base_read_path
     @check_extension(".txt")
     def read_pfeiffer_data(self, filepath: Path) -> pd.DataFrame:
         """ Read data stored by Pfeiffer vacuum monitoring software. """
         # Extract rows including the header
         df = pd.read_csv(filepath, sep="\t", skiprows=[0, 2, 3, 4])
         # Combine data and time columns together
         df["Date"] = df["Date"] + " " + df["Time"]
@@ -240,31 +255,34 @@
         # Extract forward scan array as every second element
         forward_counts = np.stack(split_array[::2])
         # Extract backward scan array as every shifted second element
         # Flip scan so that backward and forward scans represent the same data
         backward_counts = np.flip(np.stack(split_array[1::2]), axis=1)
         return forward_counts, backward_counts
 
-    def read_pixelscanner_data(self, filepath: Path) -> (np.ndarray, np.ndarray):
+    def read_pixelscanner_data(self, filepath: Path) -> (pySPM.SPM_image, pySPM.SPM_image):
         df = self.read_into_dataframe(filepath)
         num_pixels = int(np.sqrt(len(df) // 2))
 
         if num_pixels ** 2 != len(df) // 2:
             raise ValueError("Number of pixels does not match data length.")
 
         try:
-            forward, backward = self.__get_forward_backward_counts(df["count_rates"], num_pixels)
+            fwd, bwd = self.__get_forward_backward_counts(df["count_rates"], num_pixels)
         except KeyError:
             try:
-                forward, backward = self.__get_forward_backward_counts(df["Count Rates (cps)"], num_pixels)
+                fwd, bwd = self.__get_forward_backward_counts(df["Count Rates (cps)"], num_pixels)
             except KeyError:
                 # Support old data format
-                forward = df["forward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
-                backward = df["backward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
-        return forward, backward
+                fwd = df["forward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
+                bwd = df["backward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
+
+        fwd = pySPM.SPM_image(fwd, channel="Forward", _type="NV-PL")
+        bwd = pySPM.SPM_image(bwd, channel="Backward", _type="NV-PL")
+        return fwd, bwd
 
     @add_base_write_path
     @check_extension(".pkl")
     def save_pkl(self, filepath: Path, obj: object):
         """ Saves processed pickle files for plotting/further analysis. """
         with open(filepath, 'wb') as f:
             pickle.dump(obj, f)
```

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/measurement_dataclass.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/measurement_dataclass.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/qudi_hira_analysis/qudi_fit_logic.py` & `qudi_hira_analysis-1.4.3/qudi_hira_analysis/qudi_fit_logic.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.2/README.md` & `qudi_hira_analysis-1.4.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -79,15 +79,68 @@
 The `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.
 
 - The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.
 
 - The dictionary values are `MeasurementDataclass` objects whose schema is shown
   visually [here](#measurement-dataclass-schema).
 
-### Example 1: Autocorrelation measurements (Antibunching fit)
+### Example 0: NV-PL measurements
+
+```python
+pixel_scanner_measurements = dh.load_measurements(measurement_str="PixelScanner")
+
+fwd, bwd = pixel_scanner_measurements["20230101-0420-00"].data
+
+# If size is known, it can be specified here
+fwd.size["real"] = {"x": 1e-6, "y": 1e-6, "unit": "m"}
+
+fig, ax = plt.subplots()
+
+# Perform (optional) image corrections
+fwd.filter_gaussian(sigma=0.5)
+
+# Add scale bar, color bar and plot the data
+img = fwd.show(cmap="inferno", ax=ax)
+fwd.add_scale(length=1e-6, ax=ax, height=1)
+cbar = fig.colorbar(img)
+cbar.set_label("NV-PL (kcps)")
+
+# Save the figure to the figure folder specified earlier
+dh.save_figures(filepath="nv_pl_scan", fig=fig, only_jpg=True)
+```
+
+### Example 1: Nanonis AFM measurements
+
+```python
+afm_measurements = dh.load_measurements(measurement_str="Scan", extension=".sxm")
+
+afm = afm_measurements["20230101-0420-00"].data
+
+# Print the channels available in the data
+afm.list_channels()
+topo = afm.get_channel("Z")
+
+fig, ax = plt.subplots()
+
+# Perform (optional) image corrections
+topo.correct_lines()
+topo.correct_plane()
+topo.filter_lowpass(fft_radius=20)
+topo.zero_min()
+
+# Add scale bar, color bar and plot the data
+img = topo.show(cmap="inferno", ax=ax)
+topo.add_scale(length=1e-6, ax=ax, height=1, fontsize=10)
+cbar = fig.colorbar(img)
+cbar.set_label("Height (nm)")
+
+dh.save_figures(filepath="afm_topo", fig=fig, only_jpg=True)
+``` 
+
+### Example 2: Autocorrelation measurements (Antibunching fit)
 
 ```python
 autocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")
 
 fig, ax = plt.subplots()
 
 for autocorrelation in autocorrelation_measurements.values():
@@ -99,15 +152,15 @@
     # Plot the fit
     sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
 # Save the figure to the figure folder specified earlier
 dh.save_figures(filepath="autocorrelation_variation", fig=fig)
 ```
 
-### Example 2: ODMR measurements (double Lorentzian 15N fit)
+### Example 3: ODMR measurements (double Lorentzian fit)
 
 ```python
 odmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)
 
 fig, ax = plt.subplots()
 
 for odmr in odmr_measurements.values():
@@ -115,15 +168,15 @@
     fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,
                                   fit_function=dh.fit_function.lorentzian_double)
     sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
 dh.save_figures(filepath="odmr_variation", fig=fig)
 ```
 
-### Example 3: Rabi measurements (sine exponential decay fit)
+### Example 4: Rabi measurements (sine exponential decay fit)
 
 ```python
 rabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)
 
 fig, ax = plt.subplots()
 
 for rabi in rabi_measurements.values():
@@ -131,15 +184,15 @@
     fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,
                                   fit_function=dh.fit_function.sineexponentialdecay)
     sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
 dh.save_figures(filepath="rabi_variation", fig=fig)
 ```
 
-### Example 4: Temperature data
+### Example 5: Temperature data
 
 ```python
 temperature_measurements = dh.load_measurements(measurement_str="Temperature")
 
 temperature = pd.concat([t.data for t in temperature_measurements.values()])
 
 fig, ax = plt.subplots()
```

### Comparing `qudi_hira_analysis-1.4.2/setup.py` & `qudi_hira_analysis-1.4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'pandas>=2.0.0,<3.0.0',
  'pyspm>=0.3.0,<0.4.0',
  'tqdm>=4.64.1,<5.0.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'qudi-hira-analysis',
-    'version': '1.4.2',
+    'version': '1.4.3',
     'description': 'A Python toolkit to analzye photon timetrace data from qubit sensors',
-    'long_description': '[![DOI](https://zenodo.org/badge/288670453.svg)](https://zenodo.org/badge/latestdoi/288670453)\n[![Downloads](https://pepy.tech/badge/qudi-hira-analysis)](https://pepy.tech/project/qudi-hira-analysis)\n[![PyPi version](https://img.shields.io/pypi/v/qudi-hira-analysis)](https://pypi.python.org/pypi/qudi-hira-analysis/)\n[![Python 3.10](https://img.shields.io/badge/python-3.10-orange.svg)](https://www.python.org/downloads/release/python-3100//)\n[![Python 3.11](https://img.shields.io/badge/python-3.11-orange.svg)](https://www.python.org/downloads/release/python-3110//)\n\n# Qudi Hira Analysis\n\nThis toolkit automates a large portion of the work surrounding data analysis on quantum sensing experiments where the\nprimary raw data extracted is photon counts.\n\nThe high level interface is abstracted, and provides a set of functions to automate data import, handling and analysis.\nIt is designed to be exposed through Jupyter Notebooks, although the abstract interface allows it to be integrated into\nlarger, more general frameworks as well (with only some pain). Using the toolkit itself should only require a\nbeginner-level understanding of Python.\n\nIt also aims to improve transparency and reproducibility in experimental data analysis. In an ideal scenario,\ntwo lines of code are sufficient to recreate all output data.\n\nPython offers some very handy features like dataclasses, which are heavily used by this toolkit. Dataclasses offer a\nfull OOP (object-oriented programming) experience while analyzing complex data sets. They provide a solid and\ntransparent structure to the data to\nreduce errors arising from data fragmentation. This generally comes at a large performance cost, but this is (largely)\nsidestepped by lazy loading data and storing metadata instead wherever possible.\n\n## Installation\n\n```bash\npip install qudi-hira-analysis\n```\n\n## Citation\n\nIf you are publishing scientific results, you can cite this work as:  https://doi.org/10.5281/zenodo.7604670\n\n## Examples\n\nFirst set up the `DataHandler` object (henceforth referred to as `dh`) with the correct paths to the data and figure\nfolders.\n\nEverything revolves around the `dh` object. It is the main interface to the toolkit and is initialized with the\nfollowing required arguments:\n\n- `data_folder` is the main folder where all the data is stored, it can be the direct path to the data, or composed of\n  several sub-folders, each containing the data for a specific measurement\n- `figure_folder` is the folder where the output figures will be saved\n\nOptional arguments:\n\n- `measurement_folder` is the specific sub-folder in `data_folder` where the data for a specific measurement is stored\n\n```python\nfrom pathlib import Path\nimport matplotlib.pyplot as plt\nimport seaborn as sns\n\nfrom qudi_hira_analysis import DataHandler\n\ndh = DataHandler(\n    data_folder=Path("C:\\\\", "Data"),\n    figure_folder=Path("C:\\\\", "QudiHiraAnalysis"),\n    measurement_folder=Path("20230101_NV1")\n)\n```\n\nTo load a specific set of measurements from the data folder, use the `dh.load_measurements()` method, which takes the\nfollowing required arguments:\n\n- `measurement_str` is the string that is used to identify the measurement. It is used to filter the data files in the\n  `data_folder` and `measurement_folder` (if specified)\n\nOptional arguments:\n\n- `qudi` is a boolean. If `True`, the data is assumed to be in the format used by Qudi (default: True)\n- `pulsed` is a boolean. If `True`, the data is assumed to be in the format used by Qudi for pulsed measurements (\n  default: False)\n- `extension` is the extension of the data files (default: ".dat")\n\nThe `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.\n\n- The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.\n\n- The dictionary values are `MeasurementDataclass` objects whose schema is shown\n  visually [here](#measurement-dataclass-schema).\n\n### Example 1: Autocorrelation measurements (Antibunching fit)\n\n```python\nautocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")\n\nfig, ax = plt.subplots()\n\nfor autocorrelation in autocorrelation_measurements.values():\n    # Plot the data\n    sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)\n    # Fit the data using the antibunching function\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data,\n                                  fit_function=dh.fit_function.antibunching)\n    # Plot the fit\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax)\n\n# Save the figure to the figure folder specified earlier\ndh.save_figures(filepath="autocorrelation_variation", fig=fig)\n```\n\n### Example 2: ODMR measurements (double Lorentzian 15N fit)\n\n```python\nodmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)\n\nfig, ax = plt.subplots()\n\nfor odmr in odmr_measurements.values():\n    sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,\n                                  fit_function=dh.fit_function.lorentzian_double)\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax)\n\ndh.save_figures(filepath="odmr_variation", fig=fig)\n```\n\n### Example 3: Rabi measurements (sine exponential decay fit)\n\n```python\nrabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)\n\nfig, ax = plt.subplots()\n\nfor rabi in rabi_measurements.values():\n    sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,\n                                  fit_function=dh.fit_function.sineexponentialdecay)\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax)\n\ndh.save_figures(filepath="rabi_variation", fig=fig)\n```\n\n### Example 4: Temperature data\n\n```python\ntemperature_measurements = dh.load_measurements(measurement_str="Temperature")\n\ntemperature = pd.concat([t.data for t in temperature_measurements.values()])\n\nfig, ax = plt.subplots()\nsns.lineplot(data=temperature, x="Time", y="Temperature", ax=ax)\ndh.save_figures(filepath="temperature_monitoring", fig=fig)\n```\n\n## Measurement Dataclass Schema\n\n```mermaid\nflowchart LR\n    subgraph Standard Data\n        MeasurementDataclass --o filepath1[filepath: Path];\n        MeasurementDataclass --o data1[data: DataFrame];\n        MeasurementDataclass --o params1[params: dict];\n        MeasurementDataclass --o timestamp1[timestamp: datetime.datetime];\n        MeasurementDataclass --o methods1[get_param_from_filename: Callable];\n        MeasurementDataclass --o methods2[set_datetime_index: Callable];\n    end\n    subgraph Pulsed Data\n        MeasurementDataclass -- pulsed --> PulsedMeasurementDataclass;\n        PulsedMeasurementDataclass -- measurement --> PulsedMeasurement;\n        PulsedMeasurement --o filepath2[filepath: Path];\n        PulsedMeasurement --o data2[data: DataFrame];\n        PulsedMeasurement --o params2[params: dict];\n        PulsedMeasurementDataclass -- laser_pulses --> LaserPulses;\n        LaserPulses --o filepath3[filepath: Path];\n        LaserPulses --o data3[data: DataFrame];\n        LaserPulses --o params3[params: dict];\n        PulsedMeasurementDataclass -- timetrace --> RawTimetrace;\n        RawTimetrace --o filepath4[filepath: Path];\n        RawTimetrace --o data4[data: DataFrame];\n        RawTimetrace --o params4[params: dict];\n    end\n```\n\n## Supports common fitting routines\n\nTo get the full list of available fit routines, use the `dh.fit_function` attribute. The fit functions are:\n\n| Dimension | Fit                           |\n|-----------|-------------------------------|\n| 1d        | decayexponential              |\n|           | biexponential                 |\n|           | decayexponentialstretched     |\n|           | gaussian                      |\n|           | gaussiandouble                |\n|           | gaussianlinearoffset          |\n|           | hyperbolicsaturation          |\n|           | linear                        |\n|           | lorentzian                    |\n|           | lorentziandouble              |\n|           | lorentziantriple              |\n|           | sine                          |\n|           | sinedouble                    |\n|           | sinedoublewithexpdecay        |\n|           | sinedoublewithtwoexpdecay     |\n|           | sineexponentialdecay          |\n|           | sinestretchedexponentialdecay |\n|           | sinetriple                    |\n|           | sinetriplewithexpdecay        |\n|           | sinetriplewiththreeexpdecay   |\n| 2d        | twoDgaussian                  |\n\n## Inbuilt measurement tree visualizer\n\n```ipython\n>>> dh.data_folder_tree()\n\n# Output\n├── 20211116_NetworkAnalysis_SampleIn_UpperPin.csv\n├── 20211116_NetworkAnalysis_SampleOut_UpperPin.csv\n├── 20211116_NetworkAnalysis_TipIn_LowerPin.csv\n├── 20211116_NetworkAnalysis_TipIn_UpperPin.csv\n├── 20211116_NetworkAnalysis_TipOut_LowerPin.csv\n├── 20211116_NetworkAnalysis_TipOut_UpperPin.csv\n├── ContactTestingMeasurementHead\n│   ├── C2_Reference.txt\n│   ├── C2_SampleLowerPin.txt\n│   ├── C2_SampleUpperPin.txt\n│   ├── C2_TipLowerPin.txt\n│   └── C2_TipUpperPin.txt\n├── Sample_MW_Pin_comparision.png\n├── Tip_MW_Pin_comparision.png\n└── Tip_Sample_MW_Pin_comparision.png\n```\n\n## Overall Schema\n\n```mermaid\nflowchart TD\n    IOHandler <-- Handle IO operations --> DataLoader;\n    DataLoader <-- Map IO callables --> DataHandler;\n    Qudi[Qudi FitLogic] --> AnalysisLogic;\n    AnalysisLogic -- Inject fit functions --> DataHandler;\n    DataHandler -- Fit data --> Plot;\n    DataHandler -- Structure data --> MeasurementDataclass;\n    MeasurementDataclass -- Plot data --> Plot[JupyterLab Notebook];\n    Plot -- Save plotted data --> DataHandler;\n    style MeasurementDataclass fill: #bbf, stroke: #f66, stroke-width: 2px, color: #fff, stroke-dasharray: 5 5\n```\n\n## License\n\nThis license of this project is located in the top level folder under `LICENSE`. Some specific files contain their\nindividual licenses in the file header docstring.\n\n## Build\n\n### Prerequisites\n\nLatest version of:\n\n- [Poetry](https://python-poetry.org) (recommended) or [conda](https://docs.conda.io/en/latest/miniconda.html) package\n  manager\n- [git](https://git-scm.com/downloads) version control system\n\n### Clone the repository\n\n```shell\ngit clone https://github.com/dineshpinto/qudi-hira-analysis.git\n```\n\n### Installing dependencies with Poetry\n\n```bash\npoetry install\n```\n\n#### Add Poetry environment to Jupyter kernel\n\n```bash\npoetry run python -m ipykernel install --user --name=qudi-hira-analysis\n```\n\n### OR installing dependencies with conda\n\n#### Creating the conda environment\n\n```shell\nconda env create -f tools/conda-env-xx.yml\n```\n\nwhere `xx` is either `win10`, `osx-intel` or `osx-apple-silicon`.\n\n#### Activate conda environment\n\n```shell\nconda activate qudi-hira-analysis\n```\n\n#### Add conda environment to Jupyter kernel\n\n```shell\npython -m ipykernel install --user --name=qudi-hira-analysis\n```\n\n### Start the analysis\n\n#### If installed with Poetry\n\n```shell\npoetry run jupyter lab\n```\n\n#### OR with conda\n\n```shell\njupyter lab\n```\n\nDon\'t forget to switch to the `qudi-hira-analysis` kernel in JupyterLab.\n\n## Makefile\n\nThe Makefile located in `notebooks/` is configured to generate a variety of outputs:\n\n+ `make pdf` : Converts all notebooks to PDF (requires LaTeX backend)\n+ `make html`: Converts all notebooks to HTML\n+ `make py`  : Converts all notebooks to Python (can be useful for VCS)\n+ `make all` : Sequentially runs all the notebooks in folder\n\nTo use the `make` command on Windows you can install [Chocolatey](https://chocolatey.org/install), then\ninstall make with `choco install make`\n',
+    'long_description': '[![DOI](https://zenodo.org/badge/288670453.svg)](https://zenodo.org/badge/latestdoi/288670453)\n[![Downloads](https://pepy.tech/badge/qudi-hira-analysis)](https://pepy.tech/project/qudi-hira-analysis)\n[![PyPi version](https://img.shields.io/pypi/v/qudi-hira-analysis)](https://pypi.python.org/pypi/qudi-hira-analysis/)\n[![Python 3.10](https://img.shields.io/badge/python-3.10-orange.svg)](https://www.python.org/downloads/release/python-3100//)\n[![Python 3.11](https://img.shields.io/badge/python-3.11-orange.svg)](https://www.python.org/downloads/release/python-3110//)\n\n# Qudi Hira Analysis\n\nThis toolkit automates a large portion of the work surrounding data analysis on quantum sensing experiments where the\nprimary raw data extracted is photon counts.\n\nThe high level interface is abstracted, and provides a set of functions to automate data import, handling and analysis.\nIt is designed to be exposed through Jupyter Notebooks, although the abstract interface allows it to be integrated into\nlarger, more general frameworks as well (with only some pain). Using the toolkit itself should only require a\nbeginner-level understanding of Python.\n\nIt also aims to improve transparency and reproducibility in experimental data analysis. In an ideal scenario,\ntwo lines of code are sufficient to recreate all output data.\n\nPython offers some very handy features like dataclasses, which are heavily used by this toolkit. Dataclasses offer a\nfull OOP (object-oriented programming) experience while analyzing complex data sets. They provide a solid and\ntransparent structure to the data to\nreduce errors arising from data fragmentation. This generally comes at a large performance cost, but this is (largely)\nsidestepped by lazy loading data and storing metadata instead wherever possible.\n\n## Installation\n\n```bash\npip install qudi-hira-analysis\n```\n\n## Citation\n\nIf you are publishing scientific results, you can cite this work as:  https://doi.org/10.5281/zenodo.7604670\n\n## Examples\n\nFirst set up the `DataHandler` object (henceforth referred to as `dh`) with the correct paths to the data and figure\nfolders.\n\nEverything revolves around the `dh` object. It is the main interface to the toolkit and is initialized with the\nfollowing required arguments:\n\n- `data_folder` is the main folder where all the data is stored, it can be the direct path to the data, or composed of\n  several sub-folders, each containing the data for a specific measurement\n- `figure_folder` is the folder where the output figures will be saved\n\nOptional arguments:\n\n- `measurement_folder` is the specific sub-folder in `data_folder` where the data for a specific measurement is stored\n\n```python\nfrom pathlib import Path\nimport matplotlib.pyplot as plt\nimport seaborn as sns\n\nfrom qudi_hira_analysis import DataHandler\n\ndh = DataHandler(\n    data_folder=Path("C:\\\\", "Data"),\n    figure_folder=Path("C:\\\\", "QudiHiraAnalysis"),\n    measurement_folder=Path("20230101_NV1")\n)\n```\n\nTo load a specific set of measurements from the data folder, use the `dh.load_measurements()` method, which takes the\nfollowing required arguments:\n\n- `measurement_str` is the string that is used to identify the measurement. It is used to filter the data files in the\n  `data_folder` and `measurement_folder` (if specified)\n\nOptional arguments:\n\n- `qudi` is a boolean. If `True`, the data is assumed to be in the format used by Qudi (default: True)\n- `pulsed` is a boolean. If `True`, the data is assumed to be in the format used by Qudi for pulsed measurements (\n  default: False)\n- `extension` is the extension of the data files (default: ".dat")\n\nThe `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.\n\n- The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.\n\n- The dictionary values are `MeasurementDataclass` objects whose schema is shown\n  visually [here](#measurement-dataclass-schema).\n\n### Example 0: NV-PL measurements\n\n```python\npixel_scanner_measurements = dh.load_measurements(measurement_str="PixelScanner")\n\nfwd, bwd = pixel_scanner_measurements["20230101-0420-00"].data\n\n# If size is known, it can be specified here\nfwd.size["real"] = {"x": 1e-6, "y": 1e-6, "unit": "m"}\n\nfig, ax = plt.subplots()\n\n# Perform (optional) image corrections\nfwd.filter_gaussian(sigma=0.5)\n\n# Add scale bar, color bar and plot the data\nimg = fwd.show(cmap="inferno", ax=ax)\nfwd.add_scale(length=1e-6, ax=ax, height=1)\ncbar = fig.colorbar(img)\ncbar.set_label("NV-PL (kcps)")\n\n# Save the figure to the figure folder specified earlier\ndh.save_figures(filepath="nv_pl_scan", fig=fig, only_jpg=True)\n```\n\n### Example 1: Nanonis AFM measurements\n\n```python\nafm_measurements = dh.load_measurements(measurement_str="Scan", extension=".sxm")\n\nafm = afm_measurements["20230101-0420-00"].data\n\n# Print the channels available in the data\nafm.list_channels()\ntopo = afm.get_channel("Z")\n\nfig, ax = plt.subplots()\n\n# Perform (optional) image corrections\ntopo.correct_lines()\ntopo.correct_plane()\ntopo.filter_lowpass(fft_radius=20)\ntopo.zero_min()\n\n# Add scale bar, color bar and plot the data\nimg = topo.show(cmap="inferno", ax=ax)\ntopo.add_scale(length=1e-6, ax=ax, height=1, fontsize=10)\ncbar = fig.colorbar(img)\ncbar.set_label("Height (nm)")\n\ndh.save_figures(filepath="afm_topo", fig=fig, only_jpg=True)\n``` \n\n### Example 2: Autocorrelation measurements (Antibunching fit)\n\n```python\nautocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")\n\nfig, ax = plt.subplots()\n\nfor autocorrelation in autocorrelation_measurements.values():\n    # Plot the data\n    sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)\n    # Fit the data using the antibunching function\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data,\n                                  fit_function=dh.fit_function.antibunching)\n    # Plot the fit\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax)\n\n# Save the figure to the figure folder specified earlier\ndh.save_figures(filepath="autocorrelation_variation", fig=fig)\n```\n\n### Example 3: ODMR measurements (double Lorentzian fit)\n\n```python\nodmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)\n\nfig, ax = plt.subplots()\n\nfor odmr in odmr_measurements.values():\n    sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,\n                                  fit_function=dh.fit_function.lorentzian_double)\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax)\n\ndh.save_figures(filepath="odmr_variation", fig=fig)\n```\n\n### Example 4: Rabi measurements (sine exponential decay fit)\n\n```python\nrabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)\n\nfig, ax = plt.subplots()\n\nfor rabi in rabi_measurements.values():\n    sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,\n                                  fit_function=dh.fit_function.sineexponentialdecay)\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax)\n\ndh.save_figures(filepath="rabi_variation", fig=fig)\n```\n\n### Example 5: Temperature data\n\n```python\ntemperature_measurements = dh.load_measurements(measurement_str="Temperature")\n\ntemperature = pd.concat([t.data for t in temperature_measurements.values()])\n\nfig, ax = plt.subplots()\nsns.lineplot(data=temperature, x="Time", y="Temperature", ax=ax)\ndh.save_figures(filepath="temperature_monitoring", fig=fig)\n```\n\n## Measurement Dataclass Schema\n\n```mermaid\nflowchart LR\n    subgraph Standard Data\n        MeasurementDataclass --o filepath1[filepath: Path];\n        MeasurementDataclass --o data1[data: DataFrame];\n        MeasurementDataclass --o params1[params: dict];\n        MeasurementDataclass --o timestamp1[timestamp: datetime.datetime];\n        MeasurementDataclass --o methods1[get_param_from_filename: Callable];\n        MeasurementDataclass --o methods2[set_datetime_index: Callable];\n    end\n    subgraph Pulsed Data\n        MeasurementDataclass -- pulsed --> PulsedMeasurementDataclass;\n        PulsedMeasurementDataclass -- measurement --> PulsedMeasurement;\n        PulsedMeasurement --o filepath2[filepath: Path];\n        PulsedMeasurement --o data2[data: DataFrame];\n        PulsedMeasurement --o params2[params: dict];\n        PulsedMeasurementDataclass -- laser_pulses --> LaserPulses;\n        LaserPulses --o filepath3[filepath: Path];\n        LaserPulses --o data3[data: DataFrame];\n        LaserPulses --o params3[params: dict];\n        PulsedMeasurementDataclass -- timetrace --> RawTimetrace;\n        RawTimetrace --o filepath4[filepath: Path];\n        RawTimetrace --o data4[data: DataFrame];\n        RawTimetrace --o params4[params: dict];\n    end\n```\n\n## Supports common fitting routines\n\nTo get the full list of available fit routines, use the `dh.fit_function` attribute. The fit functions are:\n\n| Dimension | Fit                           |\n|-----------|-------------------------------|\n| 1d        | decayexponential              |\n|           | biexponential                 |\n|           | decayexponentialstretched     |\n|           | gaussian                      |\n|           | gaussiandouble                |\n|           | gaussianlinearoffset          |\n|           | hyperbolicsaturation          |\n|           | linear                        |\n|           | lorentzian                    |\n|           | lorentziandouble              |\n|           | lorentziantriple              |\n|           | sine                          |\n|           | sinedouble                    |\n|           | sinedoublewithexpdecay        |\n|           | sinedoublewithtwoexpdecay     |\n|           | sineexponentialdecay          |\n|           | sinestretchedexponentialdecay |\n|           | sinetriple                    |\n|           | sinetriplewithexpdecay        |\n|           | sinetriplewiththreeexpdecay   |\n| 2d        | twoDgaussian                  |\n\n## Inbuilt measurement tree visualizer\n\n```ipython\n>>> dh.data_folder_tree()\n\n# Output\n├── 20211116_NetworkAnalysis_SampleIn_UpperPin.csv\n├── 20211116_NetworkAnalysis_SampleOut_UpperPin.csv\n├── 20211116_NetworkAnalysis_TipIn_LowerPin.csv\n├── 20211116_NetworkAnalysis_TipIn_UpperPin.csv\n├── 20211116_NetworkAnalysis_TipOut_LowerPin.csv\n├── 20211116_NetworkAnalysis_TipOut_UpperPin.csv\n├── ContactTestingMeasurementHead\n│   ├── C2_Reference.txt\n│   ├── C2_SampleLowerPin.txt\n│   ├── C2_SampleUpperPin.txt\n│   ├── C2_TipLowerPin.txt\n│   └── C2_TipUpperPin.txt\n├── Sample_MW_Pin_comparision.png\n├── Tip_MW_Pin_comparision.png\n└── Tip_Sample_MW_Pin_comparision.png\n```\n\n## Overall Schema\n\n```mermaid\nflowchart TD\n    IOHandler <-- Handle IO operations --> DataLoader;\n    DataLoader <-- Map IO callables --> DataHandler;\n    Qudi[Qudi FitLogic] --> AnalysisLogic;\n    AnalysisLogic -- Inject fit functions --> DataHandler;\n    DataHandler -- Fit data --> Plot;\n    DataHandler -- Structure data --> MeasurementDataclass;\n    MeasurementDataclass -- Plot data --> Plot[JupyterLab Notebook];\n    Plot -- Save plotted data --> DataHandler;\n    style MeasurementDataclass fill: #bbf, stroke: #f66, stroke-width: 2px, color: #fff, stroke-dasharray: 5 5\n```\n\n## License\n\nThis license of this project is located in the top level folder under `LICENSE`. Some specific files contain their\nindividual licenses in the file header docstring.\n\n## Build\n\n### Prerequisites\n\nLatest version of:\n\n- [Poetry](https://python-poetry.org) (recommended) or [conda](https://docs.conda.io/en/latest/miniconda.html) package\n  manager\n- [git](https://git-scm.com/downloads) version control system\n\n### Clone the repository\n\n```shell\ngit clone https://github.com/dineshpinto/qudi-hira-analysis.git\n```\n\n### Installing dependencies with Poetry\n\n```bash\npoetry install\n```\n\n#### Add Poetry environment to Jupyter kernel\n\n```bash\npoetry run python -m ipykernel install --user --name=qudi-hira-analysis\n```\n\n### OR installing dependencies with conda\n\n#### Creating the conda environment\n\n```shell\nconda env create -f tools/conda-env-xx.yml\n```\n\nwhere `xx` is either `win10`, `osx-intel` or `osx-apple-silicon`.\n\n#### Activate conda environment\n\n```shell\nconda activate qudi-hira-analysis\n```\n\n#### Add conda environment to Jupyter kernel\n\n```shell\npython -m ipykernel install --user --name=qudi-hira-analysis\n```\n\n### Start the analysis\n\n#### If installed with Poetry\n\n```shell\npoetry run jupyter lab\n```\n\n#### OR with conda\n\n```shell\njupyter lab\n```\n\nDon\'t forget to switch to the `qudi-hira-analysis` kernel in JupyterLab.\n\n## Makefile\n\nThe Makefile located in `notebooks/` is configured to generate a variety of outputs:\n\n+ `make pdf` : Converts all notebooks to PDF (requires LaTeX backend)\n+ `make html`: Converts all notebooks to HTML\n+ `make py`  : Converts all notebooks to Python (can be useful for VCS)\n+ `make all` : Sequentially runs all the notebooks in folder\n\nTo use the `make` command on Windows you can install [Chocolatey](https://chocolatey.org/install), then\ninstall make with `choco install make`\n',
     'author': 'dineshpinto',
     'author_email': 'annual.fallout_0z@icloud.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dineshpinto/qudi-hira-analysis',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qudi_hira_analysis-1.4.2/PKG-INFO` & `qudi_hira_analysis-1.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qudi-hira-analysis
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python toolkit to analzye photon timetrace data from qubit sensors
 Home-page: https://github.com/dineshpinto/qudi-hira-analysis
 License: MIT
 Keywords: python,qubit,analysis,nv centers,photon timetrace
 Author: dineshpinto
 Author-email: annual.fallout_0z@icloud.com
 Requires-Python: >=3.10,<4.0
@@ -104,15 +104,68 @@
 The `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.
 
 - The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.
 
 - The dictionary values are `MeasurementDataclass` objects whose schema is shown
   visually [here](#measurement-dataclass-schema).
 
-### Example 1: Autocorrelation measurements (Antibunching fit)
+### Example 0: NV-PL measurements
+
+```python
+pixel_scanner_measurements = dh.load_measurements(measurement_str="PixelScanner")
+
+fwd, bwd = pixel_scanner_measurements["20230101-0420-00"].data
+
+# If size is known, it can be specified here
+fwd.size["real"] = {"x": 1e-6, "y": 1e-6, "unit": "m"}
+
+fig, ax = plt.subplots()
+
+# Perform (optional) image corrections
+fwd.filter_gaussian(sigma=0.5)
+
+# Add scale bar, color bar and plot the data
+img = fwd.show(cmap="inferno", ax=ax)
+fwd.add_scale(length=1e-6, ax=ax, height=1)
+cbar = fig.colorbar(img)
+cbar.set_label("NV-PL (kcps)")
+
+# Save the figure to the figure folder specified earlier
+dh.save_figures(filepath="nv_pl_scan", fig=fig, only_jpg=True)
+```
+
+### Example 1: Nanonis AFM measurements
+
+```python
+afm_measurements = dh.load_measurements(measurement_str="Scan", extension=".sxm")
+
+afm = afm_measurements["20230101-0420-00"].data
+
+# Print the channels available in the data
+afm.list_channels()
+topo = afm.get_channel("Z")
+
+fig, ax = plt.subplots()
+
+# Perform (optional) image corrections
+topo.correct_lines()
+topo.correct_plane()
+topo.filter_lowpass(fft_radius=20)
+topo.zero_min()
+
+# Add scale bar, color bar and plot the data
+img = topo.show(cmap="inferno", ax=ax)
+topo.add_scale(length=1e-6, ax=ax, height=1, fontsize=10)
+cbar = fig.colorbar(img)
+cbar.set_label("Height (nm)")
+
+dh.save_figures(filepath="afm_topo", fig=fig, only_jpg=True)
+``` 
+
+### Example 2: Autocorrelation measurements (Antibunching fit)
 
 ```python
 autocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")
 
 fig, ax = plt.subplots()
 
 for autocorrelation in autocorrelation_measurements.values():
@@ -124,15 +177,15 @@
     # Plot the fit
     sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
 # Save the figure to the figure folder specified earlier
 dh.save_figures(filepath="autocorrelation_variation", fig=fig)
 ```
 
-### Example 2: ODMR measurements (double Lorentzian 15N fit)
+### Example 3: ODMR measurements (double Lorentzian fit)
 
 ```python
 odmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)
 
 fig, ax = plt.subplots()
 
 for odmr in odmr_measurements.values():
@@ -140,15 +193,15 @@
     fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,
                                   fit_function=dh.fit_function.lorentzian_double)
     sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
 dh.save_figures(filepath="odmr_variation", fig=fig)
 ```
 
-### Example 3: Rabi measurements (sine exponential decay fit)
+### Example 4: Rabi measurements (sine exponential decay fit)
 
 ```python
 rabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)
 
 fig, ax = plt.subplots()
 
 for rabi in rabi_measurements.values():
@@ -156,15 +209,15 @@
     fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,
                                   fit_function=dh.fit_function.sineexponentialdecay)
     sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
 dh.save_figures(filepath="rabi_variation", fig=fig)
 ```
 
-### Example 4: Temperature data
+### Example 5: Temperature data
 
 ```python
 temperature_measurements = dh.load_measurements(measurement_str="Temperature")
 
 temperature = pd.concat([t.data for t in temperature_measurements.values()])
 
 fig, ax = plt.subplots()
```

