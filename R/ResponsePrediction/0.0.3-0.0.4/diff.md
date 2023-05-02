# Comparing `tmp/ResponsePrediction-0.0.3.tar.gz` & `tmp/ResponsePrediction-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ResponsePrediction-0.0.3.tar", last modified: Sat Apr 22 12:13:11 2023, max compression
+gzip compressed data, was "ResponsePrediction-0.0.4.tar", last modified: Tue May  2 11:54:25 2023, max compression
```

## Comparing `ResponsePrediction-0.0.3.tar` & `ResponsePrediction-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:13:11.124506 ResponsePrediction-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 12:12:59.000000 ResponsePrediction-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-04-22 12:13:11.124506 ResponsePrediction-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 12:12:59.000000 ResponsePrediction-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-22 12:12:59.000000 ResponsePrediction-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:13:11.124506 ResponsePrediction-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:13:11.124506 ResponsePrediction-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:13:11.124506 ResponsePrediction-0.0.3/src/ResponsePrediction/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-22 12:13:04.000000 ResponsePrediction-0.0.3/src/ResponsePrediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-22 12:12:59.000000 ResponsePrediction-0.0.3/src/ResponsePrediction/_deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-22 12:12:59.000000 ResponsePrediction-0.0.3/src/ResponsePrediction/_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-22 12:12:59.000000 ResponsePrediction-0.0.3/src/ResponsePrediction/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:13:11.124506 ResponsePrediction-0.0.3/src/ResponsePrediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-04-22 12:13:11.000000 ResponsePrediction-0.0.3/src/ResponsePrediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-22 12:13:11.000000 ResponsePrediction-0.0.3/src/ResponsePrediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:13:11.000000 ResponsePrediction-0.0.3/src/ResponsePrediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 12:13:11.000000 ResponsePrediction-0.0.3/src/ResponsePrediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 12:13:11.000000 ResponsePrediction-0.0.3/src/ResponsePrediction.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/src/ResponsePrediction/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-02 11:54:19.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/_deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/top_level.txt
```

### Comparing `ResponsePrediction-0.0.3/LICENSE` & `ResponsePrediction-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ResponsePrediction-0.0.3/PKG-INFO` & `ResponsePrediction-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResponsePrediction
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vessel wave-induced response prediction
 Author-email: Jan-Erik Hygen <j-e.hygen@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ResponsePrediction-0.0.3/pyproject.toml` & `ResponsePrediction-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ResponsePrediction-0.0.3/src/ResponsePrediction/_deterministic.py` & `ResponsePrediction-0.0.4/src/ResponsePrediction/_deterministic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from scipy.linalg import toeplitz
+from scipy.interpolate import interp1d
 import ResponsePrediction._tools as rt
 
 class Autocorrelation():
     """Response prediction using the measured autocorrelation function.
     
     Procedures
     ----------
@@ -144,27 +145,84 @@
     t0 : float
         The start point of measurement
     beta : float
         The wave direction. It is defined in the North-East-Down frame as waves going to.
         beta = 0.0 corresponds to waves coming from south moving north, and beta=pi the opposit.
     g : float
         Gravitational acceleration.
+    rao_amp : array_like
+        Array of vessel motion RAOs (m/m or rad/m) for each DOF.
+    rao_phase : array_like
+        Array of vessel motion RAO phase for each DOF. The prediction method use phase lag convention.
+        Make sure that the input RAO phase follows the same convention.
+    rao_freq : array_like
+        Array of frequencies used in motion RAO computation. 
     """
-    def __init__(self, t0, t_pred, wavedir):
+    def __init__(self, t0, t_pred, wavedir: float, rao_amp, rao_phase, rao_freq, rao_headings):
         self.t0 = t0
         self.t_pred = t_pred
         self.beta = wavedir
         self.g = 9.81
+        self.rao_amp = rao_amp
+        self.rao_phase = rao_phase
+        self.rao_freqs_rad = rao_freq
+        self.rao_headings = rao_headings
 
     def __call__(self, wave_measurement, fs=100, x=0):
         """Calculate an estimate of the wave elevation at a point x based on a measurement
         of the wave elevation."""
         self._wave_reconstruction(wave_measurement, fs)
-        return np.sum(np.real(self.amp*np.cos(self.w*self.t_pred[:, None] - self.k*np.cos(self.beta)*x)), axis=1)
+        return np.sum(np.real(self.amp*np.exp(1j*(self.w*self.t_pred[:, None] - self.k*np.cos(self.beta)*x))), axis=1)
+    
+    def motion_prediction(self, wave_measurement, dof=3, fs=100, x=0, psi=0):
+        self._wave_reconstruction(wave_measurement, fs)
+        _, rao_amp, rao_phase = self._set_raos(self.w, dof, psi)
+        return np.sum(
+            np.real(
+                self.amp*rao_amp*np.exp(1j*(self.w*self.t_pred[:, None] - self.k*np.cos(self.beta)*x - rao_phase))
+            ),
+            axis=1
+        )
 
     def _wave_reconstruction(self, wave_measurement, fs=100):
         # Use the FFT to obtain the phase-resolved wave
         zeta_hat = np.fft.rfft(wave_measurement)
         f_hat = np.fft.rfftfreq(n=wave_measurement.size, d=1/fs)
         self.w = f_hat*2*np.pi
         self.k = self.w**2/self.g
-        self.amp = zeta_hat
+        self.amp = zeta_hat/zeta_hat.size
+
+    def _set_raos(self, freqs, dof, psi):
+        rao_amp_interp_freq = interp1d(
+            self.rao_freqs_rad,
+            self.rao_amp,
+            axis=1,
+            bounds_error=False,
+            fill_value=(self.rao_amp[:, 0, :], 0)
+        )
+        rao_phase_interp_freq = interp1d(
+            self.rao_freqs_rad,
+            self.rao_phase,
+            axis=1,
+            bounds_error=False,
+            fill_value=(0, self.rao_phase[:, -1, :])
+        )
+        new_rao_amp = rao_amp_interp_freq(freqs)
+        new_rao_phase = rao_phase_interp_freq(freqs)
+
+        rao_amp_interp_angle = interp1d(
+            self.rao_headings,
+            new_rao_amp,
+            axis=2
+        )
+        rao_phase_interp_angle = interp1d(
+            self.rao_headings,
+            new_rao_phase,
+            axis=2
+        )
+        rel_angle_pipi = np.mod(self.beta - psi + np.pi, 2*np.pi) - np.pi
+        rel_angle_pos = np.where(rel_angle_pipi < 0, rel_angle_pipi + 2*np.pi, rel_angle_pipi)
+        rao = rao_amp_interp_angle(rel_angle_pos)
+        phase = rao_phase_interp_angle(rel_angle_pos)
+        print(rao.shape)
+        print(f"Relative angle: {np.rad2deg(rel_angle_pos)}")
+        return freqs, rao[dof-1], phase[dof-1]
```

### Comparing `ResponsePrediction-0.0.3/src/ResponsePrediction/_stochastic.py` & `ResponsePrediction-0.0.4/src/ResponsePrediction/_stochastic.py`

 * *Files identical despite different names*

### Comparing `ResponsePrediction-0.0.3/src/ResponsePrediction.egg-info/PKG-INFO` & `ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResponsePrediction
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vessel wave-induced response prediction
 Author-email: Jan-Erik Hygen <j-e.hygen@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

