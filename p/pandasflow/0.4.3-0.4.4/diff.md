# Comparing `tmp/pandasflow-0.4.3.tar.gz` & `tmp/pandasflow-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.4.3.tar", last modified: Thu Apr 27 15:26:41 2023, max compression
+gzip compressed data, was "pandasflow-0.4.4.tar", last modified: Tue May  2 12:30:29 2023, max compression
```

## Comparing `pandasflow-0.4.3.tar` & `pandasflow-0.4.4.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.972189 pandasflow-0.4.3/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.3/LICENCE
--rw-rw-rw-   0        0        0      694 2023-04-27 15:26:41.972189 pandasflow-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.961214 pandasflow-0.4.3/pandasflow/
--rw-rw-rw-   0        0        0      294 2023-04-27 15:23:21.000000 pandasflow-0.4.3/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.965203 pandasflow-0.4.3/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.3/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.3/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      355 2023-04-27 14:33:43.000000 pandasflow-0.4.3/pandasflow/get_import.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.967198 pandasflow-0.4.3/pandasflow/metrics/
--rw-rw-rw-   0        0        0      168 2023-04-27 14:37:44.000000 pandasflow-0.4.3/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0     1180 2023-04-27 15:22:37.000000 pandasflow-0.4.3/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.3/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.3/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.3/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.967198 pandasflow-0.4.3/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.3/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.969194 pandasflow-0.4.3/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.3/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.3/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.3/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.964206 pandasflow-0.4.3/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:26:41.973187 pandasflow-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.972189 pandasflow-0.4.3/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.3/test/__init__.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.3/test/split_tvt_test.py
--rw-rw-rw-   0        0        0      734 2023-04-27 14:51:02.000000 pandasflow-0.4.3/test/test_conf_mat.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.3/test/test_lloss_up.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.3/test/test_mean_error.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.3/test/test_split_tt.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.457468 pandasflow-0.4.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.4/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-05-02 12:30:29.457468 pandasflow-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.441322 pandasflow-0.4.4/pandasflow/
+-rw-rw-rw-   0        0        0      302 2023-05-02 12:30:18.000000 pandasflow-0.4.4/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.444045 pandasflow-0.4.4/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.4/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.4/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      371 2023-05-02 10:20:49.000000 pandasflow-0.4.4/pandasflow/get_import.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.447909 pandasflow-0.4.4/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      216 2023-05-02 11:59:40.000000 pandasflow-0.4.4/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      671 2023-05-02 12:29:16.000000 pandasflow-0.4.4/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.4.4/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.4/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.4/pandasflow/metrics/mean_error.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.448470 pandasflow-0.4.4/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.4.4/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.4/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.448914 pandasflow-0.4.4/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.4/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.451062 pandasflow-0.4.4/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.4/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.4/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.4/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.444045 pandasflow-0.4.4/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:30:29.457468 pandasflow-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.456802 pandasflow-0.4.4/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.4/test/__init__.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.4/test/split_tvt_test.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.4.4/test/test_best_f1.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.4.4/test/test_conf_mat.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.4/test/test_lloss_up.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.4/test/test_mean_error.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.4/test/test_split_tt.py
```

### Comparing `pandasflow-0.4.3/LICENCE` & `pandasflow-0.4.4/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/PKG-INFO` & `pandasflow-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.3
+Version: 0.4.4
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.3/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.4.4/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/pandasflow/metrics/conf_mat.py` & `pandasflow-0.4.4/pandasflow/metrics/conf_mat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sklearn.metrics import confusion_matrix
 import pandas as pd
 
 
 
 
-def conf_mat(df, y_true, y_pred, labels=None, sample_weight=None, normalize=None):
+def conf_mat(y_true, y_pred, labels=None, sample_weight=None, normalize=None):
 	"""Compute confusion matrix to evaluate the accuracy of a classification.
 	
 		Parameters
 		----------
 		y_true : array-like of shape (n_samples,)
 			Ground truth (correct) target values.
 
@@ -22,26 +22,24 @@
 			in ``y_true`` or ``y_pred`` are used in sorted order.
 		
 		Returns
 		-------
 		C :
 			TN, FP, FN, TP
 	"""
-	tn, fp, fn, tp = confusion_matrix(df[y_true], df[y_pred], labels=labels, sample_weight=sample_weight, normalize=normalize).ravel()
+	tn, fp, fn, tp = confusion_matrix(y_true, y_pred, labels=labels, sample_weight=sample_weight, normalize=normalize).ravel()
 	
 	table = pd.DataFrame()
 	table['']   = ['TN', 'FN']
 	table[' ']  = [tn, fn]
 	table['  '] = [fp, tp]
 	table['   '] = ['FP', 'TP']
 	table.index = ['', '']
 	
 	print(table)
 	print()
-	print('tn, fp, fn, tp')
-	print()
 	return tn, fp, fn, tp
```

### Comparing `pandasflow-0.4.3/pandasflow/metrics/lloss_up.py` & `pandasflow-0.4.4/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/pandasflow/reset_mi.py` & `pandasflow-0.4.4/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/pandasflow/split/train_test.py` & `pandasflow-0.4.4/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/pandasflow/split/train_valid_test.py` & `pandasflow-0.4.4/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.4.4/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.3
+Version: 0.4.4
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.3/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.4.4/pandasflow.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 pandasflow.egg-info/SOURCES.txt
 pandasflow.egg-info/dependency_links.txt
 pandasflow.egg-info/requires.txt
 pandasflow.egg-info/top_level.txt
 pandasflow/dev/__init__.py
 pandasflow/dev/err_mean_diff.py
 pandasflow/metrics/__init__.py
+pandasflow/metrics/best_f1.py
 pandasflow/metrics/conf_mat.py
 pandasflow/metrics/lloss_up.py
 pandasflow/metrics/mean_error.py
+pandasflow/model/__init__.py
 pandasflow/services/__init__.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
 test/split_tvt_test.py
+test/test_best_f1.py
 test/test_conf_mat.py
 test/test_lloss_up.py
 test/test_mean_error.py
 test/test_split_tt.py
```

### Comparing `pandasflow-0.4.3/setup.py` & `pandasflow-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/test/split_tvt_test.py` & `pandasflow-0.4.4/test/split_tvt_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.3/test/test_conf_mat.py` & `pandasflow-0.4.4/test/test_conf_mat.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 model = model.rename({'Exited': 'score_prod_age'}, axis=1)
 train = train.merge(model, how='left', on=['NumOfProducts', 'age_group'])
 test['age_group'] = pd.cut(test['Age'], [0, 31, 35, 40, 45, float('inf')])
 test = test.merge(model, how='left', on=['NumOfProducts', 'age_group'])
 test['y_pred'] = (test['score_prod_age'] > 0.5) * 1
 
 
-pdf.metrics.conf_mat(test, 'Exited', 'y_pred')
+pdf.metrics.conf_mat(test['Exited'], test['y_pred'])
```

### Comparing `pandasflow-0.4.3/test/test_lloss_up.py` & `pandasflow-0.4.4/test/test_lloss_up.py`

 * *Files identical despite different names*

