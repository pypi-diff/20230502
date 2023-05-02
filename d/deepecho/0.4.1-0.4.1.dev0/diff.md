# Comparing `tmp/deepecho-0.4.1.tar.gz` & `tmp/deepecho-0.4.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepecho-0.4.1.tar", last modified: Tue May  2 18:08:33 2023, max compression
+gzip compressed data, was "deepecho-0.4.1.dev0.tar", last modified: Mon May  1 23:19:44 2023, max compression
```

## Comparing `deepecho-0.4.1.tar` & `deepecho-0.4.1.dev0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.533993 deepecho-0.4.1/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       61 2023-01-10 22:50:52.000000 deepecho-0.4.1/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8325 2023-01-09 19:52:40.000000 deepecho-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3220 2023-05-02 18:08:31.000000 deepecho-0.4.1/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4825 2023-01-10 22:50:52.000000 deepecho-0.4.1/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      296 2023-01-09 19:52:40.000000 deepecho-0.4.1/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14181 2023-05-02 18:08:33.534146 deepecho-0.4.1/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7897 2023-01-10 22:50:52.000000 deepecho-0.4.1/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.531074 deepecho-0.4.1/deepecho/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      382 2023-05-02 18:08:31.000000 deepecho-0.4.1/deepecho/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.532129 deepecho-0.4.1/deepecho/data/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    28256 2023-01-09 19:52:40.000000 deepecho-0.4.1/deepecho/data/demo.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      266 2023-01-09 19:52:40.000000 deepecho-0.4.1/deepecho/demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.533074 deepecho-0.4.1/deepecho/models/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2023-01-09 19:52:40.000000 deepecho-0.4.1/deepecho/models/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10617 2023-05-02 18:08:31.000000 deepecho-0.4.1/deepecho/models/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21506 2023-01-10 22:50:52.000000 deepecho-0.4.1/deepecho/models/basic_gan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22393 2023-01-10 22:50:52.000000 deepecho-0.4.1/deepecho/models/par.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7223 2023-01-10 22:50:52.000000 deepecho-0.4.1/deepecho/sequences.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.531987 deepecho-0.4.1/deepecho.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14181 2023-05-02 18:08:33.000000 deepecho-0.4.1/deepecho.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      631 2023-05-02 18:08:33.000000 deepecho-0.4.1/deepecho.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-02 18:08:33.000000 deepecho-0.4.1/deepecho.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-02 18:08:33.000000 deepecho-0.4.1/deepecho.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1063 2023-05-02 18:08:33.000000 deepecho-0.4.1/deepecho.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        9 2023-05-02 18:08:33.000000 deepecho-0.4.1/deepecho.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1665 2023-05-02 18:08:33.534646 deepecho-0.4.1/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3196 2023-05-02 18:08:31.000000 deepecho-0.4.1/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.533223 deepecho-0.4.1/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2023-01-10 22:50:52.000000 deepecho-0.4.1/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.533594 deepecho-0.4.1/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-10 22:50:52.000000 deepecho-0.4.1/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3942 2023-01-10 22:50:52.000000 deepecho-0.4.1/tests/integration/test_basic_gan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3886 2023-01-10 22:50:52.000000 deepecho-0.4.1/tests/integration/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:08:33.533844 deepecho-0.4.1/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       37 2023-01-10 22:50:52.000000 deepecho-0.4.1/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6642 2023-01-10 22:50:52.000000 deepecho-0.4.1/tests/unit/test_sequences.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.056959 deepecho-0.4.1.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       61 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8325 2023-01-09 19:52:40.000000 deepecho-0.4.1.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2915 2023-01-10 22:53:55.000000 deepecho-0.4.1.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4825 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      296 2023-01-09 19:52:40.000000 deepecho-0.4.1.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13809 2023-05-01 23:19:44.057159 deepecho-0.4.1.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7897 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.053795 deepecho-0.4.1.dev0/deepecho/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      387 2023-01-10 22:51:22.000000 deepecho-0.4.1.dev0/deepecho/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.054867 deepecho-0.4.1.dev0/deepecho/data/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    28256 2023-01-09 19:52:40.000000 deepecho-0.4.1.dev0/deepecho/data/demo.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      266 2023-01-09 19:52:40.000000 deepecho-0.4.1.dev0/deepecho/demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.055755 deepecho-0.4.1.dev0/deepecho/models/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2023-01-09 19:52:40.000000 deepecho-0.4.1.dev0/deepecho/models/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10617 2023-05-01 23:18:26.000000 deepecho-0.4.1.dev0/deepecho/models/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21506 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/deepecho/models/basic_gan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22393 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/deepecho/models/par.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7223 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/deepecho/sequences.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.054733 deepecho-0.4.1.dev0/deepecho.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13809 2023-05-01 23:19:44.000000 deepecho-0.4.1.dev0/deepecho.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      631 2023-05-01 23:19:44.000000 deepecho-0.4.1.dev0/deepecho.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-01 23:19:44.000000 deepecho-0.4.1.dev0/deepecho.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-01 23:19:44.000000 deepecho-0.4.1.dev0/deepecho.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1063 2023-05-01 23:19:44.000000 deepecho-0.4.1.dev0/deepecho.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        9 2023-05-01 23:19:44.000000 deepecho-0.4.1.dev0/deepecho.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1670 2023-05-01 23:19:44.057687 deepecho-0.4.1.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3201 2023-05-01 23:18:26.000000 deepecho-0.4.1.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.055908 deepecho-0.4.1.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.056436 deepecho-0.4.1.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3942 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/tests/integration/test_basic_gan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3886 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/tests/integration/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 23:19:44.056805 deepecho-0.4.1.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       37 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6642 2023-01-10 22:50:52.000000 deepecho-0.4.1.dev0/tests/unit/test_sequences.py
```

### Comparing `deepecho-0.4.1/CONTRIBUTING.rst` & `deepecho-0.4.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/HISTORY.md` & `deepecho-0.4.1.dev0/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 # History
 
-## 0.4.1 - 2023-05-02
-
-This release adds support for Pandas 2.0 and PyTorch 2.0!
-
-### Maintenance
-
-* Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by @frances-h
-* Upgrade to Torch 2.0 - Issue [#70](https://github.com/sdv-dev/DeepEcho/issues/70) by @frances-h
-
 ## 0.4.0 - 2023-01-10
 
 This release adds support for python 3.10 and 3.11. It also drops support for python 3.6.
 
 ### Maintenance
 
 * Support Python 3.10 and 3.11 - Issue [#63](https://github.com/sdv-dev/DeepEcho/issues/63) by @pvk-developer
```

### Comparing `deepecho-0.4.1/LICENSE` & `deepecho-0.4.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/PKG-INFO` & `deepecho-0.4.1.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepecho
-Version: 0.4.1
+Version: 0.4.1.dev0
 Summary: Create sequential synthetic data of mixed types using a GAN.
 Home-page: https://github.com/sdv-dev/DeepEcho
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Description: <div align="center">
         <br/>
@@ -189,23 +189,14 @@
         [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
         integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
         for specific needs.
         
         
         # History
         
-        ## 0.4.1 - 2023-05-02
-        
-        This release adds support for Pandas 2.0 and PyTorch 2.0!
-        
-        ### Maintenance
-        
-        * Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by @frances-h
-        * Upgrade to Torch 2.0 - Issue [#70](https://github.com/sdv-dev/DeepEcho/issues/70) by @frances-h
-        
         ## 0.4.0 - 2023-01-10
         
         This release adds support for python 3.10 and 3.11. It also drops support for python 3.6.
         
         ### Maintenance
         
         * Support Python 3.10 and 3.11 - Issue [#63](https://github.com/sdv-dev/DeepEcho/issues/63) by @pvk-developer
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepecho Version: 0.4.1 Summary: Create sequential
-synthetic data of mixed types using a GAN. Home-page: https://github.com/sdv-
-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
-Description:
+Metadata-Version: 2.1 Name: deepecho Version: 0.4.1.dev0 Summary: Create
+sequential synthetic data of mixed types using a GAN. Home-page: https://
+github.com/sdv-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev
+License: BSL-1.1 Description:
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/deepecho.svg)](https:
 //pypi.python.org/pypi/deepecho) [![Tests](https://github.com/sdv-dev/DeepEcho/
@@ -97,19 +97,15 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 0.4.1 - 2023-05-02 This release adds
-support for Pandas 2.0 and PyTorch 2.0! ### Maintenance * Remove upper bound
-for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by
-@frances-h * Upgrade to Torch 2.0 - Issue [#70](https://github.com/sdv-dev/
-DeepEcho/issues/70) by @frances-h ## 0.4.0 - 2023-01-10 This release adds
+libraries for specific needs. # History ## 0.4.0 - 2023-01-10 This release adds
 support for python 3.10 and 3.11. It also drops support for python 3.6. ###
 Maintenance * Support Python 3.10 and 3.11 - Issue [#63](https://github.com/
 sdv-dev/DeepEcho/issues/63) by @pvk-developer * DeepEcho Package Maintenance
 Updates - Issue [#62](https://github.com/sdv-dev/DeepEcho/issues/62) by @pvk-
 developer ## 0.3.0 - 2021-11-15 This release adds support for Python 3.9 and
 updates dependencies to ensure compatibility with the rest of the SDV
 ecosystem. * Add support for Python 3.9 - Issue [#41](https://github.com/sdv-
```

### Comparing `deepecho-0.4.1/README.md` & `deepecho-0.4.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/deepecho/data/demo.csv` & `deepecho-0.4.1.dev0/deepecho/data/demo.csv`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/deepecho/models/base.py` & `deepecho-0.4.1.dev0/deepecho/models/base.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/deepecho/models/basic_gan.py` & `deepecho-0.4.1.dev0/deepecho/models/basic_gan.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/deepecho/models/par.py` & `deepecho-0.4.1.dev0/deepecho/models/par.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/deepecho/sequences.py` & `deepecho-0.4.1.dev0/deepecho/sequences.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/deepecho.egg-info/PKG-INFO` & `deepecho-0.4.1.dev0/deepecho.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepecho
-Version: 0.4.1
+Version: 0.4.1.dev0
 Summary: Create sequential synthetic data of mixed types using a GAN.
 Home-page: https://github.com/sdv-dev/DeepEcho
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Description: <div align="center">
         <br/>
@@ -189,23 +189,14 @@
         [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
         integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
         for specific needs.
         
         
         # History
         
-        ## 0.4.1 - 2023-05-02
-        
-        This release adds support for Pandas 2.0 and PyTorch 2.0!
-        
-        ### Maintenance
-        
-        * Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by @frances-h
-        * Upgrade to Torch 2.0 - Issue [#70](https://github.com/sdv-dev/DeepEcho/issues/70) by @frances-h
-        
         ## 0.4.0 - 2023-01-10
         
         This release adds support for python 3.10 and 3.11. It also drops support for python 3.6.
         
         ### Maintenance
         
         * Support Python 3.10 and 3.11 - Issue [#63](https://github.com/sdv-dev/DeepEcho/issues/63) by @pvk-developer
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepecho Version: 0.4.1 Summary: Create sequential
-synthetic data of mixed types using a GAN. Home-page: https://github.com/sdv-
-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
-Description:
+Metadata-Version: 2.1 Name: deepecho Version: 0.4.1.dev0 Summary: Create
+sequential synthetic data of mixed types using a GAN. Home-page: https://
+github.com/sdv-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev
+License: BSL-1.1 Description:
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/deepecho.svg)](https:
 //pypi.python.org/pypi/deepecho) [![Tests](https://github.com/sdv-dev/DeepEcho/
@@ -97,19 +97,15 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 0.4.1 - 2023-05-02 This release adds
-support for Pandas 2.0 and PyTorch 2.0! ### Maintenance * Remove upper bound
-for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by
-@frances-h * Upgrade to Torch 2.0 - Issue [#70](https://github.com/sdv-dev/
-DeepEcho/issues/70) by @frances-h ## 0.4.0 - 2023-01-10 This release adds
+libraries for specific needs. # History ## 0.4.0 - 2023-01-10 This release adds
 support for python 3.10 and 3.11. It also drops support for python 3.6. ###
 Maintenance * Support Python 3.10 and 3.11 - Issue [#63](https://github.com/
 sdv-dev/DeepEcho/issues/63) by @pvk-developer * DeepEcho Package Maintenance
 Updates - Issue [#62](https://github.com/sdv-dev/DeepEcho/issues/62) by @pvk-
 developer ## 0.3.0 - 2021-11-15 This release adds support for Python 3.9 and
 updates dependencies to ensure compatibility with the rest of the SDV
 ecosystem. * Add support for Python 3.9 - Issue [#41](https://github.com/sdv-
```

### Comparing `deepecho-0.4.1/deepecho.egg-info/SOURCES.txt` & `deepecho-0.4.1.dev0/deepecho.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/deepecho.egg-info/requires.txt` & `deepecho-0.4.1.dev0/deepecho.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/setup.cfg` & `deepecho-0.4.1.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.1
+current_version = 0.4.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `deepecho-0.4.1/setup.py` & `deepecho-0.4.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,10 +106,10 @@
     name='deepecho',
     packages=find_packages(include=['deepecho', 'deepecho.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/DeepEcho',
-    version='0.4.1',
+    version='0.4.1.dev0',
     zip_safe=False,
 )
```

### Comparing `deepecho-0.4.1/tests/integration/test_basic_gan.py` & `deepecho-0.4.1.dev0/tests/integration/test_basic_gan.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/tests/integration/test_par.py` & `deepecho-0.4.1.dev0/tests/integration/test_par.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.1/tests/unit/test_sequences.py` & `deepecho-0.4.1.dev0/tests/unit/test_sequences.py`

 * *Files identical despite different names*

