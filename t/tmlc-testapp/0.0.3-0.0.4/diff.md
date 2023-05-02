# Comparing `tmp/tmlc-testapp-0.0.3.tar.gz` & `tmp/tmlc-testapp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Drive_A\Python\pypidemo\dist\.tmp-nlk8s92d\tmlc-testapp-0.0.3.tar", last modified: Tue May  2 11:54:29 2023, max compression
+gzip compressed data, was "dist\tmlc-testapp-0.0.4.tar", last modified: Tue May  2 12:14:48 2023, max compression
```

## Comparing `tmlc-testapp-0.0.3.tar` & `tmlc-testapp-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:54:29.000000 tmlc-testapp-0.0.3/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 tmlc-testapp-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      653 2023-05-02 11:54:29.000000 tmlc-testapp-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 tmlc-testapp-0.0.3/README.md
--rw-rw-rw-   0        0        0      570 2023-05-02 11:53:06.000000 tmlc-testapp-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 11:54:29.000000 tmlc-testapp-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-05-02 11:53:00.000000 tmlc-testapp-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:54:29.000000 tmlc-testapp-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 11:54:29.000000 tmlc-testapp-0.0.3/src/runapp/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:24:47.000000 tmlc-testapp-0.0.3/src/runapp/__init__.py
--rw-rw-rw-   0        0        0       45 2023-05-02 11:00:50.000000 tmlc-testapp-0.0.3/src/runapp/app.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:54:29.000000 tmlc-testapp-0.0.3/src/tmlc_testapp.egg-info/
--rw-rw-rw-   0        0        0      653 2023-05-02 11:54:28.000000 tmlc-testapp-0.0.3/src/tmlc_testapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-02 11:54:29.000000 tmlc-testapp-0.0.3/src/tmlc_testapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 11:54:28.000000 tmlc-testapp-0.0.3/src/tmlc_testapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 11:54:28.000000 tmlc-testapp-0.0.3/src/tmlc_testapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 11:54:28.000000 tmlc-testapp-0.0.3/src/tmlc_testapp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 tmlc-testapp-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      344 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 tmlc-testapp-0.0.4/README.md
+-rw-rw-rw-   0        0        0      570 2023-05-02 12:12:57.000000 tmlc-testapp-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-05-02 12:13:26.000000 tmlc-testapp-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/runapp/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:24:47.000000 tmlc-testapp-0.0.4/src/runapp/__init__.py
+-rw-rw-rw-   0        0        0      690 2023-05-02 12:12:39.000000 tmlc-testapp-0.0.4/src/runapp/app.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/tmlc_testapp.egg-info/
+-rw-rw-rw-   0        0        0      344 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/tmlc_testapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/tmlc_testapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/tmlc_testapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/tmlc_testapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 12:14:48.000000 tmlc-testapp-0.0.4/src/tmlc_testapp.egg-info/top_level.txt
```

### Comparing `tmlc-testapp-0.0.3/LICENSE` & `tmlc-testapp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlc-testapp-0.0.3/pyproject.toml` & `tmlc-testapp-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "tmlc-testapp"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tmlc-testapp-0.0.3/setup.py` & `tmlc-testapp-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setup(
     name='tmlc-testapp',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     author="TMLC",
     author_email='visalakshi2001@gmail.com',
     description = "TEST APP TMLC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/visalakshi2001/tmlc-pypi',
     keywords='example project',
-    setup_requires=['vosk', 'PyAudio'],
-    install_requires=['vosk', 'PyAudio'],
+    setup_requires=['vosk', 'pipwin'],
+    install_requires=['vosk', 'pipwin'],
 
 )
```

