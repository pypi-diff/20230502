# Comparing `tmp/nalyst-0.2.5.tar.gz` & `tmp/nalyst-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.2.5.tar", last modified: Tue May  2 15:52:58 2023, max compression
+gzip compressed data, was "nalyst-0.2.6.tar", last modified: Tue May  2 16:17:52 2023, max compression
```

## Comparing `nalyst-0.2.5.tar` & `nalyst-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 15:52:58.510304 nalyst-0.2.5/
--rw-rw-rw-   0        0        0      107 2023-04-21 16:17:56.000000 nalyst-0.2.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.5/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3839 2023-05-02 15:52:58.510304 nalyst-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2723 2023-05-02 15:51:25.000000 nalyst-0.2.5/README.md
--rw-rw-rw-   0        0        0     1221 2023-05-02 15:51:02.000000 nalyst-0.2.5/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 15:52:58.505320 nalyst-0.2.5/nalyst/
--rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.5/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.5/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-0.2.5/nalyst/CorrelationAnalysis.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.5/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.5/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.5/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.5/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.5/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.5/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.5/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.5/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.5/nalyst/RegressionPlot.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.5/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.5/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.5/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-0.2.5/nalyst/TrendAnalyst.py
--rw-rw-rw-   0        0        0     1221 2023-05-02 15:51:19.000000 nalyst-0.2.5/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 15:52:58.509307 nalyst-0.2.5/nalyst.egg-info/
--rw-rw-rw-   0        0        0     3839 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 15:52:58.510304 nalyst-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-05-02 15:52:23.000000 nalyst-0.2.5/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.5/version.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:17:52.926383 nalyst-0.2.6/
+-rw-rw-rw-   0        0        0      146 2023-05-02 16:17:38.000000 nalyst-0.2.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4239 2023-05-02 16:17:52.926383 nalyst-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-05-02 16:16:51.000000 nalyst-0.2.6/README.md
+-rw-rw-rw-   0        0        0     1298 2023-05-02 16:12:27.000000 nalyst-0.2.6/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:17:52.922397 nalyst-0.2.6/nalyst/
+-rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.6/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.6/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-0.2.6/nalyst/CorrelationAnalysis.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.6/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.6/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.6/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.6/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.6/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.6/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.6/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.6/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.6/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.6/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     2333 2023-05-02 16:09:53.000000 nalyst-0.2.6/nalyst/StockVolatility.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.6/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.6/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-0.2.6/nalyst/TrendAnalyst.py
+-rw-rw-rw-   0        0        0     1298 2023-05-02 16:11:56.000000 nalyst-0.2.6/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:17:52.925387 nalyst-0.2.6/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     4239 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:17:52.926383 nalyst-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-05-02 16:17:02.000000 nalyst-0.2.6/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.6/version.py
```

### Comparing `nalyst-0.2.5/LICENSE` & `nalyst-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/PKG-INFO` & `nalyst-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.5
+Version: 0.2.6
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -19,19 +19,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-INTRODUCTION
+1. INTRODUCTION
 
 Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
-FEATURES
+2. FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
 
 Logistic Regression: a range of tools for building and analyzing logistic regression models.
 
 K-means: a tool for clustering data into k clusters.
 
@@ -46,27 +46,37 @@
 MaxAbs Scale: a tool for scaling data to the absolute maximum value of each feature.
 
 Standard Scale: a tool for standardizing data to have a mean of 0 and a standard deviation of 1.
 
 Quick model training: with this library, users can quickly and easily train machine learning models, saving time and effort.
 
 
-INSTALLATION PACKAGE
+3. INSTALLATION PACKAGE
 
 To install the library, simply run the following command in your terminal:
 
 ```text
 pip install nalyst
 
 pip install --upgrade nalyst
 
 pip show nalyst
 ```
+```
+4. IMPORT DEPENDENCY 
 
-IMPORT PACKAGES
+import numpy as np
+import matplotlib.pyplot as plt
+import yfinance as yf
+import pyttsx3
+import seaborn as sns
+import yfinance as yf
+import datetime
+```
+5. IMPORTING PACKAGES
 
 ```text
 from nalyst.LinearRegression import LinearRegression
 from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
 from nalyst.LogisticRegression import LogisticRegression, accuracy
@@ -74,23 +84,25 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.CorrelationAnalysis import LinearRegressionVisualizer
+from nalyst.RegressionPlot import RegressionPlot
+from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
+from nalyst.StockVolatility import stock_volatility
 ```
 
-SUPPORT
+6. SUPPORT
 
-If you need help or have any questions, please feel free to reach out to
+If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
-COMMUNICATION 
+7. COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
 
 YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
 
 Github: https://github.com/harryworlds/nalyst
```

### Comparing `nalyst-0.2.5/README.md` & `nalyst-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-INTRODUCTION
+1. INTRODUCTION
 
 Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
-FEATURES
+2. FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
 
 Logistic Regression: a range of tools for building and analyzing logistic regression models.
 
 K-means: a tool for clustering data into k clusters.
 
@@ -21,27 +21,37 @@
 MaxAbs Scale: a tool for scaling data to the absolute maximum value of each feature.
 
 Standard Scale: a tool for standardizing data to have a mean of 0 and a standard deviation of 1.
 
 Quick model training: with this library, users can quickly and easily train machine learning models, saving time and effort.
 
 
-INSTALLATION PACKAGE
+3. INSTALLATION PACKAGE
 
 To install the library, simply run the following command in your terminal:
 
 ```text
 pip install nalyst
 
 pip install --upgrade nalyst
 
 pip show nalyst
 ```
+```
+4. IMPORT DEPENDENCY 
 
-IMPORT PACKAGES
+import numpy as np
+import matplotlib.pyplot as plt
+import yfinance as yf
+import pyttsx3
+import seaborn as sns
+import yfinance as yf
+import datetime
+```
+5. IMPORTING PACKAGES
 
 ```text
 from nalyst.LinearRegression import LinearRegression
 from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
 from nalyst.LogisticRegression import LogisticRegression, accuracy
@@ -49,23 +59,25 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.CorrelationAnalysis import LinearRegressionVisualizer
+from nalyst.RegressionPlot import RegressionPlot
+from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
+from nalyst.StockVolatility import stock_volatility
 ```
 
-SUPPORT
+6. SUPPORT
 
-If you need help or have any questions, please feel free to reach out to
+If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
-COMMUNICATION 
+7. COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
 
 YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
 
 Github: https://github.com/harryworlds/nalyst
```

### Comparing `nalyst-0.2.5/__init__.py` & `nalyst-0.2.6/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
+from nalyst.StockVolatility import stock_volatility
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -27,9 +28,10 @@
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
     'ThresholdClassifier',
     'LinearCorrelationVisualizer',
-    'LinearRegressionVisualizer'
+    'LinearRegressionVisualizer',
+    'StockVolatility'
 ]
```

### Comparing `nalyst-0.2.5/nalyst/BetaFive.py` & `nalyst-0.2.6/nalyst/BetaFive.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/BetaMax.py` & `nalyst-0.2.6/nalyst/BetaMax.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/CorrelationAnalysis.py` & `nalyst-0.2.6/nalyst/CorrelationAnalysis.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/DecisionTree.py` & `nalyst-0.2.6/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/KMeans.py` & `nalyst-0.2.6/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/LinearRegression.py` & `nalyst-0.2.6/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/LogisticRegression.py` & `nalyst-0.2.6/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/MaxAbsScaler.py` & `nalyst-0.2.6/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/MinMaxScaler.py` & `nalyst-0.2.6/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/MonteCarloSimulator.py` & `nalyst-0.2.6/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/PCA.py` & `nalyst-0.2.6/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/RegressionPlot.py` & `nalyst-0.2.6/nalyst/RegressionPlot.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/StandardScaler.py` & `nalyst-0.2.6/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/TestTrainSplit.py` & `nalyst-0.2.6/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/ThresholdClassifier.py` & `nalyst-0.2.6/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/TrendAnalyst.py` & `nalyst-0.2.6/nalyst/TrendAnalyst.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.5/nalyst/__init__.py` & `nalyst-0.2.6/nalyst/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
+from nalyst.StockVolatility import stock_volatility
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -27,9 +28,10 @@
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
     'ThresholdClassifier',
     'LinearCorrelationVisualizer',
-    'LinearRegressionVisualizer'
+    'LinearRegressionVisualizer',
+    'StockVolatility'
 ]
```

### Comparing `nalyst-0.2.5/nalyst.egg-info/PKG-INFO` & `nalyst-0.2.6/nalyst.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.5
+Version: 0.2.6
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -19,19 +19,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-INTRODUCTION
+1. INTRODUCTION
 
 Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
-FEATURES
+2. FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
 
 Logistic Regression: a range of tools for building and analyzing logistic regression models.
 
 K-means: a tool for clustering data into k clusters.
 
@@ -46,27 +46,37 @@
 MaxAbs Scale: a tool for scaling data to the absolute maximum value of each feature.
 
 Standard Scale: a tool for standardizing data to have a mean of 0 and a standard deviation of 1.
 
 Quick model training: with this library, users can quickly and easily train machine learning models, saving time and effort.
 
 
-INSTALLATION PACKAGE
+3. INSTALLATION PACKAGE
 
 To install the library, simply run the following command in your terminal:
 
 ```text
 pip install nalyst
 
 pip install --upgrade nalyst
 
 pip show nalyst
 ```
+```
+4. IMPORT DEPENDENCY 
 
-IMPORT PACKAGES
+import numpy as np
+import matplotlib.pyplot as plt
+import yfinance as yf
+import pyttsx3
+import seaborn as sns
+import yfinance as yf
+import datetime
+```
+5. IMPORTING PACKAGES
 
 ```text
 from nalyst.LinearRegression import LinearRegression
 from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
 from nalyst.LogisticRegression import LogisticRegression, accuracy
@@ -74,23 +84,25 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.CorrelationAnalysis import LinearRegressionVisualizer
+from nalyst.RegressionPlot import RegressionPlot
+from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
+from nalyst.StockVolatility import stock_volatility
 ```
 
-SUPPORT
+6. SUPPORT
 
-If you need help or have any questions, please feel free to reach out to
+If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
-COMMUNICATION 
+7. COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
 
 YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
 
 Github: https://github.com/harryworlds/nalyst
```

### Comparing `nalyst-0.2.5/nalyst.egg-info/SOURCES.txt` & `nalyst-0.2.6/nalyst.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 nalyst/LogisticRegression.py
 nalyst/MaxAbsScaler.py
 nalyst/MinMaxScaler.py
 nalyst/MonteCarloSimulator.py
 nalyst/PCA.py
 nalyst/RegressionPlot.py
 nalyst/StandardScaler.py
+nalyst/StockVolatility.py
 nalyst/TestTrainSplit.py
 nalyst/ThresholdClassifier.py
 nalyst/TrendAnalyst.py
 nalyst/__init__.py
 nalyst.egg-info/PKG-INFO
 nalyst.egg-info/SOURCES.txt
 nalyst.egg-info/dependency_links.txt
```

### Comparing `nalyst-0.2.5/setup.py` & `nalyst-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.2.5',
+    version='0.2.6',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

