# Comparing `tmp/geode-ml-2.6.7.tar.gz` & `tmp/geode-ml-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geode-ml-2.6.7.tar", last modified: Tue May  2 15:58:18 2023, max compression
+gzip compressed data, was "geode-ml-2.6.8.tar", last modified: Tue May  2 16:01:10 2023, max compression
```

## Comparing `geode-ml-2.6.7.tar` & `geode-ml-2.6.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 15:58:18.842755 geode-ml-2.6.7/
--rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.7/LICENSE
--rw-rw-rw-   0        0        0     3803 2023-05-02 15:58:18.840755 geode-ml-2.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 15:58:18.802756 geode-ml-2.6.7/geode/
--rw-rw-rw-   0        0        0       74 2023-05-02 15:57:05.000000 geode-ml-2.6.7/geode/__init__.py
--rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.7/geode/datasets.py
--rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.7/geode/losses.py
--rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.7/geode/metrics.py
--rw-rw-rw-   0        0        0    23992 2023-05-02 15:56:07.000000 geode-ml-2.6.7/geode/models.py
--rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.7/geode/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-02 15:58:18.835754 geode-ml-2.6.7/geode_ml.egg-info/
--rw-rw-rw-   0        0        0     3803 2023-05-02 15:58:18.000000 geode-ml-2.6.7/geode_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-02 15:58:18.000000 geode-ml-2.6.7/geode_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 15:58:18.000000 geode-ml-2.6.7/geode_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-02 15:58:18.000000 geode-ml-2.6.7/geode_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 15:58:18.000000 geode-ml-2.6.7/geode_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      960 2023-05-02 15:57:15.000000 geode-ml-2.6.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 15:58:18.843756 geode-ml-2.6.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 16:01:10.648373 geode-ml-2.6.8/
+-rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.8/LICENSE
+-rw-rw-rw-   0        0        0     3803 2023-05-02 16:01:10.644405 geode-ml-2.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 16:01:10.606374 geode-ml-2.6.8/geode/
+-rw-rw-rw-   0        0        0       74 2023-05-02 16:00:31.000000 geode-ml-2.6.8/geode/__init__.py
+-rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.8/geode/datasets.py
+-rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.8/geode/losses.py
+-rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.8/geode/metrics.py
+-rw-rw-rw-   0        0        0    23456 2023-05-02 15:59:51.000000 geode-ml-2.6.8/geode/models.py
+-rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.8/geode/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:01:10.639414 geode-ml-2.6.8/geode_ml.egg-info/
+-rw-rw-rw-   0        0        0     3803 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 16:01:10.000000 geode-ml-2.6.8/geode_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      960 2023-05-02 16:00:24.000000 geode-ml-2.6.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:01:10.648373 geode-ml-2.6.8/setup.cfg
```

### Comparing `geode-ml-2.6.7/LICENSE` & `geode-ml-2.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.7/PKG-INFO` & `geode-ml-2.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.7
+Version: 2.6.8
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.7/README.md` & `geode-ml-2.6.8/README.md`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.7/geode/datasets.py` & `geode-ml-2.6.8/geode/datasets.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.7/geode/losses.py` & `geode-ml-2.6.8/geode/losses.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.7/geode/metrics.py` & `geode-ml-2.6.8/geode/metrics.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.7/geode/models.py` & `geode-ml-2.6.8/geode/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,33 +130,23 @@
                                        y_pred=y_pred,
                                        pos_label=pos_label))
 
                 jaccard_scores.append(gm.jaccard(y_true=y_true,
                                                  y_pred=y_pred,
                                                  pos_label=pos_label))
 
-                precision_scores.append(gm.precision(y_true=y_true,
-                                                     y_pred=y_pred,
-                                                     pos_label=pos_label))
-
-                recall_scores.append(gm.recall(y_true=y_true,
-                                               y_pred=y_pred,
-                                               pos_label=pos_label))
-
                 acc_scores.append(gm.total_accuracy(y_true=y_true,
                                                     y_pred=y_pred))
 
             # add scores to the metrics dictionary
             metrics_dict['true_positives'] = mean(true_positive_scores)
             metrics_dict['false_positives'] = mean(false_positive_scores)
             metrics_dict['false_negatives'] = mean(false_negative_scores)
             metrics_dict['f1'] = mean(f1_scores)
             metrics_dict['jaccard'] = mean(jaccard_scores)
-            metrics_dict['precision'] = mean(precision_scores)
-            metrics_dict['recall'] = mean(recall_scores)
             metrics_dict['accuracy'] = mean(acc_scores)
 
             dname_metrics[dname] = metrics_dict
 
         # write the dictionary to a file
         if output_path is not None:
             with open(output_path, 'w') as f:
```

### Comparing `geode-ml-2.6.7/geode/utilities.py` & `geode-ml-2.6.8/geode/utilities.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.7/geode_ml.egg-info/PKG-INFO` & `geode-ml-2.6.8/geode_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.7
+Version: 2.6.8
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.7/pyproject.toml` & `geode-ml-2.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'geode-ml'
-version = '2.6.7'
+version = '2.6.8'
 description = "Clases and methods to help with the creation of geospatial training datasets and deep-learning models."
 readme = 'README.md'
 license = {file='LICENSE'}
 authors = [
     {name = 'Matt Reichenbach', email='matthew.reichenbach@gmail.com'},
 ]
 requires-python = '>=3.7'
```

