# Comparing `tmp/JFIO-0.1.tar.gz` & `tmp/JFIO-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JFIO-0.1.tar", last modified: Tue May  2 10:37:34 2023, max compression
+gzip compressed data, was "JFIO-0.2.tar", last modified: Tue May  2 10:44:36 2023, max compression
```

## Comparing `JFIO-0.1.tar` & `JFIO-0.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:37:34.902451 JFIO-0.1/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:37:34.902451 JFIO-0.1/JFIO/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 09:56:41.000000 JFIO-0.1/JFIO/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:37:34.902451 JFIO-0.1/JFIO/write/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 09:57:36.000000 JFIO-0.1/JFIO/write/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1885 2023-05-02 10:21:36.000000 JFIO-0.1/JFIO/write/write.cpp
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:37:34.902451 JFIO-0.1/JFIO.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3028 2023-05-02 10:37:34.000000 JFIO-0.1/JFIO.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      226 2023-05-02 10:37:34.000000 JFIO-0.1/JFIO.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-02 10:37:34.000000 JFIO-0.1/JFIO.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       11 2023-05-02 10:37:34.000000 JFIO-0.1/JFIO.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-02 09:50:08.000000 JFIO-0.1/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       81 2023-05-02 10:32:27.000000 JFIO-0.1/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3028 2023-05-02 10:37:34.902451 JFIO-0.1/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2299 2023-05-02 09:53:52.000000 JFIO-0.1/README.md
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      824 2023-05-02 10:09:05.000000 JFIO-0.1/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-02 10:37:34.902451 JFIO-0.1/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      530 2023-05-02 10:16:40.000000 JFIO-0.1/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:44:36.353232 JFIO-0.2/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:44:36.353232 JFIO-0.2/JFIO/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:44:36.353232 JFIO-0.2/JFIO/ThirdParty/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-02 10:17:16.000000 JFIO-0.2/JFIO/ThirdParty/json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-02 10:05:00.000000 JFIO-0.2/JFIO/ThirdParty/pybind11_json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 09:56:41.000000 JFIO-0.2/JFIO/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:44:36.353232 JFIO-0.2/JFIO/write/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 09:57:36.000000 JFIO-0.2/JFIO/write/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1885 2023-05-02 10:21:36.000000 JFIO-0.2/JFIO/write/write.cpp
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 10:44:36.353232 JFIO-0.2/JFIO.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3028 2023-05-02 10:44:36.000000 JFIO-0.2/JFIO.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      285 2023-05-02 10:44:36.000000 JFIO-0.2/JFIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-02 10:44:36.000000 JFIO-0.2/JFIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       11 2023-05-02 10:44:36.000000 JFIO-0.2/JFIO.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-02 09:50:08.000000 JFIO-0.2/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      105 2023-05-02 10:42:14.000000 JFIO-0.2/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3028 2023-05-02 10:44:36.353232 JFIO-0.2/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2299 2023-05-02 09:53:52.000000 JFIO-0.2/README.md
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      824 2023-05-02 10:44:29.000000 JFIO-0.2/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-02 10:44:36.353232 JFIO-0.2/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      530 2023-05-02 10:16:40.000000 JFIO-0.2/setup.py
```

### Comparing `JFIO-0.1/JFIO/write/write.cpp` & `JFIO-0.2/JFIO/write/write.cpp`

 * *Files identical despite different names*

### Comparing `JFIO-0.1/JFIO.egg-info/PKG-INFO` & `JFIO-0.2/JFIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JFIO
-Version: 0.1
+Version: 0.2
 Summary: JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files.
 Home-page: https://github.com/PabloIbannez/JFIO
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JFIO-0.1/LICENSE` & `JFIO-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `JFIO-0.1/PKG-INFO` & `JFIO-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JFIO
-Version: 0.1
+Version: 0.2
 Summary: JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files.
 Home-page: https://github.com/PabloIbannez/JFIO
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JFIO-0.1/README.md` & `JFIO-0.2/README.md`

 * *Files identical despite different names*

### Comparing `JFIO-0.1/pyproject.toml` & `JFIO-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-cuda-cpp", "setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="JFIO"
-version="0.1"
+version="0.2"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `JFIO-0.1/setup.py` & `JFIO-0.2/setup.py`

 * *Files identical despite different names*

