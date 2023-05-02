# Comparing `tmp/Functions_Main-0.0.1.tar.gz` & `tmp/Functions_Main-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Functions_Main-0.0.1.tar", last modified: Tue May  2 09:36:21 2023, max compression
+gzip compressed data, was "Functions_Main-0.2.tar", last modified: Tue May  2 10:06:53 2023, max compression
```

## Comparing `Functions_Main-0.0.1.tar` & `Functions_Main-0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:36:21.262681 Functions_Main-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:36:21.250064 Functions_Main-0.0.1/Functions/
--rw-rw-rw-   0        0        0     4496 2023-05-01 12:55:51.000000 Functions_Main-0.0.1/Functions/DataBase.py
--rw-rw-rw-   0        0        0    29046 2023-05-01 14:21:09.000000 Functions_Main-0.0.1/Functions/Functions.py
--rw-rw-rw-   0        0        0       23 2023-05-01 14:23:03.000000 Functions_Main-0.0.1/Functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:36:21.260682 Functions_Main-0.0.1/Functions_Main.egg-info/
--rw-rw-rw-   0        0        0      603 2023-05-02 09:36:21.000000 Functions_Main-0.0.1/Functions_Main.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-05-02 09:36:21.000000 Functions_Main-0.0.1/Functions_Main.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:36:21.000000 Functions_Main-0.0.1/Functions_Main.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 09:36:21.000000 Functions_Main-0.0.1/Functions_Main.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 09:36:21.000000 Functions_Main-0.0.1/Functions_Main.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-05-02 09:36:21.262681 Functions_Main-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-05-02 09:28:17.000000 Functions_Main-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 09:36:21.263680 Functions_Main-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-05-02 09:35:37.000000 Functions_Main-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:06:53.682018 Functions_Main-0.2/
+drwxrwxrwx   0        0        0        0 2023-05-02 10:06:53.667005 Functions_Main-0.2/Functions/
+-rw-rw-rw-   0        0        0     4496 2023-05-01 12:55:51.000000 Functions_Main-0.2/Functions/DataBase.py
+-rw-rw-rw-   0        0        0    29046 2023-05-01 14:21:09.000000 Functions_Main-0.2/Functions/Functions.py
+-rw-rw-rw-   0        0        0       23 2023-05-01 14:23:03.000000 Functions_Main-0.2/Functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:06:53.678997 Functions_Main-0.2/Functions_Main.egg-info/
+-rw-rw-rw-   0        0        0      601 2023-05-02 10:06:53.000000 Functions_Main-0.2/Functions_Main.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-02 10:06:53.000000 Functions_Main-0.2/Functions_Main.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 10:06:53.000000 Functions_Main-0.2/Functions_Main.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-02 10:06:53.000000 Functions_Main-0.2/Functions_Main.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      601 2023-05-02 10:06:53.680996 Functions_Main-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-05-02 09:28:17.000000 Functions_Main-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 10:06:53.682018 Functions_Main-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2023-05-02 10:06:16.000000 Functions_Main-0.2/setup.py
```

### Comparing `Functions_Main-0.0.1/Functions/DataBase.py` & `Functions_Main-0.2/Functions/DataBase.py`

 * *Files identical despite different names*

### Comparing `Functions_Main-0.0.1/Functions/Functions.py` & `Functions_Main-0.2/Functions/Functions.py`

 * *Files identical despite different names*

### Comparing `Functions_Main-0.0.1/Functions_Main.egg-info/PKG-INFO` & `Functions_Main-0.2/Functions_Main.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Functions-Main
-Version: 0.0.1
+Version: 0.2
 Summary: Packages To Avoid Annoying Repettive Task
 Author: Abdus-Samad (Abdus-Samad)
 Author-email: <Samadgame09@gmail.com>
 Keywords: python,Functions,Repettive,DataBase
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Functions_Main-0.0.1/PKG-INFO` & `Functions_Main-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Functions_Main
-Version: 0.0.1
+Version: 0.2
 Summary: Packages To Avoid Annoying Repettive Task
 Author: Abdus-Samad (Abdus-Samad)
 Author-email: <Samadgame09@gmail.com>
 Keywords: python,Functions,Repettive,DataBase
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Functions_Main-0.0.1/setup.py` & `Functions_Main-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.2'
 DESCRIPTION = 'Packages To Avoid Annoying Repettive Task'
 LONG_DESCRIPTION = 'A package that allows to build your projects with easee .'
 
 # Setting up
 setup(
     name="Functions_Main",
     version=VERSION,
     author="Abdus-Samad (Abdus-Samad)",
     author_email="<Samadgame09@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['shutil'],
+    install_requires=[],
     keywords=['python', 'Functions', 'Repettive', 'DataBase'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

