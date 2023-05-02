# Comparing `tmp/tmlc-testapp-0.0.1.tar.gz` & `tmp/tmlc-testapp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tmlc-testapp-0.0.1.tar", last modified: Tue May  2 10:54:34 2023, max compression
+gzip compressed data, was "D:\Drive_A\Python\pypidemo\dist\.tmp-q7u2c1vu\tmlc-testapp-0.0.2.tar", last modified: Tue May  2 11:25:56 2023, max compression
```

## Comparing `tmlc-testapp-0.0.1.tar` & `tmlc-testapp-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 tmlc-testapp-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      283 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 tmlc-testapp-0.0.1/README.md
--rw-rw-rw-   0        0        0      595 2023-05-02 10:39:25.000000 tmlc-testapp-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      433 2023-05-02 10:52:27.000000 tmlc-testapp-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/runapp/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:24:47.000000 tmlc-testapp-0.0.1/src/runapp/__init__.py
--rw-rw-rw-   0        0        0       43 2023-05-02 10:41:12.000000 tmlc-testapp-0.0.1/src/runapp/app.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/tmlc_testapp.egg-info/
--rw-rw-rw-   0        0        0      283 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/tmlc_testapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/tmlc_testapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/tmlc_testapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/tmlc_testapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 10:54:34.000000 tmlc-testapp-0.0.1/src/tmlc_testapp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 tmlc-testapp-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      653 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 tmlc-testapp-0.0.2/README.md
+-rw-rw-rw-   0        0        0      570 2023-05-02 11:24:36.000000 tmlc-testapp-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-05-02 11:24:41.000000 tmlc-testapp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/runapp/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:24:47.000000 tmlc-testapp-0.0.2/src/runapp/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-05-02 11:00:50.000000 tmlc-testapp-0.0.2/src/runapp/app.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/tmlc_testapp.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/tmlc_testapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/tmlc_testapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/tmlc_testapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/tmlc_testapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 11:25:56.000000 tmlc-testapp-0.0.2/src/tmlc_testapp.egg-info/top_level.txt
```

### Comparing `tmlc-testapp-0.0.1/LICENSE` & `tmlc-testapp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlc-testapp-0.0.1/pyproject.toml` & `tmlc-testapp-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "tmlc-testapp"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
-description = "JAI MATA DI"
+
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/visalakshi2001/tmlc-pypi"
-"Bug Tracker" = "https://github.com/visalakshi2001/tmlc-pypi/issues"
+"Bug Tracker" = "https://github.com/visalakshi2001/tmlc-pypi/issues"
```

