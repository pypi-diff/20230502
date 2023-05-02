# Comparing `tmp/geode-ml-2.6.5.tar.gz` & `tmp/geode-ml-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geode-ml-2.6.5.tar", last modified: Mon May  1 17:56:23 2023, max compression
+gzip compressed data, was "geode-ml-2.6.6.tar", last modified: Tue May  2 15:52:41 2023, max compression
```

## Comparing `geode-ml-2.6.5.tar` & `geode-ml-2.6.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:56:23.756154 geode-ml-2.6.5/
--rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.5/LICENSE
--rw-rw-rw-   0        0        0     3803 2023-05-01 17:56:23.755158 geode-ml-2.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 17:56:23.738162 geode-ml-2.6.5/geode/
--rw-rw-rw-   0        0        0       74 2023-05-01 17:55:46.000000 geode-ml-2.6.5/geode/__init__.py
--rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.5/geode/datasets.py
--rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.5/geode/losses.py
--rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.5/geode/metrics.py
--rw-rw-rw-   0        0        0    22073 2023-05-01 17:55:31.000000 geode-ml-2.6.5/geode/models.py
--rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.5/geode/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-01 17:56:23.752149 geode-ml-2.6.5/geode_ml.egg-info/
--rw-rw-rw-   0        0        0     3803 2023-05-01 17:56:23.000000 geode-ml-2.6.5/geode_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-01 17:56:23.000000 geode-ml-2.6.5/geode_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:56:23.000000 geode-ml-2.6.5/geode_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-01 17:56:23.000000 geode-ml-2.6.5/geode_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 17:56:23.000000 geode-ml-2.6.5/geode_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      960 2023-05-01 17:55:46.000000 geode-ml-2.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 17:56:23.756154 geode-ml-2.6.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 15:52:41.859173 geode-ml-2.6.6/
+-rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.6/LICENSE
+-rw-rw-rw-   0        0        0     3803 2023-05-02 15:52:41.856580 geode-ml-2.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 15:52:41.824628 geode-ml-2.6.6/geode/
+-rw-rw-rw-   0        0        0       74 2023-05-02 15:51:25.000000 geode-ml-2.6.6/geode/__init__.py
+-rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.6/geode/datasets.py
+-rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.6/geode/losses.py
+-rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.6/geode/metrics.py
+-rw-rw-rw-   0        0        0    24059 2023-05-02 15:50:35.000000 geode-ml-2.6.6/geode/models.py
+-rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.6/geode/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:52:41.852575 geode-ml-2.6.6/geode_ml.egg-info/
+-rw-rw-rw-   0        0        0     3803 2023-05-02 15:52:41.000000 geode-ml-2.6.6/geode_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-02 15:52:41.000000 geode-ml-2.6.6/geode_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 15:52:41.000000 geode-ml-2.6.6/geode_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-02 15:52:41.000000 geode-ml-2.6.6/geode_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 15:52:41.000000 geode-ml-2.6.6/geode_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      960 2023-05-02 15:51:37.000000 geode-ml-2.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 15:52:41.859173 geode-ml-2.6.6/setup.cfg
```

### Comparing `geode-ml-2.6.5/LICENSE` & `geode-ml-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.5/PKG-INFO` & `geode-ml-2.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.5
+Version: 2.6.6
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.5/README.md` & `geode-ml-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.5/geode/datasets.py` & `geode-ml-2.6.6/geode/datasets.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.5/geode/losses.py` & `geode-ml-2.6.6/geode/losses.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.5/geode/metrics.py` & `geode-ml-2.6.6/geode/metrics.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.5/geode/models.py` & `geode-ml-2.6.6/geode/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # models.py
 
-from geode.metrics import f1, jaccard, total_accuracy
+import geode.metrics as gm
 from geode.utilities import predict_raster
 from numpy import mean, unique
 from os import listdir, makedirs
 from os.path import isdir, join
 from osgeo.gdal import Open
 import tensorflow as tf
 from tensorflow.keras.layers import Add, BatchNormalization, Concatenate, Conv2D, Dropout, Input, MaxPooling2D, \
@@ -47,80 +47,119 @@
 
         if len(self.test_imagery_names) != len(self.test_imagery_names):
             raise Exception("There are a different number of test imagery and label files.")
 
         if set(self.test_imagery_names) != set(self.test_labels_name):
             raise Exception("Test imagery and label file names do not match.")
 
-    def compute_metrics(self, output_path: str = None) -> dict:
+    def compute_metrics(self, output_path: str = None,
+                        pos_label: int = 1,
+                        verbose: bool = True) -> dict:
 
-        """Computes various metrics on a test dataset; paired images and labels should have identical filenames.
+        """Computes various metrics on a test dataset; paired images and labels should have identical filenames. Both
+        Jaccard and F1 metrics assume binary labeling.
 
         Args:
-            output_path: the path to write a text-file of metrics.
+            output_path: the path to write a text-file of metrics;
+            pos_label: the label for which to compute metrics;
+            verbose: whether to print progress.
 
         Returns:
              A dictionary containing various calculated metrics for each test raster.
 
         Raises:
             Exception: if there are no predicted rasters at test_predictions_path;
         """
 
         # coerce arguments to correct type
         output_path = str(output_path)
+        pos_label = int(pos_label)
+        verbose = bool(verbose)
 
         # check that there are predictions
         if len(listdir(self.test_predictions_path)) == 0:
             raise Exception("No predicted imagery has been generated.")
 
         # create dictionary to hold metric dictionaries
         dname_metrics = {}
 
         # get the test_filenames:
         filenames = listdir(self.test_labels_path)
 
         # loop through the test imagery
         for dname in self.data_names:
+            if verbose:
+                print(dname)
+
             # get the relevant subset
             sub_filenames = [x for x in filenames if dname in x]
 
             # create metrics dictionary
             metrics_dict = {}
 
             # create lists for each metric
-            acc_scores = []
+            true_positive_scores = []
+            false_positive_scores = []
+            false_negative_scores = []
             f1_scores = []
             jaccard_scores = []
+            precision_scores = []
+            recall_scores = []
+            acc_scores = []
 
             # loop through the test subset
             for fname in sub_filenames:
+                if verbose:
+                    print(fname)
+
                 # open the relevant datasets
                 y_true = Open(join(self.test_labels_path, fname)).ReadAsArray()
                 y_pred = Open(join(self.test_predictions_path, fname)).ReadAsArray()
 
-                # get the label values
-                labels = unique(y_true)
-
-                # compute total accuracy
-                acc_scores.append(total_accuracy(y_true, y_pred))
-
-                # compute F1 and Jaccard scores for each label
-                for label in labels:
-                    f1_scores.append(f1(y_true=y_true,
-                                        y_pred=y_pred,
-                                        pos_label=label))
-
-                    jaccard_scores.append(jaccard(y_true=y_true,
-                                                  y_pred=y_pred,
-                                                  pos_label=label))
-
-            # add F1 and Jaccard scores to the metrics dictionary
-            metrics_dict['Acc'] = mean(acc_scores)
-            metrics_dict['F1'] = mean(f1_scores)
-            metrics_dict['Jaccard'] = mean(jaccard_scores)
+                # compute metrics
+                true_positive_scores.append(gm.true_positives(y_true=y_true,
+                                                              y_pred=y_pred,
+                                                              pos_label=pos_label))
+
+                false_positive_scores.append(gm.false_positives(y_true=y_true,
+                                                                y_pred=y_pred,
+                                                                pos_label=pos_label))
+
+                false_negative_scores.append(gm.false_negatives(y_true=y_true,
+                                                                y_pred=y_pred,
+                                                                pos_label=pos_label))
+
+                f1_scores.append(gm.f1(y_true=y_true,
+                                       y_pred=y_pred,
+                                       pos_label=pos_label))
+
+                jaccard_scores.append(gm.jaccard(y_true=y_true,
+                                                 y_pred=y_pred,
+                                                 pos_label=pos_label))
+
+                precision_scores.append(gm.precision(y_true=y_true,
+                                                     y_pred=y_pred,
+                                                     pos_label=pos_label))
+
+                recall_scores.append(gm.recall(y_true=y_true,
+                                               y_pred=y_pred,
+                                               pos_label=pos_label))
+
+                acc_scores.append(gm.total_accuracy(y_true=y_true,
+                                                    y_pred=y_pred))
+
+            # add scores to the metrics dictionary
+            metrics_dict['true_positives'] = mean(true_positive_scores)
+            metrics_dict['false_positives'] = mean(false_positive_scores)
+            metrics_dict['false_negatives'] = mean(false_negative_scores)
+            metrics_dict['f1'] = mean(f1_scores)
+            metrics_dict['jaccard'] = mean(jaccard_scores)
+            metrics_dict['precision'] = mean(precision_scores)
+            metrics_dict['recall'] = mean(recall_scores)
+            metrics_dict['accuracy'] = mean(acc_scores)
 
             dname_metrics[dname] = metrics_dict
 
         # write the dictionary to a file
         if output_path is not None:
             with open(output_path, 'w') as f:
                 for key, value in dname_metrics.items():
```

### Comparing `geode-ml-2.6.5/geode/utilities.py` & `geode-ml-2.6.6/geode/utilities.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.5/geode_ml.egg-info/PKG-INFO` & `geode-ml-2.6.6/geode_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.5
+Version: 2.6.6
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.5/pyproject.toml` & `geode-ml-2.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'geode-ml'
-version = '2.6.5'
+version = '2.6.6'
 description = "Clases and methods to help with the creation of geospatial training datasets and deep-learning models."
 readme = 'README.md'
 license = {file='LICENSE'}
 authors = [
     {name = 'Matt Reichenbach', email='matthew.reichenbach@gmail.com'},
 ]
 requires-python = '>=3.7'
```

