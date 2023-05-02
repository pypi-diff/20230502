# Comparing `tmp/curvit-1.6.5.tar.gz` & `tmp/curvit-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvit-1.6.5.tar", last modified: Fri Apr 28 13:37:19 2023, max compression
+gzip compressed data, was "curvit-1.6.6.tar", last modified: Tue May  2 10:49:03 2023, max compression
```

## Comparing `curvit-1.6.5.tar` & `curvit-1.6.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 13:37:19.231493 curvit-1.6.5/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.5/LICENSE
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 13:37:19.231493 curvit-1.6.5/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.5/README.md
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 13:37:19.230493 curvit-1.6.5/curvit/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      133 2023-03-19 15:24:32.000000 curvit-1.6.5/curvit/__init__.py
--rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.5/curvit/check_curvit_variability_V.0.4.py
--rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    79693 2023-04-28 13:32:33.000000 curvit-1.6.5/curvit/curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      355 2021-06-25 20:52:41.000000 curvit-1.6.5/curvit/profile_curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1003 2022-12-10 20:44:29.000000 curvit-1.6.5/curvit/test_curvit.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 13:37:19.230493 curvit-1.6.5/curvit.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       63 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/top_level.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-28 13:37:19.231493 curvit-1.6.5/setup.cfg
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      894 2023-04-28 13:32:52.000000 curvit-1.6.5/setup.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-02 10:49:03.098118 curvit-1.6.6/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.6/LICENSE
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-02 10:49:03.098118 curvit-1.6.6/PKG-INFO
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.6/README.md
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-02 10:49:03.096118 curvit-1.6.6/curvit/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      133 2023-03-19 15:24:32.000000 curvit-1.6.6/curvit/__init__.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.6/curvit/check_curvit_variability_V.0.4.py
+-rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    79859 2023-05-02 09:51:17.000000 curvit-1.6.6/curvit/curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      355 2021-06-25 20:52:41.000000 curvit-1.6.6/curvit/profile_curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1003 2022-12-10 20:44:29.000000 curvit-1.6.6/curvit/test_curvit.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-02 10:49:03.097118 curvit-1.6.6/curvit.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-02 10:49:03.000000 curvit-1.6.6/curvit.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-05-02 10:49:03.000000 curvit-1.6.6/curvit.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-05-02 10:49:03.000000 curvit-1.6.6/curvit.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       63 2023-05-02 10:49:03.000000 curvit-1.6.6/curvit.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-05-02 10:49:03.000000 curvit-1.6.6/curvit.egg-info/top_level.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-05-02 10:49:03.098118 curvit-1.6.6/setup.cfg
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      894 2023-05-02 10:41:26.000000 curvit-1.6.6/setup.py
```

### Comparing `curvit-1.6.5/LICENSE` & `curvit-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `curvit-1.6.5/PKG-INFO` & `curvit-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.5
+Version: 1.6.6
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.5 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.6 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.5/README.md` & `curvit-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `curvit-1.6.5/curvit/check_curvit_variability_V.0.4.py` & `curvit-1.6.6/curvit/check_curvit_variability_V.0.4.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.5/curvit/curvit.py` & `curvit-1.6.6/curvit/curvit.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,22 +158,25 @@
     weighted_y = np.sum(y_bin_centres * y_array_mask) / np.sum(y_array_mask)
     
     return (weighted_x, weighted_y)
 
 
 def read_columns(events_list):
     # Reading few columns.
-    f = fits.open(events_list)
-    time = f[1].data['MJD_L2']
-    fx = f[1].data['Fx']
-    fy = f[1].data['Fy']
-    photons = f[1].data['EFFECTIVE_NUM_PHOTONS']
-    bad_flag = f[1].data['BAD FLAG']
+    hdu = fits.open(events_list)
+    time = hdu[1].data['MJD_L2']
+    fx = hdu[1].data['Fx']
+    fy = hdu[1].data['Fy']
+    photons = hdu[1].data['EFFECTIVE_NUM_PHOTONS']
+    bad_flag = hdu[1].data['BAD FLAG']
     mask = photons > 0 
     mask = np.logical_and(mask, bad_flag)
+    if 'FrameCount' in hdu[1].data.names:
+        first_frame_mask = hdu[1].data['FrameCount'] != 1
+        mask = np.logical_and(mask, first_frame_mask)
     time = time[mask]
     fx = fx[mask]
     fy = fy[mask]
     photons = photons[mask]
     return time, fx, fy, photons
```

### Comparing `curvit-1.6.5/curvit/test_curvit.py` & `curvit-1.6.6/curvit/test_curvit.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.5/curvit.egg-info/PKG-INFO` & `curvit-1.6.6/curvit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.5
+Version: 1.6.6
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.5 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.6 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.5/setup.py` & `curvit-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="curvit", 
-    version="1.6.5",
+    version="1.6.6",
     author="Prajwel Joseph",
     author_email="prajwel.joseph@gmail.com",
     description="light curves from UVIT data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prajwel/curvit",
     packages=setuptools.find_packages(),
```

