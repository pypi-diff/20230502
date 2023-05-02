# Comparing `tmp/jaco2-2.0.tar.gz` & `tmp/jaco2-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-2.0.tar", last modified: Tue May  2 15:44:52 2023, max compression
+gzip compressed data, was "jaco2-2.1.tar", last modified: Tue May  2 16:18:43 2023, max compression
```

## Comparing `jaco2-2.0.tar` & `jaco2-2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 15:44:52.088825 jaco2-2.0/
--rw-rw-rw-   0        0        0      136 2023-05-02 15:44:52.087748 jaco2-2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 15:44:52.077746 jaco2-2.0/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 15:44:51.000000 jaco2-2.0/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-05-02 15:44:52.000000 jaco2-2.0/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 15:44:51.000000 jaco2-2.0/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 15:44:51.000000 jaco2-2.0/jaco2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 15:44:52.085849 jaco2-2.0/robotControl/
--rw-rw-rw-   0        0        0    12846 2023-05-02 15:22:11.000000 jaco2-2.0/robotControl/jaco2.cpp
--rw-rw-rw-   0        0        0       42 2023-05-02 15:44:52.089749 jaco2-2.0/setup.cfg
--rw-rw-rw-   0        0        0      587 2023-05-02 15:44:30.000000 jaco2-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:18:43.087932 jaco2-2.1/
+-rw-rw-rw-   0        0        0      136 2023-05-02 16:18:43.086933 jaco2-2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 16:18:43.076445 jaco2-2.1/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 16:18:42.000000 jaco2-2.1/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-05-02 16:18:43.000000 jaco2-2.1/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:18:42.000000 jaco2-2.1/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 16:18:42.000000 jaco2-2.1/jaco2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 16:18:43.085909 jaco2-2.1/robotControl/
+-rw-rw-rw-   0        0        0    12847 2023-05-02 16:17:13.000000 jaco2-2.1/robotControl/jaco2.cpp
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:18:43.088932 jaco2-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-05-02 16:07:53.000000 jaco2-2.1/setup.py
```

### Comparing `jaco2-2.0/robotControl/jaco2.cpp` & `jaco2-2.1/robotControl/jaco2.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 	moveHome = (int (*)()) dlsym(commandLayer_handle,"MoveHome");
 
 	getDevices = (int (*)(KinovaDevice devices[MAX_KINOVA_DEVICE], int &result)) dlsym(commandLayer_handle,"GetDevices");
 	setActiveDevice = (int (*)(KinovaDevice devices)) dlsym(commandLayer_handle,"SetActiveDevice");
     getGeneralInformations = (int (*)(GeneralInformations &info)) dlsym(commandLayer_handle,"GetGeneralInformations");
 	#elif _WIN32
 	//We load the API.
-	commandLayer_handle = LoadLibrary(L"CommandLayerWindows.dll");
+	commandLayer_handle = LoadLibraryW(L"CommandLayerWindows.dll");
 
 	//We load the functions from the library
 	initAPI = (int(*)()) GetProcAddress(commandLayer_handle, "InitAPI");
 	closeAPI = (int(*)()) GetProcAddress(commandLayer_handle, "CloseAPI");
     initFingers = (int(*)()) GetProcAddress(commandLayer_handle, "InitFingers");
 
 	sendBasicTrajectory = (int(*)(TrajectoryPoint)) GetProcAddress(commandLayer_handle, "SendBasicTrajectory");
```

### Comparing `jaco2-2.0/setup.py` & `jaco2-2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
 jaco_module = Pybind11Extension(
     'jaco2',
     [str(fname) for fname in Path('robotControl').glob('*.cpp')],
     include_dirs=['./lib'],
-    extra_compile_args=['/std:c++11', '/MT', '/arch:amd64'],
+    extra_compile_args=['/Ox'],
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib']
 )
 
 setup(
     name='jaco2',
-    version=2.0,
+    version=2.1,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
     cmdclass={"build_ext": build_ext},
 )
```

