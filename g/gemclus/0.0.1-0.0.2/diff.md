# Comparing `tmp/gemclus-0.0.1.tar.gz` & `tmp/gemclus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemclus-0.0.1.tar", last modified: Thu Apr 27 15:56:34 2023, max compression
+gzip compressed data, was "gemclus-0.0.2.tar", last modified: Tue May  2 15:55:14 2023, max compression
```

## Comparing `gemclus-0.0.1.tar` & `gemclus-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/
--rw-rw-r--   0 louis     (1000) louis     (1000)      705 2023-04-27 12:43:01.000000 gemclus-0.0.1/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-04-27 12:04:58.000000 gemclus-0.0.1/MANIFEST.in
--rw-rw-r--   0 louis     (1000) louis     (1000)     3324 2023-04-27 15:56:34.710378 gemclus-0.0.1/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     2009 2023-04-27 15:51:44.000000 gemclus-0.0.1/README.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.706378 gemclus-0.0.1/gemclus/
--rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-04-27 14:43:01.000000 gemclus-0.0.1/gemclus/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    17328 2023-04-25 14:35:56.000000 gemclus-0.0.1/gemclus/_base_gemini.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/gemclus/_gemini_grads/
--rw-rw-r--   0 louis     (1000) louis     (1000)      301 2023-03-29 14:26:07.000000 gemclus-0.0.1/gemclus/_gemini_grads/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5658 2023-04-27 10:04:28.000000 gemclus-0.0.1/gemclus/_gemini_grads/_gemini_losses.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2411 2023-03-29 14:26:07.000000 gemclus-0.0.1/gemclus/_gemini_grads/_prox_grad.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/gemclus/data/
--rw-rw-r--   0 louis     (1000) louis     (1000)      113 2023-04-26 14:11:46.000000 gemclus-0.0.1/gemclus/data/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     7935 2023-04-27 08:21:50.000000 gemclus-0.0.1/gemclus/data/synthetic_data.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/gemclus/linear/
--rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-03-29 14:26:07.000000 gemclus-0.0.1/gemclus/linear/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    12600 2023-04-12 08:27:42.000000 gemclus-0.0.1/gemclus/linear/_linear_geminis.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/gemclus/mlp/
--rw-rw-r--   0 louis     (1000) louis     (1000)       89 2023-03-29 14:26:07.000000 gemclus-0.0.1/gemclus/mlp/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    10790 2023-04-12 08:27:42.000000 gemclus-0.0.1/gemclus/mlp/_mlp_geminis.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/gemclus/sparse/
--rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-03-29 14:26:07.000000 gemclus-0.0.1/gemclus/sparse/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    26134 2023-04-12 08:27:42.000000 gemclus-0.0.1/gemclus/sparse/_base_sparse.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5162 2023-04-12 08:27:42.000000 gemclus-0.0.1/gemclus/sparse/_linear_sparse.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5755 2023-04-12 08:27:42.000000 gemclus-0.0.1/gemclus/sparse/_mlp_sparse.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/gemclus/tests/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-03-29 14:26:07.000000 gemclus-0.0.1/gemclus/tests/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2885 2023-04-12 08:27:42.000000 gemclus-0.0.1/gemclus/tests/test_default.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     3974 2023-04-27 08:03:33.000000 gemclus-0.0.1/gemclus/tests/test_objectives.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5131 2023-04-12 08:27:42.000000 gemclus-0.0.1/gemclus/tests/test_path.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-27 15:56:34.710378 gemclus-0.0.1/gemclus.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3324 2023-04-27 15:56:34.000000 gemclus-0.0.1/gemclus.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      824 2023-04-27 15:56:34.000000 gemclus-0.0.1/gemclus.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-04-27 15:56:34.000000 gemclus-0.0.1/gemclus.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-04-27 15:48:30.000000 gemclus-0.0.1/gemclus.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-04-27 15:56:34.000000 gemclus-0.0.1/gemclus.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        8 2023-04-27 15:56:34.000000 gemclus-0.0.1/gemclus.egg-info/top_level.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       97 2023-04-27 14:33:43.000000 gemclus-0.0.1/pyproject.toml
--rw-rw-r--   0 louis     (1000) louis     (1000)       50 2023-04-27 12:13:50.000000 gemclus-0.0.1/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)      147 2023-04-27 15:56:34.710378 gemclus-0.0.1/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     2525 2023-04-27 15:56:32.000000 gemclus-0.0.1/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      705 2023-04-27 12:43:01.000000 gemclus-0.0.2/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-04-27 12:04:58.000000 gemclus-0.0.2/MANIFEST.in
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-02 15:55:14.577494 gemclus-0.0.2/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2010 2023-05-02 09:19:29.000000 gemclus-0.0.2/README.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-05-02 15:25:00.000000 gemclus-0.0.2/gemclus/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    20059 2023-05-02 14:58:53.000000 gemclus-0.0.2/gemclus/_base_gemini.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/_gemini_grads/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      300 2023-05-02 09:32:20.000000 gemclus-0.0.2/gemclus/_gemini_grads/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5568 2023-05-02 09:34:30.000000 gemclus-0.0.2/gemclus/_gemini_grads/_gemini_losses.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2406 2023-04-28 09:20:02.000000 gemclus-0.0.2/gemclus/_gemini_grads/_prox_grad.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/data/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-05-02 08:01:52.000000 gemclus-0.0.2/gemclus/data/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11872 2023-05-02 12:31:44.000000 gemclus-0.0.2/gemclus/data/synthetic_data.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/linear/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/linear/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    13273 2023-05-02 13:51:33.000000 gemclus-0.0.2/gemclus/linear/_linear_geminis.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/mlp/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       89 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/mlp/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11313 2023-05-02 13:51:13.000000 gemclus-0.0.2/gemclus/mlp/_mlp_geminis.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/sparse/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/sparse/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    23850 2023-05-02 15:17:21.000000 gemclus-0.0.2/gemclus/sparse/_base_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5437 2023-05-02 13:46:20.000000 gemclus-0.0.2/gemclus/sparse/_linear_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5989 2023-05-02 13:50:26.000000 gemclus-0.0.2/gemclus/sparse/_mlp_sparse.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/tests/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/tests/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2808 2023-05-02 09:19:28.000000 gemclus-0.0.2/gemclus/tests/test_data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3331 2023-05-02 13:57:17.000000 gemclus-0.0.2/gemclus/tests/test_default.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3935 2023-05-02 09:19:29.000000 gemclus-0.0.2/gemclus/tests/test_objectives.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5548 2023-05-02 14:10:19.000000 gemclus-0.0.2/gemclus/tests/test_path.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      851 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        8 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/top_level.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       97 2023-04-27 14:33:43.000000 gemclus-0.0.2/pyproject.toml
+-rw-rw-r--   0 louis     (1000) louis     (1000)       50 2023-05-02 15:54:07.000000 gemclus-0.0.2/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)      147 2023-05-02 15:55:14.577494 gemclus-0.0.2/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2525 2023-04-27 15:56:32.000000 gemclus-0.0.2/setup.py
```

### Comparing `gemclus-0.0.1/LICENSE` & `gemclus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemclus-0.0.1/PKG-INFO` & `gemclus-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemclus
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for performing discriminative clustering with gemini-trained models
 Home-page: https://github.com/gemini-clustering
 Download-URL: https://github.com/gemini-clustering
 Maintainer: Louis Ohl
 Maintainer-email: louis.ohl@inria.fr
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
@@ -28,28 +28,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # GEMCLUS - A package for discriminative clustering using GEMINI
 
-The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual information (GEMINI).
+The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual
+information (GEMINI).
 The package was written to be a scikit-learn compatible extension.
 
 You can find the complete documentation of the package here: `Link to be announced`
 
 ## Installation
 
 Use the following instruction for installing the package:
 
 ```commandline
 pip install gemclus
 ```
 
 The library requires a couple scientific package to run:
+
 + NumPy
 + Scipy
 + POT
 + Scikit-learn
 
 ## Reference
```

### Comparing `gemclus-0.0.1/README.md` & `gemclus-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # GEMCLUS - A package for discriminative clustering using GEMINI
 
-The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual information (GEMINI).
+The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual
+information (GEMINI).
 The package was written to be a scikit-learn compatible extension.
 
 You can find the complete documentation of the package here: `Link to be announced`
 
 ## Installation
 
 Use the following instruction for installing the package:
 
 ```commandline
 pip install gemclus
 ```
 
 The library requires a couple scientific package to run:
+
 + NumPy
 + Scipy
 + POT
 + Scikit-learn
 
 ## Reference
```

### Comparing `gemclus-0.0.1/gemclus/_base_gemini.py` & `gemclus-0.0.2/gemclus/_base_gemini.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from abc import ABC, abstractmethod
 from numbers import Integral, Real
 
 import numpy as np
 from sklearn.base import ClusterMixin, BaseEstimator
-from sklearn.metrics.pairwise import KERNEL_PARAMS, PAIRED_DISTANCES, pairwise_kernels, pairwise_distances
+from sklearn.metrics.pairwise import PAIRWISE_KERNEL_FUNCTIONS, PAIRED_DISTANCES, pairwise_kernels, pairwise_distances
 from sklearn.neural_network._stochastic_optimizers import AdamOptimizer, SGDOptimizer
 from sklearn.utils import check_array, check_random_state
 from sklearn.utils._param_validation import Interval, StrOptions
 from sklearn.utils.validation import check_is_fitted
 
 from gemclus._gemini_grads import mmd_ovo, mmd_ova, wasserstein_ovo, wasserstein_ova
 
@@ -34,14 +34,17 @@
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -55,24 +58,26 @@
         The number of iterations that the model took for converging.
     """
     _parameter_constraints: dict = {
         "n_clusters": [Interval(Integral, 1, None, closed="left")],
         "max_iter": [Interval(Integral, 1, None, closed="left")],
         "learning_rate": [Interval(Real, 0, None, closed="neither")],
         "solver": [StrOptions({"sgd", "adam"})],
+        "batch_size": [Interval(Integral, 1, None, closed="left"), None],
         "verbose": [bool],
         "random_state": [Interval(Integral, 0, None, closed="left"), None]
     }
 
-    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, solver="adam",
+    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, solver="adam", batch_size=None,
                  verbose=False, random_state=None):
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.learning_rate = learning_rate
         self.solver = solver
+        self.batch_size = batch_size
         self.verbose = verbose
         self.random_state = random_state
 
     @abstractmethod
     def _init_params(self, random_state):
         """
         Initialise the set of parameters :math:`\theta` parameters of the model that are used to compute
@@ -165,49 +170,61 @@
         -------
         y_pred:  ndarray of shape (n_samples, n_clusters)
             The prediction :math:`p_\theta(y|x)` probabilities of the model.
         """
         pass
 
     @abstractmethod
-    def _compute_affinity(self, X):
+    def _compute_affinity(self, X, y=None):
         """
         Compute the affinity (kernel function or distance function_ between all samples of X.
 
         Parameters
         ----------
         X: ndarray of shape (n_samples, n_features)
             The samples between which all affinities must be compute
 
+        y: ndarray of shape (n_samples, n_samples), default=None
+            Values of the affinity between samples in case of a "precomputed" affinity. Ignored if None and the affinity
+            is not precomputed.
+
         Return
         ------
         K: ndarray of shape (n_samples, n_samples)
             The symmetric affinity matrix
         """
         pass
 
     def fit(self, X, y=None):
         """Compute GEMINI clustering.
+
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Training instances to cluster.
-        y : Ignored
-            Not used, present here for API consistency by convention.
+        y : ndarray of shape (n_samples, n_samples), default=None
+            Use this parameter to give a precomputed affinity metric if the option "precomputed" was passed during
+            construction. Otherwise, it is not used and present here for API consistency by convention.
+
         Returns
         -------
         self : object
             Fitted estimator.
         """
         self._validate_params()
 
         # Check that X has the correct shape
         X = check_array(X)
         X = self._validate_data(X, accept_sparse=True, dtype=np.float64, ensure_min_samples=self.n_clusters)
 
+        if self.batch_size is None:
+            batch_size = len(X)
+        else:
+            batch_size = self.batch_size
+
         # Fix the random seed
         random_state = check_random_state(self.random_state)
 
         # Initialise the weights
         if self.verbose:
             print("Initialising parameters")
         self._init_params(random_state)
@@ -217,61 +234,79 @@
             self.optimiser_ = SGDOptimizer(weights, self.learning_rate)
         else:
             self.optimiser_ = AdamOptimizer(weights, self.learning_rate)
 
         if self.verbose:
             print(f"Computing affinity")
 
-        affinity = self._compute_affinity(X)
+        affinity = self._compute_affinity(X, y)
 
         if self.verbose:
             print(f"Starting training over {self.max_iter} iterations.")
         # Now, iterate for gradient descent
         for i in range(self.max_iter):
-            y_pred = self._infer(X)
-            _, grads = self._compute_gemini(y_pred, affinity, return_grad=True)
-            grads = self._compute_grads(X, y_pred, grads)
-            self._update_weights(weights, grads)
+            # Create batches
+            j = 0
+            all_indices = random_state.permutation(len(X))
+            while j < len(X):
+                batch_indices = all_indices[j:j + batch_size]
+                X_batch = X[batch_indices]
+                if affinity is None:
+                    affinity_batch = None  # Specific case of f-div GEMINI
+                else:
+                    affinity_batch = affinity[batch_indices][:, batch_indices]
+
+                y_pred = self._infer(X_batch)
+                _, grads = self._compute_gemini(y_pred, affinity_batch, return_grad=True)
+                grads = self._compute_grads(X_batch, y_pred, grads)
+                self._update_weights(weights, grads)
+
+                j += batch_size
 
         if self.verbose:
             print("Finished")
 
         # Return the classifier
 
         # Must save the labels
         self.labels_ = self._infer(X).argmax(1)
         self.n_iter_ = self.max_iter
 
         return self
 
     def fit_predict(self, X, y=None):
         """Compute GEMINI clustering and returns the predicted clusters.
+
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Training instances to cluster.
-        y : Ignored
-            Not used, present here for API consistency by convention.
+        y : ndarray of shape (n_samples, n_samples), default=None
+            Use this parameter to give a precomputed affinity metric if the option "precomputed" was passed during
+            construction. Otherwise, it is not used and present here for API consistency by convention.
+
         Returns
         -------
         y_pred : ndarray of shape (n_samples,)
             Vector containing the cluster label for each sample.
         """
-        return super().fit_predict(X, y)
+        return self.fit(X, y).labels_
 
     def predict_proba(self, X):
         """
         Probability estimates that are the output of the neural network p(y|x).
         The returned estimates for all classes are ordered by the
         label of classes.
+
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Vector to be scored, where `n_samples` is the number of samples and
             `n_features` is the number of features.
+
         Returns
         -------
         T : array-like of shape (n_samples, n_clusters)
             Returns the probability of the sample for each cluster in the model.
         """
         # Check is fit had been called
         check_is_fitted(self)
@@ -309,23 +344,24 @@
         """
         Return the value of the GEMINI evaluated on the given test data.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Test samples.
-        y : Ignored
-            Not used, present here for API consistency by convention.
+        y : ndarray of shape (n_samples, n_samples), default=None
+            Use this parameter to give a precomputed affinity metric if the option "precomputed" was passed during
+            construction. Otherwise, it is not used and present here for API consistency by convention.
 
         Returns
         -------
         score : float
             GEMINI evaluated on the output of ``self.predict(X)``.
         """
-        K = self._compute_affinity(X)
+        K = self._compute_affinity(X, y)
         y_pred = self.predict_proba(X)
         return self._compute_gemini(y_pred, K).item()
 
 
 class _BaseMMD(_BaseGEMINI, ABC):
     """
     Adds the MMD GEMINI to the base model.
@@ -351,14 +387,17 @@
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -369,32 +408,38 @@
     labels_: ndarray of shape (n_samples)
         The labels that were assigned to the samples passed to the :meth:`fit` method.
     n_iter_: int
         The number of iterations that the model took for converging.
     """
     _parameter_constraints: dict = {
         **_BaseGEMINI._parameter_constraints,
-        "kernel": [StrOptions(set(KERNEL_PARAMS))],
+        "kernel": [StrOptions(set(list(PAIRWISE_KERNEL_FUNCTIONS) + ["precomputed"])), callable],
         "ovo": [bool]
     }
 
-    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, kernel="linear", solver="adam", ovo=False,
-                 verbose=False, random_state=None):
+    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, kernel="linear", batch_size=None,
+                 solver="adam", ovo=False, verbose=False, random_state=None):
         super().__init__(
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.kernel = kernel
         self.ovo = ovo
 
-    def _compute_affinity(self, X):
+    def _compute_affinity(self, X, y=None):
+        if callable(self.kernel):
+            return self.kernel(X)
+        elif self.kernel == "precomputed":
+            assert y is not None, f"Kernel should be precomputed, yet no kernel was passed as parameters: y={y}"
+            return y
         return pairwise_kernels(X, metric=self.kernel)
 
     def _compute_gemini(self, y_pred, K, return_grad=False):
         if self.ovo:
             return mmd_ovo(y_pred, K, return_grad)
         else:
             return mmd_ova(y_pred, K, return_grad)
@@ -413,26 +458,29 @@
         Maximum number of epochs to perform gradient descent in a single run.
 
     learning_rate: float, default=1e-3
         Initial learning rate used. It controls the step-size in updating the weights.
 
     metric: {'cosine', 'euclidean', 'l2','l1','manhattan','cityblock'},
         default='euclidean'
-        The metric to use in combination with the Wasserstein objective. It corresponds to one value of `PAIRED_DISTANCES`.
-        Currently, all metric parameters are the default ones.
+        The metric to use in combination with the Wasserstein objective. It corresponds to one value of
+        `PAIRED_DISTANCES`. Currently, all metric parameters are the default ones.
 
     ovo: bool, default=False
         Whether to run the model using the Wasserstein OvA (False) or the Wasserstein OvO (True).
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -443,32 +491,38 @@
     labels_: ndarray of shape (n_samples)
         The labels that were assigned to the samples passed to the :meth:`fit` method.
     n_iter_: int
         The number of iterations that the model took for converging.
     """
     _parameter_constraints: dict = {
         **_BaseGEMINI._parameter_constraints,
-        "metric": [StrOptions(set(PAIRED_DISTANCES))],
+        "metric": [StrOptions(set(list(PAIRED_DISTANCES) + ["precomputed"]))],
         "ovo": [bool]
     }
 
-    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, metric="euclidean", ovo=False,
-                 solver="adam", verbose=False, random_state=None):
+    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, solver="adam", batch_size=None,
+                 metric="euclidean", ovo=False, verbose=False, random_state=None):
         super().__init__(
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.metric = metric
         self.ovo = ovo
 
-    def _compute_affinity(self, X):
+    def _compute_affinity(self, X, y=None):
+        if callable(self.metric):
+            return self.metric(X)
+        elif self.metric == "precomputed":
+            assert y is not None, f"Kernel should be precomputed, yet no kernel was passed as parameters: y={y}"
+            return y
         return pairwise_distances(X, metric=self.metric)
 
     def _compute_gemini(self, y_pred, K, return_grad=False):
         if self.ovo:
             return wasserstein_ovo(y_pred, K, return_grad)
         else:
             return wasserstein_ova(y_pred, K, return_grad)
```

### Comparing `gemclus-0.0.1/gemclus/_gemini_grads/_gemini_losses.py` & `gemclus-0.0.2/gemclus/_gemini_grads/_gemini_losses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from numpy.typing import NDArray
 import ot
 from sklearn.utils._param_validation import validate_params
 
 
 @validate_params(
     {
         "y_pred": ["array-like"],
@@ -41,14 +40,15 @@
         delta_mask = (delta == 0)
         gradient = tau_grad / (delta + delta_mask).reshape((1, -1))
         gradient[:, delta_mask] = 0
         return mmd_ova_value, gradient * clip_mask
     else:
         return mmd_ova_value
 
+
 @validate_params(
     {
         "y_pred": ["array-like"],
         "K": ["array-like"],
         "return_grad": [bool]
     }
 )
@@ -90,27 +90,25 @@
         gradient += pi @ delta / N
         gradient *= 2
 
         return mmd_ovo_value, gradient * clip_mask
     else:
         return mmd_ovo_value
 
+
 @validate_params(
     {
         "y_pred": ["array-like"],
         "D": ["array-like"],
         "return_grad": [bool]
     }
 )
 def wasserstein_ova(y_pred, D, return_grad=False):
     N, K = y_pred.shape
 
-    if return_grad:
-        grads = np.zeros(y_pred.shape)
-
     # To stabilise the computations and in order to avoid the
     # softmax overconfident values which would lead to division by 0
     # we, clamp the predictions
     epsilon = 1e-12
     clip_mask = (y_pred > epsilon) & (y_pred < 1 - epsilon)
     y_pred = np.clip(y_pred, a_min=epsilon, a_max=1 - epsilon)
 
@@ -131,14 +129,15 @@
         u_bar = np.vstack([x["u"] - x["u"].mean() for x in dual_variables]).T
         grads = u_bar / N + wasserstein_distances / N
         grads -= (y_pred * u_bar).sum(0) / (N * N * pi)
         return wasserstein_ova_value, grads * clip_mask
     else:
         return wasserstein_ova_value
 
+
 @validate_params(
     {
         "y_pred": ["array-like"],
         "D": ["array-like"],
         "return_grad": [bool]
     }
 )
```

### Comparing `gemclus-0.0.1/gemclus/_gemini_grads/_prox_grad.py` & `gemclus-0.0.2/gemclus/_gemini_grads/_prox_grad.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,15 @@
 
 def linear_prox_grad(W, alpha):
     # Shape of W is [d,h]
     # alpha is a scalar
     W_norms = np.linalg.norm(W, axis=1, keepdims=True)  # Shape [d,1]
 
     # Group lasso soft thresholding
-    W_normalised = W / W_norms
-    W_star = np.maximum(W_norms - alpha, 0) * W_normalised
+    W_star = np.maximum(W_norms - alpha, 0) * W / np.where(W_norms == 0, 1, W_norms)
 
     return W_star
 
 
 def group_linear_prox_grad(groups, W, alpha):
     W_star = np.empty(W.shape)
```

### Comparing `gemclus-0.0.1/gemclus/data/synthetic_data.py` & `gemclus-0.0.2/gemclus/data/synthetic_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,202 @@
 from numbers import Integral, Real
+from typing import Tuple
 
 import numpy as np
 from scipy.linalg import block_diag
-from typing import Tuple
-
-from sklearn.utils import check_random_state
+from sklearn.utils import check_random_state, check_array
 from sklearn.utils._param_validation import validate_params, Interval, Iterable
 
 
 @validate_params(
     {
         "n": [Interval(Integral, 1, None, closed="left")],
-        "mus": ["array-like"],
-        "sigmas": ["array-like"],
-        "pis": ["array-like", Iterable[float]],
+        "loc": ["array-like"],
+        "scale": ["array-like"],
+        "pvals": ["array-like", Iterable[float]],
         "random_state": ["random_state"]
     }
 )
-def draw_gmm(n, mus, sigmas, pis, random_state=None) -> Tuple[np.ndarray, np.ndarray]:
+def draw_gmm(n, loc, scale, pvals, random_state=None) -> Tuple[np.ndarray, np.ndarray]:
     """
     Returns :math:`n` samples drawn from a mixture of Gaussian distributions. The number of components
     is determined by the number of elements in the lists of the parameters.
 
     Parameters
     ----------
     n: int
         The number of samples to draw from the GMM.
-    mus: list of 1d ndarray
+    loc: list of 1d ndarray
         A list containing the means of all components of the Gaussian mixture distributions.
-    sigmas: list of 2d ndarray
+    scale: list of 2d ndarray
         A list containing the covariances of all components of the Gaussian mixture distribution.
-    pis: 1d ndarray
+    pvals: 1d ndarray
         The proportions of each component of the Gaussian mixture.
     random_state: int, RandomState instance or None, default=None
         Determines random number generation for dataset creation. Pass an int for reproducible output across
         multiple runs.
 
     Returns
     -------
     X: ndarray
         The array containing the samples drawn from the mixture model.
     y: ndarray
         The component from which each sample originates.
     """
+    loc = check_array(loc, ensure_2d=True, ensure_min_samples=2, input_name="Means")
+    scale = check_array(scale, allow_nd=True, ensure_min_samples=2, input_name="Covariances")
+    pvals = check_array(pvals, ensure_2d=False, ensure_min_samples=2, input_name="Proportions")
 
     # Check that the parameters have satisfying properties
-    assert len(mus) == len(sigmas), "The means and the covariances do not contain the same number of components"
-    assert len(pis) == len(sigmas), "The proportions and the covariances do not contain the same number of components"
-    assert len(pis) > 1, "The gmm requires at least two components."
-    main_dim = len(mus[0])
-    for k in range(len(pis)):
-        assert len(mus[k]) == len(sigmas[k]), f"Inconsistent shape between of {k}-th means and covariances"
-        assert len(mus[k]) == main_dim, f"Inconsistent dimensions between all components. Should be {main_dim} or" \
-                                        f" {len(mus[k])} everywhere."
-        assert pis[k] > 0, f"Proportions or components should be positive."
-        # Other checks regarding psd for covariances are included in the multivariate_normal function
-
-    assert sum(pis) == 1, "Proportions of components do not add up to one."
+    K, d = loc.shape
+    assert K == scale.shape[0], "The means and the covariances do not contain the same number of components"
+    assert d == scale.shape[1] and d == scale.shape[1], "The covariances should be square matrices"
+    assert K == pvals.shape[0], "The proportions and the means do not contain the same number of components"
+    assert np.all(pvals > 0), "Proportions or components should be positive."
+    assert np.sum(pvals) == 1, "Proportions of components do not add up to one."
 
     generator = check_random_state(random_state)
 
     # Draw samples from each distribution
 
     X = []
-    if main_dim == 1:
-        X += [generator.normal(mus[k], sigmas[k], size=(n,))]
-    else:
-        for k in range(len(mus)):
-            X += [generator.multivariate_normal(mus[k], sigmas[k], size=(n,))]
 
     # Draw the true cluster from which to draw
-    y = np.random.choice(len(mus), p=pis, size=(n,))
+    y = generator.choice(K, p=pvals, size=(n,))
+    if d == 1:
+        for k in range(len(loc)):
+            X += [generator.normal(loc[k], scale[k], size=(n,))]
+    else:
+        for k in range(len(loc)):
+            X += [generator.multivariate_normal(loc[k], scale[k], size=(n,))]
 
     X = [X[k][i].reshape((1, -1)) for i, k in enumerate(y)]
 
     return np.concatenate(X, axis=0), y
 
 
 @validate_params(
     {
         "n": [Interval(Integral, 1, None, closed="left")],
+        "loc": ["array-like"],
+        "scale": ["array-like"],
+        "df": [Interval(Real, 0, None, closed="neither")],
+        "random_state": ["random_state"]
+    }
+)
+def multivariate_student_t(n, loc, scale, df=10, random_state=None) -> np.ndarray:
+    """
+    Draws :math:`n` samples from a multivariate Student-t distribution.
+
+    Parameters
+    ----------
+    n: int
+        The number of samples to draw from the distribution.
+
+    loc: ndarray of shape (d,)
+        The position of the distribution to sample from.
+
+    scale: ndarray of shape (d,d)
+        Positive semi-definite scale matrix.
+
+    df: int, default=10
+        Degrees of freedom of the distribution. Controls the spread of the samples.
+
+    random_state: int, RandomState instance or None, default=None
+        Determines random number generation for dataset creation. Pass an int for reproducible output across
+        multiple runs.
+
+    Returns
+    -------
+    X: ndarray of shape (n,d)
+        The samples drawn from the Student-t distribution.
+    """
+    loc = check_array(loc, ensure_2d=False, input_name="Location")
+    scale = check_array(scale, ensure_2d=True, input_name="Scale")
+
+    d = len(loc)
+    assert scale.shape[0] == d and scale.shape[1] == d, "Please provide a mean and scale with consistent shapes"
+
+    generator = check_random_state(random_state)
+
+    # Start the sampling process by generating from a 0-mean multivariate distribution
+    nx = generator.multivariate_normal(np.zeros(d), scale, size=n)
+    u = generator.chisquare(df, n).reshape((-1, 1))
+    X = np.sqrt(df / u) * nx + loc.reshape((1, -1))
+
+    return X
+
+
+@validate_params(
+    {
+        "n": [Interval(Integral, 4, None, closed="left")],
+        "alpha": [Interval(Real, 0, None, closed="neither")],
+        "df": [Interval(Real, 0, None, closed="neither")],
+        "random_state": ["random_state"]
+    }
+)
+def gstm(n=500, alpha=2, df=1, random_state=None):
+    """
+    Reproduces the Gaussian-Student Mixture dataset from the GEMINI article.
+
+    Parameters
+    ----------
+    n: int, default=500
+        The number of samples to draw from the dataset.
+
+    alpha: float, default=2:
+        This parameter controls how close the means of the Gaussian distribution and the location of the Student-t
+        distribution are.
+
+    df: float, default=1
+        The degrees of freedom for the Student-t distribution.
+
+    random_state: int, RandomState instance or None, default=None
+        Determines random number generation for dataset creation. Pass an int for reproducible output across
+        multiple runs.
+
+    Returns
+    -------
+    X: ndarray
+        The samples of the dataset in an array of shape n_samples x n_features
+    y: ndarray
+        The component of the GMM from which each sample was drawn.
+
+    References
+    -----------
+    GEMINI - Ohl, L., Mattei, P. A., Bouveyron, C., Harchaoui, W., Leclercq, M., Droit, A., & Precioso, F.
+        (2022, October). Generalised Mutual Information for Discriminative Clustering. In Advances in Neural
+        Information Processing Systems.
+    """
+    generator = check_random_state(random_state)
+
+    # Build the location and scale of each distribution
+    locations = np.array([[1, 1], [1, -1], [-1, 1], [-1, -1]]) * alpha
+    covariance = np.eye(2)
+
+    # For the 3 Gaussian distribution, we draw the samples using a GMM with proportions 1/3 on 3/4 of the samples
+    n_gaussian = 3 * n // 4
+    X_gaussian, y_gaussian = draw_gmm(n_gaussian, locations[:-1], [covariance] * 3, np.ones(3) / 3, generator)
+
+    # Then we sample the student-t distribution
+    n_student = n - n_gaussian
+    X_student = multivariate_student_t(n_student, locations[-1], covariance, df, generator)
+
+    X = np.vstack([X_gaussian, X_student])
+    y = np.concatenate([y_gaussian, np.ones(n_student) * 3])
+
+    # Apply one final random permutation to shuffle the data
+    order = generator.permutation(n)
+
+    return X[order], y[order]
+
+
+@validate_params(
+    {
+        "n": [Interval(Integral, 1, None, closed="left")],
         "p": [Interval(Integral, 1, None, closed="left")],
         "mu": [Interval(Real, 0, None, closed="neither")],
         "random_state": ["random_state"]
     }
 )
 def celeux_one(n=300, p=20, mu=1.7, random_state=None) -> Tuple[np.ndarray, np.ndarray]:
     """
```

### Comparing `gemclus-0.0.1/gemclus/linear/_linear_geminis.py` & `gemclus-0.0.2/gemclus/linear/_linear_geminis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from abc import ABC
 from numbers import Real
 
 import numpy as np
 from sklearn.neural_network._stochastic_optimizers import AdamOptimizer, SGDOptimizer
 from sklearn.utils._param_validation import Interval
+from sklearn.utils.extmath import softmax
 
 from .._base_gemini import _BaseGEMINI, _BaseMMD, _BaseWasserstein
-from sklearn.utils.extmath import softmax
 
 
 class _LinearGEMINI(_BaseGEMINI, ABC):
     _parameter_constraints: dict = {
         **_BaseGEMINI._parameter_constraints,
     }
 
-    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, solver="adam",
+    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, solver="adam", batch_size=None,
                  verbose=False, random_state=None):
         super().__init__(
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
 
     def _init_params(self, random_state):
         in_threshold = np.sqrt(1 / self.n_features_in_)
         self.W_ = random_state.uniform(-in_threshold, in_threshold, size=(self.n_features_in_, self.n_clusters))
@@ -74,14 +75,17 @@
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -123,22 +127,23 @@
     """
     _parameter_constraints: dict = {
         **_BaseMMD._parameter_constraints,
         **_LinearGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, kernel="linear", solver="adam", ovo=False,
-                 verbose=False, random_state=None):
+                 batch_size=None, verbose=False, random_state=None):
         _BaseMMD.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             ovo=ovo,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
             kernel=kernel
         )
 
 
 class LinearWasserstein(_LinearGEMINI, _BaseWasserstein):
@@ -154,23 +159,26 @@
         Maximum number of epochs to perform gradient descent in a single run.
 
     learning_rate: float, default=1e-3
         Initial learning rate used. It controls the step-size in updating the weights.
 
     metric: {'cosine', 'euclidean', 'l2','l1','manhattan','cityblock'},
         default='euclidean'
-        The metric to use in combination with the Wasserstein objective. It corresponds to one value of `PAIRED_DISTANCES`.
-        Currently, all metric parameters are the default ones.
+        The metric to use in combination with the Wasserstein objective. It corresponds to one value of
+        `PAIRED_DISTANCES`. Currently, all metric parameters are the default ones.
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -212,32 +220,33 @@
     """
     _parameter_constraints: dict = {
         **_BaseWasserstein._parameter_constraints,
         **_LinearGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, metric="euclidean", ovo=False,
-                 solver="adam", verbose=False, random_state=None):
+                 solver="adam", batch_size=None, verbose=False, random_state=None):
         _BaseWasserstein.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
             ovo=ovo,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
             metric=metric
         )
 
 
 class RIM(_LinearGEMINI):
     """ Implementation of the maximisation of the classical mutual information using a logistic regression with an
-    :math:`\ell_2` penalty on the weights. This implementation follows the framework described by Krause et al. in the RIM
-    paper.
+    :math:`\ell_2` penalty on the weights. This implementation follows the framework described by Krause et al. in the
+    RIM paper.
 
     Parameters
     ----------
     n_clusters : int, default=3
         The maximum number of clusters to form as well as the number of output neurons in the neural network.
 
     max_iter: int, default=1000
@@ -251,14 +260,17 @@
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -300,48 +312,49 @@
 
     _parameter_constraints: dict = {
         **_LinearGEMINI._parameter_constraints,
         "reg": [Interval(Real, 0, None, closed="left")]
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, reg=1,
-                 solver="adam", verbose=False, random_state=None):
+                 solver="adam", batch_size=None, verbose=False, random_state=None):
         _LinearGEMINI.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
-       )
+        )
         self.reg = reg
 
-    def _compute_affinity(self, X):
+    def _compute_affinity(self, X, y=None):
         return None
 
     def _compute_gemini(self, y_pred, K, return_grad=False):
         # Start by computing mutual information
-        p_y_x = np.clip(y_pred, 1e-12, 1-1e-12)
+        p_y_x = np.clip(y_pred, 1e-12, 1 - 1e-12)
         p_y = p_y_x.mean(0)
 
         log_p_y_x = np.log(p_y_x)
         log_p_y = np.log(p_y)
 
-        cluster_entropy = np.sum(p_y*log_p_y)
-        prediction_entropy = np.sum(np.mean(p_y_x*log_p_y_x, axis=0))
+        cluster_entropy = np.sum(p_y * log_p_y)
+        prediction_entropy = np.sum(np.mean(p_y_x * log_p_y_x, axis=0))
 
-        mutual_information = prediction_entropy-cluster_entropy
+        mutual_information = prediction_entropy - cluster_entropy
 
         if return_grad:
-            gradient_mi = -log_p_y_x/log_p_y_x.shape[0] + log_p_y
+            gradient_mi = -log_p_y_x / log_p_y_x.shape[0] + log_p_y
             return mutual_information, -gradient_mi
         else:
             return mutual_information
 
     def compute_penalty(self):
-        return self.reg * np.sum(self.W_*self.W_)
+        return self.reg * np.sum(self.W_ * self.W_)
 
     def _update_weights(self, weights, gradients):
         # Add the regularisation gradient on the weight matrix
         gradients[0] += self.reg * 2 * self.W_
         self.optimiser_.update_params(weights, gradients)
```

### Comparing `gemclus-0.0.1/gemclus/mlp/_mlp_geminis.py` & `gemclus-0.0.2/gemclus/mlp/_mlp_geminis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from abc import ABC
 from numbers import Integral
 
 import numpy as np
 from sklearn.neural_network._stochastic_optimizers import AdamOptimizer, SGDOptimizer
 from sklearn.utils._param_validation import Interval
+from sklearn.utils.extmath import softmax
 
 from .._base_gemini import _BaseGEMINI, _BaseMMD, _BaseWasserstein
-from sklearn.utils.extmath import softmax
 
 
 class _MLPGEMINI(_BaseGEMINI, ABC):
     _parameter_constraints: dict = {
         **_BaseGEMINI._parameter_constraints,
         "hidden_dim": [Interval(Integral, 1, None, closed="left")],
     }
 
-    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, solver="adam", n_hidden_dim=20,
+    def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, solver="adam", n_hidden_dim=20, batch_size=None,
                  verbose=False, random_state=None):
         super().__init__(
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.n_hidden_dim = n_hidden_dim
 
     def _init_params(self, random_state):
         in_threshold = np.sqrt(1 / self.n_features_in_)
@@ -89,14 +90,17 @@
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -144,32 +148,34 @@
     """
     _parameter_constraints: dict = {
         **_BaseMMD._parameter_constraints,
         **_MLPGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, kernel="linear", ovo=False,
-                 solver="adam", verbose=False, random_state=None):
+                 solver="adam", batch_size=None, verbose=False, random_state=None):
         _MLPGEMINI.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             n_hidden_dim=n_hidden_dim,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         _BaseMMD.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
             ovo=ovo,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
             kernel=kernel
         )
 
 
 class MLPWasserstein(_MLPGEMINI, _BaseWasserstein):
@@ -188,26 +194,29 @@
         Initial learning rate used. It controls the step-size in updating the weights.
 
     n_hidden_dim: int, default=20
         The number of neurons in the hidden layer of the neural network.
 
     metric: {'cosine', 'euclidean', 'l2','l1','manhattan','cityblock'},
         default='euclidean'
-        The metric to use in combination with the Wasserstein objective. It corresponds to one value of `PAIRED_DISTANCES`.
-        Currently, all metric parameters are the default ones.
+        The metric to use in combination with the Wasserstein objective. It corresponds to one value of
+        `PAIRED_DISTANCES`.  Currently, all metric parameters are the default ones.
 
     ovo: bool, default=False
         Whether to run the model using the MMD OvA (False) or the MMD OvO (True).
 
     solver: {'sgd','adam'}, default='adam'
         The solver for weight optimisation.
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -255,29 +264,31 @@
     """
     _parameter_constraints: dict = {
         **_BaseWasserstein._parameter_constraints,
         **_MLPGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, metric="euclidean", ovo=False,
-                 solver="adam", verbose=False, random_state=None):
+                 solver="adam", batch_size=None, verbose=False, random_state=None):
         _MLPGEMINI.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             n_hidden_dim=n_hidden_dim,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         _BaseWasserstein.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
             ovo=ovo,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
             metric=metric
         )
```

### Comparing `gemclus-0.0.1/gemclus/sparse/_base_sparse.py` & `gemclus-0.0.2/gemclus/sparse/_base_sparse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 from abc import ABC
 from numbers import Real
 
 import numpy as np
 from sklearn.neural_network._stochastic_optimizers import SGDOptimizer
+from sklearn.utils import check_random_state
 from sklearn.utils._param_validation import Interval
 from sklearn.utils.extmath import softmax
 
 from .._gemini_grads import linear_prox_grad, group_mlp_prox_grad, group_linear_prox_grad, mlp_prox_grad
 from ..linear._linear_geminis import _LinearGEMINI
 from ..mlp._mlp_geminis import _MLPGEMINI
 
@@ -16,14 +17,140 @@
     if groups is not None:
         all_indices = []
         for g in groups:
             all_indices.extend(list(g))
         assert len(all_indices) == n_features_in and set(all_indices) == set(range(n_features_in)), \
             f"Groups must form a partition of the set of variable indices"
 
+def compute_val_score(clf,X, batch_size):
+    validation_gemini = 0  # clf.score(X)
+    validation_l1 = clf._group_lasso_penalty() * clf.alpha
+    j = 0
+    while j < len(X):
+        X_batch = X[j:j + batch_size]
+        validation_gemini += clf.score(X_batch) * len(X_batch)
+        j += batch_size
+    validation_gemini /= len(X)
+    return validation_gemini, validation_l1
+
+def _path(clf, X, alpha_multiplier=1.05, min_features=2, keep_threshold=0.9,
+          early_stopping_factor=0.99, max_patience=10):
+    clf._validate_data(X)
+    check_groups(clf.groups, X.shape[1])
+    if alpha_multiplier <= 1:
+        warnings.warn(f"The alpha multiplier is lower or equal to 1. This will not increase alpha during the path. "
+                      f"Setting it again to default parameters: 1.05")
+        alpha_multiplier = 1.05
+    if keep_threshold < 0 or keep_threshold > 1:
+        warnings.warn(f"The threshold to keep the best solution is outside [0,1]: {keep_threshold}, setting it "
+                      f"to default: 0.9")
+        keep_threshold = 0.9
+    if min_features <= 0:
+        warnings.warn(f"The min_features to stop the path iterations is below 0 which implies infinite loop. "
+                      f"Setting it to default: 2")
+        min_features = 2
+    elif min_features >= X.shape[1]:
+        warnings.warn(f"The min_features param is greater or equal to the number of features. This implies that "
+                      f"no path will be performed. The method is equivalent to `fit`.")
+
+    # Start by fitting the model using all features and without regularisation
+    alpha = clf.alpha
+    clf.set_params(alpha=0)
+
+    if clf.verbose:
+        print("Starting initial training with alpha = 0")
+    clf.fit(X)
+    best_gemini = clf.score(X)
+    weights = clf._get_weights()
+    best_weights = [w.copy() for w in weights]
+
+    if clf.verbose:
+        print(f"Finished initial training. GEMINI = {best_gemini}")
+
+    kernel = clf._compute_affinity(X)
+
+    generator = check_random_state(clf.random_state)
+    if clf.batch_size is not None:
+        batch_size = clf.batch_size
+    else:
+        batch_size = len(X)
+
+    alphas = [0]
+    n_features = [X.shape[1]]
+    geminis = [best_gemini]
+    group_lasso_penalties = [clf._group_lasso_penalty()]
+
+    # Re-initialise the optimiser to SGD with 0.9 momentum (default option)
+    clf.optimiser_ = SGDOptimizer(weights, clf.learning_rate)
+
+    while clf._n_selected_features() > min_features:
+        clf.alpha = alpha
+
+        # Compute the validation scores at the beginning of this step of the path
+        validation_gemini, validation_l1 = compute_val_score(clf, X, batch_size)
+
+        if clf.verbose:
+            print(f"Starting new iteration with: alpha = {clf.alpha}. Validation score is {validation_gemini}")
+
+        gemini_score = np.array([validation_gemini])
+        patience = 0
+        i = 0
+        while i < clf.max_iter and patience < max_patience:
+            all_indices = generator.permutation(len(X))
+            j = 0
+            while j < len(X):
+                batch_indices = all_indices[j:j + batch_size]
+                X_batch = X[batch_indices]
+                kernel_batch = kernel[batch_indices][:, batch_indices]
+                y_pred = clf._infer(X_batch)
+                gemini_score, grads = clf._compute_gemini(y_pred, kernel_batch, return_grad=True)
+                grads = clf._compute_grads(X_batch, y_pred, grads)
+                clf._update_weights(weights, grads)
+
+                j += batch_size
+
+            iteration_gemini, iteration_l1 = compute_val_score(clf, X, batch_size)
+
+            if iteration_gemini > (2 - early_stopping_factor) * validation_gemini \
+                    or iteration_l1 < early_stopping_factor * validation_l1:
+                validation_l1 = iteration_l1
+                validation_gemini = iteration_gemini
+                patience = 0
+            else:
+                patience += 1
+            if np.isnan(gemini_score):
+                warnings.warn(f"Unfortunately, the GEMINI converged to nan, making the entire path unsucessful."
+                              f"Please report this error. Score and gradients are: {gemini_score}, {grads}")
+                patience = max_patience
+
+            i += 1
+
+        alphas.append(alpha)
+        n_features.append(clf._n_selected_features().item())
+        geminis.append(gemini_score.item())
+        group_lasso_penalties.append(clf._group_lasso_penalty())
+
+        if clf.verbose:
+            print(f"Finished after {i} iterations. Current iteration score is {iteration_gemini - iteration_l1}. "
+                  f"Current GEMINI score is {gemini_score}. Number of features is"
+                  f" {clf._n_selected_features().item()}")
+
+        alpha *= alpha_multiplier
+        if gemini_score >= best_gemini:
+            best_gemini = gemini_score
+            if clf.verbose:
+                print("Best GEMINI score so far, saving it.")
+
+        if gemini_score >= keep_threshold * best_gemini:
+            best_weights = [w.copy() for w in weights]
+            if clf.verbose:
+                print(f"This is definitely the best score so far within threshold: {gemini_score}, {best_gemini}")
+
+    return best_weights, geminis, group_lasso_penalties, alphas, n_features
+
 
 class _SparseMLPGEMINI(_MLPGEMINI, ABC):
     """ This is the BaseSparseGEMINI template to derive to create a Sparse GEMINI MLP clustering model.
     When deriving, the only methods to adapt is the _compute_gemini methods which
     should be able to return the gradient with respect to the conditional distribution p(y|x).
 
     On top of the vanilla MLP GEMINI model, this variation brings a skip connection from the data to the cluster
@@ -34,17 +161,17 @@
 
     Parameters
     ----------
     n_clusters : int, default=3
         The maximum number of clusters to form as well as the number of output neurons in the neural network.
 
     groups: list of arrays of various shapes, default=None
-        if groups is set, it must describe a partition of the indices of variables. This will be used for performing
-        variable selection with groups of features considered to represent one variables. This option can typically be used
-        for one-hot-encoded variables.
+        If groups is set, it must describe a partition of the indices of variables. This will be used for performing
+        variable selection with groups of features considered to represent one variables. This option can typically be
+        used for one-hot-encoded variables.
 
     max_iter: int, default=1000
         Maximum number of epochs to perform gradient descent in a single run.
 
     learning_rate: float, default=1e-3
         Initial learning rate used. It controls the step-size in updating the weights.
 
@@ -59,14 +186,17 @@
 
     alpha: float, default=1e-2
         The weight of the group-lasso penalty in the optimisation scheme.
 
     M: float, default=10 The hierarchy coefficient that controls the relative strength between the group-lasso
         penalty of the skip connection and the sparsity of the first layer of the MLP.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -94,21 +224,22 @@
     _parameter_constraints: dict = {
         **_MLPGEMINI._parameter_constraints,
         "M": [Interval(Real, 0, np.inf, closed="left")],
         "lambda_": [Interval(Real, 0, np.inf, closed="neither")],
     }
 
     def __init__(self, n_clusters=3, groups=None, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, M=10,
-                 alpha=1e-2, solver="adam", verbose=False, random_state=None):
+                 alpha=1e-2, solver="adam", batch_size=None, verbose=False, random_state=None):
         super().__init__(
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             n_hidden_dim=n_hidden_dim,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.M = M
         self.alpha = alpha
         self.groups = groups
 
@@ -164,14 +295,25 @@
 
         np.copyto(self.W_skip_, new_W_skip)
         np.copyto(self.W1_, new_W1)
 
     def _n_selected_features(self):
         return (np.linalg.norm(self.W_skip_, axis=1, ord=2) != 0).sum()
 
+    def get_selection(self):
+        """
+        Retrieves the indices of features that were selected by the model.
+
+        Returns
+        -------
+        ind: ndarray
+            The indices of the selected features.
+        """
+        return np.nonzero(np.linalg.norm(self.W_skip_, axis=1, ord=2))[0]
+
     def _group_lasso_penalty(self):
         return np.linalg.norm(self.W_skip_, axis=1, ord=2).sum()
 
     def path(self, X, alpha_multiplier=1.05, min_features=2, keep_threshold=0.9, restore_best_weights=True,
              early_stopping_factor=0.99, max_patience=10):
         """
         Unfold the progressive geometric increase of the penalty weight starting from the initial alpha until
@@ -201,123 +343,27 @@
         max_patience:
             The maximum number of iterations to wait without any improvements in either the gemclus score or the
             group-lasso penalty before stopping the current step.
 
         Returns
         -------
         best_weights: list of ndarray of various shapes of length 5
-            The list containing the best weights during the path. Sequentially: W1_, W2_, W_skip_, b1_, b2_
+            The list containing the best weights during the path. Sequentially: `W1_`, `W2_`, `W_skip_`, `b1_`, `b2_`
         geminis: list of float of length T
             The history of the gemclus scores as the penalty alpha was increased.
         group_penalties: list of float of length T
             The history of the group-lasso penalties
         alphas: list of float of length T
             The history of the penalty alphas during the path.
         n_features: list of float of length T
             The number of features that were selected at step t.
         """
-        self._validate_data(X)
-        check_groups(self.groups, X.shape[1])
-        if alpha_multiplier <= 1:
-            warnings.warn(f"The alpha multiplier is lower or equal to 1. This will not increase alpha during the path. "
-                          f"Setting it again to default parameters: 1.05")
-            alpha_multiplier = 1.05
-        if keep_threshold < 0 or keep_threshold > 1:
-            warnings.warn(f"The threshold to keep the best solution is outside [0,1]: {keep_threshold}, setting it "
-                          f"to default: 0.9")
-            keep_threshold = 0.9
-        if min_features <= 0:
-            warnings.warn(f"The min_features to stop the path iterations is below 0 which implies infinite loop. "
-                          f"Setting it to default: 2")
-            min_features = 2
-        elif min_features >= X.shape[1]:
-            warnings.warn(f"The min_features param is greater or equal to the number of features. This implies that "
-                          f"no path will be performed. The method is equivalent to `fit`.")
-
-        # Start by fitting the model using all features and without regularisation
-        alpha = self.alpha
-        self.set_params(alpha=0)
-
-        if self.verbose:
-            print("Starting initial training with alpha = 0")
-        self.fit(X)
-        best_gemini = self.score(X)
-        weights = self._get_weights()
-        best_weights = [w.copy() for w in weights]
-
-        if self.verbose:
-            print(f"Finished initial training. GEMINI = {best_gemini}")
-
-        kernel = self._compute_affinity(X)
-
-        alphas = [0]
-        n_features = [X.shape[1]]
-        geminis = [best_gemini]
-        group_lasso_penalties = [self._group_lasso_penalty()]
-
-        # Re-initialise the optimiser to SGD with 0.9 momentum (default option)
-        self.optimiser_ = SGDOptimizer(weights, self.learning_rate)
-
-        while self._n_selected_features() > min_features:
-            self.alpha = alpha
-
-            # Compute the validation scores at the beginning of this step of the path
-            validation_gemini = self.score(X)
-            validation_l1 = self._group_lasso_penalty() * self.alpha
-
-            if self.verbose:
-                print(f"Starting new iteration with: alpha = {self.alpha}. Validation score is {validation_gemini}")
-
-            gemini_score = np.array([validation_gemini])
-            patience = 0
-            i = 0
-            while i < self.max_iter and patience < max_patience:
-                y_pred = self._infer(X)
-                gemini_score, grads = self._compute_gemini(y_pred, kernel, return_grad=True)
-                iteration_gemini = gemini_score
-                iteration_l1 = self._group_lasso_penalty() * self.alpha
-
-                if iteration_gemini > (2 - early_stopping_factor) * validation_gemini \
-                        or iteration_l1 < early_stopping_factor * validation_l1:
-                    validation_l1 = iteration_l1
-                    validation_gemini = iteration_gemini
-                    patience = 0
-                else:
-                    patience += 1
-                if np.isnan(gemini_score):
-                    warnings.warn(f"Unfortunately, the GEMINI converged to nan, making the entire path unsucessful."
-                                  f"Please report this error. Score and gradients are: {gemini_score}, {grads}")
-                    patience = max_patience
-
-                if patience != max_patience:
-                    grads = self._compute_grads(X, y_pred, grads)
-                    self._update_weights(weights, grads)
-
-                i += 1
-
-            alphas.append(alpha)
-            n_features.append(self._n_selected_features().item())
-            geminis.append(gemini_score.item())
-            group_lasso_penalties.append(self._group_lasso_penalty())
-
-            if self.verbose:
-                print(f"Finished after {i} iterations. Current iteration score is {iteration_gemini - iteration_l1}. "
-                      f"Current GEMINI score is {gemini_score}. Number of features is"
-                      f" {self._n_selected_features().item()}")
-
-            alpha *= alpha_multiplier
-            if gemini_score >= best_gemini:
-                best_gemini = gemini_score
-                if self.verbose:
-                    print("Best GEMINI score so far, saving it.")
-
-            if gemini_score >= keep_threshold * best_gemini:
-                best_weights = [w.copy() for w in weights]
-                if self.verbose:
-                    print(f"This is definitely the best score so far within threshold: {gemini_score}, {best_gemini}")
+        best_weights, geminis, group_lasso_penalties, alphas, n_features = _path(self, X, alpha_multiplier,
+                                                                                 min_features, keep_threshold,
+                                                                                 early_stopping_factor, max_patience)
 
         if restore_best_weights:
             if self.verbose:
                 print("Restoring best weights")
             np.copyto(self.W1_, best_weights[0])
             np.copyto(self.W2_, best_weights[1])
             np.copyto(self.W_skip_, best_weights[2])
@@ -337,17 +383,17 @@
 
     Parameters
     ----------
     n_clusters : int, default=3
         The maximum number of clusters to form as well as the number of output neurons in the neural network.
 
     groups: list of arrays of various shapes, default=None
-        if groups is set, it must describe a partition of the indices of variables. This will be used for performing
-        variable selection with groups of features considered to represent one variables. This option can typically be used
-        for one-hot-encoded variables.
+        If groups is set, it must describe a partition of the indices of variables. This will be used for performing
+        variable selection with groups of features considered to represent one variables. This option can typically be
+        used for one-hot-encoded variables.
 
     max_iter: int, default=1000
         Maximum number of epochs to perform gradient descent in a single run.
 
     learning_rate: float, default=1e-3
         Initial learning rate used. It controls the step-size in updating the weights.
 
@@ -356,14 +402,17 @@
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
     alpha: float, default=1e-2
         The weight of the group-lasso penalty in the optimisation scheme.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -382,21 +431,22 @@
     """
     _parameter_constraints: dict = {
         **_LinearGEMINI._parameter_constraints,
         "M": [Interval(Real, 0, np.inf, closed="left")],
         "lambda_": [Interval(Real, 0, np.inf, closed="neither")],
     }
 
-    def __init__(self, n_clusters=3, groups=None, max_iter=1000, learning_rate=1e-3,
-                 alpha=1e-2, solver="adam", verbose=False, random_state=None):
+    def __init__(self, n_clusters=3, groups=None, max_iter=1000, learning_rate=1e-3, alpha=1e-2, batch_size=None,
+                 solver="adam", verbose=False, random_state=None):
         super().__init__(
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.alpha = alpha
         self.groups = groups
 
     def _update_weights(self, weights, gradients):
@@ -411,14 +461,25 @@
             new_W = group_linear_prox_grad(self.groups, self.W_, self.alpha * self.optimiser_.learning_rate)
 
         np.copyto(self.W_, new_W)
 
     def _n_selected_features(self):
         return (np.linalg.norm(self.W_, axis=1, ord=2) != 0).sum()
 
+    def get_selection(self):
+        """
+        Retrieves the indices of features that were selected by the model.
+
+        Returns
+        -------
+        ind: ndarray
+            The indices of the selected features.
+        """
+        return np.nonzero(np.linalg.norm(self.W_, axis=1, ord=2))
+
     def _group_lasso_penalty(self):
         return np.linalg.norm(self.W_, axis=1, ord=2).sum()
 
     def path(self, X, alpha_multiplier=1.05, min_features=2, keep_threshold=0.9, restore_best_weights=True,
              early_stopping_factor=0.99, max_patience=10):
         """
         Unfold the progressive geometric increase of the penalty weight starting from the initial alpha until
@@ -448,124 +509,27 @@
         max_patience:
             The maximum number of iterations to wait without any improvements in either the gemclus score or the
             group-lasso penalty before stopping the current step.
 
         Returns
         -------
         best_weights: list of ndarray of various shapes of length 5
-            The list containing the best weights during the path. Sequentially: W1_, W2_, W_skip_, b1_, b2_
+            The list containing the best weights during the path. Sequentially: `W_`, `b_`
         geminis: list of float of length T
             The history of the gemclus scores as the penalty alpha was increased.
         group_penalties: list of float of length T
             The history of the group-lasso penalties
         alphas: list of float of length T
             The history of the penalty alphas during the path.
         n_features: list of float of length T
             The number of features that were selected at step t.
         """
-        self._validate_data(X)
-        check_groups(self.groups, X.shape[1])
-
-        if alpha_multiplier <= 1:
-            warnings.warn(f"The alpha multiplier is lower or equal to 1. This will not increase alpha during the path. "
-                          f"Setting it again to default parameters: 1.05")
-            alpha_multiplier = 1.05
-        if keep_threshold < 0 or keep_threshold > 1:
-            warnings.warn(f"The threshold to keep the best solution is outside [0,1]: {keep_threshold}, setting it "
-                          f"to default: 0.9")
-            keep_threshold = 0.9
-        if min_features <= 0:
-            warnings.warn(f"The min_features to stop the path iterations is below 0 which implies infinite loop. "
-                          f"Setting it to default: 2")
-            min_features = 2
-        elif min_features >= X.shape[1]:
-            warnings.warn(f"The min_features param is greater or equal to the number of features. This implies that "
-                          f"no path will be performed. The method is equivalent to `fit`.")
-
-        # Start by fitting the model using all features and without regularisation
-        alpha = self.alpha
-        self.set_params(alpha=0)
-
-        if self.verbose:
-            print("Starting initial training with alpha = 0")
-        self.fit(X)
-        best_gemini = self.score(X)
-        weights = self._get_weights()
-        best_weights = [w.copy() for w in weights]
-
-        if self.verbose:
-            print(f"Finished initial training. GEMINI = {best_gemini}")
-
-        kernel = self._compute_affinity(X)
-
-        alphas = [0]
-        n_features = [X.shape[1]]
-        geminis = [best_gemini]
-        group_lasso_penalties = [self._group_lasso_penalty()]
-
-        # Re-initialise the optimiser to SGD with 0.9 momentum (default option)
-        self.optimiser_ = SGDOptimizer(weights, self.learning_rate)
-
-        while self._n_selected_features() > min_features:
-            self.alpha = alpha
-
-            # Compute the validation scores at the beginning of this step of the path
-            validation_gemini = self.score(X)
-            validation_l1 = self._group_lasso_penalty() * self.alpha
-
-            if self.verbose:
-                print(f"Starting new iteration with: alpha = {self.alpha}. Validation score is {validation_gemini}")
-
-            gemini_score = np.array([validation_gemini])
-            patience = 0
-            i = 0
-            while i < self.max_iter and patience < max_patience:
-                y_pred = self._infer(X)
-                gemini_score, grads = self._compute_gemini(y_pred, kernel, return_grad=True)
-                iteration_gemini = gemini_score
-                iteration_l1 = self._group_lasso_penalty() * self.alpha
-
-                if iteration_gemini > (2 - early_stopping_factor) * validation_gemini \
-                        or iteration_l1 < early_stopping_factor * validation_l1:
-                    validation_l1 = iteration_l1
-                    validation_gemini = iteration_gemini
-                    patience = 0
-                else:
-                    patience += 1
-                if np.isnan(gemini_score):
-                    warnings.warn(f"Unfortunately, the GEMINI converged to nan, making the entire path unsucessful."
-                                  f"Please report this error. Score and gradients are: {gemini_score}, {grads}")
-                    patience = max_patience
-
-                if patience != max_patience:
-                    grads = self._compute_grads(X, y_pred, grads)
-                    self._update_weights(weights, grads)
-
-                i += 1
-
-            alphas.append(alpha)
-            n_features.append(self._n_selected_features().item())
-            geminis.append(gemini_score.item())
-            group_lasso_penalties.append(self._group_lasso_penalty())
-
-            if self.verbose:
-                print(f"Finished after {i} iterations. Current iteration score is {iteration_gemini - iteration_l1}. "
-                      f"Current GEMINI score is {gemini_score}. Number of features is"
-                      f" {self._n_selected_features().item()}")
-
-            alpha *= alpha_multiplier
-            if gemini_score >= best_gemini:
-                best_gemini = gemini_score
-                if self.verbose:
-                    print("Best GEMINI score so far, saving it.")
-
-            if gemini_score >= keep_threshold * best_gemini:
-                best_weights = [w.copy() for w in weights]
-                if self.verbose:
-                    print(f"This is definitely the best score so far within threshold: {gemini_score}, {best_gemini}")
+        best_weights, geminis, group_lasso_penalties, alphas, n_features = _path(self, X, alpha_multiplier,
+                                                                                 min_features, keep_threshold,
+                                                                                 early_stopping_factor, max_patience)
 
         if restore_best_weights:
             if self.verbose:
                 print("Restoring best weights")
             np.copyto(self.W_, best_weights[0])
             np.copyto(self.b_, best_weights[1])
```

### Comparing `gemclus-0.0.1/gemclus/sparse/_linear_sparse.py` & `gemclus-0.0.2/gemclus/sparse/_linear_sparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..sparse._base_sparse import _SparseLinearGEMINI
 from .._base_gemini import _BaseMMD
+from ..sparse._base_sparse import _SparseLinearGEMINI
 
 
 class SparseLinearMMD(_SparseLinearGEMINI, _BaseMMD):
     """ This is the Sparse version of the LinearMMD clustering model.
 
     On top of the vanilla Linear GEMINI model, this variation brings a group-lasso penalty constraint to ensure
     feature selection via a proximal gradient during training.
@@ -11,16 +11,16 @@
     Parameters
     ----------
     n_clusters : int, default=3
         The maximum number of clusters to form as well as the number of output neurons in the neural network.
 
     groups: list of arrays of various shapes, default=None
         if groups is set, it must describe a partition of the indices of variables. This will be used for performing
-        variable selection with groups of features considered to represent one variables. This option can typically be used
-        for one-hot-encoded variables.
+        variable selection with groups of features considered to represent one variables. This option can typically be
+        used for one-hot-encoded variables.
         
     max_iter: int, default=1000
         Maximum number of epochs to perform gradient descent in a single run.
 
     learning_rate: float, default=1e-3
         Initial learning rate used. It controls the step-size in updating the weights.
 
@@ -37,14 +37,17 @@
 
         - 'sgd' refers to stochastic gradient descent.
         - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
 
     alpha: float, default=1e-2
         The weight of the group-lasso penalty in the optimisation scheme.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -92,28 +95,30 @@
     """
     _parameter_constraints: dict = {
         **_SparseLinearGEMINI._parameter_constraints,
         **_BaseMMD._parameter_constraints,
     }
 
     def __init__(self, n_clusters=3, groups=None, max_iter=1000, learning_rate=1e-3, kernel="linear", ovo=False,
-                 alpha=1e-2, solver="adam", verbose=False, random_state=None):
+                 alpha=1e-2, solver="adam", batch_size=None, verbose=False, random_state=None):
         _SparseLinearGEMINI.__init__(self,
                                      n_clusters=n_clusters,
                                      groups=groups,
                                      max_iter=max_iter,
                                      learning_rate=learning_rate,
                                      solver=solver,
+                                     batch_size=batch_size,
                                      verbose=verbose,
                                      random_state=random_state,
                                      alpha=alpha
                                      )
         _BaseMMD.__init__(self,
                           n_clusters=n_clusters,
                           max_iter=max_iter,
                           learning_rate=learning_rate,
                           solver=solver,
                           kernel=kernel,
                           ovo=ovo,
+                          batch_size=batch_size,
                           verbose=verbose,
                           random_state=random_state,
-                          )
+                          )
```

### Comparing `gemclus-0.0.1/gemclus/sparse/_mlp_sparse.py` & `gemclus-0.0.2/gemclus/sparse/_mlp_sparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..sparse._base_sparse import _SparseMLPGEMINI
 from .._base_gemini import _BaseMMD
+from ..sparse._base_sparse import _SparseMLPGEMINI
 
 
 class SparseMLPMMD(_SparseMLPGEMINI, _BaseMMD):
     """ This is the Sparse Version of the MLP MMD model.
 
     On top of the vanilla MLP GEMINI model, this variation brings a skip connection from the data to the cluster
     output. This skip connection ensures a sparsity constraint through a group-lasso penalty and a proximal gradient
@@ -14,16 +14,16 @@
     Parameters
     ----------
     n_clusters : int, default=3
         The maximum number of clusters to form as well as the number of output neurons in the neural network.
 
     groups: list of arrays of various shapes, default=None
         if groups is set, it must describe a partition of the indices of variables. This will be used for performing
-        variable selection with groups of features considered to represent one variables. This option can typically be used
-        for one-hot-encoded variables.
+        variable selection with groups of features considered to represent one variables. This option can typically be
+        used for one-hot-encoded variables.
 
     max_iter: int, default=1000
         Maximum number of epochs to perform gradient descent in a single run.
 
     learning_rate: float, default=1e-3
         Initial learning rate used. It controls the step-size in updating the weights.
 
@@ -46,14 +46,17 @@
 
     alpha: float, default=1e-2
         The weight of the group-lasso penalty in the optimisation scheme.
 
     M: float, default=10 The hierarchy coefficient that controls the relative strength between the group-lasso
         penalty of the skip connection and the sparsity of the first layer of the MLP.
 
+    batch_size: int, default=None
+        The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
     verbose: bool, default=False
         Whether to print progress messages to stdout
 
     random_state: int, RandomState instance, default=None
         Determines random number generation for weights and bias initialisation.
         Pass an int for reproducible results across multiple function calls.
 
@@ -107,34 +110,35 @@
     >>> clf.score(X)
     1.7664211836410726
     """
     _parameter_constraints: dict = {
         **_SparseMLPGEMINI._parameter_constraints,
     }
 
-    def __init__(self, n_clusters=3, groups=None, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, kernel="linear", M=10,
-                 alpha=1e-2, ovo=False, solver="adam", verbose=False, random_state=None):
+    def __init__(self, n_clusters=3, groups=None, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, kernel="linear",
+                 M=10, batch_size=None, alpha=1e-2, ovo=False, solver="adam", verbose=False, random_state=None):
         _SparseMLPGEMINI.__init__(
             self,
             n_clusters=n_clusters,
             groups=groups,
             max_iter=max_iter,
             learning_rate=learning_rate,
             n_hidden_dim=n_hidden_dim,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
             M=M,
             alpha=alpha
         )
         _BaseMMD.__init__(
             self,
             n_clusters=n_clusters,
             max_iter=max_iter,
             learning_rate=learning_rate,
             kernel=kernel,
             ovo=ovo,
             solver=solver,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
         )
-
```

### Comparing `gemclus-0.0.1/gemclus/tests/test_default.py` & `gemclus-0.0.2/gemclus/tests/test_default.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import pytest
-
 from sklearn.datasets import load_iris
 from sklearn.utils.estimator_checks import check_estimator
+from sklearn.utils.estimator_checks import check_clustering
 
-from ..linear import LinearWasserstein, LinearMMD
+from ..linear import LinearWasserstein, LinearMMD, RIM
 from ..mlp import MLPMMD, MLPWasserstein
 from ..sparse import SparseMLPMMD, SparseLinearMMD
 
 
 @pytest.fixture
 def data():
     X, y = load_iris(return_X_y=True)
     return X
 
 
 @pytest.mark.parametrize(
     "clf",
-    [LinearMMD(), MLPMMD(), LinearWasserstein(), MLPWasserstein(), SparseLinearMMD(), SparseMLPMMD()]
+    [LinearMMD(), MLPMMD(), LinearWasserstein(), MLPWasserstein(), SparseLinearMMD(), SparseMLPMMD(), RIM()]
 )
 def test_default_clf_init(clf):
     assert clf.learning_rate == 1e-3
     assert clf.n_clusters == 3
     assert clf.max_iter == 1000
     assert clf.random_state is None
     assert clf.solver == "adam"
 
 
 @pytest.mark.parametrize(
     "clf",
-    [LinearMMD, LinearWasserstein]
+    [LinearMMD, LinearWasserstein, RIM]
 )
 def test_all_linear_attributes(clf, data):
     clf = clf(max_iter=1)
     clf.fit(data)
     assert hasattr(clf, 'W_')
     assert hasattr(clf, 'b_')
     assert hasattr(clf, 'optimiser_')
@@ -81,32 +81,45 @@
 
 @pytest.mark.parametrize(
     "clf",
     [LinearMMD(), MLPMMD(), SparseMLPMMD(), SparseLinearMMD()]
 )
 def test_default_mmd(clf):
     assert clf.kernel == "linear"
-    assert clf.ovo == False
+    assert not clf.ovo
 
 
 @pytest.mark.parametrize(
     "clf",
     [LinearWasserstein(), MLPWasserstein()]
 )
 def test_default_wasserstein(clf):
     assert clf.metric == "euclidean"
-    assert clf.ovo == False
+    assert not clf.ovo
 
 
 @pytest.mark.parametrize(
     "estimator",
-    [MLPMMD(), LinearMMD(), SparseMLPMMD(), SparseLinearMMD(), MLPWasserstein(), LinearWasserstein()]
+    [MLPMMD(max_iter=5), LinearMMD(max_iter=5), SparseMLPMMD(max_iter=5), SparseLinearMMD(max_iter=5),
+     MLPWasserstein(max_iter=5), LinearWasserstein(max_iter=5), RIM(max_iter=5)]
 )
 def test_all_estimators(estimator):
-    from sklearn.utils.estimator_checks import check_clustering
     check_iterator = check_estimator(estimator, generate_only=True)
     for clf, check in check_iterator:
         if check.func == check_clustering:
-            # The check clustering function tests if we output as much clusters as promised,
+            # The check clustering function tests if we output as many clusters as promised,
             # But since GEMINI may have fewer clusters, this test will never be satisfied
             continue
         check(clf)
+
+@pytest.mark.parametrize(
+    "estimator",
+    [MLPMMD, LinearMMD, SparseMLPMMD, SparseLinearMMD, MLPWasserstein, LinearWasserstein, RIM]
+)
+@pytest.mark.parametrize(
+    "batch_size",
+    [10,50,None]
+)
+def test_batch_size(estimator, batch_size, data):
+    clf = estimator(max_iter=5, batch_size=batch_size)
+    clf.fit(data)
+    assert hasattr(clf, "labels_")
```

### Comparing `gemclus-0.0.1/gemclus/tests/test_objectives.py` & `gemclus-0.0.2/gemclus/tests/test_objectives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import pytest
-from sklearn.datasets import make_blobs
 from sklearn.metrics import pairwise_distances, pairwise_kernels
 from sklearn.utils.extmath import softmax
 
 from .._gemini_grads import wasserstein_ova, wasserstein_ovo, mmd_ova, mmd_ovo
 from ..data import celeux_one
 
 wasserstein_objectives = [wasserstein_ova, wasserstein_ovo]
@@ -14,15 +13,15 @@
 @pytest.fixture
 def data():
     return celeux_one(n=50, random_state=0)
 
 
 @pytest.fixture
 def fake_data_pred():
-    X,y = celeux_one(n=50, random_state=0)
+    X, y = celeux_one(n=50, random_state=0)
     np.random.seed(0)
     y_logits = np.random.uniform(size=(50, 3))
     return X, y_logits
 
 
 @pytest.mark.parametrize(
     "objective, affinity_fct",
```

### Comparing `gemclus-0.0.1/gemclus/tests/test_path.py` & `gemclus-0.0.2/gemclus/tests/test_path.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import pytest
 import numpy as np
-
+import pytest
 from sklearn.datasets import make_blobs
+
 from ..sparse import SparseMLPMMD, SparseLinearMMD
 
 
 @pytest.fixture
 def data():
     np.random.seed(0)
     X, y = make_blobs(n_samples=100, centers=3, cluster_std=0.1, random_state=0)
@@ -39,14 +39,15 @@
     assert np.allclose(alphas, alphas_v2)
     assert np.allclose(n_features, n_features_v2)
 
     gemini_score = clf.score(data)
 
     assert gemini_score >= 0.9 * max(geminis)
 
+
 def test_weights_coherence(data):
     clf = SparseMLPMMD(random_state=0)
 
     best_weights, geminis, penalties, alphas, n_features = clf.path(data, restore_best_weights=False)
 
     assert n_features[-1] <= 2
     assert n_features[-1] == (np.linalg.norm(clf.W1_, ord=2, axis=1) != 0).sum()
@@ -134,7 +135,17 @@
 
     for i in range(len(best_weights_v1)):
         assert np.allclose(best_weights_v1[i], best_weights_v2[i])
 
     assert np.allclose(np.array(geminis_v1), np.array(geminis_v2))
     assert np.allclose(np.array(alphas_v1), np.array(alphas_v2))
     assert np.allclose(np.array(n_features_v1), np.array(n_features_v2))
+
+@pytest.mark.parametrize(
+    "clf_class",
+    [SparseMLPMMD, SparseLinearMMD]
+)
+def test_batch_path(clf_class, data):
+    clf = clf_class(batch_size=50, random_state=0, max_iter=100)
+
+    best_weights_v1, geminis_v1, penalties_v1, alphas_v1, n_features_v1 = clf.path(data, restore_best_weights=False,
+                                                                                   min_features=data.shape[1]-1)
```

### Comparing `gemclus-0.0.1/gemclus.egg-info/PKG-INFO` & `gemclus-0.0.2/gemclus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemclus
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for performing discriminative clustering with gemini-trained models
 Home-page: https://github.com/gemini-clustering
 Download-URL: https://github.com/gemini-clustering
 Maintainer: Louis Ohl
 Maintainer-email: louis.ohl@inria.fr
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
@@ -28,28 +28,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # GEMCLUS - A package for discriminative clustering using GEMINI
 
-The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual information (GEMINI).
+The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual
+information (GEMINI).
 The package was written to be a scikit-learn compatible extension.
 
 You can find the complete documentation of the package here: `Link to be announced`
 
 ## Installation
 
 Use the following instruction for installing the package:
 
 ```commandline
 pip install gemclus
 ```
 
 The library requires a couple scientific package to run:
+
 + NumPy
 + Scipy
 + POT
 + Scikit-learn
 
 ## Reference
```

### Comparing `gemclus-0.0.1/gemclus.egg-info/SOURCES.txt` & `gemclus-0.0.2/gemclus.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 gemclus/mlp/__init__.py
 gemclus/mlp/_mlp_geminis.py
 gemclus/sparse/__init__.py
 gemclus/sparse/_base_sparse.py
 gemclus/sparse/_linear_sparse.py
 gemclus/sparse/_mlp_sparse.py
 gemclus/tests/__init__.py
+gemclus/tests/test_data.py
 gemclus/tests/test_default.py
 gemclus/tests/test_objectives.py
 gemclus/tests/test_path.py
```

### Comparing `gemclus-0.0.1/setup.py` & `gemclus-0.0.2/setup.py`

 * *Files identical despite different names*

