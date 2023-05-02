# Comparing `tmp/overloaded-iterables-0.7.19.tar.gz` & `tmp/overloaded-iterables-0.7.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.19.tar", last modified: Tue May  2 18:53:44 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.21.tar", last modified: Tue May  2 18:56:08 2023, max compression
```

## Comparing `overloaded-iterables-0.7.19.tar` & `overloaded-iterables-0.7.21.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:53:44.748589 overloaded-iterables-0.7.19/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.19/LICENSE
--rw-rw-rw-   0        0        0    10025 2023-05-02 18:53:44.750588 overloaded-iterables-0.7.19/PKG-INFO
--rw-rw-rw-   0        0        0    11888 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.19/README.md
--rw-rw-rw-   0        0        0      111 2023-05-02 18:53:44.753547 overloaded-iterables-0.7.19/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-05-01 08:50:57.000000 overloaded-iterables-0.7.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:53:44.726549 overloaded-iterables-0.7.19/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 18:53:44.733545 overloaded-iterables-0.7.19/src/overloaded_iterables/
--rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.19/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    17403 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.19/src/overloaded_iterables/classes.py
--rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.19/src/overloaded_iterables/exceptions.py
--rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.19/src/overloaded_iterables/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:53:44.748589 overloaded-iterables-0.7.19/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0    10025 2023-05-02 18:53:44.000000 overloaded-iterables-0.7.19/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-05-02 18:53:44.000000 overloaded-iterables-0.7.19/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:53:44.000000 overloaded-iterables-0.7.19/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 18:53:44.000000 overloaded-iterables-0.7.19/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 18:53:44.000000 overloaded-iterables-0.7.19/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.644570 overloaded-iterables-0.7.21/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.21/LICENSE
+-rw-rw-rw-   0        0        0    10025 2023-05-02 18:56:08.646580 overloaded-iterables-0.7.21/PKG-INFO
+-rw-rw-rw-   0        0        0    11888 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/README.md
+-rw-rw-rw-   0        0        0      116 2023-05-02 18:56:08.651569 overloaded-iterables-0.7.21/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-05-01 08:50:57.000000 overloaded-iterables-0.7.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.620570 overloaded-iterables-0.7.21/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.628570 overloaded-iterables-0.7.21/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    17403 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/classes.py
+-rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/exceptions.py
+-rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.643574 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0    10025 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.19/LICENSE` & `overloaded-iterables-0.7.21/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.19/PKG-INFO` & `overloaded-iterables-0.7.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.19
+Version: 0.7.21
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
```

### Comparing `overloaded-iterables-0.7.19/README.md` & `overloaded-iterables-0.7.21/README.md`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.19/setup.py` & `overloaded-iterables-0.7.21/setup.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.19/src/overloaded_iterables/__init__.py` & `overloaded-iterables-0.7.21/src/overloaded_iterables/__init__.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.19/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.21/src/overloaded_iterables/classes.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.19/src/overloaded_iterables/exceptions.py` & `overloaded-iterables-0.7.21/src/overloaded_iterables/exceptions.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.19/src/overloaded_iterables/utils.py` & `overloaded-iterables-0.7.21/src/overloaded_iterables/utils.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.19/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.19
+Version: 0.7.21
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
```

