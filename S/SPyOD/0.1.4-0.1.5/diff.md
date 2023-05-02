# Comparing `tmp/SPyOD-0.1.4.tar.gz` & `tmp/SPyOD-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPyOD-0.1.4.tar", last modified: Tue Mar  7 10:17:09 2023, max compression
+gzip compressed data, was "SPyOD-0.1.5.tar", last modified: Tue May  2 13:03:53 2023, max compression
```

## Comparing `SPyOD-0.1.4.tar` & `SPyOD-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:17:09.072539 SPyOD-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-07 10:16:58.000000 SPyOD-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-07 10:17:09.068539 SPyOD-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-07 10:16:58.000000 SPyOD-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-07 10:16:58.000000 SPyOD-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 10:17:09.072539 SPyOD-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:17:09.068539 SPyOD-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:17:09.068539 SPyOD-0.1.4/src/SPyOD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-07 10:17:09.000000 SPyOD-0.1.4/src/SPyOD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-07 10:17:09.000000 SPyOD-0.1.4/src/SPyOD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 10:17:09.000000 SPyOD-0.1.4/src/SPyOD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-07 10:17:09.000000 SPyOD-0.1.4/src/SPyOD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:17:09.068539 SPyOD-0.1.4/src/spyod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 10:16:58.000000 SPyOD-0.1.4/src/spyod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-03-07 10:16:58.000000 SPyOD-0.1.4/src/spyod/findpairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-03-07 10:16:58.000000 SPyOD-0.1.4/src/spyod/spod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-02 13:03:44.000000 SPyOD-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-02 13:03:53.646647 SPyOD-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-02 13:03:44.000000 SPyOD-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 13:03:44.000000 SPyOD-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:03:53.646647 SPyOD-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/src/SPyOD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/src/spyod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:44.000000 SPyOD-0.1.5/src/spyod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-02 13:03:44.000000 SPyOD-0.1.5/src/spyod/findpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-05-02 13:03:44.000000 SPyOD-0.1.5/src/spyod/spod.py
```

### Comparing `SPyOD-0.1.4/LICENSE` & `SPyOD-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.4/PKG-INFO` & `SPyOD-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SPyOD
-Version: 0.1.4
+Version: 0.1.5
 Summary: Spectral Proper Orthogonal Decomposition
-Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>
+Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber <moritz.sieber@tu-berlin.de>
 Project-URL: Homepage, https://github.com/grigorishat/SPyOD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: SPyOD Version: 0.1.4 Summary: Spectral Proper
+Metadata-Version: 2.1 Name: SPyOD Version: 0.1.5 Summary: Spectral Proper
 Orthogonal Decomposition Author-email: Grigorios Hatzissawidis
-hatzissawidis@fst.tu-darmstadt.de> Project-URL: Homepage, https://github.com/
-grigorishat/SPyOD Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE # Spectral Proper Orthogonal Decomposition ## Table of
-contents * [Description](#description) * [Installation](#installation) *
-[License](#license) * [Contact us](#contact-us) * [Contributors](#contributors)
-## Description __SPyOD__ is the python implementation of the Spectral Proper
+hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber
+sieber@tu-berlin.de> Project-URL: Homepage, https://github.com/grigorishat/
+SPyOD Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE # Spectral Proper Orthogonal Decomposition ## Table of contents *
+[Description](#description) * [Installation](#installation) * [License]
+(#license) * [Contact us](#contact-us) * [Contributors](#contributors) ##
+Description __SPyOD__ is the python implementation of the Spectral Proper
 Orthogonal Decomposition published by [Sieber et al. in 2016](https://
 www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/spectral-
 proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A). It includes
 two __.py-files__: - `spod.py` - Includes the function `spod` which calculates
 the SPOD and - `findpairs.py` - Includes the post-processing of the SPOD in the
 function `findpairs` which finds linked modes as described in [Sieber et al. in
 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/
```

### Comparing `SPyOD-0.1.4/README.md` & `SPyOD-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.4/pyproject.toml` & `SPyOD-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SPyOD"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Grigorios Hatzissawidis", email="grigorios.hatzissawidis@fst.tu-darmstadt.de" },
+  { name="Moritz Sieber", email="moritz.sieber@tu-berlin.de" },
 ]
 description = "Spectral Proper Orthogonal Decomposition"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `SPyOD-0.1.4/src/SPyOD.egg-info/PKG-INFO` & `SPyOD-0.1.5/src/SPyOD.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SPyOD
-Version: 0.1.4
+Version: 0.1.5
 Summary: Spectral Proper Orthogonal Decomposition
-Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>
+Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber <moritz.sieber@tu-berlin.de>
 Project-URL: Homepage, https://github.com/grigorishat/SPyOD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: SPyOD Version: 0.1.4 Summary: Spectral Proper
+Metadata-Version: 2.1 Name: SPyOD Version: 0.1.5 Summary: Spectral Proper
 Orthogonal Decomposition Author-email: Grigorios Hatzissawidis
-hatzissawidis@fst.tu-darmstadt.de> Project-URL: Homepage, https://github.com/
-grigorishat/SPyOD Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE # Spectral Proper Orthogonal Decomposition ## Table of
-contents * [Description](#description) * [Installation](#installation) *
-[License](#license) * [Contact us](#contact-us) * [Contributors](#contributors)
-## Description __SPyOD__ is the python implementation of the Spectral Proper
+hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber
+sieber@tu-berlin.de> Project-URL: Homepage, https://github.com/grigorishat/
+SPyOD Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE # Spectral Proper Orthogonal Decomposition ## Table of contents *
+[Description](#description) * [Installation](#installation) * [License]
+(#license) * [Contact us](#contact-us) * [Contributors](#contributors) ##
+Description __SPyOD__ is the python implementation of the Spectral Proper
 Orthogonal Decomposition published by [Sieber et al. in 2016](https://
 www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/spectral-
 proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A). It includes
 two __.py-files__: - `spod.py` - Includes the function `spod` which calculates
 the SPOD and - `findpairs.py` - Includes the post-processing of the SPOD in the
 function `findpairs` which finds linked modes as described in [Sieber et al. in
 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/
```

### Comparing `SPyOD-0.1.4/src/spyod/findpairs.py` & `SPyOD-0.1.5/src/spyod/findpairs.py`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.4/src/spyod/spod.py` & `SPyOD-0.1.5/src/spyod/spod.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,77 +82,87 @@
                     np.diag(transpose(a)*a)/Nsnap = lambda.
     mode_norm:      Norm of the single spatial modes. 1D array of length Npod. For
                     classical POD (Nfilt=0) the norm is 1 for all modes.
                     sqrt(<Ui,Ui>_w + <Vi,Vi>_w + <Wi,Wi>_w + ...) = mode_norm.
     """
     t = time.time()
     # parse input arguments
-    Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f = parse_input(args,kwargs)
+    Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f = parse_input(args, kwargs)
 
-    print("There are {} components.".format(Ncomp)) #pylint: disable=consider-using-f-string
+    if Ncomp == 1:
+        print("There is {} input component.".format(Ncomp)) #pylint: disable=consider-using-f-string
+    elif Ncomp > 1:
+        print("There are {} input components.".format(Ncomp)) #pylint: disable=consider-using-f-string
 
     if corr_type == 'temporal':
 
     # calculate temporal correlation matrix
-        R = np.zeros((Nsnap,Nsnap))
+        R = np.zeros((Nsnap, Nsnap))
 
         for ii in range(Ncomp):
-            U = np.transpose(args[ii]).reshape((Ngrid,Nsnap))
+            U = np.transpose(args[ii]).reshape((Ngrid, Nsnap))
             R = R + U.transpose() * Wxyz @ U
-        R = R/Nsnap/np.sum(Wxyz)
+        R = R / Nsnap / np.sum(Wxyz)
 
         # calculate filtered correlation matrix S
 
         if boundary == "periodic":
             # convolve periodically extended matrix with filtered diagonal matrix
 
-            ind = np.array(range(1-Nfilt, Nsnap+Nfilt+1))
-            ind = np.mod(ind-1,Nsnap)
+            ind = np.array(range(1-Nfilt, Nsnap + Nfilt + 1))
+            ind = np.mod(ind - 1, Nsnap)
             #S = convolve2d(R[np.ix_(ind, ind)], np.diag(f), mode = "valid")
             S = fftconvolve(R[np.ix_(ind, ind)], np.diag(f), mode = "valid")
 
 
         # dft case
         elif boundary == "DFTcase":
             rr = np.zeros(Nsnap)
             for ii in range(Nsnap):
-                rr[ii] = np.sum(np.diag(R,ii))*f[0]
+                rr[ii] = np.sum(np.diag(R, ii)) * f[0]
 
             # periodic boundary condition -> circulant matrix
             rr[1:] = rr[1:] + rr[:0:-1]
             S = toeplitz(rr)
 
         # convolve zero padded matrix with filter diagonal matrix
         # ("center" differs from matlab if number of rows/ columns is odd)
 
         elif boundary == "zeros":
             #S = convolve2d(R,np.diag(f), mode = "same")
-            S = fftconvolve(R, np.diag(f), mode = "same") # much faster than convolve2d
+            S = fftconvolve(R, np.diag(f), mode="same") # much faster than convolve2d
 
         # calculate eigenvalues and eigenvectors of S and sort in descending order
         # distinguish between DFTcase and periodic/ zeros, since eigh is used for symmetric matrices
 
         if boundary == "DFTcase":
 
             w, v = np.linalg.eigh(S, UPLO='U')
         else:
             w, v = np.linalg.eig(S)
 
         idx = w.argsort()[::-1]
         lmbd = w[idx] # mode variance or energy in case of velocity data
-        v = v[:,idx] # normalised temporal coefficients
+        v = v[:, idx] # normalised temporal coefficients
 
         # cut off POD modes according to the rank of matrix S
         Nrank = np.linalg.matrix_rank(S)
 
         if not Npod:
             Npod = Nrank
         elif Npod > Nrank:
             Npod = Nrank
             print('SPODrankDeficit: Correlation matrix rank is less than number of request POD modes. Npod is set to Nrank. Npod = '+ str(Nrank))
+        
+        # delete those negative eigenvalues, which are not deleted in the previous step,
+        # since correlation matrix is positive-definite or positive-semidefinite when mean flow field is subtracted
+        Nrank = len(lmbd[lmbd > 0])
+        if any(lmbd < 0) and Npod > Nrank:
+            Npod = Nrank
+            print('SPODrankDeficit: Correlation matrix rank is less than number of request POD modes. Npod is set to Nrank. Npod = '+ str(Nrank))
 
 # compute scaled temporal coefficients
         a = np.multiply(v[:,:Npod],np.sqrt(Nsnap*lmbd[:Npod]))
 
 # calculate spatial modes for all components
         a_proj = np.divide(v[:,:Npod],np.sqrt(Nsnap*lmbd[:Npod]))
         output_size = list(input_size)
@@ -193,32 +203,39 @@
                             # correlation with periodic boundary conditions
                             R[:,indi,k,:,indj,l] = np.multiply(f_ij, Uk @ np.roll(Ul,[0, ij_shift], axis=(0, 1)).transpose())
 
                         else:
                             # correlation with finite signal (zero padded)
                             u_lim = min([Nsnap-i, Nsnap-j, Nsnap])
                             l_lim = max([1-i, 1-j, 1])
-                            subi = np.array(range(l_lim, u_lim,1)) + i
-                            subj = np.array(range(l_lim, u_lim,1)) + j
-                            R[:,indi,k,:,indj,l] = np.multiply(f_ij, Uk[:,subi] @ Ul[:,subj].transpose())
+                            subi = np.array(range(l_lim, u_lim, 1)) + i
+                            subj = np.array(range(l_lim, u_lim, 1)) + j
+                            R[:, indi, k,:, indj, l] = np.multiply(f_ij, Uk[:, subi] @ Ul[:, subj].transpose())
 
         del Uk, Ul
-        R = np.reshape(R,(Ncorr,Ncorr),order='F') / (Nsnap*sum(Wxyz))
+        R = np.reshape(R,(Ncorr, Ncorr), order='F') / (Nsnap * sum(Wxyz))
 
 # calculate eigenvalues and eigenvector of R
         lmbd, v = np.linalg.eig(R) # energy of modes and normalized spatial modes
 
 # cut POD modes according to rank of matrix R if necessary
         Nrank = np.linalg.matrix_rank(R)
         if not Npod:
             Npod = Nrank
         elif Npod > Nrank:
             Npod = Nrank
             print('SPODrankDeficit: Correlation matrix rank is less than number of request POD modes. Npod is set to Nrank.')
 
+        # delete those negative eigenvalues, which are not deleted in the previous step,
+        # since correlation matrix is positive-definite or positive-semidefinite when mean flow field is subtracted
+        Nrank = len(lmbd[lmbd > 0])
+        if any(lmbd < 0) and Npod > Nrank:
+            Npod = Nrank
+            print('SPODrankDeficit: Correlation matrix rank is less than number of request POD modes. Npod is set to Nrank. Npod = '+ str(Nrank))
+
         # compute scaled temporal coefficients
         output_size = np.array(input_size)
         output_size[0] = Npod
         a = np.zeros((Nsnap,Npod),dtype = 'complex_')
         mode_norm = np.zeros((1,Npod))
         Nconvfilt = Ngrid * Nfilt2
         Ui = list()
```

