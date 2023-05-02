# Comparing `tmp/widecity_image_downloader-0.0.4.tar.gz` & `tmp/widecity_image_downloader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widecity_image_downloader-0.0.4.tar", last modified: Tue May  2 04:31:24 2023, max compression
+gzip compressed data, was "widecity_image_downloader-0.0.5.tar", last modified: Tue May  2 05:38:42 2023, max compression
```

## Comparing `widecity_image_downloader-0.0.4.tar` & `widecity_image_downloader-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 04:31:24.381916 widecity_image_downloader-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-05-02 03:27:05.000000 widecity_image_downloader-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1291 2023-05-02 04:31:24.381916 widecity_image_downloader-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-05-02 03:40:54.000000 widecity_image_downloader-0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-05-02 03:42:24.000000 widecity_image_downloader-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      731 2023-05-02 04:31:24.386411 widecity_image_downloader-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 04:31:24.341906 widecity_image_downloader-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 04:31:24.362590 widecity_image_downloader-0.0.4/src/widecity_image_downloader/
--rw-rw-rw-   0        0        0      205 2023-05-02 04:31:00.000000 widecity_image_downloader-0.0.4/src/widecity_image_downloader/Image.py
--rw-rw-rw-   0        0        0        0 2023-05-02 03:28:55.000000 widecity_image_downloader-0.0.4/src/widecity_image_downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:31:24.379538 widecity_image_downloader-0.0.4/src/widecity_image_downloader.egg-info/
--rw-rw-rw-   0        0        0     1291 2023-05-02 04:31:24.000000 widecity_image_downloader-0.0.4/src/widecity_image_downloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-05-02 04:31:24.000000 widecity_image_downloader-0.0.4/src/widecity_image_downloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 04:31:24.000000 widecity_image_downloader-0.0.4/src/widecity_image_downloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-02 04:31:24.000000 widecity_image_downloader-0.0.4/src/widecity_image_downloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 05:38:42.503564 widecity_image_downloader-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-05-02 03:27:05.000000 widecity_image_downloader-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1291 2023-05-02 05:38:42.504561 widecity_image_downloader-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-05-02 03:40:54.000000 widecity_image_downloader-0.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-02 03:42:24.000000 widecity_image_downloader-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      731 2023-05-02 05:38:42.508198 widecity_image_downloader-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 05:38:42.453428 widecity_image_downloader-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 05:38:42.469196 widecity_image_downloader-0.0.5/src/widecity_image_downloader/
+-rw-rw-rw-   0        0        0      222 2023-05-02 05:32:33.000000 widecity_image_downloader-0.0.5/src/widecity_image_downloader/Image.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 03:28:55.000000 widecity_image_downloader-0.0.5/src/widecity_image_downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:38:42.501565 widecity_image_downloader-0.0.5/src/widecity_image_downloader.egg-info/
+-rw-rw-rw-   0        0        0     1291 2023-05-02 05:38:42.000000 widecity_image_downloader-0.0.5/src/widecity_image_downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-02 05:38:42.000000 widecity_image_downloader-0.0.5/src/widecity_image_downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 05:38:42.000000 widecity_image_downloader-0.0.5/src/widecity_image_downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-02 05:38:42.000000 widecity_image_downloader-0.0.5/src/widecity_image_downloader.egg-info/top_level.txt
```

### Comparing `widecity_image_downloader-0.0.4/PKG-INFO` & `widecity_image_downloader-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widecity_image_downloader
-Version: 0.0.4
+Version: 0.0.5
 Summary: a simple package to download images from internet based on the keywords provided.
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: widecity.official@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `widecity_image_downloader-0.0.4/README.md` & `widecity_image_downloader-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `widecity_image_downloader-0.0.4/setup.cfg` & `widecity_image_downloader-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6964 6563 6974 795f 696d 6167   = widecity_imag
 00000020: 655f 646f 776e 6c6f 6164 6572 0d0a 7665  e_downloader..ve
-00000030: 7273 696f 6e20 3d20 302e 302e 340d 0a61  rsion = 0.0.4..a
+00000030: 7273 696f 6e20 3d20 302e 302e 350d 0a61  rsion = 0.0.5..a
 00000040: 7574 686f 7220 3d20 4578 616d 706c 6520  uthor = Example 
 00000050: 4175 7468 6f72 0d0a 6175 7468 6f72 5f65  Author..author_e
 00000060: 6d61 696c 203d 2077 6964 6563 6974 792e  mail = widecity.
 00000070: 6f66 6669 6369 616c 4067 6d61 696c 2e63  official@gmail.c
 00000080: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000090: 3d20 6120 7369 6d70 6c65 2070 6163 6b61  = a simple packa
 000000a0: 6765 2074 6f20 646f 776e 6c6f 6164 2069  ge to download i
```

### Comparing `widecity_image_downloader-0.0.4/src/widecity_image_downloader.egg-info/PKG-INFO` & `widecity_image_downloader-0.0.5/src/widecity_image_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widecity-image-downloader
-Version: 0.0.4
+Version: 0.0.5
 Summary: a simple package to download images from internet based on the keywords provided.
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: widecity.official@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

