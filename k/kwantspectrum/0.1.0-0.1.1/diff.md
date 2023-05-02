# Comparing `tmp/kwantspectrum-0.1.0.tar.gz` & `tmp/kwantspectrum-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kwantspectrum-0.1.0.tar", last modified: Wed May 13 20:29:30 2020, max compression
+gzip compressed data, was "dist/kwantspectrum-0.1.1.tar", last modified: Tue May  2 12:50:52 2023, max compression
```

## Comparing `kwantspectrum-0.1.0.tar` & `kwantspectrum-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/
--rw-r--r--   0 cg229074 (65563) big      (30018)     1489 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/LICENSE.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      221 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/.coveragerc
--rw-r--r--   0 cg229074 (65563) big      (30018)      635 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/MANIFEST.in
--rw-r--r--   0 cg229074 (65563) big      (30018)     6458 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/PKG-INFO
--rw-r--r--   0 cg229074 (65563) big      (30018)       38 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/setup.cfg
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum/
--rw-r--r--   0 cg229074 (65563) big      (30018)    37605 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/kwantspectrum/kwant_spectrum.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     4023 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/kwantspectrum/version.py
--rw-r--r--   0 cg229074 (65563) big      (30018)      500 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/kwantspectrum/__init__.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum/tests/
--rw-r--r--   0 cg229074 (65563) big      (30018)    15595 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/kwantspectrum/tests/test_kwant_spectrum.py
--rw-r--r--   0 cg229074 (65563) big      (30018)       43 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/kwantspectrum/tests/__init__.py
--rw-r--r--   0 cg229074 (65563) big      (30018)       60 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum/_kwant_spectrum_version.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum.egg-info/
--rw-r--r--   0 cg229074 (65563) big      (30018)       63 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum.egg-info/requires.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)        1 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum.egg-info/dependency_links.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)     6458 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum.egg-info/PKG-INFO
--rw-r--r--   0 cg229074 (65563) big      (30018)       14 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum.egg-info/top_level.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)      658 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/kwantspectrum.egg-info/SOURCES.txt
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/doc/
--rw-r--r--   0 cg229074 (65563) big      (30018)      665 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/doc/Makefile
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/doc/source/
--rw-r--r--   0 cg229074 (65563) big      (30018)     4998 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/doc/source/conf.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/doc/source/kwantdoctheme/
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2020-05-13 20:29:30.000000 kwantspectrum-0.1.0/doc/source/kwantdoctheme/static/
--rw-r--r--   0 cg229074 (65563) big      (30018)     3576 2020-03-24 15:06:12.000000 kwantspectrum-0.1.0/doc/source/kwantdoctheme/static/kwantdoctheme.css
--rw-r--r--   0 cg229074 (65563) big      (30018)      614 2020-03-24 15:06:12.000000 kwantspectrum-0.1.0/doc/source/kwantdoctheme/theme.conf
--rw-r--r--   0 cg229074 (65563) big      (30018)      140 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/doc/source/reference.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      157 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/doc/source/index.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    23861 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/doc/source/tutorial.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)       30 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/doc/source/about.rst
--rwxr-xr-x   0 cg229074 (65563) big      (30018)     5214 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/setup.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     4439 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/README.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      394 2020-05-11 12:58:11.000000 kwantspectrum-0.1.0/pytest.ini
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1489 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/LICENSE.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      221 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/.coveragerc
+-rw-r--r--   0 cg229074 (65563) big      (30018)      635 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/MANIFEST.in
+-rw-r--r--   0 cg229074 (65563) big      (30018)     6675 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/PKG-INFO
+-rw-r--r--   0 cg229074 (65563) big      (30018)       38 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/setup.cfg
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum/
+-rw-r--r--   0 cg229074 (65563) big      (30018)    41042 2023-04-17 07:20:15.000000 kwantspectrum-0.1.1/kwantspectrum/kwant_spectrum.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4021 2023-04-15 15:21:20.000000 kwantspectrum-0.1.1/kwantspectrum/version.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)      639 2023-04-15 15:21:20.000000 kwantspectrum-0.1.1/kwantspectrum/__init__.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum/tests/
+-rw-r--r--   0 cg229074 (65563) big      (30018)    15063 2023-04-17 07:16:26.000000 kwantspectrum-0.1.1/kwantspectrum/tests/test_kwant_spectrum.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)       43 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/kwantspectrum/tests/__init__.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)       60 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum/_kwant_spectrum_version.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum.egg-info/
+-rw-r--r--   0 cg229074 (65563) big      (30018)       63 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum.egg-info/requires.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)        1 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum.egg-info/dependency_links.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)     6675 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum.egg-info/PKG-INFO
+-rw-r--r--   0 cg229074 (65563) big      (30018)       14 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum.egg-info/top_level.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)      658 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/kwantspectrum.egg-info/SOURCES.txt
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/doc/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      665 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/doc/Makefile
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/doc/source/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4990 2023-04-17 07:20:15.000000 kwantspectrum-0.1.1/doc/source/conf.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/doc/source/kwantdoctheme/
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-02 12:50:52.000000 kwantspectrum-0.1.1/doc/source/kwantdoctheme/static/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3576 2020-03-24 15:06:12.000000 kwantspectrum-0.1.1/doc/source/kwantdoctheme/static/kwantdoctheme.css
+-rw-r--r--   0 cg229074 (65563) big      (30018)      614 2020-03-24 15:06:12.000000 kwantspectrum-0.1.1/doc/source/kwantdoctheme/theme.conf
+-rw-r--r--   0 cg229074 (65563) big      (30018)      140 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/doc/source/reference.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      157 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/doc/source/index.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    23861 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/doc/source/tutorial.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)       30 2020-05-11 12:58:11.000000 kwantspectrum-0.1.1/doc/source/about.rst
+-rwxr-xr-x   0 cg229074 (65563) big      (30018)     5464 2023-04-15 15:21:20.000000 kwantspectrum-0.1.1/setup.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4576 2023-04-17 07:20:15.000000 kwantspectrum-0.1.1/README.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      357 2023-04-17 07:20:15.000000 kwantspectrum-0.1.1/pytest.ini
```

### Comparing `kwantspectrum-0.1.0/LICENSE.rst` & `kwantspectrum-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `kwantspectrum-0.1.0/MANIFEST.in` & `kwantspectrum-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kwantspectrum-0.1.0/PKG-INFO` & `kwantspectrum-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwantspectrum
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adaptive band structure analyzer for Kwant leads
 Home-page: https://gitlab.kwant-project.org/kwant/kwantspectrum
 Author: T. Kloss, C. W. Groth, X. Waintal, et al.
 Author-email: kloss@itp.uni-frankfurt.de
 License: UNKNOWN
 Description: About kwantSpectrum
         ===================
@@ -18,24 +18,49 @@
         
         kwantSpectrum is distributed under the `2-clause BSD license <https://gitlab.kwant-project.org/kwant/kwantspectrum/-/blob/master/LICENSE.rst>`_
         
         Website: https://kwant-project.org/extensions/kwantspectrum
         
         Source code: https://gitlab.kwant-project.org/kwant/kwantspectrum
         
+        Conda package: https://github.com/conda-forge/kwantspectrum-feedstock
         
         
         Installation
         ############
         
-        This section covers the installation of kwantSpectrum on a GNU/Linux
-        system as Debian and Ubuntu via the command line.
+        kwantSpectrum packages are hosted on PyPI and conda.
+        The installation should work GNU/Linux system as Debian and Ubuntu,
+        as well as on MacOS and Windows.
         
-        Requirements
-        ^^^^^^^^^^^^
+        **PyPI**::
+        
+            python3 -m pip install --user kwantspectrum
+        
+        **conda**::
+        
+            conda install -c conda-forge kwantspectrum
+        
+        
+        Installation from source
+        ^^^^^^^^^^^^^^^^^^^^^^^^
+        
+        kwantSpectrum can be installed directly from the source code repository::
+        
+            python3 -m pip install --user git+https://gitlab.kwant-project.org/kwant/kwantspectrum.git
+        
+        For development, kwantSpectrum can be cloned from the official repository with::
+        
+            git clone https://gitlab.kwant-project.org/kwant/kwantspectrum.git
+        
+        The requirements listed below must be installed by hand.
+        
+        
+        Build requirements
+        ------------------
         
         kwantSpectrum has following non-Python dependency:
         
         - `Kwant <https://kwant-project.org/>`__
         
         Kwant can be installed with the following command::
         
@@ -45,59 +70,43 @@
         
         kwantSpectrum requires at least Python 3.5. The following packages must
         be installed to build kwantSpectrum:
         
         - `NumPy <https://numpy.org/>`_
         - `SciPy <https://www.scipy.org/>`_
         
-        Most packages can be installed from the command line
-        by the standard Python package manager `pip <https://pip.pypa.io/en/stable/>`_ via::
+        The packages can be installed by the standard *pip* command::
         
-            sudo pip3 install numpy scipy
+            python3 -m pip install --user numpy scipy
         
         Testing requirements
         --------------------
         The kwantSpectrum test suite requires the following Python packages:
         
         - `pytest <https://docs.pytest.org/en/latest/>`_
         - `pytest-cov <https://pytest-cov.readthedocs.io/en/latest/>`_
-        - `pytest-flake8 <https://pypi.org/project/pytest-flake8/>`_
         
         
         The packages can be installed by the standard *pip* command::
         
-            sudo pip3 install pytest pytest-cov pytest-flake8
+            python3 -m pip install --user pytest pytest-cov
         
         Documentation requirements
         --------------------------
         Building the documentation requires the following Python packages:
         
         - `matplotlib <https://matplotlib.org/>`_
         - `sphinx <https://www.sphinx-doc.org/en/master/>`_
         - `jupyter-sphinx <https://jupyter-sphinx.readthedocs.io/en/latest/>`_
         
         
         The packages can be installed by the standard *pip* command::
         
-            sudo pip3 install matplotlib sphinx jupyter-sphinx
-        
-        Building kwantSpectrum
-        ^^^^^^^^^^^^^^^^^^^^^^
-        
-        kwantSpectrum can be installed from PyPI with::
-        
-            sudo pip3 install kwantspectrum
+            python3 -m pip install --user matplotlib sphinx jupyter-sphinx
         
-        Alternatively, it can be installed directly from the source code repository::
-        
-            sudo pip3 install git+https://gitlab.kwant-project.org/kwant/kwantspectrum.git
-        
-        For development, kwantSpectrum can be cloned from the official repository with::
-        
-            git clone https://gitlab.kwant-project.org/kwant/kwantspectrum.git
         
         Test suite
         ----------
         
         Unittests can be run directly in the local source repository from the command line::
         
             pytest
@@ -161,14 +170,15 @@
         * Thomas Kloss (CEA Grenoble), kloss@itp.uni-frankfurt.de
         
         Contributors to the project are:
         
         * Christoph Groth (CEA Grenoble)
         * Xavier Waintal (CEA Grenoble)
         * Benoît Rossignol (CEA Grenoble)
+        * Bas Nijholt (Microsoft)
         
         (CEA = Commissariat à l'énergie atomique et aux énergies alternatives)
         
 Keywords: physics kwant bandstructure
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kwantspectrum-0.1.0/kwantspectrum/kwant_spectrum.py` & `kwantspectrum-0.1.1/kwantspectrum/kwant_spectrum.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,14 +142,41 @@
         if intersect:
             return not _is_zero(intersect[1] - intersect[0], tol=tol)
         return False
     return [_intersection(a, b) for a in interval_a for b in interval_b
             if large_enough(a, b)]
 
 
+def group_values(x, tol=1e-5):
+    """group a list of numerical values to a list of list, where similar
+       values are in the same list. the input must be ordered
+       and the output is ordered as in the input"""
+    x_grouped = []
+    if len(x) > 0:
+        xl = x[0]
+        group = [xl]
+        for xx in x[1:]:
+            if abs(xl - xx) > tol:
+                x_grouped.append(group)
+                group = []
+            group.append(xx)
+            xl = xx
+        x_grouped.append(group)
+    return x_grouped
+
+
+def array_sign(x):
+    """return true if all signs in array are equal"""
+    xsign = np.sign(x)
+    signchange = ((np.roll(xsign, 1) - xsign) == 0).astype(bool)
+    if signchange.all():
+        return int(xsign[0])
+    return 0
+
+
 def _cubic_coeffs(x, y, dy, axis=0):
     """Computes the cubic polynominal coefficients  in `scipy.PPoly` form
     from a function and its first derivative.
 
     Parameters
     --------
     x : array_like, shape (n,)
@@ -295,15 +322,15 @@
                 root_is_nan[i - 1] = True
     return roots[~root_is_nan]
 
 
 def _machine_epsilon_reached(x0, x1):
     """Return `True` if relative difference between `x0` and `x1` is smaller
     than machine epsilon for floats"""
-    return np.abs(x0 - x1) <= 10 * np.finfo(np.float).eps
+    return np.abs(x0 - x1) <= 10 * np.finfo(float).eps
 
 
 def _leftmost_crossing(fl, fr, xl, xr):
     """Find the leftmost crossing point of an array of functions
 
     Returns
     ----------
@@ -354,15 +381,15 @@
     a0, b0 = func0.reshape(2, -1, 1)
     a1, b1 = func1.reshape(2, 1, -1)
 
     dx = (x1 - x0) / 2
 
     a = a0 - a1 + (b0 + b1) * dx
     b = b0 - b1
-    pvec = np.array([b * b / 3, 0, a * a])
+    pvec = np.array([b * b / 3, 0, a * a], dtype=object)
     return np.polyval(pvec, dx)
 
 
 def _order_left_to_right(fl, fr, xl, xr):
     """Order the elements of a vector like function on an interval.
     The elements of the function vector on the right boundary are ordered
     according to the element ordering on the left boundary.
@@ -429,15 +456,15 @@
     @wraps(func)
     def wrapper(*args, **kwargs):
         result = func(*args, **kwargs)
         return np.insert(result, 2, np.arange(result.shape[1]), axis=0)
     return wrapper
 
 
-def _match_functions(func, xmin=-1, xmax=1, tol=1E-8, min_iter=10,
+def _match_functions(func, xmin=-1, xmax=1, tol=1E-10, min_iter=10,
                      max_iter=100000, interval_converged=None, evaluated=None):
     """Match the elements of a vector valued function, such that
     each vector element describes a continous function.
 
     Parameters
     ----------
     func : callable
@@ -551,15 +578,15 @@
     assert _is_type_array(x, 'number').all()
     assert _is_type_array(y, 'number').all()
 
     return x, y[:, 0], y[:, 1], y[:, 2].astype(int)
 
 
 def spectrum(syst, args=(), *, params=None, kmin=-np.pi, kmax=np.pi,
-             orderpoint=0, tol=1E-8, match=_match_functions):
+             orderpoint=0, tol=1E-10, tol_bs=1E-5, match=_match_functions):
     r"""Interpolate the dispersion function and provide methods to
     simplify curve sketching and analyzation the periodic spectrum.
 
     Parameters
     ----------
     syst : `kwant.system.InfiniteSystem`
         The low level infinite system for which the energies are to be
@@ -627,15 +654,15 @@
     ordering = ordering[:, band_order]
 
     # provide a function that calculates the open modes for a given energy
     mode_function = partial(syst.modes, args=args, params=params)
 
     # return a cubic interpolation of the spectrum, provide access to
     # ordering
-    band_sketching = BandSketching(x, y, dy, mode_function, tol)
+    band_sketching = BandSketching(x, y, dy, mode_function, tol_bs)
     band_sketching.ordering = ordering
     return band_sketching
 
 
 def spectra(syst, *args, **kwargs):
     """Interpolates a sequence of dispersion functions and provide methods to
     simplify curve sketching and analyzation the periodic spectra.
@@ -685,15 +712,15 @@
     Notes
     -----
     The routine designed for a periodic function that is represented
     as discrete values on a finite gridpoints.
     Finite accuracy of the data and possible unphysical results are taking into
     account by rounding value :math:`tol`.
     """
-    def __init__(self, x, y, dy, mode_function, tol=1E-8,
+    def __init__(self, x, y, dy, mode_function, tol=1E-10,
                  interpolation=_cubic_interpolation):
 
         # type and input checks
         assert x.size == y.shape[0] == dy.shape[0]
         assert y.shape == dy.shape
         assert _is_type_array(x, 'real_number').all()
         assert _is_type_array(y, 'real_number').all()
@@ -800,29 +827,64 @@
             is the total number of bands of the spectrum.
             If no open mode could be found, `mode = -1` is returned.
         """
         # type checks
         assert _is_type(k, 'real_number')
         assert _is_type(band, 'integer')
 
-        energy = self.__call__(k, band)
+        # calculate all energies to check for degenerate bands.
+        # if other bands have similar energy to the band that we are looking for,
+        # the degenerate bands are labeled (deg_mode_pos).
+        # example: system with nbands = 4, energies = [0, -1, -1, 2] at given momentum k
+        # band = 1 -> energy of the band= -1, deg_mode_pos = 0
+        # band = 2 -> energy of the band= -1, deg_mode_pos = 1
+        # when kwant is called with energy =-1, one gets two modes with similar k and
+        # positive velocity. depending on deg_mode_pos we return either the first
+        # or the second mode
+
+        energies = [self.__call__(k, b) for b in range(self.nbands)]
+        energy = energies[band]
+        similar_energy = [np.abs(ei - energy) <= self.tol and np.abs(energy) > self.tol
+                          for ei in energies]
+        ndeg = 0
+        for se in similar_energy:
+            if se:
+                ndeg += 1
+
+        deg_mode_pos = 0
+        for i, is_deg in enumerate(similar_energy):
+            if i == band:
+                break
+            if is_deg:
+                deg_mode_pos += 1
+
         try:  # kwant fails if energy is exactly at the bandgap
             modes = self._modes(energy=energy)[0]
         except ValueError:
             return -1
 
         momenta = modes.momenta
         velocities = modes.velocities
 
         # for almost flat bands, small numerical errors (of order 1E-16)
         # in the energy from the interpolation function might fail kwant's
         # mode calculation. (as the velocity of that modes is zero,
         # they do not contribute to a manybody sum anyhow).
+        if ndeg <= 1:  # no degenerate modes
+            try:
+                return np.abs(momenta[velocities > 0] - k).argmin()
+            except ValueError:
+                return -1
+        # degenerate modes with nonzero energy
         try:
-            return np.abs(momenta[velocities > 0] - k).argmin()
+            modes_deg = []
+            for i, km in enumerate(momenta[velocities > 0]):
+                if np.abs(km - k) <= 100 * self.tol:  # precision not perfect..
+                    modes_deg.append(i)
+            return modes_deg[deg_mode_pos]
         except ValueError:
             return -1
 
     def energy_to_scattering_mode(self, energy, band, kmin, kmax):
         """Finds the scattering mode index for a band giving its energy.
 
         Parameters
@@ -860,42 +922,38 @@
                    'interval=[{kmin}, {kmax}], k={k}.'
                    .format(energy=energy, band=band, kmin=kmin, kmax=kmax, k=k))
             warnings.warn(msg)
             return -1
         return self.momentum_to_scattering_mode(k[0], band)
 
     def intersect(self, f, band, derivative_order=0,
-                  kmin=None, kmax=None, tol=None, ytol=None):
-        r"""Returns all momentum (k) points, that solves the equation:
-        :math:`\partial_k^{n} E(k) = f(k),\, k_{min} \leq k \leq k_{max}`.
+                  kmin=None, kmax=None, tol=None, ytol=1e-14):
+        r"""Returns all momentum (:math:`k`) points which solve the equation:
+        :math:`\partial_k^{m} E_n(k) = f(k),\, k_{min} \leq k \leq k_{max}`.
 
         Parameters
         ----------
         f : scalar numerical value or callable
-            Equation to solve :math:`\partial_k^{n} E(k) = f`.
+            Equation to solve :math:`\partial_k^{m} E_n(k) = f`.
             If `f` is callable, solve equation:
-            :math:`\partial_k^{n} E(k) = f(k)`.
+            :math:`\partial_k^{m} E_n(k) = f(k)`.
         band : int
-            band index, requirement: `0 <= band < nbands`.
+            band index `n`, requirement: `0 <= band < nbands`.
         derivative_order : int, optional
-            Derivative order (n) of the band dispersion. Default is zero.
+            Derivative order `m` of the band dispersion. Default is zero.
         kmin : scalar numeric value, optional
             Lowest `k` point value. Default is `kmin` from initialization.
         kmax : scalar numeric value, optional
             Largest `k` point value. Default is `kmax` from initialization.
         tol : float, optional
             Numerical tolerance, `k` points closer tol are merged to the same
             point. Default is the `tol` from initialization.
         ytol : float, optional
             Numerical tolerance to remove noise if the
-            spectrum :math:`\partial_k^{n} E(k)` is almost flat.
-            Values for the spectrum are set to thier mean value
-            (averaged over all momentum points where the band is sampled), if
-            they flucutate more than `ytol`.
-            Default is the `tol` from initialization.
+            spectrum :math:`\partial_k^{m} E_n(k)` is almost flat below ytol.
 
         Returns
         -------
         k : numpy list.
             List of momentum (k) points, that solves the above equation.
 
         Notes
@@ -906,16 +964,14 @@
 
         if kmin is None:
             kmin = self.kmin
         if kmax is None:
             kmax = self.kmax
         if tol is None:
             tol = self.tol
-        if ytol is None:
-            ytol = self.tol
 
         # type and input checks
         assert _is_type(band, 'integer')
         assert _is_type(derivative_order, 'integer')
         assert _is_type(kmin, 'real_number')
         assert _is_type(kmax, 'real_number')
         assert _is_type(tol, 'real_number')
@@ -934,43 +990,62 @@
 
         if callable(f):
             f = f(self.x)
 
         if derivative_order == 0:  # use tabulated values, faster
             y = self.y[:, band]
             dy = self.dy[:, band]
+        elif derivative_order == 1:
+            y = self.dy[:, band]
+            dy = self._func(self.x, derivative_order + 1)[:, band]
         else:
             y = self._func(self.x, derivative_order)[:, band]
             dy = self._func(self.x, derivative_order + 1)[:, band]
 
-        # filter numerical noise if curve is flat
-        y_mean = np.mean(y)
-        if _is_zero(y_mean, ytol):
-            y_mean = 0
-        y[np.abs(y - y_mean) < ytol] = y_mean
-        dy[np.abs(dy) < ytol] = 0
-
-        roots = self.interpolation(self.x, y - f, dy).roots()
+        g = y - f  # roots of g give the intersection points we are seeking
+        roots = self.interpolation(self.x, g, dy).roots()
         roots = remove_nan(roots)
 
+        # remove spurious points in case of numerical noise
+        if f == 0 and derivative_order == 1:  # special case important for tkwant
+            roots_grouped = group_values(roots, tol)
+            group_averages = [np.mean(group) for group in roots_grouped]
+
+            remove_element = []
+            for i, km in enumerate(group_averages):
+                if km - tol > kmin and km + tol < kmax:
+                    ym = self.__call__(km, band)
+                    kl = np.linspace(km - tol, km - tol / 2, 5)
+                    yl = self.__call__(kl, band) - ym
+                    sign_left = array_sign(yl)
+                    kr = np.linspace(km + tol / 2, km + tol, 5)
+                    yr = self.__call__(kr, band) - ym
+                    sign_right = array_sign(yr)
+                    sign_change = sign_left * sign_right != 1
+                    almost_zero = (np.abs(np.mean(yl)) + np.abs(np.mean(yr)) < ytol)
+                    if sign_change or almost_zero:
+                        remove_element.append(i)
+
+            roots = np.array([elem for i, elem in enumerate(group_averages) if i not in remove_element])
+
         if self.period:
             roots = _periodic(roots, *self.period)
 
         try:
             period_len = self.period[1] - self.period[0]
             npe = int((kmax - kmin) // period_len)  # number of periods
             images = period_len * np.arange(-npe + 1, npe).reshape(2 * npe - 1, -1)
             roots = _unique(np.sort(np.ravel(roots + images)), tol)
         except:  # no periodic image, npe = 0
             roots = _unique(np.sort(roots), tol)
 
         return roots[_is_inside(roots, kmin, kmax)]
 
     def intervals(self, band, derivative_order=0, lower=None, upper=None,
-                  kmin=None, kmax=None, tol=None):
+                  kmin=None, kmax=None, tol=None, ytol=1e-14):
         r"""returns a list of momentum (`k`) intervals that solves the equation
         :math:`\text{lower} \leq  \partial^m_k E_n(k)  \leq \text{upper}`
 
         Parameters
         ----------
         band : int
             band index `n`, requirement: `0 <= n < nbands`.
@@ -985,14 +1060,18 @@
         kmin : scalar numeric value, optional
             Lowest `k` point value. Default is `kmin` from initialization.
         kmax : scalar numeric value, optional
             Largest `k` point value. Default is `kmax` from initialization.
         tol : float, optional
             Tolerance of the interval selection, such that intervals smaller
             `tol` are neglected and two intervals closer `tol` are merged.
+        ytol : float, optional
+            Numerical tolerance to remove noise if the
+            spectrum :math:`\partial_k^{m} E_n(k)` is almost flat below ytol.
+            Default is the `tol` from initialization.
 
         Returns
         -------
         intervals : list.
             Ordered list of momentum intervals :math:`[k_i, k_{i+1}]`.
             Each interval is given in form of a tuple.
         """
@@ -1012,24 +1091,25 @@
         assert _is_type(derivative_order, 'integer')
         assert _is_type(kmin, 'real_number')
         assert _is_type(kmax, 'real_number')
         assert _is_type(tol, 'real_number')
         assert 0 <= band < self.nbands, 'band index out of range'
         assert kmin <= kmax, 'bounds swapped'
         assert tol > 0
+        assert ytol > 0
 
         crossings = [kmin, kmax]
         if lower is not None:
             crossings = np.append(crossings, self.intersect(lower, band,
                                                             derivative_order,
-                                                            kmin, kmax, tol))
+                                                            kmin, kmax, tol, ytol))
 
         if upper is not None:
             crossings = np.append(crossings, self.intersect(upper, band,
                                                             derivative_order,
-                                                            kmin, kmax, tol))
+                                                            kmin, kmax, tol, ytol))
 
         crossings = _unique(np.sort(crossings), tol)
 
         return [x for x in _pairwise(crossings)
                 if (not _is_zero(x[1] - x[0], tol)
                     and _is_inside(f(x), lower, upper))]
```

### Comparing `kwantspectrum-0.1.0/kwantspectrum/version.py` & `kwantspectrum-0.1.1/kwantspectrum/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,23 +100,20 @@
     if version_tags:
         release, *_ = sorted(version_tags)  # prefer e.g. "2.0" over "2.0rc1"
         return release
     else:
         return ''.join(('unknown', '+g', git_hash))
 
 
-def init(version_file='_kwant_spectrum_version.py'):
-    global version, version_is_from_git
+def get_version(version_file='_kwant_spectrum_version.py'):
     version_info = {}
     with open(os.path.join(package_root, version_file), 'rb') as f:
         exec(f.read(), {}, version_info)
     version = version_info['version']
     version_is_from_git = (version == "__use_git__")
     if version_is_from_git:
         version = get_version_from_git()
         if not version:
             version = get_version_from_git_archive(version_info)
         if not version:
             version = "unknown"
-
-
-init()
+    return version, version_is_from_git
```

### Comparing `kwantspectrum-0.1.0/kwantspectrum/tests/test_kwant_spectrum.py` & `kwantspectrum-0.1.1/kwantspectrum/tests/test_kwant_spectrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,39 +265,35 @@
     assert mode == -1
     # check that result is similar to reordered kwant result
     bands = kwant.physics.Bands(make_lead().finalized())
     energies = [bands(k)[order] for k, order in zip(ba.x, ba.ordering)]
     assert_array_almost_equal(ba.y, energies)
 
 
-def test_spectrum_with_flat_band():
+def test_spectrum_with_degenerate_bands():
+
+    def toy_lead_spinsystem(a=1):
+
+        sigma0 = np.array([[1, 0], [0, 1]])
+
+        lat = kwant.lattice.square(a=a, norbs=2)
+        lead = kwant.Builder(kwant.TranslationalSymmetry((-a, 0)))
+        lead[lat(0, 0)] = 0 * sigma0
+        lead[lat.neighbors()] = - sigma0
 
-    # edgecase with tree bands, where the second band is flat but with tiny noise
-    def make_lead_with_flat_band(ll=3):
-        lat = kwant.lattice.square(norbs=1)
-        lead = kwant.Builder(kwant.TranslationalSymmetry((-1, 1)))
-        lead[[lat(0, j) for j in range(ll)]] = 0
-        lead[lat.neighbors()] = -1
         return lead
 
-    lead = make_lead_with_flat_band().finalized()
+    lead = toy_lead_spinsystem().finalized()
     spectrum = ks.spectrum(lead)
 
-    assert_array_almost_equal([0], spectrum.intersect(f=0, band=0, derivative_order=1))
-    assert spectrum.intersect(f=0, band=1, derivative_order=1).size == 0
-    assert_array_almost_equal([0], spectrum.intersect(f=0, band=2, derivative_order=1))
-
-    # the spectrum has also no wendepunkt
-    assert spectrum.intersect(f=0, band=0, derivative_order=2).size == 0
-    assert spectrum.intersect(f=0, band=1, derivative_order=2).size == 0
-    assert spectrum.intersect(f=0, band=2, derivative_order=2).size == 0
-
-    # one can lower the tolerance to recover the result with the numerical noise
-    assert spectrum.intersect(f=0, band=1, derivative_order=1, ytol=1E-20).size > 0
-    assert spectrum.intersect(f=0, band=1, derivative_order=2, ytol=1E-20).size > 0
+    # check that the two modes are not the same
+    # here by chance they are similar to the band index, but this is generally
+    # not the case.
+    assert spectrum.momentum_to_scattering_mode(0.2, 0) == 0
+    assert spectrum.momentum_to_scattering_mode(0.2, 1) == 1
 
 
 def test_function_mapping():
     def func(xx):
         # the two functions in f(x) cross at
         # x = [-1, (3 - np.sqrt(13)) / 2, (3 + np.sqrt(13)) / 2]
         def f(x):
```

### Comparing `kwantspectrum-0.1.0/kwantspectrum.egg-info/PKG-INFO` & `kwantspectrum-0.1.1/kwantspectrum.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwantspectrum
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adaptive band structure analyzer for Kwant leads
 Home-page: https://gitlab.kwant-project.org/kwant/kwantspectrum
 Author: T. Kloss, C. W. Groth, X. Waintal, et al.
 Author-email: kloss@itp.uni-frankfurt.de
 License: UNKNOWN
 Description: About kwantSpectrum
         ===================
@@ -18,24 +18,49 @@
         
         kwantSpectrum is distributed under the `2-clause BSD license <https://gitlab.kwant-project.org/kwant/kwantspectrum/-/blob/master/LICENSE.rst>`_
         
         Website: https://kwant-project.org/extensions/kwantspectrum
         
         Source code: https://gitlab.kwant-project.org/kwant/kwantspectrum
         
+        Conda package: https://github.com/conda-forge/kwantspectrum-feedstock
         
         
         Installation
         ############
         
-        This section covers the installation of kwantSpectrum on a GNU/Linux
-        system as Debian and Ubuntu via the command line.
+        kwantSpectrum packages are hosted on PyPI and conda.
+        The installation should work GNU/Linux system as Debian and Ubuntu,
+        as well as on MacOS and Windows.
         
-        Requirements
-        ^^^^^^^^^^^^
+        **PyPI**::
+        
+            python3 -m pip install --user kwantspectrum
+        
+        **conda**::
+        
+            conda install -c conda-forge kwantspectrum
+        
+        
+        Installation from source
+        ^^^^^^^^^^^^^^^^^^^^^^^^
+        
+        kwantSpectrum can be installed directly from the source code repository::
+        
+            python3 -m pip install --user git+https://gitlab.kwant-project.org/kwant/kwantspectrum.git
+        
+        For development, kwantSpectrum can be cloned from the official repository with::
+        
+            git clone https://gitlab.kwant-project.org/kwant/kwantspectrum.git
+        
+        The requirements listed below must be installed by hand.
+        
+        
+        Build requirements
+        ------------------
         
         kwantSpectrum has following non-Python dependency:
         
         - `Kwant <https://kwant-project.org/>`__
         
         Kwant can be installed with the following command::
         
@@ -45,59 +70,43 @@
         
         kwantSpectrum requires at least Python 3.5. The following packages must
         be installed to build kwantSpectrum:
         
         - `NumPy <https://numpy.org/>`_
         - `SciPy <https://www.scipy.org/>`_
         
-        Most packages can be installed from the command line
-        by the standard Python package manager `pip <https://pip.pypa.io/en/stable/>`_ via::
+        The packages can be installed by the standard *pip* command::
         
-            sudo pip3 install numpy scipy
+            python3 -m pip install --user numpy scipy
         
         Testing requirements
         --------------------
         The kwantSpectrum test suite requires the following Python packages:
         
         - `pytest <https://docs.pytest.org/en/latest/>`_
         - `pytest-cov <https://pytest-cov.readthedocs.io/en/latest/>`_
-        - `pytest-flake8 <https://pypi.org/project/pytest-flake8/>`_
         
         
         The packages can be installed by the standard *pip* command::
         
-            sudo pip3 install pytest pytest-cov pytest-flake8
+            python3 -m pip install --user pytest pytest-cov
         
         Documentation requirements
         --------------------------
         Building the documentation requires the following Python packages:
         
         - `matplotlib <https://matplotlib.org/>`_
         - `sphinx <https://www.sphinx-doc.org/en/master/>`_
         - `jupyter-sphinx <https://jupyter-sphinx.readthedocs.io/en/latest/>`_
         
         
         The packages can be installed by the standard *pip* command::
         
-            sudo pip3 install matplotlib sphinx jupyter-sphinx
-        
-        Building kwantSpectrum
-        ^^^^^^^^^^^^^^^^^^^^^^
-        
-        kwantSpectrum can be installed from PyPI with::
-        
-            sudo pip3 install kwantspectrum
+            python3 -m pip install --user matplotlib sphinx jupyter-sphinx
         
-        Alternatively, it can be installed directly from the source code repository::
-        
-            sudo pip3 install git+https://gitlab.kwant-project.org/kwant/kwantspectrum.git
-        
-        For development, kwantSpectrum can be cloned from the official repository with::
-        
-            git clone https://gitlab.kwant-project.org/kwant/kwantspectrum.git
         
         Test suite
         ----------
         
         Unittests can be run directly in the local source repository from the command line::
         
             pytest
@@ -161,14 +170,15 @@
         * Thomas Kloss (CEA Grenoble), kloss@itp.uni-frankfurt.de
         
         Contributors to the project are:
         
         * Christoph Groth (CEA Grenoble)
         * Xavier Waintal (CEA Grenoble)
         * Benoît Rossignol (CEA Grenoble)
+        * Bas Nijholt (Microsoft)
         
         (CEA = Commissariat à l'énergie atomique et aux énergies alternatives)
         
 Keywords: physics kwant bandstructure
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kwantspectrum-0.1.0/kwantspectrum.egg-info/SOURCES.txt` & `kwantspectrum-0.1.1/kwantspectrum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kwantspectrum-0.1.0/doc/Makefile` & `kwantspectrum-0.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kwantspectrum-0.1.0/doc/source/conf.py` & `kwantspectrum-0.1.1/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # The path is set in the Makefile, so that it also affects the Jupyter kernel
 # executed through the jupyter-sphinx extension.
 
 # -- Project information -----------------------------------------------------
 
 project = 'kwantspectrum'
-copyright = '2018-2019, T. Kloss, C. W. Groth, X. Waintal, et al.'
+copyright = '2018-2023, T. Kloss, C. W. Groth, X. Waintal, et al.'
 author = 'T. Kloss, C. W. Groth, X. Waintal, et al.'
 
 # The full version, including alpha/beta/rc tags.
 import kwantspectrum
 release = kwantspectrum.__version__
 
 # The short X.Y version.
@@ -34,15 +34,15 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
     'sphinx.ext.mathjax',
-    'jupyter_sphinx.execute',
+    'jupyter_sphinx',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -54,15 +54,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `kwantspectrum-0.1.0/doc/source/kwantdoctheme/static/kwantdoctheme.css` & `kwantspectrum-0.1.1/doc/source/kwantdoctheme/static/kwantdoctheme.css`

 * *Files identical despite different names*

### Comparing `kwantspectrum-0.1.0/doc/source/kwantdoctheme/theme.conf` & `kwantspectrum-0.1.1/doc/source/kwantdoctheme/theme.conf`

 * *Files identical despite different names*

### Comparing `kwantspectrum-0.1.0/doc/source/tutorial.rst` & `kwantspectrum-0.1.1/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `kwantspectrum-0.1.0/setup.py` & `kwantspectrum-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 #!/usr/bin/env python3
 
 import os
 import importlib
 import subprocess
 from setuptools import setup, find_packages
+
+# Until there is an alternative way to add custom build steps, make sure that
+# setuptools' local distutils copy is used.  This works around the removal of
+# distutils from stdlib.  See https://github.com/pypa/setuptools/issues/2928.
+os.environ['SETUPTOOLS_USE_DISTUTILS'] = 'local'
 from distutils.command.build import build as build_orig
 from setuptools.command.sdist import sdist as sdist_orig
 
 
 STATIC_VERSION_PATH = ('kwantspectrum', '_kwant_spectrum_version.py')
 
 distr_root = os.path.dirname(os.path.abspath(__file__))
@@ -24,16 +29,15 @@
     # Let kwantspectrum itself determine its own version.
     # We cannot simply import kwantspectrum, as it is not built yet.
     spec = importlib.util.spec_from_file_location('version', 'kwantspectrum/version.py')
     version_module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(version_module)
 
     version_module.ensure_python()
-    version = version_module.version
-    version_is_from_git = version_module.version_is_from_git
+    version, version_is_from_git = version_module.get_version()
 
 
 def write_version(fname):
     # This could be a hard link, so try to delete it first.  Is there any way
     # to do this atomically together with opening?
     try:
         os.remove(fname)
```

### Comparing `kwantspectrum-0.1.0/README.rst` & `kwantspectrum-0.1.1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -10,24 +10,49 @@
 
 kwantSpectrum is distributed under the `2-clause BSD license <https://gitlab.kwant-project.org/kwant/kwantspectrum/-/blob/master/LICENSE.rst>`_
 
 Website: https://kwant-project.org/extensions/kwantspectrum
 
 Source code: https://gitlab.kwant-project.org/kwant/kwantspectrum
 
+Conda package: https://github.com/conda-forge/kwantspectrum-feedstock
 
 
 Installation
 ############
 
-This section covers the installation of kwantSpectrum on a GNU/Linux
-system as Debian and Ubuntu via the command line.
+kwantSpectrum packages are hosted on PyPI and conda.
+The installation should work GNU/Linux system as Debian and Ubuntu,
+as well as on MacOS and Windows.
 
-Requirements
-^^^^^^^^^^^^
+**PyPI**::
+
+    python3 -m pip install --user kwantspectrum
+
+**conda**::
+
+    conda install -c conda-forge kwantspectrum
+
+
+Installation from source
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+kwantSpectrum can be installed directly from the source code repository::
+
+    python3 -m pip install --user git+https://gitlab.kwant-project.org/kwant/kwantspectrum.git
+
+For development, kwantSpectrum can be cloned from the official repository with::
+
+    git clone https://gitlab.kwant-project.org/kwant/kwantspectrum.git
+
+The requirements listed below must be installed by hand.
+
+
+Build requirements
+------------------
 
 kwantSpectrum has following non-Python dependency:
 
 - `Kwant <https://kwant-project.org/>`__
 
 Kwant can be installed with the following command::
 
@@ -37,59 +62,43 @@
 
 kwantSpectrum requires at least Python 3.5. The following packages must
 be installed to build kwantSpectrum:
 
 - `NumPy <https://numpy.org/>`_
 - `SciPy <https://www.scipy.org/>`_
 
-Most packages can be installed from the command line
-by the standard Python package manager `pip <https://pip.pypa.io/en/stable/>`_ via::
+The packages can be installed by the standard *pip* command::
 
-    sudo pip3 install numpy scipy
+    python3 -m pip install --user numpy scipy
 
 Testing requirements
 --------------------
 The kwantSpectrum test suite requires the following Python packages:
 
 - `pytest <https://docs.pytest.org/en/latest/>`_
 - `pytest-cov <https://pytest-cov.readthedocs.io/en/latest/>`_
-- `pytest-flake8 <https://pypi.org/project/pytest-flake8/>`_
 
 
 The packages can be installed by the standard *pip* command::
 
-    sudo pip3 install pytest pytest-cov pytest-flake8
+    python3 -m pip install --user pytest pytest-cov
 
 Documentation requirements
 --------------------------
 Building the documentation requires the following Python packages:
 
 - `matplotlib <https://matplotlib.org/>`_
 - `sphinx <https://www.sphinx-doc.org/en/master/>`_
 - `jupyter-sphinx <https://jupyter-sphinx.readthedocs.io/en/latest/>`_
 
 
 The packages can be installed by the standard *pip* command::
 
-    sudo pip3 install matplotlib sphinx jupyter-sphinx
-
-Building kwantSpectrum
-^^^^^^^^^^^^^^^^^^^^^^
-
-kwantSpectrum can be installed from PyPI with::
-
-    sudo pip3 install kwantspectrum
+    python3 -m pip install --user matplotlib sphinx jupyter-sphinx
 
-Alternatively, it can be installed directly from the source code repository::
-
-    sudo pip3 install git+https://gitlab.kwant-project.org/kwant/kwantspectrum.git
-
-For development, kwantSpectrum can be cloned from the official repository with::
-
-    git clone https://gitlab.kwant-project.org/kwant/kwantspectrum.git
 
 Test suite
 ----------
 
 Unittests can be run directly in the local source repository from the command line::
 
     pytest
@@ -153,9 +162,10 @@
 * Thomas Kloss (CEA Grenoble), kloss@itp.uni-frankfurt.de
 
 Contributors to the project are:
 
 * Christoph Groth (CEA Grenoble)
 * Xavier Waintal (CEA Grenoble)
 * Benoît Rossignol (CEA Grenoble)
+* Bas Nijholt (Microsoft)
 
 (CEA = Commissariat à l'énergie atomique et aux énergies alternatives)
```

