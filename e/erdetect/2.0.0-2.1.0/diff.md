# Comparing `tmp/erdetect-2.0.0.tar.gz` & `tmp/erdetect-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdetect-2.0.0.tar", last modified: Tue Apr 11 21:27:05 2023, max compression
+gzip compressed data, was "erdetect-2.1.0.tar", last modified: Tue May  2 18:53:36 2023, max compression
```

## Comparing `erdetect-2.0.0.tar` & `erdetect-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.393794 erdetect-2.0.0/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35823 2022-01-28 21:02:26.000000 erdetect-2.0.0/LICENSE
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-04-11 21:27:05.393972 erdetect-2.0.0/PKG-INFO
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3745 2023-04-11 19:56:10.000000 erdetect-2.0.0/README.md
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.290667 erdetect-2.0.0/erdetect/
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      592 2023-04-11 19:55:20.000000 erdetect-2.0.0/erdetect/__init__.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1318 2022-09-14 18:21:38.000000 erdetect-2.0.0/erdetect/__main__.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46087 2023-04-11 20:29:06.000000 erdetect-2.0.0/erdetect/_erdetect.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.324763 erdetect-2.0.0/erdetect/core/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.0.0/erdetect/core/__init__.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    43840 2022-11-11 02:45:10.000000 erdetect-2.0.0/erdetect/core/config.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    13275 2022-09-13 16:33:39.000000 erdetect-2.0.0/erdetect/core/detection.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.338553 erdetect-2.0.0/erdetect/core/metrics/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3088 2022-09-13 23:06:23.000000 erdetect-2.0.0/erdetect/core/metrics/metric_cross_proj.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3706 2022-09-13 23:06:25.000000 erdetect-2.0.0/erdetect/core/metrics/metric_waveform.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     8720 2022-09-13 16:33:39.000000 erdetect-2.0.0/erdetect/core/peak_finder.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    28038 2023-04-11 20:29:20.000000 erdetect-2.0.0/erdetect/main_cli.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.351941 erdetect-2.0.0/erdetect/utils/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.0.0/erdetect/utils/__init__.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4002 2023-04-11 17:56:08.000000 erdetect-2.0.0/erdetect/utils/misc.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-04-11 16:50:27.000000 erdetect-2.0.0/erdetect/version.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.392319 erdetect-2.0.0/erdetect/views/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:17.000000 erdetect-2.0.0/erdetect/views/__init__.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7934 2022-09-13 16:33:39.000000 erdetect-2.0.0/erdetect/views/output_images.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.296405 erdetect-2.0.0/erdetect.egg-info/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/PKG-INFO
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      605 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/SOURCES.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/dependency_links.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       83 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/requires.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/top_level.txt
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1412 2023-04-11 19:58:59.000000 erdetect-2.0.0/pyproject.toml
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      192 2023-04-11 21:27:05.399132 erdetect-2.0.0/setup.cfg
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:36.006484 erdetect-2.1.0/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35823 2022-01-28 21:02:26.000000 erdetect-2.1.0/LICENSE
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-05-02 18:53:36.006651 erdetect-2.1.0/PKG-INFO
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3745 2023-05-02 18:50:51.000000 erdetect-2.1.0/README.md
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.872543 erdetect-2.1.0/erdetect/
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      645 2023-04-11 21:39:35.000000 erdetect-2.1.0/erdetect/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1318 2022-09-14 18:21:38.000000 erdetect-2.1.0/erdetect/__main__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46285 2023-05-02 18:40:17.000000 erdetect-2.1.0/erdetect/_erdetect.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.920078 erdetect-2.1.0/erdetect/core/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.1.0/erdetect/core/__init__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    43840 2022-11-11 02:45:10.000000 erdetect-2.1.0/erdetect/core/config.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    13275 2022-09-13 16:33:39.000000 erdetect-2.1.0/erdetect/core/detection.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.935451 erdetect-2.1.0/erdetect/core/metrics/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3088 2022-09-13 23:06:23.000000 erdetect-2.1.0/erdetect/core/metrics/metric_cross_proj.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3876 2023-04-22 23:02:05.000000 erdetect-2.1.0/erdetect/core/metrics/metric_waveform.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     8720 2022-09-13 16:33:39.000000 erdetect-2.1.0/erdetect/core/peak_finder.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    28225 2023-04-12 23:50:34.000000 erdetect-2.1.0/erdetect/main_cli.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.945484 erdetect-2.1.0/erdetect/utils/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.1.0/erdetect/utils/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4002 2023-04-11 17:56:08.000000 erdetect-2.1.0/erdetect/utils/misc.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-05-02 18:09:18.000000 erdetect-2.1.0/erdetect/version.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.977898 erdetect-2.1.0/erdetect/views/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:17.000000 erdetect-2.1.0/erdetect/views/__init__.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    26184 2023-05-02 18:51:47.000000 erdetect-2.1.0/erdetect/views/gui.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7934 2022-09-13 16:33:39.000000 erdetect-2.1.0/erdetect/views/output_images.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.886980 erdetect-2.1.0/erdetect.egg-info/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/PKG-INFO
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      688 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       83 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/requires.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/top_level.txt
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1412 2023-05-02 18:52:08.000000 erdetect-2.1.0/pyproject.toml
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      192 2023-05-02 18:53:36.008703 erdetect-2.1.0/setup.cfg
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:36.005727 erdetect-2.1.0/tests/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      968 2023-04-11 21:42:57.000000 erdetect-2.1.0/tests/test_fileio.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       43 2023-04-11 21:43:02.000000 erdetect-2.1.0/tests/test_gui.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      211 2023-04-11 21:42:59.000000 erdetect-2.1.0/tests/test_process.py
```

### Comparing `erdetect-2.0.0/LICENSE` & `erdetect-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/PKG-INFO` & `erdetect-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdetect
-Version: 2.0.0
+Version: 2.1.0
 Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
 Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
 License: GPLv3
 Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
```

### Comparing `erdetect-2.0.0/README.md` & `erdetect-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect/__init__.py` & `erdetect-2.1.0/erdetect/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 if sys.version_info < (3, 8, 0):
     sys.exit("Python 3.8 or later is required.")
 
 # flatten access
 from ieegprep.utils.console import CustomLoggingFormatter
 from erdetect.version import __version__
 from erdetect._erdetect import process_subset
-__all__ = ['process_subset', '__version__']
+from erdetect.views.gui import open_gui
+__all__ = ['process_subset', 'open_gui', '__version__']
 
 # logging
 import logging
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 logger_ch = logging.StreamHandler(stream=sys.stdout)
 logger_ch.setFormatter(CustomLoggingFormatter())
```

### Comparing `erdetect-2.0.0/erdetect/__main__.py` & `erdetect-2.1.0/erdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect/_erdetect.py` & `erdetect-2.1.0/erdetect/_erdetect.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,24 @@
 
     """
 
     # check the input arguments
     if not bids_subset_data_path:
         logging.error('Empty or invalid input data path, make sure to provide a path to subset data (e.g. \'/bids_data_root/subj-01/ieeg/sub-01_run-06.edf\'), exiting...')
         return
+
+    bids_subset_data_path = os.path.abspath(os.path.expanduser(os.path.expandvars(bids_subset_data_path)))
     if not exists(bids_subset_data_path):
         logging.error('Input data path (\'' + bids_subset_data_path + '\') could not be found.\nMake sure to provide a path to subset data (e.g. \'/bids_data_root/subj-01/ieeg/sub-01_run-06.edf\'), exiting...')
         return
+
     if not output_dir:
         logging.error('Empty or invalid output directory, exiting...')
         return
+    output_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(output_dir)))
 
     # derive the bids subset root from the full path
     try:
         bids_subset_root = bids_subset_data_path[:bids_subset_data_path.rindex('_')]
     except ValueError:
         logging.error('Invalid input data path, make sure to provide a path to subset data (e.g. \'/bids_data_root/subj-01/ieeg/sub-01_run-06.edf\'), exiting...')
         return
```

### Comparing `erdetect-2.0.0/erdetect/core/config.py` & `erdetect-2.1.0/erdetect/core/config.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect/core/detection.py` & `erdetect-2.1.0/erdetect/core/detection.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect/core/metrics/metric_cross_proj.py` & `erdetect-2.1.0/erdetect/core/metrics/metric_cross_proj.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect/core/metrics/metric_waveform.py` & `erdetect-2.1.0/erdetect/core/metrics/metric_waveform.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 
     # Design a butterworth (band-pass) filter
     # Note: the 'buttord' output here differs slight from matlab, because the scipy make a change in scipy 0.14.0 where
     #       the choice of which end of the transition region was switched from the stop-band edge to the pass-band edge
     n_band, wn_band = signal.buttord([high_p, low_p], [high_s, low_s], Rp, Rs, True)
     bf_b, bf_a = signal.butter(n_band, wn_band, 'band', analog=False)
 
+    # band-pass can only be performed with enough samples, return nan elsewise
+    if metric_data.shape[0] <= 3 * (max(len(bf_b), len(bf_a)) - 1):
+        return np.nan
+
     # Perform the band-passing
     # Note: custom padlen to match the way matlab does it (-1 is omitted in scipy)
     metric_data = signal.filtfilt(bf_b, bf_a, metric_data, padtype='odd', padlen=3 * (max(len(bf_b), len(bf_a)) - 1))
 
     # calculate the band power using a hilbert transformation
     band_power_sm = np.power(abs(signal.hilbert(metric_data)), 2)
```

### Comparing `erdetect-2.0.0/erdetect/core/peak_finder.py` & `erdetect-2.1.0/erdetect/core/peak_finder.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect/main_cli.py` & `erdetect-2.1.0/erdetect/main_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,17 @@
     logging.info('')
 
 
     #
     # Find and process participants and their datasets
     #
 
+    args.bids_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.bids_dir)))
+    args.output_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.output_dir)))
+
     logging.info('--------------------------------- Participants and data subsets ----------------------------------')
     log_indented_line('BIDS input path:', args.bids_dir)
     log_indented_line('Output path:', args.output_dir)
     logging.info('')
 
     # print optional search arguments
     optional_search_argument = False
```

### Comparing `erdetect-2.0.0/erdetect/utils/misc.py` & `erdetect-2.1.0/erdetect/utils/misc.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect/views/output_images.py` & `erdetect-2.1.0/erdetect/views/output_images.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.0.0/erdetect.egg-info/PKG-INFO` & `erdetect-2.1.0/erdetect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdetect
-Version: 2.0.0
+Version: 2.1.0
 Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
 Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
 License: GPLv3
 Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
```

### Comparing `erdetect-2.0.0/erdetect.egg-info/SOURCES.txt` & `erdetect-2.1.0/erdetect.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,8 +17,12 @@
 erdetect/core/detection.py
 erdetect/core/peak_finder.py
 erdetect/core/metrics/metric_cross_proj.py
 erdetect/core/metrics/metric_waveform.py
 erdetect/utils/__init__.py
 erdetect/utils/misc.py
 erdetect/views/__init__.py
-erdetect/views/output_images.py
+erdetect/views/gui.py
+erdetect/views/output_images.py
+tests/test_fileio.py
+tests/test_gui.py
+tests/test_process.py
```

### Comparing `erdetect-2.0.0/pyproject.toml` & `erdetect-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [project]
 name = "erdetect"
 description = "A package for the automatic detection of evoked responses in SPES/CCEP data"
 readme = "README.md"
 license = { text="GPLv3" }
 requires-python = ">=3.8"
 dependencies = [
-    "ieegprep >= 1.1.0",
+    "ieegprep >= 1.2.0",
     "numpy >= 1.22.3",
     "scipy >= 1.8.0",
     "matplotlib >= 3.5.1",
     "bids_validator >= 1.9.3",
 ]
 keywords = ["evoked response", "detection", "ieeg", "n1", "SPES", "CCEP"]
 authors = [{ name="Max van den Boom", email="m.a.vandenboom84@gmail.com" }]
```

