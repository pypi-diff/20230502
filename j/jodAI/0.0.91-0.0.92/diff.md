# Comparing `tmp/jodAI-0.0.91.tar.gz` & `tmp/jodAI-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jodAI-0.0.91.tar", last modified: Mon May  1 22:14:15 2023, max compression
+gzip compressed data, was "jodAI-0.0.92.tar", last modified: Mon May  1 22:17:32 2023, max compression
```

## Comparing `jodAI-0.0.91.tar` & `jodAI-0.0.92.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:14:15.418834 jodAI-0.0.91/
--rw-rw-rw-   0        0        0        0 2023-04-27 20:43:23.000000 jodAI-0.0.91/Licence.txt.txt
--rw-rw-rw-   0        0        0      176 2023-05-01 22:14:15.417833 jodAI-0.0.91/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 22:14:15.409824 jodAI-0.0.91/jodAI/
--rw-rw-rw-   0        0        0    32534 2023-05-01 22:13:11.000000 jodAI-0.0.91/jodAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:14:15.415842 jodAI-0.0.91/jodAI.egg-info/
--rw-rw-rw-   0        0        0      176 2023-05-01 22:14:14.000000 jodAI-0.0.91/jodAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-01 22:14:15.000000 jodAI-0.0.91/jodAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:14:14.000000 jodAI-0.0.91/jodAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 22:14:15.000000 jodAI-0.0.91/jodAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 22:14:15.418834 jodAI-0.0.91/setup.cfg
--rw-rw-rw-   0        0        0      228 2023-05-01 22:14:05.000000 jodAI-0.0.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:17:32.460149 jodAI-0.0.92/
+-rw-rw-rw-   0        0        0        0 2023-04-27 20:43:23.000000 jodAI-0.0.92/Licence.txt.txt
+-rw-rw-rw-   0        0        0      176 2023-05-01 22:17:32.459151 jodAI-0.0.92/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 22:17:32.453140 jodAI-0.0.92/jodAI/
+-rw-rw-rw-   0        0        0    33939 2023-05-01 22:17:19.000000 jodAI-0.0.92/jodAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:17:32.458141 jodAI-0.0.92/jodAI.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-05-01 22:17:31.000000 jodAI-0.0.92/jodAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-05-01 22:17:32.000000 jodAI-0.0.92/jodAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 22:17:31.000000 jodAI-0.0.92/jodAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 22:17:32.000000 jodAI-0.0.92/jodAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 22:17:32.460149 jodAI-0.0.92/setup.cfg
+-rw-rw-rw-   0        0        0      228 2023-05-01 22:17:25.000000 jodAI-0.0.92/setup.py
```

### Comparing `jodAI-0.0.91/jodAI/__init__.py` & `jodAI-0.0.92/jodAI/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -896,8 +896,55 @@
         ans.append(a)
     write(ans)
     # print KB
 
 main()
 
 
+
+
+###################### LINGEAR Regression #############################
+
+
+# Simple Linear Regression
+# Importing the libraries
+import numpy as np
+import matplotlib.pyplot as plt
+import pandas as pd
+
+# Importing the dataset
+dataset = pd.read_csv('https://github.com/krishnaik06/simple-LinearRegression/raw/master/Salary_Data.csv')
+X = dataset.iloc[:, :-1].values
+y = dataset.iloc[:, 1].values
+
+# Splitting the dataset into the Training set and Test set
+from sklearn.model_selection import train_test_split
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size
+= 1/3, random_state = 0)
+# Fitting Simple Linear Regression to the Training set
+from sklearn.linear_model import LinearRegression
+regressor = LinearRegression()
+regressor.fit(X_train, y_train)
+# Predicting the Test set results
+y_pred = regressor.predict(X_test)
+# Visualising the Training set results
+plt.scatter(X_train, y_train, color = 'red')
+plt.plot(X_train, regressor.predict(X_train), color = 'blue')
+[<matplotlib.lines.Line2D at 0x7f16d33fc850>]
+
+
+## run after this ##
+
+# Visualising the Test set results
+# Plot for the TEST
+plt.scatter(X_test, y_test, color = 'red')
+plt.plot(X_train, regressor.predict(X_train), color = 'blue')
+# Ploting the regression line
+plt.title('Salary vs Experience (Test set)')
+plt.xlabel('Years of Experience')
+plt.ylabel('Salary')
+plt.show()
+
+
+
+
 """)
```

