# Comparing `tmp/widecity_image_downloader-0.0.0-py3-none-any.whl.zip` & `tmp/widecity_image_downloader-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1688 bytes, number of entries: 7
+Zip file size: 2295 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 03:28 widecity_image_downloader/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 03:30 widecity_image_downloader/main.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 03:42 widecity_image_downloader-0.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-02 03:42 widecity_image_downloader-0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 03:42 widecity_image_downloader-0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-May-02 03:42 widecity_image_downloader-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      649 b- defN 23-May-02 03:42 widecity_image_downloader-0.0.0.dist-info/RECORD
-7 files, 864 bytes uncompressed, 496 bytes compressed:  42.6%
+-rw-rw-rw-  2.0 fat      188 b- defN 23-May-02 04:10 widecity_image_downloader/main.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 04:12 widecity_image_downloader-0.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1291 b- defN 23-May-02 04:12 widecity_image_downloader-0.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 04:12 widecity_image_downloader-0.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-May-02 04:12 widecity_image_downloader-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      653 b- defN 23-May-02 04:12 widecity_image_downloader-0.0.1.dist-info/RECORD
+7 files, 2250 bytes uncompressed, 1103 bytes compressed:  51.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: widecity_image_downloader/__init__.py
 Comment: 
 
 Filename: widecity_image_downloader/main.py
 Comment: 
 
-Filename: widecity_image_downloader-0.0.0.dist-info/LICENSE
+Filename: widecity_image_downloader-0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: widecity_image_downloader-0.0.0.dist-info/METADATA
+Filename: widecity_image_downloader-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: widecity_image_downloader-0.0.0.dist-info/WHEEL
+Filename: widecity_image_downloader-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: widecity_image_downloader-0.0.0.dist-info/top_level.txt
+Filename: widecity_image_downloader-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: widecity_image_downloader-0.0.0.dist-info/RECORD
+Filename: widecity_image_downloader-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## widecity_image_downloader/main.py

```diff
@@ -0,0 +1,12 @@
+00000000: 6672 6f6d 2073 696d 706c 655f 696d 6167  from simple_imag
+00000010: 655f 646f 776e 6c6f 6164 2069 6d70 6f72  e_download impor
+00000020: 7420 7369 6d70 6c65 5f69 6d61 6765 5f64  t simple_image_d
+00000030: 6f77 6e6c 6f61 640d 0a0d 0a72 6573 706f  ownload....respo
+00000040: 6e73 6520 3d20 7369 6d70 6c65 5f69 6d61  nse = simple_ima
+00000050: 6765 5f64 6f77 6e6c 6f61 642e 446f 776e  ge_download.Down
+00000060: 6c6f 6164 6572 0d0a 6b65 7977 6f72 6473  loader..keywords
+00000070: 203d 205b 2766 6c6f 7765 7273 275d 0d0a   = ['flowers']..
+00000080: 0d0a 666f 7220 6b77 2069 6e20 6b65 7977  ..for kw in keyw
+00000090: 6f72 6473 3a0d 0a20 2020 2072 6573 706f  ords:..    respo
+000000a0: 6e73 6528 292e 646f 776e 6c6f 6164 286b  nse().download(k
+000000b0: 772c 3229 0d0a 2020 2020 0d0a            w,2)..    ..
```

