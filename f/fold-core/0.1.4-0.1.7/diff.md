# Comparing `tmp/fold_core-0.1.4.tar.gz` & `tmp/fold_core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.1.4.tar", max compression
+gzip compressed data, was "fold_core-0.1.7.tar", max compression
```

## Comparing `fold_core-0.1.4.tar` & `fold_core-0.1.7.tar`

### file list

```diff
@@ -1,56 +1,59 @@
--rw-r--r--   0        0        0     3870 2023-04-25 14:21:08.507826 fold_core-0.1.4/LICENSE
--rw-r--r--   0        0        0    10376 2023-04-25 14:21:08.507826 fold_core-0.1.4/README.md
--rw-r--r--   0        0        0     3820 2023-04-25 14:21:08.543828 fold_core-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/__init__.py
--rw-r--r--   0        0        0     5400 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/base.py
--rw-r--r--   0        0        0      529 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10261 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1577 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/common.py
--rw-r--r--   0        0        0     6272 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2226 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6384 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4785 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3261 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/sample.py
--rw-r--r--   0        0        0     2064 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/select.py
--rw-r--r--   0        0        0     4632 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/target.py
--rw-r--r--   0        0        0      345 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2408 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1931 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3198 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0      590 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/checks.py
--rw-r--r--   0        0        0     9973 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/common.py
--rw-r--r--   0        0        0     2109 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/convenience.py
--rw-r--r--   0        0        0     7138 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/encase.py
--rw-r--r--   0        0        0      852 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/inference.py
--rw-r--r--   0        0        0     2993 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/memory.py
--rw-r--r--   0        0        0     6545 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/training.py
--rw-r--r--   0        0        0     1845 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/types.py
--rw-r--r--   0        0        0      756 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/update.py
--rw-r--r--   0        0        0      381 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/base.py
--rw-r--r--   0        0        0     1926 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4349 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2187 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/random.py
--rw-r--r--   0        0        0     4310 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/py.typed
--rw-r--r--   0        0        0     6724 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/splitters.py
--rw-r--r--   0        0        0      928 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     6034 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8593 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4281 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     3312 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      798 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6569 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5675 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     7624 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3701 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      887 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4414 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/window.py
--rw-r--r--   0        0        0     2171 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/checks.py
--rw-r--r--   0        0        0      638 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/dataframe.py
--rw-r--r--   0        0        0     2240 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1591 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/list.py
--rw-r--r--   0        0        0     2955 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1716 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/trim.py
--rw-r--r--   0        0        0    13173 1970-01-01 00:00:00.000000 fold_core-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-05-02 13:09:22.050625 fold_core-0.1.7/LICENSE
+-rw-r--r--   0        0        0    10102 2023-05-02 13:09:22.050625 fold_core-0.1.7/README.md
+-rw-r--r--   0        0        0     3820 2023-05-02 13:09:22.086625 fold_core-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/__init__.py
+-rw-r--r--   0        0        0     6200 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/base.py
+-rw-r--r--   0        0        0      570 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10261 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1577 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6272 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2226 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6384 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     2857 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/optimize.py
+-rw-r--r--   0        0        0     4785 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3261 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     2231 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4632 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/target.py
+-rw-r--r--   0        0        0      345 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1439 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3198 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0     1264 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/checks.py
+-rw-r--r--   0        0        0    11552 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/common.py
+-rw-r--r--   0        0        0     7138 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2886 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/global.py
+-rw-r--r--   0        0        0      852 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/inference.py
+-rw-r--r--   0        0        0     2993 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     6387 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1845 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/types.py
+-rw-r--r--   0        0        0      756 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/update.py
+-rw-r--r--   0        0        0     2243 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/wrap.py
+-rw-r--r--   0        0        0      381 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3219 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/base.py
+-rw-r--r--   0        0        0     1926 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4349 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2187 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/random.py
+-rw-r--r--   0        0        0     5169 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/py.typed
+-rw-r--r--   0        0        0     6724 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/splitters.py
+-rw-r--r--   0        0        0     1003 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6034 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8593 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4775 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     5393 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      798 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6569 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     6557 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     8858 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3836 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/scaling.py
+-rw-r--r--   0        0        0     4808 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      887 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4414 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     2216 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/checks.py
+-rw-r--r--   0        0        0      638 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/dataframe.py
+-rw-r--r--   0        0        0     2240 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1591 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/list.py
+-rw-r--r--   0        0        0     4496 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1716 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    12899 1970-01-01 00:00:00.000000 fold_core-0.1.7/PKG-INFO
```

### Comparing `fold_core-0.1.4/LICENSE` & `fold_core-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/README.md` & `fold_core-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         Collection Link
         </a>
     </td>
     <td> - </td>
   </tr>
   <tr>
     <td> 
-    🖋️ Back to the Future with Time Series Forecasting
+    🖋️ Why we ended up building an Adaptive ML engine for Time Series
     </td>
     <td>Blog</td>
     <td>Public Release Blog Post </td>
     <td> 
         <a href='https://www.appliedexploration.com/p/back-to-the-future-with-time-series' target="_blank">
         Blog post on Applied Exploration 
         </a>
@@ -214,17 +214,17 @@
 Join our   <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a> for live discussion! 
 
 Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
 
 ## Licence & Usage
 
 We want to **bring much-needed transparency, speed and rigour** to the process of creating Time Series ML pipelines, while also building a sustainable business, that can support the ecosystem in the long-term.
-Fold's licence is inbetween [source-available](https://en.wikipedia.org/wiki/Source-available_software) and a traditional commercial software licence. It requires a paid licence for any commercial use, after the initial, 30 day trial period. Deployment is only possible with the additional purchase of `fold-extended`, a product currently in development. 
+Fold's licence is inbetween [source-available](https://en.wikipedia.org/wiki/Source-available_software) and a traditional commercial software licence. It requires a paid licence for any commercial use, after the initial, 30 day trial period.
 
-We also want to contribute to open research by giving free access to non-commercial use of `fold`. If you are a researcher and would like to get access to Dream Faster's all of available tools, please <a href='mailto:info@dreamfaster.ai?subject=Research Licence'>contact us here</a>. 
+We also want to contribute to open research by giving free access to non-commercial, research use of `fold`. 
 
 [Read more](https://dream-faster.github.io/fold/product/license/)
 
 ## Limitations
 
 - No intermittent time series support, very limited support for missing values.
 - No hierarchical time series support.
```

#### html2text {}

```diff
@@ -49,23 +49,23 @@
 and use `modin` to handle out-of-memory datasets (full support for modin is
 coming in April).** - Bridging the gap between Online and Mini-Batch learning.
 **â Mix and match `xgboost` with ARIMA, in a single pipeline. Boost your
 model's accuracy by updating them on every timestamp, if desired.** - Update
 your deployed models, easily, as new data flows in.
 **â Real world is not static. Let your models adapt, without the need to re-
 train from scratch.**  ## Examples, Walkthroughs and Blog Posts
-Name                                               Type        Dataset   Docs Link   Colab
-                                                               Type
-â¡ï¸ Core Walkthrough                      Walkthrough Energy    Notebook    Colab
-ð Speed Comparison of Fold to other librarieWalkthrough Weather   Notebook    Colab
-ð Example Collection                        Example     Weather & Collection  -
-                                                               Synthetic Link
-ðï¸ Back to the Future with Time Series             Public    Blog_post
-Forecasting                                        Blog        Release   on_Applied  -
-                                                               Blog Post Exploration
+Name                                                                   Type        Dataset   Docs Link   Colab
+                                                                                   Type
+â¡ï¸ Core Walkthrough                                          Walkthrough Energy    Notebook    Colab
+ð Speed Comparison of Fold to other libraries                   Walkthrough Weather   Notebook    Colab
+ð Example Collection                                            Example     Weather & Collection  -
+                                                                                   Synthetic Link
+                                                                                   Public    Blog_post
+ðï¸ Why we ended up building an Adaptive ML engine for Time Bloges      Release   on_Applied  -
+                                                                                   Blog Post Exploration
 
 ## Core Features - Supports both Regression and Classification tasks. - Online
 and Mini-batch learning. - Feature selection and other transformations on an
 expanding/rolling window basis - Use any scikit-learn/tabular model natively! -
 Use any univariate or sequence models (wrappers provided in [fold-wrappers]
 (https://github.com/dream-faster/fold-wrappers)). - Use any Deep Learning Time
 Series models (wrappers provided in [fold-wrappers](https://github.com/dream-
@@ -95,15 +95,12 @@
 Community] for live discussion! Submit an issue or reach out to us on info at
 dream-faster.ai for any inquiries. ## Licence & Usage We want to **bring much-
 needed transparency, speed and rigour** to the process of creating Time Series
 ML pipelines, while also building a sustainable business, that can support the
 ecosystem in the long-term. Fold's licence is inbetween [source-available]
 (https://en.wikipedia.org/wiki/Source-available_software) and a traditional
 commercial software licence. It requires a paid licence for any commercial use,
-after the initial, 30 day trial period. Deployment is only possible with the
-additional purchase of `fold-extended`, a product currently in development. We
-also want to contribute to open research by giving free access to non-
-commercial use of `fold`. If you are a researcher and would like to get access
-to Dream Faster's all of available tools, please contact_us_here. [Read more]
-(https://dream-faster.github.io/fold/product/license/) ## Limitations - No
+after the initial, 30 day trial period. We also want to contribute to open
+research by giving free access to non-commercial, research use of `fold`. [Read
+more](https://dream-faster.github.io/fold/product/license/) ## Limitations - No
 intermittent time series support, very limited support for missing values. - No
 hierarchical time series support.
```

### Comparing `fold_core-0.1.4/pyproject.toml` & `fold_core-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.1.4"
+version = "0.1.7"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -124,15 +124,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.1.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.1.4/src/fold/base.py` & `fold_core-0.1.7/src/fold/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 
 from __future__ import annotations
 
 import enum
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Callable, List, Optional, Tuple, TypeVar, Union
+from typing import Callable, Iterable, List, Optional, Tuple, TypeVar, Union
 
 import pandas as pd
 
+from fold.splitters import SingleWindowSplitter
+
 T = TypeVar("T", Optional[pd.Series], pd.Series)
 
 
 class Composite(ABC):
     """
     A Composite contains other transformations.
     """
@@ -56,15 +58,15 @@
         secondary_results: List[pd.DataFrame],
         y: Optional[pd.Series],
         in_sample: bool,
     ) -> pd.DataFrame:
         raise NotImplementedError
 
     @abstractmethod
-    def clone(self, clone_child_transformations: Callable) -> "Composite":
+    def clone(self, clone_child_transformations: Callable) -> Composite:
         raise NotImplementedError
 
     def before_fit(self, X: pd.DataFrame) -> None:
         pass
 
     def preprocess_primary(
         self, X: pd.DataFrame, index: int, y: T, fit: bool
@@ -78,14 +80,34 @@
         results_primary: List[pd.DataFrame],
         index: int,
         fit: bool,
     ) -> Tuple[pd.DataFrame, T]:
         return X, y
 
 
+class Optimizer(ABC):
+    splitter: SingleWindowSplitter
+
+    @abstractmethod
+    def get_candidates(self) -> Iterable["Pipeline"]:
+        raise NotImplementedError
+
+    @abstractmethod
+    def get_optimized_pipeline(self) -> Optional["Pipeline"]:
+        raise NotImplementedError
+
+    @abstractmethod
+    def process_candidate_results(self, results: List[pd.DataFrame]):
+        raise NotImplementedError
+
+    @abstractmethod
+    def clone(self, clone_child_transformations: Callable) -> Optimizer:
+        raise NotImplementedError
+
+
 class Transformation(ABC):
     """
     A transformation is a single step in a pipeline.
     """
 
     @dataclass
     class Properties:
@@ -145,14 +167,24 @@
 
 class InvertibleTransformation(Transformation, ABC):
     @abstractmethod
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         raise NotImplementedError
 
 
+class Tunable(ABC):
+    @abstractmethod
+    def get_params(self) -> dict:
+        raise NotImplementedError
+
+    @abstractmethod
+    def set_params(self, **parameters):
+        raise NotImplementedError
+
+
 class FeatureSelector(Transformation):
     selected_features: List[str]
 
 
 Transformations = Union[
     Transformation,
     "Composite",
```

### Comparing `fold_core-0.1.4/src/fold/composites/__init__.py` & `fold_core-0.1.7/src/fold/composites/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,11 +2,12 @@
 
 
 from ..base import Composite
 from .columns import EnsembleEachColumn, SkipNA, TransformEachColumn
 from .concat import Concat, Pipeline, TransformColumn
 from .ensemble import Ensemble
 from .metalabeling import MetaLabeling
+from .optimize import OptimizeGridSearch
 from .residual import ModelResiduals
 from .sample import Sample
 from .select import SelectBest
 from .target import TransformTarget
```

### Comparing `fold_core-0.1.4/src/fold/composites/columns.py` & `fold_core-0.1.7/src/fold/composites/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/composites/common.py` & `fold_core-0.1.7/src/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/composites/concat.py` & `fold_core-0.1.7/src/fold/composites/concat.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/composites/ensemble.py` & `fold_core-0.1.7/src/fold/composites/ensemble.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/composites/metalabeling.py` & `fold_core-0.1.7/src/fold/composites/metalabeling.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/composites/residual.py` & `fold_core-0.1.7/src/fold/composites/residual.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/composites/sample.py` & `fold_core-0.1.7/src/fold/composites/sample.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/composites/select.py` & `fold_core-0.1.7/src/fold/composites/select.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from __future__ import annotations
 
-from typing import Callable, List, Optional
+from typing import Callable, Iterable, List, Optional
 
 import pandas as pd
 
-from ..base import Composite, Pipelines, Transformations
+from ..base import Optimizer, Pipeline, Pipelines
 from .common import get_concatenated_names
 
 
-class SelectBest(Composite):
-    """
-    Don't use this just yet. Coming later.
-    """
-
-    properties = Composite.Properties()
+class SelectBest(Optimizer):
+    selected_pipeline: Optional[Pipeline] = None
 
     def __init__(
         self,
-        models: Pipelines,
+        pipelines: Pipelines,
         scorer: Callable,
         is_scorer_loss: bool = True,
-        selected_model: Optional[Transformations] = None,
     ) -> None:
-        self.models = models
-        self.name = "SelectBest-" + get_concatenated_names(models)
+        self.pipelines = pipelines
+        self.name = "SelectBest-" + get_concatenated_names(pipelines)
         self.scorer = scorer
         self.is_scorer_loss = is_scorer_loss
-        self.selected_model = selected_model
 
-    def postprocess_result_primary(
-        self, results: List[pd.DataFrame], y: Optional[pd.Series]
-    ) -> pd.DataFrame:
-        if self.selected_model is None:
-            scores = [self.scorer(y, result) for result in results]
-            selected_index = (
-                scores.index(min(scores))
-                if self.is_scorer_loss
-                else scores.index(max(scores))
-            )
-            self.selected_model = [self.models[selected_index]]
-            return results[selected_index]
-        else:
-            return results[0]
-
-    def get_child_transformations_primary(self) -> Pipelines:
-        if self.selected_model is None:
-            return self.models
-        else:
-            return self.selected_model
+    @classmethod
+    def from_cloned_instance(
+        cls,
+        pipelines: Pipelines,
+        scorer: Callable,
+        is_scorer_loss: bool,
+        selected_pipeline: Optional[Pipeline],
+    ) -> SelectBest:
+        instance = cls(pipelines, scorer, is_scorer_loss)
+        instance.selected_pipeline = selected_pipeline
+        return instance
+
+    def get_candidates(self) -> Iterable["Pipeline"]:
+        return self.pipelines
+
+    def get_optimized_pipeline(self) -> Optional["Pipeline"]:
+        return self.selected_pipeline
+
+    def process_candidate_results(self, results: List[pd.DataFrame], y: pd.Series):
+        if self.selected_pipeline is not None:
+            raise ValueError("Optimizer is already fitted.")
+
+        scores = [self.scorer(y, result) for result in results]
+        selected_index = (
+            scores.index(min(scores))
+            if self.is_scorer_loss
+            else scores.index(max(scores))
+        )
+        self.selected_pipeline = [self.pipelines[selected_index]]
 
     def clone(self, clone_child_transformations: Callable) -> SelectBest:
-        return SelectBest(
-            models=clone_child_transformations(self.models),
+        return SelectBest.from_cloned_instance(
+            pipelines=clone_child_transformations(self.pipelines),
             scorer=self.scorer,
             is_scorer_loss=self.is_scorer_loss,
-            selected_model=clone_child_transformations(self.selected_model)
-            if self.selected_model is not None
+            selected_pipeline=clone_child_transformations(self.selected_pipeline)
+            if self.selected_pipeline is not None
             else None,
         )
```

### Comparing `fold_core-0.1.4/src/fold/composites/target.py` & `fold_core-0.1.7/src/fold/composites/target.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/loop/backend/ray.py` & `fold_core-0.1.7/src/fold/loop/backend/ray.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,23 +31,24 @@
                 X, y, sample_weights, transformations, split, never_update, backend
             )
             for split in splits
         ]
     )
 
 
-def process_primary_child_transformations(
+def process_child_transformations(
     func: Callable,
     list_of_child_transformations_with_index: List,
     composite: Composite,
     X: pd.DataFrame,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
     stage: Stage,
     backend: Backend,
+    results_primary: Optional[List[pd.DataFrame]],
 ):
     func = ray.remote(func)
     X = ray.put(X)
     y = ray.put(y)
     return ray.get(
         [
             func.remote(
@@ -55,43 +56,12 @@
                 index,
                 child_transformation,
                 X,
                 y,
                 sample_weights,
                 stage,
                 backend,
-            )
-            for index, child_transformation in list_of_child_transformations_with_index
-        ]
-    )
-
-
-def process_secondary_child_transformations(
-    func: Callable,
-    list_of_child_transformations_with_index: List,
-    composite: Composite,
-    X: pd.DataFrame,
-    y: Optional[pd.Series],
-    sample_weights: Optional[pd.Series],
-    results_primary: List[pd.DataFrame],
-    stage: Stage,
-    backend: Backend,
-):
-    func = ray.remote(func)
-    X = ray.put(X)
-    y = ray.put(y)
-    return ray.get(
-        [
-            func.remote(
-                composite,
-                index,
-                child_transformation,
-                X,
-                y,
-                sample_weights,
                 results_primary,
-                stage,
-                backend,
             )
             for index, child_transformation in list_of_child_transformations_with_index
         ]
     )
```

### Comparing `fold_core-0.1.4/src/fold/loop/backend/sequential.py` & `fold_core-0.1.7/src/fold/loop/backend/sequential.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,50 +24,32 @@
 ):
     return [
         func(X, y, sample_weights, transformations, split, never_update, backend)
         for split in tqdm(splits, disable=silent)
     ]
 
 
-def process_primary_child_transformations(
+def process_child_transformations(
     func: Callable,
     list_of_child_transformations_with_index: List,
     composite: Composite,
     X: pd.DataFrame,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
     stage: Stage,
     backend: Backend,
-):
-    return [
-        func(
-            composite, index, child_transformation, X, y, sample_weights, stage, backend
-        )
-        for index, child_transformation in list_of_child_transformations_with_index
-    ]
-
-
-def process_secondary_child_transformations(
-    func: Callable,
-    list_of_child_transformations_with_index: List,
-    composite: Composite,
-    X: pd.DataFrame,
-    y: Optional[pd.Series],
-    sample_weights: Optional[pd.Series],
-    results_primary: List[pd.DataFrame],
-    stage: Stage,
-    backend: Backend,
+    results_primary: Optional[List[pd.DataFrame]],
 ):
     return [
         func(
             composite,
             index,
             child_transformation,
             X,
             y,
             sample_weights,
-            results_primary,
             stage,
             backend,
+            results_primary,
         )
         for index, child_transformation in list_of_child_transformations_with_index
     ]
```

### Comparing `fold_core-0.1.4/src/fold/loop/backtesting.py` & `fold_core-0.1.7/src/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/loop/checks.py` & `fold_core-0.1.7/src/fold/loop/checks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
+from logging import warn
 from typing import Optional, Tuple
 
 import pandas as pd
 
+from ..utils.trim import trim_initial_nans
+
 
 def check_types(
     X: Optional[pd.DataFrame], y: pd.Series
 ) -> Tuple[pd.DataFrame, pd.Series]:
     if X is None:
         X = pd.DataFrame(0, index=y.index, columns=["X_not_available"])
     else:
         assert isinstance(X, pd.DataFrame), "X must be a pandas DataFrame."
     assert isinstance(y, pd.Series), "y must be a pandas Series."
+
+    X_trimmed, _ = trim_initial_nans(X, y)
+    if len(X_trimmed) < len(X):
+        warn(
+            f"Detected initial NaNs in X ({ len(X) - len(X_trimmed) } instances), that'll be trimmed internally. Please trim your data before passing it to the model."
+        )
     return X, y
+
+
+def check_types_multi_series(data: pd.DataFrame):
+    assert isinstance(data, pd.DataFrame), "data must be a pandas DataFrame."
+    assert "y" in data.columns, "data must have a column `y`."
+    assert "ds" in data.columns, "data must have a column `ds`."
+    assert "unique_id" in data.columns, "data must have a column `unique_id`."
```

### Comparing `fold_core-0.1.4/src/fold/loop/common.py` & `fold_core-0.1.7/src/fold/loop/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import List, Optional
 
 import pandas as pd
 
-from ..base import Composite, Transformation, Transformations
+from ..base import Composite, Optimizer, Transformation, Transformations
 from ..models.base import Model
 from ..utils.checks import is_prediction, is_X_available
 from ..utils.trim import trim_initial_nans
 from .backend import get_backend_dependent_functions
 from .memory import postprocess_X_y_into_memory, preprocess_X_y_with_memory
 from .types import Backend, Stage
 
@@ -38,14 +38,17 @@
                 X, y, sample_weights, transformation, stage, backend
             )
         return X
 
     elif isinstance(transformations, Composite):
         return process_composite(transformations, X, y, sample_weights, stage, backend)
 
+    elif isinstance(transformations, Optimizer):
+        return process_optimizer(transformations, X, y, sample_weights, stage, backend)
+
     elif isinstance(transformations, Transformation) or isinstance(
         transformations, Model
     ):
         # If the transformation needs to be "online", and we're in the update stage, we need to run the inner loop.
         if (
             transformations.properties.mode == Transformation.Properties.Mode.online
             and stage in [Stage.update, Stage.update_online_only]
@@ -84,23 +87,24 @@
     backend: Backend,
 ) -> pd.DataFrame:
     backend_functions = get_backend_dependent_functions(backend)
 
     composite.before_fit(X)
     primary_transformations = composite.get_child_transformations_primary()
 
-    results_primary = backend_functions.process_primary_child_transformations(
+    results_primary = backend_functions.process_child_transformations(
         __process_primary_child_transform,
         enumerate(primary_transformations),
         composite,
         X,
         y,
         sample_weights,
         stage,
         backend,
+        None,
     )
 
     if composite.properties.primary_only_single_pipeline:
         assert len(results_primary) == 1, ValueError(
             "Expected single output from primary transformations, got"
             f" {len(results_primary)} instead."
         )
@@ -110,24 +114,24 @@
         )
 
     secondary_transformations = composite.get_child_transformations_secondary()
 
     if secondary_transformations is None:
         return composite.postprocess_result_primary(results_primary, y)
 
-    results_secondary = backend_functions.process_secondary_child_transformations(
+    results_secondary = backend_functions.process_child_transformations(
         __process_secondary_child_transform,
         enumerate(secondary_transformations),
         composite,
         X,
         y,
         sample_weights,
-        results_primary,
         stage,
         backend,
+        results_primary,
     )
 
     if composite.properties.secondary_only_single_pipeline:
         assert len(results_secondary) == 1, ValueError(
             "Expected single output from secondary transformations, got"
             f" {len(results_secondary)} instead."
         )
@@ -138,14 +142,48 @@
         )
 
     return composite.postprocess_result_secondary(
         results_primary, results_secondary, y, in_sample=stage == Stage.inital_fit
     )
 
 
+def process_optimizer(
+    optimizer: Optimizer,
+    X: pd.DataFrame,
+    y: Optional[pd.Series],
+    sample_weights: Optional[pd.Series],
+    stage: Stage,
+    backend: Backend,
+) -> pd.DataFrame:
+    backend_functions = get_backend_dependent_functions(backend)
+
+    optimized_pipeline = optimizer.get_optimized_pipeline()
+    if optimized_pipeline is None:
+        # Optimized needs to run the search
+        candidates = optimizer.get_candidates()
+
+        results_primary = backend_functions.process_child_transformations(
+            __process_candidates,
+            enumerate(candidates),
+            optimizer,
+            X,
+            y,
+            sample_weights,
+            stage,
+            backend,
+            None,
+        )
+        optimizer.process_candidate_results(results_primary, y)
+
+    optimized_pipeline = optimizer.get_optimized_pipeline()
+    return recursively_transform(
+        X, y, sample_weights, optimized_pipeline, stage, backend
+    )
+
+
 def process_with_inner_loop(
     transformation: Transformation,
     X: pd.DataFrame,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
 ) -> pd.DataFrame:
     if len(X) == 0:
@@ -238,38 +276,53 @@
     # 3. update (if we're in the update stage)
     if stage == Stage.update:
         transformation.update(X_with_memory, y_with_memory, sample_weights)
         postprocess_X_y_into_memory(transformation, X, y, False)
     return return_value.loc[X.index]
 
 
+def __process_candidates(
+    optimizer: Optimizer,
+    index: int,
+    child_transform: Transformations,
+    X: pd.DataFrame,
+    y: Optional[pd.Series],
+    sample_weights: Optional[pd.Series],
+    stage: Stage,
+    backend: Backend,
+    results_primary: Optional[List[pd.DataFrame]],
+) -> pd.DataFrame:
+    return recursively_transform(X, y, sample_weights, child_transform, stage, backend)
+
+
 def __process_primary_child_transform(
     composite: Composite,
     index: int,
     child_transform: Transformations,
     X: pd.DataFrame,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
     stage: Stage,
     backend: Backend,
+    results_primary: Optional[List[pd.DataFrame]],
 ) -> pd.DataFrame:
     X, y = composite.preprocess_primary(X, index, y, fit=stage.is_fit_or_update())
     return recursively_transform(X, y, sample_weights, child_transform, stage, backend)
 
 
 def __process_secondary_child_transform(
     composite: Composite,
     index: int,
     child_transform: Transformations,
     X: pd.DataFrame,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
-    results_primary: List[pd.DataFrame],
     stage: Stage,
     backend: Backend,
+    results_primary: Optional[List[pd.DataFrame]],
 ) -> pd.DataFrame:
     X, y = composite.preprocess_secondary(
         X, y, results_primary, index, fit=stage.is_fit_or_update()
     )
     return recursively_transform(X, y, sample_weights, child_transform, stage, backend)
```

### Comparing `fold_core-0.1.4/src/fold/loop/convenience.py` & `fold_core-0.1.7/src/fold/loop/wrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,37 +14,39 @@
     WrapSKLearnRegressor,
 )
 from fold.transformations.sklearn import (
     WrapSKLearnFeatureSelector,
     WrapSKLearnTransformation,
 )
 
-from ..base import Composite, Pipeline, Transformation
+from ..base import Composite, Optimizer, Pipeline, Transformation
 from ..transformations.function import WrapFunction
 
 
-def replace_transformation_if_not_fold_native(
+def wrap_transformation_if_needed(
     transformation: Pipeline,
 ) -> Pipeline:
     if isinstance(transformation, List):
-        return [replace_transformation_if_not_fold_native(t) for t in transformation]
+        return [wrap_transformation_if_needed(t) for t in transformation]
     elif isinstance(transformation, RegressorMixin):
-        return WrapSKLearnRegressor(transformation)
+        return WrapSKLearnRegressor.from_model(transformation)
     elif isinstance(transformation, ClassifierMixin):
-        return WrapSKLearnClassifier(transformation)
+        return WrapSKLearnClassifier.from_model(transformation)
     elif isinstance(transformation, Callable):
         return WrapFunction(transformation, None)
     elif isinstance(transformation, SelectorMixin):
-        return WrapSKLearnFeatureSelector(transformation)
+        return WrapSKLearnFeatureSelector.from_model(transformation)
     elif isinstance(transformation, TransformerMixin):
-        return WrapSKLearnTransformation(transformation)
+        return WrapSKLearnTransformation.from_model(transformation)
     elif isinstance(transformation, SKLearnPipeline):
         return WrapSKLearnPipeline(transformation)
     elif isinstance(transformation, Composite):
-        return transformation.clone(replace_transformation_if_not_fold_native)
+        return transformation.clone(wrap_transformation_if_needed)
+    elif isinstance(transformation, Optimizer):
+        return transformation.clone(wrap_transformation_if_needed)
     elif isinstance(transformation, Transformation):
         return transformation
     elif find_spec("fold_wrappers") is not None:
         from fold_wrappers.convenience import wrap_transformation_if_possible
 
         return wrap_transformation_if_possible(transformation)
     else:
```

### Comparing `fold_core-0.1.4/src/fold/loop/encase.py` & `fold_core-0.1.7/src/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/loop/inference.py` & `fold_core-0.1.7/src/fold/loop/inference.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/loop/memory.py` & `fold_core-0.1.7/src/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/loop/training.py` & `fold_core-0.1.7/src/fold/loop/training.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import (
-    Composite,
-    DeployablePipeline,
-    Pipeline,
-    TrainedPipelines,
-    Transformation,
-)
+from ..base import DeployablePipeline, Pipeline, TrainedPipelines
 from ..splitters import Fold, SlidingWindowSplitter, Splitter
 from ..utils.list import wrap_in_list
 from .backend import get_backend_dependent_functions
 from .checks import check_types
 from .common import deepcopy_pipelines, recursively_transform
-from .convenience import replace_transformation_if_not_fold_native
 from .types import Backend, Stage, TrainMethod
+from .wrap import wrap_transformation_if_needed
 
 
 def train(
     pipeline: Pipeline,
     X: Optional[pd.DataFrame],
     y: pd.Series,
     splitter: Splitter,
@@ -59,41 +53,41 @@
         The fitted pipelines, for all folds.
     """
     X, y = check_types(X, y)
     train_method = TrainMethod.from_str(train_method)
     backend = Backend.from_str(backend)
 
     if isinstance(splitter, SlidingWindowSplitter):
-        assert train_method == TrainMethod.parallel, (
+        assert train_method != TrainMethod.sequential, (
             "SlidingWindowSplitter is conceptually incompatible with"
             " TrainMethod.sequential"
         )
 
     pipeline = wrap_in_list(pipeline)
-    pipeline = replace_transformation_if_not_fold_native(pipeline)
+    pipeline = wrap_transformation_if_needed(pipeline)
 
     splits = splitter.splits(length=len(y))
     backend_functions = get_backend_dependent_functions(backend)
     if len(splits) == 0:
         raise ValueError("No splits were generated by the Splitter.")
 
     if train_method == TrainMethod.parallel_with_search and len(splits) > 1:
-        first_batch_index, first_batch_transformations = process_pipeline_window(
+        first_batch_index, first_batch_transformations = _process_pipeline_window(
             X,
             y,
             sample_weights,
             pipeline,
             splits[0],
             never_update=True,
             backend=backend,
         )
 
         rest_idx, rest_transformations = zip(
             *backend_functions.train_transformations(
-                process_pipeline_window,
+                _process_pipeline_window,
                 first_batch_transformations,
                 X,
                 y,
                 sample_weights,
                 splits[1:],
                 False,
                 backend,
@@ -101,15 +95,15 @@
             )
         )
         processed_idx = [first_batch_index] + list(rest_idx)
         processed_pipelines = [first_batch_transformations] + list(rest_transformations)
     elif train_method == TrainMethod.parallel and len(splits) > 1:
         processed_idx, processed_pipelines = zip(
             *backend_functions.train_transformations(
-                process_pipeline_window,
+                _process_pipeline_window,
                 pipeline,
                 X,
                 y,
                 sample_weights,
                 splits,
                 True,
                 backend,
@@ -118,15 +112,15 @@
         )
 
     else:
         processed_idx = []
         processed_pipelines = []
         processed_pipeline = pipeline
         for split in splits:
-            processed_id, processed_pipeline = process_pipeline_window(
+            processed_id, processed_pipeline = _process_pipeline_window(
                 X,
                 y,
                 sample_weights,
                 processed_pipeline,
                 split,
                 False,
                 backend,
@@ -149,16 +143,16 @@
     X: pd.DataFrame,
     y: pd.Series,
     sample_weights: Optional[pd.Series] = None,
 ) -> DeployablePipeline:
     X, y = check_types(X, y)
 
     pipeline = wrap_in_list(pipeline)
-    pipeline = replace_transformation_if_not_fold_native(pipeline)
-    _, transformations = process_pipeline_window(
+    pipeline = wrap_transformation_if_needed(pipeline)
+    _, transformations = _process_pipeline_window(
         X,
         y,
         sample_weights,
         pipeline,
         Fold(
             order=0,
             model_index=0,
@@ -171,38 +165,38 @@
         ),
         True,
         backend=Backend.no,
     )
     return transformations
 
 
-def process_pipeline_window(
+def _process_pipeline_window(
     X: pd.DataFrame,
     y: pd.Series,
     sample_weights: Optional[pd.Series],
-    transformations: List[Union[Transformation, Composite]],
+    pipeline: Pipeline,
     split: Fold,
     never_update: bool,
     backend: Backend,
-) -> Tuple[int, List[Union[Transformation, Composite]]]:
+) -> Tuple[int, Pipeline]:
     stage = Stage.inital_fit if (split.order == 0 or never_update) else Stage.update
     window_start = (
         split.update_window_start if stage == Stage.update else split.train_window_start
     )
     window_end = (
         split.update_window_end if stage == Stage.update else split.train_window_end
     )
-    X_train = X.iloc[window_start:window_end]
+    X_train: pd.DataFrame = X.iloc[window_start:window_end]  # type: ignore
     y_train = y.iloc[window_start:window_end]
 
     sample_weights_train = (
         sample_weights.iloc[window_start:window_end]
         if sample_weights is not None
         else None
     )
 
-    transformations = deepcopy_pipelines(transformations)
+    pipeline = deepcopy_pipelines(pipeline)
     X_train = recursively_transform(
-        X_train, y_train, sample_weights_train, transformations, stage, backend
+        X_train, y_train, sample_weights_train, pipeline, stage, backend
     )
 
-    return split.model_index, transformations
+    return split.model_index, pipeline
```

### Comparing `fold_core-0.1.4/src/fold/loop/types.py` & `fold_core-0.1.7/src/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/loop/update.py` & `fold_core-0.1.7/src/fold/loop/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/models/base.py` & `fold_core-0.1.7/src/fold/models/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/models/baseline.py` & `fold_core-0.1.7/src/fold/models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/models/dummy.py` & `fold_core-0.1.7/src/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/models/random.py` & `fold_core-0.1.7/src/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/models/sklearn.py` & `fold_core-0.1.7/src/fold/models/sklearn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
+from __future__ import annotations
 
-from typing import Optional, Union
+from typing import Optional, Type, Union
 
 import pandas as pd
 
-from ..base import Transformation, fit_noop
+from ..base import Transformation, Tunable, fit_noop
 from .base import Model
 
 
-class WrapSKLearnClassifier(Model):
+class WrapSKLearnClassifier(Model, Tunable):
     """
     Wraps an SKLearn Classifier model.
     There's no need to use it directly, `fold` automatically wraps all sklearn classifiers into this class.
     """
 
     properties = Model.Properties(
         requires_X=True, model_type=Model.Properties.ModelType.classifier
     )
 
-    def __init__(self, model) -> None:
-        self.model = model
-        self.name = model.__class__.__name__
+    def __init__(
+        self,
+        model_class: Type,
+        init_args: dict,
+    ) -> None:
+        self.model = model_class(**init_args)
+        self.name = self.model.__class__.__name__
+
+    @classmethod
+    def from_model(cls, model) -> WrapSKLearnClassifier:
+        return cls(model_class=model.__class__, init_args=model.get_params())
 
     def fit(
         self, X: pd.DataFrame, y: pd.Series, sample_weights: Optional[pd.Series] = None
     ) -> None:
         if hasattr(self.model, "partial_fit"):
             self.model.partial_fit(X, y, sample_weights)
         else:
@@ -54,28 +63,42 @@
             index=X.index,
             name=f"predictions_{self.name}",
         )
         return pd.concat([predictions, probabilities], axis="columns")
 
     predict_in_sample = predict
 
+    def get_params(self) -> dict:
+        return self.model.get_params()
+
+    def set_params(self, **params) -> None:
+        self.model.set_params(**params)
+
 
-class WrapSKLearnRegressor(Model):
+class WrapSKLearnRegressor(Model, Tunable):
     """
     Wraps an SKLearn regressor model.
     There's no need to use it directly, `fold` automatically wraps all sklearn regressors into this class.
     """
 
     properties = Model.Properties(
         requires_X=True, model_type=Model.Properties.ModelType.regressor
     )
 
-    def __init__(self, model) -> None:
-        self.model = model
-        self.name = model.__class__.__name__
+    def __init__(
+        self,
+        model_class: Type,
+        init_args: dict,
+    ) -> None:
+        self.model = model_class(**init_args)
+        self.name = self.model.__class__.__name__
+
+    @classmethod
+    def from_model(cls, model) -> WrapSKLearnRegressor:
+        return cls(model_class=model.__class__, init_args=model.get_params())
 
     def fit(
         self, X: pd.DataFrame, y: pd.Series, sample_weights: Optional[pd.Series] = None
     ) -> None:
         if hasattr(self.model, "partial_fit"):
             self.model.partial_fit(X, y, sample_weights)
         else:
@@ -96,14 +119,20 @@
             data=self.model.predict(X).squeeze(),
             index=X.index,
             name=f"predictions_{self.name}",
         ).to_frame()
 
     predict_in_sample = predict
 
+    def get_params(self) -> dict:
+        return self.model.get_params()
+
+    def set_params(self, **params) -> None:
+        self.model.set_params(**params)
+
 
 class WrapSKLearnPipeline(Model):
     """
     Wraps an scikit-learn Pipeline.
     It's usage is discouraged, as it's not possible to update an scikit-learn Pipeline with new data.
     Fold has all the primitives that scikit-learn Pipelines provide, just wrap your Transformations into an array.
     """
```

### Comparing `fold_core-0.1.4/src/fold/splitters.py` & `fold_core-0.1.7/src/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/transformations/__init__.py` & `fold_core-0.1.7/src/fold/transformations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     AddMonth,
     AddQuarter,
     AddSecond,
     AddWeek,
     AddWeekOfYear,
     AddYear,
 )
-from .difference import Difference
+from .difference import Difference, TakeReturns
 from .function import WrapFunction
 from .holidays import AddHolidayFeatures
 from .lags import AddLagsX, AddLagsY
-from .math import AddConstant, TakeLog, TurnPositive
+from .math import AddConstant, MultiplyBy, TakeLog, TurnPositive
+from .scaling import MinMaxScaler, StandardScaler
 from .sklearn import WrapSKLearnFeatureSelector, WrapSKLearnTransformation
 from .update import DontUpdate
 from .window import AddWindowFeatures
```

### Comparing `fold_core-0.1.4/src/fold/transformations/columns.py` & `fold_core-0.1.7/src/fold/transformations/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/transformations/date.py` & `fold_core-0.1.7/src/fold/transformations/date.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/transformations/dev.py` & `fold_core-0.1.7/src/fold/transformations/dev.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 
 class Breakpoint(Transformation):
     """
     A transformation that stops execution at the specified point.
     """
 
+    name = "Breakpoint"
     properties = Transformation.Properties(requires_X=False)
 
     def __init__(
         self,
         stop_at_fit: bool = True,
         stop_at_update: bool = True,
         stop_at_transform: bool = True,
     ) -> None:
-        self.name = "Debug"
         self.stop_at_fit = stop_at_fit
         self.stop_at_update = stop_at_update
         self.stop_at_transform = stop_at_transform
 
     def fit(
         self,
         X: pd.DataFrame,
@@ -67,23 +67,23 @@
     properties = InvertibleTransformation.Properties(requires_X=False)
     __test__ = False
     no_of_calls_fit = 0
     no_of_calls_update = 0
     no_of_calls_transform_insample = 0
     no_of_calls_transform_outofsample = 0
     no_of_calls_inverse_transform = 0
+    name = "Test"
 
     def __init__(
         self,
         fit_func: Callable,
         transform_func: Callable,
         update_func: Optional[Callable] = None,
         inverse_transform_func: Optional[Callable] = None,
     ) -> None:
-        self.name = "Test"
         self.fit_func = fit_func
         self.transform_func = transform_func
         self.update_func = update_func
         self.inverse_transform_func = inverse_transform_func
 
     def fit(
         self,
@@ -138,7 +138,27 @@
         return return_value
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         self.no_of_calls_inverse_transform += 1
         if self.inverse_transform_func is not None:
             return self.inverse_transform_func(X)
         return X
+
+
+class Lookahead(Transformation):
+    """
+    A transformation that stops execution at the specified point.
+    """
+
+    name = "Lookahead"
+    properties = Transformation.Properties(
+        requires_X=False,
+        mode=Transformation.Properties.Mode.online,
+        memory_size=0,
+        _internal_supports_minibatch_backtesting=True,
+    )
+
+    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+        return self._state.memory_y.to_frame()
+
+    fit = fit_noop
+    update = fit
```

### Comparing `fold_core-0.1.4/src/fold/transformations/difference.py` & `fold_core-0.1.7/src/fold/transformations/difference.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import Optional
+from typing import Optional, Union
 
 import pandas as pd
 
-from ..base import InvertibleTransformation
+from ..base import InvertibleTransformation, Transformation
 from ..utils.dataframe import to_series
 
 
 class Difference(InvertibleTransformation):
     """
     Performs differencing.
     Sesonal differencing can be achieved by setting `lag` to the seasonality of the data.
@@ -51,19 +51,21 @@
     References
     ----------
 
     [Stationarity and differencing](https://otexts.com/fpp2/stationarity.html)
     """
 
     name = "Difference"
-    first_values_X: Optional[pd.DataFrame] = None
+    properties = InvertibleTransformation.Properties(requires_X=False)
+
+    first_values_X: Optional[Union[pd.DataFrame, pd.Series]] = None
+    last_values_X: Optional[Union[pd.DataFrame, pd.Series]] = None
 
     def __init__(self, lag: int = 1) -> None:
         self.lag = lag
-        self.properties = InvertibleTransformation.Properties(requires_X=False)
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
     ) -> None:
@@ -96,7 +98,74 @@
                 X.iloc[i :: self.lag] = X.iloc[i :: self.lag].cumsum()
             return X
         else:
             X = pd.concat([to_series(self.last_values_X), X], axis="index")
             for i in range(self.lag):
                 X.iloc[i :: self.lag] = X.iloc[i :: self.lag].cumsum()
             return X.iloc[self.lag :]
+
+
+class TakeReturns(Transformation):
+    """
+    Takes the returns (percentage change between the current and a prior element).
+
+    Examples
+    --------
+    ```pycon
+    >>> from fold.loop import train_backtest
+    >>> from fold.splitters import SlidingWindowSplitter
+    >>> from fold.transformations import TakeReturns
+    >>> from fold.utils.tests import generate_sine_wave_data
+    >>> X, y  = generate_sine_wave_data(freq="min")
+    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> pipeline = TakeReturns()
+    >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
+    >>> X["sine"].loc[preds.index].head()
+    2021-12-31 15:40:00   -0.0000
+    2021-12-31 15:41:00    0.0126
+    2021-12-31 15:42:00    0.0251
+    2021-12-31 15:43:00    0.0377
+    2021-12-31 15:44:00    0.0502
+    Freq: T, Name: sine, dtype: float64
+    >>> preds["sine"].head()
+    2021-12-31 15:40:00   -1.000000
+    2021-12-31 15:41:00        -inf
+    2021-12-31 15:42:00    0.992063
+    2021-12-31 15:43:00    0.501992
+    2021-12-31 15:44:00    0.331565
+    Freq: T, Name: sine, dtype: float64
+
+    ```
+
+    References
+    ----------
+
+    """
+
+    name = "TakeReturns"
+    properties = InvertibleTransformation.Properties(requires_X=False)
+
+    last_values_X: Optional[Union[pd.DataFrame, pd.Series]] = None
+
+    def fit(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        sample_weights: Optional[pd.Series] = None,
+    ) -> None:
+        self.last_values_X = X.iloc[-1:None]
+
+    def update(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        sample_weights: Optional[pd.Series] = None,
+    ) -> None:
+        self.last_values_X = X.iloc[-1:None]
+
+    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+        if in_sample:
+            return X.pct_change()
+        else:
+            return (
+                pd.concat([self.last_values_X, X], axis="index").pct_change().iloc[1:]
+            )
```

### Comparing `fold_core-0.1.4/src/fold/transformations/function.py` & `fold_core-0.1.7/src/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/transformations/holidays.py` & `fold_core-0.1.7/src/fold/transformations/holidays.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/transformations/lags.py` & `fold_core-0.1.7/src/fold/transformations/lags.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 from typing import List, Tuple, Union
 
 import pandas as pd
 
 from fold.utils.checks import is_X_available
 
-from ..base import Transformation, fit_noop
+from ..base import Transformation, Tunable, fit_noop
 from ..utils.list import flatten, transform_range_to_list, wrap_in_list
 
 
-class AddLagsY(Transformation):
+class AddLagsY(Transformation, Tunable):
     """
     Adds past values of `y`.
 
     Parameters
     ----------
     lags : List[int], range
         A list of lags (of the target) to add as features.
@@ -70,16 +70,29 @@
         else:
             # If X is just an DataFrame with zeros, then just return the lags
             return lags
 
     fit = fit_noop
     update = fit_noop
 
+    def get_params(self) -> dict:
+        return {"lags": self.lags}
 
-class AddLagsX(Transformation):
+    def set_params(self, **parameters):
+        for parameter, value in parameters.items():
+            setattr(self, parameter, value)
+        self.properties = Transformation.Properties(
+            requires_X=False,
+            mode=Transformation.Properties.Mode.online,
+            memory_size=max(self.lags),
+            _internal_supports_minibatch_backtesting=True,
+        )
+
+
+class AddLagsX(Transformation, Tunable):
     """
     Adds past values of `X` for the desired column(s).
 
     Parameters
     ----------
     columns_and_lags : List[ColumnAndLag], ColumnAndLag
         A tuple (or a list of tuples) of the column name and a single or a list of lags to add as features.
@@ -148,7 +161,18 @@
                     )
                 else:
                     X_lagged[f"{column}_lag_{lag}"] = X[column].shift(lag)[-len(X) :]
         return pd.concat([X, X_lagged], axis="columns")
 
     fit = fit_noop
     update = fit_noop
+
+    def get_params(self) -> dict:
+        return {"columns_and_lags": self.columns_and_lags}
+
+    def set_params(self, **parameters):
+        for parameter, value in parameters.items():
+            setattr(self, parameter, value)
+        self.properties = Transformation.Properties(
+            requires_X=True,
+            memory_size=max(flatten([l for _, l in self.columns_and_lags])),
+        )
```

### Comparing `fold_core-0.1.4/src/fold/transformations/math.py` & `fold_core-0.1.7/src/fold/transformations/math.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 
 from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-from fold.base import InvertibleTransformation, fit_noop
+from fold.base import InvertibleTransformation, Tunable, fit_noop
 
 
-class TakeLog(InvertibleTransformation):
+class TakeLog(InvertibleTransformation, Tunable):
     """
     Takes the logarithm of the data.
 
     Parameters
     ----------
     base : int, str, optional
         The base of the logarithm, by default "e".
@@ -78,16 +78,23 @@
             return 2**X
         else:
             raise ValueError(f"Invalid base: {self.base}")
 
     fit = fit_noop
     update = fit_noop
 
+    def get_params(self) -> dict:
+        return {"base": self.base}
 
-class AddConstant(InvertibleTransformation):
+    def set_params(self, **parameters):
+        for parameter, value in parameters.items():
+            setattr(self, parameter, value)
+
+
+class AddConstant(InvertibleTransformation, Tunable):
 
     """
     Adds a constant to the data.
 
     Parameters
     ----------
     constant: int, float, Dict[str, Union[float, int]]
@@ -154,14 +161,21 @@
         if constant is dict:
             constant = next(iter(constant.values()))
         return X - constant
 
     fit = fit_noop
     update = fit_noop
 
+    def get_params(self) -> dict:
+        return {"constant": self.constant}
+
+    def set_params(self, **parameters):
+        for parameter, value in parameters.items():
+            setattr(self, parameter, value)
+
 
 class TurnPositive(InvertibleTransformation):
     """
     Adds a constant to the data, varying by column, so that all values are positive.
     It identifies the constant during training, and applies it during inference (and backtesting).
     Therefore there's no guarantee that the data will be positive during inference (and backtesting).
 
@@ -216,7 +230,36 @@
             axis="columns",
         )
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         return X - next(iter(self.constant.values()))
 
     update = fit_noop
+
+
+class MultiplyBy(InvertibleTransformation, Tunable):
+    """
+    Multiplies the data by a constant.
+    """
+
+    name = "MultiplyBy"
+    properties = InvertibleTransformation.Properties(requires_X=True)
+    constant: float
+
+    def __init__(self, constant: float) -> None:
+        self.constant = constant
+
+    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+        return X * self.constant
+
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
+        return X / self.constant
+
+    fit = fit_noop
+    update = fit_noop
+
+    def get_params(self) -> dict:
+        return {"constant": self.constant}
+
+    def set_params(self, **parameters):
+        for parameter, value in parameters.items():
+            setattr(self, parameter, value)
```

### Comparing `fold_core-0.1.4/src/fold/transformations/sklearn.py` & `fold_core-0.1.7/src/fold/transformations/sklearn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
+from __future__ import annotations
 
 from inspect import getfullargspec
-from typing import Optional
+from typing import Optional, Type
 
 import pandas as pd
 
-from ..base import FeatureSelector, Transformation, fit_noop
+from ..base import (
+    FeatureSelector,
+    InvertibleTransformation,
+    Transformation,
+    Tunable,
+    fit_noop,
+)
 
 
-class WrapSKLearnTransformation(Transformation):
+class WrapSKLearnTransformation(Transformation, Tunable):
     """
     Wraps an SKLearn Transformation.
     There's no need to use it directly, `fold` automatically wraps all sklearn transformations into this class.
     """
 
     properties = Transformation.Properties(requires_X=True)
 
-    def __init__(self, transformation) -> None:
-        if hasattr(transformation, "set_output"):
-            transformation = transformation.set_output(transform="pandas")
-        self.transformation = transformation
-        self.name = transformation.__class__.__name__
+    def __init__(
+        self,
+        transformation_class: Type,
+        init_args: dict,
+    ) -> None:
+        self.transformation = transformation_class(**init_args)
+        if hasattr(self.transformation, "set_output"):
+            self.transformation = self.transformation.set_output(transform="pandas")
+        self.name = self.transformation.__class__.__name__
+
+    @classmethod
+    def from_model(cls, model) -> WrapSKLearnTransformation:
+        return cls(transformation_class=model.__class__, init_args=model.get_params())
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
     ) -> None:
@@ -57,32 +72,50 @@
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         if hasattr(self.transformation, "set_output"):
             return self.transformation.transform(X)
         else:
             return pd.DataFrame(self.transformation.transform(X), columns=X.columns)
 
+    def get_params(self) -> dict:
+        return self.transformation.get_params()
+
+    def set_params(self, **params) -> None:
+        self.transformation.set_params(**params)
+
+
+class WrapInvertibleSKLearnTransformation(
+    WrapSKLearnTransformation, InvertibleTransformation
+):
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         return pd.Series(self.transformation.inverse_transform(X), index=X.index)
 
 
-class WrapSKLearnFeatureSelector(FeatureSelector):
+class WrapSKLearnFeatureSelector(FeatureSelector, Tunable):
     """
     Wraps an SKLearn Feature Selector class, stores the selected columns in `selected_features` property.
     There's no need to use it directly, `fold` automatically wraps all sklearn feature selectors into this class.
     """
 
     properties = Transformation.Properties(requires_X=True)
     selected_features: Optional[str] = None
 
-    def __init__(self, transformation) -> None:
-        if hasattr(transformation, "set_output"):
-            transformation = transformation.set_output(transform="pandas")
-        self.transformation = transformation
-        self.name = transformation.__class__.__name__
+    def __init__(
+        self,
+        transformation_class: Type,
+        init_args: dict,
+    ) -> None:
+        self.transformation = transformation_class(**init_args)
+        if hasattr(self.transformation, "set_output"):
+            self.transformation = self.transformation.set_output(transform="pandas")
+        self.name = self.transformation.__class__.__name__
+
+    @classmethod
+    def from_model(cls, model) -> WrapSKLearnFeatureSelector:
+        return cls(transformation_class=model.__class__, init_args=model.get_params())
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
     ) -> None:
@@ -93,8 +126,14 @@
             self.selected_features = X.columns[
                 self.transformation.get_support()
             ].to_list()
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         return X[self.selected_features]
 
+    def get_params(self) -> dict:
+        return self.transformation.get_params()
+
+    def set_params(self, **params) -> None:
+        self.transformation.set_params(**params)
+
     update = fit_noop
```

### Comparing `fold_core-0.1.4/src/fold/transformations/update.py` & `fold_core-0.1.7/src/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/transformations/window.py` & `fold_core-0.1.7/src/fold/transformations/window.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/utils/checks.py` & `fold_core-0.1.7/src/fold/utils/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from typing import List
 
 import pandas as pd
 
+from fold.utils.dataframe import to_series
+
 
 def is_prediction(input: pd.DataFrame) -> bool:
     if len(input.columns) == 1:
         return (
             input.columns[0].startswith("predictions_")
             if isinstance(input.columns[0], str)
             else False
@@ -33,15 +35,15 @@
             or (len(df.columns) == 1 and df.isna().sum()[0] == len(df))
             for df in results
         ]
     )
 
 
 def get_prediction_column(input: pd.DataFrame) -> pd.Series:
-    return input[get_prediction_column_name(input)].squeeze()
+    return to_series(input[get_prediction_column_name(input)])
 
 
 def get_prediction_column_name(input: pd.DataFrame) -> str:
     candidates = [col for col in input.columns if col.startswith("predictions_")]
     if len(candidates) == 0:
         if len(input.columns) == 1:
             return input.columns[0]
```

### Comparing `fold_core-0.1.4/src/fold/utils/dataframe.py` & `fold_core-0.1.7/src/fold/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/utils/dataset.py` & `fold_core-0.1.7/src/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/utils/list.py` & `fold_core-0.1.7/src/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/src/fold/utils/trim.py` & `fold_core-0.1.7/src/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.4/PKG-INFO` & `fold_core-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.1.4
+Version: 0.1.7
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
 Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
@@ -215,15 +215,15 @@
         Collection Link
         </a>
     </td>
     <td> - </td>
   </tr>
   <tr>
     <td> 
-    🖋️ Back to the Future with Time Series Forecasting
+    🖋️ Why we ended up building an Adaptive ML engine for Time Series
     </td>
     <td>Blog</td>
     <td>Public Release Blog Post </td>
     <td> 
         <a href='https://www.appliedexploration.com/p/back-to-the-future-with-time-series' target="_blank">
         Blog post on Applied Exploration 
         </a>
@@ -270,17 +270,17 @@
 Join our   <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a> for live discussion! 
 
 Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
 
 ## Licence & Usage
 
 We want to **bring much-needed transparency, speed and rigour** to the process of creating Time Series ML pipelines, while also building a sustainable business, that can support the ecosystem in the long-term.
-Fold's licence is inbetween [source-available](https://en.wikipedia.org/wiki/Source-available_software) and a traditional commercial software licence. It requires a paid licence for any commercial use, after the initial, 30 day trial period. Deployment is only possible with the additional purchase of `fold-extended`, a product currently in development. 
+Fold's licence is inbetween [source-available](https://en.wikipedia.org/wiki/Source-available_software) and a traditional commercial software licence. It requires a paid licence for any commercial use, after the initial, 30 day trial period.
 
-We also want to contribute to open research by giving free access to non-commercial use of `fold`. If you are a researcher and would like to get access to Dream Faster's all of available tools, please <a href='mailto:info@dreamfaster.ai?subject=Research Licence'>contact us here</a>. 
+We also want to contribute to open research by giving free access to non-commercial, research use of `fold`. 
 
 [Read more](https://dream-faster.github.io/fold/product/license/)
 
 ## Limitations
 
 - No intermittent time series support, very limited support for missing values.
 - No hierarchical time series support.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.1.4 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.7 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
 rigour. License: Proprietary Keywords: time-series,machine-
 learning,forecasting,forecast,nowcast,models,time-series-regression,time-
 series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: Other/Proprietary License Classifier: Operating
@@ -86,23 +86,23 @@
 and use `modin` to handle out-of-memory datasets (full support for modin is
 coming in April).** - Bridging the gap between Online and Mini-Batch learning.
 **â Mix and match `xgboost` with ARIMA, in a single pipeline. Boost your
 model's accuracy by updating them on every timestamp, if desired.** - Update
 your deployed models, easily, as new data flows in.
 **â Real world is not static. Let your models adapt, without the need to re-
 train from scratch.**  ## Examples, Walkthroughs and Blog Posts
-Name                                               Type        Dataset   Docs Link   Colab
-                                                               Type
-â¡ï¸ Core Walkthrough                      Walkthrough Energy    Notebook    Colab
-ð Speed Comparison of Fold to other librarieWalkthrough Weather   Notebook    Colab
-ð Example Collection                        Example     Weather & Collection  -
-                                                               Synthetic Link
-ðï¸ Back to the Future with Time Series             Public    Blog_post
-Forecasting                                        Blog        Release   on_Applied  -
-                                                               Blog Post Exploration
+Name                                                                   Type        Dataset   Docs Link   Colab
+                                                                                   Type
+â¡ï¸ Core Walkthrough                                          Walkthrough Energy    Notebook    Colab
+ð Speed Comparison of Fold to other libraries                   Walkthrough Weather   Notebook    Colab
+ð Example Collection                                            Example     Weather & Collection  -
+                                                                                   Synthetic Link
+                                                                                   Public    Blog_post
+ðï¸ Why we ended up building an Adaptive ML engine for Time Bloges      Release   on_Applied  -
+                                                                                   Blog Post Exploration
 
 ## Core Features - Supports both Regression and Classification tasks. - Online
 and Mini-batch learning. - Feature selection and other transformations on an
 expanding/rolling window basis - Use any scikit-learn/tabular model natively! -
 Use any univariate or sequence models (wrappers provided in [fold-wrappers]
 (https://github.com/dream-faster/fold-wrappers)). - Use any Deep Learning Time
 Series models (wrappers provided in [fold-wrappers](https://github.com/dream-
@@ -132,15 +132,12 @@
 Community] for live discussion! Submit an issue or reach out to us on info at
 dream-faster.ai for any inquiries. ## Licence & Usage We want to **bring much-
 needed transparency, speed and rigour** to the process of creating Time Series
 ML pipelines, while also building a sustainable business, that can support the
 ecosystem in the long-term. Fold's licence is inbetween [source-available]
 (https://en.wikipedia.org/wiki/Source-available_software) and a traditional
 commercial software licence. It requires a paid licence for any commercial use,
-after the initial, 30 day trial period. Deployment is only possible with the
-additional purchase of `fold-extended`, a product currently in development. We
-also want to contribute to open research by giving free access to non-
-commercial use of `fold`. If you are a researcher and would like to get access
-to Dream Faster's all of available tools, please contact_us_here. [Read more]
-(https://dream-faster.github.io/fold/product/license/) ## Limitations - No
+after the initial, 30 day trial period. We also want to contribute to open
+research by giving free access to non-commercial, research use of `fold`. [Read
+more](https://dream-faster.github.io/fold/product/license/) ## Limitations - No
 intermittent time series support, very limited support for missing values. - No
 hierarchical time series support.
```

