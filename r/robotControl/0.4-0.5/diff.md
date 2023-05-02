# Comparing `tmp/robotControl-0.4.tar.gz` & `tmp/robotControl-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotControl-0.4.tar", last modified: Tue May  2 09:42:02 2023, max compression
+gzip compressed data, was "robotControl-0.5.tar", last modified: Tue May  2 09:47:19 2023, max compression
```

## Comparing `robotControl-0.4.tar` & `robotControl-0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:42:02.364348 robotControl-0.4/
--rw-rw-rw-   0        0        0      143 2023-05-02 09:42:02.364348 robotControl-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 09:42:02.344854 robotControl-0.4/robotControl.egg-info/
--rw-rw-rw-   0        0        0      143 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 09:42:02.000000 robotControl-0.4/robotControl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 09:42:02.364348 robotControl-0.4/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-05-02 09:41:42.000000 robotControl-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:42:02.361367 robotControl-0.4/src/
--rw-rw-rw-   0        0        0    12847 2023-05-02 09:41:41.000000 robotControl-0.4/src/main.cpp
+drwxrwxrwx   0        0        0        0 2023-05-02 09:47:19.783111 robotControl-0.5/
+-rw-rw-rw-   0        0        0      143 2023-05-02 09:47:19.783111 robotControl-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 09:47:19.774735 robotControl-0.5/robotControl.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-05-02 09:47:19.000000 robotControl-0.5/robotControl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-02 09:47:19.000000 robotControl-0.5/robotControl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:47:19.000000 robotControl-0.5/robotControl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 09:47:19.000000 robotControl-0.5/robotControl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 09:47:19.000000 robotControl-0.5/robotControl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:47:19.783111 robotControl-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-05-02 09:46:44.000000 robotControl-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:47:19.783111 robotControl-0.5/src/
+-rw-rw-rw-   0        0        0    12847 2023-05-02 09:41:41.000000 robotControl-0.5/src/main.cpp
```

### Comparing `robotControl-0.4/setup.py` & `robotControl-0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     extra_link_args=['-Wl,-rpath,$ORIGIN/../lib']
 ),]
 
 
 setuptools.setup(
     name='robotControl',
     install_requires=['pybind11'],
-    version=0.4,
+    version=0.5,
     author='Daniel Dharampal',
     description='A binding of simple jaco2 SDK commands for python',
     ext_modules=jaco_module,
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `robotControl-0.4/src/main.cpp` & `robotControl-0.5/src/main.cpp`

 * *Files identical despite different names*

