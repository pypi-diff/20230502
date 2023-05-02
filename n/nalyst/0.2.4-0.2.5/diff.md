# Comparing `tmp/nalyst-0.2.4.tar.gz` & `tmp/nalyst-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.2.4.tar", last modified: Tue May  2 15:11:28 2023, max compression
+gzip compressed data, was "nalyst-0.2.5.tar", last modified: Tue May  2 15:52:58 2023, max compression
```

## Comparing `nalyst-0.2.4.tar` & `nalyst-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 15:11:28.070153 nalyst-0.2.4/
--rw-rw-rw-   0        0        0      107 2023-04-21 16:17:56.000000 nalyst-0.2.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3858 2023-05-02 15:11:28.070153 nalyst-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2742 2023-05-02 15:10:53.000000 nalyst-0.2.4/README.md
--rw-rw-rw-   0        0        0     1232 2023-05-02 15:09:50.000000 nalyst-0.2.4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 15:11:28.065168 nalyst-0.2.4/nalyst/
--rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.4/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.4/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     3020 2023-05-02 15:09:11.000000 nalyst-0.2.4/nalyst/CorrelationAnalysis.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.4/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.4/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.4/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.4/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.4/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.4/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.4/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.4/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.4/nalyst/RegressionPlot.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.4/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.4/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.4/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0     2771 2023-05-02 15:08:58.000000 nalyst-0.2.4/nalyst/TrendAnalyst.py
--rw-rw-rw-   0        0        0     1232 2023-05-02 15:09:46.000000 nalyst-0.2.4/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 15:11:28.069156 nalyst-0.2.4/nalyst.egg-info/
--rw-rw-rw-   0        0        0     3858 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 15:11:27.000000 nalyst-0.2.4/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 15:11:28.071149 nalyst-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-05-02 15:11:11.000000 nalyst-0.2.4/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.4/version.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:52:58.510304 nalyst-0.2.5/
+-rw-rw-rw-   0        0        0      107 2023-04-21 16:17:56.000000 nalyst-0.2.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3839 2023-05-02 15:52:58.510304 nalyst-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2723 2023-05-02 15:51:25.000000 nalyst-0.2.5/README.md
+-rw-rw-rw-   0        0        0     1221 2023-05-02 15:51:02.000000 nalyst-0.2.5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:52:58.505320 nalyst-0.2.5/nalyst/
+-rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.5/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.5/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-0.2.5/nalyst/CorrelationAnalysis.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.5/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.5/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.5/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.5/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.5/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.5/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.5/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.5/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.5/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.5/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.5/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.5/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-0.2.5/nalyst/TrendAnalyst.py
+-rw-rw-rw-   0        0        0     1221 2023-05-02 15:51:19.000000 nalyst-0.2.5/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:52:58.509307 nalyst-0.2.5/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     3839 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 15:52:58.000000 nalyst-0.2.5/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 15:52:58.510304 nalyst-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-05-02 15:52:23.000000 nalyst-0.2.5/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.5/version.py
```

### Comparing `nalyst-0.2.4/LICENSE` & `nalyst-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/PKG-INFO` & `nalyst-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.4
+Version: 0.2.5
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -74,16 +74,16 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.CorrelationAnalysis import correlation_analysis
-from nalyst.TrendAnalyst import linear_regression_trend, LinearRegressionVisualizer
+from nalyst.CorrelationAnalysis import LinearRegressionVisualizer
+from nalyst.TrendAnalyst import LinearRegressionVisualizer
 ```
 
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION
```

### Comparing `nalyst-0.2.4/README.md` & `nalyst-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.CorrelationAnalysis import correlation_analysis
-from nalyst.TrendAnalyst import linear_regression_trend, LinearRegressionVisualizer
+from nalyst.CorrelationAnalysis import LinearRegressionVisualizer
+from nalyst.TrendAnalyst import LinearRegressionVisualizer
 ```
 
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION
```

### Comparing `nalyst-0.2.4/__init__.py` & `nalyst-0.2.5/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
-from nalyst.CorrelationAnalysis import correlation_analysis
-from nalyst.TrendAnalyst import LinearModel, linear_regression_trend, LinearRegressionVisualizer
+from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
+from nalyst.TrendAnalyst import LinearRegressionVisualizer
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -26,10 +26,10 @@
     'StandardScaler',
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
     'ThresholdClassifier',
-    'RegressionPlot',
-    'CorrelationAnalysis'
+    'LinearCorrelationVisualizer',
+    'LinearRegressionVisualizer'
 ]
```

### Comparing `nalyst-0.2.4/nalyst/BetaFive.py` & `nalyst-0.2.5/nalyst/BetaFive.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/BetaMax.py` & `nalyst-0.2.5/nalyst/BetaMax.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/CorrelationAnalysis.py` & `nalyst-0.2.5/nalyst/CorrelationAnalysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 import matplotlib.pyplot as plt
 import yfinance as yf
 import pyttsx3
 import seaborn as sns
 import yfinance as yf
 import datetime
 
+# stock price
+
 
 class Stock:
     def __init__(self, ticker):
         self.ticker = ticker
 
     def price(self):
         return yf.download(self.ticker)
 
+# LinearModel
+
 
 class LinearModel:
     def LinearRegression(self, x, y):
         n = len(x)
         sum_x = np.sum(x)
         sum_y = np.sum(y)
         sum_xy = np.sum(x * y)
         sum_x2 = np.sum(x ** 2)
         b1 = (n * sum_xy - sum_x * sum_y) / (n * sum_x2 - sum_x ** 2)
         bo = (sum_y - b1 * sum_x) / n
-
         return b1, bo
 
+# Plotting graph
+
 
 class Plot:
     def __init__(self, x, y):
         self.x = x
         self.y = y
 
     def ScatterPlot(self, x_pred, y_pred):
@@ -47,25 +52,28 @@
                         color="white", alpha=0.5, label="Below best-fit line")
         sns.lineplot(x=self.x, y=y_pred, color="yellow", label="Best-fit line")
         plt.xlabel("Stock A")
         plt.ylabel("Stock B")
         plt.grid(color='white', linestyle='--', linewidth=1, alpha=0.5)
         plt.legend()
         plt.show()
+# speech to text model
 
 
 def speech(text):
     engine = pyttsx3.init()
     engine.setProperty('rate', 180)
     engine.setProperty('volume', 1.0)
     engine.say(text)
     engine.runAndWait()
 
+# Linear Regression visualisation Model
 
-class LinearRegressionVisualizer:
+
+class LinearCorrelationVisualizer:
     def __init__(self, stock_a, stock_b):
         self.stock_a = stock_a
         self.stock_b = stock_b
 
     def visualize(self):
         days = 365*2
         stock_data_a = Stock(self.stock_a).price().tail(days)
@@ -79,14 +87,7 @@
         print(f"Slope: {slope}")
         print(f"Intercept: {intercept}")
         y_pred = [intercept + slope * xi for xi in x]
         obj3 = Plot(x, y)
         obj3.ScatterPlot(x, y_pred)
         speech_text = f"The linear model for correlation analysis between {self.stock_a} and {self.stock_b} is showing {trend}."
         speech(speech_text)
-
-
-stock_a = input("Enter the x (Independent Variable): ")
-stock_b = input("Enter the y (Dependent Variable): ")
-correlation_analysis = LinearRegressionVisualizer(
-    stock_a=stock_a, stock_b=stock_b)
-correlation_analysis.visualize()
```

### Comparing `nalyst-0.2.4/nalyst/DecisionTree.py` & `nalyst-0.2.5/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/KMeans.py` & `nalyst-0.2.5/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/LinearRegression.py` & `nalyst-0.2.5/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/LogisticRegression.py` & `nalyst-0.2.5/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/MaxAbsScaler.py` & `nalyst-0.2.5/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/MinMaxScaler.py` & `nalyst-0.2.5/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/MonteCarloSimulator.py` & `nalyst-0.2.5/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/PCA.py` & `nalyst-0.2.5/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/RegressionPlot.py` & `nalyst-0.2.5/nalyst/RegressionPlot.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/StandardScaler.py` & `nalyst-0.2.5/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/TestTrainSplit.py` & `nalyst-0.2.5/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/ThresholdClassifier.py` & `nalyst-0.2.5/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/TrendAnalyst.py` & `nalyst-0.2.5/nalyst/TrendAnalyst.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/nalyst/__init__.py` & `nalyst-0.2.5/nalyst/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
-from nalyst.CorrelationAnalysis import correlation_analysis
-from nalyst.TrendAnalyst import LinearModel, linear_regression_trend, LinearRegressionVisualizer
+from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
+from nalyst.TrendAnalyst import LinearRegressionVisualizer
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -26,10 +26,10 @@
     'StandardScaler',
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
     'ThresholdClassifier',
-    'RegressionPlot',
-    'CorrelationAnalysis'
+    'LinearCorrelationVisualizer',
+    'LinearRegressionVisualizer'
 ]
```

### Comparing `nalyst-0.2.4/nalyst.egg-info/PKG-INFO` & `nalyst-0.2.5/nalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.4
+Version: 0.2.5
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -74,16 +74,16 @@
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.CorrelationAnalysis import correlation_analysis
-from nalyst.TrendAnalyst import linear_regression_trend, LinearRegressionVisualizer
+from nalyst.CorrelationAnalysis import LinearRegressionVisualizer
+from nalyst.TrendAnalyst import LinearRegressionVisualizer
 ```
 
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION
```

### Comparing `nalyst-0.2.4/nalyst.egg-info/SOURCES.txt` & `nalyst-0.2.5/nalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.4/setup.py` & `nalyst-0.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.2.4',
+    version='0.2.5',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

