# Comparing `tmp/pycodata-0.7.0.tar.gz` & `tmp/pycodata-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodata-0.7.0.tar", last modified: Fri Apr 28 05:11:50 2023, max compression
+gzip compressed data, was "pycodata-0.7.1.tar", last modified: Tue May  2 16:46:51 2023, max compression
```

## Comparing `pycodata-0.7.0.tar` & `pycodata-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.555708 pycodata-0.7.0/
--rw-r--r--   0 milan      (501) staff       (20)       20 2023-04-22 07:20:52.000000 pycodata-0.7.0/INSTALL.TXT
--rw-r--r--   0 milan      (501) staff       (20)    35823 2023-04-22 07:20:52.000000 pycodata-0.7.0/LICENSE.TXT
--rw-r--r--   0 milan      (501) staff       (20)      195 2023-04-22 07:20:52.000000 pycodata-0.7.0/MANIFEST.in
--rw-r--r--   0 milan      (501) staff       (20)      996 2023-04-28 05:11:50.555056 pycodata-0.7.0/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)      418 2023-04-26 19:43:03.000000 pycodata-0.7.0/README.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.549111 pycodata-0.7.0/pycodata/
--rw-r--r--   0 milan      (501) staff       (20)       97 2023-04-22 07:20:52.000000 pycodata-0.7.0/pycodata/__init__.py
--rw-r--r--   0 milan      (501) staff       (20)    49578 2023-04-22 07:20:52.000000 pycodata-0.7.0/pycodata/codata.h
--rw-r--r--   0 milan      (501) staff       (20)    94969 2023-04-27 23:24:15.000000 pycodata-0.7.0/pycodata/cpycodata.c
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.554226 pycodata-0.7.0/pycodata/tests/
--rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.0/pycodata/tests/__init__.py
--rw-r--r--   0 milan      (501) staff       (20)      365 2023-04-27 23:38:11.000000 pycodata-0.7.0/pycodata/tests/test_lib.py
--rw-r--r--   0 milan      (501) staff       (20)      555 2023-04-28 04:56:46.000000 pycodata-0.7.0/pycodata/version.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.552641 pycodata-0.7.0/pycodata.egg-info/
--rw-r--r--   0 milan      (501) staff       (20)      996 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)      369 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/SOURCES.txt
--rw-r--r--   0 milan      (501) staff       (20)        1 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/dependency_links.txt
--rw-r--r--   0 milan      (501) staff       (20)        9 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/top_level.txt
--rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.0/requirements.txt
--rw-r--r--   0 milan      (501) staff       (20)       38 2023-04-28 05:11:50.555909 pycodata-0.7.0/setup.cfg
--rw-r--r--   0 milan      (501) staff       (20)     1562 2023-04-28 05:03:25.000000 pycodata-0.7.0/setup.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.799064 pycodata-0.7.1/
+-rw-r--r--   0 milan      (501) staff       (20)       20 2023-04-22 07:20:52.000000 pycodata-0.7.1/INSTALL.TXT
+-rw-r--r--   0 milan      (501) staff       (20)    35823 2023-04-22 07:20:52.000000 pycodata-0.7.1/LICENSE.TXT
+-rw-r--r--   0 milan      (501) staff       (20)      195 2023-04-22 07:20:52.000000 pycodata-0.7.1/MANIFEST.in
+-rw-r--r--   0 milan      (501) staff       (20)      996 2023-05-02 16:46:51.798020 pycodata-0.7.1/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)      418 2023-04-26 19:43:03.000000 pycodata-0.7.1/README.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.792064 pycodata-0.7.1/pycodata/
+-rw-r--r--   0 milan      (501) staff       (20)       97 2023-04-22 07:20:52.000000 pycodata-0.7.1/pycodata/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)    49602 2023-05-02 16:27:41.000000 pycodata-0.7.1/pycodata/codata.h
+-rw-r--r--   0 milan      (501) staff       (20)    94969 2023-04-27 23:24:15.000000 pycodata-0.7.1/pycodata/cpycodata.c
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.796475 pycodata-0.7.1/pycodata/tests/
+-rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.1/pycodata/tests/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)      365 2023-04-27 23:38:11.000000 pycodata-0.7.1/pycodata/tests/test.py
+-rw-r--r--   0 milan      (501) staff       (20)      555 2023-05-02 16:31:16.000000 pycodata-0.7.1/pycodata/version.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.795218 pycodata-0.7.1/pycodata.egg-info/
+-rw-r--r--   0 milan      (501) staff       (20)      996 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)      365 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/SOURCES.txt
+-rw-r--r--   0 milan      (501) staff       (20)        1 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/dependency_links.txt
+-rw-r--r--   0 milan      (501) staff       (20)        9 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/top_level.txt
+-rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.1/requirements.txt
+-rw-r--r--   0 milan      (501) staff       (20)       38 2023-05-02 16:46:51.799263 pycodata-0.7.1/setup.cfg
+-rw-r--r--   0 milan      (501) staff       (20)     1562 2023-04-28 05:03:25.000000 pycodata-0.7.1/setup.py
```

### Comparing `pycodata-0.7.0/LICENSE.TXT` & `pycodata-0.7.1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `pycodata-0.7.0/PKG-INFO` & `pycodata-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodata
-Version: 0.7.0
+Version: 0.7.1
 Summary: pycodata
 Home-page: https://milanskocic.github.io/codata/index.html
 Download-URL: https://github.com/MilanSkocic/codata
 Author: Milan Skocic
 Author-email: milan.skocic@icloud.com
 Maintainer: Milan Skocic
 Maintainer-email: milan.skocic@icloud.com
```

### Comparing `pycodata-0.7.0/pycodata/codata.h` & `pycodata-0.7.1/pycodata/codata.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 /**
 * @file
 * @brief Codata module - autogenerated.
 */
 
+const int YEAR = 2018;
+
 const double ALPHA_PARTICLE_ELECTRON_MASS_RATIO=7294.29954142e0;/**<   */
 const double U_ALPHA_PARTICLE_ELECTRON_MASS_RATIO=0.00000024e0;/**<   */
 
 const double ALPHA_PARTICLE_MASS=6.6446573357e-27;/**< kg */
 const double U_ALPHA_PARTICLE_MASS=0.0000000020e-27;/**< kg */
 
 const double ALPHA_PARTICLE_MASS_ENERGY_EQUIVALENT=5.9719201914e-10;/**< J */
```

### Comparing `pycodata-0.7.0/pycodata/cpycodata.c` & `pycodata-0.7.1/pycodata/cpycodata.c`

 * *Files identical despite different names*

### Comparing `pycodata-0.7.0/pycodata/version.py` & `pycodata-0.7.1/pycodata/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,14 @@
            '__author_email__',
            '__maintainer__',
            '__maintainer_email__',
            '__copyright__',
            '__license__']
 
 __package_name__ = "pycodata"
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 __author__ = "Milan Skocic"
 __author_email__ = "milan.skocic@icloud.com"
 __maintainer__ = __author__
 __maintainer_email__ = __author_email__
 __copyright__ = 'Copyright (C) 2023 ' + __author__
 __license__ = 'GNU General Public License v3 (GPLv3)'
```

### Comparing `pycodata-0.7.0/pycodata.egg-info/PKG-INFO` & `pycodata-0.7.1/pycodata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodata
-Version: 0.7.0
+Version: 0.7.1
 Summary: pycodata
 Home-page: https://milanskocic.github.io/codata/index.html
 Download-URL: https://github.com/MilanSkocic/codata
 Author: Milan Skocic
 Author-email: milan.skocic@icloud.com
 Maintainer: Milan Skocic
 Maintainer-email: milan.skocic@icloud.com
```

### Comparing `pycodata-0.7.0/setup.py` & `pycodata-0.7.1/setup.py`

 * *Files identical despite different names*

