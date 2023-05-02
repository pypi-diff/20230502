# Comparing `tmp/pandas_dq-1.8.tar.gz` & `tmp/pandas_dq-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_dq-1.8.tar", last modified: Fri Apr  7 22:22:56 2023, max compression
+gzip compressed data, was "pandas_dq-1.9.tar", last modified: Fri Apr 14 01:05:04 2023, max compression
```

## Comparing `pandas_dq-1.8.tar` & `pandas_dq-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 22:22:56.949926 pandas_dq-1.8/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11357 2023-04-02 23:27:15.000000 pandas_dq-1.8/LICENSE
--rwxrwxrwx   0 ram       (1000) ram       (1000)      610 2022-04-07 23:06:53.000000 pandas_dq-1.8/MANIFEST.in
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11353 2023-04-07 22:22:56.945937 pandas_dq-1.8/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)     9530 2023-04-07 22:10:48.000000 pandas_dq-1.8/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 22:22:56.913926 pandas_dq-1.8/pandas_dq.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11353 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      232 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       49 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       10 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)    44456 2023-04-07 22:17:06.000000 pandas_dq-1.8/pandas_dq.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)       52 2023-04-07 12:15:09.000000 pandas_dq-1.8/requirements.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-07 22:22:56.953927 pandas_dq-1.8/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)      883 2023-04-07 21:49:21.000000 pandas_dq-1.8/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-14 01:05:04.873379 pandas_dq-1.9/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11357 2023-04-02 23:27:15.000000 pandas_dq-1.9/LICENSE
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      610 2022-04-07 23:06:53.000000 pandas_dq-1.9/MANIFEST.in
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13238 2023-04-14 01:05:04.868391 pandas_dq-1.9/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11247 2023-04-13 14:19:40.000000 pandas_dq-1.9/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-14 01:05:04.840371 pandas_dq-1.9/pandas_dq.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13238 2023-04-14 01:05:03.000000 pandas_dq-1.9/pandas_dq.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      232 2023-04-14 01:05:04.000000 pandas_dq-1.9/pandas_dq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-14 01:05:03.000000 pandas_dq-1.9/pandas_dq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       49 2023-04-14 01:05:03.000000 pandas_dq-1.9/pandas_dq.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       10 2023-04-14 01:05:03.000000 pandas_dq-1.9/pandas_dq.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    51909 2023-04-13 16:18:20.000000 pandas_dq-1.9/pandas_dq.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       52 2023-04-07 12:15:09.000000 pandas_dq-1.9/requirements.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-14 01:05:04.876372 pandas_dq-1.9/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      883 2023-04-13 12:07:32.000000 pandas_dq-1.9/setup.py
```

### Comparing `pandas_dq-1.8/LICENSE` & `pandas_dq-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_dq-1.8/MANIFEST.in` & `pandas_dq-1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pandas_dq-1.8/PKG-INFO` & `pandas_dq-1.9/pandas_dq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pandas_dq
-Version: 1.8
+Name: pandas-dq
+Version: 1.9
 Summary: Clean your data using a scikit-learn transformer in a single line of code
 Home-page: https://github.com/AutoViML/pandas_dq
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # pandas_dq
         Analyze and clean your data in a single line of code with a Scikit-Learn compatible Transformer.
         
@@ -18,27 +18,31 @@
         <li><a href="#maintainers">Maintainers</a></li>
         <li><a href="#contributing">Contributing</a></li>
         <li><a href="#license">License</a></li>
         </ul>
         <p>
         
         ## Introduction
+        `pandas_dq` is a new python library for data quality analysis and improvement. It is fast, efficient and scalable. 
+        
+        <b>Alert!</b>: If you are using `pandas version 2.0` ("the new pandas"), beware that weird errors are popping up in all kinds of libraries that use pandas underneath. Our `pandas_dq` library is no exception. So if you plan to use `pandas_dq` with `pandas version 2.0`, beware that you may see weird errors and we can't and won't fix them!
+        
         ### What is pandas_dq?
-        `pandas_dq` is a new python library for automatically cleaning your dirty dataset using pandas scikit_learn functions. You can analyze your dataset and fix them - all in a single line of code!
+        `pandas_dq` is a new python library for automatically cleaning your dirty dataset using pandas scikit_learn functions. You can analyze your dataset and fix them - all in a single line of code! Recent addition: pandas_dq can check your dataset data types against a specific schema.
         
         ![pandas_dq](./images/pandas_dq_logo.png)
         
         ## Uses
-        `pandas_dq` has two important modules: `dq_report` and `Fix_DQ`. 
+        `pandas_dq` has multiple important modules: `dq_report`, `Fix_DQ` and now `DataSchemeChecker`. <br>
         
         ### 1.  dq_report function
         
         ![dq_report_code](./images/find_dq_screenshot.png)
         
-        <p>`dq_report` is a function that is the most popular way to use pandas_dq and it performs following data quality analysis steps:
+        <p>`dq_report` prints a data quality report after it analyzes your dataset for the issues:
         <ol>
         <li>It detects ID columns</li>
         <li>It detects zero-variance columns </li>
         <li>It identifies rare categories (less than 5% of categories in a column)</li>
         <li>It finds infinite values in a column</li>
         <li>It detects mixed data types (i.e. a column that has more than a single data type)</li>
         <li>It detects outliers (i.e. a float column that is beyond the Inter Quartile Range)</li>
@@ -70,18 +74,35 @@
         <li>It detects duplicate rows and drops one of them or keeps only one copy of duplicate rows</li>
         <li>It detects duplicate columns and drops one of them or keeps only one copy</li>
         <li>It detects skewed distributions and applies log or box-cox transformations on them </li>
         <li>It detects imbalanced classes and leaves them as it is </li>
         <li>It detects feature leakage and drops one of those features if they are highly correlated to target </li>
         </ol>
         
-        
-        ###  How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
+        <b>How can we use Fix_DQ in GridSearchCV to find the best model pipeline?</b>
         <p>This is another way to find the best data cleaning steps for your train data and then use the cleaned data in hyper parameter tuning using GridSearchCV or RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.<br>
         
+        ### 3.  DataSchemaChecker class: a scikit_learn transformer that can check if a pandas dataframe conforms to a given schema and transform it.
+        The class has two methods: fit and transform. You need to initialize the class with a schema that you want to compare your data's dtypes against. A schema is a dictionary that maps column names to data types. 
+        
+        ```
+                Example of a schema: all python dtypes must be surrounded by quote strings.
+                {'name': 'string',
+                 'age': 'float32',
+                 'gender': 'object',
+                 'income': 'float64',
+                 'target': 'integer'}
+        ```
+        
+        The fit method takes a dataframe as an argument and checks if it matches the schema. The fit method first checks if the number of columns in the dataframe and the schema are equal. If not, it creates an exception. Finally, the fit method prints a table of exceptions it found in your data against the given schema. 
+        
+        The transform method takes a dataframe as n argument and based on the given schema and the exceptions, converts all the exception data columns to the given schema. If not, it skips the column and prints out an error message.
+        
+        ![dq_ds](./images/data_schema_checker.png)
+        
         ## Install
         <p>
         
         **Prerequsites:**
         <ol>
         <li><b>pandas_dq is built using pandas, numpy and scikit-learn - that's all.</b> It should run on almost all Python3 Anaconda installations without additional installs. You won't have to import any special libraries.</li>
         </ol>
```

#### html2text {}

```diff
@@ -1,28 +1,35 @@
-Metadata-Version: 2.1 Name: pandas_dq Version: 1.8 Summary: Clean your data
+Metadata-Version: 2.1 Name: pandas-dq Version: 1.9 Summary: Clean your data
 using a scikit-learn transformer in a single line of code Home-page: https://
 github.com/AutoViML/pandas_dq Author: Ram Seshadri License: Apache License 2.0
 Description: # pandas_dq Analyze and clean your data in a single line of code
 with a Scikit-Learn compatible Transformer. # Table of Contents
     * What_is_pandas_dq
     * How_to_use_pandas_dq
     * How_to_install_pandas_dq
     * Usage
     * API
     * Maintainers
     * Contributing
     * License
-## Introduction ### What is pandas_dq? `pandas_dq` is a new python library for
-automatically cleaning your dirty dataset using pandas scikit_learn functions.
-You can analyze your dataset and fix them - all in a single line of code! !
-[pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has two important
-modules: `dq_report` and `Fix_DQ`. ### 1. dq_report function ![dq_report_code]
-(./images/find_dq_screenshot.png)
-`dq_report` is a function that is the most popular way to use pandas_dq and it
-performs following data quality analysis steps:
+## Introduction `pandas_dq` is a new python library for data quality analysis
+and improvement. It is fast, efficient and scalable. Alert!: If you are using
+`pandas version 2.0` ("the new pandas"), beware that weird errors are popping
+up in all kinds of libraries that use pandas underneath. Our `pandas_dq`
+library is no exception. So if you plan to use `pandas_dq` with `pandas version
+2.0`, beware that you may see weird errors and we can't and won't fix them! ###
+What is pandas_dq? `pandas_dq` is a new python library for automatically
+cleaning your dirty dataset using pandas scikit_learn functions. You can
+analyze your dataset and fix them - all in a single line of code! Recent
+addition: pandas_dq can check your dataset data types against a specific
+schema. ![pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has
+multiple important modules: `dq_report`, `Fix_DQ` and now `DataSchemeChecker`.
+### 1. dq_report function ![dq_report_code](./images/find_dq_screenshot.png)
+`dq_report` prints a data quality report after it analyzes your dataset for the
+issues:
    1. It detects ID columns
    2. It detects zero-variance columns
    3. It identifies rare categories (less than 5% of categories in a column)
    4. It finds infinite values in a column
    5. It detects mixed data types (i.e. a column that has more than a single
       data type)
    6. It detects outliers (i.e. a float column that is beyond the Inter
@@ -68,19 +75,33 @@
       duplicate rows
   10. It detects duplicate columns and drops one of them or keeps only one copy
   11. It detects skewed distributions and applies log or box-cox
       transformations on them
   12. It detects imbalanced classes and leaves them as it is
   13. It detects feature leakage and drops one of those features if they are
       highly correlated to target
-### How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
+How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
 This is another way to find the best data cleaning steps for your train data
 and then use the cleaned data in hyper parameter tuning using GridSearchCV or
 RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.
-## Install
+### 3. DataSchemaChecker class: a scikit_learn transformer that can check if a
+pandas dataframe conforms to a given schema and transform it. The class has two
+methods: fit and transform. You need to initialize the class with a schema that
+you want to compare your data's dtypes against. A schema is a dictionary that
+maps column names to data types. ``` Example of a schema: all python dtypes
+must be surrounded by quote strings. {'name': 'string', 'age': 'float32',
+'gender': 'object', 'income': 'float64', 'target': 'integer'} ``` The fit
+method takes a dataframe as an argument and checks if it matches the schema.
+The fit method first checks if the number of columns in the dataframe and the
+schema are equal. If not, it creates an exception. Finally, the fit method
+prints a table of exceptions it found in your data against the given schema.
+The transform method takes a dataframe as n argument and based on the given
+schema and the exceptions, converts all the exception data columns to the given
+schema. If not, it skips the column and prints out an error message. ![dq_ds]
+(./images/data_schema_checker.png) ## Install
 **Prerequsites:**
    1. pandas_dq is built using pandas, numpy and scikit-learn - that's all. It
       should run on almost all Python3 Anaconda installations without
       additional installs. You won't have to import any special libraries.
 The best method to install pandas_dq is to use pip:
 ``` pip install pandas_dq ``` To install from source: ``` cd  git clone
 git@github.com:AutoViML/pandas_dq.git ``` or download and unzip https://
```

### Comparing `pandas_dq-1.8/README.md` & `pandas_dq-1.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 <li><a href="#maintainers">Maintainers</a></li>
 <li><a href="#contributing">Contributing</a></li>
 <li><a href="#license">License</a></li>
 </ul>
 <p>
 
 ## Introduction
+`pandas_dq` is a new python library for data quality analysis and improvement. It is fast, efficient and scalable. 
+
+<b>Alert!</b>: If you are using `pandas version 2.0` ("the new pandas"), beware that weird errors are popping up in all kinds of libraries that use pandas underneath. Our `pandas_dq` library is no exception. So if you plan to use `pandas_dq` with `pandas version 2.0`, beware that you may see weird errors and we can't and won't fix them!
+
 ### What is pandas_dq?
-`pandas_dq` is a new python library for automatically cleaning your dirty dataset using pandas scikit_learn functions. You can analyze your dataset and fix them - all in a single line of code!
+`pandas_dq` is a new python library for automatically cleaning your dirty dataset using pandas scikit_learn functions. You can analyze your dataset and fix them - all in a single line of code! Recent addition: pandas_dq can check your dataset data types against a specific schema.
 
 ![pandas_dq](./images/pandas_dq_logo.png)
 
 ## Uses
-`pandas_dq` has two important modules: `dq_report` and `Fix_DQ`. 
+`pandas_dq` has multiple important modules: `dq_report`, `Fix_DQ` and now `DataSchemeChecker`. <br>
 
 ### 1.  dq_report function
 
 ![dq_report_code](./images/find_dq_screenshot.png)
 
-<p>`dq_report` is a function that is the most popular way to use pandas_dq and it performs following data quality analysis steps:
+<p>`dq_report` prints a data quality report after it analyzes your dataset for the issues:
 <ol>
 <li>It detects ID columns</li>
 <li>It detects zero-variance columns </li>
 <li>It identifies rare categories (less than 5% of categories in a column)</li>
 <li>It finds infinite values in a column</li>
 <li>It detects mixed data types (i.e. a column that has more than a single data type)</li>
 <li>It detects outliers (i.e. a float column that is beyond the Inter Quartile Range)</li>
@@ -63,18 +67,35 @@
 <li>It detects duplicate rows and drops one of them or keeps only one copy of duplicate rows</li>
 <li>It detects duplicate columns and drops one of them or keeps only one copy</li>
 <li>It detects skewed distributions and applies log or box-cox transformations on them </li>
 <li>It detects imbalanced classes and leaves them as it is </li>
 <li>It detects feature leakage and drops one of those features if they are highly correlated to target </li>
 </ol>
 
-
-###  How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
+<b>How can we use Fix_DQ in GridSearchCV to find the best model pipeline?</b>
 <p>This is another way to find the best data cleaning steps for your train data and then use the cleaned data in hyper parameter tuning using GridSearchCV or RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.<br>
 
+### 3.  DataSchemaChecker class: a scikit_learn transformer that can check if a pandas dataframe conforms to a given schema and transform it.
+The class has two methods: fit and transform. You need to initialize the class with a schema that you want to compare your data's dtypes against. A schema is a dictionary that maps column names to data types. 
+
+```
+        Example of a schema: all python dtypes must be surrounded by quote strings.
+        {'name': 'string',
+         'age': 'float32',
+         'gender': 'object',
+         'income': 'float64',
+         'target': 'integer'}
+```
+
+The fit method takes a dataframe as an argument and checks if it matches the schema. The fit method first checks if the number of columns in the dataframe and the schema are equal. If not, it creates an exception. Finally, the fit method prints a table of exceptions it found in your data against the given schema. 
+
+The transform method takes a dataframe as n argument and based on the given schema and the exceptions, converts all the exception data columns to the given schema. If not, it skips the column and prints out an error message.
+
+![dq_ds](./images/data_schema_checker.png)
+
 ## Install
 <p>
 
 **Prerequsites:**
 <ol>
 <li><b>pandas_dq is built using pandas, numpy and scikit-learn - that's all.</b> It should run on almost all Python3 Anaconda installations without additional installs. You won't have to import any special libraries.</li>
 </ol>
```

#### html2text {}

```diff
@@ -4,22 +4,29 @@
     * How_to_use_pandas_dq
     * How_to_install_pandas_dq
     * Usage
     * API
     * Maintainers
     * Contributing
     * License
-## Introduction ### What is pandas_dq? `pandas_dq` is a new python library for
-automatically cleaning your dirty dataset using pandas scikit_learn functions.
-You can analyze your dataset and fix them - all in a single line of code! !
-[pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has two important
-modules: `dq_report` and `Fix_DQ`. ### 1. dq_report function ![dq_report_code]
-(./images/find_dq_screenshot.png)
-`dq_report` is a function that is the most popular way to use pandas_dq and it
-performs following data quality analysis steps:
+## Introduction `pandas_dq` is a new python library for data quality analysis
+and improvement. It is fast, efficient and scalable. Alert!: If you are using
+`pandas version 2.0` ("the new pandas"), beware that weird errors are popping
+up in all kinds of libraries that use pandas underneath. Our `pandas_dq`
+library is no exception. So if you plan to use `pandas_dq` with `pandas version
+2.0`, beware that you may see weird errors and we can't and won't fix them! ###
+What is pandas_dq? `pandas_dq` is a new python library for automatically
+cleaning your dirty dataset using pandas scikit_learn functions. You can
+analyze your dataset and fix them - all in a single line of code! Recent
+addition: pandas_dq can check your dataset data types against a specific
+schema. ![pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has
+multiple important modules: `dq_report`, `Fix_DQ` and now `DataSchemeChecker`.
+### 1. dq_report function ![dq_report_code](./images/find_dq_screenshot.png)
+`dq_report` prints a data quality report after it analyzes your dataset for the
+issues:
    1. It detects ID columns
    2. It detects zero-variance columns
    3. It identifies rare categories (less than 5% of categories in a column)
    4. It finds infinite values in a column
    5. It detects mixed data types (i.e. a column that has more than a single
       data type)
    6. It detects outliers (i.e. a float column that is beyond the Inter
@@ -65,19 +72,33 @@
       duplicate rows
   10. It detects duplicate columns and drops one of them or keeps only one copy
   11. It detects skewed distributions and applies log or box-cox
       transformations on them
   12. It detects imbalanced classes and leaves them as it is
   13. It detects feature leakage and drops one of those features if they are
       highly correlated to target
-### How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
+How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
 This is another way to find the best data cleaning steps for your train data
 and then use the cleaned data in hyper parameter tuning using GridSearchCV or
 RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.
-## Install
+### 3. DataSchemaChecker class: a scikit_learn transformer that can check if a
+pandas dataframe conforms to a given schema and transform it. The class has two
+methods: fit and transform. You need to initialize the class with a schema that
+you want to compare your data's dtypes against. A schema is a dictionary that
+maps column names to data types. ``` Example of a schema: all python dtypes
+must be surrounded by quote strings. {'name': 'string', 'age': 'float32',
+'gender': 'object', 'income': 'float64', 'target': 'integer'} ``` The fit
+method takes a dataframe as an argument and checks if it matches the schema.
+The fit method first checks if the number of columns in the dataframe and the
+schema are equal. If not, it creates an exception. Finally, the fit method
+prints a table of exceptions it found in your data against the given schema.
+The transform method takes a dataframe as n argument and based on the given
+schema and the exceptions, converts all the exception data columns to the given
+schema. If not, it skips the column and prints out an error message. ![dq_ds]
+(./images/data_schema_checker.png) ## Install
 **Prerequsites:**
    1. pandas_dq is built using pandas, numpy and scikit-learn - that's all. It
       should run on almost all Python3 Anaconda installations without
       additional installs. You won't have to import any special libraries.
 The best method to install pandas_dq is to use pip:
 ``` pip install pandas_dq ``` To install from source: ``` cd  git clone
 git@github.com:AutoViML/pandas_dq.git ``` or download and unzip https://
```

### Comparing `pandas_dq-1.8/pandas_dq.egg-info/PKG-INFO` & `pandas_dq-1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pandas-dq
-Version: 1.8
+Name: pandas_dq
+Version: 1.9
 Summary: Clean your data using a scikit-learn transformer in a single line of code
 Home-page: https://github.com/AutoViML/pandas_dq
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # pandas_dq
         Analyze and clean your data in a single line of code with a Scikit-Learn compatible Transformer.
         
@@ -18,27 +18,31 @@
         <li><a href="#maintainers">Maintainers</a></li>
         <li><a href="#contributing">Contributing</a></li>
         <li><a href="#license">License</a></li>
         </ul>
         <p>
         
         ## Introduction
+        `pandas_dq` is a new python library for data quality analysis and improvement. It is fast, efficient and scalable. 
+        
+        <b>Alert!</b>: If you are using `pandas version 2.0` ("the new pandas"), beware that weird errors are popping up in all kinds of libraries that use pandas underneath. Our `pandas_dq` library is no exception. So if you plan to use `pandas_dq` with `pandas version 2.0`, beware that you may see weird errors and we can't and won't fix them!
+        
         ### What is pandas_dq?
-        `pandas_dq` is a new python library for automatically cleaning your dirty dataset using pandas scikit_learn functions. You can analyze your dataset and fix them - all in a single line of code!
+        `pandas_dq` is a new python library for automatically cleaning your dirty dataset using pandas scikit_learn functions. You can analyze your dataset and fix them - all in a single line of code! Recent addition: pandas_dq can check your dataset data types against a specific schema.
         
         ![pandas_dq](./images/pandas_dq_logo.png)
         
         ## Uses
-        `pandas_dq` has two important modules: `dq_report` and `Fix_DQ`. 
+        `pandas_dq` has multiple important modules: `dq_report`, `Fix_DQ` and now `DataSchemeChecker`. <br>
         
         ### 1.  dq_report function
         
         ![dq_report_code](./images/find_dq_screenshot.png)
         
-        <p>`dq_report` is a function that is the most popular way to use pandas_dq and it performs following data quality analysis steps:
+        <p>`dq_report` prints a data quality report after it analyzes your dataset for the issues:
         <ol>
         <li>It detects ID columns</li>
         <li>It detects zero-variance columns </li>
         <li>It identifies rare categories (less than 5% of categories in a column)</li>
         <li>It finds infinite values in a column</li>
         <li>It detects mixed data types (i.e. a column that has more than a single data type)</li>
         <li>It detects outliers (i.e. a float column that is beyond the Inter Quartile Range)</li>
@@ -70,18 +74,35 @@
         <li>It detects duplicate rows and drops one of them or keeps only one copy of duplicate rows</li>
         <li>It detects duplicate columns and drops one of them or keeps only one copy</li>
         <li>It detects skewed distributions and applies log or box-cox transformations on them </li>
         <li>It detects imbalanced classes and leaves them as it is </li>
         <li>It detects feature leakage and drops one of those features if they are highly correlated to target </li>
         </ol>
         
-        
-        ###  How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
+        <b>How can we use Fix_DQ in GridSearchCV to find the best model pipeline?</b>
         <p>This is another way to find the best data cleaning steps for your train data and then use the cleaned data in hyper parameter tuning using GridSearchCV or RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.<br>
         
+        ### 3.  DataSchemaChecker class: a scikit_learn transformer that can check if a pandas dataframe conforms to a given schema and transform it.
+        The class has two methods: fit and transform. You need to initialize the class with a schema that you want to compare your data's dtypes against. A schema is a dictionary that maps column names to data types. 
+        
+        ```
+                Example of a schema: all python dtypes must be surrounded by quote strings.
+                {'name': 'string',
+                 'age': 'float32',
+                 'gender': 'object',
+                 'income': 'float64',
+                 'target': 'integer'}
+        ```
+        
+        The fit method takes a dataframe as an argument and checks if it matches the schema. The fit method first checks if the number of columns in the dataframe and the schema are equal. If not, it creates an exception. Finally, the fit method prints a table of exceptions it found in your data against the given schema. 
+        
+        The transform method takes a dataframe as n argument and based on the given schema and the exceptions, converts all the exception data columns to the given schema. If not, it skips the column and prints out an error message.
+        
+        ![dq_ds](./images/data_schema_checker.png)
+        
         ## Install
         <p>
         
         **Prerequsites:**
         <ol>
         <li><b>pandas_dq is built using pandas, numpy and scikit-learn - that's all.</b> It should run on almost all Python3 Anaconda installations without additional installs. You won't have to import any special libraries.</li>
         </ol>
```

#### html2text {}

```diff
@@ -1,28 +1,35 @@
-Metadata-Version: 2.1 Name: pandas-dq Version: 1.8 Summary: Clean your data
+Metadata-Version: 2.1 Name: pandas_dq Version: 1.9 Summary: Clean your data
 using a scikit-learn transformer in a single line of code Home-page: https://
 github.com/AutoViML/pandas_dq Author: Ram Seshadri License: Apache License 2.0
 Description: # pandas_dq Analyze and clean your data in a single line of code
 with a Scikit-Learn compatible Transformer. # Table of Contents
     * What_is_pandas_dq
     * How_to_use_pandas_dq
     * How_to_install_pandas_dq
     * Usage
     * API
     * Maintainers
     * Contributing
     * License
-## Introduction ### What is pandas_dq? `pandas_dq` is a new python library for
-automatically cleaning your dirty dataset using pandas scikit_learn functions.
-You can analyze your dataset and fix them - all in a single line of code! !
-[pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has two important
-modules: `dq_report` and `Fix_DQ`. ### 1. dq_report function ![dq_report_code]
-(./images/find_dq_screenshot.png)
-`dq_report` is a function that is the most popular way to use pandas_dq and it
-performs following data quality analysis steps:
+## Introduction `pandas_dq` is a new python library for data quality analysis
+and improvement. It is fast, efficient and scalable. Alert!: If you are using
+`pandas version 2.0` ("the new pandas"), beware that weird errors are popping
+up in all kinds of libraries that use pandas underneath. Our `pandas_dq`
+library is no exception. So if you plan to use `pandas_dq` with `pandas version
+2.0`, beware that you may see weird errors and we can't and won't fix them! ###
+What is pandas_dq? `pandas_dq` is a new python library for automatically
+cleaning your dirty dataset using pandas scikit_learn functions. You can
+analyze your dataset and fix them - all in a single line of code! Recent
+addition: pandas_dq can check your dataset data types against a specific
+schema. ![pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has
+multiple important modules: `dq_report`, `Fix_DQ` and now `DataSchemeChecker`.
+### 1. dq_report function ![dq_report_code](./images/find_dq_screenshot.png)
+`dq_report` prints a data quality report after it analyzes your dataset for the
+issues:
    1. It detects ID columns
    2. It detects zero-variance columns
    3. It identifies rare categories (less than 5% of categories in a column)
    4. It finds infinite values in a column
    5. It detects mixed data types (i.e. a column that has more than a single
       data type)
    6. It detects outliers (i.e. a float column that is beyond the Inter
@@ -68,19 +75,33 @@
       duplicate rows
   10. It detects duplicate columns and drops one of them or keeps only one copy
   11. It detects skewed distributions and applies log or box-cox
       transformations on them
   12. It detects imbalanced classes and leaves them as it is
   13. It detects feature leakage and drops one of those features if they are
       highly correlated to target
-### How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
+How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
 This is another way to find the best data cleaning steps for your train data
 and then use the cleaned data in hyper parameter tuning using GridSearchCV or
 RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.
-## Install
+### 3. DataSchemaChecker class: a scikit_learn transformer that can check if a
+pandas dataframe conforms to a given schema and transform it. The class has two
+methods: fit and transform. You need to initialize the class with a schema that
+you want to compare your data's dtypes against. A schema is a dictionary that
+maps column names to data types. ``` Example of a schema: all python dtypes
+must be surrounded by quote strings. {'name': 'string', 'age': 'float32',
+'gender': 'object', 'income': 'float64', 'target': 'integer'} ``` The fit
+method takes a dataframe as an argument and checks if it matches the schema.
+The fit method first checks if the number of columns in the dataframe and the
+schema are equal. If not, it creates an exception. Finally, the fit method
+prints a table of exceptions it found in your data against the given schema.
+The transform method takes a dataframe as n argument and based on the given
+schema and the exceptions, converts all the exception data columns to the given
+schema. If not, it skips the column and prints out an error message. ![dq_ds]
+(./images/data_schema_checker.png) ## Install
 **Prerequsites:**
    1. pandas_dq is built using pandas, numpy and scikit-learn - that's all. It
       should run on almost all Python3 Anaconda installations without
       additional installs. You won't have to import any special libraries.
 The best method to install pandas_dq is to use pip:
 ``` pip install pandas_dq ``` To install from source: ``` cd  git clone
 git@github.com:AutoViML/pandas_dq.git ``` or download and unzip https://
```

### Comparing `pandas_dq-1.8/pandas_dq.py` & `pandas_dq-1.9/pandas_dq.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,20 +96,34 @@
         else:
             print("Unsupported file format. Please use CSV, parquet, feather or arrow.")
             return data
         ######## This is to sample the data if it is too large ###
         if df.shape[0] >= 1000000:
             df = df.sample(100000)
     elif isinstance(data, pd.DataFrame):
-        print("We use the input dataframe as is...")
         df = data
     else:
         print("Invalid input. Please provide a string (filename) or a dataframe.")
         return
 
+    # Drop duplicate rows
+    dup_rows = df.duplicated().sum()
+    if dup_rows > 0:
+        print(f'Alert: Dropping {dup_rows} duplicate rows can sometimes cause column data types to change to object. Double-check!')
+        df = df.drop_duplicates()
+    
+    # Drop duplicate columns
+    dup_cols = df.columns[df.columns.duplicated()]
+    if len(dup_cols) > 0:
+        print(f'Alert: Dropping {len(dup_cols)} duplicate cols which can cause column data types to change to object. Double-check!')
+        ### DO NOT MODIFY THIS LINE. TOOK A LONG TIME TO MAKE IT WORK!!!
+        ###  THis is the only way that dropping duplicate columns works. This is not found anywhere!
+        df = df.T[df.T.index.duplicated(keep='first')].T
+
+
     ### This is the column that lists our data quality issues
     new_col = 'DQ Issue'
     good_col = "The Good News"
     bad_col = "The Bad News"
 
     # Create an empty dataframe to store the data quality issues
     dq_df1 = pd.DataFrame(columns=[good_col, bad_col])
@@ -168,14 +182,33 @@
     ### now generate the data quality starter dataframe
     dq_df2 = data_types.join(missing_data).join(unique_values).join(minimum_values).join(maximum_values)
 
     ### set up additional columns    
     dq_df2["first_comma"] = ""
     dq_df2[new_col] = f""
     
+    #### This is the first thing you need to do ###############
+    if dup_rows > 0:
+        new_string =  f"There are {dup_rows} duplicate columns in the dataset. Keep only one copy of them."
+        dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
+        dq_df1.loc[bad_col,'first_comma'] = ', '
+    else:
+        new_string =  f"There are no duplicate rows in this dataset"
+        dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
+        dq_df1.loc[good_col,'first_comma'] = ', '
+    ### DO NOT CHANGE THE NEXT LINE. The logic for columns is different. 
+    if len(dup_cols) > 0:
+        new_string =  f"There are {len(dup_cols)} duplicate columns in the dataset. Keep only one copy of {dup_cols}."
+        dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
+        dq_df1.loc[bad_col,'first_comma'] = ', '
+    else:
+        new_string =  f"There are no duplicate columns in this datatset"
+        dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
+        dq_df1.loc[good_col,'first_comma'] = ', '
+
     # Detect ID columns in dataset and recommend removing them
     if len(id_cols) > 0:
         new_string = f"There are ID columns in the dataset. Recommend removing them before modeling."
         dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
         dq_df1.loc[bad_col,'first_comma'] = ', '
         for col in id_cols:
             # Append a row to the dq_df1 with the column name and the issue only if the column has a missing value
@@ -279,34 +312,14 @@
                 dq_df2.loc[col,'first_comma'] = ', '
     else:
         new_string =  f"There are no columns with mixed (more than one) dataypes in this dataset"
         dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
         dq_df1.loc[good_col,'first_comma'] = ', '
 
                 
-    # Detect duplicate rows and columns
-    dup_rows = df.duplicated().sum()
-    dup_cols = df.T.duplicated().sum()
-    if dup_rows > 0:
-        new_string =  f"There are {len(dup_rows)} duplicate columns in the dataset. Keep only one copy of {dup_rows}."
-        dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
-        dq_df1.loc[bad_col,'first_comma'] = ', '
-    else:
-        new_string =  f"There are no duplicate rows in this dataset"
-        dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
-        dq_df1.loc[good_col,'first_comma'] = ', '
-    if dup_cols > 0:
-        new_string =  f"There are {len(dup_cols)} duplicate columns in the dataset. Keep only one copy of {dup_cols}."
-        dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
-        dq_df1.loc[bad_col,'first_comma'] = ', '
-    else:
-        new_string =  f"There are no duplicate columns in this datatset"
-        dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
-        dq_df1.loc[good_col,'first_comma'] = ', '
-
     # Detect outliers in numeric cols
     num_cols = df.select_dtypes(include=["int", "float"]).columns.tolist() # Get numerical columns
     if len(num_cols) > 0:
         first_time = True
         outlier_cols = []
         for col in num_cols:
             q1 = df[col].quantile(0.25) # Get the first quartile
@@ -601,32 +614,57 @@
             if col in self.upper_bounds_:
                 # Replace the infinite values with the upper bound
                 X[col] = X[col].replace([np.inf, -np.inf], self.upper_bounds_[col])
         
         # Return the DataFrame with replaced infinite values
         return X
 
+    def detect_duplicates(self, X):
+        # Check if X is a pandas DataFrame
+        if not isinstance(X, pd.DataFrame):
+            # Convert X to a pandas DataFrame
+            X = pd.DataFrame(X)
+        
+        # Drop duplicate rows
+        dup_rows = X.duplicated().sum()
+        if dup_rows > 0:
+            print(f'Alert: Detecting {dup_rows} duplicate rows...')
+        
+        # Drop duplicate columns
+        dup_cols = X.columns[X.columns.duplicated()]
+        ### Remember that the logic for columns is different. Don't change this line!
+        if len(dup_cols) > 0:
+            print(f'Alert: Detecting {len(dup_cols)} duplicate cols...')
+            ### DO NOT TOUCH THIS LINE!! IT TOOK A LONG TIME TO MAKE IT WORK!!
+            ### Also if you don't delete these columns, then nothing after this line will work!
+            X = X.T[X.T.index.duplicated(keep='first')].T
+        
+        # Return the DataFrame with no duplicates
+        return X
+
     # Define a function to detect duplicate rows and columns and keep only one copy
-    def drop_duplicates(self, X):
+    def drop_duplicated(self, X):
         # Check if X is a pandas DataFrame
         if not isinstance(X, pd.DataFrame):
             # Convert X to a pandas DataFrame
             X = pd.DataFrame(X)
         
         # Drop duplicate rows
         dup_rows = X.duplicated().sum()
         if dup_rows > 0:
             print(f'Alert: Dropping {dup_rows} duplicate rows can sometimes cause column data types to change to object. Double-check!')
-            X = X.drop_duplicates()
+            X = X.drop_duplicates(keep='first')
         
         # Drop duplicate columns
-        dup_cols = X.T.duplicated().sum()
-        if dup_cols > 0:
-            print(f'Alert: Dropping {dup_cols} duplicate cols can sometimes cause column data types to change to object. Double-check!')
-            X = X.T.drop_duplicates().T
+        dup_cols = X.columns[X.columns.duplicated()]
+        ### Remember that the logic for columns is different. Don't change this line!
+        if len(dup_cols) > 0:
+            print(f'Alert: Dropping {len(dup_cols)} duplicate cols: {dup_cols}!')
+            ### DO NOT TOUCH THIS LINE!! IT TOOK A LONG TIME TO MAKE IT WORK!!
+            X = X.T[X.T.index.duplicated(keep='first')].T
         
         # Return the DataFrame with no duplicates
         return X
     
     # Define a function to detect skewed distributions and apply a proper transformation to the column
     def transform_skewed(self, X):
         # Check if X is a pandas DataFrame
@@ -662,14 +700,17 @@
             X = pd.DataFrame(X)
         
         # Get the numerical columns
         num_cols = X.select_dtypes(include=["int", "float"]).columns.tolist()
         float_cols = X.select_dtypes(include=["float"]).columns.tolist()
         non_float_cols = left_subtract(X.columns, float_cols)
 
+        ### First and foremost you must drop duplicate columns and rows
+        X = self.detect_duplicates(X)
+
         # Detect ID columns
         self.id_cols_ = [column for column in non_float_cols if X[column].nunique() == X.shape[0]]
         if len(self.id_cols_) > 0:
             print(f"{len(self.id_cols_)} ID cols will be dropped from further processing: {self.id_cols_}")
 
         # Detect zero-variance columns
         self.zero_var_cols_ = [column for column in non_float_cols if X[column].nunique() == 1]
@@ -760,14 +801,18 @@
     
     # Define the transform method that calls the cap_outliers and impute_missing functions on the input DataFrame
     def transform(self, X):
         # Check if X is a pandas DataFrame
         if not isinstance(X, pd.DataFrame):
             # Convert X to a pandas DataFrame
             X = pd.DataFrame(X)
+
+        # First find duplicate columns and rows
+        X = self.drop_duplicated(X)
+
         
         ### drop mixed data type columns from further processing ##
         if len(self.id_cols_) > 0:
             X = X.drop(self.id_cols_, axis=1)
 
         ### drop mixed data type columns from further processing ##
         if len(self.zero_var_cols_) > 0:
@@ -788,16 +833,14 @@
             if len(left_subtract(self.drop_corr_cols_,self.mixed_type_cols_)) > 0:
                 extra_cols = left_subtract(self.drop_corr_cols_,self.mixed_type_cols_)
             elif len(left_subtract(self.mixed_type_cols_,drop_corr_cols_)) > 0:
                 extra_cols = left_subtract(self.mixed_type_cols_, self.drop_corr_cols_)
             if len(extra_cols) > 0:
                 X = X.drop(extra_cols, axis=1)
             
-        # find duplicate columns and rows
-        X = self.drop_duplicates(X)
         
         # Call the impute_missing function first and assign it to a new variable 
         imputed_X = self.impute_missing(X)
 
         if self.quantile is None:
             #### Don't do any processing if quantile is set to None ###
             capped_X = copy.deepcopy(imputed_X)
@@ -812,15 +855,146 @@
         rare_X = self.group_rare_categories(infinite_X)
         
         # Call the power transformer function on rare_X and assign it to a new variable 
         transformed_X = self.transform_skewed(rare_X)
                 
         # Return the transformed DataFrame
         return transformed_X
+################################################################################
+from IPython.display import display
+# Import BaseEstimator and TransformerMixin from sklearn
+from sklearn.base import BaseEstimator, TransformerMixin
+import copy
+class DataSchemaChecker(BaseEstimator, TransformerMixin):
+    """
+    A class to check if a pandas dataframe conforms to a given schema.
+
+    Attributes:
+        schema (dict): A dictionary that maps column names to data types.
+    
+    Example of a schema: all python dtypes must be surrounded by quote strings.
+    {'name': 'string',
+     'age': 'float32',
+     'gender': 'object',
+     'income': 'float64',
+     'target': 'integer'}
+
+    Methods:
+        fit(df): Checks if the dataframe matches the schema and prints a table of errors if any.
+    """
+    def __init__(self, schema):
+        """
+        Initializes the DataFrameSchemaChecker object with a schema.
+
+        Args:
+            schema (dict): A dictionary that maps column names to data types.
+            
+        Example of a schema: all python dtypes must be surrounded by quote strings.
+        {'name': 'string',
+         'age': 'float32',
+         'gender': 'object',
+         'income': 'float64',
+         'target': 'integer'}
+        """
+        self.schema = schema
+
+    def fit(self, df):
+        """
+        Checks if the dataframe matches the schema and prints a table of errors if any.
+
+        Args:
+            df (pd.DataFrame): The dataframe to be checked.
+
+        Raises:
+            ValueError: If the number of columns in the dataframe does not match the number of columns in the schema or if the schema contains an invalid data type.
+
+        Returns:
+            None
+        """
+        # Check if the number of columns in the dataframe matches the number of columns in the schema
+        if len(df.columns) != len(self.schema):
+            raise ValueError("The number of columns in the dataframe does not match the number of columns in the schema")
+
+        # Translate the schema to pandas dtypes
+        translated_schema = {}
+        for column, dtype in self.schema.items():
+            if dtype in ["string","object","category", "str"]:
+                translated_schema[column] = "object"
+            elif dtype in ["text","NLP","nlp"]:
+                translated_schema[column] = "object"
+            elif dtype in ["boolean","bool"]:
+                translated_schema[column] = "bool"
+            elif dtype in [ "np.int8", "np.int16", 
+                            "int8", "int16"]:
+                translated_schema[column] = "int16"
+            elif dtype in ["int32", "np.int32"]:
+                translated_schema[column] = "int32"
+            elif dtype in ["integer","int", "int64", "np.int64"]:
+                translated_schema[column] = "int64"
+            elif dtype in ["date"]:
+                translated_schema[column] = "datetime64[ns]"                
+            elif dtype in ["float"]:
+                translated_schema[column] = "float64"
+            elif dtype in ["np.float32", "float32"]: 
+                translated_schema[column] = "float32"
+            elif dtype in ["np.float64", "float64"]:
+                translated_schema[column] = "float64"
+            else:
+                raise ValueError("Invalid data type: {}".format(dtype))
+
+        # Check if the data types of the columns in the dataframe match the data types in the schema
+        errors = []
+        for column, dtype in translated_schema.items():
+            # Get the actual data type of the column
+            actual_dtype = df[column].dtype
+            # Compare with the expected data type
+            if actual_dtype != dtype:
+                # Append an error message to the list
+                errors.append({
+                    "column": column,
+                    "expected_dtype": dtype,
+                    "actual_dtype": actual_dtype,
+                    "data_dtype_mismatch": "Column '{}' has data type '{}' but expected '{}'".format(
+                        column, actual_dtype, dtype)})
+        
+        # Print a table of errors if there are any
+        if errors:
+            # Create a dataframe from the list of errors
+            self.error_df_ = pd.DataFrame(errors)
+            # Display the dataframe using IPython.display
+            display(self.error_df_)
+        else:
+            print("**No Data Schema Errors**")
+
+        return self
+            
+    def transform(self, df):
+        """
+        Transforms the dataframe dtype to the expected dtype if the dataframe has been fit with DataSchemaChecker
+
+        Args:
+            df (pd.DataFrame): The dataframe to be transformed using DataSchemaChecker's error_df_ variable.
+
+        Raises:
+            Error: If the datatype for a column cannot be transformed as requested.
+
+        Returns:
+            modified dataframe (df)
+        """        
+        df = copy.deepcopy(df)
+        if len(self.error_df_) > 0:
+            # Loop over the rows in the DataFrame.
+            for i, row in self.error_df_.iterrows():
+                column = row['column']
+                try:
+                    df[column] = df[column].astype(self.error_df_["expected_dtype"][0])
+                except:
+                    print(f"Converting {column} to {self.error_df_['expected_dtype'][0]} is erroring. Please convert it yourself.")
+                
+        return df
 
 ############################################################################################
 module_type = 'Running' if  __name__ == "__main__" else 'Imported'
-version_number =  '1.8'
+version_number =  '1.9'
 print(f"""{module_type} pandas_dq ({version_number}). Always upgrade to get latest version.
-from pandas_dq import dq_report, Fix_DQ
 """)
 #################################################################################
```

### Comparing `pandas_dq-1.8/setup.py` & `pandas_dq-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandas_dq",
-    version="1.8",
+    version="1.9",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Clean your data using a scikit-learn transformer in a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/pandas_dq",
```

