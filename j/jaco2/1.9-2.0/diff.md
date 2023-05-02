# Comparing `tmp/jaco2-1.9.tar.gz` & `tmp/jaco2-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-1.9.tar", last modified: Tue May  2 15:32:40 2023, max compression
+gzip compressed data, was "jaco2-2.0.tar", last modified: Tue May  2 15:44:52 2023, max compression
```

## Comparing `jaco2-1.9.tar` & `jaco2-2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 15:32:40.605983 jaco2-1.9/
--rw-rw-rw-   0        0        0      136 2023-05-02 15:32:40.604965 jaco2-1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 15:32:40.603926 jaco2-1.9/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 15:32:40.000000 jaco2-1.9/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-05-02 15:32:40.000000 jaco2-1.9/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 15:32:40.000000 jaco2-1.9/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 15:32:40.000000 jaco2-1.9/jaco2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 15:32:40.605983 jaco2-1.9/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-05-02 15:32:26.000000 jaco2-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:44:52.088825 jaco2-2.0/
+-rw-rw-rw-   0        0        0      136 2023-05-02 15:44:52.087748 jaco2-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 15:44:52.077746 jaco2-2.0/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 15:44:51.000000 jaco2-2.0/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-05-02 15:44:52.000000 jaco2-2.0/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 15:44:51.000000 jaco2-2.0/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 15:44:51.000000 jaco2-2.0/jaco2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 15:44:52.085849 jaco2-2.0/robotControl/
+-rw-rw-rw-   0        0        0    12846 2023-05-02 15:22:11.000000 jaco2-2.0/robotControl/jaco2.cpp
+-rw-rw-rw-   0        0        0       42 2023-05-02 15:44:52.089749 jaco2-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      587 2023-05-02 15:44:30.000000 jaco2-2.0/setup.py
```

### Comparing `jaco2-1.9/setup.py` & `jaco2-2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
 jaco_module = Pybind11Extension(
     'jaco2',
-    [str(fname) for fname in Path('src').glob('*.cpp')],
+    [str(fname) for fname in Path('robotControl').glob('*.cpp')],
     include_dirs=['./lib'],
-    extra_compile_args=['-O3', 'utf8'],
+    extra_compile_args=['/std:c++11', '/MT', '/arch:amd64'],
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib']
 )
 
 setup(
     name='jaco2',
-    version=1.9,
+    version=2.0,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
     cmdclass={"build_ext": build_ext},
 )
```

