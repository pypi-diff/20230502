# Comparing `tmp/robotControl-0.3.tar.gz` & `tmp/robotControl-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotControl-0.3.tar", last modified: Tue May  2 09:31:39 2023, max compression
+gzip compressed data, was "robotControl-0.4.tar", last modified: Tue May  2 09:42:02 2023, max compression
```

## Comparing `robotControl-0.3.tar` & `robotControl-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:31:39.809144 robotControl-0.3/
--rw-rw-rw-   0        0        0      143 2023-05-02 09:31:39.809144 robotControl-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 09:31:39.809144 robotControl-0.3/robotControl.egg-info/
--rw-rw-rw-   0        0        0      143 2023-05-02 09:31:39.000000 robotControl-0.3/robotControl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-02 09:31:39.000000 robotControl-0.3/robotControl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:31:39.000000 robotControl-0.3/robotControl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 09:31:39.000000 robotControl-0.3/robotControl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 09:31:39.000000 robotControl-0.3/robotControl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 09:31:39.809144 robotControl-0.3/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-05-02 09:30:53.000000 robotControl-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:31:39.809144 robotControl-0.3/src/
--rw-rw-rw-   0        0        0    12847 2023-05-02 07:53:35.000000 robotControl-0.3/src/jaco2.cpp
+drwxrwxrwx   0        0        0        0 2023-05-02 09:42:02.364348 robotControl-0.4/
+-rw-rw-rw-   0        0        0      143 2023-05-02 09:42:02.364348 robotControl-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 09:42:02.344854 robotControl-0.4/robotControl.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:42:02.364348 robotControl-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-05-02 09:41:42.000000 robotControl-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:42:02.361367 robotControl-0.4/src/
+-rw-rw-rw-   0        0        0    12847 2023-05-02 09:41:41.000000 robotControl-0.4/src/main.cpp
```

### Comparing `robotControl-0.3/setup.py` & `robotControl-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from pathlib import Path
-
+import setuptools
 from pybind11.setup_helpers import Pybind11Extension, build_ext
-from setuptools import setup
 
-jaco_module = Pybind11Extension(
+jaco_module = [Pybind11Extension(
     'robotControl',
-    [str(fname) for fname in Path('src').glob('*.cpp')],
+    sources=["src/main.cpp"],
     include_dirs=['./lib'],
     extra_compile_args=['-O3', '/utf-8'],
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib']
-)
+),]
+
 
-setup(
+setuptools.setup(
     name='robotControl',
     install_requires=['pybind11'],
-    version=0.3,
+    version=0.4,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
-    ext_modules=[jaco_module],
+    ext_modules=jaco_module,
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `robotControl-0.3/src/jaco2.cpp` & `robotControl-0.4/src/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * Headerfile for jaco2 SDK bindings
  * Created on: Apr 12, 2023
  * Author: Daniel Dharampal
  */ 
 
 #include "KinovaTypes.h"
 #include <iostream>
-#include "pybind11/pybind11.h"
+#include <pybind11/pybind11.h>
 #ifdef __linux__ 
 #include <dlfcn.h>
 #include <vector>
 #include "Kinova.API.CommLayerUbuntu.h"
 #include "Kinova.API.UsbCommandLayerUbuntu.h"
 #include <stdio.h>
 #include <unistd.h>
```

