# Comparing `tmp/jaco2-2.6.tar.gz` & `tmp/jaco2-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-2.6.tar", last modified: Tue May  2 17:19:42 2023, max compression
+gzip compressed data, was "jaco2-2.7.tar", last modified: Tue May  2 17:21:58 2023, max compression
```

## Comparing `jaco2-2.6.tar` & `jaco2-2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:19:42.794556 jaco2-2.6/
--rw-rw-rw-   0        0        0      136 2023-05-02 17:19:42.791818 jaco2-2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 17:19:42.790684 jaco2-2.6/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 17:19:42.000000 jaco2-2.6/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-05-02 17:19:42.000000 jaco2-2.6/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:19:42.000000 jaco2-2.6/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 17:19:42.000000 jaco2-2.6/jaco2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 17:19:42.791818 jaco2-2.6/robotControl/
--rw-rw-rw-   0        0        0    12847 2023-05-02 17:16:14.000000 jaco2-2.6/robotControl/jaco2.cpp
--rw-rw-rw-   0        0        0       42 2023-05-02 17:19:42.794556 jaco2-2.6/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-05-02 17:19:30.000000 jaco2-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:21:58.094807 jaco2-2.7/
+-rw-rw-rw-   0        0        0      136 2023-05-02 17:21:58.090290 jaco2-2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 17:21:58.085892 jaco2-2.7/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 17:21:57.000000 jaco2-2.7/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-05-02 17:21:57.000000 jaco2-2.7/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:21:57.000000 jaco2-2.7/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 17:21:57.000000 jaco2-2.7/jaco2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:21:58.090290 jaco2-2.7/robotControl/
+-rw-rw-rw-   0        0        0    12847 2023-05-02 17:16:14.000000 jaco2-2.7/robotControl/jaco2.cpp
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:21:58.094807 jaco2-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-05-02 17:21:45.000000 jaco2-2.7/setup.py
```

### Comparing `jaco2-2.6/robotControl/jaco2.cpp` & `jaco2-2.7/robotControl/jaco2.cpp`

 * *Files identical despite different names*

### Comparing `jaco2-2.6/setup.py` & `jaco2-2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jaco_module = Pybind11Extension(
     'jaco2',
     [str(fname) for fname in Path('robotControl').glob('*.cpp')],
     include_dirs=['.'],
     extra_compile_args=['/Ox'],
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib'],
-    data_files=[('', ['CommandLayerEthernet.dll', 'CommandLayerWindows.dll', 'CommunicationLayerEthernet.dll', 'CommunicationLayerWindows.dll'])],
+    data_files=[('.', ['CommandLayerEthernet.dll', 'CommandLayerWindows.dll', 'CommunicationLayerEthernet.dll', 'CommunicationLayerWindows.dll'])],
 )
 
 setup(
     name='jaco2',
-    version=2.6,
+    version=2.7,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
     cmdclass={"build_ext": build_ext},
 )
```

