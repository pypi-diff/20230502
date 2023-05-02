# Comparing `tmp/tunesurvey-0.0.3.tar.gz` & `tmp/tunesurvey-0.0.4.tar.gz`

## Comparing `tunesurvey-0.0.3.tar` & `tunesurvey-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,27 @@
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/demo.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/__init__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/cleansing.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/skLists.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/tsReshape.py
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/ts_torchLists.py
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/vectorized_search_by_term.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/PKG-INFO
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/top_level.txt
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/LICENSE
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/demo.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/demo2.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/setup.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/.ipynb_checkpoints/demo-checkpoint.py
+-rw-r--r--   0        0        0   100995 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/catboost_info/catboost_training.json
+-rw-r--r--   0        0        0    17316 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/catboost_info/learn_error.tsv
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/catboost_info/time_left.tsv
+-rw-r--r--   0        0        0    60870 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/catboost_info/learn/events.out.tfevents
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/__init__.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/boostingLists.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/cleansing.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/forceCollect.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/mathExpand.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/skLists.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/testExpand.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/tsReshape.py
+-rw-r--r--   0        0        0    20242 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/tsVectorize.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/ts_torchLists.py
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/src/tuneSurvey/vectorized_search_by_term.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/tuneSurvey.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/tuneSurvey.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/tuneSurvey.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/tuneSurvey.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 tunesurvey-0.0.4/PKG-INFO
```

### Comparing `tunesurvey-0.0.3/src/tuneSurvey/cleansing.py` & `tunesurvey-0.0.4/src/tuneSurvey/cleansing.py`

 * *Files identical despite different names*

### Comparing `tunesurvey-0.0.3/src/tuneSurvey/skLists.py` & `tunesurvey-0.0.4/src/tuneSurvey/skLists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+"""tune grids for sklearn models
+        note skmodels have model().__class__.__name__
+        and that model() itself can be called m = SVR(), m(**par) can be called
+        this is why they have a ()  in the modelInit slot
+
+        modelList_sklearn_[classifier or regressor] [_lite] is the grid
+        search_s is hence the simplest loop  on the grid
+"""
+
+
 from sklearn.model_selection import GridSearchCV
 from sklearn.svm import SVR, SVC
 from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
 from sklearn.neural_network import MLPRegressor, MLPClassifier
 from sklearn.ensemble import BaggingRegressor, AdaBoostRegressor, GradientBoostingRegressor, BaggingClassifier, AdaBoostClassifier, GradientBoostingClassifier
 
 from sklearn.linear_model import LinearRegression, ElasticNet
@@ -11,20 +21,25 @@
 #from pyearth import Earth
 
 from m5py import M5Prime, export_text_m5
 from cubist import Cubist
 import numpy as np
 
 
+def append_from(l,k = "form", v = "tabular"):
+        for i in l:
+                d=i
+                d[k] = v
+                i=d
 
 
 
 modelList_sklearn_regressor_lite = [{'modelInit' : ElasticNet(),
              'par':{'alpha': [.1,.5,1.0],
-                   'l1_ratio': np.linspace(0.0,1.0,11),
+                   'l1_ratio': np.linspace(0.1,.9,11),
                    'max_iter' : [1000000]}},
              {'modelInit':PLSRegression(),
              'par':{'n_components': [1,2,3,4,5]}},#n<= min samples features targets
              {'modelInit' : SVR(),
               'par' : { 'C':[10000,1000, 100, 10, 1, .1],
                      'epsilon': [0.1, 0.01, 0.05, 0.001],
                      'gamma': ['scale', 'auto']}},
@@ -36,14 +51,17 @@
              {'modelInit' : RandomForestRegressor(),
               'par' : {'n_estimators': [10, 50, 100, 150, 200, 400, 600]}},
              {'modelInit' : AdaBoostRegressor(),
               'par' : {'learning_rate': [.1, 1]}},
              {'modelInit' : GradientBoostingRegressor(),
               'par' : {'learning_rate': [.1, 1]}}]
 
+
+append_from(modelList_sklearn_regressor_lite, "inter", True)
+
 modelList_sklearn_regressor = [{'modelInit' : ElasticNet(),
              'par':{'alpha': [.1,.5,1.0],
                    'l1_ratio': np.linspace(0.0,1.0,11),
                    'max_iter' : [1000000]}},
              {'modelInit':PLSRegression(),
              'par':{'n_components': [1,2,3,4,5]}},#n<= min samples features targets
              {'modelInit' : SVR(),
```

### Comparing `tunesurvey-0.0.3/src/tuneSurvey/tsReshape.py` & `tunesurvey-0.0.4/src/tuneSurvey/vectorized_search_by_term.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     for i in range(n_var):
         if verbose:
             print("working on:" + str(modelName),"model",i)
         m_Yi.append(search_function(model, param_grid = parameters, cv=cv).fit(X,Y[:,i]))
     return m_Yi
 
 
-def saveModelList_s(modelList,X,Y,path="sklModels",verbose=False):
+def saveModelList_s(modelList,X,Y,path="sklModels",verbose=verbose):
     """save a list of model named by modelSequence() convention"""
     pgd = ParameterGrid(modelList['par'])
     if verbose:
         print("Permutating models and saving")
     for i, pars in enumerate(pgd):
         m = deepcopy(modelList['modelInit'])
         if verbose:
```

### Comparing `tunesurvey-0.0.3/tuneSurvey.egg-info/PKG-INFO` & `tunesurvey-0.0.4/tuneSurvey.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `tunesurvey-0.0.3/LICENSE` & `tunesurvey-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tunesurvey-0.0.3/README.md` & `tunesurvey-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 # tuneSurvey
 
-Survey on combination of preprocesses/ features/ model types and hyperparameters on their performances and implications on the data.
+Survey on models, pipelines and AutoML strategies for competitive modeling tasks.
+
+The purpose of this package is to:
+ - enlist a number of existing preprocessing, modeling and model-selection strategies
+ - search within all combinations above(can use brute force, optimization algorithms or inference-based strategies) to get desired accuracy (or compromised with complexity, e.x. AICs, R^2 scores)
+ - investigate stability of models and strategies w.r.t subsets of data, validation folds etc.
+ - approximate benchmarks (time and computation resources) w.r.t data size, model parameters, tune grid sizes etc.
+
+See demo.py for a quick demo.
+
+For each modules and function, use help() to access doc string help.
 
 Inspired by the question "can we automate what is done by statisticians". Answering only one part of the question: "how to automate predictive model selection?"
 The purpose overlaps with various AutoMLs online. But I wish this "modelzoo" cares about tuning and selecting simpler models to:
  - avoid overfitting
  - save time on computing (with default high or low level parallelization)
  - give inferences and interpretations of the data just like [1].
  - compare and visualize if the model selection(AutoML) process is repeatable, stable without data-leaking.
@@ -43,14 +53,15 @@
 (1) Applied Predictive Modeling. Kuhn an Johnson
 Much of the "historical order of models" loosely follows this book.
 (2) Deep Learning. Goodfellow
 On regularizations and kernelizations, and how to tune models
 (3) This lecture by Prof. Hulten(and the prerequisites for NFL theorem) https://www.youtube.com/watch?v=ZXWv3aA8JsI
 (4) This video by Optuna https://www.youtube.com/watch?v=P6NwZVl8ttc
 (5) This website by Prof. Miles Cranmer https://astroautomata.com/PySR/
+(6) The Kaggle Workbook
 
 
 Let's reduce overfit, find interpretability and safety in the modelfitting process!
 
 For the list of relevant Hackathon project I participated that inspired and inspired by this package project:
 [1]UCI 2022 ML Hackathon https://www.informatics.uci.edu/uci-ml-repository-highlights-four-impactful-projects-at-2022-ml-hackathon/
 [2]Embark Datathon Data@UCI 2023 https://devpost.com/software/montreal-crime-space-time-analysis
```

### Comparing `tunesurvey-0.0.3/pyproject.toml` & `tunesurvey-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "tuneSurvey"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Hao Li", email="lhrcplanes@qq.com" },
 ]
 description = "Automatic tuning of machine learning models and surveying on the performance across subsets, variables, features, hyperparameters and pipelines"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tunesurvey-0.0.3/PKG-INFO` & `tunesurvey-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
 Name: tuneSurvey
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automatic tuning of machine learning models and surveying on the performance across subsets, variables, features, hyperparameters and pipelines
 Project-URL: Homepage, https://pypi.org/project/tuneSurvey/0.0.1/
 Project-URL: Bug Tracker, https://github.com/HaoLi111/tuneSurvey/issues
 Author-email: Hao Li <lhrcplanes@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # tuneSurvey
 
-Survey on combination of preprocesses/ features/ model types and hyperparameters on their performances and implications on the data.
+Survey on models, pipelines and AutoML strategies for competitive modeling tasks.
+
+The purpose of this package is to:
+ - enlist a number of existing preprocessing, modeling and model-selection strategies
+ - search within all combinations above(can use brute force, optimization algorithms or inference-based strategies) to get desired accuracy (or compromised with complexity, e.x. AICs, R^2 scores)
+ - investigate stability of models and strategies w.r.t subsets of data, validation folds etc.
+ - approximate benchmarks (time and computation resources) w.r.t data size, model parameters, tune grid sizes etc.
+
+See demo.py for a quick demo.
+
+For each modules and function, use help() to access doc string help.
 
 Inspired by the question "can we automate what is done by statisticians". Answering only one part of the question: "how to automate predictive model selection?"
 The purpose overlaps with various AutoMLs online. But I wish this "modelzoo" cares about tuning and selecting simpler models to:
  - avoid overfitting
  - save time on computing (with default high or low level parallelization)
  - give inferences and interpretations of the data just like [1].
  - compare and visualize if the model selection(AutoML) process is repeatable, stable without data-leaking.
@@ -57,14 +67,15 @@
 (1) Applied Predictive Modeling. Kuhn an Johnson
 Much of the "historical order of models" loosely follows this book.
 (2) Deep Learning. Goodfellow
 On regularizations and kernelizations, and how to tune models
 (3) This lecture by Prof. Hulten(and the prerequisites for NFL theorem) https://www.youtube.com/watch?v=ZXWv3aA8JsI
 (4) This video by Optuna https://www.youtube.com/watch?v=P6NwZVl8ttc
 (5) This website by Prof. Miles Cranmer https://astroautomata.com/PySR/
+(6) The Kaggle Workbook
 
 
 Let's reduce overfit, find interpretability and safety in the modelfitting process!
 
 For the list of relevant Hackathon project I participated that inspired and inspired by this package project:
 [1]UCI 2022 ML Hackathon https://www.informatics.uci.edu/uci-ml-repository-highlights-four-impactful-projects-at-2022-ml-hackathon/
 [2]Embark Datathon Data@UCI 2023 https://devpost.com/software/montreal-crime-space-time-analysis
```

