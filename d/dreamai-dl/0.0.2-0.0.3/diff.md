# Comparing `tmp/dreamai_dl-0.0.2.tar.gz` & `tmp/dreamai_dl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_dl-0.0.2.tar", last modified: Tue May  2 20:12:59 2023, max compression
+gzip compressed data, was "dreamai_dl-0.0.3.tar", last modified: Tue May  2 21:03:13 2023, max compression
```

## Comparing `dreamai_dl-0.0.2.tar` & `dreamai_dl-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 20:12:59.297266 dreamai_dl-0.0.2/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.2/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.2/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-02 20:12:59.297266 dreamai_dl-0.0.2/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.2/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 20:12:59.297266 dreamai_dl-0.0.2/dreamai_dl/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 20:12:54.000000 dreamai_dl-0.0.2/dreamai_dl/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-02 20:03:53.000000 dreamai_dl-0.0.2/dreamai_dl/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      165 2023-05-02 20:03:53.000000 dreamai_dl-0.0.2/dreamai_dl/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      643 2023-05-02 19:59:21.000000 dreamai_dl-0.0.2/dreamai_dl/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      346 2023-05-02 20:03:53.000000 dreamai_dl-0.0.2/dreamai_dl/utils.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 20:12:59.297266 dreamai_dl-0.0.2/dreamai_dl.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-02 20:12:59.000000 dreamai_dl-0.0.2/dreamai_dl.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      396 2023-05-02 20:12:59.000000 dreamai_dl-0.0.2/dreamai_dl.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 20:12:59.000000 dreamai_dl-0.0.2/dreamai_dl.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-02 20:12:59.000000 dreamai_dl-0.0.2/dreamai_dl.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.2/dreamai_dl.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1257 2023-05-02 20:12:59.000000 dreamai_dl-0.0.2/dreamai_dl.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-02 20:12:59.000000 dreamai_dl-0.0.2/dreamai_dl.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1936 2023-05-02 20:12:54.000000 dreamai_dl-0.0.2/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 20:12:59.297266 dreamai_dl-0.0.2/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.2/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 21:03:13.731446 dreamai_dl-0.0.3/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.3/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.3/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-02 21:03:13.731446 dreamai_dl-0.0.3/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.3/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 21:03:13.731446 dreamai_dl-0.0.3/dreamai_dl/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 21:03:06.000000 dreamai_dl-0.0.3/dreamai_dl/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-02 21:03:06.000000 dreamai_dl-0.0.3/dreamai_dl/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      165 2023-05-02 21:03:06.000000 dreamai_dl-0.0.3/dreamai_dl/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      690 2023-05-02 21:02:32.000000 dreamai_dl-0.0.3/dreamai_dl/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      346 2023-05-02 21:03:06.000000 dreamai_dl-0.0.3/dreamai_dl/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 21:03:13.731446 dreamai_dl-0.0.3/dreamai_dl.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-02 21:03:13.000000 dreamai_dl-0.0.3/dreamai_dl.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      396 2023-05-02 21:03:13.000000 dreamai_dl-0.0.3/dreamai_dl.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 21:03:13.000000 dreamai_dl-0.0.3/dreamai_dl.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-02 21:03:13.000000 dreamai_dl-0.0.3/dreamai_dl.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.3/dreamai_dl.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1257 2023-05-02 21:03:13.000000 dreamai_dl-0.0.3/dreamai_dl.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-02 21:03:13.000000 dreamai_dl-0.0.3/dreamai_dl.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1936 2023-05-02 21:03:03.000000 dreamai_dl-0.0.3/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 21:03:13.731446 dreamai_dl-0.0.3/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.3/setup.py
```

### Comparing `dreamai_dl-0.0.2/LICENSE` & `dreamai_dl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.2/PKG-INFO` & `dreamai_dl-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_dl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.2/dreamai_dl/imports.py` & `dreamai_dl-0.0.3/dreamai_dl/imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import timm
 import torch
 import torch.nn as nn
 import lightning as L
-import torchmetrics as tm
+import torchmetrics as TM
 import torch.nn.functional as F
 from torchvision.utils import make_grid
 from torchvision import transforms, models
+import torchvision.transforms.functional as TF
 from torch.utils.data import Dataset, DataLoader
 
 from dreamai.core import *
 from dreamai.vision import *
 from dreamai.imports import *
 
 from fastai.torch_core import Module
```

### Comparing `dreamai_dl-0.0.2/dreamai_dl.egg-info/PKG-INFO` & `dreamai_dl-0.0.3/dreamai_dl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-dl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.2/dreamai_dl.egg-info/requires.txt` & `dreamai_dl-0.0.3/dreamai_dl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.2/settings.ini` & `dreamai_dl-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_dl
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_dl
 nbs_path = nbs
 recursive = True
```

### Comparing `dreamai_dl-0.0.2/setup.py` & `dreamai_dl-0.0.3/setup.py`

 * *Files identical despite different names*

