# Comparing `tmp/robotControl-0.8.tar.gz` & `tmp/robotControl-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotControl-0.8.tar", last modified: Tue May  2 09:57:56 2023, max compression
+gzip compressed data, was "robotControl-0.9.tar", last modified: Tue May  2 09:59:53 2023, max compression
```

## Comparing `robotControl-0.8.tar` & `robotControl-0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:57:56.675153 robotControl-0.8/
--rw-rw-rw-   0        0        0      143 2023-05-02 09:57:56.672284 robotControl-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 09:57:56.639234 robotControl-0.8/robotControl.egg-info/
--rw-rw-rw-   0        0        0      143 2023-05-02 09:57:56.000000 robotControl-0.8/robotControl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-02 09:57:56.000000 robotControl-0.8/robotControl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:57:56.000000 robotControl-0.8/robotControl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 09:57:56.000000 robotControl-0.8/robotControl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 09:57:56.000000 robotControl-0.8/robotControl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 09:57:56.675153 robotControl-0.8/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-05-02 09:56:59.000000 robotControl-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:57:56.663685 robotControl-0.8/src/
--rw-rw-rw-   0        0        0    12942 2023-05-02 09:57:42.000000 robotControl-0.8/src/main.cpp
+drwxrwxrwx   0        0        0        0 2023-05-02 09:59:53.829723 robotControl-0.9/
+-rw-rw-rw-   0        0        0      143 2023-05-02 09:59:53.829723 robotControl-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 09:59:53.821581 robotControl-0.9/robotControl.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-05-02 09:59:53.000000 robotControl-0.9/robotControl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-02 09:59:53.000000 robotControl-0.9/robotControl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:59:53.000000 robotControl-0.9/robotControl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 09:59:53.000000 robotControl-0.9/robotControl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 09:59:53.000000 robotControl-0.9/robotControl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:59:53.829723 robotControl-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-05-02 09:59:29.000000 robotControl-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:59:53.829723 robotControl-0.9/src/
+-rw-rw-rw-   0        0        0    13227 2023-05-02 09:59:25.000000 robotControl-0.9/src/main.cpp
```

### Comparing `robotControl-0.8/setup.py` & `robotControl-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib']
 ),]
 
 
 setuptools.setup(
     name='robotControl',
     install_requires=['pybind11'],
-    version=0.8,
+    version=0.9,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=jaco_module,
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `robotControl-0.8/src/main.cpp` & `robotControl-0.9/src/main.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
  * Headerfile for jaco2 SDK bindings
  * Created on: Apr 12, 2023
  * Author: Daniel Dharampal
  */ 
 
 #include "C:\Users\amy_m\OneDrive\Dokumenter\Carl - UNI\Semester 2\Projekt\Communication_robot\Build\lib\KinovaTypes.h"
 #include <iostream>
-#include "pybind11/pybind11.h"
+#include "C:\Users\amy_m\OneDrive\Dokumenter\Carl - UNI\Semester 2\Projekt\Communication_robot\Build\src\pybind11\pybind11.h"
 #ifdef __linux__ 
 #include <dlfcn.h>
 #include <vector>
 #include "Kinova.API.CommLayerUbuntu.h"
 #include "Kinova.API.UsbCommandLayerUbuntu.h"
 #include <stdio.h>
 #include <unistd.h>
 #elif _WIN32
 #include <Windows.h>
-#include "CommunicationLayer.h"
-#include "CommandLayer.h"
+#include "C:\Users\amy_m\OneDrive\Dokumenter\Carl - UNI\Semester 2\Projekt\Communication_robot\Build\lib\CommunicationLayer.h"
+#include "C:\Users\amy_m\OneDrive\Dokumenter\Carl - UNI\Semester 2\Projekt\Communication_robot\Build\lib\CommandLayer.h"
 #include <conio.h>
 #include <iostream>
 #endif
 
 using namespace std;
 
 //A handle to the API.
```

