# Comparing `tmp/aplr-2.5.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-2.6.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 291304 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   321024 b- defN 23-Apr-23 13:46 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   331776 b- defN 23-Apr-23 13:50 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-23 13:41 aplr/__init__.py
--rw-rw-rw-  2.0 fat     6009 b- defN 23-Apr-23 13:41 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-Apr-23 13:50 aplr-2.5.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      626 b- defN 23-Apr-23 13:50 aplr-2.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-23 13:50 aplr-2.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-23 13:50 aplr-2.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      690 b- defN 23-Apr-23 13:50 aplr-2.5.0.dist-info/RECORD
-9 files, 661399 bytes uncompressed, 290132 bytes compressed:  56.1%
+Zip file size: 293000 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   322560 b- defN 23-May-02 15:54 aplr_cpp.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   333824 b- defN 23-May-02 15:58 aplr_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-02 15:48 aplr/__init__.py
+-rw-rw-rw-  2.0 fat     6151 b- defN 23-May-02 15:48 aplr/aplr.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      626 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      690 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/RECORD
+9 files, 665125 bytes uncompressed, 291828 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: aplr/__init__.py
 Comment: 
 
 Filename: aplr/aplr.py
 Comment: 
 
-Filename: aplr-2.5.0.dist-info/LICENSE
+Filename: aplr-2.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-2.5.0.dist-info/METADATA
+Filename: aplr-2.6.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-2.5.0.dist-info/WHEEL
+Filename: aplr-2.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-2.5.0.dist-info/top_level.txt
+Filename: aplr-2.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-2.5.0.dist-info/RECORD
+Filename: aplr-2.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aplr/aplr.py

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import numpy.typing as npt
 from typing import List
 import aplr_cpp
 
 
 class APLRRegressor():
-    def __init__(self, m:int=1000, v:float=0.1, random_state:int=0, family:str="gaussian", link_function:str="identity", n_jobs:int=0, validation_ratio:float=0.2, intercept:float=np.nan, bins:int=300, max_interaction_level:int=1, max_interactions:int=100000, min_observations_in_split:int=20, ineligible_boosting_steps_added:int=10, max_eligible_terms:int=5, verbosity:int=0, tweedie_power:float=1.5, validation_tuning_metric:str="default"):
+    def __init__(self, m:int=1000, v:float=0.1, random_state:int=0, family:str="gaussian", link_function:str="identity", n_jobs:int=0, validation_ratio:float=0.2, intercept:float=np.nan, bins:int=300, max_interaction_level:int=1, max_interactions:int=100000, min_observations_in_split:int=20, ineligible_boosting_steps_added:int=10, max_eligible_terms:int=5, verbosity:int=0, tweedie_power:float=1.5, validation_tuning_metric:str="default", quantile:float=0.5):
         self.m=m
         self.v=v
         self.random_state=random_state
         self.family=family
         self.link_function=link_function
         self.n_jobs=n_jobs
         self.validation_ratio=validation_ratio
@@ -19,14 +19,15 @@
         self.max_interactions=max_interactions
         self.min_observations_in_split=min_observations_in_split
         self.ineligible_boosting_steps_added=ineligible_boosting_steps_added
         self.max_eligible_terms=max_eligible_terms
         self.verbosity=verbosity
         self.tweedie_power=tweedie_power
         self.validation_tuning_metric=validation_tuning_metric
+        self.quantile=quantile
 
         #Creating aplr_cpp and setting parameters
         self.APLRRegressor=aplr_cpp.APLRRegressor()
         self.__set_params_cpp()
 
     #Sets parameters for aplr_cpp.APLRRegressor cpp object
     def __set_params_cpp(self):
@@ -43,14 +44,15 @@
         self.APLRRegressor.max_interactions=self.max_interactions
         self.APLRRegressor.min_observations_in_split=self.min_observations_in_split
         self.APLRRegressor.ineligible_boosting_steps_added=self.ineligible_boosting_steps_added
         self.APLRRegressor.max_eligible_terms=self.max_eligible_terms
         self.APLRRegressor.verbosity=self.verbosity
         self.APLRRegressor.tweedie_power=self.tweedie_power
         self.APLRRegressor.validation_tuning_metric=self.validation_tuning_metric
+        self.APLRRegressor.quantile=self.quantile
 
     def fit(self, X:npt.ArrayLike, y:npt.ArrayLike, sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[],group:npt.ArrayLike = np.empty(0)):
         self.__set_params_cpp()
         self.APLRRegressor.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints,group)
 
     def predict(self, X:npt.ArrayLike, cap_predictions_to_minmax_in_training:bool=True)->npt.ArrayLike:
         return self.APLRRegressor.predict(X, cap_predictions_to_minmax_in_training)
@@ -112,15 +114,16 @@
             "max_interaction_level":self.max_interaction_level,
             "max_interactions":self.max_interactions,
             "verbosity":self.verbosity,
             "min_observations_in_split":self.min_observations_in_split,
             "ineligible_boosting_steps_added":self.ineligible_boosting_steps_added,
             "max_eligible_terms":self.max_eligible_terms,
             "tweedie_power":self.tweedie_power,
-            "validation_tuning_metric":self.validation_tuning_metric
+            "validation_tuning_metric":self.validation_tuning_metric,
+            "quantile":self.quantile
         }
 
     #For sklearn
     def set_params(self, **parameters):
         for parameter, value in parameters.items():
             setattr(self, parameter, value)
         self.__set_params_cpp()
```

## Comparing `aplr-2.5.0.dist-info/LICENSE` & `aplr-2.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aplr-2.5.0.dist-info/METADATA` & `aplr-2.6.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 2.5.0
+Version: 2.6.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
```

## Comparing `aplr-2.5.0.dist-info/RECORD` & `aplr-2.6.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-aplr_cpp.cp39-win_amd64.pyd,sha256=e2m0OOJejnQl_jhYQdVUKTFhcnbGlCuVeXZqOGeSeKE,321024
-aplr_cpp.pypy39-pp73-win_amd64.pyd,sha256=61SPQAmUgoMcQNkmYP0FnnExGKSaIfieXbP5mtjYpzw,331776
+aplr_cpp.cp39-win_amd64.pyd,sha256=7ol9ZgSLuzq8CwiKogEBFFv9I1GSaoijGWlcaxNUakU,322560
+aplr_cpp.pypy39-pp73-win_amd64.pyd,sha256=X7QY2gBAuv-fnuLc7wCKgJt9j6CasElw9kpRvvaI2uw,333824
 aplr/__init__.py,sha256=jLHRAp1zq22wmHqFIghBqfVSnMBnd27LjffHgzI07Hw,19
-aplr/aplr.py,sha256=5AWYY5QUOhlvlMAdTgyFwGvCqqQ3ff8QZYudxh2IHl4,6009
-aplr-2.5.0.dist-info/LICENSE,sha256=YOMo-RaL4P7edMZGD96-NskKpxyMZdP3-WiiMMmihNk,1134
-aplr-2.5.0.dist-info/METADATA,sha256=LMaJm0JIfqHIrsPdQQGCuRd20-dLC1LjXGRCjP5mCrI,626
-aplr-2.5.0.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
-aplr-2.5.0.dist-info/top_level.txt,sha256=DXVC0RIFGpzVnPeKWAZTXQdJheOEZL51Wip6Fx7zbR4,14
-aplr-2.5.0.dist-info/RECORD,,
+aplr/aplr.py,sha256=md6z28MbPZsRTD876fKWyOiF7Jo-ttZPhfp-rHP_WKY,6151
+aplr-2.6.0.dist-info/LICENSE,sha256=YOMo-RaL4P7edMZGD96-NskKpxyMZdP3-WiiMMmihNk,1134
+aplr-2.6.0.dist-info/METADATA,sha256=U0MkI2r_VltIkwe5YMkvui0A6HcobequJaqdZJb-4KY,626
+aplr-2.6.0.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
+aplr-2.6.0.dist-info/top_level.txt,sha256=DXVC0RIFGpzVnPeKWAZTXQdJheOEZL51Wip6Fx7zbR4,14
+aplr-2.6.0.dist-info/RECORD,,
```

