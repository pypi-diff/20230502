# Comparing `tmp/simulateIRAS-0.1.0.post3.tar.gz` & `tmp/simulateIRAS-0.1.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulateIRAS-0.1.0.post3.tar", last modified: Tue May  2 17:15:49 2023, max compression
+gzip compressed data, was "simulateIRAS-0.1.0.post4.tar", last modified: Tue May  2 19:04:41 2023, max compression
```

## Comparing `simulateIRAS-0.1.0.post3.tar` & `simulateIRAS-0.1.0.post4.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.602424 simulateIRAS-0.1.0.post3/
--rw-rw-rw-   0        0        0    35184 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/LICENSE
--rw-rw-rw-   0        0        0       27 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/MANIFEST.in
--rw-rw-rw-   0        0        0     4099 2023-05-02 17:15:49.601424 simulateIRAS-0.1.0.post3/PKG-INFO
--rw-rw-rw-   0        0        0     3289 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.588424 simulateIRAS-0.1.0.post3/examples/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.593424 simulateIRAS-0.1.0.post3/examples/dataRegression/
--rw-rw-rw-   0        0        0        6 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/dataRegression/dataRegression.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.594424 simulateIRAS-0.1.0.post3/examples/simpleSimulation/
--rw-rw-rw-   0        0        0    52782 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/simpleSimulation/IRASTestK.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.595427 simulateIRAS-0.1.0.post3/examples/simpleSimulation/Solutions/
--rw-rw-rw-   0        0        0   193070 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/simpleSimulation/Solutions/SimulatedIRAS.txt
--rw-rw-rw-   0        0        0     2402 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/simpleSimulation/simpleSimulation.py
--rw-rw-rw-   0        0        0       99 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/pyproject.toml
--rw-rw-rw-   0        0        0      375 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 17:15:49.602424 simulateIRAS-0.1.0.post3/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-02 17:15:33.000000 simulateIRAS-0.1.0.post3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.596428 simulateIRAS-0.1.0.post3/src/
--rw-rw-rw-   0        0        0        2 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.600424 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/
--rw-rw-rw-   0        0        0     4099 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9956 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.601424 simulateIRAS-0.1.0.post3/tests/
--rw-rw-rw-   0        0        0      146 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/tests/test_code.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.324933 simulateIRAS-0.1.0.post4/
+-rw-rw-rw-   0        0        0    35184 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4099 2023-05-02 19:04:41.323928 simulateIRAS-0.1.0.post4/PKG-INFO
+-rw-rw-rw-   0        0        0     3289 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.293928 simulateIRAS-0.1.0.post4/examples/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.299929 simulateIRAS-0.1.0.post4/examples/dataRegression/
+-rw-rw-rw-   0        0        0     8080 2023-05-02 18:56:34.000000 simulateIRAS-0.1.0.post4/examples/dataRegression/dataRegression.py
+-rw-rw-rw-   0        0        0     8096 2023-05-02 18:58:36.000000 simulateIRAS-0.1.0.post4/examples/dataRegression/dataRegression2.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.306928 simulateIRAS-0.1.0.post4/examples/simpleSimulation/
+-rw-rw-rw-   0        0        0    52782 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/IRASTestK.txt
+-rw-rw-rw-   0        0        0   193070 2023-05-02 17:24:17.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/SimulatedIRAS.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.307929 simulateIRAS-0.1.0.post4/examples/simpleSimulation/Solutions/
+-rw-rw-rw-   0        0        0   193070 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/Solutions/SimulatedIRAS.txt
+-rw-rw-rw-   0        0        0     2862 2023-05-02 18:48:22.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/simpleSimulation.py
+-rw-rw-rw-   0        0        0       99 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/pyproject.toml
+-rw-rw-rw-   0        0        0      375 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 19:04:41.324933 simulateIRAS-0.1.0.post4/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-02 19:04:20.000000 simulateIRAS-0.1.0.post4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.308929 simulateIRAS-0.1.0.post4/src/
+-rw-rw-rw-   0        0        0        2 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.322929 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/
+-rw-rw-rw-   0        0        0     4099 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10027 2023-05-02 19:03:40.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.323928 simulateIRAS-0.1.0.post4/tests/
+-rw-rw-rw-   0        0        0      146 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/tests/test_code.py
```

### Comparing `simulateIRAS-0.1.0.post3/LICENSE` & `simulateIRAS-0.1.0.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post3/PKG-INFO` & `simulateIRAS-0.1.0.post4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0.post3
+Version: 0.1.0.post4
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simulateIRAS-0.1.0.post3/README.md` & `simulateIRAS-0.1.0.post4/README.md`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post3/examples/simpleSimulation/IRASTestK.txt` & `simulateIRAS-0.1.0.post4/examples/simpleSimulation/IRASTestK.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post3/examples/simpleSimulation/Solutions/SimulatedIRAS.txt` & `simulateIRAS-0.1.0.post4/examples/simpleSimulation/SimulatedIRAS.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post3/examples/simpleSimulation/simpleSimulation.py` & `simulateIRAS-0.1.0.post4/examples/simpleSimulation/simpleSimulation.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,18 +32,32 @@
 
 # Simulates the 4 polarization- and azimuth-resolved IRAS spectra
 simulatedSpectra = iras.SimulatePolarizationAzimuthSpectra_3Layer(simulationWavenumber,
                         nVacuum, nSubstrate, nAdsorbate,
                         filmThickness, angle)
 simulatedSpectra = simulatedSpectra.real
 
-# Plots the 4 polarization- and azimuth-resolved IRAS spectra
+# Plots the k parameters IRAS spectra
 plt.figure(0); plt.clf()
 plt.xlabel("$\mathregular{Wavenumber\ (cm^{-1})}$")
 plt.ylabel("$\mathregular{\Delta R / R}$")
+plt.plot(simulationWavenumber, dataK[0],label="k(x))")
+plt.plot(simulationWavenumber, dataK[1],label="k(y)")
+plt.plot(simulationWavenumber, dataK[2],label="k(z)")
+plt.xlim(1900, 3000)
+plt.legend()
+plt.tight_layout()
+plt.ion()
+plt.show()
+plt.savefig("Figure0.png", dpi=300, format='png')
+
+# Plots the 4 polarization- and azimuth-resolved IRAS spectra
+plt.figure(1); plt.clf()
+plt.xlabel("$\mathregular{Wavenumber\ (cm^{-1})}$")
+plt.ylabel("$\mathregular{\Delta R / R}$")
 plt.plot(simulatedSpectra[0], simulatedSpectra[1],label="s(y)")
 plt.plot(simulatedSpectra[0], simulatedSpectra[2],label="p(xz)")
 plt.plot(simulatedSpectra[0], simulatedSpectra[3],label="s(x)")
 plt.plot(simulatedSpectra[0], simulatedSpectra[4],label="p(yz)")
 plt.xlim(1900, 3000)
 plt.legend()
 plt.tight_layout()
```

### Comparing `simulateIRAS-0.1.0.post3/setup.py` & `simulateIRAS-0.1.0.post4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="simulateIRAS",
-    version = '0.1.0-3',
+    version = '0.1.0-4',
     description="A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements",
     py_modules = ["simulateIRAS"],
     package_dir = {'':'src'},
     
     author="coconnor24",
     author_email="coconnor@g.harvard.edu",
```

### Comparing `simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/PKG-INFO` & `simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0.post3
+Version: 0.1.0.post4
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simulateIRAS-0.1.0.post3/src/simulateIRAS.py` & `simulateIRAS-0.1.0.post4/src/simulateIRAS.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import scipy.fftpack as ft
 
 
 def ImportSpectra(file):
     data = np.genfromtxt(file,dtype=float, unpack=True, delimiter=",", skip_header=True)
     return(data)
     
-def CalculateResidualAbsoluteDifference(data,sim, weight):
-    stepX = np.absolute(data[0][0]-data[0][1])
+def CalculateResidualAbsoluteDifference(data,sim, weightS, weightP):
+    stepX = np.absolute(data[0][0]-data[0][1]); numXsteps = length(data[0])
     diffY0 = np.absolute(data[1]-sim[1]); diffY1 = np.absolute(data[2]-sim[2])
     diffY2 = np.absolute(data[3]-sim[3]); diffY3 = np.absolute(data[4]-sim[4])
-    total = (np.sum(diffY0) + np.sum(diffY1)*weight + np.sum(diffY2) + np.sum(diffY3)*weight)*stepX
+    total = (np.sum(diffY0)*weightS + np.sum(diffY1)*weightP + np.sum(diffY2)*weightS + np.sum(diffY3)*weightP)*stepX*(numXsteps-1)
     return total
 
 def CalcIndexRefractFromK(kParameters):
     """
     Calculates the complex index of refraction from the k parameters (imaginary index of refraction)
     using a Kramers-Kronig (or Hilbert for mathematicians) transformation
```

