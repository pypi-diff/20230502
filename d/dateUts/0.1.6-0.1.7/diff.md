# Comparing `tmp/dateUts-0.1.6.tar.gz` & `tmp/dateUts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dateUts-0.1.6.tar", last modified: Wed Apr 26 21:24:11 2023, max compression
+gzip compressed data, was "dateUts-0.1.7.tar", last modified: Mon May  1 22:51:05 2023, max compression
```

## Comparing `dateUts-0.1.6.tar` & `dateUts-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 21:24:11.822960 dateUts-0.1.6/
--rw-rw-rw-   0        0        0      644 2023-04-26 21:23:08.000000 dateUts-0.1.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.1.6/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4331 2023-04-26 21:24:11.821963 dateUts-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3159 2023-04-26 21:06:44.000000 dateUts-0.1.6/README.md
--rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.1.6/commands.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 21:24:11.790048 dateUts-0.1.6/dateUts/
--rw-rw-rw-   0        0        0     4964 2023-04-26 21:20:07.000000 dateUts-0.1.6/dateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 21:24:11.820966 dateUts-0.1.6/dateUts.egg-info/
--rw-rw-rw-   0        0        0     4331 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 21:24:11.822960 dateUts-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-04-26 21:22:35.000000 dateUts-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:51:05.669511 dateUts-0.1.7/
+-rw-rw-rw-   0        0        0      644 2023-04-26 21:23:08.000000 dateUts-0.1.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.1.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4331 2023-05-01 22:51:05.668514 dateUts-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3159 2023-04-26 21:06:44.000000 dateUts-0.1.7/README.md
+-rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.1.7/commands.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 22:51:05.643581 dateUts-0.1.7/dateUts/
+-rw-rw-rw-   0        0        0     4964 2023-04-26 21:20:07.000000 dateUts-0.1.7/dateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:51:05.667516 dateUts-0.1.7/dateUts.egg-info/
+-rw-rw-rw-   0        0        0     4331 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 22:51:05.669511 dateUts-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-01 22:50:57.000000 dateUts-0.1.7/setup.py
```

### Comparing `dateUts-0.1.6/CHANGELOG.txt` & `dateUts-0.1.7/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.6/LICENCE.txt` & `dateUts-0.1.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.6/PKG-INFO` & `dateUts-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.6
+Version: 0.1.7
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dateUts-0.1.6/README.md` & `dateUts-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.6/dateUts/__init__.py` & `dateUts-0.1.7/dateUts/__init__.py`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.6/dateUts.egg-info/PKG-INFO` & `dateUts-0.1.7/dateUts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.6
+Version: 0.1.7
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dateUts-0.1.6/setup.py` & `dateUts-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dateUts',
-  version='0.1.6',
+  version='0.1.7',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

