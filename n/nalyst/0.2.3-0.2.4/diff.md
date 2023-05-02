# Comparing `tmp/nalyst-0.2.3.tar.gz` & `tmp/nalyst-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.2.3.tar", last modified: Fri Apr 21 16:19:30 2023, max compression
+gzip compressed data, was "nalyst-0.2.4.tar", last modified: Tue May  2 15:11:28 2023, max compression
```

## Comparing `nalyst-0.2.3.tar` & `nalyst-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 16:19:30.851935 nalyst-0.2.3/
--rw-rw-rw-   0        0        0      107 2023-04-21 16:17:56.000000 nalyst-0.2.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3712 2023-04-21 16:19:30.850824 nalyst-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2023-04-21 16:18:11.000000 nalyst-0.2.3/README.md
--rw-rw-rw-   0        0        0     1045 2023-04-21 15:49:06.000000 nalyst-0.2.3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 16:19:30.843314 nalyst-0.2.3/nalyst/
--rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.3/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.3/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.3/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.3/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.3/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.3/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.3/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.3/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.3/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.3/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.3/nalyst/RegressionPlot.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.3/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.3/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.3/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0     1045 2023-04-21 15:49:53.000000 nalyst-0.2.3/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 16:19:30.849803 nalyst-0.2.3/nalyst.egg-info/
--rw-rw-rw-   0        0        0     3712 2023-04-21 16:19:30.000000 nalyst-0.2.3/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-04-21 16:19:30.000000 nalyst-0.2.3/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 16:19:30.000000 nalyst-0.2.3/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-21 16:19:30.000000 nalyst-0.2.3/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 16:19:30.000000 nalyst-0.2.3/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 16:19:30.851935 nalyst-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-21 16:17:41.000000 nalyst-0.2.3/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.3/version.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:11:28.070153 nalyst-0.2.4/
+-rw-rw-rw-   0        0        0      107 2023-04-21 16:17:56.000000 nalyst-0.2.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3858 2023-05-02 15:11:28.070153 nalyst-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2742 2023-05-02 15:10:53.000000 nalyst-0.2.4/README.md
+-rw-rw-rw-   0        0        0     1232 2023-05-02 15:09:50.000000 nalyst-0.2.4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:11:28.065168 nalyst-0.2.4/nalyst/
+-rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.4/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.4/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     3020 2023-05-02 15:09:11.000000 nalyst-0.2.4/nalyst/CorrelationAnalysis.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.4/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.4/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.4/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.4/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.4/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.4/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.4/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.4/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.4/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.4/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.4/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.4/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     2771 2023-05-02 15:08:58.000000 nalyst-0.2.4/nalyst/TrendAnalyst.py
+-rw-rw-rw-   0        0        0     1232 2023-05-02 15:09:46.000000 nalyst-0.2.4/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:11:28.069156 nalyst-0.2.4/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     3858 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 15:11:28.071149 nalyst-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-05-02 15:11:11.000000 nalyst-0.2.4/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.4/version.py
```

### Comparing `nalyst-0.2.3/LICENSE` & `nalyst-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/PKG-INFO` & `nalyst-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.3
+Version: 0.2.4
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -74,14 +74,16 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
+from nalyst.CorrelationAnalysis import correlation_analysis
+from nalyst.TrendAnalyst import linear_regression_trend, LinearRegressionVisualizer
 ```
 
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION
```

### Comparing `nalyst-0.2.3/README.md` & `nalyst-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
+from nalyst.CorrelationAnalysis import correlation_analysis
+from nalyst.TrendAnalyst import linear_regression_trend, LinearRegressionVisualizer
 ```
 
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION
```

### Comparing `nalyst-0.2.3/__init__.py` & `nalyst-0.2.4/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
+from nalyst.CorrelationAnalysis import correlation_analysis
+from nalyst.TrendAnalyst import LinearModel, linear_regression_trend, LinearRegressionVisualizer
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -24,9 +26,10 @@
     'StandardScaler',
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
     'ThresholdClassifier',
-    'RegressionPlot'
+    'RegressionPlot',
+    'CorrelationAnalysis'
 ]
```

### Comparing `nalyst-0.2.3/nalyst/BetaFive.py` & `nalyst-0.2.4/nalyst/BetaFive.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/BetaMax.py` & `nalyst-0.2.4/nalyst/BetaMax.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/DecisionTree.py` & `nalyst-0.2.4/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/KMeans.py` & `nalyst-0.2.4/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/LinearRegression.py` & `nalyst-0.2.4/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/LogisticRegression.py` & `nalyst-0.2.4/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/MaxAbsScaler.py` & `nalyst-0.2.4/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/MinMaxScaler.py` & `nalyst-0.2.4/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/MonteCarloSimulator.py` & `nalyst-0.2.4/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/PCA.py` & `nalyst-0.2.4/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/RegressionPlot.py` & `nalyst-0.2.4/nalyst/RegressionPlot.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/StandardScaler.py` & `nalyst-0.2.4/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/TestTrainSplit.py` & `nalyst-0.2.4/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/ThresholdClassifier.py` & `nalyst-0.2.4/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.3/nalyst/__init__.py` & `nalyst-0.2.4/nalyst/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
+from nalyst.CorrelationAnalysis import correlation_analysis
+from nalyst.TrendAnalyst import LinearModel, linear_regression_trend, LinearRegressionVisualizer
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -24,9 +26,10 @@
     'StandardScaler',
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
     'ThresholdClassifier',
-    'RegressionPlot'
+    'RegressionPlot',
+    'CorrelationAnalysis'
 ]
```

### Comparing `nalyst-0.2.3/nalyst.egg-info/PKG-INFO` & `nalyst-0.2.4/nalyst.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.3
+Version: 0.2.4
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -74,14 +74,16 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
+from nalyst.CorrelationAnalysis import correlation_analysis
+from nalyst.TrendAnalyst import linear_regression_trend, LinearRegressionVisualizer
 ```
 
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION
```

### Comparing `nalyst-0.2.3/nalyst.egg-info/SOURCES.txt` & `nalyst-0.2.4/nalyst.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 README.md
 __init__.py
 pyproject.toml
 setup.py
 version.py
 nalyst/BetaFive.py
 nalyst/BetaMax.py
+nalyst/CorrelationAnalysis.py
 nalyst/DecisionTree.py
 nalyst/KMeans.py
 nalyst/LinearRegression.py
 nalyst/LogisticRegression.py
 nalyst/MaxAbsScaler.py
 nalyst/MinMaxScaler.py
 nalyst/MonteCarloSimulator.py
 nalyst/PCA.py
 nalyst/RegressionPlot.py
 nalyst/StandardScaler.py
 nalyst/TestTrainSplit.py
 nalyst/ThresholdClassifier.py
+nalyst/TrendAnalyst.py
 nalyst/__init__.py
 nalyst.egg-info/PKG-INFO
 nalyst.egg-info/SOURCES.txt
 nalyst.egg-info/dependency_links.txt
 nalyst.egg-info/requires.txt
 nalyst.egg-info/top_level.txt
```

### Comparing `nalyst-0.2.3/setup.py` & `nalyst-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.2.3',
+    version='0.2.4',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

