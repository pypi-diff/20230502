# Comparing `tmp/iterative_stats-0.0.2.tar.gz` & `tmp/iterative_stats-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterative_stats-0.0.2.tar", max compression
+gzip compressed data, was "iterative_stats-0.0.4.tar", max compression
```

## Comparing `iterative_stats-0.0.2.tar` & `iterative_stats-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,19 @@
--rw-r--r--   0        0        0     1518 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/LICENSE
--rw-r--r--   0        0        0     2163 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/README.md
--rw-r--r--   0        0        0      542 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/iterative_stats/abstract_iterative_statistics.py
--rw-r--r--   0        0        0     1378 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/iterative_stats/iterative_covariance.py
--rw-r--r--   0        0        0      617 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/iterative_stats/iterative_extrema.py
--rw-r--r--   0        0        0      384 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/iterative_stats/iterative_mean.py
--rw-r--r--   0        0        0     1098 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/iterative_stats/iterative_variance.py
--rw-r--r--   0        0        0       84 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/iterative_stats/utils/logger.py
--rw-r--r--   0        0        0     1196 2022-10-25 19:30:48.150977 iterative_stats-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 iterative_stats-0.0.2/setup.py
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 iterative_stats-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-05-02 12:49:58.009526 iterative_stats-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6928 2023-05-02 12:49:58.009526 iterative_stats-0.0.4/README.md
+-rw-r--r--   0        0        0     1357 2023-05-02 12:49:58.009526 iterative_stats-0.0.4/iterative_stats/abstract_iterative_statistics.py
+-rw-r--r--   0        0        0     2038 2023-05-02 12:49:58.009526 iterative_stats-0.0.4/iterative_stats/iterative_covariance.py
+-rw-r--r--   0        0        0     4374 2023-05-02 12:49:58.009526 iterative_stats-0.0.4/iterative_stats/iterative_dotproduct.py
+-rw-r--r--   0        0        0     1055 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/iterative_extrema.py
+-rw-r--r--   0        0        0     1661 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/iterative_mean.py
+-rw-r--r--   0        0        0     2205 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/iterative_quantile.py
+-rw-r--r--   0        0        0      920 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/iterative_threshold.py
+-rw-r--r--   0        0        0     1751 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/iterative_variance.py
+-rw-r--r--   0        0        0       63 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/sensitivity/__init__.py
+-rw-r--r--   0        0        0     9146 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/sensitivity/abstract_sensitivity.py
+-rw-r--r--   0        0        0     1864 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/sensitivity/sensitivity_jansen.py
+-rw-r--r--   0        0        0     3740 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/sensitivity/sensitivity_martinez.py
+-rw-r--r--   0        0        0     3401 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/sensitivity/sensitivity_saltelli.py
+-rw-r--r--   0        0        0      277 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/utils/dot_prod.py
+-rw-r--r--   0        0        0       84 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/iterative_stats/utils/logger.py
+-rw-r--r--   0        0        0     1255 2023-05-02 12:49:58.013527 iterative_stats-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7651 1970-01-01 00:00:00.000000 iterative_stats-0.0.4/PKG-INFO
```

### Comparing `iterative_stats-0.0.2/LICENSE` & `iterative_stats-0.0.4/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Frederique ROBIN
+Copyright (c) 2022, Frederique Robin, Alejandro Ribes, Anthony Geay
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `iterative_stats-0.0.2/iterative_stats/iterative_variance.py` & `iterative_stats-0.0.4/iterative_stats/iterative_threshold.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-from typing import Dict 
 import numpy as np
+import copy 
 
 from iterative_stats.abstract_iterative_statistics import AbstractIterativeStatistics
-from iterative_stats.iterative_mean import IterativeMean
 from iterative_stats.utils.logger import logger 
 
-class IterativeVariance(AbstractIterativeStatistics):
-    def __init__(self, conf: Dict):
-        super().__init__(conf)
-        self.mean = IterativeMean(conf)
-        self.sumOfCenteredSquares = np.zeros(conf.get('vector_size'))
+class IterativeThreshold(AbstractIterativeStatistics):
+    """
+        Iterative Threshold
+    """
+
+    def __init__(self, dim:int = 1, min_threshold: np.array = None, max_threshold: np.array = None, state: object = None):
+        super().__init__(dim, state)
+        self.min_threshold = min_threshold
+        self.max_threshold = max_threshold
 
     def increment(self, data):
         self.iteration += 1
 
-        if self.iteration > 1 : 
-            self.sumOfCenteredSquares += (
-                (self.iteration - 1) * (data - self.mean.get_stats()) ** 2 / self.iteration
-            )
-
-        # update mean 
-        self.mean.increment(data)
-
-        # compute variance
-        if self.iteration > 1 :
-            self.state = self.sumOfCenteredSquares / (self.iteration - 1)
-        logger.debug(f'increment= {self.increment}, variance= {self.state}')
+        if self.min_threshold is not None:
+            res_min = data >= self.min_threshold
+        else :
+            res_min = np.ones(self.dim)
+        if self.max_threshold is not None:
+            res_max = data <= self.max_threshold
+        else :
+            res_max = np.ones(self.dim)
 
-    def get_variance(self):
-        return self.state 
-
-    def get_mean(self):
-        return self.mean.get_stats()
+        self.state += res_min & res_max
+
```

### Comparing `iterative_stats-0.0.2/pyproject.toml` & `iterative_stats-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "iterative_stats"
-version = "0.0.2"
+version = "0.0.4"
 description = "This package implements iterative algorithms to compute some basics statistics"
 authors = ['Frederique Robin']
 readme = "README.md"
 license = "LICENSE" 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
+python = ">=3.8,<3.11"
 pyyaml = "6.0"
 numpy = "^1.19.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.1"
 autopep8 = "1.6.0"
+openturns = "1.19"
+scipy = "~1.8.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

