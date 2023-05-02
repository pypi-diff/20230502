# Comparing `tmp/large-image-source-tifffile-1.20.6.dev7.tar.gz` & `tmp/large-image-source-tifffile-1.20.6.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.20.6.dev7.tar", last modified: Mon Apr 24 16:45:35 2023, max compression
+gzip compressed data, was "large-image-source-tifffile-1.20.6.dev9.tar", last modified: Mon Apr 24 18:04:53 2023, max compression
```

## Comparing `large-image-source-tifffile-1.20.6.dev7.tar` & `large-image-source-tifffile-1.20.6.dev9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 16:45:35.068704 large-image-source-tifffile-1.20.6.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-04-24 16:45:34.000000 large-image-source-tifffile-1.20.6.dev7/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-04-24 16:45:35.068704 large-image-source-tifffile-1.20.6.dev7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-04-24 16:45:34.000000 large-image-source-tifffile-1.20.6.dev7/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 16:45:35.064704 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19914 2023-04-24 16:43:43.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-04-24 16:43:43.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 16:45:35.064704 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-04-24 16:45:34.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-04-24 16:45:35.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 16:45:34.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-24 16:45:34.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-04-24 16:45:34.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-04-24 16:45:34.000000 large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-24 16:45:35.068704 large-image-source-tifffile-1.20.6.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-04-24 16:43:43.000000 large-image-source-tifffile-1.20.6.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 18:04:52.996337 large-image-source-tifffile-1.20.6.dev9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-04-24 18:04:52.996337 large-image-source-tifffile-1.20.6.dev9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 18:04:52.996337 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19914 2023-04-24 18:02:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-04-24 18:02:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 18:04:52.996337 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-04-24 18:04:52.000000 large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-24 18:04:52.996337 large-image-source-tifffile-1.20.6.dev9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-04-24 18:02:52.000000 large-image-source-tifffile-1.20.6.dev9/setup.py
```

### Comparing `large-image-source-tifffile-1.20.6.dev7/LICENSE` & `large-image-source-tifffile-1.20.6.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.20.6.dev7/PKG-INFO` & `large-image-source-tifffile-1.20.6.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.20.6.dev7
+Version: 1.20.6.dev9
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.20.6.dev7/README.rst` & `large-image-source-tifffile-1.20.6.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.20.6.dev7/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.20.6.dev9/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.20.6.dev7
+Version: 1.20.6.dev9
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.20.6.dev7/setup.py` & `large-image-source-tifffile-1.20.6.dev9/setup.py`

 * *Files identical despite different names*

