# Comparing `tmp/dongwha_datalab-0.0.0.2-py3-none-any.whl.zip` & `tmp/dongwha_datalab-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 1593 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       20 b- defN 23-Mar-14 06:54 data_lab/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-14 06:54 data_lab/data_lab.py
--rw-rw-rw-  2.0 fat      240 b- defN 23-Mar-14 06:55 dongwha_datalab-0.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-14 06:55 dongwha_datalab-0.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Mar-14 06:55 dongwha_datalab-0.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      487 b- defN 23-Mar-14 06:55 dongwha_datalab-0.0.0.2.dist-info/RECORD
-6 files, 910 bytes uncompressed, 699 bytes compressed:  23.2%
+Zip file size: 5576 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       29 b- defN 23-May-02 02:09 data_lab/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-14 06:58 data_lab/data_lab.py
+-rw-rw-rw-  2.0 fat    16679 b- defN 23-May-02 02:14 data_lab/mlops.py
+-rw-rw-rw-  2.0 fat      285 b- defN 23-May-02 02:19 dongwha_datalab-0.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 02:19 dongwha_datalab-0.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-02 02:19 dongwha_datalab-0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      561 b- defN 23-May-02 02:19 dongwha_datalab-0.0.0.3.dist-info/RECORD
+7 files, 17708 bytes uncompressed, 4572 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: data_lab/__init__.py
 Comment: 
 
 Filename: data_lab/data_lab.py
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.2.dist-info/METADATA
+Filename: data_lab/mlops.py
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.2.dist-info/WHEEL
+Filename: dongwha_datalab-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.2.dist-info/top_level.txt
+Filename: dongwha_datalab-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.2.dist-info/RECORD
+Filename: dongwha_datalab-0.0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: dongwha_datalab-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_lab/__init__.py

```diff
@@ -1 +1 @@
-__all__=['data_lab']
+__all__=['data_lab', 'mlops']
```

