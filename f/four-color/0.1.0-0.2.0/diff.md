# Comparing `tmp/four_color-0.1.0-py3-none-any.whl.zip` & `tmp/four_color-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7621 bytes, number of entries: 6
+Zip file size: 7620 bytes, number of entries: 6
 -rw-r--r--  2.0 unx     2934 b- defN 80-Jan-01 00:00 four_color/__init__.py
 -rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 four_color/__main__.py
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 four_color-0.1.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 four_color-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1428 b- defN 16-Jan-01 00:00 four_color-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      465 b- defN 16-Jan-01 00:00 four_color-0.1.0.dist-info/RECORD
-6 files, 16961 bytes uncompressed, 6787 bytes compressed:  60.0%
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 four_color-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 four_color-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1373 b- defN 80-Jan-01 00:00 four_color-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx      465 b- defN 16-Jan-01 00:00 four_color-0.2.0.dist-info/RECORD
+6 files, 16906 bytes uncompressed, 6786 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: four_color/__init__.py
 Comment: 
 
 Filename: four_color/__main__.py
 Comment: 
 
-Filename: four_color-0.1.0.dist-info/LICENSE
+Filename: four_color-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: four_color-0.1.0.dist-info/WHEEL
+Filename: four_color-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: four_color-0.1.0.dist-info/METADATA
+Filename: four_color-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: four_color-0.1.0.dist-info/RECORD
+Filename: four_color-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `four_color-0.1.0.dist-info/LICENSE` & `four_color-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `four_color-0.1.0.dist-info/METADATA` & `four_color-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: four-color
-Version: 0.1.0
+Version: 0.2.0
 Summary: `four_color` is a package for Four Color Problem.
 Home-page: https://github.com/SaitoTsutomu/four_color
 License: Apache-2.0
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: flask (>=2.2.2,<3.0.0)
-Requires-Dist: networkx (>=2.8.8,<3.0.0)
-Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pulp (>=2.7.0,<3.0.0)
 Description-Content-Type: text/x-rst
 
 `four_color` is a package for Four Color Problem.
 ::
 
 * Download picture from https://www.dropbox.com/s/twiscp9h15so8no/sample.png?dl=1
```

