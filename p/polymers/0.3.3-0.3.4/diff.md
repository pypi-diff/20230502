# Comparing `tmp/polymers-0.3.3-cp39-none-win_amd64.whl.zip` & `tmp/polymers-0.3.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1384610 bytes, number of entries: 6
--rw-r--r--  4.6 unx     4213 b- defN 23-Apr-27 19:06 polymers-0.3.3.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-27 19:06 polymers-0.3.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     1569 b- defN 23-Apr-27 19:06 polymers-0.3.3.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      115 b- defN 23-Apr-27 19:06 polymers/__init__.py
--rwxr-xr-x  4.6 unx  5851648 b- defN 23-Apr-27 19:06 polymers/polymers.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      484 b- defN 23-Apr-27 19:06 polymers-0.3.3.dist-info/RECORD
-6 files, 5858125 bytes uncompressed, 1383740 bytes compressed:  76.4%
+Zip file size: 1446874 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     4213 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1569 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      115 b- defN 23-May-01 22:10 polymers/__init__.py
+-rwxr-xr-x  4.6 unx  6094336 b- defN 23-May-01 22:10 polymers/polymers.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      484 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/RECORD
+6 files, 6100813 bytes uncompressed, 1446004 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: polymers-0.3.3.dist-info/METADATA
+Filename: polymers-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: polymers-0.3.3.dist-info/WHEEL
+Filename: polymers-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: polymers-0.3.3.dist-info/license_files/LICENSE
+Filename: polymers-0.3.4.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: polymers/__init__.py
 Comment: 
 
 Filename: polymers/polymers.cp39-win_amd64.pyd
 Comment: 
 
-Filename: polymers-0.3.3.dist-info/RECORD
+Filename: polymers-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `polymers-0.3.3.dist-info/METADATA` & `polymers-0.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymers
-Version: 0.3.3
+Version: 0.3.4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: cffi
@@ -15,16 +15,16 @@
 Keywords: julia,polymers,python,rust
 Author: Michael R. Buche
 Author-email: mrbuche@sandia.gov
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Documentation, https://polymers.readthedocs.io
-Project-URL: Repository, https://github.com/sandialabs/polymers
 Project-URL: Homepage, https://sandialabs.github.io/Polymers
+Project-URL: Repository, https://github.com/sandialabs/polymers
 
 # Polymers Modeling Library
 
 [![website](https://img.shields.io/badge/GitHub-website-6e5494?logo=github)](https://sandialabs.github.io/Polymers)
 [![examples](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/binder.svg)](https://mybinder.org/v2/gh/sandialabs/Polymers/main)
 
 The library is implemented entirely in Rust, including the Python API. The Julia API calls the Rust library.
```

## Comparing `polymers-0.3.3.dist-info/license_files/LICENSE` & `polymers-0.3.4.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

