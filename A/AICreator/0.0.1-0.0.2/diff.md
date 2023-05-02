# Comparing `tmp/AICreator-0.0.1.tar.gz` & `tmp/AICreator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AICreator-0.0.1.tar", last modified: Tue May  2 13:44:30 2023, max compression
+gzip compressed data, was "AICreator-0.0.2.tar", last modified: Tue May  2 13:49:49 2023, max compression
```

## Comparing `AICreator-0.0.1.tar` & `AICreator-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:44:30.204968 AICreator-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:44:30.197338 AICreator-0.0.1/AICreator.egg-info/
--rw-rw-rw-   0        0        0      559 2023-05-02 13:44:29.000000 AICreator-0.0.1/AICreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-05-02 13:44:30.000000 AICreator-0.0.1/AICreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:44:29.000000 AICreator-0.0.1/AICreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 13:44:29.000000 AICreator-0.0.1/AICreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 13:44:29.000000 AICreator-0.0.1/AICreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 13:44:30.198845 AICreator-0.0.1/AICreatorPackage/
--rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.0.1/AICreatorPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:44:30.201855 AICreator-0.0.1/AICreatorPackage/functions/
--rw-rw-rw-   0        0        0      698 2023-05-02 13:30:27.000000 AICreator-0.0.1/AICreatorPackage/functions/AICreatorPackage.py
--rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.0.1/AICreatorPackage/functions/__init__.py
--rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-05-02 13:44:30.203854 AICreator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.0.1/README.txt
--rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.0.1/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-02 13:44:30.204968 AICreator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-05-02 12:11:50.000000 AICreator-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:49:49.693660 AICreator-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:49:49.684771 AICreator-0.0.2/AICreator.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-05-02 13:49:49.000000 AICreator-0.0.2/AICreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-05-02 13:49:49.000000 AICreator-0.0.2/AICreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:49:49.000000 AICreator-0.0.2/AICreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 13:49:49.000000 AICreator-0.0.2/AICreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 13:49:49.000000 AICreator-0.0.2/AICreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 13:49:49.685786 AICreator-0.0.2/AICreatorPackage/
+-rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.0.2/AICreatorPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:49:49.689666 AICreator-0.0.2/AICreatorPackage/functions/
+-rw-rw-rw-   0        0        0      698 2023-05-02 13:30:27.000000 AICreator-0.0.2/AICreatorPackage/functions/AICreatorPackage.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.0.2/AICreatorPackage/functions/__init__.py
+-rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2023-05-02 13:49:49.692660 AICreator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.0.2/README.txt
+-rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.0.2/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:49:49.693660 AICreator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-02 13:49:17.000000 AICreator-0.0.2/setup.py
```

### Comparing `AICreator-0.0.1/AICreator.egg-info/PKG-INFO` & `AICreator-0.0.2/AICreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.0.1/AICreatorPackage/functions/AICreatorPackage.py` & `AICreator-0.0.2/AICreatorPackage/functions/AICreatorPackage.py`

 * *Files identical despite different names*

### Comparing `AICreator-0.0.1/LICENCE.txt` & `AICreator-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `AICreator-0.0.1/PKG-INFO` & `AICreator-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.0.1/setup.py` & `AICreator-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='AICreator',
-    version='0.0.1',
+    version='0.0.2',
     description='AI Creator Package By - oren',
     long_description=open('README.txt').read(),
     url='',
     author='oren',
     author_email='orennadle@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='ai',
     packages=find_packages(),
-    install_requires=['CreateAPI']
+    install_requires=['requests']
 )
```

