# Comparing `tmp/nalyst-0.2.6.tar.gz` & `tmp/nalyst-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.2.6.tar", last modified: Tue May  2 16:17:52 2023, max compression
+gzip compressed data, was "nalyst-0.2.7.tar", last modified: Tue May  2 16:30:35 2023, max compression
```

## Comparing `nalyst-0.2.6.tar` & `nalyst-0.2.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:17:52.926383 nalyst-0.2.6/
--rw-rw-rw-   0        0        0      146 2023-05-02 16:17:38.000000 nalyst-0.2.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.6/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4239 2023-05-02 16:17:52.926383 nalyst-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-05-02 16:16:51.000000 nalyst-0.2.6/README.md
--rw-rw-rw-   0        0        0     1298 2023-05-02 16:12:27.000000 nalyst-0.2.6/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:17:52.922397 nalyst-0.2.6/nalyst/
--rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.6/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.6/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-0.2.6/nalyst/CorrelationAnalysis.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.6/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.6/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.6/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.6/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.6/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.6/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.6/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.6/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.6/nalyst/RegressionPlot.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.6/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     2333 2023-05-02 16:09:53.000000 nalyst-0.2.6/nalyst/StockVolatility.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.6/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.6/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-0.2.6/nalyst/TrendAnalyst.py
--rw-rw-rw-   0        0        0     1298 2023-05-02 16:11:56.000000 nalyst-0.2.6/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:17:52.925387 nalyst-0.2.6/nalyst.egg-info/
--rw-rw-rw-   0        0        0     4239 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 16:17:52.000000 nalyst-0.2.6/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 16:17:52.926383 nalyst-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-05-02 16:17:02.000000 nalyst-0.2.6/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.6/version.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:30:35.799154 nalyst-0.2.7/
+-rw-rw-rw-   0        0        0      146 2023-05-02 16:17:38.000000 nalyst-0.2.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4239 2023-05-02 16:30:35.798158 nalyst-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-05-02 16:16:51.000000 nalyst-0.2.7/README.md
+-rw-rw-rw-   0        0        0     1298 2023-05-02 16:12:27.000000 nalyst-0.2.7/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:30:35.794171 nalyst-0.2.7/nalyst/
+-rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.7/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.7/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-0.2.7/nalyst/CorrelationAnalysis.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.7/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.7/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.7/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.7/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.7/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.7/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.7/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.7/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.7/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.7/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     2341 2023-05-02 16:29:32.000000 nalyst-0.2.7/nalyst/StockVolatility.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.7/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.7/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-0.2.7/nalyst/TrendAnalyst.py
+-rw-rw-rw-   0        0        0     1298 2023-05-02 16:11:56.000000 nalyst-0.2.7/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:30:35.797161 nalyst-0.2.7/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     4239 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:30:35.799154 nalyst-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-05-02 16:29:45.000000 nalyst-0.2.7/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.7/version.py
```

### Comparing `nalyst-0.2.6/LICENSE` & `nalyst-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/PKG-INFO` & `nalyst-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.2.6/README.md` & `nalyst-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/__init__.py` & `nalyst-0.2.7/__init__.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/BetaFive.py` & `nalyst-0.2.7/nalyst/BetaFive.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/BetaMax.py` & `nalyst-0.2.7/nalyst/BetaMax.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/CorrelationAnalysis.py` & `nalyst-0.2.7/nalyst/CorrelationAnalysis.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/DecisionTree.py` & `nalyst-0.2.7/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/KMeans.py` & `nalyst-0.2.7/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/LinearRegression.py` & `nalyst-0.2.7/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/LogisticRegression.py` & `nalyst-0.2.7/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/MaxAbsScaler.py` & `nalyst-0.2.7/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/MinMaxScaler.py` & `nalyst-0.2.7/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/MonteCarloSimulator.py` & `nalyst-0.2.7/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/PCA.py` & `nalyst-0.2.7/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/RegressionPlot.py` & `nalyst-0.2.7/nalyst/RegressionPlot.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/StandardScaler.py` & `nalyst-0.2.7/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/StockVolatility.py` & `nalyst-0.2.7/nalyst/StockVolatility.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,11 +57,11 @@
     print(result)
     tts = pyttsx3.init()
     tts.setProperty('rate', 160)
     tts.say(result)
     tts.runAndWait()
 
 
-stock = yf.Ticker(str(str(input(" Enter your stock ticker: ").upper())))
-stock = stock.history(period=input(" Enter Number of days (eg 365d): "))
-stock = stock.Close
-stock_volatility(stock)
+# stock = yf.Ticker(str(str(input(" Enter your stock ticker: ").upper())))
+# stock = stock.history(period=input(" Enter Number of days (eg 365d): "))
+# stock = stock.Close
+# stock_volatility(stock)
```

### Comparing `nalyst-0.2.6/nalyst/TestTrainSplit.py` & `nalyst-0.2.7/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/ThresholdClassifier.py` & `nalyst-0.2.7/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/TrendAnalyst.py` & `nalyst-0.2.7/nalyst/TrendAnalyst.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst/__init__.py` & `nalyst-0.2.7/nalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/nalyst.egg-info/PKG-INFO` & `nalyst-0.2.7/nalyst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.2.6/nalyst.egg-info/SOURCES.txt` & `nalyst-0.2.7/nalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.6/setup.py` & `nalyst-0.2.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.2.6',
+    version='0.2.7',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

