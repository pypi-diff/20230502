# Comparing `tmp/koya_utilities-0.0.8-py2.py3-none-any.whl.zip` & `tmp/koya_utilities-0.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 10141 bytes, number of entries: 8
--rw-r--r--  2.0 unx       56 b- defN 22-Aug-23 02:01 koya_utilities/__init__.py
--rw-r--r--  2.0 unx     7149 b- defN 22-Aug-23 02:57 koya_utilities/koya_train.py
+Zip file size: 7621 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       30 b- defN 22-Aug-23 16:59 koya_utilities/__init__.py
 -rw-r--r--  2.0 unx    19374 b- defN 22-Aug-17 13:59 koya_utilities/koya_utilities.py
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-23 02:58 koya_utilities-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      508 b- defN 22-Aug-23 02:58 koya_utilities-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Aug-23 02:58 koya_utilities-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 22-Aug-23 02:58 koya_utilities-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      674 b- defN 22-Aug-23 02:58 koya_utilities-0.0.8.dist-info/RECORD
-8 files, 27886 bytes uncompressed, 8951 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx        0 b- defN 22-Aug-23 17:10 koya_utilities-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      508 b- defN 22-Aug-23 17:10 koya_utilities-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Aug-23 17:10 koya_utilities-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 22-Aug-23 17:10 koya_utilities-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      589 b- defN 22-Aug-23 17:10 koya_utilities-0.0.9.dist-info/RECORD
+7 files, 20626 bytes uncompressed, 6563 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: koya_utilities/__init__.py
 Comment: 
 
-Filename: koya_utilities/koya_train.py
-Comment: 
-
 Filename: koya_utilities/koya_utilities.py
 Comment: 
 
-Filename: koya_utilities-0.0.8.dist-info/LICENSE
+Filename: koya_utilities-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: koya_utilities-0.0.8.dist-info/METADATA
+Filename: koya_utilities-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: koya_utilities-0.0.8.dist-info/WHEEL
+Filename: koya_utilities-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: koya_utilities-0.0.8.dist-info/top_level.txt
+Filename: koya_utilities-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: koya_utilities-0.0.8.dist-info/RECORD
+Filename: koya_utilities-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## koya_utilities/__init__.py

```diff
@@ -1,2 +1 @@
 from .koya_utilities import *
-from .koya_train import *
```

