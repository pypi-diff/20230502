# Comparing `tmp/simulateIRAS-0.1.0.post4.tar.gz` & `tmp/simulateIRAS-0.1.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulateIRAS-0.1.0.post4.tar", last modified: Tue May  2 19:04:41 2023, max compression
+gzip compressed data, was "simulateIRAS-0.1.0.post5.tar", last modified: Tue May  2 19:13:36 2023, max compression
```

## Comparing `simulateIRAS-0.1.0.post4.tar` & `simulateIRAS-0.1.0.post5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.324933 simulateIRAS-0.1.0.post4/
--rw-rw-rw-   0        0        0    35184 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/LICENSE
--rw-rw-rw-   0        0        0       27 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/MANIFEST.in
--rw-rw-rw-   0        0        0     4099 2023-05-02 19:04:41.323928 simulateIRAS-0.1.0.post4/PKG-INFO
--rw-rw-rw-   0        0        0     3289 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.293928 simulateIRAS-0.1.0.post4/examples/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.299929 simulateIRAS-0.1.0.post4/examples/dataRegression/
--rw-rw-rw-   0        0        0     8080 2023-05-02 18:56:34.000000 simulateIRAS-0.1.0.post4/examples/dataRegression/dataRegression.py
--rw-rw-rw-   0        0        0     8096 2023-05-02 18:58:36.000000 simulateIRAS-0.1.0.post4/examples/dataRegression/dataRegression2.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.306928 simulateIRAS-0.1.0.post4/examples/simpleSimulation/
--rw-rw-rw-   0        0        0    52782 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/IRASTestK.txt
--rw-rw-rw-   0        0        0   193070 2023-05-02 17:24:17.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/SimulatedIRAS.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.307929 simulateIRAS-0.1.0.post4/examples/simpleSimulation/Solutions/
--rw-rw-rw-   0        0        0   193070 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/Solutions/SimulatedIRAS.txt
--rw-rw-rw-   0        0        0     2862 2023-05-02 18:48:22.000000 simulateIRAS-0.1.0.post4/examples/simpleSimulation/simpleSimulation.py
--rw-rw-rw-   0        0        0       99 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/pyproject.toml
--rw-rw-rw-   0        0        0      375 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 19:04:41.324933 simulateIRAS-0.1.0.post4/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-02 19:04:20.000000 simulateIRAS-0.1.0.post4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.308929 simulateIRAS-0.1.0.post4/src/
--rw-rw-rw-   0        0        0        2 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.322929 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/
--rw-rw-rw-   0        0        0     4099 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 19:04:41.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10027 2023-05-02 19:03:40.000000 simulateIRAS-0.1.0.post4/src/simulateIRAS.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:04:41.323928 simulateIRAS-0.1.0.post4/tests/
--rw-rw-rw-   0        0        0      146 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post4/tests/test_code.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.753524 simulateIRAS-0.1.0.post5/
+-rw-rw-rw-   0        0        0    35184 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4099 2023-05-02 19:13:36.753524 simulateIRAS-0.1.0.post5/PKG-INFO
+-rw-rw-rw-   0        0        0     3289 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.731524 simulateIRAS-0.1.0.post5/examples/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.738524 simulateIRAS-0.1.0.post5/examples/dataRegression/
+-rw-rw-rw-   0        0        0     8080 2023-05-02 18:56:34.000000 simulateIRAS-0.1.0.post5/examples/dataRegression/dataRegression.py
+-rw-rw-rw-   0        0        0     8096 2023-05-02 18:58:36.000000 simulateIRAS-0.1.0.post5/examples/dataRegression/dataRegression2.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.740523 simulateIRAS-0.1.0.post5/examples/simpleSimulation/
+-rw-rw-rw-   0        0        0    52782 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/IRASTestK.txt
+-rw-rw-rw-   0        0        0   193070 2023-05-02 17:24:17.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/SimulatedIRAS.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.740523 simulateIRAS-0.1.0.post5/examples/simpleSimulation/Solutions/
+-rw-rw-rw-   0        0        0   193070 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/Solutions/SimulatedIRAS.txt
+-rw-rw-rw-   0        0        0     2862 2023-05-02 18:48:22.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/simpleSimulation.py
+-rw-rw-rw-   0        0        0       99 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/pyproject.toml
+-rw-rw-rw-   0        0        0      375 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 19:13:36.753524 simulateIRAS-0.1.0.post5/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-02 19:13:19.000000 simulateIRAS-0.1.0.post5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.742523 simulateIRAS-0.1.0.post5/src/
+-rw-rw-rw-   0        0        0        2 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.752524 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/
+-rw-rw-rw-   0        0        0     4099 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10024 2023-05-02 19:13:05.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.752524 simulateIRAS-0.1.0.post5/tests/
+-rw-rw-rw-   0        0        0      146 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/tests/test_code.py
```

### Comparing `simulateIRAS-0.1.0.post4/LICENSE` & `simulateIRAS-0.1.0.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/PKG-INFO` & `simulateIRAS-0.1.0.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0.post4
+Version: 0.1.0.post5
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simulateIRAS-0.1.0.post4/README.md` & `simulateIRAS-0.1.0.post5/README.md`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/examples/dataRegression/dataRegression.py` & `simulateIRAS-0.1.0.post5/examples/dataRegression/dataRegression.py`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/examples/dataRegression/dataRegression2.py` & `simulateIRAS-0.1.0.post5/examples/dataRegression/dataRegression2.py`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/examples/simpleSimulation/IRASTestK.txt` & `simulateIRAS-0.1.0.post5/examples/simpleSimulation/IRASTestK.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/examples/simpleSimulation/SimulatedIRAS.txt` & `simulateIRAS-0.1.0.post5/examples/simpleSimulation/SimulatedIRAS.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/examples/simpleSimulation/Solutions/SimulatedIRAS.txt` & `simulateIRAS-0.1.0.post5/examples/simpleSimulation/Solutions/SimulatedIRAS.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/examples/simpleSimulation/simpleSimulation.py` & `simulateIRAS-0.1.0.post5/examples/simpleSimulation/simpleSimulation.py`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/setup.py` & `simulateIRAS-0.1.0.post5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="simulateIRAS",
-    version = '0.1.0-4',
+    version = '0.1.0-5',
     description="A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements",
     py_modules = ["simulateIRAS"],
     package_dir = {'':'src'},
     
     author="coconnor24",
     author_email="coconnor@g.harvard.edu",
```

### Comparing `simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/PKG-INFO` & `simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0.post4
+Version: 0.1.0.post5
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simulateIRAS-0.1.0.post4/src/simulateIRAS.egg-info/SOURCES.txt` & `simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post4/src/simulateIRAS.py` & `simulateIRAS-0.1.0.post5/src/simulateIRAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def ImportSpectra(file):
     data = np.genfromtxt(file,dtype=float, unpack=True, delimiter=",", skip_header=True)
     return(data)
     
 def CalculateResidualAbsoluteDifference(data,sim, weightS, weightP):
-    stepX = np.absolute(data[0][0]-data[0][1]); numXsteps = length(data[0])
+    stepX = np.absolute(data[0][0]-data[0][1]); numXsteps = len(data[0])
     diffY0 = np.absolute(data[1]-sim[1]); diffY1 = np.absolute(data[2]-sim[2])
     diffY2 = np.absolute(data[3]-sim[3]); diffY3 = np.absolute(data[4]-sim[4])
     total = (np.sum(diffY0)*weightS + np.sum(diffY1)*weightP + np.sum(diffY2)*weightS + np.sum(diffY3)*weightP)*stepX*(numXsteps-1)
     return total
 
 def CalcIndexRefractFromK(kParameters):
     """
```

