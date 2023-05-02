# Comparing `tmp/spectralib-0.0.8.tar.gz` & `tmp/spectralib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralib-0.0.8.tar", last modified: Wed Apr 26 19:55:40 2023, max compression
+gzip compressed data, was "spectralib-0.0.9.tar", last modified: Wed Apr 26 21:54:50 2023, max compression
```

## Comparing `spectralib-0.0.8.tar` & `spectralib-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:55:40.148389 spectralib-0.0.8/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:55:40.144821 spectralib-0.0.8/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1611 2023-04-26 19:07:37.000000 spectralib-0.0.8/README.md
--rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 19:55:40.149907 spectralib-0.0.8/setup.cfg
--rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 19:51:28.000000 spectralib-0.0.8/setup.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:55:39.617206 spectralib-0.0.8/src/
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:55:39.802054 spectralib-0.0.8/src/spectralib/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.8/src/spectralib/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.8/src/spectralib/filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3098 2023-04-26 13:08:36.000000 spectralib-0.0.8/src/spectralib/frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3690 2023-04-26 19:46:00.000000 spectralib-0.0.8/src/spectralib/pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.8/src/spectralib/rfi.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:55:39.928900 spectralib-0.0.8/src/spectralib.egg-info/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:55:39.000000 spectralib-0.0.8/src/spectralib.egg-info/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)      438 2023-04-26 19:55:39.000000 spectralib-0.0.8/src/spectralib.egg-info/SOURCES.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 19:55:39.000000 spectralib-0.0.8/src/spectralib.egg-info/dependency_links.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 19:55:39.000000 spectralib-0.0.8/src/spectralib.egg-info/top_level.txt
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:55:40.110920 spectralib-0.0.8/src/tests/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.8/src/tests/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.8/src/tests/benchmark.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.8/src/tests/test_filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.8/src/tests/test_frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2103 2023-04-26 19:48:19.000000 spectralib-0.0.8/src/tests/test_pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.8/src/tests/test_rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-27 07:11:16.804715 spectralib-0.0.9/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-27 07:11:16.798242 spectralib-0.0.9/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2092 2023-04-26 20:36:56.000000 spectralib-0.0.9/README.md
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-27 07:11:16.807188 spectralib-0.0.9/setup.cfg
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-27 07:10:28.000000 spectralib-0.0.9/setup.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-27 07:11:15.906020 spectralib-0.0.9/src/
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-27 07:11:16.198618 spectralib-0.0.9/src/spectralib/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.9/src/spectralib/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     6919 2023-04-27 07:09:56.000000 spectralib-0.0.9/src/spectralib/filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3098 2023-04-26 13:08:36.000000 spectralib-0.0.9/src/spectralib/frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3690 2023-04-26 19:46:00.000000 spectralib-0.0.9/src/spectralib/pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.9/src/spectralib/rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-27 07:11:16.404976 spectralib-0.0.9/src/spectralib.egg-info/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-27 07:11:15.000000 spectralib-0.0.9/src/spectralib.egg-info/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      438 2023-04-27 07:11:15.000000 spectralib-0.0.9/src/spectralib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-27 07:11:15.000000 spectralib-0.0.9/src/spectralib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-27 07:11:15.000000 spectralib-0.0.9/src/spectralib.egg-info/top_level.txt
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-27 07:11:16.735467 spectralib-0.0.9/src/tests/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.9/src/tests/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.9/src/tests/benchmark.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.9/src/tests/test_filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.9/src/tests/test_frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2103 2023-04-26 19:48:19.000000 spectralib-0.0.9/src/tests/test_pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.9/src/tests/test_rfi.py
```

### Comparing `spectralib-0.0.8/PKG-INFO` & `spectralib-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.8/README.md` & `spectralib-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -34,8 +34,21 @@
  - `git clone https://github.com/jack-white1/SPECTRALib`
  - `cd SPECTRALib/examples`
  - `python example_rfi.py` or `python3 example_rfi.py`
  - `python example_frb.py` or `python3 example_frb.py`
  - `python example_pulsar.py` or `python3 example_pulsar.py`
 
  # Documentation
- 
+ 
+ ## Filterbank Functions
+
+ 
+ ## RFI Functions
+ The RFI modelling in spectralib is designed to be as modular and parametric as possible.
+
+ ## FRB Functions
+To simulate the smearing seen at higher DMs and lower frequencies, there is an optional function to simulate FRBs at a higher resolution than the time and frequency quantization of the filterbank.
+
+ ## Pulsar Functions
+ Conceptually, spectralib models either solitary or binary pulsars as a series of FRBs. 
+ 
+
```

### Comparing `spectralib-0.0.8/setup.py` & `spectralib-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="spectralib",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     classifiers=[
         "Development Status :: 1 - Planning",
     ],
     author="Jack White",
     author_email="jack.white@eng.ox.ac.uk",
```

### Comparing `spectralib-0.0.8/src/spectralib/filterbank.py` & `spectralib-0.0.9/src/spectralib/filterbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     plt.close(fig)  # Close the figure to free up memory
 
 def dedisperse_filterbank_to_timeseries(data, DM, tsamp, foff, fch1):
     dedispersed_data = dedisperse_filterbank(data, DM, tsamp, foff, fch1)
     timeseries = np.sum(dedispersed_data, axis=0)
     return timeseries
 
-
 def dedisperse_filterbank(data, DM, tsamp, foff, fch1):
     nchans, nsamp = data.shape
     dedispersed_data = np.zeros_like(data)
     offsets = calculate_dispersion_offsets(DM, fch1, foff, nchans, tsamp)
 
     for i in range(nchans):
         offset = int(offsets[i])
```

### Comparing `spectralib-0.0.8/src/spectralib/frb.py` & `spectralib-0.0.9/src/spectralib/frb.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.8/src/spectralib/pulsar.py` & `spectralib-0.0.9/src/spectralib/pulsar.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.8/src/spectralib/rfi.py` & `spectralib-0.0.9/src/spectralib/rfi.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.8/src/spectralib.egg-info/PKG-INFO` & `spectralib-0.0.9/src/spectralib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.8/src/tests/benchmark.py` & `spectralib-0.0.9/src/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.8/src/tests/test_filterbank.py` & `spectralib-0.0.9/src/tests/test_filterbank.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.8/src/tests/test_frb.py` & `spectralib-0.0.9/src/tests/test_frb.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.8/src/tests/test_pulsar.py` & `spectralib-0.0.9/src/tests/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.8/src/tests/test_rfi.py` & `spectralib-0.0.9/src/tests/test_rfi.py`

 * *Files identical despite different names*

