# Comparing `tmp/overloaded-iterables-0.7.27.tar.gz` & `tmp/overloaded-iterables-0.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.27.tar", last modified: Tue May  2 19:12:27 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.30.tar", last modified: Tue May  2 19:21:35 2023, max compression
```

## Comparing `overloaded-iterables-0.7.27.tar` & `overloaded-iterables-0.7.30.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.076313 overloaded-iterables-0.7.27/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.27/LICENSE
--rw-rw-rw-   0        0        0    12615 2023-05-02 19:12:27.079328 overloaded-iterables-0.7.27/PKG-INFO
--rw-rw-rw-   0        0        0    11888 2023-05-02 18:58:12.000000 overloaded-iterables-0.7.27/README.md
--rw-rw-rw-   0        0        0      111 2023-05-02 19:12:27.081310 overloaded-iterables-0.7.27/setup.cfg
--rw-rw-rw-   0        0        0     1645 2023-05-02 19:12:09.000000 overloaded-iterables-0.7.27/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.052312 overloaded-iterables-0.7.27/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.059310 overloaded-iterables-0.7.27/src/overloaded_iterables/
--rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    17403 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/classes.py
--rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/exceptions.py
--rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.075312 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0    12615 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-05-02 19:12:27.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 19:21:35.978100 overloaded-iterables-0.7.30/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.30/LICENSE
+-rw-rw-rw-   0        0        0    12615 2023-05-02 19:21:35.979037 overloaded-iterables-0.7.30/PKG-INFO
+-rw-rw-rw-   0        0        0    11888 2023-05-02 18:58:12.000000 overloaded-iterables-0.7.30/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-02 19:21:35.986039 overloaded-iterables-0.7.30/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-05-02 19:21:30.000000 overloaded-iterables-0.7.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:21:35.941054 overloaded-iterables-0.7.30/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:21:35.957037 overloaded-iterables-0.7.30/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.30/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    17349 2023-05-02 19:21:03.000000 overloaded-iterables-0.7.30/src/overloaded_iterables/classes.py
+-rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.30/src/overloaded_iterables/exceptions.py
+-rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.30/src/overloaded_iterables/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:21:35.977033 overloaded-iterables-0.7.30/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0    12615 2023-05-02 19:21:35.000000 overloaded-iterables-0.7.30/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-02 19:21:35.000000 overloaded-iterables-0.7.30/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:21:35.000000 overloaded-iterables-0.7.30/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 19:21:35.000000 overloaded-iterables-0.7.30/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 19:21:35.000000 overloaded-iterables-0.7.30/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.27/LICENSE` & `overloaded-iterables-0.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.27/PKG-INFO` & `overloaded-iterables-0.7.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.27
+Version: 0.7.30
 Summary: Overloaded version of the built-in python classes: list and set, to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot,queue,stack
 Platform: windows
```

### Comparing `overloaded-iterables-0.7.27/README.md` & `overloaded-iterables-0.7.30/README.md`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.27/setup.py` & `overloaded-iterables-0.7.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         encoding="utf-8"
     )as file_obj:
         data = file_obj.read()
     return data
 
 setup(
     name='overloaded-iterables',
-    version='0.7.27',
+    version='0.7.30',
     description='Overloaded version of the built-in python classes: list and set, to include some extra functionalities.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     license='MIT',
     author='Prithoo Medhi',
     author_email='prithoo11335@gmail.com',
     packages=find_packages(where='src'),
```

### Comparing `overloaded-iterables-0.7.27/src/overloaded_iterables/__init__.py` & `overloaded-iterables-0.7.30/src/overloaded_iterables/__init__.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.27/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.30/src/overloaded_iterables/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,14 @@
         """
         Insert a single or sequence of values to the end of the Stack object.
         """
         type_check = (type(value) == list or type(value) == set or type(value) == OverloadedList or type(value) == OverloadedSet or type(value) == tuple)
         if value is not None and not type_check:
             self.append(value)
         elif value is not None and type_check:
-            print(f"extending {value} to the stack")
             self.extend(value)
 
     def pop(self, num:int=1):
         """
         Remove the latest `num: int | default: 1` elements from the top (highest index) of the stack
         """
         if num > self.len:
```

### Comparing `overloaded-iterables-0.7.27/src/overloaded_iterables/exceptions.py` & `overloaded-iterables-0.7.30/src/overloaded_iterables/exceptions.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.27/src/overloaded_iterables/utils.py` & `overloaded-iterables-0.7.30/src/overloaded_iterables/utils.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.7.30/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.27
+Version: 0.7.30
 Summary: Overloaded version of the built-in python classes: list and set, to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot,queue,stack
 Platform: windows
```

