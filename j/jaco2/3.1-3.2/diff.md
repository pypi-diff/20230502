# Comparing `tmp/jaco2-3.1.tar.gz` & `tmp/jaco2-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-3.1.tar", last modified: Tue May  2 18:32:27 2023, max compression
+gzip compressed data, was "jaco2-3.2.tar", last modified: Tue May  2 20:04:57 2023, max compression
```

## Comparing `jaco2-3.1.tar` & `jaco2-3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:32:27.290121 jaco2-3.1/
--rw-rw-rw-   0        0        0      136 2023-05-02 18:32:27.289535 jaco2-3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 18:32:27.267240 jaco2-3.1/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 18:32:27.290989 jaco2-3.1/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-05-02 18:32:14.000000 jaco2-3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:32:27.286526 jaco2-3.1/src/
--rw-rw-rw-   0        0        0   852480 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommandLayerEthernet.dll
--rw-rw-rw-   0        0        0   964096 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommandLayerWindows.dll
--rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommunicationLayerEthernet.dll
--rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommunicationLayerWindows.dll
--rw-rw-rw-   0        0        0    12861 2023-05-02 18:23:10.000000 jaco2-3.1/src/jaco2.cpp
+drwxrwxrwx   0        0        0        0 2023-05-02 20:04:57.398688 jaco2-3.2/
+-rw-rw-rw-   0        0        0      136 2023-05-02 20:04:57.398688 jaco2-3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 20:04:57.383148 jaco2-3.2/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 20:04:57.000000 jaco2-3.2/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-02 20:04:57.000000 jaco2-3.2/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 20:04:57.000000 jaco2-3.2/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 20:04:57.000000 jaco2-3.2/jaco2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 20:04:57.398688 jaco2-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-05-02 19:04:00.000000 jaco2-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:04:57.398688 jaco2-3.2/src/
+-rw-rw-rw-   0        0        0   852480 2023-05-02 18:07:32.000000 jaco2-3.2/src/CommandLayerEthernet.dll
+-rw-rw-rw-   0        0        0   964096 2023-05-02 18:07:32.000000 jaco2-3.2/src/CommandLayerWindows.dll
+-rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.2/src/CommunicationLayerEthernet.dll
+-rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.2/src/CommunicationLayerWindows.dll
+-rw-rw-rw-   0        0        0    13190 2023-05-02 20:04:44.000000 jaco2-3.2/src/jaco2.cpp
```

### Comparing `jaco2-3.1/setup.py` & `jaco2-3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     [str(fname) for fname in Path('src').glob('*.cpp')],
     include_dirs=['.'],
     extra_compile_args=['/Ox'],
 )
 
 setup(
     name='jaco2',
-    version=3.1,
+    version=3.2,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
     data_files=['src/CommandLayerEthernet.dll', 'src/CommandLayerWindows.dll', 'src/CommunicationLayerEthernet.dll', 'src/CommunicationLayerWindows.dll'],
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `jaco2-3.1/src/CommandLayerEthernet.dll` & `jaco2-3.2/src/CommandLayerEthernet.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.1/src/CommandLayerWindows.dll` & `jaco2-3.2/src/CommandLayerWindows.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.1/src/CommunicationLayerEthernet.dll` & `jaco2-3.2/src/CommunicationLayerEthernet.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.1/src/CommunicationLayerWindows.dll` & `jaco2-3.2/src/CommunicationLayerWindows.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.1/src/jaco2.cpp` & `jaco2-3.2/src/jaco2.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #include <unistd.h>
 #elif _WIN32
 #include <Windows.h>
 #include "CommunicationLayer.h"
 #include "CommandLayer.h"
 #include <conio.h>
 #include <iostream>
+#include <string>
+#include <filesystem>
 #endif
 
 using namespace std;
 
 
 //A handle to the API.
 #ifdef __linux__ 
@@ -60,15 +62,20 @@
 	moveHome = (int (*)()) dlsym(commandLayer_handle,"MoveHome");
 
 	getDevices = (int (*)(KinovaDevice devices[MAX_KINOVA_DEVICE], int &result)) dlsym(commandLayer_handle,"GetDevices");
 	setActiveDevice = (int (*)(KinovaDevice devices)) dlsym(commandLayer_handle,"SetActiveDevice");
     getGeneralInformations = (int (*)(GeneralInformations &info)) dlsym(commandLayer_handle,"GetGeneralInformations");
 	#elif _WIN32
 	//We load the API.
-	commandLayer_handle = LoadLibraryW(L"/LIBPATH:src/CommandLayerWindows.dll");
+	std::filesystem::path this_file_path(__FILE__);
+    std::filesystem::path this_file_dir = this_file_path.parent_path();
+    std::filesystem::path dll_path = this_file_dir / "CommandLayerWindows.dll";
+    std::cout << "DLL path: " << dll_path << std::endl;
+	std::wstring dll_path_wide = dll_path.wstring();
+	commandLayer_handle = LoadLibraryW(dll_path_wide.c_str());
 
 	//We load the functions from the library
 	initAPI = (int(*)()) GetProcAddress(commandLayer_handle, "InitAPI");
 	closeAPI = (int(*)()) GetProcAddress(commandLayer_handle, "CloseAPI");
     initFingers = (int(*)()) GetProcAddress(commandLayer_handle, "InitFingers");
 
 	sendBasicTrajectory = (int(*)(TrajectoryPoint)) GetProcAddress(commandLayer_handle, "SendBasicTrajectory");
```

