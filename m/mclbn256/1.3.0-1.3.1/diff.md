# Comparing `tmp/mclbn256-1.3.0-py3-none-win_amd64.whl.zip` & `tmp/mclbn256-1.3.1-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 769684 bytes, number of entries: 8
--rw-r--r--  2.0 unx    54330 b- stor 22-Aug-25 19:04 mclbn256/mclbn256.py
--rw-rw-r--  2.0 unx       46 b- stor 22-Jul-15 18:34 mclbn256/__init__.py
--rw-rw-r--  2.0 unx   707072 b- stor 22-Jul-15 18:36 mclbn256/libmclbn256.dll
-?rw-------  2.0 unx     3706 b- stor 22-Aug-25 19:10 mclbn256-1.3.0.dist-info/METADATA
-?rw-------  2.0 unx       85 b- stor 22-Aug-25 19:10 mclbn256-1.3.0.dist-info/WHEEL
-?rw-------  2.0 unx        9 b- stor 22-Aug-25 19:10 mclbn256-1.3.0.dist-info/top_level.txt
-?rw-------  2.0 unx      676 b- stor 22-Aug-25 19:10 mclbn256-1.3.0.dist-info/RECORD
-?rw-------  2.0 unx     2674 b- stor 22-Aug-25 19:10 mclbn256-1.3.0.dist-info/LICENSE
-8 files, 768598 bytes uncompressed, 768598 bytes compressed:  0.0%
+Zip file size: 1477746 bytes, number of entries: 7
+-rw-r--r--  2.0 unx  1469718 b- stor 23-May-02 03:43 mclbn256/mclbn256.py
+-rw-r--r--  2.0 unx       45 b- stor 23-May-02 03:43 mclbn256/__init__.py
+?rw-------  2.0 unx     3658 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/METADATA
+?rw-------  2.0 unx       85 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/WHEEL
+?rw-------  2.0 unx        9 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/top_level.txt
+?rw-------  2.0 unx      595 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/RECORD
+?rw-------  2.0 unx     2674 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/LICENSE
+7 files, 1476784 bytes uncompressed, 1476784 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: mclbn256/mclbn256.py
 Comment: 
 
 Filename: mclbn256/__init__.py
 Comment: 
 
-Filename: mclbn256/libmclbn256.dll
+Filename: mclbn256-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: mclbn256-1.3.0.dist-info/METADATA
+Filename: mclbn256-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: mclbn256-1.3.0.dist-info/WHEEL
+Filename: mclbn256-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mclbn256-1.3.0.dist-info/top_level.txt
+Filename: mclbn256-1.3.1.dist-info/RECORD
 Comment: 
 
-Filename: mclbn256-1.3.0.dist-info/RECORD
-Comment: 
-
-Filename: mclbn256-1.3.0.dist-info/LICENSE
+Filename: mclbn256-1.3.1.dist-info/LICENSE
 Comment: 
 
 Zip file comment:
```

## mclbn256/mclbn256.py

```diff
@@ -1,20 +1,48 @@
 from ctypes import Structure, c_uint64, cdll, c_char_p, create_string_buffer
 from hashlib import blake2b, sha256
+"""
+Load the bn254 mcl shared object file and its mcl core dependency from this directory
+(with filepaths constructed for GH Actions), and write it to disk in a temporary file
+location. The mcl binary can then be read from disk directly and exported when the
+library is invoked without depending on linkage by the host OS.
+"""
 import platform
-import pkg_resources
+import tempfile
+import sys
+import os
+
+# Determine OS type
+pl = platform.system()
+arch = platform.processor()
+
+# Read hex-encoded mcl shared object file.
+if True:#arch == 'arm':
+    mcl_bs = bytes.fromhex('')  # pylint: disable=line-too-long
+
+# Generate a temporary folder structure on disk to which to write the mcl binaries.
+temp_dir = tempfile.TemporaryDirectory()  # pylint: disable=consider-using-with
+LOADER_TEMP_PATH = temp_dir.name
+if False: print(LOADER_TEMP_PATH)
+os.makedirs(os.path.join(LOADER_TEMP_PATH, 'lib'))
+LIB_EXT = ".dll" if pl == "Windows" else ".dylib" if pl == "Darwin" else ".so"
+fd_libmcl = open(os.path.join(LOADER_TEMP_PATH, 'lib', 'libmcl'+LIB_EXT), "wb")
+fd_libmclbn256 = open(os.path.join(LOADER_TEMP_PATH, 'libmclbn256'+LIB_EXT), "wb")
+fd_libmcl.write(mcl_bs)
+fd_libmclbn256.write(mclbn256_bs)
+# Close temp file to avoid multiprocess access error on Windows
+fd_libmcl.close()
+fd_libmclbn256.close()
+# Manual cleanup is optional, but saves ~1mb of space on dist immediately after being called.
+cleanup = temp_dir.cleanup
 
 def load_library(path_name):
-    if platform.system() == 'Windows':
-        lib_ext = ".dll"
-    elif platform.system() == 'Darwin':
-        lib_ext = ".dylib"
-    else:
-        lib_ext = ".so"
-    return cdll.LoadLibrary(pkg_resources.resource_filename('mclbn256', path_name+lib_ext))
+    return cdll.LoadLibrary(os.path.join(LOADER_TEMP_PATH, path_name+LIB_EXT))
+
 
 #
 # Define constants needed to replace the C headers
 #
 mclBn_CurveFp254BNb = 0
 EMBEDDING_DEGREE = 12
 DIMENSIONALITY = 3
```

## mclbn256/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from mclbn256.mclbn256 import Fr, G1, G2, GT
+from mclbn256.mclbn256 import Fr, G1, G2, GT
```

## Comparing `mclbn256-1.3.0.dist-info/METADATA` & `mclbn256-1.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mclbn256
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python bindings for the BN254/256 pairing-friendly curve supported by the MCl library.
 Home-page: https://github.com/nthparty/mclbn256
 Author: Wyatt Howe
 Author-email: Wyatt@nthparty.com
-Project-URL: Bug Tracker, https://github.com/nthparty/mclbn256/issues
+/issues
+License: None
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 mclbn256.py
```

## Comparing `mclbn256-1.3.0.dist-info/LICENSE` & `mclbn256-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*
