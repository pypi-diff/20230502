# Comparing `tmp/simulateIRAS-0.1.0.post2.tar.gz` & `tmp/simulateIRAS-0.1.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulateIRAS-0.1.0.post2.tar", last modified: Mon May  1 21:06:23 2023, max compression
+gzip compressed data, was "simulateIRAS-0.1.0.post3.tar", last modified: Tue May  2 17:15:49 2023, max compression
```

## Comparing `simulateIRAS-0.1.0.post2.tar` & `simulateIRAS-0.1.0.post3.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.768756 simulateIRAS-0.1.0.post2/
--rw-rw-rw-   0        0        0    35184 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/LICENSE
--rw-rw-rw-   0        0        0       27 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/MANIFEST.in
--rw-rw-rw-   0        0        0      893 2023-05-01 21:06:23.768756 simulateIRAS-0.1.0.post2/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/README.md
--rw-rw-rw-   0        0        0       99 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 21:06:23.768756 simulateIRAS-0.1.0.post2/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-01 21:06:12.000000 simulateIRAS-0.1.0.post2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.757759 simulateIRAS-0.1.0.post2/src/
--rw-rw-rw-   0        0        0        2 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.763755 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/
--rw-rw-rw-   0        0        0      893 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9905 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.767758 simulateIRAS-0.1.0.post2/tests/
--rw-rw-rw-   0        0        0      146 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/tests/test_code.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.602424 simulateIRAS-0.1.0.post3/
+-rw-rw-rw-   0        0        0    35184 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4099 2023-05-02 17:15:49.601424 simulateIRAS-0.1.0.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     3289 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.588424 simulateIRAS-0.1.0.post3/examples/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.593424 simulateIRAS-0.1.0.post3/examples/dataRegression/
+-rw-rw-rw-   0        0        0        6 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/dataRegression/dataRegression.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.594424 simulateIRAS-0.1.0.post3/examples/simpleSimulation/
+-rw-rw-rw-   0        0        0    52782 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/simpleSimulation/IRASTestK.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.595427 simulateIRAS-0.1.0.post3/examples/simpleSimulation/Solutions/
+-rw-rw-rw-   0        0        0   193070 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/simpleSimulation/Solutions/SimulatedIRAS.txt
+-rw-rw-rw-   0        0        0     2402 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/examples/simpleSimulation/simpleSimulation.py
+-rw-rw-rw-   0        0        0       99 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/pyproject.toml
+-rw-rw-rw-   0        0        0      375 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:15:49.602424 simulateIRAS-0.1.0.post3/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-02 17:15:33.000000 simulateIRAS-0.1.0.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.596428 simulateIRAS-0.1.0.post3/src/
+-rw-rw-rw-   0        0        0        2 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.600424 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/
+-rw-rw-rw-   0        0        0     4099 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 17:15:49.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9956 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/src/simulateIRAS.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:49.601424 simulateIRAS-0.1.0.post3/tests/
+-rw-rw-rw-   0        0        0      146 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post3/tests/test_code.py
```

### Comparing `simulateIRAS-0.1.0.post2/LICENSE` & `simulateIRAS-0.1.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post2/setup.py` & `simulateIRAS-0.1.0.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="simulateIRAS",
-    version = '0.1.0-2',
+    version = '0.1.0-3',
     description="A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements",
     py_modules = ["simulateIRAS"],
     package_dir = {'':'src'},
     
     author="coconnor24",
     author_email="coconnor@g.harvard.edu",
```

### Comparing `simulateIRAS-0.1.0.post2/src/simulateIRAS.py` & `simulateIRAS-0.1.0.post3/src/simulateIRAS.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,46 +12,66 @@
 def CalculateResidualAbsoluteDifference(data,sim, weight):
     stepX = np.absolute(data[0][0]-data[0][1])
     diffY0 = np.absolute(data[1]-sim[1]); diffY1 = np.absolute(data[2]-sim[2])
     diffY2 = np.absolute(data[3]-sim[3]); diffY3 = np.absolute(data[4]-sim[4])
     total = (np.sum(diffY0) + np.sum(diffY1)*weight + np.sum(diffY2) + np.sum(diffY3)*weight)*stepX
     return total
 
-def SimulatePolarizationAzimuthSpectra(wavenumber,nVacuum,nSubstrate,nAdsorbate, filmThickness,angle):
+def CalcIndexRefractFromK(kParameters):
+    """
+    Calculates the complex index of refraction from the k parameters (imaginary index of refraction)
+    using a Kramers-Kronig (or Hilbert for mathematicians) transformation
+    
+    Inputs:
+        kParameters: a 2D (3 x n) matrix with k(w) parameters (np.array)
+        
+    Returns:
+        complexIndexRefractAdsorbate: a 2D (3 x n) matrix with the complex index of refraction (np.array)
+    """
+    complexIndexRefractAdsorbateX = ft.hilbert(kParameters[0]) + 1.0j * kParameters[0]
+    complexIndexRefractAdsorbateY = ft.hilbert(kParameters[1]) + 1.0j * kParameters[1]
+    complexIndexRefractAdsorbateZ = ft.hilbert(kParameters[2]) + 1.0j * kParameters[2]
+    complexIndexRefractAdsorbate = np.array([complexIndexRefractAdsorbateX,
+                                  complexIndexRefractAdsorbateY,
+                                  complexIndexRefractAdsorbateZ],
+                                dtype=complex)
+    return complexIndexRefractAdsorbate
+
+def SimulatePolarizationAzimuthSpectra_3Layer(wavenumber,nVacuum,nSubstrate,nAdsorbate, filmThickness,angle):
     """Simulates 4 polarization- and azimuth-resolved spectra
     
     Inputs: 
            wavenumber: a 2D (1 x n) matrix with the simulation wavenumbers (np.array)
            nVacuum: a 2D (3 x n) matrix with the vacuum complex index of refraction (np.array)
            nSubstrate: a 2D (3 x n) matrix with the substrate complex index of refraction (np.array)
            nAdsorbate: a 2D (3 x n) matrix with the adsorbate complex index of refraction (np.array)
            filmThickness: adsorbate layer thickness or approximate coverage as partial layer thickness (np.array)
            angle: light incident to surface normal angle
         
     Returns:
         spectra 4: a 2D matrix (5xn) consisting of wavenumber, S, P, rotate S and rotate P simulated spectra
     """
     
-    spectraS = CalculateSPolarSpectra(wavenumber,
+    spectraS = CalculateSPolarSpectra_3Layer(wavenumber,
                             nVacuum, nSubstrate, nAdsorbate,
                             filmThickness, angle)
-    spectraP = CalculatePPolarSpectra(wavenumber,
+    spectraP = CalculatePPolarSpectra_3Layer(wavenumber,
                             nVacuum, nSubstrate, nAdsorbate,
                             filmThickness, angle)
-    spectraS_rotate = CalculateSPolarSpectra(wavenumber,
+    spectraS_rotate = CalculateSPolarSpectra_3Layer(wavenumber,
                             RotateMatrix(nVacuum), RotateMatrix(nSubstrate), RotateMatrix(nAdsorbate),
                             filmThickness, angle)
-    spectraP_rotate = CalculatePPolarSpectra(wavenumber,
+    spectraP_rotate = CalculatePPolarSpectra_3Layer(wavenumber,
                             RotateMatrix(nVacuum), RotateMatrix(nSubstrate), RotateMatrix(nAdsorbate),
                             filmThickness, angle)
     spectra4 = np.array([wavenumber,spectraS,spectraP,spectraS_rotate,spectraP_rotate])
     return spectra4
 
 # s-polarization from Chabal_1987_(SemiconInterfaces_workshop_full_book), for the k-vector projected into the x-direction on the surface (i.e. electric field in the y-direction on the surface)
-def CalculateSPolarSpectra(wavenumber,refractionVacuum,refractionSubstrate,refractionAdsorbate,filmThickness,angle):
+def CalculateSPolarSpectra_3Layer(wavenumber,refractionVacuum,refractionSubstrate,refractionAdsorbate,filmThickness,angle):
     """Calculates p-polarized IRAS spectra according to Eqn: 2.19 of Chabal YJ (1987) Vibrational Properties at Semiconductor Surfaces and Interfaces. In: Le Lay G, Derrien J, Boccara N (eds) Semiconductor Interfaces: Formation and Properties. Springer Berlin Heidelberg, Berlin, Heidelberg
     Inputs:
            wavenumber: a 2D (1 x n) matrix with the simulation wavenumbers (np.array)
            refractionVacuum: a 2D (3 x n) matrix with the vacuum complex index of refraction (np.array)
            refractionSubstrate: a 2D (3 x n) matrix with the substrate complex index of refraction (np.array)
            refractionAdsorbate: a 2D (3 x n) matrix with the adsorbate complex index of refraction (np.array)
            filmThickness: adsorbate layer thickness or approximate coverage as partial layer thickness (np.array)
@@ -62,15 +82,15 @@
     """
     eVacuum = refractionVacuum**2; eSubstrate = refractionSubstrate**2; eAdsorbate = refractionAdsorbate**2
     Imag = (eSubstrate[1] - eAdsorbate[1]) / (eSubstrate[1]-eVacuum[1])
     deltaRR = 8 * np.pi  * wavenumber * refractionVacuum[1] * filmThickness * np.cos(angle) * np.imag(Imag)
     return deltaRR
 
 # p-polarization from Chabal_1987_(SemiconInterfaces_workshop_full_book), for the k-vector projected into the x-direction on the surface (i.e. electric field in the xz-direction on the surface)
-def CalculatePPolarSpectra(wavenumber,refractionVacuum,refractionSubstrate,refractionAdsorbate,filmThickness,angle):
+def CalculatePPolarSpectra_3Layer(wavenumber,refractionVacuum,refractionSubstrate,refractionAdsorbate,filmThickness,angle):
     """Calculates p-polarized IRAS spectra according to Eqn: 2.27 of Chabal YJ (1987) Vibrational Properties at Semiconductor Surfaces and Interfaces. In: Le Lay G, Derrien J, Boccara N (eds) Semiconductor Interfaces: Formation and Properties. Springer Berlin Heidelberg, Berlin, Heidelberg
     Inputs:
            wavenumber: a 2D (1 x n) matrix with the simulation wavenumbers (np.array)
            refractionVacuum: a 2D (3 x n) matrix with the vacuum complex index of refraction (np.array)
            refractionSubstrate: a 2D (3 x n) matrix with the substrate complex index of refraction (np.array)
            refractionAdsorbate: a 2D (3 x n) matrix with the adsorbate complex index of refraction (np.array)
            filmThickness: adsorbate layer thickness or approximate coverage as partial layer thickness (np.array)
@@ -124,15 +144,15 @@
         constantComplex: a complex expression of the form X + Yj 
         
     Returns:
         a 2D (1 x n) matrix with the complex numbers (np.array)
     """
     return np.full(wavenumberX.shape,yComplex)
        
-def GenerateIsotropic(spectraWavenumber,constantComplex,dimensions = 3):
+def GenerateIsotropicMatrix(spectraWavenumber,constantComplex,dimensions = 3):
     """
     Generates an appropriately sized 3D isotrophic matrix (same dependence based on direction)
     
     Inputs:
         spectraWavenumber: a 2D (1 x n) matrix with the simulation wavenumbers (np.array)
         constantComplex: a complex expression of the form X + Yj 
         dimensions: the number of dimensions to generate for the isotropic matrix (integer)
@@ -141,34 +161,14 @@
         complexMatrix: a mD (m x n) matrix with the complex numbers (np.array)
     """
     complexMatrixX = GenerateConstantComplexMatrix(spectraWavenumber,constantComplex) # Complex Index of Refraction (w) for the vacuum layer in the x-direction
     for n in range (0,dimensions):
         if n == 0: complexMatrix = complexMatrixX
         else:    complexMatrix = np.vstack((complexMatrix,complexMatrixX))
     return complexMatrix
-    
-def CalcIndexRefractFromK(kParameters):
-    """
-    Calculates the complex index of refraction from the k parameters (imaginary index of refraction)
-    using a Kramers-Kronig (or Hilbert for mathematicians) transformation
-    
-    Inputs:
-        kParameters: a 2D (3 x n) matrix with k(w) parameters (np.array)
-        
-    Returns:
-        complexIndexRefractAdsorbate: a 2D (3 x n) matrix with the complex index of refraction (np.array)
-    """
-    complexIndexRefractAdsorbateX = ft.hilbert(kParameters[0]) + 1.0j * kParameters[0]
-    complexIndexRefractAdsorbateY = ft.hilbert(kParameters[1]) + 1.0j * kParameters[1]
-    complexIndexRefractAdsorbateZ = ft.hilbert(kParameters[2]) + 1.0j * kParameters[2]
-    complexIndexRefractAdsorbate = np.array([complexIndexRefractAdsorbateX,
-                                  complexIndexRefractAdsorbateY,
-                                  complexIndexRefractAdsorbateZ],
-                                dtype=complex)
-    return complexIndexRefractAdsorbate
 
 def RotateMatrix(matrix,initial="xyz",final="yxz"):
     """
     Reorders matrix directional component elements according to crystal azimuth rotation
     
     Inputs:
         matrix: a 2D (3 x n) matrix to be rotated (np.array)
```

