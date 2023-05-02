# Comparing `tmp/stemdiff-4.2.9.tar.gz` & `tmp/stemdiff-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemdiff-4.2.9.tar", last modified: Sun Dec 12 12:50:05 2021, max compression
+gzip compressed data, was "stemdiff-5.0.0.tar", last modified: Tue May  2 21:45:28 2023, max compression
```

## Comparing `stemdiff-4.2.9.tar` & `stemdiff-5.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-12-12 12:50:05.659282 stemdiff-4.2.9/
--rw-rw-rw-   0        0        0      243 2021-12-11 16:39:22.000000 stemdiff-4.2.9/CITATION
--rw-rw-rw-   0        0        0     1340 2021-12-11 16:39:46.000000 stemdiff-4.2.9/LICENCE
--rw-rw-rw-   0        0        0      139 2021-12-12 12:41:28.000000 stemdiff-4.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2553 2021-12-12 12:50:05.659282 stemdiff-4.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2021-12-11 11:44:40.000000 stemdiff-4.2.9/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-4.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-12-12 12:50:05.660336 stemdiff-4.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1280 2021-10-21 21:47:36.000000 stemdiff-4.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-12 12:50:05.588028 stemdiff-4.2.9/src/
-drwxrwxrwx   0        0        0        0 2021-12-12 12:50:05.644277 stemdiff-4.2.9/src/stemdiff/
--rw-rw-rw-   0        0        0      183 2021-12-12 12:41:49.000000 stemdiff-4.2.9/src/stemdiff/__init__.py
--rw-rw-rw-   0        0        0     4849 2021-10-23 21:17:56.000000 stemdiff-4.2.9/src/stemdiff/const.py
--rw-rw-rw-   0        0        0    13779 2021-10-16 09:18:50.000000 stemdiff-4.2.9/src/stemdiff/dbase.py
--rw-rw-rw-   0        0        0    13575 2021-11-08 21:45:05.000000 stemdiff-4.2.9/src/stemdiff/io.py
--rw-rw-rw-   0        0        0     8624 2021-12-08 19:22:10.000000 stemdiff-4.2.9/src/stemdiff/psf.py
--rw-rw-rw-   0        0        0     4953 2021-10-16 09:13:02.000000 stemdiff-4.2.9/src/stemdiff/radial.py
--rw-rw-rw-   0        0        0    13174 2021-11-08 22:12:58.000000 stemdiff-4.2.9/src/stemdiff/sum.py
-drwxrwxrwx   0        0        0        0 2021-12-12 12:50:05.656137 stemdiff-4.2.9/src/stemdiff.egg-info/
--rw-rw-rw-   0        0        0     2553 2021-12-12 12:50:05.000000 stemdiff-4.2.9/src/stemdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2021-12-12 12:50:05.000000 stemdiff-4.2.9/src/stemdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-12 12:50:05.000000 stemdiff-4.2.9/src/stemdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-12-12 12:50:05.000000 stemdiff-4.2.9/src/stemdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.920915 stemdiff-5.0.0/
+-rw-rw-rw-   0        0        0      243 2021-12-11 16:39:22.000000 stemdiff-5.0.0/CITATION
+-rw-rw-rw-   0        0        0     1340 2021-12-11 16:39:46.000000 stemdiff-5.0.0/LICENCE
+-rw-rw-rw-   0        0        0      139 2021-12-12 12:41:28.000000 stemdiff-5.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3053 2023-05-02 21:45:28.920915 stemdiff-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2496 2023-05-02 21:44:30.000000 stemdiff-5.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-5.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:45:28.920915 stemdiff-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2022-08-26 14:48:12.000000 stemdiff-5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.872384 stemdiff-5.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.904949 stemdiff-5.0.0/src/stemdiff/
+-rw-rw-rw-   0        0        0      794 2023-04-30 14:47:13.000000 stemdiff-5.0.0/src/stemdiff/__init__.py
+-rw-rw-rw-   0        0        0     5224 2023-05-02 21:01:54.000000 stemdiff-5.0.0/src/stemdiff/dbase.py
+-rw-rw-rw-   0        0        0     5058 2023-05-02 21:03:20.000000 stemdiff-5.0.0/src/stemdiff/detectors.py
+-rw-rw-rw-   0        0        0     4437 2023-04-30 15:34:56.000000 stemdiff-5.0.0/src/stemdiff/gvars.py
+-rw-rw-rw-   0        0        0    27995 2023-05-02 20:50:16.000000 stemdiff-5.0.0/src/stemdiff/io.py
+-rw-rw-rw-   0        0        0    11432 2023-05-02 18:17:46.000000 stemdiff-5.0.0/src/stemdiff/psf.py
+-rw-rw-rw-   0        0        0    12382 2023-05-02 21:20:53.000000 stemdiff-5.0.0/src/stemdiff/sum.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.916274 stemdiff-5.0.0/src/stemdiff.egg-info/
+-rw-rw-rw-   0        0        0     3053 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/top_level.txt
```

### Comparing `stemdiff-4.2.9/LICENCE` & `stemdiff-5.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `stemdiff-4.2.9/PKG-INFO` & `stemdiff-5.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,31 @@
-Metadata-Version: 2.1
-Name: stemdiff
-Version: 4.2.9
-Summary: Convert 4D-STEM data to a single powder diffraction pattern.
-Home-page: https://github.com/mirekslouf/stemdiff/
-Author: Mirek Slouf
-Author-email: mirek.slouf@gmail.com
-License: MIT
-Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 STEMDIFF :: Simple processing of 4D-STEM data
 ---------------------------------------------
 
 * The **STEMDIFF package** converts... <br>
   ... a 4D-STEM dataset from a SEM microscope (huge and complex) <br>
   ... to a single powder diffraction pattern (simple and easy to work with).
 * The STEMDIFF package is a key part of our **4D-STEM/PNBD** method, <br>
   which was described (together with the package) in open-access publications:
 	1. *Nanomaterials* 11 (2021) 962.
 	   [https://doi.org/10.3390/nano11040962](https://doi.org/10.3390/nano11040962)
-	2. *Materials* 14 (2011) 7550.
+	2. *Materials* 14 (2021) 7550.
        [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
-* If you use STEMDIFF in your research, **please cite** the 2nd publication.
+* If you use STEMDIFF package, **please cite** the 2nd publication (or both :-).
 
 Principle
 ---------
 
-<img src="https://raw.githubusercontent.com/mirekslouf/stemdiff/main/docs/images/principle2.png" alt="STEMDIFF principle" width="500"/>
+<img src="https://mirekslouf.github.io/stemdiff/images/principle2.png" alt="STEMDIFF principle" width="500"/>
+
+Quick start
+-----------
+
+* Install stemdiff: `pip install stemdiff`
+* TODO
 
 Documentation, help and examples
 --------------------------------
 
 More detailed help, demo and source code including documentation are in
 [GitHub](https://mirekslouf.github.io/stemdiff).
 
@@ -52,8 +41,15 @@
 	  &rArr; better resolution 
 * Version 4.2 = like v4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
-
+* Version 5.0 = complete rewrite of v4.2
+	* all features of v4.2 (summation, filtering, deconvolution)
+	* plus several generalizations and improvements, namely:
+		- possibility to define and use more detectors/datafile formats
+		- better filtering (which can employ number of diffractions)
+		- possibility to define more types of deconvolution
+	* no conversion of 2D-diffractograms to 1D-profiles
+		- this was improved and moved to sister package EDIFF
```

### Comparing `stemdiff-4.2.9/setup.py` & `stemdiff-5.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,8 +28,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"],
     license='MIT',
     package_dir={"":"src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
+    install_requires=
+        ["numpy", "matplotlib", "scipy", "pandas", "scikit-image"], 
     include_package_data=True)
```

### Comparing `stemdiff-4.2.9/src/stemdiff/const.py` & `stemdiff-5.0.0/src/stemdiff/gvars.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,114 @@
 '''
-stemdiff.const
+stemdiff.gvars
 --------------
-Constants for package stemdiff.
+Global variables/objects for package stemdiff.
+
+The global variables are used throughout the whole program.
+In order to be easily accessible, they are defined as two objects:
+    
+* SourceData = an object defining the input datafiles.
+* DiffImages = an object desribing basic/common features of all NBD patterns.
+
+The usage of stemdiff.gvars module is quite simple.
+In 99% cases, we just add the following code at beginning of STEMDIFF script
+(the arguments have to be adjusted to given experiment, of course):
+    
+>>> # Define source data
+>>> # (datafiles from TimePix detector
+>>> # (saved in data directory: D:/DATA.SH/STEMDIFF/SAMPLE_8
+>>> # (datafiles are in subdirs: 01,02,... and named as: *.dat
+>>> SDATA = stemdiff.gvars.SourceData(
+>>>     detector  = stemdiff.detectors.TimePix(),
+>>>     data_dir  = r'D:/DATA.SH/STEMDIFF/SAMPLE_8',
+>>>     filenames = r'??/*.dat')
+>>>
+>>> # Set parameters of diffractin images
+>>> # (we consider only central region with imgsize=100
+>>> # (size of the region for PSF estimate will be: psfsize=30
+>>> # (values of other/all args => documentation of stemdiff.gvars.DiffImages
+>>> DIFFIMAGES = stemdiff.gvars.DiffImages(
+>>>    imgsize=100, psfsize=30,
+>>>    ctype=2, csquare=20, cintensity=0.8,
+>>>    peak_height=100, peak_dist=9)
 '''
 
-# Key constants
-# (these costants are not expected to change for given microscope
-# (they can be adjusted if the program is used for a different microscope
-
-DET_SIZE = 256
-'''DET_SIZE = size of pixelated detector (in pixels :-)'''
-
-RESCALE  = 4
-'''RESCALE = scaling coefficient: final image size = DET_SIZE * RESCALE'''
-
-# Additional settings
-# (these settings/objects must be adjusted acc. to experimental conditions
-# (typically, the objects are defined at the beginning of the master script
-# centering = parameters for the determination of the center of 4D-STEM images
-# summation = parameters for the summation of 2D-STEM images
+from pathlib import Path
 
-class centering:
+class SourceData:
     '''
-    Set parameters for determination of center of 4D-STEM datafiles.
+    Define the input datafiles.
     
-    Typical usage
-    -------------
-    In a script, use the following two commands:
-        
-        >>> import stemdiff.const
-        >>> CENTERING = stemdiff.const.centering(
-        >>>     ctype=1,csquare=30,cintensity=0.8)
-        
-    Typical values of the arguments:
-        
-    * `ctype=1` ..fixed center, determined from the 1st file
-    * `csquare=30` ..find center in a central square with size 30 pixels 
-    * `cintensity=0.8` ..ignore intensities < 0.8 * maximal intensity
-    
-    Variable CENTERING, which contains the centering object,
-    is usually employed as an argument in the functions
-    that create database of files, determine PSF and sum datafiles.
-    
-    More help & detailed description of parameters
-    ----------------------------------------------
-    In a console, type the following two commands:
-        
-        >>> import stemdiff.const
-        >>> help(stemdiff.const.centering)
+    Parameters
+    ----------
+    data_dir : str (which will be passed to Path method)
+        This parameter is passed to Path method from pathlib library.
+        It is strongly recommeded to use r-strings.
+        Example: `data_dir = r'd:/data.sh/stemdiff/tio2'`.
+    files : str (which will be passed to data_dir.glob method)
+        This parameter is passed to Path.glob method from pathlib library.
+        It is strongly recommeded to use r-strings.
+        Example1: `datafiles = r'*.dat'` = all `*.dat` files in parent_dir;
+        Example2: `datafiles = r'??/*.dat'` = all `*.dat` in subdirs `01,02...`
+    
+    Returns
+    -------
+    DataFiles object.
     '''
-    
-    def __init__(self, ctype=1, csquare=None, cintensity=None):
-        '''
-        Initialize parameters for center determination.
 
-        Parameters
-        ----------
-        ctype : integer (values: 0, 1, 2)
-            * 0 = intensity center not determined, geometrical center is used
-            * 1 = center determined from the first image and kept constant
-            * 2 = center is determined for each individual image
-        csquare : integer (interval: 10--DET_SIZE)
-            Size of the central square (in pixels),
-            within which the center of intensity is searched for.
-        cintensity : float (interval: 0--1)
-            Intensity fraction, which is used for center determination.
-            Example: cintensity=0.9 => take only pixels > 0.9 * max.intensity.
-
-        Returns
-        -------
-        Centering object.
+    def __init__(self, detector, data_dir, filenames):
         '''
-        self.ctype = ctype
-        self.csquare = csquare
-        self.cintensity = cintensity
+        Initialize DataFiles object.
+        The parameters are described above in class definition.
+        '''
+        self.detector = detector
+        self.data_dir = Path(data_dir)
+        self.filenames = self.data_dir.glob(filenames)
         
-class summation:
+class DiffImages:
     '''
-    Set parameters for summation of 4D-STEM datafiles.
+    Set parameters/characteristics of experimental diffraction images.
     
-    Typical usage
-    -------------
-    In a script, use the following two commands:
-        
-        >>> import stemdiff.const
-        >>> SUMMATION =
-        >>>     stemdiff.const.summation(psfsize=130,imgsize=125,iterate=30)
-
-    Typical values of the arguments:
-    
-    * `psfsize=130` ..size of a central square for PSF determination
-    * `imgsize=125` ..size of a central square for summation
-    * `iterate=30`  ..number of iterations during deconvolution
-    * (psfsize > imgsize) => minimization of deconvolution artifacts
-    * (imgsize < DET_SIZE) => ignore weak diffraction at the edges
-    * (iterate=30) => a starting point; final number usually higher
-
-    Variable SUMMATION, which contains the summation object,
-    is usually employed as an argument in the functions
-    that determine PSF and sum datafiles.
-    
-    More help & detailed description of parameters
-    ----------------------------------------------
-    In a console, use the following two commands:
-            
-        >>> import stemdiff.const
-        >>> help(stemdiff.const.summation)
+    Parameters
+    ----------
+    imgsize : integer, smaller than detector_size
+        Size of array read from the detector is reduced to imgsize.
+        If given, we sum only the central square with size = imgsize.
+        Smaller area = higher speed;
+        outer area = just weak diffractions.   
+    psfize : integer, smaller than detector_size
+        Size/edge of central square, from which 2D-PSF is determined.
+    ctype : integer, values = 0,1,2
+        0 = intensity center not determined, geometrical center is used;
+        1 = center determined from the first image and kept constant;
+        2 = center is determined for each individual image.
+    csquare : integer, interval = 10--DET_SIZE
+        Size of the central square (in pixels),
+        within which the center of intensity is searched for.
+    cintensity : float, interval = 0--1
+        Intensity fraction, which is used for center determination.
+        Example: cintensity=0.9 => consider only pixels > 0.9 * max.intensity.
+    peak_height : float, optional, default is 100
+        Search for peaks whose intensity > peak_height.
+    peak_dist : integer, optional, default is 3
+        Minimal distance between possible neighboring peaks.
+
+    Returns
+    -------
+    DiffImages object.
     '''
-
-    def __init__(self, psfsize=None, imgsize=None, iterate=None):
+    
+    def __init__(self, 
+                 imgsize=100, psfsize=30,
+                 ctype=2, csquare=20, cintensity=0.8,
+                 peak_height=100, peak_dist=3):
         '''
-        Initialize parameters for summation.
-
-        Parameters
-        ----------
-        psfize : integer (interval: something--DET_SIZE)
-            Size/edge of central square, from which 2D-PSF will be determined.
-        imgsize : integer (interval: something --DET_SIZE)
-            Size of array read from the detector is reduced to imgsize.
-            If given, we sum only the central square with size = imgsize.
-            Smaller area = higher speed; outer area = just weak diffractions.   
-        iterate : integer  
-            Number of iterations during PSF deconvolution.
-
-        Returns
-        -------
-        Summation object.
+        Initialize parameters for center determination.
+        The parameters are described above in class definition.
         '''
-        self.psfsize = psfsize
         self.imgsize = imgsize
-        self.iterate = iterate
+        self.psfsize = psfsize
+        self.ctype = ctype
+        self.csquare = csquare
+        self.cintensity = cintensity
+        self.peak_height = peak_height
+        self.peak_dist = peak_dist
```

### Comparing `stemdiff-4.2.9/src/stemdiff/psf.py` & `stemdiff-5.0.0/src/stemdiff/psf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,54 @@
 '''
 stemdiff.psf
 ------------
-Calculate a 2D-PSF function from low-entropy 4D-STEM datafiles.
+The calculation a 2D-PSF function from low-entropy 4D-STEM datafiles.
 
 PSF = Point Spread Function = XY-spread of the primary beam
 '''
 
 import numpy as np
 import matplotlib.pyplot as plt
 import stemdiff.io, stemdiff.dbase
-from stemdiff.const import DET_SIZE, RESCALE
 
-def psf_from_lowS_files(
-        DBASE,SUMMATION,R=RESCALE,S=None,P=None,N=None):
-    '''
-    Extract 2D-PSF from datafiles with low Shannon entropy S.
-    PSF (= point-spread function) is taken from the central region/spot.
-    
-    Parameters
-    ----------
-    DBASE : str or pathlib object
-        Filename of database containing
-        names of all datafiles and their Shannon entropy values.
-    SUMMATION : summation object
-        Summation parameters; here we need the size/edge
-        of the central square, from which 2D-PSF will be determined.
-    R : integer
-        Rescale coefficient;
-        PSF function is rescaled/enlarged R-times.
-        Typical values of R are 2 or 4; default is stemdiff.const.RESCALE.
-    S : float
-        Shannon entropy value;
-        if S is given, PSF will be extracted only from files with entropy < S.
-    P : float
-        Percent of files with the lowest entropy;
-        if P is given, PSF will be extracted only from the P% of low-S files.
-    N : integer
-        Number of files with the lowest entropy;
-        if N is given, PSF will be extracted only from those N files.
-    
-    Returns:
-    --------
-    2D numpy array
-        The array with the saved 2D-PSF function, which represents
-        the experimentally determined XY-spread of the primary beam.
-        The array is a sum of central areas/spots of input datafiles
-        (divided by number of summed datafiles to get reasonable scale).
-        
-    Note:
-    -----
-    Priority of parameters : S > P > N
-        i.e. if S is given, P and N are ignored etc.
-    '''
-    # Get filenames with low entropy values
-    lowS_datafiles = stemdiff.dbase.get_low_S_files(DBASE, S=S, P=P, N=N)
-    # Get PSF function
-    psf = psf_from_datafiles(lowS_datafiles,SUMMATION, R=R)
-    return(psf)
-
-def psf_from_datafiles(df,SUMMATION,R=RESCALE):
-    '''
-    Parameters
-    ----------
-    df: pandas DataFrame row iterator
-        DataFrame columns: DatafileName,Entropy,Xcenter,Ycenter.
-    SUMMATION: summation object
-        Summation parameters; here we need the SUMMATION.psfsize
-        = edge of the central square, from which 2D-PSF will be determined.
-        If SUMMATION.psfsize is not given => take PSF from the whole array.
-    R: integer
-        Rescale coefficient;
-        PSF function is rescaled/enlarged R-times.
-        Typical values of R are 2 or 4; default is stemdiff.const.RESCALE.
-   
-    Returns
-    -------
-    2D numpy array
-        The array represents experimental PSF;
-        it is a sum of central areas/spots of input datafiles
-        (divided by number of summed datafiles to get reasonable scale).
-    '''
-    # Prepare variables
-    # a) number of datafilesr
-    n = 0
-    # b) array for PSF
-    psf = np.zeros((DET_SIZE*R,DET_SIZE*R), dtype=np.float)
-    if SUMMATION.psfsize:
-        # If SUMMATION.psfsize is defined => reduce array dimension
-        rsize = SUMMATION.psfsize * R
-        xc,yc = ( (DET_SIZE*R)//2, (DET_SIZE*R)//2 )
-        psf = stemdiff.io.reduce_array_size(psf,rsize,xc,yc)    
-    # Go through the files...
-    for index,datafile in df:
-        n += 1
-        arr = stemdiff.io.read_datafile(datafile.DatafileName)
-        # ..rescale array
-        arr = stemdiff.io.rescale_array(arr, R)
-        if SUMMATION.psfsize:
-            # ...read coordinates of the center
-            xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
-            # ..cut central square (the area containing central spot)    
-            arr = stemdiff.io.reduce_array_size(arr,rsize,xc,yc)
-        psf += arr
-    # Calculate final experimental PSF
-    # (divide sum by number of summed files in order to get reasonable values
-    psf = np.round(psf/n).astype(np.uint16)
-    # Convert square mask to round mask ~ set corners to zero
-    # psfsize = SUMMATION.psfsize
-    # xc,yc   = (psfsize/2, psfsize/2) 
-    # for x in range(psfsize):
-    #     for y in range(psfsize):
-    #         r = np.sqrt((x-xc)**2 + (y-yc)**2)
-    #         if r > psfsize/2: psf[x,y] = 0
-    # Return final array
-    return(psf)
-
-def save_psf(arr, output_file):
+def save_psf_to_disk(arr, output_file):
     """
     Save PSF function;
-    the function is saved in the form of 2D-numpy array.
+    the function is saved as a file in NumPy format = NPY-file.
 
     Parameters
     ----------
     arr : 2D-numpy array
         The array with the saved 2D-PSF function, which represents
         the experimentally determined XY-spread of the primary beam. 
     output_file : str
         Name of the output file (without extension);
-        the saved file will be named [output_file].npy.
+        the saved file will be named *output_file*.npy.
+    
     Returns
     -------
-    None.
-        The result is the saved array in numpy format = [output_file].npy
+    Nothing
+        The result is the PSF = 2D-array in numpy format = *output_file*.npy.
     """
     np.save(output_file, arr)
 
-def read_psf(input_file):
+def read_psf_from_disk(input_file):
     """
     Read PSF function;
-    the function is saved in the form of 2D-numpy array.
+    the function is read from a file in NumPy format = NPY-file.
 
     Parameters
     ----------
     input_file : str
-        The saved file with the PSF function;
-        the function is saved as file in numpy format = [input_file].npy.
+        The saved file with the PSF function = NPY-file.
 
     Returns
     -------
     2D-numpy array
-        The array with the saved 2D-PSF function, which represents
+        The array with the 2D-PSF function, which represents
         the experimentally determined XY-spread of the primary beam.
     """
     arr = np.load(input_file, allow_pickle=True)
     return(arr)
 
 def plot_psf(arr, plt_type='2D', plt_size=None, output=None):
     '''
@@ -173,27 +68,27 @@
     output : str, optional, default=None
         The name of the output file:
         if [output] is given, the function also saves the plot
         with a filename [output].png; otherwise the plot is just shown.
         
     Returns
     -------
-    Nothing.
+    Nothing
          The function just shows the plot of PSF in 2D or 3D.
     '''
     # Copy of arr variable
     # (in order not to change original array during (possible) resizing
     arr2 = arr.copy()
     # Prepare variables
     Xsize,Ysize = arr.shape
     xc,yc = (int(Xsize/2),int(Ysize/2))
     # Reduce array size for plotting, if required
     # (here we work with the array copy so as not to change to original
     if plt_size:
-        arr2 = stemdiff.io.reduce_array_size(arr2,plt_size,xc,yc)
+        arr2 = stemdiff.io.Arrays.remove_edges(arr2,plt_size,xc,yc)
     if plt_type=='2D':
         plt.imshow(arr2)
         plt.colorbar()
     else:
         # Prepare meshgrid for 3D-plotting
         Xsize,Ysize = arr2.shape
         Xhalf,Yhalf = int(Xsize/2),int(Ysize/2)
@@ -211,19 +106,192 @@
         # (a) Define Z-scale
         # ax.set_zlim(0,12000)
         # (b) Separate thousands by comma
         # (according to https://stackoverflow.com/q/25973581
         # (extra number 8 in the format sets the size of number = 8 places
         # (this adds extra space in front of the number - offset from Z-axis
         # ax.zaxis.set_major_formatter(
-        #     plt.matplotlib.ticker.StrMethodFormatter('{x:8,.0f}'))
-        
+        #     plt.matplotlib.ticker.StrMethodFormatter('{x:8,.0f}'))       
         plt.tight_layout()
     # Final output: show the plot (and save it, if it was requested)
     if output == None:
     # (if argument [output] was not given => just show the plot
         plt.show()
     else:
     # (if argument [output] was given => save the plot and then show it
     # (it must be done in this order - because plt.show() clears the plot!
         plt.savefig(output, dpi=300)
-        plt.show()
+        plt.show()
+
+def circular_mask(w, h, center=None, radius=None):
+    '''
+    Create a circular mask for rectangular array
+
+    Parameters
+    ----------
+    h : int
+        Height of the array.
+    w : int
+        Width of the array.
+    center : list or tuple of two integers, optional, default is None
+        Center of the mask.
+        If None, center will be a geometric center of array.
+    radius : int, optional, default is None
+        Radius of the mask.
+        If None, radius will be the distance to the shorter array wall. 
+
+    Returns
+    -------
+    mask : 2D-array of bool values
+        Circular mask: arr * mask = arr with zero values outside the mask.
+        
+    Note
+    ----
+    Copy+pasted and slightly modified from www.
+    GoogleSearch: numpy create circular mask on rectangular array
+    https://stackoverflow.com/q/44865023
+    '''
+    # Determine center and radius, if arguments were None.
+    if center is None: 
+        # use the middle of the image
+        center = (int(h/2), int(w/2))
+    if radius is None:
+        # use the smallest distance between the center and image walls
+        radius = min(center[0], center[1], h-center[0], w-center[1])
+    # Create orthogonal grid and calculate distance from center
+    # (exmplanation => https://stackoverflow.com/q/44865023
+    Y, X = np.ogrid[:w, :h]
+    dist_from_center = np.sqrt((X - center[0])**2 + (Y-center[1])**2)
+    # Calculate mask
+    # (explanation => https://stackoverflow.com/q/44865023
+    mask = dist_from_center <= radius
+    # Return the mask
+    # (2D-boolean array to modify original array
+    # (arr * mask = array with zero values outsid the mask
+    return(mask)
+
+class PSFtype1:
+    
+    def get_psf(SDATA, DIFFIMAGES, df, circular=False):
+        '''
+        Get PSF of type1 = estimated from datafiles with low/no diffractions.
+
+        Parameters
+        ----------
+        SDATA : stemdiff.gvars.SourceData object
+            The object describes source data (detector, data_dir, filenames).
+        DIFFIMAGES : stemdiff.gvars.DiffImages object
+            Object describing the diffraction images/patterns.
+        df : pandas.DataFrame object
+            Database with datafile names and characteristics.
+            PSF is estimated from the files included in this database.
+            Typically, df is a sub-database containing low-diffracting files.
+        circular : bool, optional, default is False
+            If True, apply circular mask - change square PSF to circular PSF.
+            
+        Returns
+        -------
+        psf : 2D-numpy array
+            The array represents estimate of experimental PSF.
+        '''
+        # (0) Prepare variables
+        file_counter = 0
+        R = SDATA.detector.upscale
+        det_size = SDATA.detector.detector_size
+        psf_size = DIFFIMAGES.psfsize
+        # (1) Prepare empty array for PSF calculation
+        psf = np.zeros((det_size*R, det_size*R), dtype=np.float)
+        if psf_size:
+            psf =  np.zeros((psf_size*R, psf_size*R), dtype=np.float)
+        else:
+            psf =  np.zeros((det_size*R, det_size*R), dtype=np.float)
+        # (2) Go through the files and calculate average PSF out of them
+        for index,datafile in df.iterrows():
+            # (a) Read datafile to array and increase file_counter
+            file_to_read = SDATA.data_dir.joinpath(datafile.DatafileName)
+            arr = stemdiff.io.Datafiles.read(SDATA, file_to_read)
+            file_counter += 1
+            # (b) Rescale array
+            arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
+            # (c) Remove edges if psf_size is given
+            if psf_size:
+                xc,yc = stemdiff.io.Arrays.find_center(arr,
+                    central_square = DIFFIMAGES.csquare*R,
+                    cintensity = DIFFIMAGES.cintensity)
+                arr = stemdiff.io.Arrays.remove_edges(arr,
+                    rsize = psf_size*R, xc=round(xc), yc=round(yc))
+                psf += arr
+            else:
+                psf += arr
+        # (3) Calculate final experimental PSF
+        # (divide sum by no_of_summed_files in order to get reasonable values
+        psf = np.round(psf/file_counter).astype(np.uint16)
+        # (4) Return final experimental PSF
+        return(psf)
+
+class PSFtype2:
+    
+    def get_psf(arr, psf_size, circular=False):
+        '''
+        Get PSF of type2 = estimated small central region of datafile.
+
+        Parameters
+        ----------
+        arr : 2D-numpy array
+            The array/datafile, from which the PSF is to be determined.
+            The array is a square with geometrical center = intensity center.
+            See *Technical notes* below for more details and consequences.
+        psf_size : int
+            The size/diameter of PSF function to be determined.
+        circular : bool, optional, default is False
+            If True, apply circular mask - change square PSF to circular PSF.
+            
+        Returns
+        -------
+        psf : 2D-numpy array
+            The array represents estimate of experimental PSF.
+
+        Technical notes
+        --------------
+        In our algorithm, we send a square centered array to this function.
+        This means that intensity center = geometric center of the array.
+        Consequence: we do not have to determine intensity center
+        and waste time - it is enough to calculate geometrical center.
+        '''
+        # Get center
+        # (just geometrical center as explained in the docstring
+        xc = yc = arr.shape[0]//2
+        # Remove edges
+        # (leave only central square with psf_size 
+        psf = stemdiff.io.Arrays.remove_edges(arr, psf_size, xc,yc)
+        # Remove background
+        # (PSF is from the center, it "sits" on some background intensity
+        psf = psf - np.min(psf)
+        # Convert square PSF to circular PSF if requested
+        if circular:
+            # Apply mask
+            psf = psf * circular_mask(psf_size, psf_size)
+            # Remove the remnants of background
+            # (after removing edges, array values may be slightly above zero!
+            # (1) We subtract the 2nd lowest value - the lowest are the zeros
+            the_second_lowest_value = np.min(psf[psf != np.min(psf)])
+            psf = psf - the_second_lowest_value
+            # (2) All negative values shoud go back above zero!
+            psf = np.where(psf < 0, 0, psf)
+        # Return final PSF
+        return(psf)
+
+class PSFtype3:
+    
+    def get_psf():
+        # TODO - Radim
+        # Individual PSF from whole datafile, cake-method.
+        pass
+
+class PSFtype4:
+    
+    def get_psf():
+        # TODO - Radim
+        # 1) Individual PSF from whole datafile (like PSFtype3).)
+        # 2) Subtract the PSF from whole datafile (background removal).
+        # 3) Final deconvolution performed with PSF from center (like Type2).
+        pass
```

### Comparing `stemdiff-4.2.9/src/stemdiff/sum.py` & `stemdiff-5.0.0/src/stemdiff/sum.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,311 +1,286 @@
 '''
 stemdiff.sum
 ------------
-Sum 4D-STEM datafiles to create one 2D powder diffraction file.
+The summation of 4D-STEM datafiles to create one 2D powder diffraction file.
+
+In stemdiff, we can sum datafiles in with or without 2D-PSF deconvolution.
+We just call function sum_datafiles with various arguments as explained below.
+The key argument determining type of deconvolution is deconv:
+    
+* deconv=0 = sum *without* deconvolution
+* deconv=1 = sum deconvolution, fixed PSF from selected datafiles
+* deconv=2 = sum with deconvolution, individual PSF from central region
+* deconv=3 = sum with deconvolution, individual PSF from whole datafile
 '''
 
 import numpy as np
 import stemdiff.io
 import stemdiff.dbase
-import stemdiff.radial
-from stemdiff.const import DET_SIZE, RESCALE
-from skimage import transform, restoration
-
-def sum_all(DBASE,SUMMATION,R=RESCALE):
-    """
-    Sum all datafiles from 4D-STEM dataset.
+from skimage import restoration
 
-    Parameters
-    ----------
-    DBASE : str or pathlib object
-        Name of the database file that contains
-        [filename, entropy and XY-center] of each datafile of 4D-STEM dataset.
+def sum_datafiles(
+        SDATA, DIFFIMAGES,
+        df, deconv=0, iterate=10, psf=None):
+    '''
+    Sum datafiles from a 4D-STEM dataset.
     
-    SUMMATION : summation object
-        The summation object contains parameters for the summation.
-        The object is usually defined in advance as follows:
-            
-            >>> import stemdiff.const
-            >>> SUMMATION = stemdiff.const.summation(
-            >>>     psfsize=130,imgsize=125,iterate=30)
-            
-        More information about the summation parameters:
-                
-            >>> import stemdiff.const
-            >>> help(stemdiff.const.summation)        
-            
-    R : int, optional, default=stemdiff.const.RESCALE
-        * The final diffractogram size = size-of-original-array * RESCALE.
-        * The RESCALE parameter is defined/imported from stemdiff.const
-        * The optimal value of R is 4 ~ we use 4-times upscaling.
-        * It is not recommened to change this default.
-        
-    Returns
-    -------
-    arr : 2D-numpy array
-        The array represents the calculated 2D-PNBD diffraction pattern.
-    """
-    all_datafiles = stemdiff.dbase.get_all_datafiles(DBASE)
-    arr = stemdiff.sum.sum_4Dstem_datafiles(
-        all_datafiles, R=R, imgsize=SUMMATION.imgsize)
-    return(arr)
-
-def sum_highS(DBASE,SUMMATION,R=RESCALE, S=None, P=None, N=None):
-    """
-    Sum high-entropy datafiles from 4D-STEM dataset;
-    the number of high-entropy files is determined by parameter S, P or N.
-
     Parameters
     ----------
-    DBASE : str or pathlib object
-        Name of the database file that contains
-        [filename, entropy and XY-center] of each datafile of 4D-STEM dataset.
-    
-    SUMMATION : summation object
-        The summation object contains parameters for the summation.
-        The object is usually defined in advance as follows:
-            
-            >>> import stemdiff.const
-            >>> SUMMATION = stemdiff.const.summation(
-            >>>     psfsize=130,imgsize=125,iterate=30)
-        
-        More information about the summation parameters:
+    SDATA : stemdiff.gvars.SourceData object
+        The object describes source data (detector, data_dir, filenames).
+    DIFFIMAGES : stemdiff.gvars.DiffImages object
+        Object describing the diffraction images/patterns.
+    df : pandas.DataFrame object
+        Database with datafile names and characteristics.
+    deconv : int, optional, default is 0
+        Deconvolution type:
+        0 = no deconvolution,
+        1 = deconvolution based on external PSF,
+        2 = deconvolution based on PSF from central region,
+        3 = deconvolution based on PSF from whole datafile.    
+    iterate : integer, optional, default is 10  
+        Number of iterations during the deconvolution.
+    psf : 2D-numpy array or None, optional, default is None
+        Array representing 2D-PSF function.
+        Relevant only for deconv = 1.
         
-            >>> import stemdiff.const
-            >>> help(stemdiff.const.summation)        
-         
-    R : int, optional, default=stemdiff.const.RESCALE
-        * The final diffractogram size = size-of-original-array * RESCALE.
-        * The RESCALE parameter is defined/imported from stemdiff.const
-        * The optimal value is R = 4, i.e. we use 4-times upscaling.
-        * It is not recommened to change this default.
-    
-    S : Shannon entropy
-        that separaters high- and low-S files;
-        (trivial case: the function just returns the value of S).
-
-    P : Percent of files
-        that determines how many percent of high- or low-S files we want;
-        (here we calculate the S-value separating the high/low-S files and
-        the calculated value depends on parameter high_entropy_files below).
-
-    N : Number of files
-        that determines how many high- or low-S files we want;
-        (here we calculate the S-value separating the high/low-S files and
-        the calculated value depends on parameter high_entropy_files below).
-    
     Returns
     -------
-    arr : 2D-numpy array
-        The array represents the calculated 2D-PNBD diffraction pattern.
-    """
-    highS_datafiles = stemdiff.dbase.get_high_S_files(DBASE, P=P, N=N, S=S)
-    arr = stemdiff.sum.sum_4Dstem_datafiles(
-        highS_datafiles, R=R, imgsize=SUMMATION.imgsize)
+    final_arr : 2D numpy array
+        The array is a sum of datafiles;
+        if the datafiles are pre-filtered, we get sum of filtered datafiles,
+        if PSF is given, we get sum of datafiles with PSF deconvolution.
+    
+    Technical notes
+    ---------------
+    This function works as signpost.
+    It reads the summation parameters and
+    calls more specific summation function.
+    '''
+    if deconv == 0:
+        arr = sum_without_deconvolution(
+            SDATA, DIFFIMAGES, df)
+    elif deconv == 1:
+        arr = sum_with_deconvolution_type1( 
+            SDATA, DIFFIMAGES, df, psf, iterate)
+    elif deconv == 2:
+        arr = sum_with_deconvolution_type2(
+            SDATA, DIFFIMAGES, df, iterate)
+    elif deconv == 3:
+        arr = sum_with_deconvolution_type3(
+            SDATA, DIFFIMAGES, df, iterate)
+    else:
+        print(f'Unknown deconvolution type: deconv={deconv}')
+        print('Nothing to do.')
+        return(None)
     return(arr)
 
-def sum_highS_deconv(DBASE,SUMMATION,PSF,R=RESCALE, S=None, P=None, N=None):
-    """
-    Sum high-entropy datafiles from 4D-STEM dataset with deconvolution.
-    
-    * the number of high-S files is determined by parameter S, P or N
-    * the number of deconvolution iterations is in SUMMATION parameter
+def sum_without_deconvolution(SDATA, DIFFIMAGES, df):
+    '''
+    Sum datafiles wihtout deconvolution.
 
-    Parameters
-    ----------
-    DBASE : str or pathlib object
-        Name of the database file that contains
-        [filename, entropy and XY-center] of each datafile of 4D-STEM dataset.
-        The database is usually created by functions in stemdiff.dbase module.
-    
-    SUMMATION : summation object
-        The summation object contains parameters for the summation.
-        The object is usually defined in advance as follows:
-        
-            >>> import stemdiff.const
-            >>> SUMMATION = stemdiff.const.summation(
-            >>>     psfsize=130,imgsize=125,iterate=30)
-        
-        More information about the summation parameters:
-        
-            >>> import stemdiff.const
-            >>> help(stemdiff.const.summation)        
-    
-    PSF : str or pathlib object
-        Name of the file that contains 2D-PSF function.
-        The PSF is saved in NPY-file (numpy array in numpy format).
-        The PSF is usually created by: stemdiff.psf.psf_from_lowS_files
-        
-    R : int, optional, default=stemdiff.const.RESCALE
-        * The final diffractogram size = size-of-original-array * RESCALE.
-        * The RESCALE parameter is defined/imported from stemdiff.const
-        * The optimal value is R = 4, i.e. we use 4-fold upscaling.
-        * It is not recommened to change this default.
+    * Parameters of the function:
+        - This function is usually called from stemdiff.sum.sum_files.
+        - The parameters are transferred from the sum_files function
+'''
+    # Prepare variables
+    n = 0  # number of summed datafiles
+    R = SDATA.detector.upscale
+    img_size = DIFFIMAGES.imgsize
+    # Prepare array for summation
+    # (for summation without deconvolution array size = detector size
+    # (we will sum original datafiles, just without the borders/edges  
+    # (rescaling to higher resolution can be done AFTER the summation
+    sum_arr   = np.zeros((img_size,img_size), dtype=np.float)
+    # Sum datafiles
+    for index,datafile in df.iterrows():
+        # Read datafile to array
+        datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
+        arr = stemdiff.io.Datafiles.read(SDATA, datafile_name)
+        # Reduce array size = cut borders, keep just central region
+        # (some border region is ALWAYS cut, due to detector edge artifacts
+        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
+        # Add current datafile/array to summation
+        sum_arr += arr
+        # Update n = number of summed arrays
+        n += 1
+    # Prepare final array:
+    # (1) normalize summation, 2) rescale to higher res, 3) convert to final
+    sum_arr = sum_arr/n
+    sum_arr = stemdiff.io.Arrays.rescale(sum_arr, R, order=3)
+    final_arr = np.round(sum_arr).astype(np.uint16)
+    # Return the final array
+    return(final_arr)
+
+def sum_with_deconvolution_type1(SDATA, DIFFIMAGES, df, psf, iterate):
+    '''
+    Sum datafiles with 2D-PSF deconvolution of type1.
     
-    S : Shannon entropy
-        that separaters high- and low-S files;
-        (trivial case: the function just returns the value of S).
-
-    P : Percent of files
-        that determines how many percent of high- or low-S files we want;
-        (here we calculate the S-value separating the high/low-S files and
-        the calculated value depends on parameter high_entropy_files below).
-
-    N : Number of files
-        that determines how many high- or low-S files we want;
-        (here we calculate the S-value separating the high/low-S files and
-        the calculated value depends on parameter high_entropy_files below).
+    This function is usually called from stemdiff.sum.sum_datafiles.
+    For argument description see the abovementioned function.
     
-    Returns
-    -------
-    arr : 2D-numpy array
-        The array represents the calculated 2D-PNBD diffraction pattern.
-    """ 
-    highS_datafiles = stemdiff.dbase.get_high_S_files(
-        DBASE, P=P, S=S, N=N)
-    arr = stemdiff.sum.sum_4Dstem_datafiles(
-        highS_datafiles, R, PSF,
-        itr=SUMMATION.iterate, imgsize=SUMMATION.imgsize)
-    return(arr)
+    * What is deconvolution type1:
+        - Richardson-Lucy deconvolution.
+        - 2D-PSF function estimated from files with negligible diffractions.
+        - Therefore, the 2D-PSF function is the same for all summed datafiles.
+    * Parameters of the function:
+        - This function is usually called from stemdiff.sum.sum_files.
+        - The parameters are transferred from the sum_files function
+    '''
+    # Prepare variables .......................................................
+    n = 0
+    R = SDATA.detector.upscale
+    img_size = DIFFIMAGES.imgsize
+    # Prepare array for summation
+    # (arr size = detector size * R => deconvolution on rescaled/upscaled array
+    sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float)
+    # Sum datafiles
+    # (we sum datafiles cut, rescaled, and deconvoluted
+    # (rescaling DURING the summation => smoother deconvolution function
+    # Sum with deconvolution, external PSF from low-diffracting files .........
+    for index,datafile in df.iterrows():
+        # (0) Simple progress indicator
+        print('.', end='')
+        # (1) Read datafile
+        datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
+        arr = stemdiff.io.Datafiles.read(SDATA, datafile_name) 
+        # (2) Remove edges
+        # (reason: edges usually contain weak or neglibible difractions
+        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
+        # (3) Upscale array
+        # (reason: deconvolution should be performed at higher resolution
+        # ( -logically, more pixels means smoother PSF => better deconvolution
+        # ( -surprisingly, upscaling increases real final resolution
+        arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
+        # (4) Deconvolute using the external PSF
+        # (a) save np.max, normalize
+        # (reason: deconvolution algorithm requires normalized arrays...
+        # (...and we save original max.intensity to re-normalize the result
+        norm_const = np.max(arr)
+        arr_norm = arr/np.max(arr)
+        psf_norm = psf/np.max(psf)
+        # (b) perform the deconvolution
+        arr_deconv = restoration.richardson_lucy(
+            arr_norm, psf_norm, num_iter=iterate)
+        # (c) restore original range of intensities = re-normalize
+        arr = arr_deconv * norm_const
+        # (6) Add rescaled and deconvoluted array to summation
+        sum_arr += arr
+        # (7) Updated n = number of summed arrays
+        n += 1
+    # Finalize and return result ..............................................
+    # (a) terminate simple progress indicator
+    print('End')
+    # (b) normalize the final array
+    sum_arr = sum_arr/n
+    # (c) convert to final array with integer values
+    # (why integer values? => arr with int's can be plotted as image and saved
+    final_arr = np.round(sum_arr).astype(np.uint16)
+    # (d) return the finalized array
+    return(final_arr)
 
-def sum_4Dstem_datafiles(df,R=RESCALE, PSF=None, itr=None, imgsize=None):
+
+def sum_with_deconvolution_type2(SDATA, DIFFIMAGES, df, iterate):
     '''
-    Sum input datafiles from a 4D-STEM dataset.
-    This function can be called directly, but typically it is called
-    from functions *sum_all*, *sum_highS*, and *sum_highS_deconv*.
+    Sum datafiles with 2D-PSF deconvolution of type2.
     
-    Parameters
-    ----------
-    df: pandas DataFrame row iterator
-        DataFrame columns: DatafileName,Entropy,Xcenter,Ycenter.
-    R : integer
-        Rescale coefficient;
-        the size of the final array is rescaled/multiplied by factor R.
-        If PSF is given, the rescaling is performed before deconvolution.
-        Note: PSF should the same rescale coefficient as given here!
-    PSF : 2D numpy array
-        PSF = point spread function for deconvolution
-    itr : integer 
-        Number of iterations during R-L deconvolution
-    imgsize: integer
-        Size of array read from the detector is reduced to imgsize.
-        If imgsize is given, we sum only the central square with edge=imgsize.
-        Smaller central area gives higher speed during deconvolution,
-        while the outer area usually contains just the weakest diffractions.
-        
-    Returns
-    -------
-    final_arr : 2D numpy array
-        The array is a sum of datafiles;
-        if the datafiles are pre-filtered, we get sum of filtered datafiles,
-        if PSF is given, we get sum of datafiles with PSF deconvolution.
+    This function is usually called from stemdiff.sum.sum_datafiles.
+    For argument description see the abovementioned function.
+
+    * What is deconvolution type2:
+        - Richardson-Lucy deconvolution.
+        - The 2D-PSF function estimated from central region of each datafile.
+    * Parameters of the function:
+        - This function is usually called from stemdiff.sum.sum_files.
+        - The parameters are transferred from the sum_files function
     '''
-    # Prepare variables ......................................................
+    # Prepare variables .......................................................
     n = 0
-    if imgsize:
-        arr_size = imgsize
-        xc,yc = (None,None)
-    else:
-        arr_size = DET_SIZE
-    # Sum without deconvolution ..............................................
-    if type(PSF)==type(None):
-        # Prepare files
-        # (arr size = detector size => rescaling at the end - see below
-        sum_arr   = np.zeros((arr_size,arr_size), dtype=np.float)
-        final_arr = np.zeros((arr_size,arr_size), dtype=np.uint16)
-        # Sum datafiles
-        # (rescaling can be done AFTER summation if there is no deconvolution
-        for index,datafile in df:
-            arr = stemdiff.io.read_datafile(datafile.DatafileName)
-            # If rsize was given, reduce array size
-            if imgsize:
-                xc,yc = (round(datafile.Xcenter/R),round(datafile.Ycenter/R))
-                arr = stemdiff.io.reduce_array_size(arr,imgsize,xc,yc)
-            sum_arr += arr
-            n += 1
-        # Rescale final datafile
-        norm_const = np.max(sum_arr)
-        sum_arr = transform.rescale(sum_arr, R, order=3)
-        sum_arr = sum_arr/np.max(sum_arr) * norm_const
-    # Sum with deconvolution .................................................
-    else:
-        # Read PSF and normalize it
-        # (normalization of PSF is necessary for deconvolution algorithm
-        psf = stemdiff.psf.read_psf(PSF)
-        psf = psf/np.sum(psf)
-        # Prepare files
-        # (array size = detector size * R => rescaling during summation
-        # (if imsize was given, detector size is reduced to imsize
-        sum_arr   = np.zeros((arr_size*R,arr_size*R), dtype=np.float)
-        final_arr = np.zeros((arr_size*R,arr_size*R), dtype=np.uint16)
-        # Sum datafiles with rescaling and deconvolution
-        # (rescaling must be done during summagion BEFORE deconvolution
-        for index,datafile in df:
-            print('.',end='')
-            arr = stemdiff.io.read_datafile(datafile.DatafileName)
-            # Rescale array
-            # (rescaling is done before reducing detector/array size
-            # (this should result in more precise center determination
-            arr = stemdiff.io.rescale_array(arr, R)
-            # If rsize parameter was given, reduce detector area
-            if imgsize:
-                xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
-                arr = stemdiff.io.reduce_array_size(arr,imgsize*R,xc,yc)
-            # Normalize array
-            # (normalization must be done before deconvolution
-            # (BUT we save norm.const to restore orig.intensity at the end            
-            norm_const = np.max(arr)
-            arr = arr/np.max(arr)
-            # Deconvolution
-            arr = restoration.richardson_lucy(arr, psf, iterations=itr)
-            # Multiply by the saved normalization constant
-            arr = arr * norm_const
-            # Add rescaled and deconvoluted file to summation
-            sum_arr += arr
-            n += 1
-        print()
-    # Calculate final array ..................................................
-    # (divide sum by number of summed files in order to get reasonable values
-    final_arr = np.round(sum_arr/n).astype(np.uint16)
-    # Return final array
+    R = SDATA.detector.upscale
+    img_size = DIFFIMAGES.imgsize
+    psf_size = DIFFIMAGES.psfsize
+    # Prepare array for summation
+    # (arr size = detector size * R => deconvolution on rescaled/upscaled array
+    sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float)
+    # Sum datafiles
+    # (we sum datafiles cut, rescaled, and deconvoluted
+    # (rescaling DURING the summation => smoother deconvolution function
+    # Sum with deconvolution, PSF from center of image ........................
+    for index,datafile in df.iterrows():
+        # (0) Simple progress indicator
+        print('.', end='')
+        # (1) Read datafile
+        datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
+        arr = stemdiff.io.Datafiles.read(SDATA, datafile_name) 
+        # (2) Remove edges
+        # (reason: edges usually contain weak or neglibible difractions
+        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
+        # (3) Upscale array
+        # (reason: deconvolution should be performed at higher resolution
+        # ( -logically, more pixels means smoother PSF => better deconvolution
+        # ( -surprisingly, upscaling increases real final resolution
+        arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
+        # (4) Prepare PSF from the center of given array
+        psf = stemdiff.psf.PSFtype2.get_psf(arr, psf_size, circular=True)
+        # (5) Deconvolute
+        # (a) save np.max, normalize
+        # (reason: deconvolution algorithm requires normalized arrays...
+        # (...and we save original max.intensity to re-normalize the result
+        norm_const = np.max(arr)
+        arr_norm = arr/np.max(arr)
+        psf_norm = psf/np.max(psf)
+        # (b) perform the deconvolution
+        arr_deconv = restoration.richardson_lucy(
+            arr_norm, psf_norm, num_iter=iterate)
+        # (c) restore original range of intensities = re-normalize
+        arr = arr_deconv * norm_const
+        # (6) Add rescaled and deconvoluted array to summation
+        sum_arr += arr
+        # (7) Updated n = number of summed arrays
+        n += 1
+    # Finalize and return result ..............................................
+    # (a) terminate simple progress indicator
+    print('End')
+    # (b) normalize the final array
+    sum_arr = sum_arr/n
+    # (c) convert to final array with integer values
+    # (why integer values? => arr with int's can be plotted as image and saved
+    final_arr = np.round(sum_arr).astype(np.uint16)
+    # (d) return the finalized array
     return(final_arr)
 
-def save_results(
-        arr, output, icut=300, itype='8bit', rdist=True, show2d=False):
+def sum_with_deconvolution_type3(
+        DETECTOR, DATAFILES, DIFFIMAGES, df, iterate):
+    '''
+    Sum datafiles with 2D-PSF deconvolution of type3.
+    
+    * What deconvolution type3:
+        - Richardson-Lucy deconvolution.
+        - The 2D-PSF function is estimated from each (whole) datafile.
+        - The diffractions in 2D-PSF are removed by means of "cake method".
+    * Parameters of the function:
+        - This function is usually called from stemdiff.sum.sum_files.
+        - The parameters are transferred from the sum_files function
     '''
-    Save results of summation (final 2D-image + optional 1D-radial profile).
+    pass
 
-    Parameters
-    ----------
-    arr : 2D numpy array
-        Array representing 2D-PNBD diffractogram.
-    output : string
-        Filename of output 2D-diffratogram and its 1D-radial distribution;
-        name of 2D-diffractogram will be [output.png],
-        name of 1D-radial distribution will be [output.txt].
-    icut : integer, optional, default=300
-        Cut of intensity;
-        if icut = 300, all image intensities > 300 will be set equal to 300.
-    itype : string ('8bit'  or '16bit'), optional, default='8bit'
-        Type of the image with 2D-PNBD diffractogram: 8 or 16 bit grayscale.   
-    rdist : boolean, optional, default =True
-        If rdist=True, calculate and save also 1D-radial distribution.
-        The saved file = [output].txt, where output is the argument above.
-    show : boolean, optional, default = False
-        
-    Returns
-    -------
-    None.
-        The outputs are saved 2D-diffractogram and its 1D-profile.
+def sum_with_deconvolution_type4(
+        DETECTOR, DATAFILES, DIFFIMAGES, df, iterate):
     '''
-    # Prepare filenames
-    output_2d_image   = output + '.png'
-    output_1d_profile = output + '.txt'
-    # a) Save summation = 2D-array as image
-    stemdiff.io.save_array(arr, output_2d_image, icut, itype)
-    # b) Calculate and save 1D-radial profile of the image
-    if rdist:
-        stemdiff.radial.save_radial_distribution(arr, output_1d_profile)
-    # c) If show2d=True, show the 2D image = diffractogram
-    if show2d:
-        stemdiff.io.show_array(arr, icut, itype)
+    Sum datafiles with 2D-PSF deconvolution of type4.
+    
+    * What is deconvolution type4: 
+        - Richardson-Lucy deconvolution.
+        - The 2D-PSF function estimated from whole datafile (~type3).
+        - The 2D-PSF subtracted from the datafile (background removal).
+        - Final deconvolution with 2D-PSF from central region (~type2).
+    * Parameters of the function:
+        - This function is usually called from stemdiff.sum.sum_files.
+        - The parameters are transferred from the sum_files function
+    '''
+    pass
+    
+
```

### Comparing `stemdiff-4.2.9/src/stemdiff.egg-info/PKG-INFO` & `stemdiff-5.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: stemdiff
-Version: 4.2.9
+Version: 5.0.0
 Summary: Convert 4D-STEM data to a single powder diffraction pattern.
 Home-page: https://github.com/mirekslouf/stemdiff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -21,22 +20,28 @@
 * The **STEMDIFF package** converts... <br>
   ... a 4D-STEM dataset from a SEM microscope (huge and complex) <br>
   ... to a single powder diffraction pattern (simple and easy to work with).
 * The STEMDIFF package is a key part of our **4D-STEM/PNBD** method, <br>
   which was described (together with the package) in open-access publications:
 	1. *Nanomaterials* 11 (2021) 962.
 	   [https://doi.org/10.3390/nano11040962](https://doi.org/10.3390/nano11040962)
-	2. *Materials* 14 (2011) 7550.
+	2. *Materials* 14 (2021) 7550.
        [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
-* If you use STEMDIFF in your research, **please cite** the 2nd publication.
+* If you use STEMDIFF package, **please cite** the 2nd publication (or both :-).
 
 Principle
 ---------
 
-<img src="https://raw.githubusercontent.com/mirekslouf/stemdiff/main/docs/images/principle2.png" alt="STEMDIFF principle" width="500"/>
+<img src="https://mirekslouf.github.io/stemdiff/images/principle2.png" alt="STEMDIFF principle" width="500"/>
+
+Quick start
+-----------
+
+* Install stemdiff: `pip install stemdiff`
+* TODO
 
 Documentation, help and examples
 --------------------------------
 
 More detailed help, demo and source code including documentation are in
 [GitHub](https://mirekslouf.github.io/stemdiff).
 
@@ -52,8 +57,15 @@
 	  &rArr; better resolution 
 * Version 4.2 = like v4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
-
+* Version 5.0 = complete rewrite of v4.2
+	* all features of v4.2 (summation, filtering, deconvolution)
+	* plus several generalizations and improvements, namely:
+		- possibility to define and use more detectors/datafile formats
+		- better filtering (which can employ number of diffractions)
+		- possibility to define more types of deconvolution
+	* no conversion of 2D-diffractograms to 1D-profiles
+		- this was improved and moved to sister package EDIFF
```

