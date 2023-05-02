# Comparing `tmp/screcode-0.1.2.dev202304290408-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202305020534-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 119321 bytes, number of entries: 6
+Zip file size: 119319 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
 -rw-r--r--  2.0 unx    61731 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304290408.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304290408.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304290408.dist-info/RECORD
-6 files, 212517 bytes uncompressed, 118417 bytes compressed:  44.3%
+-rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305020534.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305020534.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202305020534.dist-info/RECORD
+6 files, 212562 bytes uncompressed, 118415 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304290408.dist-info/METADATA
+Filename: screcode-0.1.2.dev202305020534.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304290408.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202305020534.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304290408.dist-info/RECORD
+Filename: screcode-0.1.2.dev202305020534.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `screcode-0.1.2.dev202304290408.dist-info/METADATA` & `screcode-0.1.2.dev202305020534.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304290408
+Version: 0.1.2.dev202305020534
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: adjustText (>=0.7)
 Requires-Dist: anndata (>=0.8.0,<0.9.0)
 Requires-Dist: datetime (>=4.0)
 Requires-Dist: harmonypy (>=0.0.9)
 Requires-Dist: matplotlib (>=3.4.3)
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: scikit-learn (>=0.24)
```

