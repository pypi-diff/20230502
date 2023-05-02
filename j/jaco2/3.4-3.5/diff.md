# Comparing `tmp/jaco2-3.4.tar.gz` & `tmp/jaco2-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-3.4.tar", last modified: Tue May  2 21:01:10 2023, max compression
+gzip compressed data, was "jaco2-3.5.tar", last modified: Tue May  2 21:45:42 2023, max compression
```

## Comparing `jaco2-3.4.tar` & `jaco2-3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:01:10.294807 jaco2-3.4/
--rw-rw-rw-   0        0        0      136 2023-05-02 21:01:10.294807 jaco2-3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 21:01:10.256688 jaco2-3.4/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 21:01:10.000000 jaco2-3.4/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-02 21:01:10.000000 jaco2-3.4/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:01:10.000000 jaco2-3.4/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 21:01:10.000000 jaco2-3.4/jaco2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 21:01:10.294807 jaco2-3.4/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-05-02 21:01:01.000000 jaco2-3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:01:10.294807 jaco2-3.4/src/
--rw-rw-rw-   0        0        0   852480 2023-05-02 18:07:32.000000 jaco2-3.4/src/CommandLayerEthernet.dll
--rw-rw-rw-   0        0        0   964096 2023-05-02 18:07:32.000000 jaco2-3.4/src/CommandLayerWindows.dll
--rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.4/src/CommunicationLayerEthernet.dll
--rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.4/src/CommunicationLayerWindows.dll
--rw-rw-rw-   0        0        0    13614 2023-05-02 21:01:05.000000 jaco2-3.4/src/jaco2.cpp
+drwxrwxrwx   0        0        0        0 2023-05-02 21:45:42.541096 jaco2-3.5/
+-rw-rw-rw-   0        0        0      136 2023-05-02 21:45:42.541096 jaco2-3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 21:45:42.516781 jaco2-3.5/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 21:45:42.000000 jaco2-3.5/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-02 21:45:42.000000 jaco2-3.5/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:45:42.000000 jaco2-3.5/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 21:45:42.000000 jaco2-3.5/jaco2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:45:42.541096 jaco2-3.5/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-05-02 21:45:30.000000 jaco2-3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:45:42.541096 jaco2-3.5/src/
+-rw-rw-rw-   0        0        0   852480 2023-05-02 18:07:32.000000 jaco2-3.5/src/CommandLayerEthernet.dll
+-rw-rw-rw-   0        0        0   964096 2023-05-02 18:07:32.000000 jaco2-3.5/src/CommandLayerWindows.dll
+-rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.5/src/CommunicationLayerEthernet.dll
+-rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.5/src/CommunicationLayerWindows.dll
+-rw-rw-rw-   0        0        0    13799 2023-05-02 21:45:21.000000 jaco2-3.5/src/jaco2.cpp
```

### Comparing `jaco2-3.4/setup.py` & `jaco2-3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 from setuptools import setup
 import glob
 
 jaco_module = Pybind11Extension(
     'jaco2',
     [str(fname) for fname in Path('src').glob('*.cpp')],
     include_dirs=['.'],
-    library_dirs=['src'],
     extra_compile_args=['/Ox'],
 )
 
 setup(
     name='jaco2',
-    version=3.4,
+    version=3.5,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
     data_files=[("dll_lib", ['src/CommandLayerEthernet.dll', 'src/CommandLayerWindows.dll', 'src/CommunicationLayerEthernet.dll', 'src/CommunicationLayerWindows.dll'])],
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `jaco2-3.4/src/CommandLayerEthernet.dll` & `jaco2-3.5/src/CommandLayerEthernet.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.4/src/CommandLayerWindows.dll` & `jaco2-3.5/src/CommandLayerWindows.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.4/src/CommunicationLayerEthernet.dll` & `jaco2-3.5/src/CommunicationLayerEthernet.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.4/src/CommunicationLayerWindows.dll` & `jaco2-3.5/src/CommunicationLayerWindows.dll`

 * *Files identical despite different names*

### Comparing `jaco2-3.4/src/jaco2.cpp` & `jaco2-3.5/src/jaco2.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -65,26 +65,32 @@
 	setActiveDevice = (int (*)(KinovaDevice devices)) dlsym(commandLayer_handle,"SetActiveDevice");
     getGeneralInformations = (int (*)(GeneralInformations &info)) dlsym(commandLayer_handle,"GetGeneralInformations");
 	#elif _WIN32
 	//We load the API.
 	/*std::filesystem::path this_file_path(__FILE__);
     std::filesystem::path this_file_dir = this_file_path.parent_path();
     std::filesystem::path dll_path = this_file_dir / "CommandLayerWindows.dll";
-	std::wstring dll_path_wide = dll_path.wstring();
+	std::wstring dll_path_wide = dll_path.wstring();*/
 
 	// Get the absolute path of the current source file
-    std::string exe_path = __FILE__;
-    exe_path = exe_path.substr(0, exe_path.rfind('\\'));
+    //std::string exe_path = __FILE__;
+    //exe_path = exe_path.substr(0, exe_path.rfind('\\'));
 
     // Construct the path to the DLL file
-    std::string dll_name = "my_dll.dll";
-    std::string dll_path = exe_path + "\\" + dll_name;
-	commandLayer_handle = LoadLibraryW(std::wstring(dll_path.begin(), dll_path.end()).c_str());*/
+    //std::string dll_name = "CommandLayerWindows.dll";
+    //std::string dll_path = exe_path + "\\" + dll_name;
+	//commandLayer_handle = LoadLibraryW(std::wstring(dll_path.begin(), dll_path.end()).c_str());
+
+
+	// Construct the path to the DLL file
+	std::filesystem::path dll_path = std::filesystem::path("jaco2-3.5.data") / "data" / "dll_lib" / "CommandLayerEthernet.dll";
+	
 	//std::wstring dll_path_wide = L"./example_lib/" + std::wstring("CommandLayerWindows.dll");
-	commandLayer_handle = LoadLibrary("CommandLayerWindows.dll");
+	
+	commandLayer_handle = LoadLibraryW(dll_path.c_str());
 
 	//We load the functions from the library
 	initAPI = (int(*)()) GetProcAddress(commandLayer_handle, "InitAPI");
 	closeAPI = (int(*)()) GetProcAddress(commandLayer_handle, "CloseAPI");
     initFingers = (int(*)()) GetProcAddress(commandLayer_handle, "InitFingers");
 
 	sendBasicTrajectory = (int(*)(TrajectoryPoint)) GetProcAddress(commandLayer_handle, "SendBasicTrajectory");
```

