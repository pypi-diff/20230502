# Comparing `tmp/rapidocr_openvino_gpu-1.0.0.tar.gz` & `tmp/rapidocr_openvino_gpu-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidocr_openvino_gpu-1.0.0.tar", last modified: Mon May  1 23:31:21 2023, max compression
+gzip compressed data, was "rapidocr_openvino_gpu-1.0.3.tar", last modified: Tue May  2 02:03:06 2023, max compression
```

## Comparing `rapidocr_openvino_gpu-1.0.0.tar` & `rapidocr_openvino_gpu-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/
--rw-rw-r--   0 jk        (1000) jk        (1000)    11356 2023-05-01 22:33:58.000000 rapidocr_openvino_gpu-1.0.0/LICENSE.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)     1034 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/PKG-INFO
--rwxrwxr-x   0 jk        (1000) jk        (1000)      244 2023-05-01 23:25:21.000000 rapidocr_openvino_gpu-1.0.0/README.md
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v2_cls/
--rwxr-xr-x   0 jk        (1000) jk        (1000)      110 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v2_cls/__init__.py
--rwxr-xr-x   0 jk        (1000) jk        (1000)     4078 2023-05-01 23:11:36.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v2_cls/text_cls.py
--rwxr-xr-x   0 jk        (1000) jk        (1000)     1164 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v2_cls/utils.py
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_det/
--rwxr-xr-x   0 jk        (1000) jk        (1000)      111 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_det/__init__.py
--rwxr-xr-x   0 jk        (1000) jk        (1000)     4061 2023-05-01 23:08:30.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_det/text_detect.py
--rwxr-xr-x   0 jk        (1000) jk        (1000)    13428 2023-04-20 19:49:20.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_det/utils.py
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_rec/
--rwxr-xr-x   0 jk        (1000) jk        (1000)       42 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_rec/__init__.py
--rwxr-xr-x   0 jk        (1000) jk        (1000)     4679 2023-05-01 23:10:55.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_rec/text_recognize.py
--rwxr-xr-x   0 jk        (1000) jk        (1000)     2557 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_rec/utils.py
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/
--rw-rw-r--   0 jk        (1000) jk        (1000)     1034 2023-05-01 23:31:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/PKG-INFO
--rw-rw-r--   0 jk        (1000) jk        (1000)      894 2023-05-01 23:31:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/SOURCES.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)        1 2023-05-01 23:31:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/dependency_links.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)       84 2023-05-01 23:31:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/entry_points.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)      115 2023-05-01 23:31:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/requires.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)       55 2023-05-01 23:31:21.000000 rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/top_level.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)       79 2023-05-01 23:31:21.960775 rapidocr_openvino_gpu-1.0.0/setup.cfg
--rw-rw-r--   0 jk        (1000) jk        (1000)     2285 2023-05-01 23:30:04.000000 rapidocr_openvino_gpu-1.0.0/setup.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/
+-rw-rw-r--   0 jk        (1000) jk        (1000)    11356 2023-05-01 22:33:58.000000 rapidocr_openvino_gpu-1.0.3/LICENSE.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1034 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/PKG-INFO
+-rwxrwxr-x   0 jk        (1000) jk        (1000)      244 2023-05-01 23:25:21.000000 rapidocr_openvino_gpu-1.0.3/README.md
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v2_cls/
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      110 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v2_cls/__init__.py
+-rwxr-xr-x   0 jk        (1000) jk        (1000)     4078 2023-05-01 23:11:36.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v2_cls/text_cls.py
+-rwxr-xr-x   0 jk        (1000) jk        (1000)     1164 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v2_cls/utils.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_det/
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      111 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_det/__init__.py
+-rwxr-xr-x   0 jk        (1000) jk        (1000)     4061 2023-05-01 23:08:30.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_det/text_detect.py
+-rwxr-xr-x   0 jk        (1000) jk        (1000)    13428 2023-04-20 19:49:20.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_det/utils.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_rec/
+-rwxr-xr-x   0 jk        (1000) jk        (1000)       42 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_rec/__init__.py
+-rwxr-xr-x   0 jk        (1000) jk        (1000)     4679 2023-05-01 23:10:55.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_rec/text_recognize.py
+-rwxr-xr-x   0 jk        (1000) jk        (1000)     2557 2023-04-20 03:01:21.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_rec/utils.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1034 2023-05-02 02:03:06.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/PKG-INFO
+-rw-rw-r--   0 jk        (1000) jk        (1000)      894 2023-05-02 02:03:06.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/SOURCES.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)        1 2023-05-02 02:03:06.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/dependency_links.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)       79 2023-05-02 02:03:06.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/entry_points.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)      115 2023-05-02 02:03:06.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/requires.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)       55 2023-05-02 02:03:06.000000 rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/top_level.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)       79 2023-05-02 02:03:06.073025 rapidocr_openvino_gpu-1.0.3/setup.cfg
+-rw-rw-r--   0 jk        (1000) jk        (1000)     2280 2023-05-02 02:02:46.000000 rapidocr_openvino_gpu-1.0.3/setup.py
```

### Comparing `rapidocr_openvino_gpu-1.0.0/LICENSE.txt` & `rapidocr_openvino_gpu-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/PKG-INFO` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: rapidocr_openvino_gpu
-Version: 1.0.0
+Name: rapidocr-openvino-gpu
+Version: 1.0.3
 Summary: A cross platform OCR Library based on OpenVINO.
 Home-page: https://github.com/jaggiK/RapidOCR
 Author: SWHL
 Author-email: jagadishkmahendran@gmail.com
 License: Apache-2.0
-Download-URL: https://github.com/jaggiK/rapidocr_openvino_gpu/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/jaggiK/rapidocr_openvino_gpu/archive/refs/tags/1.0.3.tar.gz
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v2_cls/text_cls.py` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v2_cls/text_cls.py`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v2_cls/utils.py` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v2_cls/utils.py`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_det/text_detect.py` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_det/text_detect.py`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_det/utils.py` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_det/utils.py`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_rec/text_recognize.py` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_rec/text_recognize.py`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/ch_ppocr_v3_rec/utils.py` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/ch_ppocr_v3_rec/utils.py`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/PKG-INFO` & `rapidocr_openvino_gpu-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: rapidocr-openvino-gpu
-Version: 1.0.0
+Name: rapidocr_openvino_gpu
+Version: 1.0.3
 Summary: A cross platform OCR Library based on OpenVINO.
 Home-page: https://github.com/jaggiK/RapidOCR
 Author: SWHL
 Author-email: jagadishkmahendran@gmail.com
 License: Apache-2.0
-Download-URL: https://github.com/jaggiK/rapidocr_openvino_gpu/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/jaggiK/rapidocr_openvino_gpu/archive/refs/tags/1.0.3.tar.gz
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `rapidocr_openvino_gpu-1.0.0/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/SOURCES.txt` & `rapidocr_openvino_gpu-1.0.3/rapidocr_openvino_gpu/rapidocr_openvino_gpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidocr_openvino_gpu-1.0.0/setup.py` & `rapidocr_openvino_gpu-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     return readme
 
 
 MODULE_NAME = 'rapidocr_openvino_gpu'
 
 obtainer = GetPyPiLatestVersion()
 latest_version = obtainer(MODULE_NAME)
-VERSION_NUM = "1.0.0"#obtainer.version_add_one(latest_version)
+VERSION_NUM = "1.0.3"#obtainer.version_add_one(latest_version)
 
 # 优先提取commit message中的语义化版本号，如无，则自动加1
 if len(sys.argv) > 2:
     match_str = ' '.join(sys.argv[2:])
     matched_versions = obtainer.extract_version(match_str)
     if matched_versions:
         VERSION_NUM = matched_versions
@@ -57,11 +57,11 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.6,<=3.10',
     entry_points={
-        'console_scripts': [f'{MODULE_NAME}={MODULE_NAME}.rapid_ocr_api:main'],
+        'console_scripts': [f'{MODULE_NAME}={MODULE_NAME}.rapid_ocr_api'],
     },
-    download_url="https://github.com/jaggiK/rapidocr_openvino_gpu/archive/refs/tags/1.0.0.tar.gz",
+    download_url="https://github.com/jaggiK/rapidocr_openvino_gpu/archive/refs/tags/1.0.3.tar.gz",
 )
```

