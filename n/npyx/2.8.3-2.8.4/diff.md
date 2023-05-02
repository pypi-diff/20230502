# Comparing `tmp/npyx-2.8.3.tar.gz` & `tmp/npyx-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/npyx-2.8.3.tar", last modified: Fri Apr 28 13:30:52 2023, max compression
+gzip compressed data, was "dist/npyx-2.8.4.tar", last modified: Tue May  2 16:46:35 2023, max compression
```

## Comparing `npyx-2.8.3.tar` & `npyx-2.8.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-28 13:30:52.299945 npyx-2.8.3/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.8.3/LICENSE.md
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-28 13:30:52.299945 npyx-2.8.3/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    31591 2023-03-28 09:45:46.000000 npyx-2.8.3/README.md
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-28 13:30:52.295945 npyx-2.8.3/npyx/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      789 2023-04-28 13:29:58.000000 npyx-2.8.3/npyx/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.8.3/npyx/behav.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/circuitProphyler.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   106738 2023-04-20 20:31:09.000000 npyx-2.8.3/npyx/corr.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    28838 2023-04-20 18:33:44.000000 npyx-2.8.3/npyx/datasets.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    56712 2023-04-20 20:40:50.000000 npyx-2.8.3/npyx/feat.py
--rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17109 2023-04-20 18:33:44.000000 npyx-2.8.3/npyx/gl.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38231 2023-04-28 10:55:51.000000 npyx-2.8.3/npyx/h5.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.8.3/npyx/histo.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.8.3/npyx/info.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    49232 2023-04-14 12:13:22.000000 npyx-2.8.3/npyx/inout.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/merger.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.8.3/npyx/metrics.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5152 2023-04-28 13:28:54.000000 npyx-2.8.3/npyx/ml.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   149779 2023-04-25 12:52:34.000000 npyx-2.8.3/npyx/plot.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/preprocess.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    40231 2023-04-23 14:37:23.000000 npyx-2.8.3/npyx/spk_t.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    47559 2023-04-20 18:33:44.000000 npyx-2.8.3/npyx/spk_wvf.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/stats.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/testing.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-24 11:24:27.000000 npyx-2.8.3/npyx/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-28 13:30:52.299945 npyx-2.8.3/npyx.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      492 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/top_level.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-04-28 13:30:52.299945 npyx-2.8.3/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1491 2023-04-14 12:19:49.000000 npyx-2.8.3/setup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-02 16:46:35.062060 npyx-2.8.4/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.8.4/LICENSE.md
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-05-02 16:46:35.062060 npyx-2.8.4/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    31591 2023-03-28 09:45:46.000000 npyx-2.8.4/README.md
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-02 16:46:35.062060 npyx-2.8.4/npyx/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      789 2023-05-02 16:43:42.000000 npyx-2.8.4/npyx/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.8.4/npyx/behav.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.8.4/npyx/circuitProphyler.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   106738 2023-04-20 20:31:09.000000 npyx-2.8.4/npyx/corr.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    28838 2023-04-20 18:33:44.000000 npyx-2.8.4/npyx/datasets.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    56712 2023-04-20 20:40:50.000000 npyx-2.8.4/npyx/feat.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17109 2023-04-20 18:33:44.000000 npyx-2.8.4/npyx/gl.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    39776 2023-05-02 16:40:12.000000 npyx-2.8.4/npyx/h5.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.8.4/npyx/histo.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.8.4/npyx/info.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    49232 2023-04-14 12:13:22.000000 npyx-2.8.4/npyx/inout.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.8.4/npyx/merger.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.8.4/npyx/metrics.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5152 2023-04-28 13:28:54.000000 npyx-2.8.4/npyx/ml.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.8.4/npyx/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   150035 2023-05-01 10:52:10.000000 npyx-2.8.4/npyx/plot.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.8.4/npyx/preprocess.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    40231 2023-04-23 14:37:23.000000 npyx-2.8.4/npyx/spk_t.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    47559 2023-04-20 18:33:44.000000 npyx-2.8.4/npyx/spk_wvf.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.8.4/npyx/stats.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.8.4/npyx/testing.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-24 11:24:27.000000 npyx-2.8.4/npyx/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-02 16:46:35.062060 npyx-2.8.4/npyx.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-05-02 16:46:35.000000 npyx-2.8.4/npyx.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      492 2023-05-02 16:46:35.000000 npyx-2.8.4/npyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-05-02 16:46:35.000000 npyx-2.8.4/npyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2023-05-02 16:46:35.000000 npyx-2.8.4/npyx.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-05-02 16:46:35.000000 npyx-2.8.4/npyx.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-05-02 16:46:35.062060 npyx-2.8.4/setup.cfg
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1491 2023-04-14 12:19:49.000000 npyx-2.8.4/setup.py
```

### Comparing `npyx-2.8.3/LICENSE.md` & `npyx-2.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/PKG-INFO` & `npyx-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.8.3
+Version: 2.8.4
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `npyx-2.8.3/README.md` & `npyx-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/__init__.py` & `npyx-2.8.4/npyx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,10 +36,10 @@
  .behav
  .merger
  .circuitProphyler
  .feat
  .h5
 """
 
-__version__ = "2.8.3"
+__version__ = "2.8.4"
 
 print(f"npyx version {__version__} imported.")
```

### Comparing `npyx-2.8.3/npyx/behav.py` & `npyx-2.8.4/npyx/behav.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/circuitProphyler.py` & `npyx-2.8.4/npyx/circuitProphyler.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/corr.py` & `npyx-2.8.4/npyx/corr.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/datasets.py` & `npyx-2.8.4/npyx/datasets.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/feat.py` & `npyx-2.8.4/npyx/feat.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/gl.py` & `npyx-2.8.4/npyx/gl.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/h5.py` & `npyx-2.8.4/npyx/h5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import gc
 import json
 import re
 import sys
 import time
 import warnings
 from pathlib import Path
+from io import StringIO
+
+import warnings
+warnings.filterwarnings("ignore")
 
 import h5py
 import numpy as np
 from tqdm import tqdm
 
 from npyx.gl import check_periods, get_units
 from npyx.inout import (
@@ -184,15 +188,15 @@
         will result in a key of 'my_note' and a value of "Cool info" being stored in the HDF5 file
         for this unit.
     """
 
     if selective_overwrite is not None:
         assert isinstance(
             selective_overwrite, list
-        ), "Selective_overwrite must be a list of strings."
+        ), "Selective_overwrite must be None or a list of strings."
     else:
         selective_overwrite = []
 
     dp        = Path(dp)
     meta      = read_metadata(dp)
     samp_rate = meta["highpass"]["sampling_rate"]
     # hard-coded parameters
@@ -293,19 +297,19 @@
 
             if optostims is not None:
                 write_to_group(neuron_group, "optostims", optostims)
 
         # sane spikes
         key = "sane_spikes"
         if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite):
-            t = neuron_group["spike_indices"][...]
+            t = neuron_group["spike_indices"][()]
             if sane_spikes is None:
                 if sane_before_opto:
                     if "optostims" in neuron_group:
-                        optostims = neuron_group["optostims"][...]
+                        optostims = neuron_group["optostims"][()]
                     # Only consider spikes 10s before first opto onset
                     end_spont_period = (optostims[0, 0] - 10) * samp_rate
                     sane_spikes = t < end_spont_period
                 elif sane_periods is not None and sane_periods != "all":
                     sane_spikes = (t * 0).astype(bool)
                     for sane_period in sane_periods:
                         sane_spikes = sane_spikes | (t >= sane_period[0] * samp_rate) & (t <= sane_period[1] * samp_rate)
@@ -333,27 +337,30 @@
 
 
         # --------------- waveform-related ---------------#
 
         pbar.set_description(f"Extracting waveform-related data for unit '{relative_unit_path}'...")
         pbar.update(1)
 
-        # make sure that peak channel is reloaded if raw voltage data must be included
-        raw_voltage_keys = ["raw_voltage_snippet", "raw_waveforms"] if include_raw_snippets else []
+        # define fields which are needed to compute anything related
+        # to the extraction of raw data
+        # or the selection of periods from which raw data should be extracted
+        raw_data_keys = [
+            "mean_waveform_preprocessed",
+            "peakchan_SNR",
+            "raw_voltage_snippet",
+            "raw_waveforms",
+            "fn_fp_filtered_spikes",
+            "sane_spikes"]
 
         # extract waveforms (and also load peak channel found by dsmatching)
         keys = [
-            "mean_waveform_preprocessed",
             "channel_ids",
             "channelmap",
-            "amplitudes",
-            "peakchan_SNR",
-            "raw_voltage_snippet",
-            "raw_waveforms",
-        ] + raw_voltage_keys
+            "amplitudes"] + raw_data_keys
         if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
             # must recompute chan_bottom and chan_top - suboptimal, can be rewritten
             dsm_tuple = wvf_dsmatch(dp, unit_id,
                 t_waveforms=waveform_samples, periods=sane_periods,
                 again=again_npyx_wvf, plot_debug=plot_debug,
                 n_waves_used_for_matching=n_waveforms_for_matching,
                 med_sub=True, nRangeMedSub=None)
@@ -370,22 +377,23 @@
             write_to_group(neuron_group, "channel_ids", np.arange(chan_bottom, chan_top, dtype=np.dtype("uint16")))
             write_to_group(neuron_group, "channelmap", cm[chan_bottom:chan_top, 1:3])
 
         # scaling factor
         write_to_group(neuron_group, "scaling_factor", meta["bit_uV_conv_factor"], overwrite_h5)
 
         # Extraction of voltage snippet
-        keys = ["channel_noise_std", "peakchan_SNR", "raw_voltage_snippet"]
+        keys = ["channel_noise_std", "peakchan_SNR", "raw_voltage_snippet", "fn_fp_filtered_spikes", "sane_spikes"]
         if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
             # find optimal window for raw snippet
             if raw_window is None:
-                good_t = neuron_group["spike_indices"][...][neuron_group["fn_fp_filtered_spikes"][...]]
+                good_spikes_m = neuron_group["fn_fp_filtered_spikes"][()] & neuron_group["sane_spikes"][()]
+                good_t = neuron_group["spike_indices"][()][good_spikes_m]
                 # handle cases where there is no good fp/fn section
                 if not np.any(good_t):
-                    good_t = neuron_group["spike_indices"][...]
+                    good_t = neuron_group["spike_indices"][()]
                 raw_window = find_stable_recording_period(
                     good_t,
                     samp_rate,
                     meta["recording_length_seconds"] * samp_rate,
                     target_period = 30,
                     b             = 1000,
                     sd            = 10000,
@@ -397,29 +405,29 @@
                 scale             = False,
                 med_sub           = False,
                 whiten            = False,
                 center_chans_on_0 = False,
                 hpfilt            = False) # already int16
 
         # inclusion of voltage snippet
-        keys = ["raw_voltage_snippet", "voltage_snippet_start_index"]
+        keys = ["raw_voltage_snippet", "voltage_snippet_start_index", "fn_fp_filtered_spikes", "sane_spikes"]
         if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite) and include_raw_snippets:
             raw_snippet_halfrange = np.clip(raw_snippet_halfrange, 0, 10)
             c1                    = max(0, peak_chan_rel - raw_snippet_halfrange)
             c2                    = min(chunk.shape[0] - 1, peak_chan_rel + raw_snippet_halfrange + 1)
             raw_snippet           = chunk[c1:c2, :]
             write_to_group(neuron_group, "raw_voltage_snippet", raw_snippet)  # still centered on peak channel, but half the size
             write_to_group(neuron_group, "voltage_snippet_start_index", int(raw_window[0] * samp_rate))
 
         # extraction of raw waveforms 3d matrix
-        key = "raw_waveforms"
-        if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite) and include_raw_snippets:
+        keys = ["raw_waveforms", "fn_fp_filtered_spikes", "sane_spikes"]
+        if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite) and include_raw_snippets:
             # relect spike ids
             spike_ids  = ids(dp, unit_id, enforced_rp=0)
-            spike_mask = neuron_group["fn_fp_filtered_spikes"][...] & neuron_group["sane_spikes"][...]
+            spike_mask = neuron_group["fn_fp_filtered_spikes"][()] & neuron_group["sane_spikes"][()]
             if np.any(spike_mask):
                 spike_ids = spike_ids[spike_mask]
 
             assert n_raw_waveforms > 0, "n_raw_waveforms must be > 0"
             if len(spike_ids) > n_raw_waveforms:
                 random_ids = np.random.randint(0, spike_ids.shape[0]-1, n_raw_waveforms)
                 spike_ids  = spike_ids[random_ids]
@@ -429,24 +437,24 @@
                                             spike_ids=spike_ids, med_sub_in_time=False,  ignore_ks_chanfilt=True)
             raw_waveforms = raw_waveforms[:, :, chan_bottom:chan_top].transpose(0,2,1)
 
             # recast to int16
             raw_waveforms = raw_waveforms / meta["bit_uV_conv_factor"]
             raw_waveforms = raw_waveforms.astype(np.int16)
 
-            write_to_group(neuron_group, key, raw_waveforms)
+            write_to_group(neuron_group, "raw_waveforms", raw_waveforms)
 
 
         # --------------- quality metrics 2/2 ---------------#
 
         pbar.set_description(f"Computing SNR for unit '{relative_unit_path}'...")
         pbar.update(1)
 
         # SNR
-        keys = ["channel_noise_std", "peakchan_SNR"]
+        keys = ["channel_noise_std", "peakchan_SNR", "fn_fp_filtered_spikes", "sane_spikes"]
         if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
             # both chunk and raw waveforms are in bits (int16)
             mad           = np.median(np.abs(chunk - np.median(chunk, axis=1)[:, None]), axis=1)
             std_estimate  = mad / 0.6745  # Convert to std
             # peakchan_S  = np.ptp(dsm_waveform[:, peak_chan]) #overestimate
             w             = neuron_group["raw_waveforms"][()].mean(0)
             emp_peak_chan = np.argmax(np.ptp(w, axis=1))
@@ -473,23 +481,19 @@
 
 
         # --------------- unit labels ---------------#
 
         pbar.set_description(f"Adding labels for unit '{relative_unit_path}'...")
         pbar.update(1)
         
-        # layer
-        write_to_group(neuron_group, "phyllum_layer",       "", overwrite_h5)
-        write_to_group(neuron_group, "human_layer",         "", overwrite_h5)
-
-        # ground truth labels
-        write_to_group(neuron_group, "expert_label",        "", overwrite_h5)
-        write_to_group(neuron_group, "ground_truth_label",  "", overwrite_h5)
-        write_to_group(neuron_group, "ground_truth_source", "", overwrite_h5)
-        write_to_group(neuron_group, "mli_cluster",         "", overwrite_h5)
+        # layer and ground truth labels
+        for key in ["phyllum_layer", "human_layer",
+                    "expert_label", "ground_truth_label", "ground_truth_source", "mli_cluster"]:
+            if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite):
+                write_to_group(neuron_group, key,       "", overwrite_h5)
 
         pbar.set_description(f"Done with '{relative_unit_path}'.")
         pbar.refresh()
         time.sleep(0.01)
         pbar.close()
 
     return relative_unit_path
@@ -520,15 +524,15 @@
                 "line": "mouseline", # can be anything
                 "dp": "/path/to/dataset", # path to neuropixels dataset
                 "units": [u1, u2, u3, u4], # optotagged/unlabelled units to add to h5
                 "ss": [u5, u6], # simple spikes to add to h5
                 "cs": [u7, u8], # complex spikes to add to h5
                 "sane_periods":{u1:[[t1,t2], [t3,t4]], u2:[], u3:[],
                                 u4:[], u5:[], u6:[], u7:[], u8:[]} # windows of time to use to compute features etc for any particular neuron, in seconds.
-                "global_sane_period": [[t1,t2], [t3,t4]], # windows of time to use to compute features etc for all neurons, in seconds
+                "global_sane_periods": [[t1,t2], [t3,t4]], # windows of time to use to compute features etc for all neurons, in seconds
                 }
         - h5_path: path/to/database_file.h5
         - lab_id: str, lab id. see format at www.tinyurl.com/c4database
         - preprocess_if_raw: bool, whether to high-pass filter the raw data
                              if it is found to be so (for Hull lab)
         - delete_original_data: bool, whether to delete the original raw file if it is preprocessed
                                 according to preprocess_if_raw
@@ -568,25 +572,25 @@
             optolabel = "PkC_ss"
         genetic_line       = ds["line"]
         units              = ds["units"]
         ss                 = ds["ss"]
         cs                 = ds["cs"]
         good_units         = list(get_units(dp, "good", again=True))
         sane_periods_dic   = ds["sane_periods"] if "sane_periods" in ds else {}
-        global_sane_period = sane_periods_dic["global"] if "global_sane_period" in sane_periods_dic else []
+        global_sane_periods = ds["global_sane_periods"] if "global_sane_periods" in ds else []
 
         if include_all_good:
             units_for_h5 = np.unique(units + ss + cs + good_units)
         else:
             units_for_h5 = units + ss + cs
 
         for u in units_for_h5:
             sane_periods = sane_periods_dic[u] if u in sane_periods_dic else None
-            if sane_periods is None and np.any(global_sane_period):
-                sane_periods = global_sane_period
+            if sane_periods is None and np.any(global_sane_periods):
+                sane_periods = global_sane_periods
 
             add_unit_h5(
                 h5_path,
                 dp,
                 u,
                 lab_id,
                 genetic_line=genetic_line,
@@ -752,34 +756,76 @@
         dataset_path = str(Path(relative_unit_path).parent)
         if len(h5_file[dataset_path].keys()) == 0:
             del h5_file[dataset_path]
 
 
 ### h5 vizualisation functions
 
+def get_absolute_neuron_ids(h5_path):
+    h5_contents = print_h5_contents(h5_path, txt_output=False)
+    return [p.split('/')[0] for p in h5_contents if ('_neuron_' in p.split('/')[0])]
+
+def get_neuron_id_dict(h5_path):
+    
+    absolute_neuron_ids = get_absolute_neuron_ids(h5_path)
+
+    neuron_id_dict = {}
+    with h5py.File(h5_path, "r") as hdf:
+        for neuron_id in absolute_neuron_ids:
+
+            neuron_relative_id = int(hdf[neuron_id]['neuron_relative_id'][()])
+            dataset = hdf[neuron_id]['dataset_id'][()].decode()
+
+            relative_id_path = f"datasets/{dataset}/{neuron_relative_id}"
+            neuron_id_dict[neuron_id] = relative_id_path
+
+            if dataset not in neuron_id_dict: neuron_id_dict[dataset] = {}
+            neuron_id_dict[dataset][neuron_relative_id] = neuron_id
 
-def print_h5_contents(h5_path, txt_output=False):
+    return neuron_id_dict
+
+def print_h5_contents(h5_path, display = False, txt_output=False):
     """
     h5_path: str, path to .h5 file
     txt_output: bool, if True prints contents to file
     (same name as h5 name_content.txt)
+
+    Returns:
+        - list of paths in h5 file
     """
     h5_path = Path(h5_path)
     if txt_output:
         txt_output_path = h5_path.parent / f"{h5_path.name[:-3]}_content.txt"
+
+    
     with h5py.File(h5_path, "a") as hdf:
+
+        # save to variable
+        print_output    = StringIO()
+        original_stdout = sys.stdout
+        sys.stdout      = print_output
+        visititems(hdf, visitor_func)
+        print_string   = print_output.getvalue().split('\n')
+        sys.stdout      = original_stdout
+
+        # save to txt file
         if txt_output:
             with open(txt_output_path, "w") as txt:
                 original_stdout = sys.stdout
-                sys.stdout = txt
+                sys.stdout      = txt
                 visititems(hdf, visitor_func)
-                sys.stdout = original_stdout
-        else:
+                sys.stdout      = original_stdout
+
+        # print to console
+        if display:
             visititems(hdf, visitor_func)
 
+    return print_string
+            
+
 
 def visititems(group, func):
     with h5py._hl.base.phil:
 
         def proxy(name):
             """Call the function with the text name, not bytes"""
             name = group._d(name)
```

### Comparing `npyx-2.8.3/npyx/info.py` & `npyx-2.8.4/npyx/info.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/inout.py` & `npyx-2.8.4/npyx/inout.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/merger.py` & `npyx-2.8.4/npyx/merger.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/metrics.py` & `npyx-2.8.4/npyx/metrics.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/ml.py` & `npyx-2.8.4/npyx/ml.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/model.py` & `npyx-2.8.4/npyx/model.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/plot.py` & `npyx-2.8.4/npyx/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,14 +335,16 @@
             "You must provide vmin, vmax and cmap to show a colorbar."
         fig = add_colorbar(fig, ax, None, vmin, vmax,
                  cbar_w, cbar_h, cticks, clabel, clabel_w, clabel_s, cticks_s, cmap) 
 
     if prettify:
         fig.patch.set_facecolor('white')
     if saveFig:
+        if figname is None and title is not None:
+            figname = title
         save_mpl_fig(fig, figname, saveDir, _format, dpi=500)
 
     return fig, ax
 
 def save_mpl_fig(fig, figname, saveDir, _format, dpi=500):
 
     # Fix matplotlib resolution and make text editable
@@ -897,15 +899,15 @@
         return axs
 
 #%% Waveforms or raw data ##############################################################################################
 
 def plot_wvf(dp, u=None, Nchannels=12, chStart=None, n_waveforms=300, t_waveforms=2.8,
              periods='all', spike_ids=None, wvf_batch_size=10, ignore_nwvf=True, again=False,
              whiten=False, med_sub=False, hpfilt=False, hpfiltf=300, nRangeWhiten=None, nRangeMedSub=None,
-             title = '', plot_std=True, plot_mean=True, plot_templates=False, color='dodgerblue',
+             title = None, plot_std=True, plot_mean=True, plot_templates=False, color='dodgerblue',
              labels=False, show_channels=True, scalebar_w=5, ticks_lw=1, sample_lines=0, ylim=[0,0],
              saveDir='~/Downloads', saveFig=False, saveData=False, _format='pdf',
              ignore_ks_chanfilt = True,
              ax_edge_um_x=22, ax_edge_um_y=18, margin=0.12, figw_inch=6, figh_inch=None,
              as_heatmap=False, use_dsmatch=False, verbose=False):
     '''
     To plot main channel alone: use Nchannels=1, chStart=None
@@ -1030,26 +1032,30 @@
         x_tplts = x[(n_samples-tplts.shape[1])//2:(n_samples-tplts.shape[1])//2+tplts.shape[1]] # Plot 82 datapoints between 0 and 82/30 ms
         tplt_chani_rel=peak_chan_i-chStart_i if chStart is None else np.argmax(np.max(datam, 1)-np.min(datam, 1))
     else:
         x_tplts = None
         tplts = None
         tplt_chani_rel = None
 
+    # define a title
+    if title is None:
+        title = f"wvf {int(u)}@{int(cm[peak_chan_i, 0])}"
+
     return plt_wvf(data, subcm, datastd,
              x_tplts, tplts, tplt_chani_rel, fs,
              title, plot_std, plot_mean, plot_templates,
              color, labels, show_channels,
              scalebar_w, ticks_lw, sample_lines, ylim,
              saveDir, saveFig, saveData, _format,
              ax_edge_um_x, ax_edge_um_y, margin,
              figw_inch, figh_inch, as_heatmap)
 
 def plt_wvf(waveforms, subcm=None, waveforms_std=None,
             x_tplts=None, tplts=None, tplt_chani_rel=None, fs=30000,
-            title = '', plot_std=True, plot_mean=True, plot_templates=False,
+            title = None, plot_std=True, plot_mean=True, plot_templates=False,
             color='dodgerblue', labels=False, show_channels=True,
             scalebar_w=5, ticks_lw=1, sample_lines=0, ylim=[0,0],
              saveDir='~/Downloads', saveFig=False, saveData=False, _format='pdf',
              ax_edge_um_x=22, ax_edge_um_y=18, margin=0.12,
              figw_inch=6, figh_inch=None, as_heatmap=False):
     """
     Waveform plotting utility function.
@@ -1194,14 +1200,15 @@
             ax[i_bottomleft].text(0.5, ylim1-0.05*ylimdiff, '1 ms', weight='bold', size=18, va='top', ha='center')
             ax[i_bottomleft].plot([0,0],[ylim1,ylim1+y_scale], c='k', lw=scalebar_w)
             ax[i_bottomleft].text(-0.05*xlimdiff, ylim1+y_scale*0.5, f'{y_scale} \u03bcV', weight='bold', size=18, va='center', ha='right')
 
         fig.suptitle(t=title, x=0.5, y=0.92+0.02*(len(title.split('\n'))-1), size=18, weight='bold', va='top')
 
     # Save figure
+    if title is None: title="waveforms"
     if saveFig:
         save_mpl_fig(fig, title, saveDir, _format)
     if saveData:
         save_np_array(waveforms, title, saveDir)
 
     return fig
 
@@ -1481,15 +1488,15 @@
 
     # Offset data
     plt_offsets = np.arange(0, len(channels)*offset, offset)
     plt_offsets = np.tile(plt_offsets[:,np.newaxis], (1, rc.shape[1]))
     rc+=plt_offsets
 
     fig=plot_raw(dp, times, None, None, channels, filt_key='highpass',
-             offset=450, color=bg_color, lw=lw, bg_alpha=bg_alpha,
+             offset=offset, color=bg_color, lw=lw, bg_alpha=bg_alpha,
              title=title, _format='pdf',  saveDir=saveDir, saveFig=0, figsize=figsize, again=False,
              center_chans_on_0=True, whiten=whiten, med_sub=med_sub, hpfilt=hpfilt, hpfiltf=hpfiltf,
              nRangeWhiten=nRangeWhiten, nRangeMedSub=nRangeMedSub, use_ks_w_matrix=False, ignore_ks_chanfilt=ignore_ks_chanfilt,
              filter_forward=filter_forward, filter_backward=filter_backward,
              plot_ylabels=plot_ylabels, show_allyticks=show_allyticks, yticks_jump=yticks_jump, plot_baselines=False,
              events=events, set0atEvent=set0atEvent,
              ax=ax, ext_data=None, ext_datachans=np.arange(384),
@@ -1521,33 +1528,34 @@
         events=[e-times[0] for e in events] # offset to times[0]
         if set0atEvent:
             tx_ms=tx_ms-events[0]*1000
             events=[e-events[0] for e in events]
 
     for iu, u in enumerate(units):
         print('plotting unit {}...'.format(u))
-        peakChan=get_peak_chan(dp,u, use_template=False)
+        peakChan=get_peak_chan(dp,u, use_template=True)
         assert peakChan in channels, "WARNING the peak channel of {}, {}, is not in the set of channels plotted here!".format(u, peakChan)
         peakChan_rel=np.nonzero(peakChan==channels)[0][0]
         ch1, ch2 = max(0,peakChan_rel-Nchan_plot//2), min(rc.shape[0], peakChan_rel-Nchan_plot//2+Nchan_plot)
         t=trn(dp,u) # in samples
         twin=t[(t>t1+spk_w1)&(t<t2-spk_w2)] # get spikes starting minimum spk_w1 after window start and ending maximum spk_w2 before window end
         twin-=t1 # set t1 as time 0
         for t_spki, t_spk in enumerate(twin):
-            print('plotting spike {}/{}...'.format(t_spki, len(twin)))
+            print('plotting spike {}/{}...'.format(t_spki+1, len(twin)), end='  ')
             spk_id=(tx>=t_spk-spk_w1)&(tx<=t_spk+spk_w2)
             if pyqtgraph:
                 win,p = fig
                 for line in np.arange(ch1, ch2, 1):
                     p.plot(tx_ms[line, spk_id].T, rc[line, spk_id].T, linewidth=1, pen=tuple(npa(colors[iu])*255))
                 fig = win,p
             else:
                 ax.plot(tx_ms[ch1:ch2, spk_id].T, rc[ch1:ch2, spk_id].T, lw=lw_color, color=colors[iu])
                 #ax.plot(tx_ms[peakChan_rel, spk_id].T, rc[peakChan_rel, spk_id].T, lw=1.5, color=color)
                 fig.tight_layout()
+        print("\n")
 
     ax.set_ylim([-offset, rc.max()+offset/2])
 
     if saveFig:
         rcn = '{}_{}_t{}-{}_ch{}-{}'.format(op.basename(dp), list(units), times[0], times[1], channels[0], channels[-1]) # raw chunk name
         rcn=rcn+'_whitened' if whiten else rcn+'_raw'
         if title is not None: rcn=title
@@ -1969,15 +1977,15 @@
     # Plot as 2D grid of PSTHs
     if not as_heatmap:
 
         (nrows, ncols) = (len(events), len(trains)) if not transpose else (len(trains), len(events))
         if overlap_events: (nrows, ncols) = (1,ncols) if not transpose else (nrows, 1)
 
         if figh is None: figh=nrows*1.5 # 10 for 7 is good
-        if figratio is None: figratio=1.2
+        if figratio is None: figratio=3
         figw=figh*(ncols/nrows)*figratio
         figsize=(figw,figh)
 
         # pre-generate figure axes
         fig = plt.figure(figsize=figsize)
         ax_ids=np.arange(nrows*ncols).reshape((nrows,ncols))+1
         axes=ax_ids.copy().astype(object)
```

### Comparing `npyx-2.8.3/npyx/preprocess.py` & `npyx-2.8.4/npyx/preprocess.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/spk_t.py` & `npyx-2.8.4/npyx/spk_t.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/spk_wvf.py` & `npyx-2.8.4/npyx/spk_wvf.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/stats.py` & `npyx-2.8.4/npyx/stats.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/testing.py` & `npyx-2.8.4/npyx/testing.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx/utils.py` & `npyx-2.8.4/npyx/utils.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.3/npyx.egg-info/PKG-INFO` & `npyx-2.8.4/npyx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.8.3
+Version: 2.8.4
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `npyx-2.8.3/setup.py` & `npyx-2.8.4/setup.py`

 * *Files identical despite different names*

