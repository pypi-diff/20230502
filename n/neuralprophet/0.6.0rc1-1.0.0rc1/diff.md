# Comparing `tmp/neuralprophet-0.6.0rc1.tar.gz` & `tmp/neuralprophet-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralprophet-0.6.0rc1.tar", max compression
+gzip compressed data, was "neuralprophet-1.0.0rc1.tar", max compression
```

## Comparing `neuralprophet-0.6.0rc1.tar` & `neuralprophet-1.0.0rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1070 2022-11-24 05:34:19.680929 neuralprophet-0.6.0rc1/LICENSE
--rw-r--r--   0        0        0     7464 2023-04-15 04:16:53.611613 neuralprophet-0.6.0rc1/README.md
--rw-r--r--   0        0        0     1394 2023-04-15 04:16:53.703131 neuralprophet-0.6.0rc1/neuralprophet/__init__.py
--rw-r--r--   0        0        0      398 2023-04-15 04:16:53.703711 neuralprophet-0.6.0rc1/neuralprophet/__main__.py
--rw-r--r--   0        0        0       25 2023-04-15 04:17:20.775326 neuralprophet-0.6.0rc1/neuralprophet/_version.py
--rw-r--r--   0        0        0      683 2023-04-15 04:16:53.704907 neuralprophet-0.6.0rc1/neuralprophet/components/README.md
--rw-r--r--   0        0        0       46 2023-04-15 04:16:53.705091 neuralprophet-0.6.0rc1/neuralprophet/components/__init__.py
--rw-r--r--   0        0        0      931 2023-04-15 04:16:53.706486 neuralprophet-0.6.0rc1/neuralprophet/components/base.py
--rw-r--r--   0        0        0       49 2023-04-15 04:16:53.707158 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-15 04:16:53.707535 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/base.py
--rw-r--r--   0        0        0     3681 2023-04-15 04:16:53.708049 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/linear.py
--rw-r--r--   0        0        0     4037 2023-04-15 04:16:53.708543 neuralprophet-0.6.0rc1/neuralprophet/components/router.py
--rw-r--r--   0        0        0       44 2023-04-15 04:16:53.708862 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/__init__.py
--rw-r--r--   0        0        0      546 2023-04-15 04:16:53.709089 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/base.py
--rw-r--r--   0        0        0     6220 2023-04-15 04:16:53.709368 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/fourier.py
--rw-r--r--   0        0        0       38 2023-04-15 04:16:53.709633 neuralprophet-0.6.0rc1/neuralprophet/components/trend/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-15 04:16:53.709985 neuralprophet-0.6.0rc1/neuralprophet/components/trend/base.py
--rw-r--r--   0        0        0     3826 2023-04-15 04:16:53.710238 neuralprophet-0.6.0rc1/neuralprophet/components/trend/linear.py
--rw-r--r--   0        0        0    16977 2023-04-15 04:16:53.710507 neuralprophet-0.6.0rc1/neuralprophet/components/trend/piecewise_linear.py
--rw-r--r--   0        0        0     1198 2023-04-15 04:16:53.711296 neuralprophet-0.6.0rc1/neuralprophet/components/trend/static.py
--rw-r--r--   0        0        0    16531 2023-04-15 04:16:53.712670 neuralprophet-0.6.0rc1/neuralprophet/configure.py
--rw-r--r--   0        0        0     1841 2023-04-15 04:16:53.714315 neuralprophet-0.6.0rc1/neuralprophet/custom_loss_metrics.py
--rw-r--r--   0        0        0    23809 2023-04-15 04:16:53.715073 neuralprophet-0.6.0rc1/neuralprophet/data/process.py
--rw-r--r--   0        0        0     6803 2023-04-15 04:16:53.716051 neuralprophet-0.6.0rc1/neuralprophet/data/split.py
--rw-r--r--   0        0        0      878 2023-04-15 04:16:53.716561 neuralprophet-0.6.0rc1/neuralprophet/data/transform.py
--rw-r--r--   0        0        0    63826 2023-04-15 04:16:53.717906 neuralprophet-0.6.0rc1/neuralprophet/df_utils.py
--rw-r--r--   0        0        0   121126 2023-04-15 04:16:53.719900 neuralprophet-0.6.0rc1/neuralprophet/forecaster.py
--rw-r--r--   0        0        0      849 2023-04-15 04:16:53.721434 neuralprophet-0.6.0rc1/neuralprophet/hdays_utils.py
--rw-r--r--   0        0        0     2635 2023-04-15 04:16:53.722875 neuralprophet-0.6.0rc1/neuralprophet/logger.py
--rw-r--r--   0        0        0      601 2023-04-14 18:24:09.467754 neuralprophet-0.6.0rc1/neuralprophet/np_types.py
--rw-r--r--   0        0        0    20046 2023-04-15 04:16:53.724158 neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_matplotlib.py
--rw-r--r--   0        0        0    28793 2023-04-15 04:16:53.725746 neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_plotly.py
--rw-r--r--   0        0        0    28822 2023-04-15 04:16:53.726943 neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_matplotlib.py
--rw-r--r--   0        0        0    33617 2023-04-15 04:16:53.728146 neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_plotly.py
--rw-r--r--   0        0        0    25987 2023-04-15 04:16:53.729478 neuralprophet-0.6.0rc1/neuralprophet/plot_utils.py
--rw-r--r--   0        0        0    29297 2023-04-15 04:16:53.731451 neuralprophet-0.6.0rc1/neuralprophet/time_dataset.py
--rw-r--r--   0        0        0    42383 2023-04-15 04:16:53.734947 neuralprophet-0.6.0rc1/neuralprophet/time_net.py
--rw-r--r--   0        0        0    20958 2023-04-14 18:24:09.472906 neuralprophet-0.6.0rc1/neuralprophet/torch_prophet.py
--rw-r--r--   0        0        0    19981 2023-04-15 04:16:53.737476 neuralprophet-0.6.0rc1/neuralprophet/uncertainty.py
--rw-r--r--   0        0        0    31119 2023-04-15 04:16:53.738755 neuralprophet-0.6.0rc1/neuralprophet/utils.py
--rw-r--r--   0        0        0     1679 2023-04-15 04:16:53.739371 neuralprophet-0.6.0rc1/neuralprophet/utils_metrics.py
--rw-r--r--   0        0        0     4542 2023-04-15 04:16:53.740338 neuralprophet-0.6.0rc1/neuralprophet/utils_torch.py
--rw-r--r--   0        0        0     1773 2023-04-15 04:17:13.016717 neuralprophet-0.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     8535 1970-01-01 00:00:00.000000 neuralprophet-0.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-11 03:56:33.361031 neuralprophet-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     7464 2023-04-11 03:56:33.361315 neuralprophet-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     1394 2023-04-21 15:39:58.444129 neuralprophet-1.0.0rc1/neuralprophet/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-11 03:56:33.495958 neuralprophet-1.0.0rc1/neuralprophet/__main__.py
+-rw-r--r--   0        0        0       80 2023-05-01 00:38:34.064106 neuralprophet-1.0.0rc1/neuralprophet/_version.py
+-rw-r--r--   0        0        0      683 2023-04-11 03:56:33.496281 neuralprophet-1.0.0rc1/neuralprophet/components/README.md
+-rw-r--r--   0        0        0       46 2023-04-11 03:56:33.496404 neuralprophet-1.0.0rc1/neuralprophet/components/__init__.py
+-rw-r--r--   0        0        0      931 2023-04-11 03:56:33.496735 neuralprophet-1.0.0rc1/neuralprophet/components/base.py
+-rw-r--r--   0        0        0       49 2023-04-11 03:56:33.496919 neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-11 03:56:33.497045 neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/base.py
+-rw-r--r--   0        0        0     3681 2023-04-11 03:56:33.497213 neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/linear.py
+-rw-r--r--   0        0        0     4037 2023-04-11 03:56:33.497388 neuralprophet-1.0.0rc1/neuralprophet/components/router.py
+-rw-r--r--   0        0        0       44 2023-04-11 03:56:33.497577 neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/__init__.py
+-rw-r--r--   0        0        0      546 2023-04-11 03:56:33.497732 neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/base.py
+-rw-r--r--   0        0        0     6233 2023-04-25 00:15:27.316872 neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/fourier.py
+-rw-r--r--   0        0        0       38 2023-04-11 03:56:33.498092 neuralprophet-1.0.0rc1/neuralprophet/components/trend/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-11 03:56:33.498379 neuralprophet-1.0.0rc1/neuralprophet/components/trend/base.py
+-rw-r--r--   0        0        0     3826 2023-04-11 03:56:33.498530 neuralprophet-1.0.0rc1/neuralprophet/components/trend/linear.py
+-rw-r--r--   0        0        0    16977 2023-04-11 03:56:33.498689 neuralprophet-1.0.0rc1/neuralprophet/components/trend/piecewise_linear.py
+-rw-r--r--   0        0        0     1192 2023-05-01 00:38:34.066678 neuralprophet-1.0.0rc1/neuralprophet/components/trend/static.py
+-rw-r--r--   0        0        0    16539 2023-04-29 03:11:28.086704 neuralprophet-1.0.0rc1/neuralprophet/configure.py
+-rw-r--r--   0        0        0     1841 2023-04-11 03:56:33.499338 neuralprophet-1.0.0rc1/neuralprophet/custom_loss_metrics.py
+-rw-r--r--   0        0        0    30579 2023-04-26 23:04:01.544631 neuralprophet-1.0.0rc1/neuralprophet/data/process.py
+-rw-r--r--   0        0        0    10167 2023-04-26 23:04:01.545927 neuralprophet-1.0.0rc1/neuralprophet/data/split.py
+-rw-r--r--   0        0        0     1066 2023-04-25 00:15:27.319938 neuralprophet-1.0.0rc1/neuralprophet/data/transform.py
+-rw-r--r--   0        0        0    64143 2023-04-26 23:04:01.547169 neuralprophet-1.0.0rc1/neuralprophet/df_utils.py
+-rw-r--r--   0        0        0   129823 2023-05-01 00:38:34.068428 neuralprophet-1.0.0rc1/neuralprophet/forecaster.py
+-rw-r--r--   0        0        0      849 2023-04-11 03:56:33.501111 neuralprophet-1.0.0rc1/neuralprophet/hdays_utils.py
+-rw-r--r--   0        0        0     2635 2023-04-11 03:56:33.501254 neuralprophet-1.0.0rc1/neuralprophet/logger.py
+-rw-r--r--   0        0        0      652 2023-04-25 00:15:27.325505 neuralprophet-1.0.0rc1/neuralprophet/np_types.py
+-rw-r--r--   0        0        0    18839 2023-05-01 00:38:34.069551 neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_matplotlib.py
+-rw-r--r--   0        0        0    30131 2023-05-01 00:38:34.070758 neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_plotly.py
+-rw-r--r--   0        0        0    28822 2023-04-20 23:16:46.978853 neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_matplotlib.py
+-rw-r--r--   0        0        0    33763 2023-04-28 21:18:49.926179 neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_plotly.py
+-rw-r--r--   0        0        0    25991 2023-04-28 21:18:49.926766 neuralprophet-1.0.0rc1/neuralprophet/plot_utils.py
+-rw-r--r--   0        0        0    30218 2023-05-01 00:38:34.072455 neuralprophet-1.0.0rc1/neuralprophet/time_dataset.py
+-rw-r--r--   0        0        0    46087 2023-05-01 00:38:34.074004 neuralprophet-1.0.0rc1/neuralprophet/time_net.py
+-rw-r--r--   0        0        0    20958 2023-04-11 03:56:33.504567 neuralprophet-1.0.0rc1/neuralprophet/torch_prophet.py
+-rw-r--r--   0        0        0    16350 2023-05-01 00:38:34.077835 neuralprophet-1.0.0rc1/neuralprophet/uncertainty.py
+-rw-r--r--   0        0        0    31338 2023-04-28 21:18:49.927939 neuralprophet-1.0.0rc1/neuralprophet/utils.py
+-rw-r--r--   0        0        0     1679 2023-04-11 03:56:33.505366 neuralprophet-1.0.0rc1/neuralprophet/utils_metrics.py
+-rw-r--r--   0        0        0     4697 2023-04-28 21:18:49.928323 neuralprophet-1.0.0rc1/neuralprophet/utils_torch.py
+-rw-r--r--   0        0        0     2323 2023-05-01 00:43:12.288724 neuralprophet-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     9039 1970-01-01 00:00:00.000000 neuralprophet-1.0.0rc1/PKG-INFO
```

### Comparing `neuralprophet-0.6.0rc1/LICENSE` & `neuralprophet-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/README.md` & `neuralprophet-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/__init__.py` & `neuralprophet-1.0.0rc1/neuralprophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/README.md` & `neuralprophet-1.0.0rc1/neuralprophet/components/README.md`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/base.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/base.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/linear.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/router.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/router.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/base.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/fourier.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/fourier.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         Returns
         -------
             torch.Tensor
                 Forecast component of dims (batch, n_forecasts)
         """
         device = s[list(s.keys())[0]].device
         x = torch.zeros(
-            size=(s[list(s.keys())[0]].shape[0], self.n_forecasts, len(self.quantiles)),
+            size=(s[list(s.keys())[0]].shape[0], s[list(s.keys())[0]].shape[1], len(self.quantiles)),
             device=device,
         )
         for name, features in s.items():
             x = x + self.compute_fourier(features, name, meta)
         return x
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/trend/base.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/trend/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/trend/linear.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/trend/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/trend/piecewise_linear.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/trend/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/components/trend/static.py` & `neuralprophet-1.0.0rc1/neuralprophet/components/trend/static.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 Metadata about the all the samples of the model input batch. Contains the following:
                     * ``df_name`` (list, str), time series ID corresponding to each sample of the input batch.
         Returns
         -------
             torch.Tensor
                 Trend component, same dimensions as input t
         """
-        return self.bias.unsqueeze(dim=0).repeat(t.shape[0], self.n_forecasts, 1)
+        return self.bias.unsqueeze(dim=0).repeat(t.shape[0], t.shape[1], 1)
 
     @property
     def get_trend_deltas(self):
         pass
 
     def add_regularization(self):
         pass
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/configure.py` & `neuralprophet-1.0.0rc1/neuralprophet/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 from neuralprophet.custom_loss_metrics import PinballLoss
 
 log = logging.getLogger("NP.config")
 
 
 @dataclass
 class Model:
-    num_hidden_layers: int
-    d_hidden: Optional[int]
+    lagged_reg_layers: Optional[List[int]]
 
 
 @dataclass
 class Normalization:
     normalize: str
     global_normalization: bool
     global_time_normalization: bool
@@ -341,14 +340,15 @@
         self.periods[name] = Season(resolution=resolution, period=period, arg=arg, condition_name=condition_name)
 
 
 @dataclass
 class AR:
     n_lags: int
     ar_reg: Optional[float] = None
+    ar_layers: Optional[List[int]] = None
 
     def __post_init__(self):
         if self.ar_reg is not None and self.ar_reg > 0:
             if self.ar_reg < 0:
                 raise ValueError("regularization must be >= 0")
             self.reg_lambda = 0.0001 * self.ar_reg
         else:
@@ -379,16 +379,15 @@
 
 @dataclass
 class LaggedRegressor:
     reg_lambda: Optional[float]
     as_scalar: bool
     normalize: Union[bool, str]
     n_lags: int
-    num_hidden_layers: Optional[int]
-    d_hidden: Optional[int]
+    lagged_reg_layers: Optional[List[int]]
 
     def __post_init__(self):
         if self.reg_lambda is not None:
             if self.reg_lambda < 0:
                 raise ValueError("regularization must be >= 0")
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/custom_loss_metrics.py` & `neuralprophet-1.0.0rc1/neuralprophet/custom_loss_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/data/transform.py` & `neuralprophet-1.0.0rc1/neuralprophet/data/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import logging
 
 import pandas as pd
 
 from neuralprophet import df_utils
+from neuralprophet.configure import Normalization
 
 log = logging.getLogger("NP.data.transforming")
 
 
-def _normalize(model, df):
+def _normalize(df: pd.DataFrame, config_normalization: Normalization) -> pd.DataFrame:
     """Apply data scales.
 
     Applies data scaling factors to df using data_params.
 
     Parameters
     ----------
         df : pd.DataFrame
             dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
+        config_normalization: Normalization
+            Normalization configuration
 
     Returns
     -------
         df: pd.DataFrame, normalized
     """
     df, _, _, _ = df_utils.prep_or_copy_df(df)
     df_norm = pd.DataFrame()
     for df_name, df_i in df.groupby("ID"):
-        data_params = model.config_normalization.get_data_params(df_name)
+        data_params = config_normalization.get_data_params(df_name)
         df_i.drop("ID", axis=1, inplace=True)
         df_aux = df_utils.normalize(df_i, data_params).copy(deep=True)
         df_aux["ID"] = df_name
         df_norm = pd.concat((df_norm, df_aux), ignore_index=True)
     return df_norm
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/df_utils.py` & `neuralprophet-1.0.0rc1/neuralprophet/df_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
     df: pd.DataFrame,
     check_y: bool = True,
     covariates=None,
     regressors=None,
     events=None,
     seasonalities=None,
     future: Optional[bool] = None,
-) -> Tuple[pd.DataFrame, List]:
+) -> Tuple[pd.DataFrame, List, List]:
     """Performs basic data sanity checks and ordering,
     as well as prepare dataframe for fitting or predicting.
 
     Parameters
     ----------
         df : pd.DataFrame
             containing column ``ds``
@@ -552,37 +552,42 @@
     checked_df = pd.DataFrame()
     for df_name, df_i in df.groupby("ID"):
         df_aux = check_single_dataframe(df_i, check_y, covariates, regressors, events, seasonalities)
         df_aux = df_aux.copy(deep=True)
         df_aux["ID"] = df_name
         checked_df = pd.concat((checked_df, df_aux), ignore_index=True)
     regressors_to_remove = []
+    lag_regressors_to_remove = []
     if regressors is not None:
         for reg in regressors:
             if len(df[reg].unique()) < 2:
                 log.warning(
                     "Encountered future regressor with only unique values in training set across all IDs."
                     "Automatically removed variable."
                 )
                 regressors_to_remove.append(reg)
-    if future:
-        return checked_df, regressors_to_remove
     if covariates is not None:
         for covar in covariates:
             if len(df[covar].unique()) < 2:
                 log.warning(
                     "Encountered lagged regressor with only unique values in training set across all IDs."
                     "Automatically removed variable."
                 )
-                regressors_to_remove.append(covar)
+                lag_regressors_to_remove.append(covar)
+    if future:
+        return checked_df, regressors_to_remove, lag_regressors_to_remove
     if len(regressors_to_remove) > 0:
         regressors_to_remove = list(set(regressors_to_remove))
-        checked_df = checked_df.drop(*regressors_to_remove, axis=1)
+        checked_df = checked_df.drop(regressors_to_remove, axis=1)
+        assert checked_df is not None
+    if len(lag_regressors_to_remove) > 0:
+        lag_regressors_to_remove = list(set(lag_regressors_to_remove))
+        checked_df = checked_df.drop(lag_regressors_to_remove, axis=1)
         assert checked_df is not None
-    return checked_df, regressors_to_remove
+    return checked_df, regressors_to_remove, lag_regressors_to_remove
 
 
 def _crossvalidation_split_df(df, n_lags, n_forecasts, k, fold_pct, fold_overlap_pct=0.0):
     """Splits data in k folds for crossvalidation.
 
     Parameters
     ----------
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/forecaster.py` & `neuralprophet-1.0.0rc1/neuralprophet/forecaster.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     _reshape_raw_predictions_to_forecst_df,
     _validate_column_name,
 )
 from neuralprophet.data.split import _make_future_dataframe, _maybe_extend_df
 from neuralprophet.data.transform import _normalize
 from neuralprophet.logger import MetricsLogger
 from neuralprophet.plot_forecast_matplotlib import plot, plot_components
+from neuralprophet.plot_forecast_plotly import conformal_plot_plotly
 from neuralprophet.plot_forecast_plotly import plot as plot_plotly
 from neuralprophet.plot_forecast_plotly import plot_components as plot_components_plotly
 from neuralprophet.plot_model_parameters_matplotlib import plot_parameters
 from neuralprophet.plot_model_parameters_plotly import plot_parameters as plot_parameters_plotly
 from neuralprophet.plot_utils import get_valid_configuration, log_warning_deprecation_plotly, select_plotting_backend
 from neuralprophet.uncertainty import Conformal
 
@@ -164,24 +165,26 @@
             how much sparsity to induce in the AR-coefficients
 
             Note
             ----
             Large values (~1-100) will limit the number of nonzero coefficients dramatically.
             Small values (~0.001-1.0) will allow more non-zero coefficients.
             default: 0 no regularization of coefficients.
+        ar_layers : list of int, optional
+            array of hidden layer dimensions of the AR-Net. Specifies number of hidden layers (number of entries)
+            and layer dimension (list entry).
 
         COMMENT
         Model Config
         COMMENT
         n_forecasts : int
             Number of steps ahead of prediction time step to forecast.
-        num_hidden_layers : int, optional
-            number of hidden layer to include in AR-Net (defaults to 0)
-        d_hidden : int, optional
-            dimension of hidden layers of the AR-Net. Ignored if ``num_hidden_layers`` == 0.
+        lagged_reg_layers : list of int, optional
+            array of hidden layer dimensions of the Covar-Net. Specifies number of hidden layers (number of entries)
+            and layer dimension (list entry).
 
         COMMENT
         Train Config
         COMMENT
         learning_rate : float
             Maximum learning rate setting for 1cycle policy scheduler.
 
@@ -340,17 +343,17 @@
         weekly_seasonality: np_types.SeasonalityArgument = "auto",
         daily_seasonality: np_types.SeasonalityArgument = "auto",
         seasonality_mode: np_types.SeasonalityMode = "additive",
         seasonality_reg: float = 0,
         season_global_local: np_types.SeasonGlobalLocalMode = "global",
         n_forecasts: int = 1,
         n_lags: int = 0,
-        num_hidden_layers: int = 0,
-        d_hidden: Optional[int] = None,
+        ar_layers: Optional[list] = [],
         ar_reg: Optional[float] = None,
+        lagged_reg_layers: Optional[list] = [],
         learning_rate: Optional[float] = None,
         epochs: Optional[int] = None,
         batch_size: Optional[int] = None,
         loss_func: Union[str, torch.nn.modules.loss._Loss, Callable] = "Huber",
         optimizer: Union[str, Type[torch.optim.Optimizer]] = "AdamW",
         newer_samples_weight: float = 2,
         newer_samples_start: float = 0.0,
@@ -410,26 +413,20 @@
                 DeprecationWarning(
                     "Providing metrics to collect via `collect_metrics` in NeuralProphet is deprecated and will be removed in a future version. The metrics are now configure in the `fit()` method via `metrics`."
                 )
             )
         self.metrics = utils_metrics.get_metrics(collect_metrics)
 
         # AR
-        self.config_ar = configure.AR(
-            n_lags=n_lags,
-            ar_reg=ar_reg,
-        )
+        self.config_ar = configure.AR(n_lags=n_lags, ar_reg=ar_reg, ar_layers=ar_layers)
         self.n_lags = self.config_ar.n_lags
         self.max_lags = self.n_lags
 
         # Model
-        self.config_model = configure.Model(
-            num_hidden_layers=num_hidden_layers,
-            d_hidden=d_hidden,
-        )
+        self.config_model = configure.Model(lagged_reg_layers=lagged_reg_layers)
 
         # Trend
         self.config_trend = configure.Trend(
             growth=growth,
             changepoints=changepoints,
             n_changepoints=n_changepoints,
             changepoints_range=changepoints_range,
@@ -476,16 +473,14 @@
         self.highlight_forecast_step_n = None
         self.true_ar_weights = None
 
     def add_lagged_regressor(
         self,
         names: Union[str, List[str]],
         n_lags: Union[int, np_types.Literal["auto", "scalar"]] = "auto",
-        num_hidden_layers: Optional[int] = None,
-        d_hidden: Optional[int] = None,
         regularization: Optional[float] = None,
         normalize: Union[bool, str] = "auto",
     ):
         """Add a covariate or list of covariate time series as additional lagged regressors to be used for fitting and predicting.
         The dataframe passed to ``fit`` and ``predict`` will have the column with the specified name to be used as
         lagged regressor. When normalize=True, the covariate will be normalized unless it is binary.
 
@@ -493,29 +488,22 @@
         ----------
             names : string or list
                 name of the regressor/list of regressors.
             n_lags : int
                 previous regressors time steps to use as input in the predictor (covar order)
                 if ``auto``, time steps will be equivalent to the AR order (default)
                 if ``scalar``, all the regressors will only use last known value as input
-            num_hidden_layers : int
-                number of hidden layers to include in Lagged-Regressor-Net (defaults to same configuration as AR-Net)
-            d_hidden : int
-                dimension of hidden layers of the Lagged-Regressor-Net. Ignored if ``num_hidden_layers`` == 0.
             regularization : float
                 optional  scale for regularization strength
             normalize : bool
                 optional, specify whether this regressor will benormalized prior to fitting.
                 if ``auto``, binary regressors will not be normalized.
         """
-        if num_hidden_layers is None:
-            num_hidden_layers = self.config_model.num_hidden_layers
+        lagged_reg_layers = self.config_model.lagged_reg_layers
 
-        if d_hidden is None:
-            d_hidden = self.config_model.d_hidden
         if n_lags == 0 or n_lags is None:
             n_lags = 0
             log.warning(
                 "Please, set n_lags to a value greater than 0 or to the options 'scalar' or 'auto'. No lags will be added to regressors when n_lags = 0 or n_lags is None"
             )
         if n_lags == "auto":
             if self.n_lags is not None and self.n_lags > 0:
@@ -533,24 +521,30 @@
             log.info("n_lags = 'scalar', number of lags for regressor is set to 1")
         only_last_value = False if n_lags > 1 else True
         if self.fitted:
             raise Exception("Regressors must be added prior to model fitting.")
         if not isinstance(names, list):
             names = [names]
         for name in names:
-            _validate_column_name(self, name)
+            _validate_column_name(
+                name=name,
+                config_events=self.config_events,
+                config_country_holidays=self.config_country_holidays,
+                config_seasonality=self.config_seasonality,
+                config_lagged_regressors=self.config_lagged_regressors,
+                config_regressors=self.config_regressors,
+            )
             if self.config_lagged_regressors is None:
                 self.config_lagged_regressors = OrderedDict()
             self.config_lagged_regressors[name] = configure.LaggedRegressor(
                 reg_lambda=regularization,
                 normalize=normalize,
                 as_scalar=only_last_value,
                 n_lags=n_lags,
-                num_hidden_layers=num_hidden_layers,
-                d_hidden=d_hidden,
+                lagged_reg_layers=lagged_reg_layers,
             )
         return self
 
     def parameters(self):
         return self.config
 
     def state_dict(self):
@@ -601,15 +595,22 @@
         if self.fitted:
             raise Exception("Regressors must be added prior to model fitting.")
         if regularization is not None:
             if regularization < 0:
                 raise ValueError("regularization must be >= 0")
             if regularization == 0:
                 regularization = None
-        _validate_column_name(self, name)
+        _validate_column_name(
+            name=name,
+            config_events=self.config_events,
+            config_country_holidays=self.config_country_holidays,
+            config_seasonality=self.config_seasonality,
+            config_lagged_regressors=self.config_lagged_regressors,
+            config_regressors=self.config_regressors,
+        )
 
         if self.config_regressors is None:
             self.config_regressors = OrderedDict()
         self.config_regressors[name] = configure.Regressor(reg_lambda=regularization, normalize=normalize, mode=mode)
         return self
 
     def add_events(
@@ -650,15 +651,22 @@
             if regularization == 0:
                 regularization = None
 
         if not isinstance(events, list):
             events = [events]
 
         for event_name in events:
-            _validate_column_name(self, event_name)
+            _validate_column_name(
+                name=event_name,
+                config_events=self.config_events,
+                config_country_holidays=self.config_country_holidays,
+                config_seasonality=self.config_seasonality,
+                config_lagged_regressors=self.config_lagged_regressors,
+                config_regressors=self.config_regressors,
+            )
             self.config_events[event_name] = configure.Event(
                 lower_window=lower_window, upper_window=upper_window, reg_lambda=regularization, mode=mode
             )
         return self
 
     def add_country_holidays(
         self,
@@ -757,17 +765,32 @@
             >>> m.add_seasonality(name="weekly_fall", period=7, fourier_order=4, condition_name="fall")
         """
         if self.fitted:
             raise Exception("Seasonality must be added prior to model fitting.")
         if name in ["daily", "weekly", "yearly"]:
             log.error("Please use inbuilt daily, weekly, or yearly seasonality or set another name.")
         # Do not Allow overwriting built-in seasonalities
-        _validate_column_name(self, name, seasons=True)
+        _validate_column_name(
+            name=name,
+            config_events=self.config_events,
+            config_country_holidays=self.config_country_holidays,
+            config_seasonality=self.config_seasonality,
+            config_lagged_regressors=self.config_lagged_regressors,
+            config_regressors=self.config_regressors,
+            seasons=True,
+        )
         if condition_name is not None:
-            _validate_column_name(self, condition_name)
+            _validate_column_name(
+                name=condition_name,
+                config_events=self.config_events,
+                config_country_holidays=self.config_country_holidays,
+                config_seasonality=self.config_seasonality,
+                config_lagged_regressors=self.config_lagged_regressors,
+                config_regressors=self.config_regressors,
+            )
         if fourier_order <= 0:
             raise ValueError("Fourier Order must be > 0")
         self.config_seasonality.append(
             name=name, period=period, resolution=fourier_order, condition_name=condition_name, arg="custom"
         )
         return self
 
@@ -886,15 +909,26 @@
             progress = None
 
         # Pre-processing
         # Copy df and save list of unique time series IDs (the latter for global-local modelling if enabled)
         df, _, _, self.id_list = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=True, exogenous=True)
         self.data_freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(self, df, freq=self.data_freq)
+        df = _handle_missing_data(
+            df=df,
+            freq=self.data_freq,
+            n_lags=self.n_lags,
+            n_forecasts=self.n_forecasts,
+            config_missing=self.config_missing,
+            config_regressors=self.config_regressors,
+            config_lagged_regressors=self.config_lagged_regressors,
+            config_events=self.config_events,
+            config_seasonality=self.config_seasonality,
+            predicting=False,
+        )
 
         # Setup for global-local modelling: If there is only a single time series, then self.id_list = ['__df__']
         self.num_trends_modelled = len(self.id_list) if self.config_trend.trend_global_local == "local" else 1
         self.num_seasonalities_modelled = len(self.id_list) if self.config_seasonality.global_local == "local" else 1
         self.meta_used_in_model = self.num_trends_modelled != 1 or self.num_seasonalities_modelled != 1
 
         if self.fitted is True and not continue_training:
@@ -917,15 +951,26 @@
                 checkpointing_enabled=checkpointing,
                 continue_training=continue_training,
                 num_workers=num_workers,
             )
         else:
             df_val, _, _, _ = df_utils.prep_or_copy_df(validation_df)
             df_val = _check_dataframe(self, df_val, check_y=False, exogenous=False)
-            df_val = _handle_missing_data(self, df_val, freq=self.data_freq)
+            df_val = _handle_missing_data(
+                df=df_val,
+                freq=self.data_freq,
+                n_lags=self.n_lags,
+                n_forecasts=self.n_forecasts,
+                config_missing=self.config_missing,
+                config_regressors=self.config_regressors,
+                config_lagged_regressors=self.config_lagged_regressors,
+                config_events=self.config_events,
+                config_seasonality=self.config_seasonality,
+                predicting=False,
+            )
             metrics_df = self._train(
                 df,
                 df_val=df_val,
                 progress_bar_enabled=bool(progress),
                 metrics_enabled=bool(self.metrics),
                 checkpointing_enabled=checkpointing,
                 continue_training=continue_training,
@@ -985,33 +1030,55 @@
         """
         if raw:
             log.warning("Raw forecasts are incompatible with plotting utilities")
         if self.fitted is False:
             raise ValueError("Model has not been fitted. Predictions will be random.")
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         # to get all forecasteable values with df given, maybe extend into future:
-        df, periods_added = _maybe_extend_df(self, df)
-        df = _prepare_dataframe_to_predict(self, df)
+        df, periods_added = _maybe_extend_df(
+            df=df,
+            n_forecasts=self.n_forecasts,
+            max_lags=self.max_lags,
+            freq=self.data_freq,
+            config_regressors=self.config_regressors,
+            config_events=self.config_events,
+        )
+        df = _prepare_dataframe_to_predict(model=self, df=df, max_lags=self.max_lags, freq=self.data_freq)
         # normalize
-        df = _normalize(self, df)
+        df = _normalize(df=df, config_normalization=self.config_normalization)
         forecast = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             dates, predicted, components = self._predict_raw(
                 df_i, df_name, include_components=decompose, prediction_frequency=self.prediction_frequency
             )
             df_i = df_utils.drop_missing_from_df(
                 df_i, self.config_missing.drop_missing, self.predict_steps, self.n_lags
             )
             if raw:
-                fcst = _convert_raw_predictions_to_raw_df(self, dates, predicted, components)
+                fcst = _convert_raw_predictions_to_raw_df(
+                    dates=dates,
+                    predicted=predicted,
+                    n_forecasts=self.n_forecasts,
+                    quantiles=self.config_train.quantiles,
+                    components=components,
+                )
                 if periods_added[df_name] > 0:
                     fcst = fcst[:-1]
             else:
                 fcst = _reshape_raw_predictions_to_forecst_df(
-                    self, df_i, predicted, components, self.prediction_frequency, dates
+                    df=df_i,
+                    predicted=predicted,
+                    components=components,
+                    prediction_frequency=self.prediction_frequency,
+                    dates=dates,
+                    n_forecasts=self.n_forecasts,
+                    max_lags=self.max_lags,
+                    freq=self.data_freq,
+                    quantiles=self.config_train.quantiles,
+                    config_lagged_regressors=self.config_lagged_regressors,
                 )
                 if periods_added[df_name] > 0:
                     fcst = fcst[: -periods_added[df_name]]
             forecast = pd.concat((forecast, fcst), ignore_index=True)
         df = df_utils.return_df_in_original_format(forecast, received_ID_col, received_single_time_series)
         self.predict_steps = self.n_forecasts
         return df
@@ -1028,16 +1095,27 @@
             pd.DataFrame
                 evaluation metrics
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
         if self.fitted is False:
             log.warning("Model has not been fitted. Test results will be random.")
         df = _check_dataframe(self, df, check_y=True, exogenous=True)
-        _ = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=self.data_freq)
-        df = _handle_missing_data(self, df, freq=self.data_freq)
+        freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=self.data_freq)
+        df = _handle_missing_data(
+            df=df,
+            freq=freq,
+            n_lags=self.n_lags,
+            n_forecasts=self.n_forecasts,
+            config_missing=self.config_missing,
+            config_regressors=self.config_regressors,
+            config_lagged_regressors=self.config_lagged_regressors,
+            config_events=self.config_events,
+            config_seasonality=self.config_seasonality,
+            predicting=False,
+        )
         loader = self._init_val_loader(df)
         # Use Lightning to calculate metrics
         val_metrics = self.trainer.test(self.model, dataloaders=loader)
         val_metrics_df = pd.DataFrame(val_metrics)
         # TODO Check whether supported by Lightning
         if not self.config_normalization.global_normalization:
             log.warning("Note that the metrics are displayed in normalized scale because of local normalization.")
@@ -1154,15 +1232,26 @@
             0	2022-12-05	7.89	data1
             1	2022-12-13	8.02	data2
             2	2022-12-13	8.30	data3
         """
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(self, df, freq=freq, predicting=False)
+        df = _handle_missing_data(
+            df=df,
+            freq=freq,
+            n_lags=self.n_lags,
+            n_forecasts=self.n_forecasts,
+            config_missing=self.config_missing,
+            config_regressors=self.config_regressors,
+            config_lagged_regressors=self.config_lagged_regressors,
+            config_events=self.config_events,
+            config_seasonality=self.config_seasonality,
+            predicting=False,
+        )
         df_train, df_val = df_utils.split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             valid_p=valid_p,
             inputs_overbleed=True,
             local_split=local_split,
@@ -1322,15 +1411,26 @@
             0	2022-12-10	8.09	data1
             1	2022-12-10	8.25	data2
             2	2022-12-10	7.55	data3
         """
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(self, df, freq=freq, predicting=False)
+        df = _handle_missing_data(
+            df=df,
+            freq=freq,
+            n_lags=self.n_lags,
+            n_forecasts=self.n_forecasts,
+            config_missing=self.config_missing,
+            config_regressors=self.config_regressors,
+            config_lagged_regressors=self.config_lagged_regressors,
+            config_events=self.config_events,
+            config_seasonality=self.config_seasonality,
+            predicting=False,
+        )
         folds = df_utils.crossvalidation_split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             k=k,
             fold_pct=fold_pct,
             fold_overlap_pct=fold_overlap_pct,
@@ -1374,15 +1474,26 @@
         -------
             tuple of k tuples [(folds_val, folds_test), …]
                 elements same as :meth:`crossvalidation_split_df` returns
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(self, df, freq=freq, predicting=False)
+        df = _handle_missing_data(
+            df=df,
+            freq=freq,
+            n_lags=self.n_lags,
+            n_forecasts=self.n_forecasts,
+            config_missing=self.config_missing,
+            config_regressors=self.config_regressors,
+            config_lagged_regressors=self.config_lagged_regressors,
+            config_events=self.config_events,
+            config_seasonality=self.config_seasonality,
+            predicting=False,
+        )
         folds_val, folds_test = df_utils.double_crossvalidation_split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             k=k,
             valid_pct=valid_pct,
             test_pct=test_pct,
@@ -1488,20 +1599,23 @@
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         events_dict = df_utils.create_dict_for_events_or_regressors(df, events_df, "events")
         regressors_dict = df_utils.create_dict_for_events_or_regressors(df, regressors_df, "regressors")
 
         df_future_dataframe = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             df_aux = _make_future_dataframe(
-                self,
+                model=self,
                 df=df_i,
                 events_df=events_dict[df_name],
                 regressors_df=regressors_dict[df_name],
                 periods=periods,
                 n_historic_predictions=n_historic_predictions,
+                n_forecasts=self.n_forecasts,
+                max_lags=self.max_lags,
+                freq=self.data_freq,
             )
             df_aux["ID"] = df_name
             df_future_dataframe = pd.concat((df_future_dataframe, df_aux), ignore_index=True)
 
         df_future = df_utils.return_df_in_original_format(
             df_future_dataframe, received_ID_col, received_single_time_series
         )
@@ -1537,15 +1651,15 @@
                 input df with negative values handled
         """
         # Identify the columns to process
         # Either process the provided columns or default to all columns
         if columns:
             cols = columns
         else:
-            cols = list(df.select_dtypes(include=np.number).columns)
+            cols = list(df.select_dtypes(include=np.number).columns)  # type: ignore
         # Handle the negative values
         for col in cols:
             df = df_utils.handle_negative_values(df, col=col, handle_negatives=handle)
         return df
 
     def predict_trend(self, df: pd.DataFrame, quantile: float = 0.5):
         """Predict only trend component of the model.
@@ -1563,25 +1677,25 @@
                 trend on prediction dates.
         """
         if quantile is not None and not (0 < quantile < 1):
             raise ValueError("The quantile specified need to be a float in-between (0,1)")
 
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
-        df = _normalize(self, df)
+        df = _normalize(df=df, config_normalization=self.config_normalization)
         df_trend = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             t = torch.from_numpy(np.expand_dims(df_i["t"].values, 1))  # type: ignore
 
             # Creating and passing meta, in this case the meta['df_name'] is the ID of the dataframe
             # Note: meta is only used on the trend method if trend_global_local is not "global"
             meta = OrderedDict()
             meta["df_name"] = [df_name for _ in range(t.shape[0])]
             if self.meta_used_in_model:
-                meta_name_tensor = torch.tensor([self.model.id_dict[i] for i in meta["df_name"]])
+                meta_name_tensor = torch.tensor([self.model.id_dict[i] for i in meta["df_name"]])  # type: ignore
             else:
                 meta_name_tensor = None
 
             quantile_index = self.config_train.quantiles.index(quantile)
             trend = self.model.trend(t, meta_name_tensor).detach().numpy()[:, :, quantile_index].squeeze()
 
             data_params = self.config_normalization.get_data_params(df_name)
@@ -1607,15 +1721,15 @@
                 seasonal components with columns of name <seasonality component name>
         """
         if quantile is not None and not (0 < quantile < 1):
             raise ValueError("The quantile specified need to be a float in-between (0,1)")
 
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
-        df = _normalize(self, df)
+        df = _normalize(df=df, config_normalization=self.config_normalization)
         df_seasonal = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             dataset = time_dataset.TimeDataset(
                 df_i,
                 name=df_name,
                 config_seasonality=self.config_seasonality,
                 # n_lags=0,
@@ -1632,15 +1746,15 @@
             for inputs, _, meta in loader:
                 # Meta as a tensor for prediction
                 if self.model.config_seasonality is None:
                     meta_name_tensor = None
                 elif self.model.config_seasonality.global_local == "local":
                     meta = OrderedDict()
                     meta["df_name"] = [df_name for _ in range(inputs["time"].shape[0])]
-                    meta_name_tensor = torch.tensor([self.model.id_dict[i] for i in meta["df_name"]])
+                    meta_name_tensor = torch.tensor([self.model.id_dict[i] for i in meta["df_name"]])  # type: ignore
                 else:
                     meta_name_tensor = None
 
                 for name in self.config_seasonality.periods:
                     features = inputs["seasonalities"][name]
                     quantile_index = self.config_train.quantiles.index(quantile)
                     y_season = torch.squeeze(
@@ -1680,22 +1794,23 @@
             Specifies plotting backend to use for all plots. Can be configured individually for each plot.
 
             Options
                 * ``plotly-resampler``: Use the plotly backend for plotting in resample mode. This mode uses the
                     plotly-resampler package to accelerate visualizing large data by resampling it. Only supported for
                     jupyterlab notebooks and vscode notebooks.
                 * ``plotly``: Use the plotly backend for plotting
+                * ``plotly-static``: Use the plotly backend to generate static svg
                 * ``matplotlib``: use matplotlib for plotting
         """
-        if plotting_backend in ["plotly", "matplotlib", "plotly-resampler"]:
+        if plotting_backend in ["plotly", "matplotlib", "plotly-resampler", "plotly-static"]:
             self.plotting_backend = plotting_backend
             log_warning_deprecation_plotly(self.plotting_backend)
         else:
             raise ValueError(
-                "The parameter `plotting_backend` must be either 'plotly', 'plotly-resampler' or 'matplotlib'."
+                "The parameter `plotting_backend` must be either 'plotly', 'plotly-resampler', 'plotly-resampler' or 'matplotlib'."
             )
 
     def highlight_nth_step_ahead_of_each_forecast(self, step_number: Optional[int] = None):
         """Set which forecast step to focus on for metrics evaluation and plotting.
 
         Parameters
         ----------
@@ -1743,14 +1858,15 @@
 
                 Options
                 * ``plotly-resampler``: Use the plotly backend for plotting in resample mode. This mode uses the
                     plotly-resampler package to accelerate visualizing large data by resampling it. For some
                     environments (colab, pycharm interpreter) plotly-resampler might not properly vizualise the figures.
                     In this case, consider switching to 'plotly-auto'.
                 * ``plotly``: Use the plotly backend for plotting
+                * ``plotly-static``: Use the plotly backend to generate static svg
                 * ``matplotlib``: use matplotlib for plotting
                 * (default) None: Plotting backend ist set automatically. Use plotly with resampling for jupyterlab
                     notebooks and vscode notebooks. Automatically switch to plotly without resampling for all other
                     environments.
             forecast_in_focus: int
                 optinal, i-th step ahead forecast to plot
 
@@ -1812,14 +1928,15 @@
                 fcst=fcst,
                 quantiles=self.config_train.quantiles,
                 xlabel=xlabel,
                 ylabel=ylabel,
                 figsize=tuple(x * 70 for x in figsize),
                 highlight_forecast=forecast_in_focus,
                 resampler_active=plotting_backend == "plotly-resampler",
+                plotly_static=plotting_backend == "plotly-static",
             )
         else:
             return plot(
                 fcst=fcst,
                 quantiles=self.config_train.quantiles,
                 ax=ax,
                 xlabel=xlabel,
@@ -1930,18 +2047,20 @@
 
                 Options
                 * ``plotly-resampler``: Use the plotly backend for plotting in resample mode. This mode uses the
                     plotly-resampler package to accelerate visualizing large data by resampling it. For some
                     environments (colab, pycharm interpreter) plotly-resampler might not properly vizualise the figures.
                     In this case, consider switching to 'plotly-auto'.
                 * ``plotly``: Use the plotly backend for plotting
+                * ``plotly-static``: Use the plotly backend to generate static svg
                 * ``matplotlib``: use matplotlib for plotting
                 ** (default) None: Plotting backend ist set automatically. Use plotly with resampling for jupyterlab
                     notebooks and vscode notebooks. Automatically switch to plotly without resampling for all other
                     environments.
+                * (default) None
         Returns
         -------
             matplotlib.axes.Axes
                 plot of NeuralProphet forecasting
         """
         if self.max_lags == 0:
             raise ValueError("Use the standard plot function for models without lags.")
@@ -1980,14 +2099,15 @@
                 quantiles=self.config_train.quantiles,
                 ylabel=ylabel,
                 xlabel=xlabel,
                 figsize=tuple(x * 70 for x in figsize),
                 highlight_forecast=self.highlight_forecast_step_n,
                 line_per_origin=True,
                 resampler_active=plotting_backend == "plotly-resampler",
+                plotly_static=plotting_backend == "plotly-static",
             )
         else:
             return plot(
                 fcst=fcst,
                 quantiles=self.config_train.quantiles,
                 ax=ax,
                 ylabel=ylabel,
@@ -2052,14 +2172,15 @@
 
                 Options
                 * ``plotly-resampler``: Use the plotly backend for plotting in resample mode. This mode uses the
                     plotly-resampler package to accelerate visualizing large data by resampling it. For some
                     environments (colab, pycharm interpreter) plotly-resampler might not properly vizualise the figures.
                     In this case, consider switching to 'plotly-auto'.
                 * ``plotly``: Use the plotly backend for plotting
+                * ``plotly-static``: Use the plotly backend to generate static svg
                 * ``matplotlib``: use matplotlib for plotting
                 * (default) None: Plotting backend ist set automatically. Use plotly with resampling for jupyterlab
                     notebooks and vscode notebooks. Automatically switch to plotly without resampling for all other
                     environments.
             components: str or list, optional
                 name or list of names of components to plot
 
@@ -2143,14 +2264,15 @@
                 m=self,
                 fcst=fcst,
                 plot_configuration=valid_plot_configuration,
                 figsize=tuple(x * 70 for x in figsize) if figsize else (700, 210),
                 df_name=df_name,
                 one_period_per_season=one_period_per_season,
                 resampler_active=plotting_backend == "plotly-resampler",
+                plotly_static=plotting_backend == "plotly-static",
             )
         else:
             return plot_components(
                 m=self,
                 fcst=fcst,
                 plot_configuration=valid_plot_configuration,
                 quantile=self.config_train.quantiles[0],  # plot components only for median quantile
@@ -2206,23 +2328,23 @@
 
                 Options
                 * ``plotly-resampler``: Use the plotly backend for plotting in resample mode. This mode uses the
                     plotly-resampler package to accelerate visualizing large data by resampling it. For some
                     environments (colab, pycharm interpreter) plotly-resampler might not properly vizualise the figures.
                     In this case, consider switching to 'plotly-auto'.
                 * ``plotly``: Use the plotly backend for plotting
+                * ``plotly-static``: Use the plotly backend to generate static svg
                 * ``matplotlib``: use matplotlib for plotting
                 * (default) None: Plotting backend ist set automatically. Use plotly with resampling for jupyterlab
                     notebooks and vscode notebooks. Automatically switch to plotly without resampling for all other
                     environments.
 
                 Note
                 ----
                 For multiple time series and local modeling of at least one component, the df_name parameter is required.
-
             quantile : float
                 The quantile for which the model parameters are to be plotted
 
                 Note
                 ----
                 None (default):  Parameters will be plotted for the median quantile.
 
@@ -2288,25 +2410,41 @@
         )
 
         # Check whether a local or global plotting backend is set.
         plotting_backend = select_plotting_backend(model=self, plotting_backend=plotting_backend)
 
         log_warning_deprecation_plotly(plotting_backend)
         if plotting_backend.startswith("plotly"):
-            return plot_parameters_plotly(
-                m=self,
-                quantile=quantile,
-                weekly_start=weekly_start,
-                yearly_start=yearly_start,
-                figsize=tuple(x * 70 for x in figsize) if figsize else (700, 210),
-                df_name=valid_plot_configuration["df_name"],
-                plot_configuration=valid_plot_configuration,
-                forecast_in_focus=forecast_in_focus,
-                resampler_active=plotting_backend == "plotly-resampler",
-            )
+            if plotting_backend == "plotly-static":
+                fig = plot_parameters_plotly(
+                    m=self,
+                    quantile=quantile,
+                    weekly_start=weekly_start,
+                    yearly_start=yearly_start,
+                    figsize=tuple(x * 70 for x in figsize) if figsize else (700, 210),
+                    df_name=valid_plot_configuration["df_name"],
+                    plot_configuration=valid_plot_configuration,
+                    forecast_in_focus=forecast_in_focus,
+                    resampler_active=plotting_backend == "plotly-resampler",
+                    plotly_static=plotting_backend == "plotly-static",
+                )
+                fig.show("svg")
+            else:
+                return plot_parameters_plotly(
+                    m=self,
+                    quantile=quantile,
+                    weekly_start=weekly_start,
+                    yearly_start=yearly_start,
+                    figsize=tuple(x * 70 for x in figsize) if figsize else (700, 210),
+                    df_name=valid_plot_configuration["df_name"],
+                    plot_configuration=valid_plot_configuration,
+                    forecast_in_focus=forecast_in_focus,
+                    resampler_active=plotting_backend == "plotly-resampler",
+                    plotly_static=plotting_backend == "plotly-static",
+                )
         else:
             return plot_parameters(
                 m=self,
                 quantile=quantile,
                 weekly_start=weekly_start,
                 yearly_start=yearly_start,
                 figsize=figsize,
@@ -2331,16 +2469,16 @@
             config_regressors=self.config_regressors,
             config_events=self.config_events,
             config_holidays=self.config_country_holidays,
             config_normalization=self.config_normalization,
             n_forecasts=self.n_forecasts,
             n_lags=self.n_lags,
             max_lags=self.max_lags,
-            num_hidden_layers=self.config_model.num_hidden_layers,
-            d_hidden=self.config_model.d_hidden,
+            ar_layers=self.config_ar.ar_layers,
+            lagged_reg_layers=self.config_model.lagged_reg_layers,
             metrics=self.metrics,
             id_list=self.id_list,
             num_trends_modelled=self.num_trends_modelled,
             num_seasonalities_modelled=self.num_seasonalities_modelled,
             meta_used_in_model=self.meta_used_in_model,
         )
         log.debug(self.model)
@@ -2366,20 +2504,20 @@
             df=df,
             config_lagged_regressors=self.config_lagged_regressors,
             config_regressors=self.config_regressors,
             config_events=self.config_events,
             config_seasonality=self.config_seasonality,
         )
 
-        df = _normalize(self, df)
+        df = _normalize(df=df, config_normalization=self.config_normalization)
         # if not self.fitted:
         if self.config_trend.changepoints is not None:
             # scale user-specified changepoint times
             df_aux = pd.DataFrame({"ds": pd.Series(self.config_trend.changepoints)})
-            self.config_trend.changepoints = _normalize(self, df_aux)["t"].values  # type: ignore # types are numpy.ArrayLike and list
+            self.config_trend.changepoints = _normalize(df=df_aux, config_normalization=self.config_normalization)["t"].values  # type: ignore # types are numpy.ArrayLike and list
 
         # df_merged, _ = df_utils.join_dataframes(df)
         # df_merged = df_merged.sort_values("ds")
         # df_merged.drop_duplicates(inplace=True, keep="first", subset=["ds"])
         df_merged = df_utils.merge_dataframes(df)
         self.config_seasonality = utils.set_auto_seasonalities(df_merged, config_seasonality=self.config_seasonality)
         if self.config_country_holidays is not None:
@@ -2388,15 +2526,20 @@
         dataset = _create_dataset(
             self, df, predict_mode=False, prediction_frequency=self.prediction_frequency
         )  # needs to be called after set_auto_seasonalities
 
         # Determine the max_number of epochs
         self.config_train.set_auto_batch_epoch(n_data=len(dataset))
 
-        loader = DataLoader(dataset, batch_size=self.config_train.batch_size, shuffle=True, num_workers=num_workers)
+        loader = DataLoader(
+            dataset,
+            batch_size=self.config_train.batch_size,
+            shuffle=True,
+            num_workers=num_workers,
+        )
 
         return loader
 
     def _init_val_loader(self, df):
         """Executes data preparation steps and initiates evaluation procedure.
 
         Parameters
@@ -2405,15 +2548,15 @@
                 dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
 
         Returns
         -------
             torch DataLoader
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
-        df = _normalize(self, df)
+        df = _normalize(df=df, config_normalization=self.config_normalization)
         dataset = _create_dataset(self, df, predict_mode=False)
         loader = DataLoader(dataset, batch_size=min(1024, len(dataset)), shuffle=False, drop_last=False)
         return loader
 
     def _train(
         self,
         df: pd.DataFrame,
@@ -2617,15 +2760,17 @@
         loader = DataLoader(dataset, batch_size=min(1024, len(df)), shuffle=False, drop_last=False)
         if self.n_forecasts > 1:
             dates = df["ds"].iloc[self.max_lags : -self.n_forecasts + 1]
         else:
             dates = df["ds"].iloc[self.max_lags :]
 
         # Pass the include_components flag to the model
-        self.model.set_compute_components(include_components)
+        if include_components:
+            self.model.set_compute_components(include_components)
+            self.model.set_covar_weights(self.model.get_covar_weights())
         # Compute the predictions and components (if requested)
         result = self.trainer.predict(self.model, loader)
         # Extract the prediction and components
         predicted, component_vectors = zip(*result)
         predicted = np.concatenate(predicted)
 
         # Post-process and normalize the predictions
@@ -2688,14 +2833,15 @@
     def conformal_predict(
         self,
         df: pd.DataFrame,
         calibration_df: pd.DataFrame,
         alpha: Union[float, Tuple[float, float]],
         method: str = "naive",
         plotting_backend: Optional[str] = None,
+        show_all_PI: bool = False,
         **kwargs,
     ) -> pd.DataFrame:
         """Apply a given conformal prediction technique to get the uncertainty prediction intervals (or q-hats). Then predict.
 
         Parameters
         ----------
             df : pd.DataFrame
@@ -2720,33 +2866,80 @@
                     environments (colab, pycharm interpreter) plotly-resampler might not properly vizualise the figures.
                     In this case, consider switching to 'plotly-auto'.
                     * ``plotly``: Use the plotly backend for plotting
                     * ``matplotlib``: Use matplotlib backend for plotting
                     * (default) None: Plotting backend ist set automatically. Use plotly with resampling for jupyterlab
                     notebooks and vscode notebooks. Automatically switch to plotly without resampling for all other
                     environments.
+            show_all_PI : bool
+                whether to return all prediction intervals (including quantile regression and conformal prediction)
             kwargs : dict
                 additional predict parameters for test df
 
         Returns
         -------
             pd.DataFrame, Optional[pd.DataFrame]
                 test dataframe with the conformal prediction intervals and evaluation dataframe if evaluate set to True
         """
         # get predictions for calibration dataframe
         df_cal = self.predict(calibration_df)
         # get predictions for test dataframe
         df_test = self.predict(df, **kwargs)
+
         # initiate Conformal instance
         c = Conformal(
             alpha=alpha,
             method=method,
             n_forecasts=self.n_forecasts,
             quantiles=self.config_train.quantiles,
         )
-        # call Conformal's predict to output test df with conformal prediction intervals
-        df_forecast = c.predict(df=df_test, df_cal=df_cal)
+
+        df_forecast = c.predict(df=df_test, df_cal=df_cal, show_all_PI=show_all_PI)
+
         # plot one-sided prediction interval width with q
         if plotting_backend:
             c.plot(plotting_backend)
 
         return df_forecast
+
+    def conformal_plot(
+        self,
+        df: pd.DataFrame,
+        n_highlight: Optional[int] = 1,
+        plotting_backend: Optional[str] = None,
+    ):
+        """Plot conformal prediction intervals and quantile regression intervals.
+
+        Parameters
+        ----------
+            df : pd.DataFrame
+                conformal forecast dataframe when ``show_all_PI`` is set to True
+            n_highlight : Optional
+                i-th step ahead forecast to use for statistics and plotting.
+        """
+        if not any("+" in col for col in df.columns):
+            raise ValueError(
+                "Conformal prediction intervals not found. Please set `show_all_PI` to True when calling `conformal_predict`."
+            )
+
+        # quantile regression dataframe
+        cols = list(df.columns)
+        qr_cols = [col for col in df.columns if "%" in col and "qhat" not in col]
+        forecast_cols = cols[: self.n_forecasts + 2]
+        df_qr = df[forecast_cols + qr_cols]
+
+        fig = self.highlight_nth_step_ahead_of_each_forecast(n_highlight).plot(df_qr, plotting_backend="plotly")
+
+        # get conformal prediction intervals
+        cp_cols = [col for col in df.columns if f"qhat{n_highlight}" in col]
+
+        plotting_backend = select_plotting_backend(model=self, plotting_backend=plotting_backend)
+        if plotting_backend.startswith("plotly"):
+            return conformal_plot_plotly(
+                fig, df.loc[:, ["ds", cp_cols[0]]], df.loc[:, ["ds", cp_cols[1]]], plotting_backend
+            )
+        else:
+            log.warning(
+                DeprecationWarning(
+                    "Matplotlib plotting backend is deprecated and will be removed in a future release. Please use the plotly backend instead."
+                )
+            )
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/hdays_utils.py` & `neuralprophet-1.0.0rc1/neuralprophet/hdays_utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/logger.py` & `neuralprophet-1.0.0rc1/neuralprophet/logger.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/np_types.py` & `neuralprophet-1.0.0rc1/neuralprophet/np_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 from typing import Dict, List, Union
 
+import torch
 import torchmetrics
 
 # Ensure compatibility with python 3.7
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -17,7 +18,9 @@
 SeasonalityArgument = Union[Literal["auto"], bool, int]
 
 GrowthMode = Literal["off", "linear", "discontinuous"]
 
 CollectMetricsMode = Union[List[str], bool, Dict[str, torchmetrics.Metric]]
 
 SeasonGlobalLocalMode = Literal["global", "local"]
+
+Components = Dict[str, torch.Tensor]
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_matplotlib.py` & `neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_matplotlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,47 +84,43 @@
     ds = fcst["ds"].dt.to_pydatetime()
     colname = "yhat"
     step = 1
     # if plot_latest_forecast(), column names become "origin-x", with origin-0 being the latest forecast
     if line_per_origin:
         colname = "origin-"
         step = 0
-    # all yhat column names, including quantiles
-    yhat_col_names = [col_name for col_name in fcst.columns if f"{colname}" in col_name]
-    # without quants
-    yhat_col_names_no_qts = [
-        col_name for col_name in yhat_col_names if f"{colname}" in col_name and "%" not in col_name
-    ]
+    # all yhat column names without quantiles
+    yhat_col_names = [col_name for col_name in fcst.columns if col_name.startswith(colname) and "%" not in col_name]
 
     if highlight_forecast is None or line_per_origin:
-        for i, name in enumerate(yhat_col_names_no_qts):
+        for i, name in enumerate(yhat_col_names):
             ax.plot(
                 ds,
                 fcst[f"{colname}{i if line_per_origin else i + 1}"],
                 ls="-",
                 c="#0072B2",
                 alpha=0.2 + 2.0 / (i + 2.5),
                 label=name,
             )
 
-    if len(quantiles) > 1:
-        for i in range(1, len(quantiles)):
-            ax.fill_between(
-                ds,
-                fcst[f"{colname}{step}"],
-                fcst[f"{colname}{step} {round(quantiles[i] * 100, 1)}%"],
-                color="#0072B2",
-                alpha=0.2,
-            )
+        if len(quantiles) > 1:
+            for i in range(1, len(quantiles)):
+                ax.fill_between(
+                    ds,
+                    fcst[f"{colname}{step}"],
+                    fcst[f"{colname}{step} {round(quantiles[i] * 100, 1)}%"],
+                    color="#0072B2",
+                    alpha=0.2,
+                )
 
     if highlight_forecast is not None:
         if line_per_origin:
             num_forecast_steps = sum(fcst["origin-0"].notna())
             steps_from_last = num_forecast_steps - highlight_forecast
-            for i in range(len(yhat_col_names_no_qts)):
+            for i in range(len(yhat_col_names)):
                 x = ds[-(1 + i + steps_from_last)]
                 y = fcst[f"origin-{i}"].values[-(1 + i + steps_from_last)]
                 ax.plot(x, y, "bx")
         else:
             ax.plot(ds, fcst[f"yhat{highlight_forecast}"], ls="-", c="b", label=f"yhat{highlight_forecast}")
             ax.plot(ds, fcst[f"yhat{highlight_forecast}"], "bx", label=f"yhat{highlight_forecast}")
 
@@ -134,28 +130,14 @@
                         ds,
                         fcst[f"yhat{highlight_forecast}"],
                         fcst[f"yhat{highlight_forecast} {round(quantiles[i] * 100, 1)}%"],
                         color="#0072B2",
                         alpha=0.2,
                     )
 
-    # Plot any conformal prediction intervals
-    if any("+ qhat" in col for col in yhat_col_names) and any("- qhat" in col for col in yhat_col_names):
-        quantile_hi = str(max(quantiles) * 100)
-        quantile_lo = str(min(quantiles) * 100)
-        if f"yhat1 {quantile_hi}% + qhat_hi1" in fcst.columns and f"yhat1 {quantile_lo}% - qhat_lo1" in fcst.columns:
-            ax.plot(ds, fcst[f"yhat1 {quantile_hi}% + qhat_hi1"], c="r", label=f"yhat1 {quantile_hi}% + qhat_hi1")
-            ax.plot(ds, fcst[f"yhat1 {quantile_lo}% - qhat_lo1"], c="r", label=f"yhat1 {quantile_lo}% - qhat_lo1")
-        elif f"yhat1 {quantile_hi}% + qhat1" in fcst.columns and f"yhat1 {quantile_hi}% - qhat1" in fcst.columns:
-            ax.plot(ds, fcst[f"yhat1 {quantile_hi}% + qhat1"], c="r", label=f"yhat1 {quantile_hi}% + qhat1")
-            ax.plot(ds, fcst[f"yhat1 {quantile_lo}% - qhat1"], c="r", label=f"yhat1 {quantile_lo}% - qhat1")
-        else:
-            ax.plot(ds, fcst["yhat1 + qhat1"], c="r", label="yhat1 + qhat1")
-            ax.plot(ds, fcst["yhat1 - qhat1"], c="r", label="yhat1 - qhat1")
-
     ax.plot(ds, fcst["y"], "k.", label="actual y")
 
     # Specify formatting to workaround matplotlib issue #12925
     locator = AutoDateLocator(interval_multiples=False)
     formatter = AutoDateFormatter(locator)
     ax.xaxis.set_major_locator(locator)
     ax.xaxis.set_major_formatter(formatter)
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_plotly.py` & `neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_plotly.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     quantiles,
     xlabel="ds",
     ylabel="y",
     highlight_forecast=None,
     line_per_origin=False,
     figsize=(700, 210),
     resampler_active=False,
+    plotly_static=False,
 ):
     """
     Plot the NeuralProphet forecast
 
     Parameters
     ---------
         fcst : pd.DataFrame
@@ -69,14 +70,16 @@
             i-th step ahead forecast to highlight.
         line_per_origin : bool
             Print a line per forecast of one per forecast age
         figsize : tuple
             Width, height in inches.
         resampler_active : bool
             Flag whether to activate the plotly-resampler
+        plotly_static: bool
+            Flag whether to generate a static svg image
 
     Returns
     -------
         Plotly figure
     """
     if resampler_active:
         register_plotly_resampler(mode="auto")
@@ -91,24 +94,20 @@
     ds = fcst["ds"].dt.to_pydatetime()
     colname = "yhat"
     step = 1
     # if plot_latest_forecast(), column names become "origin-x", with origin-0 being the latest forecast
     if line_per_origin:
         colname = "origin-"
         step = 0
-    # all yhat column names, including quantiles
-    yhat_col_names = [col_name for col_name in fcst.columns if f"{colname}" in col_name]
-    # without quants
-    yhat_col_names_no_qts = [
-        col_name for col_name in yhat_col_names if f"{colname}" in col_name and "%" not in col_name
-    ]
+    # all yhat column names
+    yhat_col_names = [col_name for col_name in fcst.columns if col_name.startswith(colname) and "%" not in col_name]
     data = []
 
     if highlight_forecast is None or line_per_origin:
-        for i, yhat_col_name in enumerate(yhat_col_names_no_qts):
+        for i, yhat_col_name in enumerate(yhat_col_names):
             data.append(
                 go.Scatter(
                     name=yhat_col_name,
                     x=ds,
                     y=fcst[f"{colname}{i if line_per_origin else i + 1}"],
                     mode="lines",
                     line=dict(color=f"rgba(45, 146, 255, {0.2 + 2.0 / (i + 2.5)})", width=line_width),
@@ -146,15 +145,15 @@
                     )
                 )
 
     if highlight_forecast is not None:
         if line_per_origin:
             num_forecast_steps = sum(fcst["origin-0"].notna())
             steps_from_last = num_forecast_steps - highlight_forecast
-            for i, yhat_col_name in enumerate(yhat_col_names_no_qts):
+            for i, yhat_col_name in enumerate(yhat_col_names):
                 x = [ds[-(1 + i + steps_from_last)]]
                 y = [fcst[f"origin-{i}"].values[-(1 + i + steps_from_last)]]
                 data.append(
                     go.Scatter(
                         name=yhat_col_name,
                         x=x,
                         y=y,
@@ -222,25 +221,29 @@
             rangeslider=dict(visible=True),
             **xaxis_args,
         ),
         yaxis=go.layout.YAxis(title=ylabel, **yaxis_args),
         **layout_args,
     )
     fig = go.Figure(data=data, layout=layout)
+    unregister_plotly_resampler()
+    if plotly_static:
+        fig = fig.show("svg")
     return fig
 
 
 def plot_components(
     m,
     fcst,
     plot_configuration,
     df_name="__df__",
     one_period_per_season=False,
     figsize=(700, 210),
     resampler_active=False,
+    plotly_static=False,
 ):
     """
     Plot the NeuralProphet forecast components.
 
     Parameters
     ----------
         m : NeuralProphet
@@ -253,14 +256,16 @@
             ID from time series that should be plotted
         one_period_per_season : bool
             Plot one period per season, instead of the true seasonal components of the forecast.
         figsize : tuple
             Width, height in inches.
         resampler_active : bool
             Flag whether to activate the plotly-resampler
+        plotly_static: bool
+            Flag whether to generate a static svg image
 
     Returns
     -------
         Plotly figure
     """
     log.debug("Plotting forecast components")
     if resampler_active:
@@ -333,14 +338,17 @@
         for trace in trace_object["traces"]:
             fig.add_trace(trace, row=j + 1, col=1)  # adapt var name to plotly-resampler
         fig.update_layout(legend={"y": 0.1, "traceorder": "reversed"})
 
     # Reset multiplicative axes labels after tight_layout adjustment
     for ax in multiplicative_axes:
         ax = set_y_as_percent(ax)
+    unregister_plotly_resampler()
+    if plotly_static:
+        fig = fig.show("svg")
     return fig
 
 
 def get_forecast_component_props(
     fcst,
     comp_name,
     plot_name=None,
@@ -810,14 +818,15 @@
             y=q_hi,
             annotation_text=f"q1_hi = {round(q_hi, 2)}",
             annotation_position="bottom left",
             line_width=1,
             line_color="red",
         )
         fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
+        unregister_plotly_resampler()
         return fig
 
 
 def plot_interval_width_per_timestep(q_hats, method, resampler_active=False):
     """Plot the nonconformity scores as well as the one-sided interval width (q).
 
     Parameters
@@ -869,8 +878,38 @@
             x="Timestep Number",
             y=["One-Sided Lower Interval Width", "One-Sided Upper Interval Width"],
             title=f"{method} One-Sided Interval Width with q per Timestep",
             width=600,
             height=400,
         )
     fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
+    unregister_plotly_resampler()
+    return fig
+
+
+def conformal_plot_plotly(fig, df_cp_lo, df_cp_hi, plotting_backend):
+    """Plot conformal prediction intervals and quantile regression intervals in one plot
+
+    Parameters
+    ----------
+        fig : plotly.graph_objects.Figure
+            Figure showing the quantile regression intervals
+        df_cp_lo : dataframe
+            dataframe containing the lower bound of the conformal prediction intervals
+        df_cp_hi : dataframe
+            dataframe containing the upper bound of the conformal prediction intervals
+    """
+    col_lo = df_cp_lo.columns
+    trace_cp_lo = go.Scatter(
+        name=f"cp_{col_lo[1]}", x=df_cp_lo["ds"], y=df_cp_lo[col_lo[1]], mode="lines", line=dict(color="red")
+    )
+
+    col_hi = df_cp_hi.columns
+    trace_cp_hi = go.Scatter(
+        name=f"cp_{col_hi[1]}", x=df_cp_hi["ds"], y=df_cp_hi[col_hi[1]], mode="lines", line=dict(color="red")
+    )
+
+    fig.add_trace(trace_cp_lo)
+    fig.add_trace(trace_cp_hi)
+    if plotting_backend == "plotly-static":
+        fig = fig.show("svg")
     return fig
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_matplotlib.py` & `neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_matplotlib.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_plotly.py` & `neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,14 +813,15 @@
     quantile=0.5,
     weekly_start=0,
     yearly_start=0,
     figsize=(700, 210),
     df_name=None,
     forecast_in_focus=None,
     resampler_active=False,
+    plotly_static=False,
 ):
     """Plot the parameters that the model is composed of, visually.
 
     Parameters
     ----------
         m : NeuralProphet
             Fitted model
@@ -856,14 +857,16 @@
             optinal, i-th step ahead forecast to plot
 
             Note
             ----
             None (default): plot self.highlight_forecast_step_n by default
         resampler_active : bool
             Flag whether to activate the plotly-resampler
+        plotly_static: bool
+            Flag whether to generate a static svg image
 
     Returns:
         Plotly figure
     """
     if resampler_active:
         register_plotly_resampler(mode="auto")
     else:
@@ -951,9 +954,9 @@
 
         xaxis.update(trace_object["xaxis"])
         yaxis.update(trace_object["yaxis"])
         xaxis.update(**xaxis_args)
         yaxis.update(**yaxis_args)
         for trace in trace_object["traces"]:
             fig.add_trace(trace, row=i + 1, col=1)  # adapt var name to plotly-resampler
-
+        unregister_plotly_resampler()
     return fig
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/plot_utils.py` & `neuralprophet-1.0.0rc1/neuralprophet/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,21 +400,21 @@
                             "plot_name": f'Lagged Regressor "{name}" ({forecast_in_focus})-ahead',
                             "comp_name": f"lagged_regressor_{name}{forecast_in_focus}",
                         }
                     )
         elif validator == "plot_parameters":
             for name in m.config_lagged_regressors.keys():
                 if m.config_lagged_regressors[name].as_scalar:
-                    lagged_scalar_regressors.append((name, m.model.get_covar_weights(name).detach().numpy()))
+                    lagged_scalar_regressors.append((name, m.model.get_covar_weights()[name].detach().numpy()))
                 else:
                     plot_components.append(
                         {
                             "plot_name": "lagged weights",
                             "comp_name": f'Lagged Regressor "{name}"',
-                            "weights": m.model.get_covar_weights(name).detach().numpy(),
+                            "weights": m.model.get_covar_weights()[name].detach().numpy(),
                             "focus": forecast_in_focus,
                         }
                     )
 
     # Add Events
     additive_events = []
     multiplicative_events = []
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/time_dataset.py` & `neuralprophet-1.0.0rc1/neuralprophet/time_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,77 +14,77 @@
 
 log = logging.getLogger("NP.time_dataset")
 
 
 class GlobalTimeDataset(Dataset):
     def __init__(self, df, **kwargs):
         """Initialize Timedataset from time-series df.
-
         Parameters
         ----------
             df : pd.DataFrame
                 dataframe containing column ``ds``, ``y``, and optionally``ID`` and
                 normalized columns normalized columns ``ds``, ``y``, ``t``, ``y_scaled``
             **kwargs : dict
                 Identical to :meth:`tabularize_univariate_datetime`
         """
-        self.combined_timedataset = []
-        # TODO (future): vectorize
-        self.length = 0
-        for df_name, df_i in df.groupby("ID"):
-            timedataset = TimeDataset(df_i, df_name, **kwargs)
-            self.length += timedataset.length
-            for i in range(0, len(timedataset)):
-                self.combined_timedataset.append(timedataset[i])
+        # # TODO (future): vectorize
+        timedatasets = [TimeDataset(df_i, df_name, **kwargs) for df_name, df_i in df.groupby("ID")]
+        self.combined_timedataset = [item for timedataset in timedatasets for item in timedataset]
+        self.length = sum(timedataset.length for timedataset in timedatasets)
 
     def __len__(self):
         return self.length
 
     def __getitem__(self, idx):
         return self.combined_timedataset[idx]
 
 
 class TimeDataset(Dataset):
     """Create a PyTorch dataset of a tabularized time-series"""
 
     def __init__(self, df, name, **kwargs):
         """Initialize Timedataset from time-series df.
-
         Parameters
         ----------
             df : pd.DataFrame
                 Time series data
             name : str
                 Name of time-series
             **kwargs : dict
                 Identical to :meth:`tabularize_univariate_datetime`
         """
         self.name = name
         self.length = None
         self.inputs = OrderedDict({})
         self.targets = None
         self.meta = OrderedDict({})
-        self.two_level_inputs = ["seasonalities", "covariates"]
+        self.two_level_inputs = [
+            "seasonalities",
+            "covariates",
+            "events",
+            "regressors",
+        ]
         inputs, targets, drop_missing = tabularize_univariate_datetime(df, **kwargs)
         self.init_after_tabularized(inputs, targets)
         self.filter_samples_after_init(kwargs["prediction_frequency"])
         self.drop_nan_after_init(df, kwargs["predict_steps"], drop_missing)
 
     def drop_nan_after_init(self, df, predict_steps, drop_missing):
         """Checks if inputs/targets contain any NaN values and drops them, if user opts to.
-
         Parameters
         ----------
             drop_missing : bool
                 whether to automatically drop missing samples from the data
+            predict_steps : int
+                number of steps to predict
         """
         nan_idx = []
         for i, (inputs, targets, meta) in enumerate(self):
             for key, data in inputs.items():  # key: lags/seasonality, data: torch tensor (oder OrderedDict)
-                if key in self.two_level_inputs or key == "events" or key == "regressors":
+                if key in self.two_level_inputs:
                     # Extract tensor out of OrderedDict to see if it contains NaNs
                     tuple_list = list(data.items())
                     tensor = tuple_list[0][1]
                     if np.isnan(np.array(tensor)).any() and (i not in nan_idx):
                         nan_idx.append(i)
                 else:
                     # save index of the NaN-containing sample
@@ -94,52 +94,50 @@
                 if (
                     i < len(self) - predict_steps
                 ):  # do not remove the targets that were inserted for prediction at the end
                     nan_idx.append(i)  # nan_idx contains all indices of inputs/targets containing 1 or more NaN values
         if drop_missing and len(nan_idx) > 0:
             log.warning(f"{len(nan_idx)} samples with missing values were dropped from the data. ")
             for key, data in self.inputs.items():
-                if key not in ["time", "lags"]:
+                if key not in ["time", "lags"]:  # "time_lagged"
                     for name, features in data.items():
                         self.inputs[key][name] = np.delete(self.inputs[key][name], nan_idx, 0)
                 else:
                     self.inputs[key] = np.delete(self.inputs[key], nan_idx, 0)
             self.targets = np.delete(self.targets, nan_idx, 0)
             self.length = self.inputs["time"].shape[0]
         if not drop_missing and len(nan_idx) > 0:
             raise ValueError(
                 "Inputs/targets with missing values detected. "
                 "Please either adjust imputation parameters, or set 'drop_missing' to True to drop those samples."
             )
 
     def init_after_tabularized(self, inputs, targets=None):
         """Create Timedataset with data.
-
         Parameters
         ----------
             inputs : ordered dict
                 Identical to returns from :meth:`tabularize_univariate_datetime`
             targets : np.array, float
                 Identical to returns from :meth:`tabularize_univariate_datetime`
         """
         inputs_dtype = {
             "time": torch.float,
             "timestamps": np.datetime64,
-            # "changepoints": torch.bool,
             "seasonalities": torch.float,
             "events": torch.float,
             "lags": torch.float,
             "covariates": torch.float,
             "regressors": torch.float,
         }
         targets_dtype = torch.float
         self.length = inputs["time"].shape[0]
 
         for key, data in inputs.items():
-            if key in self.two_level_inputs or key == "events" or key == "regressors":
+            if key in self.two_level_inputs:
                 self.inputs[key] = OrderedDict({})
                 for name, features in data.items():
                     self.inputs[key][name] = torch.from_numpy(features.astype(float)).type(inputs_dtype[key])
             else:
                 if key == "timestamps":
                     self.inputs[key] = data
                 else:
@@ -148,48 +146,49 @@
         self.meta["df_name"] = self.name
         # Pre-compute all samples for faster iteration in __getitem__
         self.samples = []
         for index in range(self.length):
             sample = OrderedDict({})
             for key, data in self.inputs.items():
                 if key in self.two_level_inputs:
-                    sample[key] = OrderedDict({})
-                    for name, period_features in self.inputs[key].items():
-                        sample[key][name] = period_features[index]
-                elif key == "events" or key == "regressors":
-                    sample[key] = OrderedDict({})
-                    for mode, features in self.inputs[key].items():
-                        sample[key][mode] = features[index, :, :]
+                    if (
+                        key == "events" or key == "regressors"
+                    ):  # or key == "events_lagged" or key == "regressors_lagged":
+                        sample[key] = OrderedDict({})
+                        for mode, features in self.inputs[key].items():
+                            sample[key][mode] = features[index, :, :]
+                    else:
+                        sample[key] = OrderedDict({})
+                        for name, period_features in self.inputs[key].items():
+                            sample[key][name] = period_features[index]
                 else:
                     sample[key] = data[index]
             self.samples.append(sample)
 
     def filter_samples_after_init(
         self,
         prediction_frequency=None,
     ):
         """Filters samples from the dataset based on the forecast frequency.
-
         Parameters
         ----------
             prediction_frequency : int
                 periodic interval in which forecasts should be made.
-
             Note
             ----
             E.g. if prediction_frequency=7, forecasts are only made on every 7th step (once in a week in case of daily resolution).
         """
         if prediction_frequency is None or prediction_frequency == 1:
             return
         # Only the first target timestamp is of interest for filtering
         timestamps = pd.to_datetime([sample["timestamps"][0] for sample in self.samples])
         masks = []
         for key, value in prediction_frequency.items():
             if key == "daily-hour":
-                mask = timestamps.hour == value + 1  # + 1 because prediction starts one step after origin
+                mask = timestamps.hour == value + 1  # because prediction starts one step after origin
             elif key == "weekly-day":
                 mask = timestamps.dayofweek == value + 1
             elif key == "monthly-day":
                 mask = timestamps.day == value + 1
             elif key == "yearly-month":
                 mask = timestamps.month == value + 1
             elif key == "hourly-minute":
@@ -206,29 +205,25 @@
         self.inputs.pop("timestamps")
         for sample in self.samples:
             sample.pop("timestamps")
         self.length = len(self.samples)
 
     def __getitem__(self, index):
         """Overrides parent class method to get an item at index.
-
         Parameters
         ----------
             index : int
                 Sample location in dataset
-
         Returns
         -------
         OrderedDict
             Model inputs, each of len(df) but with varying dimensions
-
             Note
             ----
             Contains the following data:
-
             Model Inputs
                 * ``time`` (np.array, float), dims: (num_samples, 1)
                 * ``seasonalities`` (OrderedDict), named seasonalities
                 each with features (np.array, float) - dims: (num_samples, n_features[name])
                 * ``lags`` (np.array, float), dims: (num_samples, n_lags)
                 * ``covariates`` (OrderedDict), named covariates,
                 each with features (np.array, float) of dims: (num_samples, n_lags)
@@ -260,20 +255,18 @@
     config_country_holidays=None,
     config_lagged_regressors: Optional[configure.ConfigLaggedRegressors] = None,
     config_regressors: Optional[configure.ConfigFutureRegressors] = None,
     config_missing=None,
     prediction_frequency=None,
 ):
     """Create a tabular dataset from univariate timeseries for supervised forecasting.
-
     Note
     ----
     Data must have no gaps.
     If data contains missing values, they are ignored for the creation of the dataset.
-
     Parameters
     ----------
         df : pd.DataFrame
             Sequence of observations with original ``ds``, ``y`` and normalized ``t``, ``y_scaled`` columns
         config_seasonality : configure.ConfigSeasonality
             Configuration for seasonalities
         n_lags : int
@@ -286,28 +279,24 @@
             Configurations (holiday_names, upper, lower windows, regularization) for country specific holidays
         config_lagged_regressors : configure.ConfigLaggedRegressors
             Configurations for lagged regressors
         config_regressors : configure.ConfigFutureRegressors
             Configuration for regressors
         predict_mode : bool
             Chooses the prediction mode
-
             Options
                 * (default) ``False``: Includes target values
                 * ``True``: Does not include targets but includes entire dataset as input
-
     Returns
     -------
         OrderedDict
             Model inputs, each of len(df) but with varying dimensions
-
             Note
             ----
             Contains the following data:
-
             Model Inputs
                 * ``time`` (np.array, float), dims: (num_samples, 1)
                 * ``seasonalities`` (OrderedDict), named seasonalities
                 each with features (np.array, float) - dims: (num_samples, n_features[name])
                 * ``lags`` (np.array, float), dims: (num_samples, n_lags)
                 * ``covariates`` (OrderedDict), named covariates,
                 each with features (np.array, float) of dims: (num_samples, n_lags)
@@ -325,52 +314,68 @@
 
     def _stride_time_features_for_forecasts(x):
         # only for case where n_lags > 0
         if x.dtype != np.float64:
             dtype = np.datetime64
         else:
             dtype = np.float64
+        return np.array([x[i + max_lags - n_lags : i + max_lags + n_forecasts] for i in range(n_samples)], dtype=dtype)
+
+    def _stride_future_time_features_for_forecasts(x):
+        # only for case where n_lags > 0
+        if x.dtype != np.float64:
+            dtype = np.datetime64
+        else:
+            dtype = np.float64
         return np.array([x[max_lags + i : max_lags + i + n_forecasts] for i in range(n_samples)], dtype=dtype)
 
+    def _stride_lagged_features(df_col_name, feature_dims):
+        # only for case where max_lags > 0
+        assert feature_dims >= 1
+        series = df.loc[:, df_col_name].values
+        # Added dtype=np.float64 to solve the problem with np.isnan for ubuntu test
+        return np.array(
+            [series[i + max_lags - feature_dims : i + max_lags] for i in range(n_samples)], dtype=np.float64
+        )
+
+    def _stride_timestamps_for_forecasts(x):
+        # only for case where n_lags > 0
+        if x.dtype != np.float64:
+            dtype = np.datetime64
+        else:
+            dtype = np.float64
+        return np.array([x[i + max_lags : i + max_lags + n_forecasts] for i in range(n_samples)], dtype=dtype)
+
     # time is the time at each forecast step
     t = df.loc[:, "t"].values
     if max_lags == 0:
         assert n_forecasts == 1
         time = np.expand_dims(t, 1)
     else:
         time = _stride_time_features_for_forecasts(t)
-    inputs["time"] = time
+    inputs["time"] = time  # contains n_lags + n_forecasts
 
     if prediction_frequency is not None:
         ds = df.loc[:, "ds"].values
-        if max_lags == 0:
+        if max_lags == 0:  # is it rather n_lags?
             timestamps = np.expand_dims(ds, 1)
         else:
-            timestamps = _stride_time_features_for_forecasts(ds)
+            timestamps = _stride_timestamps_for_forecasts(ds)
         inputs["timestamps"] = timestamps
 
     if config_seasonality is not None:
         seasonalities = seasonal_features_from_dates(df, config_seasonality)
         for name, features in seasonalities.items():
             if max_lags == 0:
                 seasonalities[name] = np.expand_dims(features, axis=1)
             else:
                 # stride into num_forecast at dim=1 for each sample, just like we did with time
                 seasonalities[name] = _stride_time_features_for_forecasts(features)
         inputs["seasonalities"] = seasonalities
 
-    def _stride_lagged_features(df_col_name, feature_dims):
-        # only for case where max_lags > 0
-        assert feature_dims >= 1
-        series = df.loc[:, df_col_name].values
-        # Added dtype=np.float64 to solve the problem with np.isnan for ubuntu test
-        return np.array(
-            [series[i + max_lags - feature_dims : i + max_lags] for i in range(n_samples)], dtype=np.float64
-        )
-
     if n_lags > 0 and "y" in df.columns:
         inputs["lags"] = _stride_lagged_features(df_col_name="y_scaled", feature_dims=n_lags)
 
     if config_lagged_regressors is not None and max_lags > 0:
         covariates = OrderedDict({})
         for covar in df.columns:
             if covar in config_lagged_regressors:
@@ -388,30 +393,29 @@
             if additive_regressors is not None:
                 regressors["additive"] = np.expand_dims(additive_regressors, axis=1)
             if multiplicative_regressors is not None:
                 regressors["multiplicative"] = np.expand_dims(multiplicative_regressors, axis=1)
         else:
             if additive_regressors is not None:
                 additive_regressor_feature_windows = []
+                # additive_regressor_feature_windows_lagged = []
                 for i in range(0, additive_regressors.shape[1]):
                     # stride into num_forecast at dim=1 for each sample, just like we did with time
                     stride = _stride_time_features_for_forecasts(additive_regressors[:, i])
                     additive_regressor_feature_windows.append(stride)
                 additive_regressors = np.dstack(additive_regressor_feature_windows)
                 regressors["additive"] = additive_regressors
 
             if multiplicative_regressors is not None:
                 multiplicative_regressor_feature_windows = []
                 for i in range(0, multiplicative_regressors.shape[1]):
-                    # stride into num_forecast at dim=1 for each sample, just like we did with time
                     stride = _stride_time_features_for_forecasts(multiplicative_regressors[:, i])
                     multiplicative_regressor_feature_windows.append(stride)
                 multiplicative_regressors = np.dstack(multiplicative_regressor_feature_windows)
                 regressors["multiplicative"] = multiplicative_regressors
-
         inputs["regressors"] = regressors
 
     # get the events features
     if config_events is not None or config_country_holidays is not None:
         additive_events, multiplicative_events = make_events_features(df, config_events, config_country_holidays)
 
         events = OrderedDict({})
@@ -427,105 +431,103 @@
                     # stride into num_forecast at dim=1 for each sample, just like we did with time
                     additive_event_feature_windows.append(_stride_time_features_for_forecasts(additive_events[:, i]))
                 additive_events = np.dstack(additive_event_feature_windows)
                 events["additive"] = additive_events
 
             if multiplicative_events is not None:
                 multiplicative_event_feature_windows = []
+                # multiplicative_event_feature_windows_lagged = []
                 for i in range(0, multiplicative_events.shape[1]):
                     # stride into num_forecast at dim=1 for each sample, just like we did with time
                     multiplicative_event_feature_windows.append(
                         _stride_time_features_for_forecasts(multiplicative_events[:, i])
                     )
                 multiplicative_events = np.dstack(multiplicative_event_feature_windows)
                 events["multiplicative"] = multiplicative_events
-
         inputs["events"] = events
+
     if predict_mode:
-        targets = np.empty_like(time)
+        targets = np.empty_like(time[:, n_lags:])
         targets = np.nan_to_num(targets)
     else:
-        targets = _stride_time_features_for_forecasts(df["y_scaled"].values)
+        targets = _stride_future_time_features_for_forecasts(df["y_scaled"].values)
 
     tabularized_input_shapes_str = ""
     for key, value in inputs.items():
-        if key in ["seasonalities", "covariates", "events", "regressors"]:
+        if key in [
+            "seasonalities",
+            "covariates",
+            "events",
+            "regressors",
+        ]:
             for name, period_features in value.items():
                 tabularized_input_shapes_str += f"    {name} {key} {period_features}\n"
         else:
             tabularized_input_shapes_str += f"    {key} {value.shape} \n"
     log.debug(f"Tabularized inputs shapes: \n{tabularized_input_shapes_str}")
 
     return inputs, targets, config_missing.drop_missing
 
 
 def fourier_series(dates, period, series_order):
     """Provides Fourier series components with the specified frequency and order.
-
     Note
     ----
     Identical to OG Prophet.
-
     Parameters
     ----------
         dates : pd.Series
             Containing timestamps
         period : float
             Number of days of the period
         series_order : int
             Number of fourier components
-
     Returns
     -------
         np.array
             Matrix with seasonality features
     """
     # convert to days since epoch
     t = np.array((dates - datetime(1970, 1, 1)).dt.total_seconds().astype(float)) / (3600 * 24.0)
     return fourier_series_t(t, period, series_order)
 
 
 def fourier_series_t(t, period, series_order):
     """Provides Fourier series components with the specified frequency and order.
-
     Note
     ----
     This function is identical to Meta AI's Prophet Library
-
     Parameters
     ----------
         t : pd.Series, float
             Containing time as floating point number of days
         period : float
             Number of days of the period
         series_order : int
             Number of fourier components
-
     Returns
     -------
         np.array
             Matrix with seasonality features
     """
     features = np.column_stack(
         [fun((2.0 * (i + 1) * np.pi * t / period)) for i in range(series_order) for fun in (np.sin, np.cos)]
     )
     return features
 
 
 def make_country_specific_holidays_df(year_list, country):
     """
     Make dataframe of country specific holidays for given years and countries
-
     Parameters
     ----------
         year_list : list
             List of years
         country : str, list
             List of country names
-
     Returns
     -------
         pd.DataFrame
             Containing country specific holidays df with columns 'ds' and 'holiday'
     """
     # iterate over countries and get holidays for each country
     # convert to list if not already
@@ -541,28 +543,26 @@
         country_specific_holidays_dict[holiday].append(pd.to_datetime(date))
     return country_specific_holidays_dict
 
 
 def _create_event_offset_features(event, config, feature, additive_events, multiplicative_events):
     """
     Create event offset features for the given event, config and feature
-
     Parameters
     ----------
         event : str
             Name of the event
         config : configure.ConfigEvents
             User specified events, holidays, and country specific holidays
         feature : pd.Series
             Feature for the event
         additive_events : pd.DataFrame
             Dataframe of additive events
         multiplicative_events : pd.DataFrame
             Dataframe of multiplicative events
-
     Returns
     -------
         tuple
             Tuple of additive_events and multiplicative_events
     """
     lw = config.lower_window
     uw = config.upper_window
@@ -575,24 +575,22 @@
         else:
             multiplicative_events[key] = offset_feature
 
 
 def make_events_features(df, config_events: Optional[configure.ConfigEvents] = None, config_country_holidays=None):
     """
     Construct arrays of all event features
-
     Parameters
     ----------
         df : pd.DataFrame
             Dataframe with all values including the user specified events (provided by user)
         config_events : configure.ConfigEvents
             User specified events, each with their upper, lower windows (int), regularization
         config_country_holidays : configure.ConfigCountryHolidays
             Configurations (holiday_names, upper, lower windows, regularization) for country specific holidays
-
     Returns
     -------
         np.array
             All additive event features (both user specified and country specific)
         np.array
             All multiplicative event features (both user specified and country specific)
     """
@@ -634,29 +632,26 @@
         multiplicative_events = None
 
     return additive_events, multiplicative_events
 
 
 def make_regressors_features(df, config_regressors):
     """Construct arrays of all scalar regressor features
-
     Parameters
     ----------
         df : pd.DataFrame
             Dataframe with all values including the user specified regressors
         config_regressors : configure.ConfigFutureRegressors
             User specified regressors config
-
     Returns
     -------
         np.array
             All additive regressor features
         np.array
             All multiplicative regressor features
-
     """
     additive_regressors = pd.DataFrame()
     multiplicative_regressors = pd.DataFrame()
 
     for reg in df.columns:
         if reg in config_regressors:
             mode = config_regressors[reg].mode
@@ -677,24 +672,21 @@
         multiplicative_regressors = None
 
     return additive_regressors, multiplicative_regressors
 
 
 def seasonal_features_from_dates(df, config_seasonality: configure.ConfigSeasonality):
     """Dataframe with seasonality features.
-
     Includes seasonality features, holiday features, and added regressors.
-
     Parameters
     ----------
         df : pd.DataFrame
             Dataframe with all values
         config_seasonality : configure.ConfigSeasonality
             Configuration for seasonalities
-
     Returns
     -------
         OrderedDict
             Dictionary with keys for each period name containing an np.array
             with the respective regression features. each with dims: (len(dates), 2*fourier_order)
     """
     dates = df["ds"]
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/time_net.py` & `neuralprophet-1.0.0rc1/neuralprophet/time_net.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import logging
 import math
 from collections import OrderedDict
+from functools import reduce
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 import torchmetrics
 
-from neuralprophet import configure, np_types, utils
+from neuralprophet import configure, np_types
 from neuralprophet.components.router import get_future_regressors, get_seasonality, get_trend
-from neuralprophet.utils_torch import init_parameter
+from neuralprophet.utils import (
+    check_for_regularization,
+    config_events_to_model_dims,
+    reg_func_events,
+    reg_func_regressors,
+    reg_func_season,
+    reg_func_trend,
+)
+from neuralprophet.utils_torch import init_parameter, interprete_model
 
 log = logging.getLogger("NP.time_net")
 
 
 class TimeNet(pl.LightningModule):
     """Linear time regression fun and some not so linear fun.
-
     A modular model that models classic time-series components
         * trend
         * seasonality
         * auto-regression (as AR-Net)
         * covariates (as AR-Net)
         * apriori regressors
         * events and holidays
@@ -40,124 +48,97 @@
         config_lagged_regressors: Optional[configure.ConfigLaggedRegressors] = None,
         config_regressors: Optional[configure.ConfigFutureRegressors] = None,
         config_events: Optional[configure.ConfigEvents] = None,
         config_holidays: Optional[configure.ConfigCountryHolidays] = None,
         n_forecasts: int = 1,
         n_lags: int = 0,
         max_lags: int = 0,
-        num_hidden_layers: int = 0,
-        d_hidden: Optional[int] = None,
+        ar_layers: Optional[List[int]] = [],
+        lagged_reg_layers: Optional[List[int]] = [],
         compute_components_flag: bool = False,
         metrics: Optional[np_types.CollectMetricsMode] = {},
         id_list: List[str] = ["__df__"],
         num_trends_modelled: int = 1,
         num_seasonalities_modelled: int = 1,
         meta_used_in_model: bool = False,
     ):
         """
         Parameters
         ----------
             quantiles : list
                 the set of quantiles estimated
-
             config_train : configure.Train
-
             config_trend : configure.Trend
-
             config_seasonality : configure.ConfigSeasonality
-
             config_ar : configure.AR
-
             config_lagged_regressors : configure.ConfigLaggedRegressors
                 Configurations for lagged regressors
             config_regressors : configure.ConfigFutureRegressors
                 Configs of regressors with mode and index.
             config_events : configure.ConfigEvents
-
             config_holidays : OrderedDict
-
             config_normalization: OrderedDict
-
             n_forecasts : int
                 number of steps to forecast. Aka number of model outputs
             n_lags : int
                 number of previous steps of time series used as input (aka AR-order)
-
                 Note
                 ----
                 The default value is ``0``, which initializes no auto-regression.
-            num_hidden_layers : int
-                Number of hidden layers (for AR-Net)
-
-                Note
-                ----
-                The default value is ``0``, which initializes no hidden layers (classic Auto-Regression).
 
             max_lags : int
                 Number of max. previous steps of time series used as input (aka AR-order).
 
-            num_hidden_layers : int
-                Number of hidden layers (for AR-Net).
-
-            d_hidden : int
-                Dimensionality of hidden layers  (for AR-Net).
+            ar_layers : list
+                List of hidden layers (for AR-Net).
 
                 Note
                 ----
-                This parameter is ignored if no hidden layers are specified.
+                The default value is ``[]``, which initializes no hidden layers.
+
+            lagged_reg_layers : list
+                List of hidden layers (for covariate-Net).
 
                 Note
                 ----
-                The default value is set to ``None``, which sets to ``n_lags + n_forecasts``.
+                The default value is ``[]``, which initializes no hidden layers.
+
 
             compute_components_flag : bool
                 Flag whether to compute the components of the model or not.
-
             metrics : dict
                 Dictionary of torchmetrics to be used during training and for evaluation.
-
             id_list : list
                 List of different time series IDs, used for global-local modelling (if enabled)
-
                 Note
                 ----
                 This parameter is set to  ``['__df__']`` if only one time series is input.
-
             num_trends_modelled : int
                 Number of different trends modelled.
-
                 Note
                 ----
                 If only 1 time series is modelled, it will be always 1.
-
                 Note
                 ----
                 For multiple time series. If trend is modelled globally the value is set
                 to 1, otherwise it is set to the number of time series modelled.
-
             num_seasonalities_modelled : int
                 Number of different seasonalities modelled.
-
                 Note
                 ----
                 If only 1 time series is modelled, it will be always 1.
-
                 Note
                 ----
                 For multiple time series. If seasonality is modelled globally the value is set
                 to 1, otherwise it is set to the number of time series modelled.
-
             meta_used_in_model : boolean
                 Whether we need to know the time series ID when we interact with the Model.
-
                 Note
                 ----
                 Will be set to ``True`` if more than one component is modelled locally.
-
-
         """
         super().__init__()
 
         # Store hyerparameters in model checkpoint
         # TODO: causes a RuntimeError under certain conditions, investigate and handle better
         try:
             self.save_hyperparameters()
@@ -197,15 +178,15 @@
         self.id_list = id_list
         self.id_dict = dict((key, i) for i, key in enumerate(id_list))
         self.num_trends_modelled = num_trends_modelled
         self.num_seasonalities_modelled = num_seasonalities_modelled
         self.meta_used_in_model = meta_used_in_model
 
         # Regularization
-        self.reg_enabled = utils.check_for_regularization(
+        self.reg_enabled = check_for_regularization(
             [
                 config_seasonality,
                 config_regressors,
                 config_lagged_regressors,
                 config_ar,
                 config_events,
                 config_trend,
@@ -244,15 +225,15 @@
                 n_forecasts=n_forecasts,
                 device=self.device,
             )
 
         # Events
         self.config_events = config_events
         self.config_holidays = config_holidays
-        self.events_dims = utils.config_events_to_model_dims(self.config_events, self.config_holidays)
+        self.events_dims = config_events_to_model_dims(self.config_events, self.config_holidays)
         if self.events_dims is not None:
             n_additive_event_params = 0
             n_multiplicative_event_params = 0
             for event, configs in self.events_dims.items():
                 if configs["mode"] not in ["additive", "multiplicative"]:
                     log.error("Event Mode {} not implemented. Defaulting to 'additive'.".format(configs["mode"]))
                     self.events_dims[event]["mode"] = "additive"
@@ -274,56 +255,39 @@
         else:
             self.config_events = None
             self.config_holidays = None
 
         # Autoregression
         self.config_ar = config_ar
         self.n_lags = n_lags
+        self.ar_layers = ar_layers
         self.max_lags = max_lags
-        self.num_hidden_layers = num_hidden_layers
-        self.d_hidden = (
-            max(4, round((n_lags + n_forecasts) / (2.0 * (num_hidden_layers + 1)))) if d_hidden is None else d_hidden
-        )
         if self.n_lags > 0:
             self.ar_net = nn.ModuleList()
             d_inputs = self.n_lags
-            for i in range(self.num_hidden_layers):
-                self.ar_net.append(nn.Linear(d_inputs, self.d_hidden, bias=True))
-                d_inputs = self.d_hidden
+            for d_hidden_i in self.ar_layers:
+                self.ar_net.append(nn.Linear(d_inputs, d_hidden_i, bias=True))
+                d_inputs = d_hidden_i
             # final layer has input size d_inputs and output size equal to no. of forecasts * no. of quantiles
             self.ar_net.append(nn.Linear(d_inputs, self.n_forecasts * len(self.quantiles), bias=False))
             for lay in self.ar_net:
                 nn.init.kaiming_normal_(lay.weight, mode="fan_in")
 
         # Lagged regressors
+        self.lagged_reg_layers = lagged_reg_layers
         self.config_lagged_regressors = config_lagged_regressors
         if self.config_lagged_regressors is not None:
-            self.covar_nets = nn.ModuleDict({})
-            for covar in self.config_lagged_regressors.keys():
-                covar_net = nn.ModuleList()
-                d_inputs = self.config_lagged_regressors[covar].n_lags
-                for i in range(self.config_lagged_regressors[covar].num_hidden_layers):
-                    d_hidden = (
-                        max(
-                            4,
-                            round(
-                                (self.config_lagged_regressors[covar].n_lags + n_forecasts)
-                                / (2.0 * (self.config_lagged_regressors[covar].num_hidden_layers + 1))
-                            ),
-                        )
-                        if self.config_lagged_regressors[covar].d_hidden is None
-                        else self.config_lagged_regressors[covar].d_hidden
-                    )
-                    covar_net.append(nn.Linear(d_inputs, d_hidden, bias=True))
-                    d_inputs = d_hidden
-                # final layer has input size d_inputs and output size equal to no. of forecasts * no. of quantiles
-                covar_net.append(nn.Linear(d_inputs, self.n_forecasts * len(self.quantiles), bias=False))
-                for lay in covar_net:
-                    nn.init.kaiming_normal_(lay.weight, mode="fan_in")
-                self.covar_nets[covar] = covar_net
+            self.covar_net = nn.ModuleList()
+            d_inputs = sum([covar.n_lags for _, covar in self.config_lagged_regressors.items()])
+            for d_hidden_i in self.lagged_reg_layers:
+                self.covar_net.append(nn.Linear(d_inputs, d_hidden_i, bias=True))
+                d_inputs = d_hidden_i
+            self.covar_net.append(nn.Linear(d_inputs, self.n_forecasts * len(self.quantiles), bias=False))
+            for lay in self.covar_net:
+                nn.init.kaiming_normal_(lay.weight, mode="fan_in")
 
         # Regressors
         self.config_regressors = config_regressors
         if self.config_regressors is not None:
             # Initialize future_regressors
             self.future_regressors = get_future_regressors(
                 config=config_regressors,
@@ -335,29 +299,64 @@
             )
         else:
             self.config_regressors = None
 
     @property
     def ar_weights(self) -> torch.Tensor:
         """sets property auto-regression weights for regularization. Update if AR is modelled differently"""
+        # TODO: this is wrong for deep networks, use utils_torch.interprete_model
         return self.ar_net[0].weight
 
-    def get_covar_weights(self, name: str) -> torch.Tensor:
-        """sets property auto-regression weights for regularization. Update if AR is modelled differently"""
-        return self.covar_nets[name][0].weight
+    def get_covar_weights(self, covar_input=None) -> torch.Tensor:
+        """
+        Get attributions of covariates network w.r.t. the model input.
+        """
+        if self.config_lagged_regressors is not None:
+            # Accumulate the lags of the covariates
+            covar_splits = np.add.accumulate(
+                [covar.n_lags for _, covar in self.config_lagged_regressors.items()][:-1]
+            ).tolist()
+            # If actual covariates are provided, use them to compute the attributions
+            if covar_input is not None:
+                covar_input = torch.cat([covar for _, covar in covar_input.items()], axis=1)
+            # Calculate the attributions w.r.t. the inputs
+            if self.lagged_reg_layers == []:
+                attributions = self.covar_net[0].weight
+            else:
+                attributions = interprete_model(self, "covar_net", "forward_covar_net", covar_input)
+            # Split the attributions into the different covariates
+            attributions_split = torch.tensor_split(
+                attributions,
+                covar_splits,
+                axis=1,
+            )
+            # Combine attributions and covariate name
+            covar_attributions = dict(zip(self.config_lagged_regressors.keys(), attributions_split))
+        else:
+            covar_attributions = None
+        return covar_attributions
+
+    def set_covar_weights(self, covar_weights: torch.Tensor):
+        """
+        Function to set the covariate weights for later interpretation in compute_components.
+        This function is needed since the gradient information is not available during the predict_step
+        method and attributions cannot be calculated in compute_components.
+
+        :param covar_weights: _description_
+        :type covar_weights: torch.Tensor
+        """
+        self.covar_weights = covar_weights
 
     def get_event_weights(self, name: str) -> Dict[str, torch.Tensor]:
         """
         Retrieve the weights of event features given the name
-
         Parameters
         ----------
             name : str
                 Event name
-
         Returns
         -------
             OrderedDict
                 Dict of the weights of all offsets corresponding to a particular event
         """
 
         event_dims = self.events_dims[name]
@@ -373,23 +372,21 @@
         for event_delim, indices in zip(event_dims["event_delim"], event_dims["event_indices"]):
             event_param_dict[event_delim] = event_params[:, indices : (indices + 1)]
         return event_param_dict
 
     def _compute_quantile_forecasts_from_diffs(self, diffs: torch.Tensor, predict_mode: bool = False) -> torch.Tensor:
         """
         Computes the actual quantile forecasts from quantile differences estimated from the model
-
         Args:
             diffs : torch.Tensor
                 tensor of dims (batch, n_forecasts, no_quantiles) which
                 contains the median quantile forecasts as well as the diffs of other quantiles
                 from the median quantile
             predict_mode : bool
                 boolean variable indicating whether the model is in prediction mode
-
         Returns:
             dim (batch, n_forecasts, no_quantiles)
                 final forecasts
         """
         if len(self.quantiles) > 1:
             # generate the actual quantile forecasts from predicted differences
             if any(quantile > 0.5 for quantile in self.quantiles):
@@ -434,15 +431,14 @@
         else:
             out = diffs
         return out
 
     def scalar_features_effects(self, features: torch.Tensor, params: nn.Parameter, indices=None) -> torch.Tensor:
         """
         Computes events component of the model
-
         Parameters
         ----------
             features : torch.Tensor, float
                 Features (either additive or multiplicative) related to event component dims (batch, n_forecasts, n_features)
             params : nn.Parameter
                 Params (either additive or multiplicative) related to events
             indices : list of int
@@ -456,285 +452,313 @@
             features = features[:, :, indices]
             params = params[:, indices]
 
         return torch.sum(features.unsqueeze(dim=2) * params.unsqueeze(dim=0).unsqueeze(dim=0), dim=-1)
 
     def auto_regression(self, lags: Union[torch.Tensor, float]) -> torch.Tensor:
         """Computes auto-regessive model component AR-Net.
-
         Parameters
         ----------
             lags  : torch.Tensor, float
                 Previous times series values, dims: (batch, n_lags)
-
         Returns
         -------
             torch.Tensor
                 Forecast component of dims: (batch, n_forecasts)
         """
         x = lags
-        for i in range(self.num_hidden_layers + 1):
+        for i in range(len(self.ar_layers) + 1):
             if i > 0:
                 x = nn.functional.relu(x)
             x = self.ar_net[i](x)
 
         # segment the last dimension to match the quantiles
         x = x.reshape(x.shape[0], self.n_forecasts, len(self.quantiles))
         return x
 
-    def covariate(self, lags: Union[torch.Tensor, float], name: str) -> torch.Tensor:
-        """Compute single covariate component.
-
-        Parameters
-        ----------
-            lags : torch.Tensor, float
-                Lagged values of covariate, dims: (batch, n_lags)
-            nam : str
-                Mame of covariate, for attribution to corresponding model weights
-
-        Returns
-        -------
-            torch.Tensor
-                Forecast component of dims (batch, n_forecasts)
-        """
-        x = lags
-        for i in range(self.config_lagged_regressors[name].num_hidden_layers + 1):
-            if i > 0:
-                x = nn.functional.relu(x)
-            x = self.covar_nets[name][i](x)
-
-        # segment the last dimension to match the quantiles
-        x = x.reshape(x.shape[0], self.n_forecasts, len(self.quantiles))
-        return x
-
-    def all_covariates(self, covariates: Dict[str, Union[torch.Tensor, float]]) -> torch.Tensor:
+    def forward_covar_net(self, covariates):
         """Compute all covariate components.
-
         Parameters
         ----------
             covariates : dict(torch.Tensor, float)
                 dict of named covariates (keys) with their features (values)
                 dims of each dict value: (batch, n_lags)
-
         Returns
         -------
             torch.Tensor
-                Forecast component of dims (batch, n_forecasts)
+                Forecast component of dims (batch, n_forecasts, quantiles)
         """
-        for i, name in enumerate(covariates.keys()):
-            if i == 0:
-                x = self.covariate(lags=covariates[name], name=name)
+        # Concat covariates into one tensor)
+        if isinstance(covariates, dict):
+            x = torch.cat([covar for _, covar in covariates.items()], axis=1)
+        else:
+            x = covariates
+        for i in range(len(self.lagged_reg_layers) + 1):
             if i > 0:
-                x = x + self.covariate(lags=covariates[name], name=name)
+                x = nn.functional.relu(x)
+            x = self.covar_net[i](x)
+
+        # segment the last dimension to match the quantiles
+        x = x.reshape(x.shape[0], self.n_forecasts, len(self.quantiles))
         return x
 
-    def forward(self, inputs: Dict, meta: Dict = None) -> torch.Tensor:
+    def forward(self, inputs: Dict, meta: Dict = None, compute_components_flag: bool = False) -> torch.Tensor:
         """This method defines the model forward pass.
-
         Note
         ----
-
         Time input is required. Minimum model setup is a linear trend.
-
         Parameters
         ----------
             inputs : dict
                 Model inputs, each of len(df) but with varying dimensions
-
                 Note
                 ----
-
                 Contains the following data:
-
                 Model Inputs
                     * ``time`` (torch.Tensor , loat), normalized time, dims: (batch, n_forecasts)
                     * ``lags`` (torch.Tensor, float), dims: (batch, n_lags)
                     * ``seasonalities`` (torch.Tensor, float), dict of named seasonalities (keys) with their features (values), dims of each dict value (batch, n_forecasts, n_features)
                     * ``covariates`` (torch.Tensor, float), dict of named covariates (keys) with their features (values), dims of each dict value: (batch, n_lags)
                     * ``events`` (torch.Tensor, float), all event features, dims (batch, n_forecasts, n_features)
                     * ``regressors``(torch.Tensor, float), all regressor features, dims (batch, n_forecasts, n_features)
                     * ``predict_mode`` (bool), optional and only passed during prediction
-
             meta : dict, default=None
                 Metadata about the all the samples of the model input batch.
-
                 Contains the following:
-
                 Model Meta:
                     * ``df_name`` (list, str), time series ID corresponding to each sample of the input batch.
-
                 Note
                 ----
                 The meta is sorted in the same way the inputs are sorted.
-
                 Note
                 ----
                 The default None value allows the forward method to be used without providing the meta argument.
                 This was designed to avoid issues with the library `lr_finder` https://github.com/davidtvs/pytorch-lr-finder
                 while having  ``config_trend.trend_global_local="local"``.
                 The turnaround consists on passing the same meta (dummy ID) to all the samples of the batch.
                 Internally, this is equivalent to use ``config_trend.trend_global_local="global"`` to find the optimal learning rate.
+            compute_components_flag : bool, default=False
+                If True, components will be computed.
 
         Returns
         -------
             torch.Tensor
                 Forecast of dims (batch, n_forecasts, no_quantiles)
         """
         # Turnaround to avoid issues when the meta argument is None and meta_used_in_model
         if meta is None and self.meta_used_in_model:
             name_id_dummy = self.id_list[0]
             meta = OrderedDict()
             meta["df_name"] = [name_id_dummy for _ in range(inputs["time"].shape[0])]
             meta = torch.tensor([self.id_dict[i] for i in meta["df_name"]], device=self.device)
 
-        additive_components = torch.zeros(
-            size=(inputs["time"].shape[0], self.n_forecasts, len(self.quantiles)), device=self.device
+        additive_components_nonstationary = torch.zeros(
+            size=(inputs["time"].shape[0], inputs["time"].shape[1], len(self.quantiles)), device=self.device
         )
-        multiplicative_components = torch.zeros(
-            size=(inputs["time"].shape[0], self.n_forecasts, len(self.quantiles)), device=self.device
+        multiplicative_components_nonstationary = torch.zeros(
+            size=(inputs["time"].shape[0], inputs["time"].shape[1], len(self.quantiles)), device=self.device
         )
+        additive_components = torch.zeros(
+            size=(inputs["time"].shape[0], self.n_forecasts, len(self.quantiles)),
+            device=self.device,
+        )
+        components = {}
 
-        if "lags" in inputs:
-            additive_components += self.auto_regression(lags=inputs["lags"])
-        # else: assert self.n_lags == 0
-
-        if "covariates" in inputs:
-            additive_components += self.all_covariates(covariates=inputs["covariates"])
+        # non-stationary components
+        trend = self.trend(t=inputs["time"], meta=meta)
+        components["trend"] = trend
 
         if "seasonalities" in inputs:
             s = self.seasonality(s=inputs["seasonalities"], meta=meta)
             if self.config_seasonality.mode == "additive":
-                additive_components += s
+                additive_components_nonstationary += s
             elif self.config_seasonality.mode == "multiplicative":
-                multiplicative_components += s
+                multiplicative_components_nonstationary += s
+            components["seasonalities"] = s
 
         if "events" in inputs:
             if "additive" in inputs["events"].keys():
-                additive_components += self.scalar_features_effects(
+                additive_events = self.scalar_features_effects(
                     inputs["events"]["additive"], self.event_params["additive"]
                 )
+                additive_components_nonstationary += additive_events
+                components["additive_events"] = additive_events
             if "multiplicative" in inputs["events"].keys():
-                multiplicative_components += self.scalar_features_effects(
+                multiplicative_events = self.scalar_features_effects(
                     inputs["events"]["multiplicative"], self.event_params["multiplicative"]
                 )
+                multiplicative_components_nonstationary += multiplicative_events
+                components["multiplicative_events"] = multiplicative_events
 
         if "regressors" in inputs:
             if "additive" in inputs["regressors"].keys():
-                additive_components += self.future_regressors(inputs["regressors"]["additive"], "additive")
+                additive_regressors = self.future_regressors(inputs["regressors"]["additive"], "additive")
+                additive_components_nonstationary += additive_regressors
+                components["additive_regressors"] = additive_regressors
             if "multiplicative" in inputs["regressors"].keys():
-                multiplicative_components += self.future_regressors(
+                multiplicative_regressors = self.future_regressors(
                     inputs["regressors"]["multiplicative"], "multiplicative"
                 )
+                multiplicative_components_nonstationary += multiplicative_regressors
+                components["multiplicative_regressors"] = multiplicative_regressors
 
-        trend = self.trend(t=inputs["time"], meta=meta)
-        out = (
-            trend
+        nonstationary_components = (  # dimensions - [batch, n_lags, median quantile]
+            trend[:, : self.n_lags, 0]
+            + additive_components_nonstationary[:, : self.n_lags, 0]
+            + trend[:, : self.n_lags, 0].detach() * multiplicative_components_nonstationary[:, : self.n_lags, 0]
+        )
+
+        # stationarized input
+        if "lags" in inputs:
+            stationarized_lags = inputs["lags"] - nonstationary_components
+            lags = self.auto_regression(lags=stationarized_lags)
+            additive_components = +lags
+            components["lags"] = lags
+
+        if "covariates" in inputs:
+            covariates = self.forward_covar_net(covariates=inputs["covariates"])
+            additive_components += covariates
+            components["covariates"] = covariates
+
+        predictions_nonstationary = (
+            trend[:, self.n_lags : inputs["time"].shape[1], :]
+            + additive_components_nonstationary[:, self.n_lags : inputs["time"].shape[1], :]
+            + trend[:, self.n_lags : inputs["time"].shape[1], :].detach()
+            * multiplicative_components_nonstationary[:, self.n_lags : inputs["time"].shape[1], :]
+        )
+        prediction = (
+            predictions_nonstationary
             + additive_components
-            + trend.detach() * multiplicative_components
             # 0 is the median quantile index
             # all multiplicative components are multiplied by the median quantile trend (uncomment line below to apply)
             # trend + additive_components + trend.detach()[:, :, 0].unsqueeze(dim=2) * multiplicative_components
         )  # dimensions - [batch, n_forecasts, no_quantiles]
 
         # check for crossing quantiles and correct them here
         if "predict_mode" in inputs.keys() and inputs["predict_mode"]:
             predict_mode = True
         else:
             predict_mode = False
-        out = self._compute_quantile_forecasts_from_diffs(out, predict_mode)
-        return out
+        prediction_with_quantiles = self._compute_quantile_forecasts_from_diffs(prediction, predict_mode)
 
-    def compute_components(self, inputs: Dict, meta: Dict) -> Dict:
-        """This method returns the values of each model component.
+        # component calculation
+        if compute_components_flag:
+            components = self.compute_components(inputs, components, meta)
+        else:
+            components = None
+
+        return prediction_with_quantiles, components
 
+    def compute_components(self, inputs: Dict, components_raw: Dict, meta: Dict) -> Dict:
+        """This method returns the values of each model component.
         Note
         ----
-
         Time input is required. Minimum model setup is a linear trend.
-
         Parameters
         ----------
             inputs : dict
                 Model inputs, each of len(df) but with varying dimensions
-
                 Note
                 ----
-
                 Contains the following data:
-
                 Model Inputs
                     * ``time`` (torch.Tensor , loat), normalized time, dims: (batch, n_forecasts)
                     * ``lags`` (torch.Tensor, float), dims: (batch, n_lags)
                     * ``seasonalities`` (torch.Tensor, float), dict of named seasonalities (keys) with their features (values), dims of each dict value (batch, n_forecasts, n_features)
                     * ``covariates`` (torch.Tensor, float), dict of named covariates (keys) with their features (values), dims of each dict value: (batch, n_lags)
                     * ``events`` (torch.Tensor, float), all event features, dims (batch, n_forecasts, n_features)
                     * ``regressors``(torch.Tensor, float), all regressor features, dims (batch, n_forecasts, n_features)
-
-        Returns
+            components_raw : dict
+                components to be computed
         -------
             dict
                 Containing forecast coomponents with elements of dims (batch, n_forecasts)
         """
         components = {}
-        components["trend"] = self.trend(t=inputs["time"], meta=meta)
+
+        components["trend"] = components_raw["trend"][:, self.n_lags : inputs["time"].shape[1], :]
         if self.config_trend is not None and "seasonalities" in inputs:
             for name, features in inputs["seasonalities"].items():
-                components[f"season_{name}"] = self.seasonality.compute_fourier(features=features, name=name, meta=meta)
+                components[f"season_{name}"] = self.seasonality.compute_fourier(
+                    features=features[:, self.n_lags : inputs["time"].shape[1], :], name=name, meta=meta
+                )
         if self.n_lags > 0 and "lags" in inputs:
-            components["ar"] = self.auto_regression(lags=inputs["lags"])
+            components["ar"] = components_raw["lags"]
         if self.config_lagged_regressors is not None and "covariates" in inputs:
-            for name, lags in inputs["covariates"].items():
-                components[f"lagged_regressor_{name}"] = self.covariate(lags=lags, name=name)
+            # Combined forward pass
+            all_covariates = components_raw["covariates"]
+            # Calculate the contribution of each covariate on each forecast
+            covar_attributions = self.covar_weights
+            # Sum the contributions of all covariates
+            covar_attribution_sum_per_forecast = reduce(
+                torch.add, [torch.sum(covar, axis=1) for _, covar in covar_attributions.items()]
+            ).to(all_covariates.device)
+            for name in inputs["covariates"].keys():
+                # Distribute the contribution of the current covariate to the combined forward pass
+                # 1. Calculate the relative share of each covariate on the total attributions
+                # 2. Multiply the relative share with the combined forward pass
+                components[f"lagged_regressor_{name}"] = torch.multiply(
+                    all_covariates,
+                    torch.divide(
+                        torch.sum(covar_attributions[name], axis=1).to(all_covariates.device),
+                        covar_attribution_sum_per_forecast,
+                    ).reshape(self.n_forecasts, len(self.quantiles)),
+                )
         if (self.config_events is not None or self.config_holidays is not None) and "events" in inputs:
             if "additive" in inputs["events"].keys():
-                components["events_additive"] = self.scalar_features_effects(
-                    features=inputs["events"]["additive"], params=self.event_params["additive"]
-                )
+                components["events_additive"] = components_raw["additive_events"][
+                    :, self.n_lags : inputs["time"].shape[1], :
+                ]
             if "multiplicative" in inputs["events"].keys():
-                components["events_multiplicative"] = self.scalar_features_effects(
-                    features=inputs["events"]["multiplicative"], params=self.event_params["multiplicative"]
-                )
+                components["events_multiplicative"] = components_raw["multiplicative_events"][
+                    :, self.n_lags : inputs["time"].shape[1], :
+                ]
             for event, configs in self.events_dims.items():
                 mode = configs["mode"]
                 indices = configs["event_indices"]
                 if mode == "additive":
-                    features = inputs["events"]["additive"]
+                    features = inputs["events"]["additive"][:, self.n_lags : inputs["time"].shape[1], :]
                     params = self.event_params["additive"]
                 else:
-                    features = inputs["events"]["multiplicative"]
+                    features = inputs["events"]["multiplicative"][:, self.n_lags : inputs["time"].shape[1], :]
                     params = self.event_params["multiplicative"]
                 components[f"event_{event}"] = self.scalar_features_effects(
                     features=features, params=params, indices=indices
                 )
         if self.config_regressors is not None and "regressors" in inputs:
             if "additive" in inputs["regressors"].keys():
-                components["future_regressors_additive"] = self.future_regressors(
-                    inputs["regressors"]["additive"], "additive"
-                )
+                components["future_regressors_additive"] = components_raw["additive_regressors"][
+                    :, self.n_lags : inputs["time"].shape[1], :
+                ]
+
             if "multiplicative" in inputs["regressors"].keys():
-                components["future_regressors_multiplicative"] = self.future_regressors(
-                    inputs["regressors"]["multiplicative"], "multiplicative"
-                )
+                components["future_regressors_multiplicative"] = components_raw["multiplicative_regressors"][
+                    :, self.n_lags : inputs["time"].shape[1], :
+                ]
+
             for regressor, configs in self.future_regressors.regressors_dims.items():
                 mode = configs["mode"]
                 index = []
                 index.append(configs["regressor_index"])
                 features = inputs["regressors"][mode]
-                components[f"future_regressor_{regressor}"] = self.future_regressors(features, mode, indeces=index)
+                components[f"future_regressor_{regressor}"] = self.future_regressors(
+                    features[:, self.n_lags : inputs["time"].shape[1], :], mode, indeces=index
+                )
+
         return components
 
     def set_compute_components(self, compute_components_flag):
         self.compute_components_flag = compute_components_flag
 
     def loss_func(self, inputs, predicted, targets):
         loss = None
         # Compute loss. no reduction.
         loss = self.config_train.loss_func(predicted, targets)
         # Weigh newer samples more.
-        loss = loss * self._get_time_based_sample_weight(t=inputs["time"])
+        loss = loss * self._get_time_based_sample_weight(t=inputs["time"][:, self.n_lags :])
         loss = loss.sum(dim=2).mean()
         # Regularize.
         if self.reg_enabled:
             steps_per_epoch = math.ceil(self.trainer.estimated_stepping_batches / self.trainer.max_epochs)
             progress_in_epoch = 1 - ((steps_per_epoch * (self.current_epoch + 1) - self.global_step) / steps_per_epoch)
             loss, reg_loss = self._add_batch_regularizations(loss, self.current_epoch, progress_in_epoch)
         else:
@@ -745,15 +769,15 @@
         inputs, targets, meta = batch
         # Global-local
         if self.meta_used_in_model:
             meta_name_tensor = torch.tensor([self.id_dict[i] for i in meta["df_name"]], device=self.device)
         else:
             meta_name_tensor = None
         # Run forward calculation
-        predicted = self.forward(inputs, meta_name_tensor)
+        predicted, _ = self.forward(inputs, meta_name_tensor)
         # Store predictions in self for later network visualization
         self.train_epoch_prediction = predicted
         # Calculate loss
         loss, reg_loss = self.loss_func(inputs, predicted, targets)
 
         # Optimization
         optimizer = self.optimizers()
@@ -780,15 +804,15 @@
         inputs, targets, meta = batch
         # Global-local
         if self.meta_used_in_model:
             meta_name_tensor = torch.tensor([self.id_dict[i] for i in meta["df_name"]], device=self.device)
         else:
             meta_name_tensor = None
         # Run forward calculation
-        predicted = self.forward(inputs, meta_name_tensor)
+        predicted, _ = self.forward(inputs, meta_name_tensor)
         # Calculate loss
         loss, reg_loss = self.loss_func(inputs, predicted, targets)
         # Metrics
         if self.metrics_enabled:
             predicted_denorm = self.denormalize(predicted[:, :, 0])
             target_denorm = self.denormalize(targets.squeeze(dim=2))
             self.log_dict(self.metrics_val(predicted_denorm, target_denorm), **self.log_args)
@@ -799,38 +823,36 @@
         inputs, targets, meta = batch
         # Global-local
         if self.meta_used_in_model:
             meta_name_tensor = torch.tensor([self.id_dict[i] for i in meta["df_name"]], device=self.device)
         else:
             meta_name_tensor = None
         # Run forward calculation
-        predicted = self.forward(inputs, meta_name_tensor)
+        predicted, _ = self.forward(inputs, meta_name_tensor)
         # Calculate loss
         loss, reg_loss = self.loss_func(inputs, predicted, targets)
         # Metrics
         if self.metrics_enabled:
+            predicted_denorm = self.denormalize(predicted[:, :, 0])
+            target_denorm = self.denormalize(targets.squeeze(dim=2))
+            self.log_dict(self.metrics_val(predicted_denorm, target_denorm), **self.log_args)
             self.log("Loss_test", loss, **self.log_args)
             self.log("RegLoss_test", reg_loss, **self.log_args)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
         inputs, _, meta = batch
         # Global-local
         if self.meta_used_in_model:
             meta_name_tensor = torch.tensor([self.id_dict[i] for i in meta["df_name"]], device=self.device)
         else:
             meta_name_tensor = None
         # Add predict_mode flag to dataset
         inputs["predict_mode"] = True
         # Run forward calculation
-        prediction = self.forward(inputs, meta_name_tensor)
-        # Calculate components (if requested)
-        if self.compute_components_flag:
-            components = self.compute_components(inputs, meta_name_tensor)
-        else:
-            components = None
+        prediction, components = self.forward(inputs, meta_name_tensor, self.compute_components_flag)
         return prediction, components
 
     def configure_optimizers(self):
         # Optimizer
         optimizer = self._optimizer(self.parameters(), lr=self.learning_rate, **self.config_train.optimizer_args)
 
         # Scheduler
@@ -856,24 +878,22 @@
             # scales end to be end weight times bigger than start weight
             # with end weight being 1.0
             weight = (1.0 + time * (end_w - 1.0)) / end_w
         return weight.unsqueeze(dim=2)  # add an extra dimension for the quantiles
 
     def _add_batch_regularizations(self, loss, epoch, progress):
         """Add regularization terms to loss, if applicable
-
         Parameters
         ----------
             loss : torch.Tensor, scalar
                 current batch loss
             epoch : int
                 current epoch number
             progress : float
                 progress within the epoch, between 0 and 1
-
         Returns
         -------
             loss, reg_loss
         """
         delay_weight = self.config_train.get_reg_delay_weight(epoch, progress)
 
         reg_loss = torch.zeros(1, dtype=torch.float, requires_grad=False, device=self.device)
@@ -883,51 +903,49 @@
                 reg_ar = self.config_ar.regularize(self.ar_weights)
                 reg_ar = torch.sum(reg_ar).squeeze() / self.n_forecasts
                 reg_loss += self.config_ar.reg_lambda * reg_ar
 
             # Regularize trend to be smoother/sparse
             l_trend = self.config_trend.trend_reg
             if self.config_trend.n_changepoints > 0 and l_trend is not None and l_trend > 0:
-                reg_trend = utils.reg_func_trend(
+                reg_trend = reg_func_trend(
                     weights=self.trend.get_trend_deltas,
                     threshold=self.config_train.trend_reg_threshold,
                 )
                 reg_loss += l_trend * reg_trend
 
             # Regularize seasonality: sparsify fourier term coefficients
             if self.config_seasonality:
                 l_season = self.config_seasonality.reg_lambda
                 if self.seasonality.season_dims is not None and l_season is not None and l_season > 0:
                     for name in self.seasonality.season_params.keys():
-                        reg_season = utils.reg_func_season(self.seasonality.season_params[name])
+                        reg_season = reg_func_season(self.seasonality.season_params[name])
                         reg_loss += l_season * reg_season
 
             # Regularize events: sparsify events features coefficients
             if self.config_events is not None or self.config_holidays is not None:
-                reg_events_loss = utils.reg_func_events(self.config_events, self.config_holidays, self)
+                reg_events_loss = reg_func_events(self.config_events, self.config_holidays, self)
                 reg_loss += reg_events_loss
 
             # Regularize regressors: sparsify regressor features coefficients
             if self.config_regressors is not None:
-                reg_regressor_loss = utils.reg_func_regressors(self.config_regressors, self)
+                reg_regressor_loss = reg_func_regressors(self.config_regressors, self)
                 reg_loss += reg_regressor_loss
 
         reg_loss = delay_weight * reg_loss
         loss = loss + reg_loss
         return loss, reg_loss
 
     def denormalize(self, ts):
         """
         Denormalize timeseries
-
         Parameters
         ----------
             target : torch.Tensor
                 ts tensor
-
         Returns
         -------
             denormalized timeseries
         """
         if self.config_normalization.global_normalization:
             shift_y = (
                 self.config_normalization.global_data_params["y"].shift
@@ -965,21 +983,21 @@
 
 
 class DeepNet(nn.Module):
     """
     A simple, general purpose, fully connected network
     """
 
-    def __init__(self, d_inputs, d_outputs, d_hidden=32, num_hidden_layers=0):
+    def __init__(self, d_inputs, d_outputs, lagged_reg_layers=[]):
         # Perform initialization of the pytorch superclass
         super(DeepNet, self).__init__()
         self.layers = nn.ModuleList()
-        for i in range(num_hidden_layers):
-            self.layers.append(nn.Linear(d_inputs, d_hidden, bias=True))
-            d_inputs = d_hidden
+        for d_hidden_i in lagged_reg_layers:
+            self.layers.append(nn.Linear(d_inputs, d_hidden_i, bias=True))
+            d_inputs = d_hidden_i
         self.layers.append(nn.Linear(d_inputs, d_outputs, bias=True))
         for lay in self.layers:
             nn.init.kaiming_normal_(lay.weight, mode="fan_in")
 
     def forward(self, x):
         """
         This method defines the network layering and activation functions
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/torch_prophet.py` & `neuralprophet-1.0.0rc1/neuralprophet/torch_prophet.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/uncertainty.py` & `neuralprophet-1.0.0rc1/neuralprophet/uncertainty.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from dataclasses import dataclass
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, List, Tuple, Union
 
 import matplotlib
+import numpy as np
 import pandas as pd
 
 from neuralprophet.plot_forecast_matplotlib import plot_interval_width_per_timestep, plot_nonconformity_scores
 from neuralprophet.plot_forecast_plotly import (
     plot_interval_width_per_timestep as plot_interval_width_per_timestep_plotly,
 )
 from neuralprophet.plot_forecast_plotly import plot_nonconformity_scores as plot_nonconformity_scores_plotly
@@ -51,79 +52,85 @@
             )
         else:
             self.symmetrical = False
             self.alpha_lo, self.alpha_hi = self.alpha
             self.q_hats = pd.DataFrame(columns=["q_hat_lo", "q_hat_hi"])
         self.noncon_scores = dict()
 
-    def predict(self, df: pd.DataFrame, df_cal: pd.DataFrame) -> pd.DataFrame:
+    def predict(self, df: pd.DataFrame, df_cal: pd.DataFrame, show_all_PI: bool = False) -> pd.DataFrame:
         """Apply a given conformal prediction technique to get the uncertainty prediction intervals (or q-hat) for test dataframe.
 
         Parameters
         ----------
             df : pd.DataFrame
                 test dataframe
             df_cal : pd.DataFrame
                 calibration dataframe
+            show_all_PI : bool
+                whether to return all prediction intervals (including quantile regression and conformal prediction)
 
             Returns
             -------
                 pd.DataFrame
                     test dataframe with uncertainty prediction intervals
 
         """
+        df_qr = df.copy()
 
         for step_number in range(1, self.n_forecasts + 1):
             # conformalize
             noncon_scores = self._get_nonconformity_scores(df_cal, step_number)
             q_hat = self._get_q_hat(df_cal, noncon_scores)
             y_hat_col = f"yhat{step_number}"
+            y_hat_lo_col = f"{y_hat_col} {min(self.quantiles) * 100}%"
+            y_hat_hi_col = f"{y_hat_col} {max(self.quantiles) * 100}%"
             if self.method == "naive" and self.symmetrical:
                 q_hat_sym = q_hat["q_hat_sym"]
-                q_hat_col = f"qhat{step_number}"
-                df[q_hat_col] = q_hat_sym
-                df[f"{y_hat_col} - {q_hat_col}"] = df[y_hat_col] - q_hat_sym
-                df[f"{y_hat_col} + {q_hat_col}"] = df[y_hat_col] + q_hat_sym
+                df[y_hat_lo_col] = df[y_hat_col] - q_hat_sym
+                df[y_hat_hi_col] = df[y_hat_col] + q_hat_sym
             elif self.method == "cqr" and self.symmetrical:
                 q_hat_sym = q_hat["q_hat_sym"]
-                q_hat_col = f"qhat{step_number}"
-                df[q_hat_col] = q_hat_sym
-                quantile_lo = str(min(self.quantiles) * 100)
-                quantile_hi = str(max(self.quantiles) * 100)
-                quantile_lo_col = f"{y_hat_col} {quantile_lo}%"
-                quantile_hi_col = f"{y_hat_col} {quantile_hi}%"
-                df[f"{quantile_lo_col} - {q_hat_col}"] = df[quantile_lo_col] - q_hat_sym
-                df[f"{quantile_lo_col} + {q_hat_col}"] = df[quantile_lo_col] + q_hat_sym
-                df[f"{quantile_hi_col} - {q_hat_col}"] = df[quantile_hi_col] - q_hat_sym
-                df[f"{quantile_hi_col} + {q_hat_col}"] = df[quantile_hi_col] + q_hat_sym
+                df[y_hat_lo_col] = df[y_hat_lo_col] - q_hat_sym
+                df[y_hat_hi_col] = df[y_hat_hi_col] + q_hat_sym
             elif self.method == "cqr" and not self.symmetrical:
                 q_hat_lo = q_hat["q_hat_lo"]
                 q_hat_hi = q_hat["q_hat_hi"]
-                q_hat_col_lo = f"qhat_lo{step_number}"
-                q_hat_col_hi = f"qhat_hi{step_number}"
-                df[q_hat_col_lo] = q_hat_lo
-                df[q_hat_col_hi] = q_hat_hi
-                quantile_lo = str(min(self.quantiles) * 100)
-                quantile_hi = str(max(self.quantiles) * 100)
-                quantile_lo_col = f"{y_hat_col} {quantile_lo}%"
-                quantile_hi_col = f"{y_hat_col} {quantile_hi}%"
-                df[f"{quantile_lo_col} - {q_hat_col_lo}"] = df[quantile_lo_col] - q_hat_lo
-                df[f"{quantile_lo_col} + {q_hat_col_lo}"] = df[quantile_lo_col] + q_hat_lo
-                df[f"{quantile_hi_col} - {q_hat_col_hi}"] = df[quantile_hi_col] - q_hat_hi
-                df[f"{quantile_hi_col} + {q_hat_col_hi}"] = df[quantile_hi_col] + q_hat_hi
+                df[y_hat_lo_col] = df[y_hat_lo_col] - q_hat_lo
+                df[y_hat_hi_col] = df[y_hat_hi_col] + q_hat_hi
             else:
                 raise ValueError(
                     f"Unknown conformal prediction method '{self.method}'. Please input either 'naive' or 'cqr'."
                 )
             if step_number == 1:
                 # save nonconformity scores of the first timestep
                 self.noncon_scores = noncon_scores
 
             # append the dictionary of q_hats to the dataframe based on the keys of the dictionary
-            self.q_hats = self.q_hats.append(q_hat, ignore_index=True)
+            q_hat_df = pd.DataFrame([q_hat])
+            self.q_hats = pd.concat([self.q_hats, q_hat_df], ignore_index=True)
+
+            # if show_all_PI is True, add the quantile regression prediction intervals
+            if show_all_PI:
+                df_quantiles = [col for col in df_qr.columns if "%" in col and f"yhat{step_number}" in col]
+                df_add = df_qr[df_quantiles]
+
+                if self.method == "naive":
+                    cp_lo_col = f"yhat{step_number} - qhat{step_number}"  # e.g. yhat1 - qhat1
+                    cp_hi_col = f"yhat{step_number} + qhat{step_number}"  # e.g. yhat1 + qhat1
+                    df.rename(columns={y_hat_lo_col: cp_lo_col, y_hat_hi_col: cp_hi_col}, inplace=True)
+                elif self.method == "cqr":
+                    qr_lo_col = (
+                        f"yhat{step_number} {max(self.quantiles) * 100}% - qhat{step_number}"  # e.g. yhat1 95% - qhat1
+                    )
+                    qr_hi_col = (
+                        f"yhat{step_number} {min(self.quantiles) * 100}% + qhat{step_number}"  # e.g. yhat1 5% + qhat1
+                    )
+                    df.rename(columns={y_hat_lo_col: qr_lo_col, y_hat_hi_col: qr_hi_col}, inplace=True)
+
+                df = pd.concat([df, df_add], axis=1, ignore_index=False)
 
         return df
 
     def _get_nonconformity_scores(self, df_cal: pd.DataFrame, step_number: int) -> dict:
         """Get the nonconformity scores using the given conformal prediction technique.
 
         Parameters
@@ -261,14 +268,15 @@
                     self.alpha,
                     initial_q_hat,
                     method,
                     resampler_active=plotting_backend == "plotly-resampler",
                 )
             else:
                 fig = plot_interval_width_per_timestep_plotly(self.q_hats, method, resampler_active=False)
+            fig.show()
         else:
             if self.n_forecasts == 1:
                 # includes nonconformity scores of the first timestep
                 fig = plot_nonconformity_scores(self.noncon_scores, self.alpha, initial_q_hat, method)
             else:
                 fig = plot_interval_width_per_timestep(self.q_hats, method)
         if plotting_backend in ["matplotlib", "plotly", "plotly-resampler"] and matplotlib.is_interactive():
@@ -287,149 +295,74 @@
     -------
         pd.DataFrame
             table containing evaluation metrics such as interval_width and miscoverage_rate
     """
     # Remove beginning rows used as lagged regressors (if any), or future dataframes without y-values
     # therefore, this ensures that all forecast rows for evaluation contains both y and y-hat
     df_forecast_eval = df_forecast.dropna(subset=["y", "yhat1"]).reset_index(drop=True)
+
     # Get evaluation params
-    method, n_forecasts, quantile_lo, quantile_hi, symmetrical = _infer_evaluate_params_from_dataset(df_forecast_eval)
     df_eval = pd.DataFrame()
+    cols = df_forecast_eval.columns
+    yhat_cols = [col for col in cols if "%" in col]
+    n_forecasts = int(re.search("yhat(\\d+)", yhat_cols[-1]).group(1))
+
+    # get the highest and lowest quantile percentages
+    quantiles = []
+    for col in yhat_cols:
+        match = re.search(r"\d+\.\d+", col)
+        if match:
+            quantiles.append(float(match.group()))
+    quantiles = sorted(set(quantiles))
 
     # Begin conformal evaluation steps
     for step_number in range(1, n_forecasts + 1):
-        y_hat_col = f"yhat{step_number}"
-        # QR Interval Evaluation (if quantiles lo & hi both exist)
-        if quantile_lo and quantile_hi:
-            quantile_lo_col = f"{y_hat_col} {quantile_lo}%"
-            quantile_hi_col = f"{y_hat_col} {quantile_hi}%"
-            # Get QR evaluation metrics
-            interval_width, miscoverage_rate = _get_evaluate_metrics_from_dataset(
-                df_forecast_eval, quantile_lo_col, quantile_hi_col
-            )
-            # Construct row dataframe with current timestep using its q-hat, interval width, and miscoverage rate
-            col_names = ["interval_width", "miscoverage_rate"]
-            row = [interval_width, miscoverage_rate]
-            df_row = pd.DataFrame([row], columns=pd.MultiIndex.from_product([[y_hat_col], ["qr"], col_names]))
-            # Add row dataframe to overall evaluation dataframe with all forecasted timesteps
-            df_eval = pd.concat([df_eval, df_row], axis=1)
-        # Naive CP Interval Evaluation
-        if method == "naive" and symmetrical:
-            q_hat_col_sym = f"qhat{step_number}"
-            q_hat_sym = df_forecast_eval.iloc[0][q_hat_col_sym]
-            quantile_lo_col = f"{y_hat_col} - {q_hat_col_sym}"
-            quantile_hi_col = f"{y_hat_col} + {q_hat_col_sym}"
-        # CQR Interval Evaluation
-        elif method == "cqr" and symmetrical:
-            q_hat_col_sym = f"qhat{step_number}"
-            q_hat_sym = df_forecast_eval.iloc[0][q_hat_col_sym]
-            quantile_lo_col = f"{y_hat_col} {quantile_lo}% - {q_hat_col_sym}"
-            quantile_hi_col = f"{y_hat_col} {quantile_hi}% + {q_hat_col_sym}"
-        elif method == "cqr" and not symmetrical:
-            q_hat_col_lo = f"qhat_lo{step_number}"
-            q_hat_col_hi = f"qhat_hi{step_number}"
-            q_hat_lo = df_forecast_eval.iloc[0][q_hat_col_lo]
-            q_hat_hi = df_forecast_eval.iloc[0][q_hat_col_hi]
-            quantile_lo_col = f"{y_hat_col} {quantile_lo}% - {q_hat_col_lo}"
-            quantile_hi_col = f"{y_hat_col} {quantile_hi}% + {q_hat_col_hi}"
+        y = df_forecast_eval["y"].values
+        # only relevant if show_all_PI is true
+        if len([col for col in cols if "qhat" in col]) > 0:
+            qhat_cols = [col for col in cols if f"qhat{step_number}" in col]
+            yhat_lo = df_forecast_eval[qhat_cols[0]].values
+            yhat_hi = df_forecast_eval[qhat_cols[-1]].values
         else:
-            raise ValueError(f"Unknown conformal prediction method '{method}'. Please input either 'naive' or 'cqr'.")
-        # Get CP evaluation metrics
-        interval_width, miscoverage_rate = _get_evaluate_metrics_from_dataset(
-            df_forecast_eval, quantile_lo_col, quantile_hi_col
-        )
+            yhat_lo = df_forecast_eval[f"yhat{step_number} {quantiles[0]}%"].values
+            yhat_hi = df_forecast_eval[f"yhat{step_number} {quantiles[-1]}%"].values
+        interval_width, miscoverage_rate = _get_evaluate_metrics_from_dataset(y, yhat_lo, yhat_hi)
+
         # Construct row dataframe with current timestep using its q-hat, interval width, and miscoverage rate
-        col_names = (
-            [f"qhat{step_number}", "interval_width", "miscoverage_rate"]
-            if symmetrical
-            else [f"qhat_lo{step_number}", f"qhat_hi{step_number}", "interval_width", "miscoverage_rate"]
-        )
-        row = (
-            [q_hat_sym, interval_width, miscoverage_rate]
-            if symmetrical
-            else [q_hat_lo, q_hat_hi, interval_width, miscoverage_rate]
-        )
-        df_row = pd.DataFrame([row], columns=pd.MultiIndex.from_product([[y_hat_col], [method], col_names]))
+        col_names = ["interval_width", "miscoverage_rate"]
+        row = [interval_width, miscoverage_rate]
+        df_row = pd.DataFrame([row], columns=pd.MultiIndex.from_product([[f"yhat{step_number}"], col_names]))
+
         # Add row dataframe to overall evaluation dataframe with all forecasted timesteps
         df_eval = pd.concat([df_eval, df_row], axis=1)
 
     return df_eval
 
 
-def _infer_evaluate_params_from_dataset(
-    df_forecast_eval: pd.DataFrame,
-) -> Tuple[str, int, Optional[str], Optional[str], bool]:
-    """Infers evaluation parameters based on the evaluation dataframe columns.
-
-    Parameters
-    ----------
-        df_forecast_eval : pd.DataFrame
-            forecast dataframe with the conformal prediction intervals
-
-    Returns
-    -------
-        str, int, Optional[str], Optional[str], bool
-            parameters to evaluate conformal prediction, only cqr outputs quantile_lo and quantile_hi
-    """
-    # check if symmetrical or asymmetrical quantiles were used by checking if qhat_lo or qhat_hi exists in df
-    if "qhat_lo1" in df_forecast_eval.columns:
-        symmetrical = False
-    else:
-        symmetrical = True
-
-    # Get n_forecasts
-    qhat_col = [col for col in df_forecast_eval.columns if col[:4] == "qhat"]
-    if symmetrical:
-        n_forecasts = int(qhat_col[-1].replace("qhat", ""))
-        # Extract conformal prediction forecast column(s)
-        cp_pattern = "yhat1\\ (.*)?\\%\\ \\+\\ qhat1"
-    else:
-        n_forecasts = int(qhat_col[-1].replace("qhat_hi", ""))
-        # Extract conformal prediction forecast column(s)
-        cp_pattern = "yhat1\\ (.*)?\\%\\ \\+\\ qhat_[A-Za-z][A-Za-z]1"
-    cp_col = [col for col in df_forecast_eval if re.compile(cp_pattern).match(col)]
-    # Get Naive method if only "yhat1 + qhat1" exist and CQR if "yhat1 {quantile} + qhat1" for both lo & hi exist
-    method = "cqr" if len(cp_col) == 2 else "naive"
-    # Extract quantile regression forecast column(s)
-    qr_pattern = "yhat1\\ (.*)?\\%$"
-    qr_col = [col for col in df_forecast_eval if re.compile(qr_pattern).match(col)]
-    # Get quantile lo & hi if QR exists else set both to None
-    if len(qr_col) == 2:
-        quantile_lo = re.findall(qr_pattern, qr_col[0])[0]
-        quantile_hi = re.findall(qr_pattern, qr_col[1])[0]
-    else:
-        quantile_lo = None
-        quantile_hi = None
-
-    return method, n_forecasts, quantile_lo, quantile_hi, symmetrical
-
-
-def _get_evaluate_metrics_from_dataset(
-    df_forecast_eval: pd.DataFrame,
-    quantile_lo_col: str,
-    quantile_hi_col: str,
-) -> Tuple[float, float]:
+def _get_evaluate_metrics_from_dataset(y: np.ndarray, yhat_lo: np.ndarray, yhat_hi: np.ndarray) -> Tuple[float, float]:
+    #     df_forecast_eval: pd.DataFrame,
+    #     quantile_lo_col: str,
+    #     quantile_hi_col: str,
+    # ) -> Tuple[float, float]:
     """Infers evaluation parameters based on the evaluation dataframe columns.
 
     Parameters
     ----------
         df_forecast_eval : pd.DataFrame
             forecast dataframe with the conformal prediction intervals
 
     Returns
     -------
         float, float
             conformal prediction evaluation metrics
     """
     # Interval width (efficiency metric)
-    quantile_lo_mean = df_forecast_eval[quantile_lo_col].mean()
-    quantile_hi_mean = df_forecast_eval[quantile_hi_col].mean()
+    quantile_lo_mean = np.mean(yhat_lo)
+    quantile_hi_mean = np.mean(yhat_hi)
     interval_width = quantile_hi_mean - quantile_lo_mean
+
     # Miscoverage rate (validity metric)
-    n_covered = df_forecast_eval.apply(
-        lambda row: bool(row[quantile_lo_col] <= row["y"] <= row[quantile_hi_col]),
-        axis=1,
-    )
-    coverage_rate = n_covered.sum() / len(df_forecast_eval)
+    n_covered = np.sum((y >= yhat_lo) & (y <= yhat_hi))
+    coverage_rate = n_covered / len(y)
     miscoverage_rate = 1 - coverage_rate
 
     return interval_width, miscoverage_rate
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/utils.py` & `neuralprophet-1.0.0rc1/neuralprophet/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,19 +181,19 @@
 
     Returns
     -------
         scalar
             Regularization loss
     """
     reg_covariate_loss = 0.0
+    weights = model.get_covar_weights()
     for covariate, configs in config_lagged_regressors.items():
         reg_lambda = configs.reg_lambda
         if reg_lambda is not None:
-            weights = model.get_covar_weights(covariate)
-            loss = torch.mean(utils_torch.penalize_nonzero(weights)).squeeze()
+            loss = torch.mean(utils_torch.penalize_nonzero(weights[covariate])).squeeze()
             reg_covariate_loss += reg_lambda * loss
 
     return reg_covariate_loss
 
 
 def reg_func_regressors(config_regressors, model):
     """
@@ -645,14 +645,18 @@
     seed : numeric
         Seed value for random number generator
 
     Note
     ----
     This needs to be set each time before fitting the model.
 
+    Example
+    -------
+    >>> from neuralprophet import set_random_seed
+    >>> set_random_seed(seed=42)
     """
     np.random.seed(seed)
     torch.manual_seed(seed)
 
 
 def set_logger_level(logger, log_level, include_handlers=False):
     if log_level is None:
@@ -678,14 +682,19 @@
     ----------
         log_level : str
             The log level of the logger objects used for printing procedure status
             updates for debugging/monitoring. Should be one of ``NOTSET``, ``DEBUG``, ``INFO``, ``WARNING``,
             ``ERROR`` or ``CRITICAL``
         include_handlers : bool
             Include any specified file/stream handlers
+
+    Example
+    -------
+    >>> from neuralprophet import set_log_level
+    >>> set_log_level("ERROR")
     """
     set_logger_level(logging.getLogger("NP"), log_level, include_handlers)
 
 
 def smooth_loss_and_suggest(lr_finder_results, window=10):
     """
     Smooth loss using a Hamming filter.
@@ -726,14 +735,15 @@
     try:
         # Find the steepest gradient and the minimum loss after that
         suggestion = lr[np.argmin(np.gradient(loss))]
     except ValueError:
         log.error(
             f"The number of loss values ({len(loss)}) is too small to estimate a learning rate. Increase the number of samples or manually set the learning rate."
         )
+        raise
     return (loss, lr, suggestion)
 
 
 def _smooth_loss(loss, beta=0.9):
     smoothed_loss = np.zeros_like(loss)
     smoothed_loss[0] = loss[0]
     for i in range(1, len(loss)):
```

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/utils_metrics.py` & `neuralprophet-1.0.0rc1/neuralprophet/utils_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0rc1/neuralprophet/utils_torch.py` & `neuralprophet-1.0.0rc1/neuralprophet/utils_torch.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,29 +70,32 @@
     elif inspect.isclass(optimizer_name) and issubclass(optimizer_name, torch.optim.Optimizer):
         optimizer = optimizer_name
     else:
         raise ValueError("The provided optimizer is not supported.")
     return optimizer, optimizer_args
 
 
-def interprete_model(target_model: pl.LightningModule, net: str, forward_func: str):
+def interprete_model(target_model: pl.LightningModule, net: str, forward_func: str, _input: torch.Tensor = None):
     """
     Returns model input attributions for a given network and forward function.
 
     Parameters
     ----------
         target_model : pl.LightningModule
             The model for which input attributions are to be computed.
 
         net : str
             Name of the network for which input attributions are to be computed.
 
         forward_func : str
             Name of the forward function for which input attributions are to be computed.
 
+        _input : torch.Tensor
+            Input for which the attributions are to be computed.
+
     Returns
     -------
         torch.Tensor
             Input attributions for the given network and forward function.
     """
     # Load the respective forward function from the model and init model interpreter
     forward = getattr(target_model, forward_func)
@@ -103,15 +106,15 @@
     # Number of input features to the net (aka n_lags)
     num_in_features = getattr(target_model, net)[0].in_features
     # Number of output features from the net (aka n_forecasts)
     num_out_features = getattr(target_model, net)[-1].out_features
     num_out_features_without_quantiles = int(num_out_features / num_quantiles)
 
     # Create a tensor of ones as model input
-    model_input = torch.ones(1, num_in_features, requires_grad=True)
+    model_input = torch.ones(1, num_in_features, requires_grad=True) if _input is None else _input
 
     # Iterate through each output feature and compute the model attribution wrt. the input
     attributions = torch.empty((0, num_in_features))
     for output_feature in range(num_out_features_without_quantiles):
         for quantile in range(num_quantiles):
             target_attribution = saliency.attribute(model_input, target=[(output_feature, quantile)], abs=False)
             attributions = torch.cat((attributions, target_attribution), 0)
```

### Comparing `neuralprophet-0.6.0rc1/pyproject.toml` & `neuralprophet-1.0.0rc1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,47 @@
 [tool.poetry]
 name = "neuralprophet"
-version = "0.6.0rc1"
+version = "1.0.0rc1"
 description = "NeuralProphet is an easy to learn framework for interpretable time series forecasting."
 authors = ["Oskar Triebe <triebe@stanford.edu>"]
 license = "MIT"
 readme = "README.md"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+]
+
+[tool.poetry.urls]
+Homepage = "https://github.com/ourownstory/neural_prophet"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
+python = ">=3.8,<3.11"
 captum = "^0.6.0"
 holidays = "^0.21"
 matplotlib = "^3.5.3"
-numpy = ">=1.21.6,<1.24.0"
+numpy = ">=1.22.0,<1.24.0"
 pandas = "^1.3.5"
 plotly = "^5.13.1"
+kaleido = "^0.2.1"
 plotly-resampler = "^0.8.3.1"
 pytorch-lightning = "^1.9.4"
 tensorboard = "^2.11.2"
 torch = "^1.13.1"
 torchmetrics = "^0.11.3"
 typing-extensions = "^4.5.0"
+nbformat = ">=4.2.0"
+livelossplot = { version = "^0.5.5", optional = true }
+
+[tool.poetry.extras]
+live = ["livelossplot"]
+
 
 [tool.poetry.group.dev.dependencies]
 black = { extras = ["jupyter"], version = "^23.1.0" }
 flake8 = "^5.0.4"
 isort = "^5.11.5"
 
 [tool.poetry.group.tests]
@@ -41,14 +59,19 @@
 myst-parser = "^0.18.1"
 nbsphinx = "^0.8.12"
 nbsphinx-link = "^1.3.0"
 sphinx = "^4.2.0"
 sphinx-fontawesome = "^0.0.6"
 furo = "^2022.9.29"
 
+
+[tool.poetry.group.pyright.dependencies]
+pandas-stubs = "<2"
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
```

### Comparing `neuralprophet-0.6.0rc1/PKG-INFO` & `neuralprophet-1.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 Metadata-Version: 2.1
 Name: neuralprophet
-Version: 0.6.0rc1
+Version: 1.0.0rc1
 Summary: NeuralProphet is an easy to learn framework for interpretable time series forecasting.
 License: MIT
 Author: Oskar Triebe
 Author-email: triebe@stanford.edu
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: live
 Requires-Dist: captum (>=0.6.0,<0.7.0)
 Requires-Dist: holidays (>=0.21,<0.22)
+Requires-Dist: kaleido (>=0.2.1,<0.3.0)
+Requires-Dist: livelossplot (>=0.5.5,<0.6.0) ; extra == "live"
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
-Requires-Dist: numpy (>=1.21.6,<1.24.0)
+Requires-Dist: nbformat (>=4.2.0)
+Requires-Dist: numpy (>=1.22.0,<1.24.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: plotly (>=5.13.1,<6.0.0)
 Requires-Dist: plotly-resampler (>=0.8.3.1,<0.9.0.0)
 Requires-Dist: pytorch-lightning (>=1.9.4,<2.0.0)
 Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
 Requires-Dist: torch (>=1.13.1,<2.0.0)
 Requires-Dist: torchmetrics (>=0.11.3,<0.12.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Homepage, https://github.com/ourownstory/neural_prophet
 Description-Content-Type: text/markdown
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ourownstory/neural_prophet?logo=github)](https://github.com/ourownstory/neural_prophet/releases)
 [![Pypi_Version](https://img.shields.io/pypi/v/neuralprophet.svg)](https://pypi.python.org/pypi/neuralprophet)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue?logo=python)](https://www.python.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](https://opensource.org/licenses/MIT)
```

