# Comparing `tmp/overloaded-iterables-0.7.21.tar.gz` & `tmp/overloaded-iterables-0.7.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.21.tar", last modified: Tue May  2 18:56:08 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.23.tar", last modified: Tue May  2 18:58:44 2023, max compression
```

## Comparing `overloaded-iterables-0.7.21.tar` & `overloaded-iterables-0.7.23.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.644570 overloaded-iterables-0.7.21/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.21/LICENSE
--rw-rw-rw-   0        0        0    10025 2023-05-02 18:56:08.646580 overloaded-iterables-0.7.21/PKG-INFO
--rw-rw-rw-   0        0        0    11888 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/README.md
--rw-rw-rw-   0        0        0      116 2023-05-02 18:56:08.651569 overloaded-iterables-0.7.21/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-05-01 08:50:57.000000 overloaded-iterables-0.7.21/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.620570 overloaded-iterables-0.7.21/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.628570 overloaded-iterables-0.7.21/src/overloaded_iterables/
--rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    17403 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/classes.py
--rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/exceptions.py
--rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.21/src/overloaded_iterables/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:56:08.643574 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0    10025 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 18:56:08.000000 overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 18:58:44.432736 overloaded-iterables-0.7.23/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.23/LICENSE
+-rw-rw-rw-   0        0        0    10025 2023-05-02 18:58:44.433736 overloaded-iterables-0.7.23/PKG-INFO
+-rw-rw-rw-   0        0        0    11888 2023-05-02 18:58:12.000000 overloaded-iterables-0.7.23/README.md
+-rw-rw-rw-   0        0        0      116 2023-05-02 18:58:44.440737 overloaded-iterables-0.7.23/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-05-01 08:50:57.000000 overloaded-iterables-0.7.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:58:44.297628 overloaded-iterables-0.7.23/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 18:58:44.304629 overloaded-iterables-0.7.23/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.23/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    17403 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.23/src/overloaded_iterables/classes.py
+-rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.23/src/overloaded_iterables/exceptions.py
+-rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.23/src/overloaded_iterables/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:58:44.428806 overloaded-iterables-0.7.23/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0    10025 2023-05-02 18:58:44.000000 overloaded-iterables-0.7.23/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-02 18:58:44.000000 overloaded-iterables-0.7.23/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:58:44.000000 overloaded-iterables-0.7.23/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 18:58:44.000000 overloaded-iterables-0.7.23/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 18:58:44.000000 overloaded-iterables-0.7.23/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.21/LICENSE` & `overloaded-iterables-0.7.23/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.21/PKG-INFO` & `overloaded-iterables-0.7.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.21
+Version: 0.7.23
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -246,13 +246,13 @@
     - Deletes `num` elements from the beginning of the object in case of `Queue` and from the end of the object in case of `Stack`.
     - Arguments: `self`, `num: int | default: 1`
     - Returns: `None` _(is an in-place method)_
     - Example:
 
         ```python
             queue = Queue(*args)
-            stack = Stavk(*args)
+            stack = Stack(*args)
             queue.pop(num=num)
             stack.pop(num=num)
         ```
```

### Comparing `overloaded-iterables-0.7.21/README.md` & `overloaded-iterables-0.7.23/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     - Deletes `num` elements from the beginning of the object in case of `Queue` and from the end of the object in case of `Stack`.
     - Arguments: `self`, `num: int | default: 1`
     - Returns: `None` _(is an in-place method)_
     - Example:
 
         ```python
             queue = Queue(*args)
-            stack = Stavk(*args)
+            stack = Stack(*args)
             queue.pop(num=num)
             stack.pop(num=num)
         ```
 
 ## Development Setup
 
 1. `git clone https://<personal-access-token>@github.com/Arkiralor/overloaded_iterables.git`
```

### Comparing `overloaded-iterables-0.7.21/setup.py` & `overloaded-iterables-0.7.23/setup.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.21/src/overloaded_iterables/__init__.py` & `overloaded-iterables-0.7.23/src/overloaded_iterables/__init__.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.21/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.23/src/overloaded_iterables/classes.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.21/src/overloaded_iterables/exceptions.py` & `overloaded-iterables-0.7.23/src/overloaded_iterables/exceptions.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.21/src/overloaded_iterables/utils.py` & `overloaded-iterables-0.7.23/src/overloaded_iterables/utils.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.21/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.7.23/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.21
+Version: 0.7.23
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -246,13 +246,13 @@
     - Deletes `num` elements from the beginning of the object in case of `Queue` and from the end of the object in case of `Stack`.
     - Arguments: `self`, `num: int | default: 1`
     - Returns: `None` _(is an in-place method)_
     - Example:
 
         ```python
             queue = Queue(*args)
-            stack = Stavk(*args)
+            stack = Stack(*args)
             queue.pop(num=num)
             stack.pop(num=num)
         ```
```

