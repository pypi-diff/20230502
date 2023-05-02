# Comparing `tmp/jaco2-2.3.tar.gz` & `tmp/jaco2-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-2.3.tar", last modified: Tue May  2 16:55:25 2023, max compression
+gzip compressed data, was "jaco2-2.4.tar", last modified: Tue May  2 16:58:44 2023, max compression
```

## Comparing `jaco2-2.3.tar` & `jaco2-2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:55:25.222656 jaco2-2.3/
--rw-rw-rw-   0        0        0      136 2023-05-02 16:55:25.222656 jaco2-2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 16:55:25.220833 jaco2-2.3/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 16:55:25.000000 jaco2-2.3/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-05-02 16:55:25.000000 jaco2-2.3/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:55:25.000000 jaco2-2.3/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 16:55:25.000000 jaco2-2.3/jaco2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 16:55:25.222656 jaco2-2.3/robotControl/
--rw-rw-rw-   0        0        0    12847 2023-05-02 16:17:13.000000 jaco2-2.3/robotControl/jaco2.cpp
--rw-rw-rw-   0        0        0       42 2023-05-02 16:55:25.222656 jaco2-2.3/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-05-02 16:55:21.000000 jaco2-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:58:44.150691 jaco2-2.4/
+-rw-rw-rw-   0        0        0      136 2023-05-02 16:58:44.142694 jaco2-2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 16:58:44.142694 jaco2-2.4/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 16:58:44.142694 jaco2-2.4/robotControl/
+-rw-rw-rw-   0        0        0    12847 2023-05-02 16:17:13.000000 jaco2-2.4/robotControl/jaco2.cpp
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:58:44.150691 jaco2-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-05-02 16:58:38.000000 jaco2-2.4/setup.py
```

### Comparing `jaco2-2.3/robotControl/jaco2.cpp` & `jaco2-2.4/robotControl/jaco2.cpp`

 * *Files identical despite different names*

### Comparing `jaco2-2.3/setup.py` & `jaco2-2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,14 @@
     include_dirs=['.'],
     extra_compile_args=['/Ox'],
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib']
 )
 
 setup(
     name='jaco2',
-    version=2.3,
+    version=2.4,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=[jaco_module],
-    data_files=['*.dll'],
+    data_files=[('jaco2', glob.glob('my_package/*.dll'))],
     cmdclass={"build_ext": build_ext},
 )
```

