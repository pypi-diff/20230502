# Comparing `tmp/jaco2-2.1.tar.gz` & `tmp/jaco2-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-2.1.tar", last modified: Tue May  2 16:18:43 2023, max compression
+gzip compressed data, was "jaco2-2.2.tar", last modified: Tue May  2 16:23:17 2023, max compression
```

## Comparing `jaco2-2.1.tar` & `jaco2-2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:18:43.087932 jaco2-2.1/
--rw-rw-rw-   0        0        0      136 2023-05-02 16:18:43.086933 jaco2-2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 16:18:43.076445 jaco2-2.1/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 16:18:42.000000 jaco2-2.1/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-05-02 16:18:43.000000 jaco2-2.1/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:18:42.000000 jaco2-2.1/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 16:18:42.000000 jaco2-2.1/jaco2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 16:18:43.085909 jaco2-2.1/robotControl/
--rw-rw-rw-   0        0        0    12847 2023-05-02 16:17:13.000000 jaco2-2.1/robotControl/jaco2.cpp
--rw-rw-rw-   0        0        0       42 2023-05-02 16:18:43.088932 jaco2-2.1/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-05-02 16:07:53.000000 jaco2-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:23:17.200685 jaco2-2.2/
+-rw-rw-rw-   0        0        0      136 2023-05-02 16:23:17.199678 jaco2-2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 16:23:17.197678 jaco2-2.2/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 16:23:17.000000 jaco2-2.2/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-05-02 16:23:17.000000 jaco2-2.2/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:23:17.000000 jaco2-2.2/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 16:23:17.000000 jaco2-2.2/jaco2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 16:23:17.198677 jaco2-2.2/robotControl/
+-rw-rw-rw-   0        0        0    12847 2023-05-02 16:17:13.000000 jaco2-2.2/robotControl/jaco2.cpp
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:23:17.200685 jaco2-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-05-02 16:21:41.000000 jaco2-2.2/setup.py
```

### Comparing `jaco2-2.1/robotControl/jaco2.cpp` & `jaco2-2.2/robotControl/jaco2.cpp`

 * *Files identical despite different names*

### Comparing `jaco2-2.1/setup.py` & `jaco2-2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
 jaco_module = Pybind11Extension(
     'jaco2',
     [str(fname) for fname in Path('robotControl').glob('*.cpp')],
-    include_dirs=['./lib'],
+    include_dirs=['.'],
     extra_compile_args=['/Ox'],
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib']
 )
 
 setup(
     name='jaco2',
-    version=2.1,
+    version=2.2,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
     cmdclass={"build_ext": build_ext},
 )
```

