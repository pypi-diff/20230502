# Comparing `tmp/samplics-0.4.5.tar.gz` & `tmp/samplics-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samplics-0.4.5.tar", max compression
+gzip compressed data, was "samplics-0.4.6.tar", max compression
```

## Comparing `samplics-0.4.5.tar` & `samplics-0.4.6.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0     9504 2022-11-18 16:37:14.052836 samplics-0.4.5/README.md
--rw-r--r--   0        0        0     2055 2023-02-17 13:27:35.450789 samplics-0.4.5/pyproject.toml
--rwxr-xr-x   0        0        0     2442 2023-02-17 13:27:50.834045 samplics-0.4.5/src/samplics/__init__.py
--rw-r--r--   0        0        0      177 2021-11-29 11:21:45.000000 samplics-0.4.5/src/samplics/categorical/__init__.py
--rw-r--r--   0        0        0    17506 2022-11-22 17:33:15.855653 samplics-0.4.5/src/samplics/categorical/comparison.py
--rw-r--r--   0        0        0    28691 2023-02-17 13:27:25.371149 samplics-0.4.5/src/samplics/categorical/tabulation.py
--rw-r--r--   0        0        0      573 2021-11-29 11:21:45.000000 samplics-0.4.5/src/samplics/datasets/__init__.py
--rw-r--r--   0        0        0     2575 2021-04-19 23:27:02.000000 samplics-0.4.5/src/samplics/datasets/data/auto.csv
--rw-r--r--   0        0        0    11931 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/birth.csv
--rw-r--r--   0        0        0      951 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/countycrop.csv
--rw-r--r--   0        0        0      461 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/countycrop_means.csv
--rw-r--r--   0        0        0     1236 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/expenditure_on_milk.csv
--rw-r--r--   0        0        0   243781 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/nhanes2.csv
--rw-r--r--   0        0        0   200898 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/nhanes2brr_subset.csv
--rw-r--r--   0        0        0   318640 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/nhanes2jk_subset.csv
--rw-r--r--   0        0        0   221603 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/nmihs_subset.csv
--rw-r--r--   0        0        0     1676 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/psu_frame.csv
--rw-r--r--   0        0        0      335 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/psu_sample.csv
--rw-r--r--   0        0        0     4986 2021-04-19 19:46:20.000000 samplics-0.4.5/src/samplics/datasets/data/ssu_sample.csv
--rw-r--r--   0        0        0     5884 2022-09-17 09:54:59.584836 samplics-0.4.5/src/samplics/datasets/datasets.py
--rwxr-xr-x   0        0        0      175 2021-11-29 11:21:45.000000 samplics-0.4.5/src/samplics/estimation/__init__.py
--rw-r--r--   0        0        0      960 2022-11-01 16:01:56.283535 samplics-0.4.5/src/samplics/estimation/calibration.py
--rwxr-xr-x   0        0        0    39689 2022-11-22 18:36:03.306764 samplics-0.4.5/src/samplics/estimation/expansion.py
--rw-r--r--   0        0        0    20703 2022-11-22 03:17:50.704502 samplics-0.4.5/src/samplics/estimation/replication.py
--rw-r--r--   0        0        0       68 2020-05-24 01:54:43.000000 samplics-0.4.5/src/samplics/py.typed
--rw-r--r--   0        0        0       72 2021-11-29 11:21:45.000000 samplics-0.4.5/src/samplics/regression/__init__.py
--rw-r--r--   0        0        0     3625 2022-11-23 00:11:38.571578 samplics-0.4.5/src/samplics/regression/glm.py
--rw-r--r--   0        0        0      301 2021-11-29 11:21:45.000000 samplics-0.4.5/src/samplics/sae/__init__.py
--rw-r--r--   0        0        0    26914 2022-11-19 01:05:01.264773 samplics-0.4.5/src/samplics/sae/eb_unit_model.py
--rw-r--r--   0        0        0    20174 2023-02-13 05:57:00.784869 samplics-0.4.5/src/samplics/sae/eblup_area_model.py
--rw-r--r--   0        0        0    22790 2022-11-19 01:12:00.459101 samplics-0.4.5/src/samplics/sae/eblup_unit_model.py
--rw-r--r--   0        0        0    19440 2022-11-19 01:05:01.261193 samplics-0.4.5/src/samplics/sae/robust_unit_model.py
--rw-r--r--   0        0        0    13780 2022-09-17 09:54:59.587353 samplics-0.4.5/src/samplics/sae/sae_core_functions.py
--rwxr-xr-x   0        0        0      876 2022-11-20 03:10:58.335741 samplics-0.4.5/src/samplics/sampling/__init__.py
--rw-r--r--   0        0        0    12991 2022-11-19 01:13:31.225123 samplics-0.4.5/src/samplics/sampling/power_functions.py
--rw-r--r--   0        0        0    33701 2022-11-21 21:34:56.685456 samplics-0.4.5/src/samplics/sampling/selection.py
--rw-r--r--   0        0        0    34922 2022-11-21 18:47:30.127565 samplics-0.4.5/src/samplics/sampling/size.py
--rw-r--r--   0        0        0    17936 2022-11-19 01:16:07.524103 samplics-0.4.5/src/samplics/sampling/size_functions.py
--rw-r--r--   0        0        0      584 2022-11-22 19:20:12.473575 samplics-0.4.5/src/samplics/utils/__init__.py
--rw-r--r--   0        0        0     9255 2022-11-22 01:44:42.359380 samplics-0.4.5/src/samplics/utils/basic_functions.py
--rw-r--r--   0        0        0     3273 2022-11-19 01:05:01.275256 samplics-0.4.5/src/samplics/utils/checks.py
--rw-r--r--   0        0        0      472 2022-11-22 19:19:11.336637 samplics-0.4.5/src/samplics/utils/errors.py
--rw-r--r--   0        0        0     6987 2022-11-22 17:56:51.550307 samplics-0.4.5/src/samplics/utils/formats.py
--rw-r--r--   0        0        0     6813 2021-11-29 11:21:45.000000 samplics-0.4.5/src/samplics/utils/hadamard.py
--rw-r--r--   0        0        0     1403 2022-11-20 05:53:29.545084 samplics-0.4.5/src/samplics/utils/types.py
--rwxr-xr-x   0        0        0      161 2021-11-29 11:21:45.000000 samplics-0.4.5/src/samplics/weighting/__init__.py
--rw-r--r--   0        0        0    24814 2022-11-19 01:05:01.273917 samplics-0.4.5/src/samplics/weighting/adjustment.py
--rw-r--r--   0        0        0    13745 2022-11-19 01:05:01.277558 samplics-0.4.5/src/samplics/weighting/replicates.py
--rw-r--r--   0        0        0    10803 1970-01-01 00:00:00.000000 samplics-0.4.5/setup.py
--rw-r--r--   0        0        0    10895 1970-01-01 00:00:00.000000 samplics-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     9504 2022-11-18 16:37:14.052836 samplics-0.4.6/README.md
+-rw-r--r--   0        0        0     2055 2023-05-02 17:30:04.906610 samplics-0.4.6/pyproject.toml
+-rwxr-xr-x   0        0        0     2442 2023-05-02 17:30:16.011081 samplics-0.4.6/src/samplics/__init__.py
+-rw-r--r--   0        0        0      177 2021-11-29 11:21:45.000000 samplics-0.4.6/src/samplics/categorical/__init__.py
+-rw-r--r--   0        0        0    17506 2022-11-22 17:33:15.855653 samplics-0.4.6/src/samplics/categorical/comparison.py
+-rw-r--r--   0        0        0    28691 2023-02-17 13:27:25.371149 samplics-0.4.6/src/samplics/categorical/tabulation.py
+-rw-r--r--   0        0        0      573 2021-11-29 11:21:45.000000 samplics-0.4.6/src/samplics/datasets/__init__.py
+-rw-r--r--   0        0        0     2575 2021-04-19 23:27:02.000000 samplics-0.4.6/src/samplics/datasets/data/auto.csv
+-rw-r--r--   0        0        0    11931 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/birth.csv
+-rw-r--r--   0        0        0      951 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/countycrop.csv
+-rw-r--r--   0        0        0      461 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/countycrop_means.csv
+-rw-r--r--   0        0        0     1236 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/expenditure_on_milk.csv
+-rw-r--r--   0        0        0   243781 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/nhanes2.csv
+-rw-r--r--   0        0        0   200898 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/nhanes2brr_subset.csv
+-rw-r--r--   0        0        0   318640 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/nhanes2jk_subset.csv
+-rw-r--r--   0        0        0   221603 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/nmihs_subset.csv
+-rw-r--r--   0        0        0     1676 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/psu_frame.csv
+-rw-r--r--   0        0        0      335 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/psu_sample.csv
+-rw-r--r--   0        0        0     4986 2021-04-19 19:46:20.000000 samplics-0.4.6/src/samplics/datasets/data/ssu_sample.csv
+-rw-r--r--   0        0        0     5884 2022-09-17 09:54:59.584836 samplics-0.4.6/src/samplics/datasets/datasets.py
+-rwxr-xr-x   0        0        0      175 2021-11-29 11:21:45.000000 samplics-0.4.6/src/samplics/estimation/__init__.py
+-rw-r--r--   0        0        0      960 2022-11-01 16:01:56.283535 samplics-0.4.6/src/samplics/estimation/calibration.py
+-rwxr-xr-x   0        0        0    39689 2022-11-22 18:36:03.306764 samplics-0.4.6/src/samplics/estimation/expansion.py
+-rw-r--r--   0        0        0    20703 2022-11-22 03:17:50.704502 samplics-0.4.6/src/samplics/estimation/replication.py
+-rw-r--r--   0        0        0       68 2020-05-24 01:54:43.000000 samplics-0.4.6/src/samplics/py.typed
+-rw-r--r--   0        0        0       72 2021-11-29 11:21:45.000000 samplics-0.4.6/src/samplics/regression/__init__.py
+-rw-r--r--   0        0        0     3625 2022-11-23 00:11:38.571578 samplics-0.4.6/src/samplics/regression/glm.py
+-rw-r--r--   0        0        0      301 2021-11-29 11:21:45.000000 samplics-0.4.6/src/samplics/sae/__init__.py
+-rw-r--r--   0        0        0    26914 2022-11-19 01:05:01.264773 samplics-0.4.6/src/samplics/sae/eb_unit_model.py
+-rw-r--r--   0        0        0    20321 2023-05-02 17:29:14.263502 samplics-0.4.6/src/samplics/sae/eblup_area_model.py
+-rw-r--r--   0        0        0    22790 2022-11-19 01:12:00.459101 samplics-0.4.6/src/samplics/sae/eblup_unit_model.py
+-rw-r--r--   0        0        0    19440 2022-11-19 01:05:01.261193 samplics-0.4.6/src/samplics/sae/robust_unit_model.py
+-rw-r--r--   0        0        0    13780 2022-09-17 09:54:59.587353 samplics-0.4.6/src/samplics/sae/sae_core_functions.py
+-rwxr-xr-x   0        0        0      876 2022-11-20 03:10:58.335741 samplics-0.4.6/src/samplics/sampling/__init__.py
+-rw-r--r--   0        0        0    12991 2022-11-19 01:13:31.225123 samplics-0.4.6/src/samplics/sampling/power_functions.py
+-rw-r--r--   0        0        0    33701 2022-11-21 21:34:56.685456 samplics-0.4.6/src/samplics/sampling/selection.py
+-rw-r--r--   0        0        0    34921 2023-03-17 07:43:07.886958 samplics-0.4.6/src/samplics/sampling/size.py
+-rw-r--r--   0        0        0    17936 2022-11-19 01:16:07.524103 samplics-0.4.6/src/samplics/sampling/size_functions.py
+-rw-r--r--   0        0        0      584 2022-11-22 19:20:12.473575 samplics-0.4.6/src/samplics/utils/__init__.py
+-rw-r--r--   0        0        0     9255 2022-11-22 01:44:42.359380 samplics-0.4.6/src/samplics/utils/basic_functions.py
+-rw-r--r--   0        0        0     3273 2022-11-19 01:05:01.275256 samplics-0.4.6/src/samplics/utils/checks.py
+-rw-r--r--   0        0        0      472 2022-11-22 19:19:11.336637 samplics-0.4.6/src/samplics/utils/errors.py
+-rw-r--r--   0        0        0     6987 2022-11-22 17:56:51.550307 samplics-0.4.6/src/samplics/utils/formats.py
+-rw-r--r--   0        0        0     6813 2021-11-29 11:21:45.000000 samplics-0.4.6/src/samplics/utils/hadamard.py
+-rw-r--r--   0        0        0     1403 2022-11-20 05:53:29.545084 samplics-0.4.6/src/samplics/utils/types.py
+-rwxr-xr-x   0        0        0      161 2021-11-29 11:21:45.000000 samplics-0.4.6/src/samplics/weighting/__init__.py
+-rw-r--r--   0        0        0    24814 2022-11-19 01:05:01.273917 samplics-0.4.6/src/samplics/weighting/adjustment.py
+-rw-r--r--   0        0        0    13745 2022-11-19 01:05:01.277558 samplics-0.4.6/src/samplics/weighting/replicates.py
+-rw-r--r--   0        0        0    10895 1970-01-01 00:00:00.000000 samplics-0.4.6/PKG-INFO
```

### Comparing `samplics-0.4.5/README.md` & `samplics-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/pyproject.toml` & `samplics-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Mamadou S Diallo <msdiallo@samplics.org>"]
 description = "Select, weight and analyze complex sample data"
 license = "MIT"
 name = "samplics"
-version = "0.4.5"
+version = "0.4.6"
 
 readme = "README.md"
 
 documentation = "https://samplics-org.github.io/samplics/"
 homepage = "https://samplics-org.github.io/samplics//"
 repository = "https://github.com/survey-methods/samplics"
```

### Comparing `samplics-0.4.5/src/samplics/__init__.py` & `samplics-0.4.6/src/samplics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,8 +99,8 @@
     "CertaintyError",
     "DimensionError",
     "MethodError",
     "ProbError",
     "SinglePSUError",
 ]
 
-__version__ = "0.4.5"
+__version__ = "0.4.6"
```

### Comparing `samplics-0.4.5/src/samplics/categorical/comparison.py` & `samplics-0.4.6/src/samplics/categorical/comparison.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/categorical/tabulation.py` & `samplics-0.4.6/src/samplics/categorical/tabulation.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/__init__.py` & `samplics-0.4.6/src/samplics/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/auto.csv` & `samplics-0.4.6/src/samplics/datasets/data/auto.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/birth.csv` & `samplics-0.4.6/src/samplics/datasets/data/birth.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/countycrop.csv` & `samplics-0.4.6/src/samplics/datasets/data/countycrop.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/expenditure_on_milk.csv` & `samplics-0.4.6/src/samplics/datasets/data/expenditure_on_milk.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/nhanes2.csv` & `samplics-0.4.6/src/samplics/datasets/data/nhanes2.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/nhanes2brr_subset.csv` & `samplics-0.4.6/src/samplics/datasets/data/nhanes2brr_subset.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/nhanes2jk_subset.csv` & `samplics-0.4.6/src/samplics/datasets/data/nhanes2jk_subset.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/nmihs_subset.csv` & `samplics-0.4.6/src/samplics/datasets/data/nmihs_subset.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/psu_frame.csv` & `samplics-0.4.6/src/samplics/datasets/data/psu_frame.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/data/ssu_sample.csv` & `samplics-0.4.6/src/samplics/datasets/data/ssu_sample.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/datasets/datasets.py` & `samplics-0.4.6/src/samplics/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/estimation/calibration.py` & `samplics-0.4.6/src/samplics/estimation/calibration.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/estimation/expansion.py` & `samplics-0.4.6/src/samplics/estimation/expansion.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/estimation/replication.py` & `samplics-0.4.6/src/samplics/estimation/replication.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/regression/glm.py` & `samplics-0.4.6/src/samplics/regression/glm.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sae/eb_unit_model.py` & `samplics-0.4.6/src/samplics/sae/eb_unit_model.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sae/eblup_area_model.py` & `samplics-0.4.6/src/samplics/sae/eblup_area_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         | fit(): fits the linear mixed model to estimate the model parameters using REMl or ML
         |   methods.
         | predict(): predicts the area level mean estimates which includes both the point   | |
         |   estimates and the taylor MSE estimate.
     """
 
     def __init__(self, method: str = "REML") -> None:
-
         if method.upper() not in ("FH", "ML", "REML"):
             raise AssertionError("Parameter method must be 'FH', 'ML, or 'REML'.")
         else:
             self.method = method.upper()
 
         # Sample data
         self.yhat: np.ndarray
@@ -99,15 +98,14 @@
         self.area_est: DictStrNum
         self.area_mse: DictStrNum
         self.area_mse_as1: DictStrNum
         self.area_mse_as2: DictStrNum
         self.area_mse_terms: dict[str, DictStrNum]
 
     def __str__(self) -> str:
-
         estimation = pd.DataFrame()
         estimation["area"] = self.area
         estimation["estimate"] = self.area_est
         estimation["mse"] = self.area_est
 
         fit = pd.DataFrame()
         fit["beta_coef"] = self.fixed_effects
@@ -123,29 +121,27 @@
         area: np.ndarray,
         yhat: np.ndarray,
         X: np.ndarray,
         sigma2_e: np.ndarray,
         sigma2_v: float,
         b_const: np.ndarray,
     ) -> tuple[np.ndarray, np.ndarray]:
-
         # V = np.diag(sigma2_v * (b_const**2) + sigma2_e)
         # V_inv = np.linalg.inv(V)
-        V_inv = np.diag(1 / (sigma2_v * (b_const**2) + sigma2_e))  
+        V_inv = np.diag(1 / (sigma2_v * (b_const**2) + sigma2_e))
         x_v_X_inv = np.linalg.inv(np.matmul(np.matmul(np.transpose(X), V_inv), X))
         x_v_x_inv_x = np.matmul(np.matmul(x_v_X_inv, np.transpose(X)), V_inv)
         beta_hat = np.matmul(x_v_x_inv_x, yhat)
         beta_cov = np.matmul(np.matmul(np.transpose(X), V_inv), X)
 
         return beta_hat.ravel(), np.linalg.inv(beta_cov)
 
     def _log_likelihood(
         self, y: np.ndarray, X: np.ndarray, beta: np.ndarray, V: np.ndarray
     ) -> Number:
-
         m = y.size
         const = m * np.log(2 * np.pi)
         ll_term1 = np.log(np.linalg.det(V))
         V_inv = np.linalg.inv(V)
         resid_term = y - np.dot(X, beta)
         if self.method in ("ML", "FH"):  # Whta is likelihood for FH
             resid_var = np.dot(np.transpose(resid_term), V_inv)
@@ -166,15 +162,14 @@
         area: np.ndarray,
         yhat: np.ndarray,
         X: np.ndarray,
         sigma2_e: np.ndarray,
         sigma2_v: Number,
         b_const: np.ndarray,
     ) -> tuple[Number, Number]:
-
         deriv_sigma = 0.0
         info_sigma = 0.0
         if self.method == "ML":
             beta, beta_cov = self._fixed_coefficients(
                 area=area,
                 yhat=yhat,
                 X=X,
@@ -282,15 +277,14 @@
         np.ndarray,
         np.ndarray,
         np.ndarray,
         np.ndarray,
         np.ndarray,
         np.ndarray,
     ]:
-
         m = self.yhat.size
         v_i = sigma2_e + sigma2_v * (b_const**2)
         V_inv = np.diag(1 / v_i)
         G = np.diag(np.ones(m) * sigma2_v)
 
         Z = np.diag(b_const)
 
@@ -397,15 +391,20 @@
         """
 
         area = numpy_array(area)
         yhat = numpy_array(yhat)
         X = numpy_array(X)
 
         error_std = numpy_array(error_std)
-        error_std = numpy_array(error_std)
+
+        if (error_std <= 0).any():
+            raise ValueError(
+                "Some of the standard errors are not strictly positive. All standard errors must be greater than 0."
+            )
+
         if isinstance(b_const, (int, float)):
             b_const = np.asarray(np.ones(area.size) * b_const)
         else:
             b_const = numpy_array(b_const)
 
         if intercept and isinstance(X, np.ndarray):
             X = np.insert(X, 0, 1, axis=1)
```

### Comparing `samplics-0.4.5/src/samplics/sae/eblup_unit_model.py` & `samplics-0.4.6/src/samplics/sae/eblup_unit_model.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sae/robust_unit_model.py` & `samplics-0.4.6/src/samplics/sae/robust_unit_model.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sae/sae_core_functions.py` & `samplics-0.4.6/src/samplics/sae/sae_core_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sampling/__init__.py` & `samplics-0.4.6/src/samplics/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sampling/power_functions.py` & `samplics-0.4.6/src/samplics/sampling/power_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sampling/selection.py` & `samplics-0.4.6/src/samplics/sampling/selection.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/sampling/size.py` & `samplics-0.4.6/src/samplics/sampling/size.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Sample size calculation module 
+"""Sample size calculation module
 
 """
 
 from __future__ import annotations
 
 import math
```

### Comparing `samplics-0.4.5/src/samplics/sampling/size_functions.py` & `samplics-0.4.6/src/samplics/sampling/size_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/utils/__init__.py` & `samplics-0.4.6/src/samplics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/utils/basic_functions.py` & `samplics-0.4.6/src/samplics/utils/basic_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/utils/checks.py` & `samplics-0.4.6/src/samplics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/utils/formats.py` & `samplics-0.4.6/src/samplics/utils/formats.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/utils/hadamard.py` & `samplics-0.4.6/src/samplics/utils/hadamard.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/utils/types.py` & `samplics-0.4.6/src/samplics/utils/types.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/weighting/adjustment.py` & `samplics-0.4.6/src/samplics/weighting/adjustment.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/src/samplics/weighting/replicates.py` & `samplics-0.4.6/src/samplics/weighting/replicates.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.5/setup.py` & `samplics-0.4.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,290 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: samplics
+Version: 0.4.6
+Summary: Select, weight and analyze complex sample data
+Home-page: https://samplics-org.github.io/samplics//
+License: MIT
+Keywords: sampling,sample,weighting,estimation,survey
+Author: Mamadou S Diallo
+Author-email: msdiallo@samplics.org
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: matplotlib (>=3.4,<4.0)
+Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: scipy (>=1.7,<2.0)
+Requires-Dist: statsmodels (>=0.13,<0.14)
+Project-URL: Documentation, https://samplics-org.github.io/samplics/
+Project-URL: Repository, https://github.com/survey-methods/samplics
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+<img src="./img/samplics_logo.jpg"  align="left" style="height: 110px; border-radius: 10%; padding: 5px;"/>
 
-packages = \
-['samplics',
- 'samplics.categorical',
- 'samplics.datasets',
- 'samplics.estimation',
- 'samplics.regression',
- 'samplics.sae',
- 'samplics.sampling',
- 'samplics.utils',
- 'samplics.weighting']
-
-package_data = \
-{'': ['*'], 'samplics.datasets': ['data/*']}
-
-install_requires = \
-['matplotlib>=3.4,<4.0',
- 'numpy>=1.21,<2.0',
- 'pandas>=1.3,<2.0',
- 'scipy>=1.7,<2.0',
- 'statsmodels>=0.13,<0.14']
-
-setup_kwargs = {
-    'name': 'samplics',
-    'version': '0.4.5',
-    'description': 'Select, weight and analyze complex sample data',
-    'long_description': '<img src="./img/samplics_logo.jpg"  align="left" style="height: 110px; border-radius: 10%; padding: 5px;"/>\n\n\n<h1> Sample Analytics </h1>\n\n[<img src="https://github.com/survey-methods/samplics/workflows/Testing/badge.svg">](https://github.com/survey-methods/samplics/actions?query=workflow%3ATesting)\n[<img src="https://github.com/survey-methods/samplics/workflows/Coverage/badge.svg">](https://github.com/survey-methods/samplics/actions?query=workflow%3ACoverage)\n[<img src="https://github.com/survey-methods/samplics/workflows/Docs/badge.svg">](https://github.com/samplics-org/samplics/actions?query=workflow%3ADocs)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.03376/status.svg)](https://doi.org/10.21105/joss.03376)\n[<img src="https://pepy.tech/badge/samplics">](https://pepy.tech/project/samplics)\n\n\n\nIn large-scale surveys, often complex random mechanisms are used to select samples. Estimates derived from such samples must reflect the random mechanism. _Samplics_ is a python package that implements a set of sampling techniques for complex survey designs. These survey sampling techniques are organized into the following four sub-packages.\n\n**Sampling** provides a set of random selection techniques used to draw a sample from a population. It also provides procedures for calculating sample sizes. The sampling subpackage contains:\n\n- Sample size calculation and allocation: Wald and Fleiss methods for proportions.\n- Equal probability of selection: simple random sampling (SRS) and systematic selection (SYS)\n- Probability proportional to size (PPS): Systematic, Brewer\'s method, Hanurav-Vijayan method, Murphy\'s method, and Rao-Sampford\'s method.\n\n**Weighting** provides the procedures for adjusting sample weights. More specifically, the weighting subpackage allows the following:\n\n- Weight adjustment due to nonresponse\n- Weight poststratification, calibration and normalization\n- Weight replication i.e. Bootstrap, BRR, and Jackknife\n\n**Estimation** provides methods for estimating the parameters of interest with uncertainty measures that are consistent with the sampling design. The estimation subpackage implements the following types of estimation methods:\n\n- Taylor-based, also called linearization methods\n- Replication-based estimation i.e. Boostrap, BRR, and Jackknife\n- Regression-based e.g. generalized regression (GREG)\n\n**Small Area Estimation (SAE).** When the sample size is not large enough to produce reliable / stable domain level estimates, SAE techniques can be used to model the output variable of interest to produce domain level estimates. This subpackage provides Area-level and Unit-level SAE methods.\n\nFor more details, visit https://samplics-org.github.io/samplics/\n\n## Usage\n\nLet\'s assume that we have a population and we would like to select a sample from it. The goal is to calculate the sample size for an expected proportion of 0.80 with a precision (half confidence interval) of 0.10.\n\n> ```python\n> from samplics.sampling import SampleSize\n>\n> sample_size = SampleSize(parameter = "proportion")\n> sample_size.calculate(target=0.80, half_ci=0.10)\n> ```\n\nFurthermore, the population is located in four natural regions i.e. North, South, East, and West. We could be interested in calculating sample sizes based on region specific requirements e.g. expected proportions, desired precisions and associated design effects.\n\n> ```python\n> from samplics.sampling import SampleSize\n>\n> sample_size = SampleSize(parameter="proportion", method="wald", stratification=True)\n>\n> expected_proportions = {"North": 0.95, "South": 0.70, "East": 0.30, "West": 0.50}\n> half_ci = {"North": 0.30, "South": 0.10, "East": 0.15, "West": 0.10}\n> deff = {"North": 1, "South": 1.5, "East": 2.5, "West": 2.0}\n>\n> sample_size = SampleSize(parameter = "proportion", method="Fleiss", stratification=True)\n> sample_size.calculate(target=expected_proportions, half_ci=half_ci, deff=deff)\n> ```\n\nTo select a sample of primary sampling units using PPS method,\nwe can use code similar to the snippets below. Note that we first use the `datasets` module to import the example dataset.\n\n> ```python\n> # First we import the example dataset\n> from samplics.datasets import load_psu_frame\n> psu_frame_dict = load_psu_frame()\n> psu_frame = psu_frame_dict["data"]\n>\n> # Code for the sample selection\n> from samplics.sampling import SampleSelection\n>\n> psu_sample_size = {"East":3, "West": 2, "North": 2, "South": 3}\n> pps_design = SampleSelection(\n>    method="pps-sys",\n>    stratification=True,\n>    with_replacement=False\n>    )\n>\n> psu_frame["psu_prob"] = pps_design.inclusion_probs(\n>    psu_frame["cluster"],\n>    psu_sample_size,\n>    psu_frame["region"],\n>    psu_frame["number_households_census"]\n>    )\n> ```\n\nThe initial weighting step is to obtain the design sample weights. In this example, we show a simple example of two-stage sampling design.\n\n> ```python\n> import pandas as pd\n>\n> from samplics.datasets import load_psu_sample, load_ssu_sample\n> from samplics.weighting import SampleWeight\n>\n> # Load PSU sample data\n> psu_sample_dict = load_psu_sample()\n> psu_sample = psu_sample_dict["data"]\n>\n> # Load PSU sample data\n> ssu_sample_dict = load_ssu_sample()\n> ssu_sample = ssu_sample_dict["data"]\n>\n> full_sample = pd.merge(\n>     psu_sample[["cluster", "region", "psu_prob"]],\n>     ssu_sample[["cluster", "household", "ssu_prob"]],\n>     on="cluster"\n> )\n>\n> full_sample["inclusion_prob"] = full_sample["psu_prob"] * full_sample["ssu_prob"]\n> full_sample["design_weight"] = 1 / full_sample["inclusion_prob"]\n> ```\n\nTo adjust the design sample weight for nonresponse,\nwe can use code similar to:\n\n> ```python\n> import numpy as np\n>\n> from samplics.weighting import SampleWeight\n>\n> # Simulate response\n> np.random.seed(7)\n> full_sample["response_status"] = np.random.choice(\n>     ["ineligible", "respondent", "non-respondent", "unknown"],\n>     size=full_sample.shape[0],\n>     p=(0.10, 0.70, 0.15, 0.05),\n> )\n> # Map custom response statuses to teh generic samplics statuses\n> status_mapping = {\n>    "in": "ineligible",\n>    "rr": "respondent",\n>    "nr": "non-respondent",\n>    "uk":"unknown"\n>    }\n> # adjust sample weights\n> full_sample["nr_weight"] = SampleWeight().adjust(\n>    samp_weight=full_sample["design_weight"],\n>    adjust_class=full_sample["region"],\n>    resp_status=full_sample["response_status"],\n>    resp_dict=status_mapping\n>    )\n> ```\n\nTo estimate population parameters using Taylor-based and replication-based methods, we can use code similar to:\n\n> ```python\n> # Taylor-based\n> from samplics.datasets import load_nhanes2\n>\n> nhanes2_dict = load_nhanes2()\n> nhanes2 = nhanes2_dict["data"]\n>\n> from samplics.estimation import TaylorEstimator\n>\n> zinc_mean_str = TaylorEstimator("mean")\n> zinc_mean_str.estimate(\n>     y=nhanes2["zinc"],\n>     samp_weight=nhanes2["finalwgt"],\n>     stratum=nhanes2["stratid"],\n>     psu=nhanes2["psuid"],\n>     remove_nan=True,\n> )\n>\n> # Replicate-based\n> from samplics.datasets import load_nhanes2brr\n>\n> nhanes2brr_dict = load_nhanes2brr()\n> nhanes2brr = nhanes2brr_dict["data"]\n>\n> from samplics.estimation import ReplicateEstimator\n>\n> ratio_wgt_hgt = ReplicateEstimator("brr", "ratio").estimate(\n>     y=nhanes2brr["weight"],\n>     samp_weight=nhanes2brr["finalwgt"],\n>     x=nhanes2brr["height"],\n>     rep_weights=nhanes2brr.loc[:, "brr_1":"brr_32"],\n>     remove_nan=True,\n> )\n>\n> ```\n\nTo predict small area parameters, we can use code similar to:\n\n> ```python\n> import numpy as np\n> import pandas as pd\n>\n> # Area-level basic method\n> from samplics.datasets import load_expenditure_milk\n>\n> milk_exp_dict = load_expenditure_milk()\n> milk_exp = milk_exp_dict["data"]\n>\n> from samplics.sae import EblupAreaModel\n>\n> fh_model_reml = EblupAreaModel(method="REML")\n> fh_model_reml.fit(\n>     yhat=milk_exp["direct_est"],\n>     X=pd.get_dummies(milk_exp["major_area"], drop_first=True),\n>     area=milk_exp["small_area"],\n>     error_std=milk_exp["std_error"],\n>     intercept=True,\n>     tol=1e-8,\n> )\n> fh_model_reml.predict(\n>     X=pd.get_dummies(milk_exp["major_area"], drop_first=True),\n>     area=milk_exp["small_area"],\n>     intercept=True,\n> )\n>\n> # Unit-level basic method\n> from samplics.datasets import load_county_crop, load_county_crop_means\n>\n> # Load County Crop sample data\n> countycrop_dict = load_county_crop()\n> countycrop = countycrop_dict["data"]\n> # Load County Crop Area Means sample data\n> countycropmeans_dict = load_county_crop_means()\n> countycrop_means = countycropmeans_dict["data"]\n>\n> from samplics.sae import EblupUnitModel\n>\n> eblup_bhf_reml = EblupUnitModel()\n> eblup_bhf_reml.fit(\n>     countycrop["corn_area"],\n>     countycrop[["corn_pixel", "soybeans_pixel"]],\n>     countycrop["county_id"],\n> )\n> eblup_bhf_reml.predict(\n>     Xmean=countycrop_means[["ave_corn_pixel", "ave_corn_pixel"]],\n>     area=np.linspace(1, 12, 12),\n> )\n>\n> ```\n\n## Installation\n\n`pip install samplics`\n\nPython 3.7 or newer is required and the main dependencies are [numpy](https://numpy.org), [pandas](https://pandas.pydata.org), [scpy](https://www.scipy.org), and [statsmodel](https://www.statsmodels.org/stable/index.html).\n\n## Contribution\n\nIf you would like to contribute to the project, please read [contributing to samplics](https://github.com/samplics-org/samplics/blob/main/CONTRIBUTING.md)\n\n## License\n\n[MIT](https://github.com/survey-methods/samplics/blob/master/license.txt)\n\n## Contact\n\ncreated by [Mamadou S. Diallo](https://twitter.com/MamadouSDiallo) - feel free to contact me!\n',
-    'author': 'Mamadou S Diallo',
-    'author_email': 'msdiallo@samplics.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://samplics-org.github.io/samplics//',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
 
+<h1> Sample Analytics </h1>
+
+[<img src="https://github.com/survey-methods/samplics/workflows/Testing/badge.svg">](https://github.com/survey-methods/samplics/actions?query=workflow%3ATesting)
+[<img src="https://github.com/survey-methods/samplics/workflows/Coverage/badge.svg">](https://github.com/survey-methods/samplics/actions?query=workflow%3ACoverage)
+[<img src="https://github.com/survey-methods/samplics/workflows/Docs/badge.svg">](https://github.com/samplics-org/samplics/actions?query=workflow%3ADocs)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.03376/status.svg)](https://doi.org/10.21105/joss.03376)
+[<img src="https://pepy.tech/badge/samplics">](https://pepy.tech/project/samplics)
+
+
+
+In large-scale surveys, often complex random mechanisms are used to select samples. Estimates derived from such samples must reflect the random mechanism. _Samplics_ is a python package that implements a set of sampling techniques for complex survey designs. These survey sampling techniques are organized into the following four sub-packages.
+
+**Sampling** provides a set of random selection techniques used to draw a sample from a population. It also provides procedures for calculating sample sizes. The sampling subpackage contains:
+
+- Sample size calculation and allocation: Wald and Fleiss methods for proportions.
+- Equal probability of selection: simple random sampling (SRS) and systematic selection (SYS)
+- Probability proportional to size (PPS): Systematic, Brewer's method, Hanurav-Vijayan method, Murphy's method, and Rao-Sampford's method.
+
+**Weighting** provides the procedures for adjusting sample weights. More specifically, the weighting subpackage allows the following:
+
+- Weight adjustment due to nonresponse
+- Weight poststratification, calibration and normalization
+- Weight replication i.e. Bootstrap, BRR, and Jackknife
+
+**Estimation** provides methods for estimating the parameters of interest with uncertainty measures that are consistent with the sampling design. The estimation subpackage implements the following types of estimation methods:
+
+- Taylor-based, also called linearization methods
+- Replication-based estimation i.e. Boostrap, BRR, and Jackknife
+- Regression-based e.g. generalized regression (GREG)
+
+**Small Area Estimation (SAE).** When the sample size is not large enough to produce reliable / stable domain level estimates, SAE techniques can be used to model the output variable of interest to produce domain level estimates. This subpackage provides Area-level and Unit-level SAE methods.
+
+For more details, visit https://samplics-org.github.io/samplics/
+
+## Usage
+
+Let's assume that we have a population and we would like to select a sample from it. The goal is to calculate the sample size for an expected proportion of 0.80 with a precision (half confidence interval) of 0.10.
+
+> ```python
+> from samplics.sampling import SampleSize
+>
+> sample_size = SampleSize(parameter = "proportion")
+> sample_size.calculate(target=0.80, half_ci=0.10)
+> ```
+
+Furthermore, the population is located in four natural regions i.e. North, South, East, and West. We could be interested in calculating sample sizes based on region specific requirements e.g. expected proportions, desired precisions and associated design effects.
+
+> ```python
+> from samplics.sampling import SampleSize
+>
+> sample_size = SampleSize(parameter="proportion", method="wald", stratification=True)
+>
+> expected_proportions = {"North": 0.95, "South": 0.70, "East": 0.30, "West": 0.50}
+> half_ci = {"North": 0.30, "South": 0.10, "East": 0.15, "West": 0.10}
+> deff = {"North": 1, "South": 1.5, "East": 2.5, "West": 2.0}
+>
+> sample_size = SampleSize(parameter = "proportion", method="Fleiss", stratification=True)
+> sample_size.calculate(target=expected_proportions, half_ci=half_ci, deff=deff)
+> ```
+
+To select a sample of primary sampling units using PPS method,
+we can use code similar to the snippets below. Note that we first use the `datasets` module to import the example dataset.
+
+> ```python
+> # First we import the example dataset
+> from samplics.datasets import load_psu_frame
+> psu_frame_dict = load_psu_frame()
+> psu_frame = psu_frame_dict["data"]
+>
+> # Code for the sample selection
+> from samplics.sampling import SampleSelection
+>
+> psu_sample_size = {"East":3, "West": 2, "North": 2, "South": 3}
+> pps_design = SampleSelection(
+>    method="pps-sys",
+>    stratification=True,
+>    with_replacement=False
+>    )
+>
+> psu_frame["psu_prob"] = pps_design.inclusion_probs(
+>    psu_frame["cluster"],
+>    psu_sample_size,
+>    psu_frame["region"],
+>    psu_frame["number_households_census"]
+>    )
+> ```
+
+The initial weighting step is to obtain the design sample weights. In this example, we show a simple example of two-stage sampling design.
+
+> ```python
+> import pandas as pd
+>
+> from samplics.datasets import load_psu_sample, load_ssu_sample
+> from samplics.weighting import SampleWeight
+>
+> # Load PSU sample data
+> psu_sample_dict = load_psu_sample()
+> psu_sample = psu_sample_dict["data"]
+>
+> # Load PSU sample data
+> ssu_sample_dict = load_ssu_sample()
+> ssu_sample = ssu_sample_dict["data"]
+>
+> full_sample = pd.merge(
+>     psu_sample[["cluster", "region", "psu_prob"]],
+>     ssu_sample[["cluster", "household", "ssu_prob"]],
+>     on="cluster"
+> )
+>
+> full_sample["inclusion_prob"] = full_sample["psu_prob"] * full_sample["ssu_prob"]
+> full_sample["design_weight"] = 1 / full_sample["inclusion_prob"]
+> ```
+
+To adjust the design sample weight for nonresponse,
+we can use code similar to:
+
+> ```python
+> import numpy as np
+>
+> from samplics.weighting import SampleWeight
+>
+> # Simulate response
+> np.random.seed(7)
+> full_sample["response_status"] = np.random.choice(
+>     ["ineligible", "respondent", "non-respondent", "unknown"],
+>     size=full_sample.shape[0],
+>     p=(0.10, 0.70, 0.15, 0.05),
+> )
+> # Map custom response statuses to teh generic samplics statuses
+> status_mapping = {
+>    "in": "ineligible",
+>    "rr": "respondent",
+>    "nr": "non-respondent",
+>    "uk":"unknown"
+>    }
+> # adjust sample weights
+> full_sample["nr_weight"] = SampleWeight().adjust(
+>    samp_weight=full_sample["design_weight"],
+>    adjust_class=full_sample["region"],
+>    resp_status=full_sample["response_status"],
+>    resp_dict=status_mapping
+>    )
+> ```
+
+To estimate population parameters using Taylor-based and replication-based methods, we can use code similar to:
+
+> ```python
+> # Taylor-based
+> from samplics.datasets import load_nhanes2
+>
+> nhanes2_dict = load_nhanes2()
+> nhanes2 = nhanes2_dict["data"]
+>
+> from samplics.estimation import TaylorEstimator
+>
+> zinc_mean_str = TaylorEstimator("mean")
+> zinc_mean_str.estimate(
+>     y=nhanes2["zinc"],
+>     samp_weight=nhanes2["finalwgt"],
+>     stratum=nhanes2["stratid"],
+>     psu=nhanes2["psuid"],
+>     remove_nan=True,
+> )
+>
+> # Replicate-based
+> from samplics.datasets import load_nhanes2brr
+>
+> nhanes2brr_dict = load_nhanes2brr()
+> nhanes2brr = nhanes2brr_dict["data"]
+>
+> from samplics.estimation import ReplicateEstimator
+>
+> ratio_wgt_hgt = ReplicateEstimator("brr", "ratio").estimate(
+>     y=nhanes2brr["weight"],
+>     samp_weight=nhanes2brr["finalwgt"],
+>     x=nhanes2brr["height"],
+>     rep_weights=nhanes2brr.loc[:, "brr_1":"brr_32"],
+>     remove_nan=True,
+> )
+>
+> ```
+
+To predict small area parameters, we can use code similar to:
+
+> ```python
+> import numpy as np
+> import pandas as pd
+>
+> # Area-level basic method
+> from samplics.datasets import load_expenditure_milk
+>
+> milk_exp_dict = load_expenditure_milk()
+> milk_exp = milk_exp_dict["data"]
+>
+> from samplics.sae import EblupAreaModel
+>
+> fh_model_reml = EblupAreaModel(method="REML")
+> fh_model_reml.fit(
+>     yhat=milk_exp["direct_est"],
+>     X=pd.get_dummies(milk_exp["major_area"], drop_first=True),
+>     area=milk_exp["small_area"],
+>     error_std=milk_exp["std_error"],
+>     intercept=True,
+>     tol=1e-8,
+> )
+> fh_model_reml.predict(
+>     X=pd.get_dummies(milk_exp["major_area"], drop_first=True),
+>     area=milk_exp["small_area"],
+>     intercept=True,
+> )
+>
+> # Unit-level basic method
+> from samplics.datasets import load_county_crop, load_county_crop_means
+>
+> # Load County Crop sample data
+> countycrop_dict = load_county_crop()
+> countycrop = countycrop_dict["data"]
+> # Load County Crop Area Means sample data
+> countycropmeans_dict = load_county_crop_means()
+> countycrop_means = countycropmeans_dict["data"]
+>
+> from samplics.sae import EblupUnitModel
+>
+> eblup_bhf_reml = EblupUnitModel()
+> eblup_bhf_reml.fit(
+>     countycrop["corn_area"],
+>     countycrop[["corn_pixel", "soybeans_pixel"]],
+>     countycrop["county_id"],
+> )
+> eblup_bhf_reml.predict(
+>     Xmean=countycrop_means[["ave_corn_pixel", "ave_corn_pixel"]],
+>     area=np.linspace(1, 12, 12),
+> )
+>
+> ```
+
+## Installation
+
+`pip install samplics`
+
+Python 3.7 or newer is required and the main dependencies are [numpy](https://numpy.org), [pandas](https://pandas.pydata.org), [scpy](https://www.scipy.org), and [statsmodel](https://www.statsmodels.org/stable/index.html).
+
+## Contribution
+
+If you would like to contribute to the project, please read [contributing to samplics](https://github.com/samplics-org/samplics/blob/main/CONTRIBUTING.md)
+
+## License
+
+[MIT](https://github.com/survey-methods/samplics/blob/master/license.txt)
+
+## Contact
+
+created by [Mamadou S. Diallo](https://twitter.com/MamadouSDiallo) - feel free to contact me!
 
-setup(**setup_kwargs)
```

