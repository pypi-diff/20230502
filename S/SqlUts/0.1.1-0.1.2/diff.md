# Comparing `tmp/SqlUts-0.1.1.tar.gz` & `tmp/SqlUts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SqlUts-0.1.1.tar", last modified: Tue Oct  4 01:45:09 2022, max compression
+gzip compressed data, was "SqlUts-0.1.2.tar", last modified: Tue May  2 14:19:43 2023, max compression
```

## Comparing `SqlUts-0.1.1.tar` & `SqlUts-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-04 01:45:09.724085 SqlUts-0.1.1/
--rw-rw-rw-   0        0        0      387 2022-08-29 11:55:24.000000 SqlUts-0.1.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-05-25 14:00:44.000000 SqlUts-0.1.1/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2022-05-25 22:21:08.000000 SqlUts-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5058 2022-10-04 01:45:09.723082 SqlUts-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2679 2022-08-29 11:55:48.000000 SqlUts-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-10-04 01:45:09.692084 SqlUts-0.1.1/SqlUts/
--rw-rw-rw-   0        0        0     1601 2022-10-04 01:44:18.000000 SqlUts-0.1.1/SqlUts/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-04 01:45:09.718088 SqlUts-0.1.1/SqlUts.egg-info/
--rw-rw-rw-   0        0        0     5058 2022-10-04 01:45:09.000000 SqlUts-0.1.1/SqlUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-10-04 01:45:09.000000 SqlUts-0.1.1/SqlUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-04 01:45:09.000000 SqlUts-0.1.1/SqlUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-10-04 01:45:09.000000 SqlUts-0.1.1/SqlUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-10-04 01:45:09.000000 SqlUts-0.1.1/SqlUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2022-10-04 01:40:33.000000 SqlUts-0.1.1/commands.txt
-drwxrwxrwx   0        0        0        0 2022-10-04 01:45:09.721085 SqlUts-0.1.1/dateUts/
--rw-rw-rw-   0        0        0     3911 2022-08-29 11:53:16.000000 SqlUts-0.1.1/dateUts/__init__.py
--rw-rw-rw-   0        0        0       42 2022-10-04 01:45:09.725083 SqlUts-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      781 2022-10-04 01:44:50.000000 SqlUts-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:19:43.197790 SqlUts-0.1.2/
+-rw-rw-rw-   0        0        0      387 2023-05-02 14:14:50.000000 SqlUts-0.1.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-05-02 14:14:50.000000 SqlUts-0.1.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-02 14:14:50.000000 SqlUts-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3590 2023-05-02 14:19:43.196791 SqlUts-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2679 2023-05-02 14:14:50.000000 SqlUts-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 14:19:43.175847 SqlUts-0.1.2/SqlUts/
+-rw-rw-rw-   0        0        0     1601 2023-05-02 14:14:50.000000 SqlUts-0.1.2/SqlUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:19:43.195794 SqlUts-0.1.2/SqlUts.egg-info/
+-rw-rw-rw-   0        0        0     3590 2023-05-02 14:19:43.000000 SqlUts-0.1.2/SqlUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-02 14:19:43.000000 SqlUts-0.1.2/SqlUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 14:19:43.000000 SqlUts-0.1.2/SqlUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-02 14:19:43.000000 SqlUts-0.1.2/SqlUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 14:19:43.000000 SqlUts-0.1.2/SqlUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2023-05-02 14:14:50.000000 SqlUts-0.1.2/commands.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 14:19:43.197790 SqlUts-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-05-02 14:18:51.000000 SqlUts-0.1.2/setup.py
```

### Comparing `SqlUts-0.1.1/LICENCE.txt` & `SqlUts-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `SqlUts-0.1.1/README.md` & `SqlUts-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `SqlUts-0.1.1/SqlUts/__init__.py` & `SqlUts-0.1.2/SqlUts/__init__.py`

 * *Files identical despite different names*

### Comparing `SqlUts-0.1.1/setup.py` & `SqlUts-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SqlUts',
-  version='0.1.1',
+  version='0.1.2',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

