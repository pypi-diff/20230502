# Comparing `tmp/se_lib-0.26.1.tar.gz` & `tmp/se_lib-0.26.2.tar.gz`

## Comparing `se_lib-0.26.1.tar` & `se_lib-0.26.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.1/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.1/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.1/selib/.DS_Store
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 se_lib-0.26.1/selib/__init__.py
--rw-r--r--   0        0        0    66122 2020-02-02 00:00:00.000000 se_lib-0.26.1/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26.1/LICENSE
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 se_lib-0.26.1/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 se_lib-0.26.1/pyproject.toml
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 se_lib-0.26.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.2/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.2/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.2/selib/.DS_Store
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 se_lib-0.26.2/selib/__init__.py
+-rw-r--r--   0        0        0    66122 2020-02-02 00:00:00.000000 se_lib-0.26.2/selib/selib.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26.2/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.2/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 se_lib-0.26.2/pyproject.toml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 se_lib-0.26.2/PKG-INFO
```

### Comparing `se_lib-0.26.1/.DS_Store` & `se_lib-0.26.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.1/selib/.DS_Store` & `se_lib-0.26.2/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.1/selib/selib.py` & `se_lib-0.26.2/selib/selib.py`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.1/LICENSE` & `se_lib-0.26.2/LICENSE`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.1/pyproject.toml` & `se_lib-0.26.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "se-lib"
-version = "0.26.1"
+version = "0.26.2"
 authors = [
   { name="se-lib Development Team", email="info@se-lib.org" },
 ]
 description = "Systems Engineering Library (se-lib)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `se_lib-0.26.1/PKG-INFO` & `se_lib-0.26.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.26.1
+Version: 0.26.2
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,40 +13,21 @@
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pysd
 Description-Content-Type: text/markdown
 
 # Systems Engineering Library (se-lib)
-Version .26.1
+Version .26.2
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ```bash
-r@mac ~/Documents/GitHub/se_lib_package ▶ python3 -m build
-* Creating venv isolated environment...
-* Installing packages in isolated environment... (hatchling)
-* Getting build dependencies for sdist...
-* Building sdist...
-* Building wheel from sdist
-* Creating venv isolated environment...
-* Installing packages in isolated environment... (hatchling)
-* Getting build dependencies for wheel...
-* Building wheel...
-Successfully built se_lib-0.2.tar.gz and se_lib-0.2-py3-none-any.whl
-r@mac ~/Documents/GitHub/se_lib_package ▶ python3 -m twine upload dist/*
-Uploading distributions to https://upload.pypi.org/legacy/
-Enter your username: __token__
-Enter your password: 
-Uploading se_lib-0.2-py3-none-any.whl
-100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 18.8/18.8 kB • 00:00 • 61.3 MB/s
-Uploading se_lib-0.2.tar.gz
-100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 18.3/18.3 kB • 00:00 • 60.5 MB/s
-
-View at:
-https://pypi.org/project/se-lib/0.2/```
+▶ python3 -m build
+▶ python3 -m twine upload dist/*
+```
```

