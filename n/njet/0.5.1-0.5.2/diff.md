# Comparing `tmp/njet-0.5.1.tar.gz` & `tmp/njet-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "njet-0.5.1.tar", last modified: Tue Mar 28 19:04:16 2023, max compression
+gzip compressed data, was "njet-0.5.2.tar", last modified: Tue May  2 11:33:13 2023, max compression
```

## Comparing `njet-0.5.1.tar` & `njet-0.5.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-03-28 19:04:16.788787 njet-0.5.1/
--rw-rw-r--   0 malte     (1000) malte     (1000)      265 2022-11-09 20:47:57.000000 njet-0.5.1/.readthedocs.yaml
--rw-rw-r--   0 malte     (1000) malte     (1000)      732 2023-01-19 12:13:38.000000 njet-0.5.1/LICENSE.txt
--rw-rw-r--   0 malte     (1000) malte     (1000)     3724 2023-03-28 19:04:16.788787 njet-0.5.1/PKG-INFO
--rw-rw-r--   0 malte     (1000) malte     (1000)     3203 2023-03-03 21:07:39.000000 njet-0.5.1/README.md
-drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-03-28 19:04:16.764787 njet-0.5.1/docs/
--rw-rw-r--   0 malte     (1000) malte     (1000)      638 2022-11-09 20:47:57.000000 njet-0.5.1/docs/Makefile
--rw-rw-r--   0 malte     (1000) malte     (1000)      799 2022-11-09 20:47:57.000000 njet-0.5.1/docs/make.bat
--rw-rw-r--   0 malte     (1000) malte     (1000)      496 2023-03-03 21:36:55.000000 njet-0.5.1/docs/requirements.txt
-drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-03-28 19:04:16.776787 njet-0.5.1/docs/source/
--rw-rw-r--   0 malte     (1000) malte     (1000)     3203 2023-03-03 21:07:39.000000 njet-0.5.1/docs/source/README.md
--rw-rw-r--   0 malte     (1000) malte     (1000)     7044 2022-11-09 20:47:57.000000 njet-0.5.1/docs/source/ad.rst
--rw-rw-r--   0 malte     (1000) malte     (1000)       92 2022-11-30 15:34:04.000000 njet-0.5.1/docs/source/common.rst
--rw-rw-r--   0 malte     (1000) malte     (1000)     2114 2023-01-19 12:16:09.000000 njet-0.5.1/docs/source/conf.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    22256 2023-03-28 10:59:29.000000 njet-0.5.1/docs/source/extras.rst
--rw-rw-r--   0 malte     (1000) malte     (1000)      860 2023-03-03 15:57:36.000000 njet-0.5.1/docs/source/functions.rst
--rw-rw-r--   0 malte     (1000) malte     (1000)      498 2023-03-09 20:24:42.000000 njet-0.5.1/docs/source/index.rst
--rw-rw-r--   0 malte     (1000) malte     (1000)     3806 2023-03-01 21:55:08.000000 njet-0.5.1/docs/source/jet.rst
--rw-rw-r--   0 malte     (1000) malte     (1000)     1657 2023-03-09 19:38:06.000000 njet-0.5.1/docs/source/poly.rst
-drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-03-28 19:04:16.764787 njet-0.5.1/njet/
--rw-rw-r--   0 malte     (1000) malte     (1000)      926 2023-03-16 13:09:20.000000 njet-0.5.1/njet/__init__.py
--rw-rw-r--   0 malte     (1000) malte     (1000)       22 2023-03-28 19:03:57.000000 njet-0.5.1/njet/_version.py
--rw-rw-r--   0 malte     (1000) malte     (1000)     6817 2023-03-16 13:06:56.000000 njet-0.5.1/njet/ad.py
--rw-rw-r--   0 malte     (1000) malte     (1000)     3580 2023-03-05 10:22:30.000000 njet-0.5.1/njet/common.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    49210 2023-03-21 10:17:25.000000 njet-0.5.1/njet/extras-Copy1.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    49145 2023-03-21 11:05:35.000000 njet-0.5.1/njet/extras-Copy2.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    49252 2023-03-24 13:34:50.000000 njet-0.5.1/njet/extras.py
--rw-rw-r--   0 malte     (1000) malte     (1000)     5486 2023-02-10 15:12:00.000000 njet-0.5.1/njet/functions.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    17316 2023-03-16 18:27:25.000000 njet-0.5.1/njet/jet-Copy1.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    17384 2023-03-23 13:07:48.000000 njet-0.5.1/njet/jet.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    12381 2023-03-21 19:58:18.000000 njet-0.5.1/njet/poly.py
-drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-03-28 19:04:16.776787 njet-0.5.1/njet.egg-info/
--rw-rw-r--   0 malte     (1000) malte     (1000)     3724 2023-03-28 19:04:16.000000 njet-0.5.1/njet.egg-info/PKG-INFO
--rw-rw-r--   0 malte     (1000) malte     (1000)      995 2023-03-28 19:04:16.000000 njet-0.5.1/njet.egg-info/SOURCES.txt
--rw-rw-r--   0 malte     (1000) malte     (1000)        1 2023-03-28 19:04:16.000000 njet-0.5.1/njet.egg-info/dependency_links.txt
--rw-rw-r--   0 malte     (1000) malte     (1000)      116 2023-03-28 19:04:16.000000 njet-0.5.1/njet.egg-info/requires.txt
--rw-rw-r--   0 malte     (1000) malte     (1000)        5 2023-03-28 19:04:16.000000 njet-0.5.1/njet.egg-info/top_level.txt
--rw-rw-r--   0 malte     (1000) malte     (1000)      683 2023-03-28 19:03:35.000000 njet-0.5.1/pyproject.toml
--rw-rw-r--   0 malte     (1000) malte     (1000)       38 2023-03-28 19:04:16.788787 njet-0.5.1/setup.cfg
--rw-rw-r--   0 malte     (1000) malte     (1000)     1214 2023-03-28 19:03:45.000000 njet-0.5.1/setup.py
-drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-03-28 19:04:16.784787 njet-0.5.1/test/
--rw-rw-r--   0 malte     (1000) malte     (1000)    13475 2023-03-01 20:11:19.000000 njet-0.5.1/test/_test.py
--rw-rw-r--   0 malte     (1000) malte     (1000)     1280 2023-02-10 16:22:05.000000 njet-0.5.1/test/example1.npy
--rw-rw-r--   0 malte     (1000) malte     (1000)     1280 2023-02-10 16:22:09.000000 njet-0.5.1/test/example1_result1.npy
--rw-rw-r--   0 malte     (1000) malte     (1000)    10496 2023-02-10 16:22:09.000000 njet-0.5.1/test/example1_result2.npy
--rw-rw-r--   0 malte     (1000) malte     (1000)      256 2023-02-10 16:22:59.000000 njet-0.5.1/test/example2_result_0.npy
--rw-rw-r--   0 malte     (1000) malte     (1000)      256 2023-02-10 16:22:59.000000 njet-0.5.1/test/example2_result_1.npy
--rw-rw-r--   0 malte     (1000) malte     (1000)      256 2023-02-10 16:22:59.000000 njet-0.5.1/test/example2_result_2.npy
--rw-rw-r--   0 malte     (1000) malte     (1000)     3531 2023-03-23 20:10:06.000000 njet-0.5.1/test/test_docs.py
--rw-rw-r--   0 malte     (1000) malte     (1000)    18253 2023-03-20 18:03:16.000000 njet-0.5.1/test/test_extras.py
--rw-rw-r--   0 malte     (1000) malte     (1000)     3454 2023-02-10 16:23:52.000000 njet-0.5.1/test/test_xmpl_issue11.py
+drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-05-02 11:33:13.524747 njet-0.5.2/
+-rw-rw-r--   0 malte     (1000) malte     (1000)      265 2022-11-09 20:47:57.000000 njet-0.5.2/.readthedocs.yaml
+-rw-rw-r--   0 malte     (1000) malte     (1000)      732 2023-01-19 12:13:38.000000 njet-0.5.2/LICENSE.txt
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3724 2023-05-02 11:33:13.524747 njet-0.5.2/PKG-INFO
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3203 2023-03-03 21:07:39.000000 njet-0.5.2/README.md
+drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-05-02 11:33:13.504747 njet-0.5.2/docs/
+-rw-rw-r--   0 malte     (1000) malte     (1000)      638 2022-11-09 20:47:57.000000 njet-0.5.2/docs/Makefile
+-rw-rw-r--   0 malte     (1000) malte     (1000)      799 2022-11-09 20:47:57.000000 njet-0.5.2/docs/make.bat
+-rw-rw-r--   0 malte     (1000) malte     (1000)      496 2023-03-03 21:36:55.000000 njet-0.5.2/docs/requirements.txt
+drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-05-02 11:33:13.508747 njet-0.5.2/docs/source/
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3203 2023-03-03 21:07:39.000000 njet-0.5.2/docs/source/README.md
+-rw-rw-r--   0 malte     (1000) malte     (1000)     7044 2022-11-09 20:47:57.000000 njet-0.5.2/docs/source/ad.rst
+-rw-rw-r--   0 malte     (1000) malte     (1000)       92 2022-11-30 15:34:04.000000 njet-0.5.2/docs/source/common.rst
+-rw-rw-r--   0 malte     (1000) malte     (1000)     2114 2023-01-19 12:16:09.000000 njet-0.5.2/docs/source/conf.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    22391 2023-04-18 07:12:51.000000 njet-0.5.2/docs/source/extras.rst
+-rw-rw-r--   0 malte     (1000) malte     (1000)      860 2023-03-03 15:57:36.000000 njet-0.5.2/docs/source/functions.rst
+-rw-rw-r--   0 malte     (1000) malte     (1000)      498 2023-03-09 20:24:42.000000 njet-0.5.2/docs/source/index.rst
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3806 2023-03-01 21:55:08.000000 njet-0.5.2/docs/source/jet.rst
+-rw-rw-r--   0 malte     (1000) malte     (1000)     1657 2023-03-09 19:38:06.000000 njet-0.5.2/docs/source/poly.rst
+drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-05-02 11:33:13.500747 njet-0.5.2/njet/
+-rw-rw-r--   0 malte     (1000) malte     (1000)      926 2023-03-16 13:09:20.000000 njet-0.5.2/njet/__init__.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)       22 2023-05-02 11:32:59.000000 njet-0.5.2/njet/_version.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)     7275 2023-04-21 12:54:35.000000 njet-0.5.2/njet/ad.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3665 2023-04-03 12:03:01.000000 njet-0.5.2/njet/common.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    49210 2023-03-21 10:17:25.000000 njet-0.5.2/njet/extras-Copy1.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    49145 2023-03-21 11:05:35.000000 njet-0.5.2/njet/extras-Copy2.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    49848 2023-04-26 13:40:10.000000 njet-0.5.2/njet/extras.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)     5486 2023-02-10 15:12:00.000000 njet-0.5.2/njet/functions.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    17316 2023-03-16 18:27:25.000000 njet-0.5.2/njet/jet-Copy1.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    17384 2023-04-21 12:42:15.000000 njet-0.5.2/njet/jet.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    12381 2023-03-21 19:58:18.000000 njet-0.5.2/njet/poly.py
+drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-05-02 11:33:13.512747 njet-0.5.2/njet.egg-info/
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3724 2023-05-02 11:33:13.000000 njet-0.5.2/njet.egg-info/PKG-INFO
+-rw-rw-r--   0 malte     (1000) malte     (1000)      995 2023-05-02 11:33:13.000000 njet-0.5.2/njet.egg-info/SOURCES.txt
+-rw-rw-r--   0 malte     (1000) malte     (1000)        1 2023-05-02 11:33:13.000000 njet-0.5.2/njet.egg-info/dependency_links.txt
+-rw-rw-r--   0 malte     (1000) malte     (1000)      116 2023-05-02 11:33:13.000000 njet-0.5.2/njet.egg-info/requires.txt
+-rw-rw-r--   0 malte     (1000) malte     (1000)        5 2023-05-02 11:33:13.000000 njet-0.5.2/njet.egg-info/top_level.txt
+-rw-rw-r--   0 malte     (1000) malte     (1000)      683 2023-05-02 11:32:22.000000 njet-0.5.2/pyproject.toml
+-rw-rw-r--   0 malte     (1000) malte     (1000)       38 2023-05-02 11:33:13.524747 njet-0.5.2/setup.cfg
+-rw-rw-r--   0 malte     (1000) malte     (1000)     1214 2023-05-02 11:32:41.000000 njet-0.5.2/setup.py
+drwxrwxr-x   0 malte     (1000) malte     (1000)        0 2023-05-02 11:33:13.524747 njet-0.5.2/test/
+-rw-rw-r--   0 malte     (1000) malte     (1000)    13475 2023-03-01 20:11:19.000000 njet-0.5.2/test/_test.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)     1280 2023-02-10 16:22:05.000000 njet-0.5.2/test/example1.npy
+-rw-rw-r--   0 malte     (1000) malte     (1000)     1280 2023-02-10 16:22:09.000000 njet-0.5.2/test/example1_result1.npy
+-rw-rw-r--   0 malte     (1000) malte     (1000)    10496 2023-02-10 16:22:09.000000 njet-0.5.2/test/example1_result2.npy
+-rw-rw-r--   0 malte     (1000) malte     (1000)      256 2023-02-10 16:22:59.000000 njet-0.5.2/test/example2_result_0.npy
+-rw-rw-r--   0 malte     (1000) malte     (1000)      256 2023-02-10 16:22:59.000000 njet-0.5.2/test/example2_result_1.npy
+-rw-rw-r--   0 malte     (1000) malte     (1000)      256 2023-02-10 16:22:59.000000 njet-0.5.2/test/example2_result_2.npy
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3531 2023-03-23 20:10:06.000000 njet-0.5.2/test/test_docs.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)    18253 2023-03-20 18:03:16.000000 njet-0.5.2/test/test_extras.py
+-rw-rw-r--   0 malte     (1000) malte     (1000)     3454 2023-02-10 16:23:52.000000 njet-0.5.2/test/test_xmpl_issue11.py
```

### Comparing `njet-0.5.1/LICENSE.txt` & `njet-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/PKG-INFO` & `njet-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: njet
-Version: 0.5.1
+Version: 0.5.2
 Summary: Lightweight automatic differentiation package for higher-order differentiation.
 Author: Malte Titze
 Author-email: mtitze@users.noreply.github.com
 License: GPL-3.0-or-later
 Project-URL: homepage, https://njet.readthedocs.io/en/latest/index.html
 Project-URL: repository, https://github.com/mtitze/njet
 Keywords: AD jet njet automatic differentiation
```

### Comparing `njet-0.5.1/README.md` & `njet-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/Makefile` & `njet-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/make.bat` & `njet-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/source/README.md` & `njet-0.5.2/docs/source/README.md`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/source/ad.rst` & `njet-0.5.2/docs/source/ad.rst`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/source/conf.py` & `njet-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/source/extras.rst` & `njet-0.5.2/docs/source/extras.rst`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,21 @@
 
 In the case that a chain of functions of the form :math:`f_N \circ f_{N - 1} ... \circ f_1` needs to be differentiated, and there are repetitions of :math:`f_k`'s in the chain, the generalized Faa di Bruno formula may help in reducing the amount of calculations required.
 
 For example, if we want to compute a chain of :math:`2^N` repetitions of the same function :math:`f`, then we can first compute the composition :math:`f_2 := f \circ f`, then the compositon :math:`f_4 := f_2 \circ f_2` and so on, until we are finished after :math:`N` steps.
 
 Moreover, if a chain indeed admits repetitions, a single point will pass through a specific function several times while it is transported from :math:`f_1` to :math:`f_N`. We can take advantage of this by calculating the derivatives at these 'intersecting' points for each unique element of the chain in parallel, using NumPy.
  
-In order to manage function chains, the dedicated class ``cderive`` has been created. This class takes a series of functions, defining the *unique* functions in the chain, an ``order`` parameter, defining the number of derivatives to be computed and an optional ``ordering`` parameter, which is a list of integers and defines the chain itself. For example, consider an alternation of a rotation and some
+To conveniently manage chains of functions, the dedicated class ``cderive`` ('chain-derive') has been implemented. This class takes a series of functions, defining the *unique* functions in the chain, an ``order`` parameter, defining the number of derivatives to be computed and an optional ``ordering`` parameter, which is a list of integers and defines the chain itself. It can be imported with the following line:
+
+.. code-block:: python
+
+    from njet.extras import cderive
+
+As an example, consider an alternation of a rotation and some
 polynomial perturbation :math:`M = 15` times:
 
 .. code-block:: python
 
     from njet.functions import sin, cos
 
     g = 1
@@ -207,15 +213,15 @@
 .. code-block:: python
 
     drp.jev(4)[0].taylor_coefficients(n_args=2)
   > {(0, 0): (-0.0911100230191827+0j),
      (1, 0): 0.34364574631604705,
      (0, 1): -0.9390993563190676}
 
-In some circumstances, however, previously computed jet-evaluations remain valid. For example, this is the case if we want to extract a subchain of a given chain, defined by a slice of neighbouring indices. We can extracted subchains from the original chain in the same manner as it can be done with lists. For example:
+In some circumstances, however, previously computed jet-evaluations remain valid. For example, this is the case if we want to extract a subchain of a given chain, defined by a slice of neighbouring indices. We can extract subchains from the original chain in the same manner as it can be done with lists. For example:
 
 .. code-block:: python
 
     mysubchain = drp[1:13]
     mysubchain.jev(3)[0].taylor_coefficients(n_args=2)
   > {(0, 0): (-0.0911100230191827+0j),
      (1, 0): 0.34364574631604705,
```

### Comparing `njet-0.5.1/docs/source/functions.rst` & `njet-0.5.2/docs/source/functions.rst`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/source/jet.rst` & `njet-0.5.2/docs/source/jet.rst`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/docs/source/poly.rst` & `njet-0.5.2/docs/source/poly.rst`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet/__init__.py` & `njet-0.5.2/njet/__init__.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet/ad.py` & `njet-0.5.2/njet/ad.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,56 @@
             out = [out]
     except:
         out = (*[ev.taylor_coefficients(**kwargs) for ev in evaluation],) # also stored in ev._tc
         if len(out) == 1 and output_format == 0:
             out = out[0]
     return out
 
+def build_tensor(D, k: int, **kwargs):
+    '''
+    Convert the components of the k-th derivative into the entries of a (self.n_args)**k tensor.
+    See njet.jet.build_tensor for details.
+    
+    Parameters
+    ----------
+    D: derive or cderive object
+    
+    k: int
+        The number of derivatives to be considered.
+    
+    Returns
+    -------
+    dict or list
+    '''
+    assert k <= D.order, f'Order ({D.order}) insufficient for requested number ({k}) of derivatives.'
+    assert hasattr(D, '_evaluation'), 'Derivative(s) need to be evaluated first. Try passing a point.'
+    try:
+        return D._evaluation.build_tensor(k=k, **kwargs)
+    except:
+        # Underlying function may be vector-valued:
+        return [ev.build_tensor(k=k, **kwargs) for ev in D._evaluation]
+
+def grad(D, *z, **kwargs):
+    '''
+    Returns the gradient of the current function.
+    See njet.jet.grad for details.
+    '''
+    if len(z) > 0:
+        _ = D(*z, **kwargs)
+    return build_tensor(D, k=1, **kwargs)
+
+def hess(D, *z, **kwargs):
+    '''
+    Returns the Hessian of the function.
+    See njet.jet.hess for details.
+    '''
+    if len(z) > 0:
+        _ = D(*z, **kwargs)
+    return build_tensor(D, k=2, **kwargs)
+
 class derive:
     '''
     Class to handle the derivatives of a (jet-)function (i.e. a function consisting of a composition
     of elementary functions).
     
     Parameters
     ----------
@@ -168,35 +210,17 @@
             Dictionary of compontens of the multivariate Taylor expansion of the given function self.jetfunc
         '''
         # These two keywords are reserved for the taylor_coefficients routine and will be removed from the input:
         mult_prm = kwargs.pop('mult_prm', True)
         mult_drv = kwargs.pop('mult_drv', True)
         # perform the computation, based on the input vector
         return taylor_coefficients(self.eval(*z, **kwargs), n_args=self.n_args, mult_prm=mult_prm, mult_drv=mult_drv)
-        
-    def build_tensor(self, k: int, **kwargs):
-        '''
-        Convert the components of the k-th derivative into the entries of a (self.n_args)**k tensor.
-        See njet.jet.build_tensor for details.
-        '''
-        assert k <= self.order, f'Order ({self.order}) insufficient for requested number ({k}) of derivatives.'
-        assert hasattr(self, '_evaluation'), 'Derivative(s) need to be evaluated first. Try passing a point.'
-        return self._evaluation.build_tensor(k=k, **kwargs)
     
-    def grad(self, *z, **kwargs):
-        '''
-        Returns the gradient of the current function.
-        See njet.jet.grad for details.
-        '''
-        if len(z) > 0:
-            _ = self(*z, **kwargs)
-        return self.build_tensor(k=1, **kwargs)
+    def build_tensor(self, *args, **kwargs):
+        return build_tensor(self, *args, **kwargs)
     
-    def hess(self, *z, **kwargs):
-        '''
-        Returns the Hessian of the function.
-        See njet.jet.hess for details.
-        '''
-        if len(z) > 0:
-            _ = self(*z, **kwargs)
-        return self.build_tensor(k=2, **kwargs)
+    def grad(self, *args, **kwargs):
+        return grad(self, *args, **kwargs)
+    
+    def hess(self, *args, **kwargs):
+        return hess(self, *args, **kwargs)
```

### Comparing `njet-0.5.1/njet/common.py` & `njet-0.5.2/njet/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
     # check if a value is zero; value may be an iterable
     check = value == 0
     if hasattr(check, '__iter__'):
         try:
             return check.all()
         except:
             return all(check)
+    elif isinstance(value, list):
+        return all([check_zero(e) for e in value])
     else:
         return check
     
 def factorials(n: int):
     k = 1
     facts = [1]
     for j in range(1, n + 1):
```

### Comparing `njet-0.5.1/njet/extras-Copy1.py` & `njet-0.5.2/njet/extras-Copy1.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet/extras-Copy2.py` & `njet-0.5.2/njet/extras-Copy2.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet/extras.py` & `njet-0.5.2/njet/extras.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from tqdm import tqdm
 from copy import copy
 import warnings
 import gc
 
 from . import jet, jetpoly, derive, taylor_coefficients
 from .common import factorials, check_zero
+from .ad import build_tensor, grad, hess
 
 def accel_asc(n: int):
     '''
     Compute the partitions of a given integer.
     
     Parameters
     ----------
@@ -445,14 +446,17 @@
         # passing through the given chain will pass through the element.
         # So for example, self.path[k] = [j1, j2, j3, ...] means that
         # the first passage through element k occurs at global position j1,
         # the second passage through element k occurs at global position j2 etc.
         self.path = {k: [] for k in uord}
         for j in range(len(self)):
             self.path[self.ordering[j]].append(j)
+            
+        # The number of input parameters equals the one of the first function:
+        self.n_args = self.dfunctions[self.ordering[0]].n_args
 
         if not reset:
             # check at least if the (new) path is consistent with the given data:
             _ = self._check_path_consistency()
         else:
             self.reset()
         
@@ -495,14 +499,15 @@
             Keyworded arguments passed to the underlying jet-functions.
             
         Returns
         -------
         single value or array-like
             The final value after the chain of functions has been traversed.
         '''
+        assert len(point) == self.n_args, f'Input point has length {len(point)}, expected: {self.n_args}'
         self._input = point
         out = [point]
         for k in range(len(self)):
             point = self.dfunctions[self.ordering[k]].jetfunc(*point, **kwargs)
             out.append(point)
         self._output = out
         return point
@@ -565,15 +570,15 @@
             
             One can pass the boolean parameter disable_tqdm to enable (if False) a progress bar.
             
         Returns
         -------
         list
             The outcome of self.compose routine (containing the jet-evaluations for each component).
-        '''        
+        '''
         _ = self.jetfunc(*point, **kwargs)
         points_at_functions = [[self._output[l] for l in range(len(self)) if self.ordering[l] == k] for k in range(self.n_functions)]
         # let Q = points_per_function[j], so Q is a list of points which needs to be computed for function j
         # Then the first element in Q is the one which needs to be applied first, etc. (for element j) by this construction.
         
         for k in tqdm(range(self.n_functions), disable=kwargs.get('disable_tqdm', True)):
             function = self.dfunctions[k].jetfunc
@@ -639,20 +644,18 @@
         kwargs_changed = False
         if hasattr(self, '_call_kwargs'):
             kwargs_changed = self._call_kwargs != kwargs
         elif len(kwargs) > 0:
             kwargs_changed = True
             
         # Determine if a (re-)evaluation is required
-        eval_required = False
-        if len(z) > 0:
-            if not all([hasattr(df, '_evaluation') for df in self.dfunctions]):
-                eval_required = True
-            elif not self._probe(*z, **kwargs):
-                eval_required = True
+        eval_required = not all([hasattr(df, '_evaluation') for df in self.dfunctions])            
+        if len(z) > 0 and not eval_required:
+            eval_required = not self._probe(*z, **kwargs)
+            
         return eval_required, kwargs_changed
 
     def __call__(self, *z, **kwargs):
         '''
         Compute the derivatives of the chain of functions at a given point.
         
         Parameters
@@ -879,14 +882,15 @@
             A function taking an integer (pos) and returning the jet-evaluation at this position. It will
             have a similar functionality than self.jev, with the difference that it will take values from
             0 to 2*len(self) instead.
         '''
         # Check if given input is stored in the database. If not, re-evaluate.
         eval_required, kwargs_changed = self._eval_memcheck(*point, **kwargs)
         if eval_required:
+            assert len(point) > 0, 'Evaluation input point required.'
             if warn:
                 warnings.warn('Input parameter(s) changed; re-evaluating ...')
             self.eval(*point, compose=False, **kwargs)
 
         # In the non-periodic case the evaluation data might have to be extended.
         # Check if end-point agrees with the start.
         inp = self.dfunctions[self.ordering[0]]._input
@@ -1016,14 +1020,23 @@
                 jets_l = ([cycling_data[k][icmp] for k in range(len(ordering)) if ordering[k] == l] for icmp in range(n_args))
                 new_functions[l]._evaluation = [_jbuild(jc) for jc in jets_l]
             result = self.__class__(*new_functions, ordering=ordering, order=self.order, run_params=self.run_params, reset=False)
         del cycling_data # without this, the memory demand will increase
         gc.collect() # cleanup to prevent cluttering of memory
         return result
     
+    def build_tensor(self, *args, **kwargs):
+        return build_tensor(self, *args, **kwargs)
+    
+    def grad(self, *args, **kwargs):
+        return grad(self, *args, **kwargs)
+    
+    def hess(self, *args, **kwargs):
+        return hess(self, *args, **kwargs)
+    
 ########################################################
 # Helper functions to deal with patterns and orderings #
 ########################################################
     
 def _pattern_reordering(ordering, pattern=(), positions=None, placeholder=-1):
     '''
     Replace a given sequence of patterns within an ordering,
```

### Comparing `njet-0.5.1/njet/functions.py` & `njet-0.5.2/njet/functions.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet/jet-Copy1.py` & `njet-0.5.2/njet/jet-Copy1.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet/jet.py` & `njet-0.5.2/njet/jet.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet/poly.py` & `njet-0.5.2/njet/poly.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/njet.egg-info/PKG-INFO` & `njet-0.5.2/njet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: njet
-Version: 0.5.1
+Version: 0.5.2
 Summary: Lightweight automatic differentiation package for higher-order differentiation.
 Author: Malte Titze
 Author-email: mtitze@users.noreply.github.com
 License: GPL-3.0-or-later
 Project-URL: homepage, https://njet.readthedocs.io/en/latest/index.html
 Project-URL: repository, https://github.com/mtitze/njet
 Keywords: AD jet njet automatic differentiation
```

### Comparing `njet-0.5.1/njet.egg-info/SOURCES.txt` & `njet-0.5.2/njet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/pyproject.toml` & `njet-0.5.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "njet"
-version = "0.5.1"
+version = "0.5.2"
 description = "Lightweight automatic differentiation package for higher-order differentiation."
 authors = [ "Malte Titze <mtitze@users.noreply.github.com>",]
 license = "GPL-3.0-or-later"
 homepage = "https://njet.readthedocs.io/en/latest/index.html"
 repository = "https://github.com/mtitze/njet"
 keywords = [ "AD", "jet", "njet", "automatic", "differentiation",]
```

### Comparing `njet-0.5.1/setup.py` & `njet-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def get_long_description():
     with open(f'./README.md', encoding='utf8') as fp:
         return fp.read()
         
 setup(
     long_description=get_long_description(),
     name='njet',
-    version='0.5.1',
+    version='0.5.2',
     description='Lightweight automatic differentiation package for higher-order differentiation.',
     long_description_content_type='text/markdown',
     python_requires='<3.11,>=3.8',
     project_urls={
         "homepage": "https://njet.readthedocs.io/en/latest/index.html",
         "repository": "https://github.com/mtitze/njet"
     },
```

### Comparing `njet-0.5.1/test/_test.py` & `njet-0.5.2/test/_test.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/test/example1.npy` & `njet-0.5.2/test/example1.npy`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/test/example1_result1.npy` & `njet-0.5.2/test/example1_result1.npy`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/test/example1_result2.npy` & `njet-0.5.2/test/example1_result2.npy`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/test/test_docs.py` & `njet-0.5.2/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/test/test_extras.py` & `njet-0.5.2/test/test_extras.py`

 * *Files identical despite different names*

### Comparing `njet-0.5.1/test/test_xmpl_issue11.py` & `njet-0.5.2/test/test_xmpl_issue11.py`

 * *Files identical despite different names*

