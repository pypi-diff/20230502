# Comparing `tmp/geode-ml-2.6.8.tar.gz` & `tmp/geode-ml-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geode-ml-2.6.8.tar", last modified: Tue May  2 16:01:10 2023, max compression
+gzip compressed data, was "geode-ml-2.6.9.tar", last modified: Tue May  2 16:20:09 2023, max compression
```

## Comparing `geode-ml-2.6.8.tar` & `geode-ml-2.6.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:01:10.648373 geode-ml-2.6.8/
--rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.8/LICENSE
--rw-rw-rw-   0        0        0     3803 2023-05-02 16:01:10.644405 geode-ml-2.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 16:01:10.606374 geode-ml-2.6.8/geode/
--rw-rw-rw-   0        0        0       74 2023-05-02 16:00:31.000000 geode-ml-2.6.8/geode/__init__.py
--rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.8/geode/datasets.py
--rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.8/geode/losses.py
--rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.8/geode/metrics.py
--rw-rw-rw-   0        0        0    23456 2023-05-02 15:59:51.000000 geode-ml-2.6.8/geode/models.py
--rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.8/geode/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:01:10.639414 geode-ml-2.6.8/geode_ml.egg-info/
--rw-rw-rw-   0        0        0     3803 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      960 2023-05-02 16:00:24.000000 geode-ml-2.6.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 16:01:10.648373 geode-ml-2.6.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 16:20:09.836173 geode-ml-2.6.9/
+-rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.9/LICENSE
+-rw-rw-rw-   0        0        0     3803 2023-05-02 16:20:09.834206 geode-ml-2.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 16:20:09.816170 geode-ml-2.6.9/geode/
+-rw-rw-rw-   0        0        0       74 2023-05-02 16:15:26.000000 geode-ml-2.6.9/geode/__init__.py
+-rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.9/geode/datasets.py
+-rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.9/geode/losses.py
+-rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.9/geode/metrics.py
+-rw-rw-rw-   0        0        0    22374 2023-05-02 16:18:39.000000 geode-ml-2.6.9/geode/models.py
+-rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.9/geode/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:20:09.831172 geode-ml-2.6.9/geode_ml.egg-info/
+-rw-rw-rw-   0        0        0     3803 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      960 2023-05-02 16:15:26.000000 geode-ml-2.6.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:20:09.836173 geode-ml-2.6.9/setup.cfg
```

### Comparing `geode-ml-2.6.8/LICENSE` & `geode-ml-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.8/PKG-INFO` & `geode-ml-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.8
+Version: 2.6.9
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.8/README.md` & `geode-ml-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.8/geode/datasets.py` & `geode-ml-2.6.9/geode/datasets.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.8/geode/losses.py` & `geode-ml-2.6.9/geode/losses.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.8/geode/metrics.py` & `geode-ml-2.6.9/geode/metrics.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.8/geode/models.py` & `geode-ml-2.6.9/geode/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                  test_labels_path: str = None,
                  test_predictions_path: str = None,
                  data_names: list = None):
 
         self.test_imagery_path = str(test_imagery_path)
         self.test_labels_path = str(test_labels_path)
         self.test_predictions_path = str(test_predictions_path)
-        self.data_names = str(data_names)
+        self.data_names = list(data_names)
         self.test_metrics = {}
         self.model = None
 
         if test_imagery_path is not None:
             self.test_imagery_names = listdir(test_imagery_path)
 
         if len(self.test_imagery_names) == 0:
@@ -93,58 +93,40 @@
             # get the relevant subset
             sub_filenames = [x for x in filenames if dname in x]
 
             # create metrics dictionary
             metrics_dict = {}
 
             # create lists for each metric
-            true_positive_scores = []
-            false_positive_scores = []
-            false_negative_scores = []
             f1_scores = []
             jaccard_scores = []
             acc_scores = []
 
             # loop through the test subset
             for fname in sub_filenames:
                 if verbose:
                     print(fname)
 
                 # open the relevant datasets
                 y_true = Open(join(self.test_labels_path, fname)).ReadAsArray()
                 y_pred = Open(join(self.test_predictions_path, fname)).ReadAsArray()
 
                 # compute metrics
-                true_positive_scores.append(gm.true_positives(y_true=y_true,
-                                                              y_pred=y_pred,
-                                                              pos_label=pos_label))
-
-                false_positive_scores.append(gm.false_positives(y_true=y_true,
-                                                                y_pred=y_pred,
-                                                                pos_label=pos_label))
-
-                false_negative_scores.append(gm.false_negatives(y_true=y_true,
-                                                                y_pred=y_pred,
-                                                                pos_label=pos_label))
-
                 f1_scores.append(gm.f1(y_true=y_true,
                                        y_pred=y_pred,
                                        pos_label=pos_label))
 
                 jaccard_scores.append(gm.jaccard(y_true=y_true,
                                                  y_pred=y_pred,
                                                  pos_label=pos_label))
 
                 acc_scores.append(gm.total_accuracy(y_true=y_true,
                                                     y_pred=y_pred))
 
             # add scores to the metrics dictionary
-            metrics_dict['true_positives'] = mean(true_positive_scores)
-            metrics_dict['false_positives'] = mean(false_positive_scores)
-            metrics_dict['false_negatives'] = mean(false_negative_scores)
             metrics_dict['f1'] = mean(f1_scores)
             metrics_dict['jaccard'] = mean(jaccard_scores)
             metrics_dict['accuracy'] = mean(acc_scores)
 
             dname_metrics[dname] = metrics_dict
 
         # write the dictionary to a file
```

### Comparing `geode-ml-2.6.8/geode/utilities.py` & `geode-ml-2.6.9/geode/utilities.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.8/geode_ml.egg-info/PKG-INFO` & `geode-ml-2.6.9/geode_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.8
+Version: 2.6.9
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.8/pyproject.toml` & `geode-ml-2.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'geode-ml'
-version = '2.6.8'
+version = '2.6.9'
 description = "Clases and methods to help with the creation of geospatial training datasets and deep-learning models."
 readme = 'README.md'
 license = {file='LICENSE'}
 authors = [
     {name = 'Matt Reichenbach', email='matthew.reichenbach@gmail.com'},
 ]
 requires-python = '>=3.7'
```

