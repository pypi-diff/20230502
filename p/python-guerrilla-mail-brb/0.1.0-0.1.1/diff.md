# Comparing `tmp/python-guerrilla_mail_brb-0.1.0.tar.gz` & `tmp/python-guerrilla_mail_brb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-guerrilla_mail_brb-0.1.0.tar", last modified: Tue May  2 10:42:28 2023, max compression
+gzip compressed data, was "python-guerrilla_mail_brb-0.1.1.tar", last modified: Tue May  2 11:16:00 2023, max compression
```

## Comparing `python-guerrilla_mail_brb-0.1.0.tar` & `python-guerrilla_mail_brb-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:42:28.900783 python-guerrilla_mail_brb-0.1.0/
--rw-rw-rw-   0        0        0    35821 2023-05-02 09:20:13.000000 python-guerrilla_mail_brb-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3038 2023-05-02 10:42:28.900783 python-guerrilla_mail_brb-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-05-02 10:39:43.000000 python-guerrilla_mail_brb-0.1.0/README.rst
--rw-rw-rw-   0        0        0    11440 2023-05-02 09:51:25.000000 python-guerrilla_mail_brb-0.1.0/guerrillamail.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:42:28.898782 python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/
--rw-rw-rw-   0        0        0     3038 2023-05-02 10:42:28.000000 python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-02 10:42:28.000000 python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:42:28.000000 python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-02 10:42:28.000000 python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 10:42:28.000000 python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-02 10:42:28.000000 python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 10:42:28.901783 python-guerrilla_mail_brb-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-05-02 10:29:02.000000 python-guerrilla_mail_brb-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:16:00.540107 python-guerrilla_mail_brb-0.1.1/
+-rw-rw-rw-   0        0        0    35821 2023-05-02 09:20:13.000000 python-guerrilla_mail_brb-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3038 2023-05-02 11:16:00.539071 python-guerrilla_mail_brb-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1948 2023-05-02 10:39:43.000000 python-guerrilla_mail_brb-0.1.1/README.rst
+-rw-rw-rw-   0        0        0    11440 2023-05-02 09:51:25.000000 python-guerrilla_mail_brb-0.1.1/guerrillamail.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:16:00.538071 python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/
+-rw-rw-rw-   0        0        0     3038 2023-05-02 11:16:00.000000 python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-02 11:16:00.000000 python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:16:00.000000 python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-02 11:16:00.000000 python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 11:16:00.000000 python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-02 11:16:00.000000 python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 11:16:00.540107 python-guerrilla_mail_brb-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-05-02 11:14:03.000000 python-guerrilla_mail_brb-0.1.1/setup.py
```

### Comparing `python-guerrilla_mail_brb-0.1.0/LICENSE` & `python-guerrilla_mail_brb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-guerrilla_mail_brb-0.1.0/PKG-INFO` & `python-guerrilla_mail_brb-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-guerrilla_mail_brb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Client for the Guerrillamail temporary email server
 Home-page: https://github.com/sutkyne/python-guerrillamail
 Author: Nathan Jones
 License: GPL3
 Keywords: guerrillamail email client cli
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-guerrilla_mail_brb-0.1.0/README.rst` & `python-guerrilla_mail_brb-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-guerrilla_mail_brb-0.1.0/guerrillamail.py` & `python-guerrilla_mail_brb-0.1.1/guerrillamail.py`

 * *Files identical despite different names*

### Comparing `python-guerrilla_mail_brb-0.1.0/python_guerrilla_mail_brb.egg-info/PKG-INFO` & `python-guerrilla_mail_brb-0.1.1/python_guerrilla_mail_brb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-guerrilla-mail-brb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Client for the Guerrillamail temporary email server
 Home-page: https://github.com/sutkyne/python-guerrillamail
 Author: Nathan Jones
 License: GPL3
 Keywords: guerrillamail email client cli
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-guerrilla_mail_brb-0.1.0/setup.py` & `python-guerrilla_mail_brb-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open('README.rst', 'r', 'utf-8') as f:
     readme = f.read()
 with open('HISTORY.rst', 'r', 'utf-8') as f:
     history = f.read()
 
 setup(
     name='python-guerrilla_mail_brb',
-    version='0.1.0',
+    version='0.1.1',
     description='Client for the Guerrillamail temporary email server',
     long_description=readme + '\n\n' + history,
     keywords='guerrillamail email client cli',
     author='Nathan Jones',
     url='https://github.com/sutkyne/python-guerrillamail',
     py_modules=['guerrillamail'],
     install_requires=[
```

