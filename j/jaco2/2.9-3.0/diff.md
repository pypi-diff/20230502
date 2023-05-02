# Comparing `tmp/jaco2-2.9.tar.gz` & `tmp/jaco2-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-2.9.tar", last modified: Tue May  2 18:11:56 2023, max compression
+gzip compressed data, was "jaco2-3.0.tar", last modified: Tue May  2 18:23:31 2023, max compression
```

## Comparing `jaco2-2.9.tar` & `jaco2-3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:11:55.997257 jaco2-2.9/
--rw-rw-rw-   0        0        0      136 2023-05-02 18:11:55.997257 jaco2-2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 18:11:55.997257 jaco2-2.9/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 18:11:55.000000 jaco2-2.9/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-05-02 18:11:55.000000 jaco2-2.9/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:11:55.000000 jaco2-2.9/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 18:11:55.000000 jaco2-2.9/jaco2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 18:11:55.997257 jaco2-2.9/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-05-02 18:11:51.000000 jaco2-2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:11:55.997257 jaco2-2.9/src/
--rw-rw-rw-   0        0        0    12847 2023-05-02 17:16:14.000000 jaco2-2.9/src/jaco2.cpp
+drwxrwxrwx   0        0        0        0 2023-05-02 18:23:31.269939 jaco2-3.0/
+-rw-rw-rw-   0        0        0      136 2023-05-02 18:23:31.261974 jaco2-3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 18:23:31.245926 jaco2-3.0/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 18:23:31.269939 jaco2-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-05-02 18:23:16.000000 jaco2-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:23:31.261974 jaco2-3.0/src/
+-rw-rw-rw-   0        0        0    12861 2023-05-02 18:23:10.000000 jaco2-3.0/src/jaco2.cpp
```

### Comparing `jaco2-2.9/setup.py` & `jaco2-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     include_dirs=['.'],
     extra_compile_args=['/Ox'],
     extra_link_args=['/LIBPATH:src/CommandLayerEthernet.dll', '/LIBPATH:src/CommandLayerWindows.dll', '/LIBPATH:src/CommunicationLayerEthernet.dll', '/LIBPATH:src/CommunicationLayerWindows.dll'],
 )
 
 setup(
     name='jaco2',
-    version=2.9,
+    version=3.0,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `jaco2-2.9/src/jaco2.cpp` & `jaco2-3.0/src/jaco2.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #include "CommandLayer.h"
 #include <conio.h>
 #include <iostream>
 #endif
 
 using namespace std;
 
+
 //A handle to the API.
 #ifdef __linux__ 
 void * commandLayer_handle;
 #elif _WIN32
 HINSTANCE commandLayer_handle;
 #endif
 
@@ -59,15 +60,15 @@
 	moveHome = (int (*)()) dlsym(commandLayer_handle,"MoveHome");
 
 	getDevices = (int (*)(KinovaDevice devices[MAX_KINOVA_DEVICE], int &result)) dlsym(commandLayer_handle,"GetDevices");
 	setActiveDevice = (int (*)(KinovaDevice devices)) dlsym(commandLayer_handle,"SetActiveDevice");
     getGeneralInformations = (int (*)(GeneralInformations &info)) dlsym(commandLayer_handle,"GetGeneralInformations");
 	#elif _WIN32
 	//We load the API.
-	commandLayer_handle = LoadLibraryW(L"CommandLayerWindows.dll");
+	commandLayer_handle = LoadLibraryW(L"/LIBPATH:src/CommandLayerWindows.dll");
 
 	//We load the functions from the library
 	initAPI = (int(*)()) GetProcAddress(commandLayer_handle, "InitAPI");
 	closeAPI = (int(*)()) GetProcAddress(commandLayer_handle, "CloseAPI");
     initFingers = (int(*)()) GetProcAddress(commandLayer_handle, "InitFingers");
 
 	sendBasicTrajectory = (int(*)(TrajectoryPoint)) GetProcAddress(commandLayer_handle, "SendBasicTrajectory");
```

