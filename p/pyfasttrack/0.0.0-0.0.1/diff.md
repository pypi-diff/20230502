# Comparing `tmp/pyfasttrack-0.0.0-py2.py3-none-any.whl.zip` & `tmp/pyfasttrack-0.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10105 bytes, number of entries: 12
+Zip file size: 10104 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     6037 b- defN 23-May-02 10:07 pyfasttrack/base_detector.py
 -rw-r--r--  2.0 unx     5099 b- defN 23-Apr-26 16:47 pyfasttrack/data.py
 -rw-r--r--  2.0 unx     1190 b- defN 23-May-02 10:13 pyfasttrack/example.py
 -rw-r--r--  2.0 unx     1125 b- defN 23-May-02 10:13 pyfasttrack/example_yolo.py
--rw-r--r--  2.0 unx     1773 b- defN 23-May-02 10:01 pyfasttrack/ft_detector.py
+-rw-r--r--  2.0 unx     1774 b- defN 23-May-02 16:45 pyfasttrack/ft_detector.py
 -rw-r--r--  2.0 unx     7647 b- defN 23-May-01 19:13 pyfasttrack/tracker.py
--rw-r--r--  2.0 unx      666 b- defN 23-May-02 10:13 pyfasttrack/yolo_detector.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-02 10:23 pyfasttrack-0.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      469 b- defN 23-May-02 10:23 pyfasttrack-0.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-02 10:23 pyfasttrack-0.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-02 10:23 pyfasttrack-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      976 b- defN 23-May-02 10:23 pyfasttrack-0.0.0.dist-info/RECORD
-12 files, 26177 bytes uncompressed, 8469 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx      667 b- defN 23-May-02 16:45 pyfasttrack/yolo_detector.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-02 16:46 pyfasttrack-0.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      469 b- defN 23-May-02 16:46 pyfasttrack-0.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-02 16:46 pyfasttrack-0.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-02 16:46 pyfasttrack-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-May-02 16:46 pyfasttrack-0.0.1.dist-info/RECORD
+12 files, 26179 bytes uncompressed, 8468 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pyfasttrack/tracker.py
 Comment: 
 
 Filename: pyfasttrack/yolo_detector.py
 Comment: 
 
-Filename: pyfasttrack-0.0.0.dist-info/LICENSE
+Filename: pyfasttrack-0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyfasttrack-0.0.0.dist-info/METADATA
+Filename: pyfasttrack-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pyfasttrack-0.0.0.dist-info/WHEEL
+Filename: pyfasttrack-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyfasttrack-0.0.0.dist-info/top_level.txt
+Filename: pyfasttrack-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfasttrack-0.0.0.dist-info/RECORD
+Filename: pyfasttrack-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyfasttrack/ft_detector.py

```diff
@@ -1,8 +1,8 @@
-import base_detector as detection
+import .base_detector as detection
 import numpy as np
 import cv2
 
 
 class FtDetector(detection.BaseDetector):
     def __init__(self, params):
         self.params = params
```

## pyfasttrack/yolo_detector.py

```diff
@@ -1,8 +1,8 @@
-import base_detector as detection
+import .base_detector as detection
 import numpy as np
 import cv2
 from ultralytics import YOLO
 import logging
 
 logging.getLogger("ultralytics").setLevel(logging.WARNING)
 logging.getLogger("tensorflow").setLevel(logging.WARNING)
```

## Comparing `pyfasttrack-0.0.0.dist-info/LICENSE` & `pyfasttrack-0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfasttrack-0.0.0.dist-info/RECORD` & `pyfasttrack-0.0.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pyfasttrack/base_detector.py,sha256=5gQdNP309mwkxoMRmWg7H1R1WzDjCKfLOLpsbDdSG_g,6037
 pyfasttrack/data.py,sha256=L7SGFlKScaF3j1_dfyN23WQjb6sGuSFmOQ1E6oagg1s,5099
 pyfasttrack/example.py,sha256=I12cTAe0hfP_Z0Ui8kluqPMBhfofSvroi2iKf3sxyPQ,1190
 pyfasttrack/example_yolo.py,sha256=I3I0wRs9gLRma00mUq9xs02VspqbgwH2gGO3wUbYCyA,1125
-pyfasttrack/ft_detector.py,sha256=OSyMreydMdlxjYWGY6-yNAWY_IkcZrn12ygWuE5aLaw,1773
+pyfasttrack/ft_detector.py,sha256=Rc79ZiSee9N_TKSHVWfZqfE2GSX7gL4AYh9M2lO5fpI,1774
 pyfasttrack/tracker.py,sha256=xPe3iSemVafJyiRuDqQJgg9VoJM6tNLLMD-1XldjkXA,7647
-pyfasttrack/yolo_detector.py,sha256=HJIB7C3_QbXQIpF957VABCj_GMOsFCDL15SnO6azbSU,666
-pyfasttrack-0.0.0.dist-info/LICENSE,sha256=eyd8Ld0p97tgTpV-GiTZc1Y8bkYccVs4bQOUnjFDIZw,1073
-pyfasttrack-0.0.0.dist-info/METADATA,sha256=COBkksBmRi8oPv4NjcKtrZWmSEuYRDnIlgEWZMbZvjw,469
-pyfasttrack-0.0.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pyfasttrack-0.0.0.dist-info/top_level.txt,sha256=VRMBOrgsgQPywDMfMJMU5UxUxE0As9L9I2QFbhM7_8c,12
-pyfasttrack-0.0.0.dist-info/RECORD,,
+pyfasttrack/yolo_detector.py,sha256=hHlBx3PdDLcJciDToqk_dQ8r5l3iaTnyMKXmslS7Itw,667
+pyfasttrack-0.0.1.dist-info/LICENSE,sha256=eyd8Ld0p97tgTpV-GiTZc1Y8bkYccVs4bQOUnjFDIZw,1073
+pyfasttrack-0.0.1.dist-info/METADATA,sha256=CeGG7sQQFKx4eTED9fLdFq5mbdyQwmhOzUEKlKZ9TRY,469
+pyfasttrack-0.0.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pyfasttrack-0.0.1.dist-info/top_level.txt,sha256=VRMBOrgsgQPywDMfMJMU5UxUxE0As9L9I2QFbhM7_8c,12
+pyfasttrack-0.0.1.dist-info/RECORD,,
```

