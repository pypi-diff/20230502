# Comparing `tmp/perceptron_pkg-abhaykeni-0.0.1.tar.gz` & `tmp/perceptron_pkg-abhaykeni-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Perceptron-Package/Perceptron-Package/dist/.tmp-1ut6ugxi/perceptron_pkg-abhaykeni-0.0.1.tar", last modified: Tue May  2 04:49:15 2023, max compression
+gzip compressed data, was "/home/runner/work/Perceptron-Package/Perceptron-Package/dist/.tmp-2xp0okea/perceptron_pkg-abhaykeni-0.0.2.tar", last modified: Tue May  2 04:59:33 2023, max compression
```

## Comparing `perceptron_pkg-abhaykeni-0.0.1.tar` & `perceptron_pkg-abhaykeni-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:49:15.000000 perceptron_pkg-abhaykeni-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 04:49:15.000000 perceptron_pkg-abhaykeni-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 04:49:01.000000 perceptron_pkg-abhaykeni-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 04:49:01.000000 perceptron_pkg-abhaykeni-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:49:15.000000 perceptron_pkg-abhaykeni-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-02 04:49:01.000000 perceptron_pkg-abhaykeni-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/oneNeuron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:49:01.000000 perceptron_pkg-abhaykeni-0.0.1/src/oneNeuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-02 04:49:01.000000 perceptron_pkg-abhaykeni-0.0.1/src/oneNeuron/perceptron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/perceptron_pkg_abhaykeni.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/perceptron_pkg_abhaykeni.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/perceptron_pkg_abhaykeni.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/perceptron_pkg_abhaykeni.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/perceptron_pkg_abhaykeni.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 04:49:14.000000 perceptron_pkg-abhaykeni-0.0.1/src/perceptron_pkg_abhaykeni.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-02 04:59:22.000000 perceptron_pkg-abhaykeni-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 04:59:22.000000 perceptron_pkg-abhaykeni-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-02 04:59:22.000000 perceptron_pkg-abhaykeni-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/oneNeuron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:59:22.000000 perceptron_pkg-abhaykeni-0.0.2/src/oneNeuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-02 04:59:22.000000 perceptron_pkg-abhaykeni-0.0.2/src/oneNeuron/perceptron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/perceptron_pkg_abhaykeni.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/perceptron_pkg_abhaykeni.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/perceptron_pkg_abhaykeni.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/perceptron_pkg_abhaykeni.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/perceptron_pkg_abhaykeni.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 04:59:33.000000 perceptron_pkg-abhaykeni-0.0.2/src/perceptron_pkg_abhaykeni.egg-info/top_level.txt
```

### Comparing `perceptron_pkg-abhaykeni-0.0.1/PKG-INFO` & `perceptron_pkg-abhaykeni-0.0.2/src/perceptron_pkg_abhaykeni.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: perceptron_pkg-abhaykeni
-Version: 0.0.1
+Name: perceptron-pkg-abhaykeni
+Version: 0.0.2
 Summary: A small package for perceptron
 Home-page: https://github.com/abhaykeni/perceptron-pkg
 Author: abhaykeni
 Author-email: abhaykeni@gmail.com
 Project-URL: Bug Tracker, https://github.com/abhaykeni/perceptron-pkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,7 +13,9 @@
 Description-Content-Type: text/markdown
 
 # Perceptron Package
 
 ## References - 
 
 * [Official Python Docs for PYPI](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
+
+* [Official Python Docs for PYPI](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries)
```

### Comparing `perceptron_pkg-abhaykeni-0.0.1/setup.py` & `perceptron_pkg-abhaykeni-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 PKG_NAME = "perceptron_pkg"
 USER_NAME = "abhaykeni"
 PROJECT_NAME = "perceptron-pkg"
 
 setuptools.setup(
     name=f"{PKG_NAME}-{USER_NAME}",
-    version="0.0.1",
+    version="0.0.2",
     author=USER_NAME,
     author_email="abhaykeni@gmail.com",
     description="A small package for perceptron",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/{USER_NAME}/{PROJECT_NAME}",
     project_urls={
```

### Comparing `perceptron_pkg-abhaykeni-0.0.1/src/oneNeuron/perceptron.py` & `perceptron_pkg-abhaykeni-0.0.2/src/oneNeuron/perceptron.py`

 * *Files identical despite different names*

### Comparing `perceptron_pkg-abhaykeni-0.0.1/src/perceptron_pkg_abhaykeni.egg-info/PKG-INFO` & `perceptron_pkg-abhaykeni-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: perceptron-pkg-abhaykeni
-Version: 0.0.1
+Name: perceptron_pkg-abhaykeni
+Version: 0.0.2
 Summary: A small package for perceptron
 Home-page: https://github.com/abhaykeni/perceptron-pkg
 Author: abhaykeni
 Author-email: abhaykeni@gmail.com
 Project-URL: Bug Tracker, https://github.com/abhaykeni/perceptron-pkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,7 +13,9 @@
 Description-Content-Type: text/markdown
 
 # Perceptron Package
 
 ## References - 
 
 * [Official Python Docs for PYPI](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
+
+* [Official Python Docs for PYPI](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries)
```

